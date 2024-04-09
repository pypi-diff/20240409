# Comparing `tmp/junifer-0.0.4.dev90.tar.gz` & `tmp/junifer-0.0.5.dev11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.4.dev90.tar", last modified: Wed Oct 18 09:16:46 2023, max compression
+gzip compressed data, was "junifer-0.0.5.dev11.tar", last modified: Tue Apr  9 11:53:24 2024, max compression
```

## Comparing `junifer-0.0.4.dev90.tar` & `junifer-0.0.5.dev11.tar`

### file list

```diff
@@ -1,389 +1,451 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.119799 junifer-0.0.4.dev90/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.099798 junifer-0.0.4.dev90/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22068 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.123798 junifer-0.0.4.dev90/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/182.enh
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/233.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/245.change
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/245.feature
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/247.doc
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/248.change
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/251.doc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/253.misc
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/254.feature
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/258.enh
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/259.enh
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/changes/newsfragments/261.misc
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14813 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.127799 junifer-0.0.4.dev90/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-18 09:16:45.000000 junifer-0.0.4.dev90/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    22716 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1106 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/afni/run_afni_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      501 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/res/run_conda.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24631 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.107798 junifer-0.0.4.dev90/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.107798 junifer-0.0.4.dev90/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.135799 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    48818 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/parcellations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13269 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31361 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10731 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/datalad_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.139799 junifer-0.0.4.dev90/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.111798 junifer-0.0.4.dev90/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.143799 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.147799 junifer-0.0.4.dev90/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21922 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/preprocess/tests/test_preprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35520 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21243 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.151799 junifer-0.0.4.dev90/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.131799 junifer-0.0.4.dev90/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6792 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-18 09:16:46.000000 junifer-0.0.4.dev90/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 09:16:46.159799 junifer-0.0.4.dev90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:16:46.155799 junifer-0.0.4.dev90/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-18 09:16:35.000000 junifer-0.0.4.dev90/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.788822 junifer-0.0.5.dev11/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.736822 junifer-0.0.5.dev11/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.736822 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.736822 junifer-0.0.5.dev11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-09 11:53:24.788822 junifer-0.0.5.dev11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.740822 junifer-0.0.5.dev11/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.724822 junifer-0.0.5.dev11/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.740822 junifer-0.0.5.dev11/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.740822 junifer-0.0.5.dev11/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.740822 junifer-0.0.5.dev11/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25488 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/changes/newsfragments/273.feature
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/extending/preprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.744822 junifer-0.0.5.dev11/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.748822 junifer-0.0.5.dev11/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26318 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.748822 junifer-0.0.5.dev11/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.748822 junifer-0.0.5.dev11/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/yamls/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.748822 junifer-0.0.5.dev11/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.748822 junifer-0.0.5.dev11/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/queue_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/htcondor_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/queue_context_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/queue_context/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/queue_context/tests/test_htcondor_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/afni/run_afni_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/res/ants/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/ants/ResampleImage
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/ants/antsApplyTransforms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/ants/antsApplyTransformsToPoints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/ants/run_ants_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/res/fsl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/fsl/applywarp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/fsl/flirt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/fsl/img2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/fsl/run_fsl_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/fsl/std2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/run_conda.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/run_conda.zsh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/run_venv.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/res/run_venv.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.752822 junifer-0.0.5.dev11/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17215 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.756822 junifer-0.0.5.dev11/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.728822 junifer-0.0.5.dev11/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.760822 junifer-0.0.5.dev11/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.728822 junifer-0.0.5.dev11/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.760822 junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    23473 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65220 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/template_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.760822 junifer-0.0.5.dev11/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/tests/test_template_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/dmcc13_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_dmcc13_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.764822 junifer-0.0.5.dev11/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.728822 junifer-0.0.5.dev11/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 11:53:20.000000 junifer-0.0.5.dev11/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-04-09 11:53:20.000000 junifer-0.0.5.dev11/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 11:53:20.000000 junifer-0.0.5.dev11/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-09 11:53:20.000000 junifer-0.0.5.dev11/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-09 11:53:20.000000 junifer-0.0.5.dev11/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/markers/complexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/sample_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.768822 junifer-0.0.5.dev11/junifer/markers/complexity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_sample_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/complexity/weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.772822 junifer-0.0.5.dev11/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/_afni_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/_junifer_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.772822 junifer-0.0.5.dev11/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.772822 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.772822 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.772822 junifer-0.0.5.dev11/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/_afni_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/_junifer_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.776822 junifer-0.0.5.dev11/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/ants/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/ants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/ants/ants_apply_transforms_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/ants/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/bold_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/fsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/fsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/fsl/apply_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/fsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/fsl/tests/test_apply_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/tests/test_bold_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/tests/test_preprocess_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/warping/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/warping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/warping/_ants_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/warping/_fsl_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/warping/space_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/preprocess/warping/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/preprocess/warping/tests/test_space_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.780822 junifer-0.0.5.dev11/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.784822 junifer-0.0.5.dev11/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.788822 junifer-0.0.5.dev11/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 11:53:24.000000 junifer-0.0.5.dev11/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:53:24.788822 junifer-0.0.5.dev11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:53:24.788822 junifer-0.0.5.dev11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_dmcc13_benchmark_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-09 11:53:19.000000 junifer-0.0.5.dev11/tox.ini
```

### Comparing `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.5.dev11/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.github/workflows/ci-docs.yml` & `junifer-0.0.5.dev11/.github/workflows/ci-docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - '.github/workflows/**'
 jobs:
   run-tests:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11', '3.12']
     steps:
       - run: 'echo "No build required"'
       - name: Create mock coverage.xml file
         run: |
           mkdir docs
           touch docs/conf.py
           echo '<?xml version="1.0" ?>' > coverage.xml
@@ -36,15 +36,16 @@
           echo '<line number="7" hits="1"/>' >> coverage.xml
           echo '</lines>' >> coverage.xml
           echo '</class>' >> coverage.xml
           echo '</classes>' >> coverage.xml
           echo '</package>' >> coverage.xml
           echo '</packages>' >> coverage.xml
           echo '</coverage>' >> coverage.xml
-        if: matrix.python-version == 3.10
+        if: matrix.python-version == 3.11
       - name: Upload mock coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
-          fail_ci_if_error: true
+          # Allow coverage upload failure
+          fail_ci_if_error: false
           flags: docs
-        if: success() && matrix.python-version == 3.10
+        if: success() && matrix.python-version == 3.11
```

### Comparing `junifer-0.0.4.dev90/.github/workflows/docs-preview.yml` & `junifer-0.0.5.dev11/.github/workflows/docs-preview.yml`

 * *Files 13% similar despite different names*

```diff
@@ -16,38 +16,52 @@
 concurrency: preview-${{ github.ref }}
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
         submodules: true
-    - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.10'
+        python-version: '3.11'
     - name: Check for sudo
       shell: bash
       run: |
         if type sudo >/dev/null 2>&1; then SUDO="sudo"; else SUDO=""; fi
         echo "SUDO=$SUDO" >> $GITHUB_ENV
     - name: Install dependencies
       run: |
         $SUDO bash -c "$(curl -fsSL http://neuro.debian.net/_files/neurodebian-travis.sh)"
         $SUDO apt-get update -qq
         $SUDO apt-get install git-annex-standalone
         python -m pip install --upgrade pip setuptools wheel
-        python -m pip install -e .[docs]
+        python -m pip install -e ".[docs,neurokit2]"
     - name: Configure git for datalad
       run: |
         git config --global user.email "runner@github.com"
         git config --global user.name "GITHUB CI Runner"
+    - name: Install ANTs
+      run: |
+        echo "++ Add universe repo"
+        sudo add-apt-repository -y universe
+
+        echo "++ Update package manager info"
+        sudo apt-get update -qq
+
+        echo "++ Downloading ANTs"
+        curl -fsSL -o ants.zip https://github.com/ANTsX/ANTs/releases/download/v2.5.1/ants-2.5.1-ubuntu-22.04-X64-gcc.zip
+        unzip ants.zip -d /opt
+        mv /opt/ants-2.5.1/bin/* /opt/ants-2.5.1
+        rm ants.zip
+        echo "/opt/ants-2.5.1" >> $GITHUB_PATH
     - name: Test build docs
       run: |
         BUILDDIR=_build/main make -C docs/ local
     - name: Deploy preview
       if: github.event_name == 'pull_request'
       uses: rossjrw/pr-preview-action@v1
       with:
```

### Comparing `junifer-0.0.4.dev90/.github/workflows/docs.yml` & `junifer-0.0.5.dev11/.github/workflows/docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -10,44 +10,58 @@
       - v*
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         # require all of history to see all tagged versions' docs
         fetch-depth: 0
         submodules: true
-    - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.10'
+        python-version: '3.11'
     - name: Check for sudo
       shell: bash
       run: |
         if type sudo >/dev/null 2>&1; then SUDO="sudo"; else SUDO=""; fi
         echo "SUDO=$SUDO" >> $GITHUB_ENV
     - name: Install dependencies
       run: |
         $SUDO bash -c "$(curl -fsSL http://neuro.debian.net/_files/neurodebian-travis.sh)"
         $SUDO apt-get update -qq
         $SUDO apt-get install git-annex-standalone
         python -m pip install --upgrade pip setuptools wheel
-        python -m pip install -e .[docs]
+        python -m pip install -e ".[docs,neurokit2]"
         python -m pip install git+https://github.com/dls-controls/sphinx-multiversion@only-arg
     - name: Configure git for datalad
       run: |
         git config --global user.email "runner@github.com"
         git config --global user.name "GITHUB CI Runner"
+    - name: Install ANTs
+      run: |
+        echo "++ Add universe repo"
+        sudo add-apt-repository -y universe
+
+        echo "++ Update package manager info"
+        sudo apt-get update -qq
+
+        echo "++ Downloading ANTs"
+        curl -fsSL -o ants.zip https://github.com/ANTsX/ANTs/releases/download/v2.5.1/ants-2.5.1-ubuntu-22.04-X64-gcc.zip
+        unzip ants.zip -d /opt
+        mv /opt/ants-2.5.1/bin/* /opt/ants-2.5.1
+        rm ants.zip
+        echo "/opt/ants-2.5.1" >> $GITHUB_PATH
     - name: Checkout gh-pages
       # As we already did a deploy of gh-pages above, it is guaranteed to be there
       # so check it out so we can selectively build docs below
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
           ref: gh-pages
           path: docs/_build
     - name: Build docs
       # Use the args we normally pass to sphinx-build, but run sphinx-multiversion
       run: |
         make -C docs/ html
```

### Comparing `junifer-0.0.4.dev90/.github/workflows/lint.yml` & `junifer-0.0.5.dev11/.github/workflows/lint.yml`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   - push
   - pull_request
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Install Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox "ruff>=0.1.0"
       - name: Run ruff
```

### Comparing `junifer-0.0.4.dev90/.github/workflows/pypi.yml` & `junifer-0.0.5.dev11/.github/workflows/pypi.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,30 +7,25 @@
       - 'v*'
 jobs:
   build-n-publish:
     name: Build and publish to PyPI
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
         submodules: true
-    - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+    - name: Set up Python 3.11
+      uses: actions/setup-python@v5
       with:
-        python-version: '3.10'
+        python-version: '3.11'
     - name: Install build
       run:
         pip install build
     - name: Build a binary wheel and a source tarball
       run:
         python -m build --sdist --wheel --outdir dist/ .
-    # - name: Publish distribution 📦 to Test PyPI
-    #   uses: pypa/gh-action-pypi-publish@master
-    #   with:
-    #     password: ${{ secrets.testpypi_token }}
-    #     repository_url: https://test.pypi.org/legacy/
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.pypi_token }}
```

### Comparing `junifer-0.0.4.dev90/.gitignore` & `junifer-0.0.5.dev11/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/.pre-commit-config.yaml` & `junifer-0.0.5.dev11/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,25 @@
       - id: check-yaml
       - id: check-toml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.15
+    rev: v0.16
     hooks:
       - id: validate-pyproject
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.1.1
     hooks:
       - id: black
         exclude: ^(docs/|examples/|tools/)
         args: [--check]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.0
+    rev: v0.1.15
     hooks:
       - id: ruff
         types_or: [python, jupyter]
         exclude: ^(__init__.py)
         args: [--output-format, grouped, --show-fixes]
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
```

### Comparing `junifer-0.0.4.dev90/LICENSE.md` & `junifer-0.0.5.dev11/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/PKG-INFO` & `junifer-0.0.5.dev11/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev90
+Version: 0.0.5.dev11
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
-Project-URL: homepage, https://juaml.github.io/junifer
-Project-URL: documentation, https://juaml.github.io/junifer
-Project-URL: repository, https://github.com/juaml/junifer
+Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
+Project-URL: Documentation, https://juaml.github.io/junifer
+Project-URL: Homepage, https://juaml.github.io/junifer
+Project-URL: Source, https://github.com/juaml/junifer
 Keywords: neuroimaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 Requires-Dist: click<8.2,>=8.1.3
 Requires-Dist: numpy<1.27,>=1.24
+Requires-Dist: scipy<=1.11.4,>=1.9.0
 Requires-Dist: datalad<0.20,>=0.15.4
 Requires-Dist: pandas<2.2,>=1.4.0
 Requires-Dist: nibabel<5.11,>=3.2.0
-Requires-Dist: nilearn<=0.11.0,>=0.9.0
+Requires-Dist: nilearn<=0.10.2,>=0.9.0
 Requires-Dist: sqlalchemy<=2.1.0,>=1.4.27
 Requires-Dist: ruamel.yaml<0.18,>=0.17
+Requires-Dist: h5py>=3.10
+Requires-Dist: httpx[http2]==0.26.0
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: templateflow>=23.0.0
 Requires-Dist: importlib_metadata; python_version < "3.10"
-Requires-Dist: h5py<3.10,>=3.8.0
+Requires-Dist: looseversion==1.3.0; python_version >= "3.12"
+Provides-Extra: all
+Requires-Dist: bctpy==0.6.0; extra == "all"
+Requires-Dist: neurokit2>=0.1.7; extra == "all"
+Provides-Extra: bct
+Requires-Dist: bctpy==0.6.0; extra == "bct"
+Provides-Extra: onthefly
+Requires-Dist: bctpy==0.6.0; extra == "onthefly"
+Provides-Extra: neurokit2
+Requires-Dist: neurokit2>=0.1.7; extra == "neurokit2"
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: seaborn<0.13,>=0.11.2; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15.0,>=0.11.0; extra == "docs"
 Requires-Dist: furo<2023.10.0,>=2022.9.29; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: julearn<0.4,>=0.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton<0.5.3,>=0.5.1; extra == "docs"
 Requires-Dist: towncrier<23.7,>=22.12.0; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid<0.10,>=0.8.1; extra == "docs"
-Provides-Extra: onthefly
-Requires-Dist: bctpy==0.6.0; extra == "onthefly"
 
 ![Junifer logo](docs/images/junifer_logo.png "junifer logo")
 
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
@@ -62,14 +76,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8176570.svg)](https://doi.org/10.5281/zenodo.8176570)
+[![FAIR checklist badge](https://fairsoftwarechecklist.net/badge.svg)](https://fairsoftwarechecklist.net/v0.2?f=31&a=32113&i=32322&r=133)
 
 ## About
 
 `junifer` is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
 
@@ -88,15 +103,15 @@
   * `external`: Module for external libraries and tools.
   * `markers`: Markers module.
   * `onthefly`: Transformation components (on-the-fly) module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
-  * `utils`: Utilities module (e.g. logging)
+  * `utils`: Utilities module (e.g. logging).
 
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
@@ -104,14 +119,29 @@
 
 You can also install via `conda`, like so:
 
 ```
 conda install -c conda-forge junifer
 ```
 
+### Optional dependencies
+
+`junifer` supports a few optional dependencies to enable certain features. You can
+install them by specifying a comma separated list within square brackets, like so:
+
+```
+pip install "junifer[bct,dev]"
+```
+
+* `bct` installs [bctpy](https://github.com/aestrivex/bctpy) to enable use of `onthefly` module.
+* `neurokit2` installs [neurokit2](https://github.com/neuropsychology/NeuroKit) to enable use of [complexity markers](https://juaml.github.io/junifer/main/api/markers.html#module-junifer.markers.complexity).
+* `all` includes all of the above.
+* `dev` installs packages needed for development.
+* `docs` installs packages needed for building documentation.
+
 ## Citation
 
 If you use `junifer` in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project's [Zenodo URL](https://doi.org/10.5281/zenodo.8176569).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.4.dev90/README.md` & `junifer-0.0.5.dev11/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8176570.svg)](https://doi.org/10.5281/zenodo.8176570)
+[![FAIR checklist badge](https://fairsoftwarechecklist.net/badge.svg)](https://fairsoftwarechecklist.net/v0.2?f=31&a=32113&i=32322&r=133)
 
 ## About
 
 `junifer` is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
 
@@ -34,15 +35,15 @@
   * `external`: Module for external libraries and tools.
   * `markers`: Markers module.
   * `onthefly`: Transformation components (on-the-fly) module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
-  * `utils`: Utilities module (e.g. logging)
+  * `utils`: Utilities module (e.g. logging).
 
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
@@ -50,14 +51,29 @@
 
 You can also install via `conda`, like so:
 
 ```
 conda install -c conda-forge junifer
 ```
 
+### Optional dependencies
+
+`junifer` supports a few optional dependencies to enable certain features. You can
+install them by specifying a comma separated list within square brackets, like so:
+
+```
+pip install "junifer[bct,dev]"
+```
+
+* `bct` installs [bctpy](https://github.com/aestrivex/bctpy) to enable use of `onthefly` module.
+* `neurokit2` installs [neurokit2](https://github.com/neuropsychology/NeuroKit) to enable use of [complexity markers](https://juaml.github.io/junifer/main/api/markers.html#module-junifer.markers.complexity).
+* `all` includes all of the above.
+* `dev` installs packages needed for development.
+* `docs` installs packages needed for building documentation.
+
 ## Citation
 
 If you use `junifer` in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project's [Zenodo URL](https://doi.org/10.5281/zenodo.8176569).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.4.dev90/codecov.yml` & `junifer-0.0.5.dev11/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/conda-env.yml` & `junifer-0.0.5.dev11/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/Makefile` & `junifer-0.0.5.dev11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/_static/css/custom.css` & `junifer-0.0.5.dev11/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/_templates/versions.html` & `junifer-0.0.5.dev11/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/builtin.rst` & `junifer-0.0.5.dev11/docs/builtin.rst`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     the `junifer.configs` module.
 
     State: this should indicate the state of the dataset. Valid options are
     - Planned
     - In Progress
     - Done
 
-    Version added: If the status is "Done", the Junifer version in which the
+    Version added: If the status is "Done", the junifer version in which the
     dataset was added. Else, a link to the Github issue or pull request
     implementing the dataset. Links to github can be added by using the
     following syntax: :gh:`<issue number>`
 
 Available
 ~~~~~~~~~
 
@@ -118,26 +118,74 @@
    * - ENKI
      - ENKI dataset for Juseless
      - Restricted
      - ``junifer.configs.juseless``
      - :gh:`47`
 
 
+Preprocessor
+------------
+
+..
+    Provide a list of the Preprocessors that are implemented or planned.
+
+    State: this should indicate the state of the preprocessor. Valid options are
+    - Planned
+    - In Progress
+    - Done
+
+    Version added: If the status is "Done", the junifer version in which the
+    preprocessor was added. Else, a link to the Github issue or pull request
+    implementing the preprocessor. Links to github can be added by using the
+    following syntax: :gh:`<issue number>`
+
+Available
+~~~~~~~~~
+
+.. list-table::
+   :widths: auto
+   :header-rows: 1
+
+   * - Class
+     - Description
+     - State
+     - Version Added
+   * - :class:`.fMRIPrepConfoundRemover`
+     - Remove confounds from ``fMRIPrep``-ed data
+     - Done
+     - 0.0.1
+   * - :class:`.SpaceWarper`
+     - | Warp / transform data from one space to another
+       | (subject-native or other template spaces)
+     - Done
+     - 0.0.4
+   * - ``Smoothing``
+     - | Apply smoothing to data, particularly useful when dealing with
+       | ``fMRIPrep``-ed data
+     - In Progress
+     - :gh:`161`
+
+
+..
+   Planned
+   ~~~~~~~
+
+
 Marker
 ------
 
 ..
     Provide a list of the Markers that are implemented or planned.
 
     State: this should indicate the state of the marker. Valid options are
     - Planned
     - In Progress
     - Done
 
-    Version added: If the status is "Done", the Junifer version in which the
+    Version added: If the status is "Done", the junifer version in which the
     marker was added. Else, a link to the Github issue or pull request
     implementing the marker. Links to github can be added by using the
     following syntax: :gh:`<issue number>`
 
 Available
 ~~~~~~~~~
 
@@ -206,68 +254,97 @@
      - Done
      - 0.0.2
    * - :class:`.TemporalSNRSpheres`
      - | Calculate temporal signal-to-noise ratio using spheres placed on
        | coordinates
      - Done
      - 0.0.2
+   * - :class:`.HurstExponent`
+     - | Calculate Hurst exponent of a time series as found in
+       | `Peng et al. (1995) <https://doi.org/10.1063/1.166141>`_
+     - Done
+     - 0.0.4
+   * - :class:`.MultiscaleEntropyAUC`
+     - | Calculate AUC of multiscale entropy of a time series as found in
+       | `Costa et al. (2002) <https://doi.org/10.1103/PhysRevLett.89.068102>`_
+     - Done
+     - 0.0.4
+   * - :class:`.PermEntropy`
+     - | Calculate permutation entropy of a time series as found in
+       | `Bandt at al. (2002) <https://doi.org/10.1103/PhysRevLett.88.174102>`_
+     - Done
+     - 0.0.4
+   * - :class:`.RangeEntropy`
+     - | Calculate range entropy of a time series as found in
+       | `Omidvarnia et al. (2018) <https://doi.org/10.3390/e20120962>`_
+     - Done
+     - 0.0.4
+   * - :class:`.RangeEntropyAUC`
+     - | Calculate AUC of range entropy of a time series as found in
+       | `Omidvarnia et al. (2018) <https://doi.org/10.3390/e20120962>`_
+     - Done
+     - 0.0.4
+   * - :class:`.SampleEntropy`
+     - | Calculate sample entropy of a time series as found in
+       | `Richman et al. (2000) <https://doi.org/10.1152/ajpheart.2000.278.6.H2039>`_
+     - Done
+     - 0.0.4
 
 Planned
 ~~~~~~~
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Description
      - Reference
    * - Connectedness
      - Compute connectedness
      - :gh:`34`
-   * - Permutation entropy, Range entropy, Multiscale entropy and Hurst exponent
-     - | Calculate Permutation entropy, Range entropy, Multiscale entropy and
-       | Hurst exponent
-     - :gh:`61`
 
 Parcellation
 ------------
 
 ..
     Provide a list of the Parcellations that are implemented or planned.
 
-    Version added: The Junifer version in which the parcellation was added.
+    Version added: The junifer version in which the parcellation was added.
 
 Available
 ~~~~~~~~~
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Options
      - Keys
-     - Version added
+     - Template Spaces
+     - Version Added
      - Publication
    * - Schaefer
      - ``n_rois``, ``yeo_networks``
      - | ``Schaefer900x7``, ``Schaefer1000x7``, ``Schaefer100x17``,
        | ``Schaefer200x17``, ``Schaefer300x17``, ``Schaefer400x17``,
        | ``Schaefer500x17``, ``Schaefer600x17``, ``Schaefer700x17``,
        | ``Schaefer800x17``, ``Schaefer900x17``, ``Schaefer1000x17``
+     - ``MNI152NLin6Asym``
      - 0.0.1
      - | Schaefer, A., Kong, R., Gordon, E.M. et al.
        | Local-Global Parcellation of the Human Cerebral Cortex from
        | Intrinsic Functional Connectivity MRI
        | Cerebral Cortex, Volume 28(9), Pages 3095–3114 (2018).
        | https://doi.org/10.1093/cercor/bhx179
    * - SUIT
      - ``space``
      - ``SUITxMNI``, ``SUITxSUIT``
+     - ``SUIT``, ``MNI152Lin6Asym``
      - 0.0.1
      - | Diedrichsen, J.
        | A spatially unbiased atlas template of the human cerebellum.
        | NeuroImage, Volume 33(1), Pages 127–138 (2006).
        | https://doi.org/10.1016/j.neuroimage.2006.05.056
    * - Tian
      - ``scale``, ``space``, ``magneticfield``
@@ -275,32 +352,35 @@
        | ``TianxS2x3TxMNI6thgeneration``, ``TianxS2x7TxMNI6thgeneration``,
        | ``TianxS3x3TxMNI6thgeneration``, ``TianxS3x7TxMNI6thgeneration``,
        | ``TianxS4x3TxMNI6thgeneration``, ``TianxS4x7TxMNI6thgeneration``,
        | ``TianxS1x3TxMNInonlinear2009cAsym``,
        | ``TianxS2x3TxMNInonlinear2009cAsym``,
        | ``TianxS3x3TxMNInonlinear2009cAsym``,
        | ``TianxS4x3TxMNInonlinear2009cAsym``
+     - ``MNI152NLin6Asym``, ``MNI152NLin2009cAsym``
      - 0.0.1
      - | Tian, Y., Margulies, D.S., Breakspear, M. et al.
        | Topographic organization of the human subcortex
        | unveiled with functional connectivity gradients.
        | Nature Neuroscience, Volume 23, Pages 1421–1432 (2020).
        | https://doi.org/10.1038/s41593-020-00711-6
    * - AICHA
      - ``version``
      - ``AICHA_v1``, ``AICHA_v2``
+     - ``MNI152Lin6Asym``
      - 0.0.3
      - | Joliot, M., Jobard, G., Naveau, M. et al.
        | AICHA: An atlas of intrinsic connectivity of homotopic areas.
        | Journal of Neuroscience Methods, Volume 254, Pages 46-59 (2015).
        | https://doi.org/10.1016/j.jneumeth.2015.07.013
    * - Shen
      - ``year``, ``n_rois``
      - | ``Shen_2013_50``, ``Shen_2013_100``, ``Shen_2013_150``,
        | ``Shen_2015_268``, ``Shen_2019_368``
+     - ``MNI152NLin2009cAsym``
      - 0.0.3
      - | Shen, X., Tokoglu, F., Papademetris, X., Constable, R.T.
        | Groupwise whole-brain parcellation from resting-state fMRI data
        | for network node identification.
        | NeuroImage, Volume 82 (2013).
        | https://doi.org/10.1016/j.neuroimage.2013.05.081.
        | Finn, E.S., Shen, X., Scheinost, D., et al.
@@ -318,20 +398,31 @@
        | ``Yan400xYeo17``, ``Yan500xYeo17``, ``Yan600xYeo17``,
        | ``Yan700xYeo17``, ``Yan800xYeo17``, ``Yan900xYeo17``,
        | ``Yan1000xYeo17``,
        | ``Yan100xKong17``, ``Yan200xKong17``, ``Yan300xKong17``,
        | ``Yan400xKong17``, ``Yan500xKong17``, ``Yan600xKong17``,
        | ``Yan700xKong17``, ``Yan800xKong17``, ``Yan900xKong17``,
        | ``Yan1000xKong17``
+     - ``MNI152NLin6Asym``
      - 0.0.3
      - | Yan, X., Kong, R., Xue, A., et al.
        | Homotopic local-global parcellation of the human cerebral cortex from
        | resting-state functional connectivity.
        | NeuroImage, Volume 273 (2023).
        | https://doi.org/10.1016/j.neuroimage.2023.120010
+   * - Brainnetome
+     - ``threshold``
+     - ``Brainnetome_thr0``, ``Brainnetome_thr25``, ``Brainnetome_thr50``
+     - ``MNI152NLin6Asym``
+     - 0.0.4
+     - | Fan, L., Li, H., Zhuo, J., et al.
+       | The Human Brainnetome Atlas: A New Brain Atlas Based on Connectional
+       | Architecture
+       | Cerebral Cortex, Volume 26(8), Pages 3508–3526 (2016).
+       | https://doi.org/10.1093/cercor/bhw157
 
 
 Planned
 ~~~~~~~
 
 .. list-table::
    :widths: auto
@@ -388,26 +479,26 @@
 
 Coordinates
 -----------
 
 ..
     Provide a list of the Coordinates that are implemented or planned.
 
-    Version added: The Junifer version in which the parcellation was added.
+    Version added: The junifer version in which the parcellation was added.
 
 Available
 ~~~~~~~~~
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Keys
-     - Version added
+     - Version Added
      - Publication
    * - Cognitive action control
      - ``CogAC``
      - 0.0.1
      - | Cieslik, E.C., Mueller, V.I., Eickhoff, C.R., Langner, R.,
        | Eickhoff, S.B.
        | Three key regions for supervisory attentional control: Evidence from
@@ -544,14 +635,23 @@
      - ``Power2013``
      - 0.0.4
      - | Power, J. D., Schlaggar, B. L., Lessov-Schlaggar, C. N., &
        | Petersen, S. E.
        | Evidence for hubs in human functional brain networks.
        | Neuron, Volume 79(4), Pages 798–813 (2013).
        | https://doi.org/10.1016/j.neuron.2013.07.035
+   * - Autobiographical Memory from Spreng et al. (2009)
+     - ``AutobiographicalMemory``
+     - 0.0.4
+     - | Spreng, R. N., Mar, R. A., Kim, A. S. N.
+       | The Common Neural Basis of Autobiographical Memory, Prospection,
+       | Navigation, Theory of Mind, and the Default Mode: A Quantitative
+       | Meta-analysis.
+       | Journal of Cognitive Neuroscience, Volume 21(3), Pages 489–510 (2009).
+       | https://doi.org/10.1162/jocn.2008.21029
 
 
 Planned
 ~~~~~~~
 
 .. list-table::
    :widths: auto
@@ -575,65 +675,72 @@
 
 Mask
 ----
 
 ..
     Provide a list of the masks that are implemented or planned.
 
-    Version added: The Junifer version in which the mask was added.
+    Version added: The junifer version in which the mask was added.
 
 Available
 ~~~~~~~~~
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Keys
-     - Version added
+     - Template Space
+     - Version Added
      - Description - Publication
    * - Vickery-Patil (Gray Matter)
      - | ``GM_prob0.2``
+     - ``MNI152Lin6Asym``
      - 0.0.1
      - | Vickery, Sam, & Patil, Kaustubh. (2022).
        | Chimpanzee and Human Gray Matter Masks [Data set]. Zenodo.
        | https://doi.org/10.5281/zenodo.6463123
    * - Vickery-Patil (Cortex + Basal Ganglia)
      - | ``GM_prob0.2_cortex``
+     - ``MNI152Lin6Asym``
      - 0.0.1
      - | Vickery, Sam, & Patil, Kaustubh. (2022).
        | Chimpanzee and Human Gray Matter Masks [Data set]. Zenodo.
        | https://doi.org/10.5281/zenodo.6463123
-   * - Nilearn's MNI152 1mm-resolution mask
+   * - ``junifer``'s custom brain mask
      - | ``compute_brain_mask``
+     - Adapts to the target data
      - 0.0.2
-     - | Compute the whole-brain mask. This mask is calculated using
-       | MNI152 1mm-resolution template mask onto the target image.
-       | See :func:`nilearn.masking.compute_brain_mask`
-   * - Nilearn's mask computed from FMRI data
+     - | Compute the whole-brain, gray-matter or white-matter mask using
+       | the template and the resolution from the target image. The
+       | templates are obtained via ``templateflow``.
+   * - ``nilearn``'s mask computed from fMRI data
      - | ``compute_epi_mask``
+     - Adapts to the target data
      - 0.0.2
      - | Compute a brain mask from fMRI data. This is based on an heuristic
        | proposed by T.Nichols: find the least dense point of the histogram,
        | between fractions ``lower_cutoff`` and ``upper_cutoff`` of the total
        | image histogram. See :func:`nilearn.masking.compute_epi_mask`
-   * - Nilearn's background mask
+   * - ``nilearn``'s background mask
      - | ``compute_background_mask``
+     - Adapts to the target data
      - 0.0.2
      - | Compute a brain mask for the images by guessing the value of the
        | background from the border of the image.
        | See :func:`nilearn.masking.compute_background_mask`
-
-   * - Nilearn's ICBM152 template gray-matter mask
+   * - ``nilearn``'s ICBM152 template gray-matter mask
      - | ``fetch_icbm152_brain_gm_mask``
+     - ``MNI152NLin2009aAsym``
      - 0.0.2
      - | Compute a gray-matter mask from the asymmetrical ICBM152 2009 template,
        | release a.
        | See :func:`nilearn.datasets.fetch_icbm152_brain_gm_mask`
 
 
-Planned
-~~~~~~~
+..
+   Planned
+   ~~~~~~~
 
 ..
   helpful site for creating tables: https://rest-sphinx-memo.readthedocs.io/en/latest/ReST.html#tables
```

### Comparing `junifer-0.0.4.dev90/docs/changes/contributors.inc` & `junifer-0.0.5.dev11/docs/changes/contributors.inc`

 * *Files 12% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 .. _Synchon Mandal: https://github.com/synchon
 .. _Benjamin Poldrack: https://github.com/bpoldrack
 .. _Vera Komeyer: https://github.com/verakye
 .. _Xuan Li: https://github.com/xuanli-ac
 .. _Sami Hamdan: https://github.com/samihamdan
 .. _Nicolas Nieto: https://github.com/N-Nieto
 .. _Felix Hoffstaedter: https://github.com/FeHoff
+.. _Tobias Muganga: https://github.com/tomug
```

### Comparing `junifer-0.0.4.dev90/docs/conf.py` & `junifer-0.0.5.dev11/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import sys
 from pathlib import Path
 
+
 # Check if sphinx-multiversion is installed
 use_multiversion = False
 try:
     import sphinx_multiversion  # noqa: F401
     use_multiversion = True
 except ImportError:
     pass
@@ -41,15 +42,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",  # include documentation from docstrings
     "sphinx.ext.autosummary",  # generate autodoc summaries
     "sphinx.ext.doctest",  # test snippets in the documentation
-    "sphinx.ext.intersphinx",  # link to other projects’ documentation
+    "sphinx.ext.intersphinx",  # link to other projects` documentation
     "sphinx.ext.mathjax",  # math support for HTML outputs in Sphinx
     "sphinx_gallery.gen_gallery",  # HTML gallery of examples
     "numpydoc",  # support for NumPy style docstrings
     "gh_substitutions",  # custom GitHub substitutions
     "sphinx_copybutton",  # copy button for code blocks
     "sphinxcontrib.mermaid",  # mermaid support
 ]
@@ -78,14 +79,15 @@
     ("py:obj", "trimboth"),  # python 3.11 error
     ("py:obj", "tmean"),  # python 3.11 error
     ("py:obj", "subclass"),  # python 3.11 error
     ("py:class", "typing.Any"),  # python 3.11 error
     # ('py:class', 'numpy.typing.ArrayLike')
     ("py:obj", "sqlalchemy.engine.Engine"),  # ignore sqlalchemy
     ("py:class", "pipeline.Pipeline"),  # nilearn
+    ("py:obj", "neurokit2.*"),  # ignore neurokit2
 ]
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages. See the documentation for
 # a list of builtin themes.
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `junifer-0.0.4.dev90/docs/contribution.rst` & `junifer-0.0.5.dev11/docs/contribution.rst`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,16 @@
 
 To view the documentation, open ``docs/_build/html/index.html``.
 
 In case you remove some files or change their filenames, you can run into
 errors when using ``make local``. In this situation you can use ``make clean``
 to clean up the already build files and then re-run ``make local``.
 
+Also, we follow British English for the documentation.
+
 
 Writing Examples
 ----------------
 
 The format used for text is reST. Check the `sphinx reST reference`_ for more
 details. The examples are run and displayed in HTML format using
 `sphinx gallery`_. To add an example, just create a ``.py`` file that starts
```

### Comparing `junifer-0.0.4.dev90/docs/extending/coordinates.rst` & `junifer-0.0.5.dev11/docs/extending/coordinates.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,69 +2,71 @@
 
 .. _adding_coordinates:
 
 Adding Coordinates
 ==================
 
 Instead of using whole-brain parcellations to aggregate voxel-wise signals from
-MR images (as for example in the :class:`.ParcelAggregation` marker), junifer
+MR images (as for example in the :class:`.ParcelAggregation` marker), ``junifer``
 allows you to specify a set of coordinates around which to draw spheres to
 aggregate (for example using the :class:`.SphereAggregation` marker) the MR
 signals from individual voxels. Now, before you start specifying your own sets
-of coordinates, check the coordinates that junifer already has
+of coordinates, check the coordinates that ``junifer`` already has
 :ref:`built in <builtin>`. If you simply want to use a well known set of
-coordinates from the literature, there is a reasonable chance, that junifer
+coordinates from the literature, there is a reasonable chance, that ``junifer``
 provides them already.
 
 If you checked the in-built coordinates, and they are not there already (for
-example if you came up with your own set of coordinates), then junifer provides
-an easy way for you to register them using the :func:`.register_coordinates`
-function, so you can use your own set of coordinates within a junifer pipeline.
+example if you came up with your own set of coordinates), then ``junifer``
+provides an easy way for you to register them using the
+:func:`.register_coordinates` function, so you can use your own set of
+coordinates within a ``junifer`` pipeline.
 
-From the API reference, we can see that it has 3 positional arguments
-(``name``, ``coordinates``, and ``voi_names``) as well as one
+From the API reference, we can see that it has 4 positional arguments
+(``name``, ``coordinates``, ``voi_names`` and ``space``) as well as one
 optional keyword argument (``overwrite``).
 
 The ``name`` argument takes a string indicating the name you want to give to
 this set of coordinates. This ``name`` can be used to obtain and operate on a
-set of coordinates in junifer. For example, you can obtain your coordinates
+set of coordinates in ``junifer``. For example, you can obtain your coordinates
 after registration by providing ``name`` to :func:`.load_coordinates`. We could
 simply call it ``"my_set_of_coordinates"``, but likely you want a more
 descriptive and more informative name most of the time.
 
 The ``coordinates`` argument takes the actual coordinates as a 2-dimensional
 :class:`numpy.ndarray`. It contains one row for every location, and three
 columns (one for each spatial dimension). That is, the first, second, and third
 columns indicate the x-, y-, and z-coordinates in MNI space respectively.
 The number of rows in the array correspond to the number of coordinates that
-belong to this set. Note, that junifer (as of yet) only works in MNI space, and
-so therefore these coordinates should always be real-world coordinates of the
-MNI space.
+belong to this set.
 
-Lastly, the ``voi_names`` argument takes a list of strings
+The ``voi_names`` argument takes a list of strings
 indicating the names of each coordinate (i.e. volume-of-interest) in the
 ``coordinates`` array. Therefore, the length of this list should correspond to
 the number of rows in the coordinates array. Now, we know everything we need to
 know to register a set of coordinates.
 
+Lastly, we specify the ``space`` that the coordinates are in, for example,
+``"MNI"`` or ``"native"`` (scanner-native space).
+
 Step 1: Prepare code to register a set of coordinates
 -----------------------------------------------------
 
 Let's make a simple script to register our coordinates. We could simply call it
 ``register_custom_coordinates.py``. We may start by importing the appropriate
 packages:
 
 .. code-block:: python
 
   from junifer.data import register_coordinates
   import numpy as np
 
 For the sake of this example, we can create a set of coordinates that belong
-to the default mode network (DMN), and register this set of coordinates with
-junifer. Note, that junifer already has a
+to the Default Mode Network (DMN), and register this set of coordinates with
+``junifer``. Note, that ``junifer`` already has a
 :ref:`set of coordinates built-in <builtin>` ("DMNBuckner") that is associated
 with the DMN. Here, we use the DMN coordinates used in a
 `nilearn example <https://nilearn.github.io/dev/auto_examples/03_connectivity/plot_sphere_based_connectome.html>`_.
 
 .. code-block:: python
 
   dmn_coords = np.array(
@@ -86,27 +88,28 @@
 simply use this to register our coordinates:
 
 .. code-block:: python
 
   register_coordinates(
       name="DMNCustom",
       coordinates=dmn_coords,
-      voi_names=voi_names
+      voi_names=voi_names,
+      space="MNI"
   )
 
-Now, when we run this script, junifer registers these coordinates and we can
+Now, when we run this script, ``junifer`` registers these coordinates and we can
 use them in subsequent analyses. Let's now consider how to use coordinate
 registration in combination with
 :ref:`codeless configuration using a YAML file <codeless>`.
 
 Step 2: Add coordinate registration to the YAML file
 ----------------------------------------------------
 
 In order to register your coordinates for a pipeline configured by a YAML file,
-you can use the ``with`` keyword provided by junifer:
+you can use the ``with`` keyword provided by ``junifer``:
 
 .. code-block:: yaml
 
   with:
     - register_custom_coordinates.py
 
 Afterwards continue configuring the rest of your pipeline in this YAML file,
```

### Comparing `junifer-0.0.4.dev90/docs/extending/datagrabber.rst` & `junifer-0.0.5.dev11/docs/extending/datagrabber.rst`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 Data Grabbers are the first step of the pipeline. Its purpose is to interpret
 the structure of a dataset and provide two specific functionalities:
 
 #. Given an *element*, provide the path to each kind of data available for this
    element (e.g. the path to the T1 image, the path to the T2 image, etc.)
 #. Provide the list of *elements* available in the dataset.
 
-In this section, we will see how to create a datagrabber for a dataset. Basic
-aspects of datagrabbers are covered in the
+In this section, we will see how to create a DataGrabber for a dataset. Basic
+aspects of DataGrabbers are covered in the
 :ref:`Understanding Data Grabbers <datagrabber>` section.
 
 .. _extending_datagrabbers_think:
 
 Step 1: Think about the element
 -------------------------------
 
 Like with any programming-related task, the first step is to think. When
-creating a Data Grabber, we need to first define what an *element* is.
+creating a DataGrabber, we need to first define what an *element* is.
 The *element* should be the smallest unit of data that can be processed. That
 is, for each element, there should be a set of data that can be processed, but
 only one of each *data type* (see :ref:`data_types`).
 
 For example, if we have a dataset from a fMRI study in which:
 
 a. both T1w and fMRI was acquired
@@ -38,36 +38,36 @@
 * ``subject``: The subject IDs, e.g. ``sub001``, ``sub002``, ... ``sub020``
 * ``session``: The session number, e.g. ``ses1``, ``ses2``
 * ``task``: The task performed, e.g. ``rest``, ``stroop``
 
 If any of these items were not part of the element, then we will have more than
 one ``T1w`` and / or ``BOLD`` image for each subject, which is not allowed.
 
-Importantly, nothing prevents that one image is part of two different elements.
-For example, it is usually the case that the ``T1w`` image is not acquired for
-each task, but once in the entire session. So in this case, the ``T1w`` image
-for the element (``sub001``, ``ses1``, ``rest``) will be the same as the
-``T1w`` image for the element (``sub001``, ``ses1``, ``stroop``).
+Importantly, nothing prevents that one image being part of two different
+elements. For example, it is usually the case that the ``T1w`` image is not
+acquired for each task, but once in the entire session. So in this case, the
+``T1w`` image for the element (``sub001``, ``ses1``, ``rest``) will be the same
+as the ``T1w`` image for the element (``sub001``, ``ses1``, ``stroop``).
 
 We will now continue this section using as an example, a dataset in BIDS format
 in which 9 subjects (``sub-01`` to ``sub-09``) were scanned each during 3
 sessions (``ses-01``, ``ses-02``, ``ses-03``) and each session included a
 ``T1w`` and a ``BOLD`` image (resting-state), except for ``ses-03`` which was
-only anatomical.
+only anatomical data.
 
 Step 2: Think about the dataset's structure
 -------------------------------------------
 
 Now that we have our element defined, we need to think about the structure of
 the dataset. Mainly, because the structure of the dataset will determine how
-the Data Grabber needs to be implemented.
+the DataGrabber needs to be implemented.
 
-Junifer provides an abstract class to deal with datasets that can be thought in
-terms of *patterns*. A *pattern* is a string that contains placeholders that are
-replaced by the actual values of the element. In our BIDS example, the path
+``junifer`` provides a concrete class to deal with datasets that can be thought
+in terms of *patterns*. A *pattern* is a string that contains placeholders that
+are replaced by the actual values of the element. In our BIDS example, the path
 to the T1w image of subject ``sub-01`` and session ``ses-01``, relative to the
 dataset location, is ``sub-01/ses-01/anat/sub-01_ses-01_T1w.nii.gz``. By
 replacing ``sub-01`` with ``sub-02``, we can obtain the T1w image of the first
 session of the second subject. Indeed, the path to the T1w images can be
 expressed as a pattern:
 
 ``{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz``
@@ -84,79 +84,92 @@
 in terms of patterns, then follow :ref:`extending_datagrabbers_pattern`.
 Otherwise, we recommend that you take time to re-think about your dataset
 structure and why it does not have clear *patterns*. Feel free to open a
 discussion in the `junifer Discussions`_ page. Most probably we can help you
 get your dataset in order.
 
 If there is no other way, then you can follow :ref:`extending_datagrabbers_base`
-to create a Data Grabber from scratch.
+to create a DataGrabber from scratch.
 
 .. _extending_datagrabbers_pattern:
 
 Step 3: Create a Data Grabber
 -----------------------------
 
 Option A: Extending from PatternDataGrabber
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The :class:`.PatternDataGrabber` class is an abstract class that has the
+The :class:`.PatternDataGrabber` class is a concrete class that has the
 functionality of understanding patterns embedded in it.
 
-Before creating the datagrabber, we need to define 3 variables:
+Before creating the DataGrabber, we need to define 3 variables:
 
 * ``types``: A list with the available :ref:`data_types` in our dataset.
-* ``patterns``: A dictionary that specifies the pattern for each data type.
+* ``patterns``: A dictionary that specifies the pattern and some additional
+  information for each data type.
 * ``replacements``: A list indicating which of the elements in the patterns
   should be replaced by the values of the element.
 
 For example, in our BIDS example, the variables will be:
 
 .. code-block:: python
 
     types = ["T1w", "BOLD"]
     patterns = {
-       "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-       "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+       "T1w": {
+           "pattern": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+           "space": "native",
+       },
+       "BOLD": {
+           "pattern": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+           "space": "MNI152NLin6Asym",
+       },
     }
     replacements = ["subject", "session"]
 
 An additional fourth variable is the ``datadir``, which should be the path to
 where the dataset is located. For example, if the dataset is located in
 ``/data/project/test/data``, then ``datadir`` should be
 ``/data/project/test/data``. Or, if we want to allow the user to specify the
 location of the dataset, we can expose the variable in the constructor, as in
 the following example.
 
-With the variables defined above, we can create our datagrabber and name it
+With the variables defined above, we can create our DataGrabber and name it
 ``ExampleBIDSDataGrabber``:
 
 .. code-block:: python
 
     from pathlib import Path
 
     from junifer.datagrabber import PatternDataGrabber
 
 
     class ExampleBIDSDataGrabber(PatternDataGrabber):
 
         def __init__(self, datadir: str | Path) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
-               "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-               "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+               "T1w": {
+                   "pattern": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+                   "space": "native",
+               },
+               "BOLD": {
+                   "pattern": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+                   "space": "MNI152NLin6Asym",
+               },
             }
             replacements = ["subject", "session"]
             super().__init__(
                datadir=datadir,
                types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
-Our datagrabber is ready to be used by junifer. However, it is still unknown
+Our DataGrabber is ready to be used by ``junifer``. However, it is still unknown
 to the library. We need to register it in the library. To do so, we need to
 use the :func:`.register_datagrabber` decorator.
 
 
 .. code-block:: python
 
     from pathlib import Path
@@ -167,29 +180,35 @@
 
     @register_datagrabber
     class ExampleBIDSDataGrabber(PatternDataGrabber):
 
         def __init__(self, datadir: str | Path) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
-               "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-               "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+               "T1w": {
+                   "pattern": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+                   "space": "native",
+               },
+               "BOLD": {
+                   "pattern": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+                   "space": "MNI152NLin6Asym",
+               },
             }
             replacements = ["subject", "session"]
             super().__init__(
                datadir=datadir,
                types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
 
-Now, we can use our datagrabber in junifer, by setting the ``datagrabber`` kind
-in the yaml file to ``ExampleBIDSDataGrabber``. Remember that we still need to
-set the ``datadir``.
+Now, we can use our DataGrabber in ``junifer``, by setting the ``datagrabber``
+kind in the yaml file to ``ExampleBIDSDataGrabber``. Remember that we still need
+to set the ``datadir``.
 
 .. code-block:: yaml
 
       datagrabber:
          kind: ExampleBIDSDataGrabber
          datadir: /data/project/test/data
 
@@ -205,15 +224,15 @@
 location of the dataset, but the location where the dataset will be cloned. It
 can now be ``None``, which means that the data will be downloaded to a
 temporary directory. To set the location of the dataset, you can use the
 ``uri`` argument in the constructor. Additionally, a ``rootdir`` argument can
 be used to specify the path to the root directory of the dataset after doing
 ``datalad clone``.
 
-In the example, the dataset is hosted in gin
+In the example, the dataset is hosted in Gin
 (``https://gin.g-node.org/juaml/datalad-example-bids``).
 
 When we clone this dataset, we will see the following structure:
 
 .. code-block::
 
       .
@@ -234,77 +253,110 @@
 Now we have our 2 additional variables:
 
 .. code-block:: python
 
     uri = "https://gin.g-node.org/juaml/datalad-example-bids"
     rootdir = "example_bids_ses"
 
-And we can create our datagrabber:
+And we can create our DataGrabber:
 
 .. code-block:: python
 
     from junifer.api.decorators import register_datagrabber
     from junifer.datagrabber import PatternDataladDataGrabber
 
 
     @register_datagrabber
     class ExampleBIDSDataGrabber(PatternDataladDataGrabber):
 
         def __init__(self) -> None:
             types = ["T1w", "BOLD"]
             patterns = {
-               "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-               "BOLD": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+               "T1w": {
+                   "pattern": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+                   "space": "native",
+               },
+               "BOLD": {
+                   "pattern": "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+                   "space": "MNI152NLin6Asym",
+               },
             }
             replacements = ["subject", "session"]
             uri = "https://gin.g-node.org/juaml/datalad-example-bids"
             rootdir = "example_bids_ses"
             super().__init__(
                datadir=None,
                uri=uri,
                rootdir=rootdir,
                types=types,
                patterns=patterns,
                replacements=replacements,
             )
 
+This approach can be used directly from the YAML, like so:
+
+.. code-block:: yaml
+
+   datagrabber:
+     - kind: PatternDataladDataGrabber
+       types:
+         - BOLD
+         - T1w
+       patterns:
+         BOLD:
+           pattern: "{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz"
+           space: MNI152NLin6Asym
+         T1w:
+           pattern: "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz"
+           space: native
+       replacements:
+         - subject
+         - session
+       uri: "https://gin.g-node.org/juaml/datalad-example-bids"
+       rootdir: example_bids_ses
 
 .. _extending_datagrabbers_base:
 
 Option B: Extending from BaseDataGrabber
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-While we could not think of a use case in which the pattern-based datagrabber
-would not be suitable, it is still possible to create a datagrabber extending
+While we could not think of a use case in which the pattern-based DataGrabber
+would not be suitable, it is still possible to create a DataGrabber extending
 from the :class:`.BaseDataGrabber` class.
 
-In order to create a datagrabber extending from :class:`.BaseDataGrabber`, we
+In order to create a DataGrabber extending from :class:`.BaseDataGrabber`, we
 need to implement the following methods:
 
 - ``get_item``: to get a single item from the dataset.
 - ``get_elements``: to get the list of all elements present in the dataset
 - ``get_element_keys``: to get the keys of the elements in the dataset.
 
 .. note::
 
    The ``__init__`` method could also be implemented, but it is not mandatory.
-   This is required if the datagrabber requires any extra parameter.
+   This is required if the DataGrabber requires any extra parameter.
 
 We will now implement our BIDS example with this method.
 
 The first method, ``get_item``, needs to obtain a single
 item from the dataset. Since this dataset requires two variables, ``subject``
 and ``session``, we will use them as parameters of ``get_item``:
 
 .. code-block:: python
 
-   def get_item(self, subject: str, session: str) -> dict[str, str]:
+   def get_item(self, subject: str, session: str) -> dict[str, dict[str, str]]:
       out = {
-         "T1w": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-         "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+         "T1w": {
+             "path": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+             "space": "native",
+         },
+         "BOLD": {
+             "path": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+             "space": "MNI152NLin6Asym",
+         },
       }
       return out
 
 
 The second method, ``get_elements``, needs to return a list of all the elements
 in the dataset. In this case, we know that the dataset contains 3 subjects and 3
 sessions, so we can create a list of all the possible combinations. However, we
@@ -335,31 +387,37 @@
 
 .. code-block:: python
 
    def get_element_keys(self) -> list[str]:
       return ["subject", "session"]
 
 
-So, to summarize, our datagrabber will look like this:
+So, to summarise, our DataGrabber will look like this:
 
 .. code-block:: python
 
    from junifer.api.decorators import register_datagrabber
    from junifer.datagrabber import BaseDataGrabber
 
 
    @register_datagrabber
    class ExampleBIDSDataGrabber(BaseDataGrabber):
 
-      def get_item(self, subject: str, session: str) -> dict[str, str]:
+      def get_item(self, subject: str, session: str) -> dict[str, dict[str, str]]:
          out = {
-            "T1w": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-            "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+            "T1w": {
+                "path": f"{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+                "space": "native",
+            },
+            "BOLD": {
+                "path": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+                "space": "MNI152NLin6Asym",
+            },
          }
-      return out
+         return out
 
       def get_elements(self) -> list[str]:
          subjects = ["sub-01", "sub-02", "sub-03"]
          sessions = ["ses-01", "ses-02"]
 
          # If we are not working on BOLD data, we can add "ses-03"
          if "BOLD" not in self.types:
@@ -399,15 +457,15 @@
 not standardised.
 
 .. note::
 
    The ``mappings`` key is only required if the ``format`` is ``adhoc``. If the
    ``format`` is ``fmriprep``, the ``mappings`` key is not required.
 
-Currently, junifer provides only one confound remover step
+Currently, ``junifer`` provides only one confound remover step
 (:class:`.fMRIPrepConfoundRemover`), which relies entirely on the ``fmriprep``
 confound variable names. Thus, if the confounds are not in ``fmriprep`` format,
 the user will need to provide the mappings between the *ad-hoc* variable names
 and the ``fmriprep`` variable names. This is done by specifying the ``adhoc``
 format and providing the mappings as a dictionary in the ``mappings`` key.
 
 In the following example, the confounds file has 3 variables that are not in the
@@ -417,24 +475,28 @@
 
 .. code-block:: python
 
    def get_item(
       self, subject: str, session: str
    ) -> dict:
       out = {
-         "BOLD": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+         "BOLD": {
+             "path": f"{subject}/{session}/func/{subject}_{session}_task-rest_bold.nii.gz",
+             "space": "MNI152NLin6Asym",
+         },
          "BOLD_confounds": {
-            "path": f"{subject}/{session}/func/{subject}_{session}_confounds.tsv",
-            "format": "adhoc",
-            "mappings": {
-               "fmriprep": {
-                  "variable1": "rot_x",
-                  "variable2": "rot_z",
-                  "variable3": "rot_y",
-               }
+             "path": f"{subject}/{session}/func/{subject}_{session}_confounds.tsv",
+             "format": "adhoc",
+             "mappings": {
+                 "fmriprep": {
+                    "variable1": "rot_x",
+                    "variable2": "rot_z",
+                    "variable3": "rot_y",
+                 },
+             },
          },
       }
 
 .. note::
 
    Not all of the mappings need to be provided. For the moment, this is used
    only by the :class:`.fMRIPrepConfoundRemover` step, which requires variables
```

### Comparing `junifer-0.0.4.dev90/docs/extending/extension.rst` & `junifer-0.0.5.dev11/docs/extending/extension.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 .. include:: ../links.inc
 
 .. _extending_extension:
 
-Creating a junifer extension
-============================
+Creating a ``junifer`` extension
+================================
 
-Junifer is designed to be easily extensible. Through the use of a registry and
-decorators, you can easily add new functionality to junifer during runtime. This
-is done by creating a new Python module and importing it before running junifer.
+``junifer`` is designed to be easily extensible. Through the use of a registry
+and decorators, you can easily add new functionality to ``junifer`` during
+runtime. This is done by creating a new Python module and importing it before
+running ``junifer``.
 
 A special consideration has to be made when using the
 :ref:`code-less configuration<codeless>`. In this case, the
 ``with`` statement can be used to import a module or run a Python file.
 
-In the following example, we instruct junifer to first import ``my_module`` and
-then run the ``my_file.py`` file.
+In the following example, we instruct ``junifer`` to first import ``my_module``
+and then run the ``my_file.py`` file:
 
 .. code-block:: yaml
 
     with:
       - my_module
       - my_file.py
 
-Thus, the code from ``my_file.py`` will be executed before running junifer. This
-is the ideal place to include junifer extensions.
+Thus, the code from ``my_file.py`` will be executed before running ``junifer``.
+This is the ideal place to include ``junifer`` extensions.
 
 .. important::
 
-   Some junifer commands will not consider files imported from files included
+   Some ``junifer`` commands will not consider files imported from files included
    in the ``with`` statement. If ``my_file.py`` imports ``my_other_file.py``,
-   some of the junifer commands will not consider ``my_other_file.py``. Either
+   some of the ``junifer`` commands will not consider ``my_other_file.py``. Either
    place all the code in one file or add multiple files to the ``with``
    statement.
```

### Comparing `junifer-0.0.4.dev90/docs/extending/index.rst` & `junifer-0.0.5.dev11/docs/extending/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 .. include:: ../links.inc
 
 .. _extending:
 
-Extending junifer
-=================
+Extending ``junifer``
+=====================
 
 While we aim to provide as many datasets and markers as possible, we are also
 interested in allowing users to extend the functionality with their own
-datagrabbers, preprocessing, markers, etc., .
+DataGrabbers, Preprocessors, Markers, etc., .
 
-It's not necessary to have the new functionality included in junifer before
+It's not necessary to have the new functionality included in ``junifer`` before
 the user can use them. The user can simply create a new Python file, code the
-desired functionality and use it with junifer. This is the first step towards
-including the new functionality in the junifer pipeline.
+desired functionality and use it with ``junifer``. This is the first step towards
+including the new functionality in the ``junifer`` pipeline.
 
-In this section we will show how to extend junifer, by creating new
-datagrabbers, preprocessing, markers, etc.,  following the *junifer* way.
+In this section we will show how to extend ``junifer``, by creating new
+DataGrabbers, Preprocessors, Markers, etc.,  following the *junifer* way.
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    extension
    datagrabber
    marker
+   preprocessor
+   dependencies
    parcellations
    coordinates
    masks
```

### Comparing `junifer-0.0.4.dev90/docs/extending/marker.rst` & `junifer-0.0.5.dev11/docs/extending/marker.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 .. include:: ../links.inc
 
 .. _extending_markers:
 
 Creating Markers
 ================
 
-Computing a marker (a.k.a. *feature*) is the main goal of junifer. While we aim
-to provide as many markers as possible, it might be the case that the marker you
-are looking for is not available. In this case, you can create your own marker
+Computing a marker (a.k.a. *feature*) is the main goal of ``junifer``. While we
+aim to provide as many Markers as possible, it might be the case that the Marker
+you are looking for is not available. In this case, you can create your own Marker
 by following this tutorial.
 
-Most of the functionality of a junifer marker has been taken care by the
+Most of the functionality of a ``junifer`` Marker has been taken care by the
 :class:`.BaseMarker` class. Thus, only a few methods are required:
 
 #. ``get_valid_inputs``: The method to obtain the list of valid inputs for the
-   marker. This is used to check that the inputs provided by the user are
+   Marker. This is used to check that the inputs provided by the user are
    valid. This method should return a list of strings, representing
    :ref:`data types <data_types>`.
-#. ``get_output_type``: The method to obtain the kind of output of the marker.
-   This is used to check that the output of the marker is compatible with the
+#. ``get_output_type``: The method to obtain the output type of the Marker.
+   This is used to check that the output of the Marker is compatible with the
    storage. This method should return a string, representing
    :ref:`storage types <storage_types>`.
-#. ``compute``: The method that given the data, computes the marker.
-#. ``__init__``: The initialisation method, where the marker is configured.
+#. ``compute``: The method that given the data, computes the Marker.
+#. ``__init__``: The initialisation method, where the Marker is configured.
 
-As an example, we will develop a ``ParcelMean`` marker, a marker that first
+As an example, we will develop a ``ParcelMean`` Marker, a Marker that first
 applies a parcellation and then computes the mean of the data in each parcel.
-This is a very simple example, but it will show you how to create a new marker.
+This is a very simple example, but it will show you how to create a new Marker.
 
 .. _extending_markers_input_output:
 
 Step 1: Configure input and output
 ----------------------------------
 
-This step is quite simple: we need to define the input and output of the marker.
+This step is quite simple: we need to define the input and output of the Marker.
 Based on the current :ref:`data types <data_types>`, we can have ``BOLD``,
 ``VBM_WM`` and ``VBM_GM`` as valid inputs.
 
 .. code-block:: python
 
     def get_valid_inputs(self) -> list[str]:
         return ["BOLD", "VBM_WM", "VBM_GM"]
 
-The output of the marker depends on the input. For ``BOLD``, it will be
+The output of the Marker depends on the input. For ``BOLD``, it will be
 ``timeseries``, while for the rest of the inputs, it will be ``vector``. Thus,
 we can define the output as:
 
 .. code-block:: python
 
-    def get_output_type(self, input_kind: str) -> str:
-        if input_kind == "BOLD":
+    def get_output_type(self, input_type: str) -> str:
+        if input_type == "BOLD":
             return "timeseries"
         else:
             return "vector"
 
 .. _extending_markers_init:
 
-Step 2: Initialise the marker
+Step 2: Initialise the Marker
 -----------------------------
 
-In this step we need to define the parameters of the marker the user can provide
-to configure how the marker will behave.
+In this step we need to define the parameters of the Marker the user can provide
+to configure how the Marker will behave.
 
-The parameters of the marker are defined in the ``__init__`` method. The
+The parameters of the Marker are defined in the ``__init__`` method. The
 :class:`.BaseMarker` class requires two optional parameters:
 
-1. ``name``: the name of the marker. This is used to identify the marker in the
+1. ``name``: the name of the Marker. This is used to identify the Marker in the
    configuration file.
-2. ``on``: a list or string with the data types that the marker will be applied
+2. ``on``: a list or string with the data types that the Marker will be applied
    to.
 
 .. attention::
 
    Only basic types (*int*, *bool* and *str*), lists, tuples and dictionaries
    are allowed as parameters. This is because the parameters are stored in
    JSON format, and JSON only supports these types.
@@ -88,37 +88,37 @@
        name: str | None = None,
     ) -> None:
         self.parcellation = parcellation
         super().__init__(on=on, name=name)
 
 .. caution::
 
-   Parameters of the marker must be stored as object attributes without using
+   Parameters of the Marker must be stored as object attributes without using
    ``_`` as prefix. This is because any attribute that starts with ``_`` will
    not be considered as a parameter and not stored as part of the metadata of
-   the marker.
+   the Marker.
 
 .. _extending_markers_compute:
 
-Step 3: Compute the marker
+Step 3: Compute the Marker
 --------------------------
 
-In this step, we will define the method that computes the marker. This method
-will be called by junifer when needed, using the data provided by the
-datagrabber, as configured by the user. The method ``compute`` has two
+In this step, we will define the method that computes the Marker. This method
+will be called by ``junifer`` when needed, using the data provided by the
+DataGrabber, as configured by the user. The method ``compute`` has two
 arguments:
 
-* ``input``: a dictionary with the data to be used to compute the marker. This
+* ``input``: a dictionary with the data to be used to compute the Marker. This
   will be the corresponding element in the :ref:`Data Object<data_object>`
   already indexed. Thus, the dictionary has at least two keys: ``data`` and
   ``path``. The first one contains the data, while the second one contains the
   path to the data. The dictionary can also contain other keys, depending on the
   data type.
 * ``extra_input``: the rest of the :ref:`Data Object<data_object>`. This is
-  useful if you want to use other data to compute the marker
+  useful if you want to use other data to compute the Marker
   (e.g.: ``BOLD_confounds`` can be used to de-confound the ``BOLD`` data).
 
 Following the example, we will compute the mean of the data in each parcel using
 :class:`nilearn.maskers.NiftiLabelsMasker`. Importantly, the output of the
 compute function must be a dictionary. This dictionary will later be passed onto
 the ``store`` method.
 
@@ -129,33 +129,31 @@
    For example, if the output is a ``vector``, the keys of the dictionary should
    be ``data`` and ``col_names``.
 
 .. code-block:: python
 
     from typing import Any
 
-    from junifer.data import load_parcellation
+    from junifer.data import get_parcellation
     from nilearn.maskers import NiftiLabelsMasker
 
 
     def compute(
        self,
        input: dict[str, Any],
        extra_input: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         # Get the data
         data = input["data"]
 
-        # Get the min of the voxels sizes and use it as the resolution
-        resolution = np.min(data.header.get_zooms()[:3])
-
-        # Load the parcellation
-        t_parcellation, t_labels, _ = load_parcellation(
+        # Get the parcellation tailored for the target
+        t_parcellation, t_labels, _ = get_parcellation(
             name=self.parcellation_name,
-            resolution=resolution,
+            target_data=input,
+            extra_input=extra_input,
         )
 
         # Create a masker
         masker = NiftiLabelsMasker(
             labels_img=t_parcellation,
             standardize=True,
             memory="nilearn_cache",
@@ -169,40 +167,41 @@
         out = {"data": out_values, "col_names": t_labels}
 
         return out
 
 
 .. _extending_markers_finalize:
 
-Step 4: Finalise the marker
+Step 4: Finalise the Marker
 ---------------------------
 
-Once all of the above steps are done, we just need to give our marker a name,
+Once all of the above steps are done, we just need to give our Marker a name,
 state its *dependencies* and register it using the ``@register_marker``
 decorator.
 
-The *dependencies* are the core packages that are required to compute the marker.
-This will be later used to keep track of the versions of the packages used to
-compute the marker. To inform junifer about the dependencies of a marker, we need
-to define a ``_DEPENDENCIES`` attribute in the class. This attribute must be a
-set, with the names of the packages as strings. For example, the ``ParcelMean``
-marker has the following dependencies:
+The :ref:`dependencies <specifying_dependencies>` are the core packages that are
+required to compute the Marker. This will be later used to keep track of the
+versions of the packages used to compute the Marker. To inform ``junifer``
+about the dependencies of a Marker, we need to define a ``_DEPENDENCIES``
+attribute in the class. This attribute must be a set, with the names of the
+packages as strings. For example, the ``ParcelMean`` marker has the
+following dependencies:
 
 .. code-block:: python
 
     _DEPENDENCIES = {"nilearn", "numpy"}
 
-Finally, we need to register the marker using the ``@register_marker`` decorator.
+Finally, we need to register the Marker using the ``@register_marker`` decorator.
 
 .. code-block:: python
 
     from typing import Any
 
     from junifer.api.decorators import register_marker
-    from junifer.data import load_parcellation
+    from junifer.data import get_parcellation
     from junifer.markers.base import BaseMarker
     from nilearn.maskers import NiftiLabelsMasker
 
 
     @register_marker
     class ParcelMean(BaseMarker):
 
@@ -216,35 +215,33 @@
         ) -> None:
             self.parcellation = parcellation
             super().__init__(on=on, name=name)
 
         def get_valid_inputs(self) -> list[str]:
             return ["BOLD", "VBM_WM", "VBM_GM"]
 
-        def get_output_type(self, input_kind: str) -> str:
-            if input_kind == "BOLD":
+        def get_output_type(self, input_type: str) -> str:
+            if input_type == "BOLD":
                 return "timeseries"
             else:
                 return "vector"
 
         def compute(
            self,
            input: dict[str, Any],
            extra_input: dict[str, Any] | None = None,
         ) -> dict[str, Any]:
             # Get the data
             data = input["data"]
 
-            # Get the min of the voxels sizes and use it as the resolution
-            resolution = np.min(data.header.get_zooms()[:3])
-
-            # Load the parcellation
-            t_parcellation, t_labels, _ = load_parcellation(
+            # Get the parcellation tailored for the target
+            t_parcellation, t_labels, _ = get_parcellation(
                 name=self.parcellation_name,
-                resolution=resolution,
+                target_data=input,
+                extra_input=extra_input,
             )
 
             # Create a masker
             masker = NiftiLabelsMasker(
                 labels_img=t_parcellation,
                 standardize=True,
                 memory="nilearn_cache",
@@ -279,16 +276,16 @@
             super().__init__(on=on, name=name)
 
         def get_valid_inputs(self):
             # TODO: Complete with the valid inputs
             valid = []
             return valid
 
-        def get_output_type(self, input_kind):
-            # TODO: Return the valid output kind for each input kind
+        def get_output_type(self, input_type):
+            # TODO: Return the valid output type for each input type
             pass
 
         def compute(self, input, extra_input):
             # TODO: compute the marker and create the output dictionary
 
             # Create the output dictionary
             out = {"data": None, "col_names": None}
```

### Comparing `junifer-0.0.4.dev90/docs/extending/masks.rst` & `junifer-0.0.5.dev11/docs/extending/masks.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 .. include:: ../links.inc
 
 .. _adding_masks:
 
 Adding Masks
 ============
 
-Many processing steps and markers in junifer allow you to specify a binary
+Many processing steps and Markers in ``junifer`` allow you to specify a binary
 mask to select voxels you want to include in the analysis. There are a number
 of masks :ref:`in-built in junifer already <builtin>`, so check if any of them
 suit your needs. Check how to use these masks :ref:`here <using_masks>`. Once
 you know how to use these masks, and you checked whether the in-built masks
 suit your needs, and you have found that they don't, you can come back here to
 learn how to use your own masks.
 
 The principle is fairly simple and quite similar to :ref:`adding_parcellations`
-and :ref:`adding_coordinates`. junifer provides a :func:`.register_mask`
-function that lets you register your own custom masks. It consists of two
-positional arguments (``name`` and ``mask_path``) and one optional keyword
-argument (``overwrite``).
+and :ref:`adding_coordinates`. ``junifer`` provides a :func:`.register_mask`
+function that lets you register your own custom masks. It consists of three
+positional arguments (``name``, ``mask_path`` and ``space``) and one optional
+keyword argument (``overwrite``).
 
 The ``name`` argument is a string indicating the name of the mask. This name
-is used to refer to that mask in junifer internally in order to obtain the
+is used to refer to that mask in ``junifer`` internally in order to obtain the
 actual mask data and perform operations on it. For example, using the name you
 can load a mask after registration using the
 :func:`.load_mask` function.
 
 The ``mask_path`` should contain the path to a valid NIfTI image with binary
-voxel values (i.e. 0 or 1). This data can then be used by junifer to mask other
-MR images.
+voxel values (i.e. 0 or 1). This data can then be used by ``junifer`` to mask
+other MR images.
+
+Lastly, we specify the ``space`` that the coordinates are in, for example,
+``"MNI152NLin6Asym"`` or ``"native"`` (scanner-native space).
 
 Step 1: Prepare code to register a mask
 ---------------------------------------
 
 A simple script called ``register_custom_mask.py`` to register a mask could
 look as follows:
 
 .. code-block:: python
 
   from pathlib import Path
 
-  from junifer.data import register_custom_mask
+  from junifer.data import register_mask
 
 
   # this path is only an example, of course use the correct path
   # on your system:
   mask_path = Path("..") / ".." / "my_custom_mask.nii.gz"
 
-  register_mask(name="my_custom_mask", mask_path=mask_path)
+  register_mask(name="my_custom_mask", mask_path=mask_path, space="native")
 
 Simple, right? Now we just have to configure a YAML file to register this mask
 so we can use it for :ref:`codeless configuration of junifer <codeless>`.
 
 Step 2: Configure a YAML file for registration of a mask
 --------------------------------------------------------
 
-In order to do this, we can use the ``with`` keyword provided by junifer:
+In order to do this, we can use the ``with`` keyword provided by ``junifer``:
 
 .. code-block:: yaml
 
   with:
     - register_custom_mask.py
 
-Then we can use this mask for any processing step or marker that takes in a
+Then we can use this mask for any processing step or Marker that takes in a
 mask as an argument. For example:
 
 .. code-block:: yaml
 
   markers:
     - name: CustomMaskParcelAggregation_mean
       kind: ParcelAggregation
       parcellation: Schaefer200x17
       method: mean
       masks: "my_custom_mask"
 
-Now, you can simply use this YAML file to run your pipeline. One important
-point to keep in mind is that if the paths given in ``register_custom_mask.py``
-are relative paths, they will be interpreted by junifer as relative to the
-jobs directory (i.e. where junifer will create submit files, logs directory and
-so on). For simplicity, you may just want to use absolute paths to avoid
-confusion, yet using relative paths is likely a better way to make your
-pipeline directory/repository more portable and therefore more reproducible for
-others. Really, once you understand how these paths are interpreted by junifer,
-it is quite easy.
+Now, you can simply use this YAML file to run your pipeline.
+
+.. important::
+
+   It's important to keep in mind that if the paths given in
+   ``register_custom_mask.py`` are relative paths, they will be interpreted
+   by junifer as relative to the jobs directory (i.e. where ``junifer`` will
+   create submit files, logs directory and so on). For simplicity, you may just
+   want to use absolute paths to avoid confusion, yet using relative paths is
+   likely a better way to make your pipeline directory / repository more portable
+   and therefore more reproducible for others. Really, once you understand how
+   paths are interpreted by ``junifer``, it is quite easy.
```

### Comparing `junifer-0.0.4.dev90/docs/extending/parcellations.rst` & `junifer-0.0.5.dev11/docs/extending/parcellations.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 .. include:: ../links.inc
 
 .. _adding_parcellations:
 
 Adding Parcellations
 ====================
 
-Before you start adding your own parcellations, check whether junifer has
+Before you start adding your own parcellations, check whether ``junifer`` has
 the parcellation :ref:`in-built already <builtin>`. Perhaps, what is available
-there will suffice to achieve your goals. However, of course junifer will not
+there will suffice to achieve your goals. However, of course ``junifer`` will not
 have every parcellation available that you may want to use, and if so, it will
-be nice to be able to add it yourself using a format that junifer understands.
+be nice to be able to add it yourself using a format that ``junifer`` understands.
 Similarly, you may even be interested in creating your own custom parcellations
-and then adding them to junifer, so you can use junifer to obtain different
-markers to assess and validate your own parcellation. So, how can you do this?
+and then adding them to ``junifer``, so you can use ``junifer`` to obtain
+different Markers to assess and validate your own parcellation. So, how can you do
+this?
 
 Since both of these use-cases are quite common, and not being able to use your
-favourite parcellation is of course quite a buzzkill, junifer actually provides
-the easy-to-use :func:`.register_parcellation` function to do just that. Let's
-try to understand the API reference and then use this function to register our
+favourite parcellation is of course quite a buzzkill, ``junifer`` actually
+provides the easy-to-use :func:`.register_parcellation` function to do just that.
+Let's try to understand the API reference and then use this function to register our
 own parcellation.
 
-From the API reference, we can see that it has 3 positional arguments
-(``name``, ``parcellation_path``, and ``parcels_labels``) as well as one
-optional keyword argument (``overwrite``).
-
-The ``name`` of the parcellation is up to you and will be the name that junifer
-will use to refer to this particular parcellation. You can think of this as
-being similar to a key in a python dictionary, i.e. a key that is used to
+From the API reference, we can see that it has 4 positional arguments
+(``name``, ``parcellation_path``, ``parcels_labels`` and ``space``) as well as
+one optional keyword argument (``overwrite``).
+
+The ``name`` of the parcellation is up to you and will be the name that
+``junifer`` will use to refer to this particular parcellation. You can think of
+this as being similar to a key in a Python dictionary, i.e. a key that is used to
 obtain and operate on the actual parcellation data. This ``name`` must always
 be a string. For example, we could call our parcellation
 ``"my_custom_parcellation"`` (Note, that in a real-world use case this is
 likely not a good name, and you should try to choose a meaningful name that
 conveys as much relevant information about your parcellation as necessary).
 
 The ``parcellation_path`` must be a ``str`` or ``Path`` object indicating a
 path to a valid NIfTI image, which contains integer labels indicating the
 individual regions-of-interest (ROIs) of your parcellation. The background in
 this parcellation should be indicated by 0, and the labels of ROIs should go
 from 1 to N (where N is the total number of ROIs in your parcellation). Now,
 we nearly have everything we need.
 
-Lastly, we also want to make sure that we can associate each integer label with
+We also want to make sure that we can associate each integer label with
 a human readable name (i.e. the name for each ROI). This serves naming the
 features that parcellation-based markers produce in an unambiguous way, such
 that a user can easily identify which ROIs were used to produce a specific
 feature (multiple ROIs, because some features consist of information from two
 or more ROIs, as for example in functional connectivity). Therefore, we provide
 junifer with a list of strings, that contains the names for each ROI. In this
 list, the label at the i-th position indicates the i-th integer label (i.e. the
 first label in this list corresponds to the first integer label in the
 parcellation and so on).
 
+Lastly, we specify the ``space`` that the parcellation is in, for example,
+``"MNI152NLin2009cAsym"`` or ``"native"`` (scanner-native space).
+
 Step 1: Prepare code to register a parcellation
 -----------------------------------------------
 
-Now we know everything that we need to know to make sure junifer can use our
-own parcellation to compute any parcellation-based marker. For example,
-a simple example could look like this:
+Now we know everything that we need to know to make sure ``junifer`` can use our
+own parcellation to compute any parcellation-based Marker. A simple example could
+look like this:
 
 .. code-block:: python
 
   from junifer.data import register_parcellation
 
   from pathlib import Path
   import numpy as np
@@ -74,49 +78,53 @@
   )
 
   my_labels = list(np.loadtxt(path_to_labels, dtype=str))
 
   register_parcellation(
       name="my_custom_parcellation",
       parcellation_path=path_to_parcellation,
-      parcels_labels=my_labels
+      parcels_labels=my_labels,
+      space="MNI152NLin2009cAsym"
   )
 
 We can run this code and it seems to work, however, how can we actually
-include the custom parcellation in a junifer pipeline using a
+include the custom parcellation in a ``junifer`` pipeline using a
 :ref:`code-less YAML configuration <codeless>`?
 
 Step 2: Add parcellation registration to the YAML file
 ------------------------------------------------------
 
-In order to use the parcellation in a junifer pipeline configured by a YAML
-file, we can save the above code in a python file, say
+In order to use the parcellation in a ``junifer`` pipeline configured by a YAML
+file, we can save the above code in a Python file, say
 ``registering_my_parcellation.py``. We can then simply add this file using the
-``with`` keyword provided by junifer:
+``with`` keyword provided by ``junifer``:
 
 .. code-block:: yaml
 
   with:
     - registering_my_parcellation.py
 
 Afterwards continue configuring the rest of the pipeline in this YAML file, and
 you will be able to use this parcellation using the name you gave the
 parcellation when registering it. For example, we can add a
-:class:`.ParcelAggregation` marker to demonstrate how this can be done:
+:class:`.ParcelAggregation` Marker to demonstrate how this can be done:
 
 .. code-block:: yaml
 
   markers:
     - name: CustomParcellation_mean
       kind: ParcelAggregation
       parcellation: my_custom_parcellation
       method: mean
 
-Now, you can simply use this YAML file to run your pipeline. One important
-point to keep in mind is that if the paths given in
-``registering_my_parcellation.py`` are relative paths, they will be interpreted
-by junifer as relative to the jobs directory (i.e. where junifer will create
-submit files, logs directory and so on). For simplicity, you may just want to
-use absolute paths to avoid confusion, yet using relative paths is likely a
-better way to make your pipeline directory/repository more portable and
-therefore more reproducible for others. Really, once you understand how these
-paths are interpreted by junifer, it is quite easy.
+Now, you can simply use this YAML file to run your pipeline.
+
+.. important::
+
+   It's important to keep in mind that if the paths given in
+   ``registering_my_parcellation.py`` are relative paths, they will be interpreted
+   by ``junifer`` as relative to the jobs directory (i.e. where ``junifer`` will
+   create submit files, logs directory and so on). For simplicity, you may just
+   want to use absolute paths to avoid confusion, yet using relative paths is
+   likely a better way to make your pipeline directory / repository more portable
+   and therefore more reproducible for others. Really, once you understand how
+   these paths are interpreted by ``junifer``, it is quite easy.
```

### Comparing `junifer-0.0.4.dev90/docs/faq.rst` & `junifer-0.0.5.dev11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/help.rst` & `junifer-0.0.5.dev11/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/images/junifer_logo.png` & `junifer-0.0.5.dev11/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/index.rst` & `junifer-0.0.5.dev11/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -47,10 +47,10 @@
 
 Funding
 =======
 
 We thank the `Helmholtz Imaging Platform <https://helmholtz-imaging.de/>`_,
 `SMHB <https://www.fz-juelich.de/en/smhb>`_ and
 `eBRAIN Health <https://www.ebrain-health.eu/>`_  (HORIZON-INFRA-2021-TECH-01)
-for supporting development of Junifer.
+for supporting development of ``junifer``.
 (The funding sources had no role in the design, implementation and evaluation of
 the pipeline.)
```

### Comparing `junifer-0.0.4.dev90/docs/links.inc` & `junifer-0.0.5.dev11/docs/links.inc`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .. _`Python`: https://python.org
 .. _`seaborn`: https://seaborn.pydata.org
 .. _`matplotlib`: https://matplotlib.org
 .. _`fMRIPrep`: https://fmriprep.org
 .. _`nilearn`: https://nilearn.github.io
 .. _`nipype`: https://nipype.readthedocs.io
 .. _`datalad`: https://datalad.org
+.. _`templateflow`: https://www.templateflow.org
 
 .. _`venv`: https://docs.python.org/3/tutorial/venv.html
 .. _`conda env`: https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html
 
 .. _`Github`: https://github.com/
 .. _`junifer Github`: https://github.com/juaml/junifer
 .. _`junifer Discussions`: https://github.com/juaml/junifer/discussions
```

### Comparing `junifer-0.0.4.dev90/docs/maintaining.rst` & `junifer-0.0.5.dev11/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.5.dev11/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/starting.rst` & `junifer-0.0.5.dev11/docs/starting.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 .. include:: links.inc
 
 .. _starting:
 
-First steps with junifer
-========================
+First steps with ``junifer``
+============================
 
 .. note::
 
    To scroll the graph left and right, click on the graph and use the arrows on your keyboard.
 
 .. mermaid::
 
    flowchart TD
      start((( Start )))
-     read_understanding(Read Understanding Junifer)
+     read_understanding(Read Understanding junifer)
      start --> read_understanding
      question_features{Can I compute\nthe features I want\nusing junifer?}
      read_understanding --> question_features
      question_features -->|Yes| read_using_final
      question_features -->|I'm not sure| read_using
      question_features -->|No| question_feature_type
      read_using --> question_features
 
-     read_using(Read Using Junifer)
+     read_using(Read Using junifer)
 
      question_feature_type{"What am I missing\nfrom junifer"}
      question_feature_type --> missing_datagrabber
      question_feature_type --> missing_preprocessing
      question_feature_type --> missing_marker
      question_feature_type --> missing_other
      missing_datagrabber("A Dataset/DataGrabber")
-     missing_preprocessing("A Preprocessing")
+     missing_preprocessing("A Preprocessor")
      missing_marker("A Marker")
      missing_other("Something else")
 
      missing_datagrabber --> question_datagrabber_junifarm
      question_datagrabber_junifarm{Is the\ndataset/datagrabber\nin juni-farm?}
      question_datagrabber_junifarm -->|Yes| read_using_final
      question_datagrabber_junifarm -->|No| read_extending_datagrabber_start
-     read_extending_datagrabber_start(Read Creating a Junifer extension)
+     read_extending_datagrabber_start(Read Creating a junifer extension)
      read_extending_datagrabber_start --> read_extending_datagrabber
      read_extending_datagrabber(Read Creating Data Grabbers)
      read_extending_datagrabber --> question_datagrabber_kind
      question_datagrabber_kind{Is your dataset\na datalad one?}
      question_datagrabber_kind -->|Yes| extend_datagrabber_datalad
      question_datagrabber_kind -->|No| extend_datagrabber_pattern
      extend_datagrabber_pattern(Use\nPatternDataGrabber)
@@ -51,87 +51,87 @@
      extend_datagrabber_datalad --> question_datagrabber_solved
      question_datagrabber_solved{Can you use\nyour data now?}
      question_datagrabber_solved -->|Yes| question_contribute_datagrabber
      question_datagrabber_solved -->|No| contact_help
      question_contribute_datagrabber{Do you think\nyour DataGrabber\nis useful for other users?}
      question_contribute_datagrabber -->|Yes| contribute_datagrabber
      question_contribute_datagrabber -->|No| final_run
-     contribute_datagrabber(Create a\nDATASET REQUEST\nissue on Github)
+     contribute_datagrabber(Create a\nDATASET REQUEST\nissue on GitHub)
      contribute_datagrabber --> final_run
 
      missing_marker --> question_marker_junifarm
      question_marker_junifarm{Is the marker\nin juni-farm?}
      question_marker_junifarm -->|Yes| read_using_final
      question_marker_junifarm -->|No| read_extending_marker_start
-     read_extending_marker_start(Read Creating a Junifer extension)
+     read_extending_marker_start(Read Creating a junifer extension)
      read_extending_marker_start --> read_extending_marker
      read_extending_marker(Read Creating Markers)
      read_extending_marker --> question_marker_solved
      question_marker_solved{Can you use\nyour marker now?}
      question_marker_solved -->|Yes| question_contribute_marker
      question_marker_solved -->|No| contact_help
      question_contribute_marker{Do you think\nyour Marker\nis useful for other users?}
      question_contribute_marker -->|Yes| contribute_marker
      question_contribute_marker -->|No| final_run
-     contribute_marker(Create a\nMARKER REQUEST\nissue on Github)
+     contribute_marker(Create a\nMARKER REQUEST\nissue on GitHub)
      contribute_marker --> final_run
 
      missing_preprocessing --> contact_help
 
      missing_mask{"A Mask?"}
      missing_parcellation{"A Parcellation?"}
      missing_coordinates{"Coordinates?"}
      missing_other_other{"Something else?"}
      missing_other --> missing_mask
      missing_other --> missing_parcellation
      missing_other --> missing_coordinates
      missing_other --> missing_other_other
      missing_other_other --> contact_help
 
-     contact_help(((Contact the\nJunifer team)))
+     contact_help(((Contact the\njunifer team)))
 
      missing_mask --> read_adding_mask_start
-     read_adding_mask_start("Read Creating a Junifer extension")
+     read_adding_mask_start("Read Creating a junifer extension")
      read_adding_mask_start --> read_adding_mask
      read_adding_mask("Read Adding Masks")
      read_adding_mask --> missing_other_solved
 
      missing_parcellation --> read_adding_parcellation_start
-     read_adding_parcellation_start("Read Creating a Junifer extension")
+     read_adding_parcellation_start("Read Creating a junifer extension")
      read_adding_parcellation_start --> read_adding_parcellation
      read_adding_parcellation("Read Adding Parcellations")
      read_adding_parcellation --> missing_other_solved
 
      missing_coordinates --> read_adding_coordinates_start
-     read_adding_coordinates_start("Read Creating a Junifer extension")
+     read_adding_coordinates_start("Read Creating a junifer extension")
      read_adding_coordinates_start --> read_adding_coordinates
      read_adding_coordinates("Read Adding Coordinates")
      read_adding_coordinates --> missing_other_solved
 
      missing_other_solved{Did you solve your issue?}
      missing_other_solved -->|Yes| read_using_final
      missing_other_solved -->|No| missing_other_contact
-     missing_other_contact(Contact the\nJunifer team)
+     missing_other_contact(Contact the\njunifer team)
      missing_other_contact --> missing_other_issue
-     missing_other_issue(((Submit a\nFEATURE REQUEST\nissue in Github)))
+     missing_other_issue(((Submit a\nFEATURE REQUEST\nissue in GitHub)))
 
-     read_using_final(Read Using Junifer)
+     read_using_final(Read Using junifer)
      read_using_final --> final_yaml
      final_yaml(Create/edit the YAML file)
      final_yaml --> final_run
      final_run(Use junifer run to test your YAML configuration)
      final_run --> question_final_run_worked
      question_final_run_worked{"Did it work?"}
      question_final_run_worked -->|No| question_error_run
      question_error_run{"Is it an issue\nwith my YAML file?"}
      question_error_run -->|Yes| final_yaml
      question_error_run -->|No| error_contact
-     error_contact(Contact the\nJunifer team)
+     error_contact(Contact the\njunifer team)
      error_contact --> error_issue
-     error_issue(((Submit a\nBUG REPORT issue\nin Github)))
+     error_issue(((Submit a\nBUG REPORT issue\nin GitHub)))
      question_final_run_worked -->|Yes| final_queue
      final_queue(Use junifer queue to compute your features)
      final_queue --> final_magic
      final_magic(((Let junifer do its magic!)))
 
      click read_understanding href "https://juaml.github.io/junifer/main/understanding/index.html"
      click read_using href "https://juaml.github.io/junifer/main/using/index.html"
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/data.rst` & `junifer-0.0.5.dev11/docs/understanding/data.rst`

 * *Files 3% similar despite different names*

```diff
@@ -99,17 +99,20 @@
 
    * - Name
      - Description
      - Example
    * - ``T1w``
      - T1w image (3D)
      - Preprocessed or Raw T1w image
+   * - ``T2w``
+     - T2w image (3D)
+     - Preprocessed or Raw T2w image
    * - ``BOLD``
      - BOLD image (4D)
-     - Preprocessed/Denoised BOLD image (fmriprep output)
+     - Preprocessed or Denoised BOLD image (fMRIPrep output)
    * - ``BOLD_confounds``
      - BOLD image confounds (CSV/TSV file)
      - Confounds that can be applied to the BOLD image.
    * - ``VBM_GM``
      - VBM Gray Matter segmentation (3D)
      - CAT output (`m0wp1` images)
    * - ``VBM_WM``
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/datagrabber.rst` & `junifer-0.0.5.dev11/docs/understanding/datagrabber.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 Data Grabber
 ============
 
 Description
 -----------
 
 The ``DataGrabber`` is an object that can provide an interface to datasets you
-want to work with in junifer. Every concrete implementation of a DataGrabber is
-aware of a particular dataset's structure and thus allows you to fetch specific
-elements of interest from the dataset. It adds the ``path`` key to each
+want to work with in ``junifer``. Every concrete implementation of a DataGrabber
+is aware of a particular dataset's structure and thus allows you to fetch
+specific elements of interest from the dataset. It adds the ``path`` key to each
 :ref:`data type <data_types>` in the :ref:`Data object <data_object>`.
 
 DataGrabbers are intended to be used as context managers. When used within a
 context, a DataGrabber takes care of any pre and post steps for interacting with
 the dataset, for example, downloading and cleaning up. As the interface
 is consistent, you always use the same procedure to interact with the DataGrabber.
 
 For example, a concrete implementation of :class:`.DataladDataGrabber` can
-provide junifer with data from a Datalad dataset. Of course, DataGrabbers are not
-only meant to work with Datalad datasets but any dataset.
+provide ``junifer`` with data from a Datalad dataset. Of course, DataGrabbers are
+not only meant to work with Datalad datasets but any dataset.
 
 If you are interested in using already provided DataGrabbers, please go to
 :doc:`../builtin`. And, if you want to implement your own DataGrabber, you need
-to provide concrete implementations of base classes already provided.
+to provide concrete implementations of abstract base classes already provided.
 
 Base Classes
 ------------
 
-In this section, we showcase different abstract base classes you might want to
-use to implement your own DataGrabber.
+In this section, we showcase different abstract and concrete base classes you
+might want to use to implement your own DataGrabber.
 
 .. list-table::
    :widths: auto
    :header-rows: 1
 
    * - Name
      - Description
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/datareader.rst` & `junifer-0.0.5.dev11/docs/understanding/datareader.rst`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 Data Reader
 ===========
 
 Description
 -----------
 
 The ``DataReader`` is an object that is responsible for actually reading data
-files in junifer. It reads the value of the key ``path`` for each
+files in ``junifer``. It reads the value of the key ``path`` for each
 :ref:`data type <data_types>` in the :ref:`Data object <data_object>` and loads
 them into memory. After reading the data into memory, it adds the key ``data``
 to the same level as ``path`` and the value is the actual data in the memory.
 
-DataReaders are meant to be used inside the datagrabber context but you can
+DataReaders are meant to be used inside the DataGrabber context but you can
 operate on them outside the context as long as the actual data is in the memory
 and the Python runtime has not garbage-collected it.
 
-For data formats not supported by junifer yet, you can either make your own
-*Data Reader* or open an issue on `junifer Github`_ and we can help you out.
+For data formats not supported by ``junifer`` yet, you can either make your own
+DataReader or open an issue on `junifer Github`_ and we can help you out.
 
 File Formats
 ------------
 
 We already provide a concrete implementation :class:`.DefaultDataReader` which
 knows how to read the following file formats:
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/marker.rst` & `junifer-0.0.5.dev11/docs/understanding/marker.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 .. important::
 
    This pre-process is not similar to pre-processing done by tools like FSL,
    SPM, AFNI, etc., . For example, one can perform confound removal on loaded
    data and then perform feature extraction.
 
-Markers are meant to be used inside the datagrabber context but you can operate
+Markers are meant to be used inside the DataGrabber context but you can operate
 on them outside the context as long as the actual data is in the memory and the
 Python runtime has not garbage-collected it.
 
-If you are interested in using already provided markers, please go to
-:doc:`../builtin`. And, if you want to implement your own marker, you need to
+If you are interested in using already provided Markers, please go to
+:doc:`../builtin`. And, if you want to implement your own Marker, you need to
 provide concrete implementation of :class:`.BaseMarker`. Specifically, you
 need to override ``get_valid_inputs``, ``get_output_type`` and ``compute``
 methods.
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/pipeline.rst` & `junifer-0.0.5.dev11/docs/understanding/pipeline.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 .. include:: ../links.inc
 
 .. _pipeline:
 
-The junifer Pipeline
-====================
+The ``junifer`` Pipeline
+========================
 
 The junifer pipeline is the main execution path of junifer. It consists of five
 steps:
 
 1. :ref:`Data Grabber <datagrabber>`: Interpret the dataset and provide a list
    of files.
 2. :ref:`Data Reader <datareader>`: Read the files.
-3. :ref:`Pre-processing <preprocess>`: Prepare the images for marker
+3. :ref:`Preprocess <preprocess>`: Prepare the files' data for marker
    computation.
-4. :ref:`Marker Computation <marker>`: Compute the marker.
-5. :ref:`Storage <storage>`: Store the marker values.
+4. :ref:`Marker Computation <marker>`: Compute the marker(s).
+5. :ref:`Storage <storage>`: Store the marker(s) values.
 
 The element that is passed across the pipeline is called the
 :ref:`Data Object<data_object>`.
 
 The following is a graphical representation of the pipeline:
 
 .. mermaid::
 
    flowchart LR
      dg[Data Grabber]
      dr[Data Reader]
-     pp[Pre-processing]
+     pp[Preprocess]
      mc[Marker Computation]
      st[Storage]
      dg --> dr
      dr --> pp
      pp --> mc
      mc --> st
 
@@ -41,15 +41,15 @@
 on multiple markers:
 
 .. mermaid::
 
    flowchart LR
      dg[Data Grabber]
      dr[Data Reader]
-     pp[Pre-processing]
+     pp[Preprocess]
      mc1[Marker Computation]
      mc2[Marker Computation]
      mc3[Marker Computation]
      mc4[Marker Computation]
      mc5[Marker Computation]
      st1[Storage]
      st2[Storage]
```

### Comparing `junifer-0.0.4.dev90/docs/understanding/storage.rst` & `junifer-0.0.5.dev11/docs/understanding/storage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 -----------
 
 The ``Storage`` is an object that is responsible for storing extracted features
 as computed from :ref:`Marker <marker>` step of the pipeline. If the pipeline is
 provided with a ``storage-like`` object, the extracted features are stored via
 that object else they are kept in memory.
 
-Storage is meant to be used inside the datagrabber context but you can operate
+Storage is meant to be used inside the DataGrabber context but you can operate
 on them outside the context as long as the processed data is in the memory and
 the Python runtime has not garbage-collected it.
 
 The :ref:`Markers <marker>` are responsible for defining what *storage kind*
 (``matrix``, ``vector``, ``timeseries``) they support for which
 :ref:`data type <data_types>` by overriding its ``get_output_type`` method. The
 storage object in turn declares and provides implementation for specific
 *storage kind*. For example, :class:`.SQLiteFeatureStorage` supports saving
 ``matrix``, ``vector`` and ``timeseries`` via ``store_matrix``, ``store_vector``
 and ``store_timeseries`` methods respectively.
 
-For storage interfaces not supported by junifer yet, you can either make your
-own ``Storage`` by providing a concrete implementation of
+For storage interfaces not supported by ``junifer`` yet, you can either make
+your own ``Storage`` by providing a concrete implementation of
 :class:`.BaseFeatureStorage` or open an issue on `junifer Github`_ and we can
 help you out.
 
 .. _storage_types:
 
 Storage Types
 -------------
```

### Comparing `junifer-0.0.4.dev90/docs/using/codeless.rst` & `junifer-0.0.5.dev11/docs/using/codeless.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 .. include:: ../links.inc
 
 .. _codeless:
 
 Code-less Configuration
 =======================
 
-On of the most important features of junifer is its capacity to run without
+One of the most important features of ``junifer`` is its capacity to run without
 writing a single line of code. This is achieved by using a configuration file
 that is written in YAML_. In this file, we configure the different steps of
 :ref:`pipeline`.
 
 As a reminder, this is how the pipeline looks like:
 
 .. mermaid::
 
    flowchart LR
      dg[Data Grabber]
      dr[Data Reader]
-     pp[Pre-processing]
+     pp[Preprocess]
      mc[Marker Computation]
      st[Storage]
      dg --> dr
      dr --> pp
      pp --> mc
      mc --> st
 
 
 Thus, the configuration file must configure each of the sections of the pipeline,
 as well as some general parameters.
 
 As an example, we will generate the configuration file for a pipeline that will
 extract the mean ``VBM_GM`` values using two different parcellations and one set
-of coordinates, from the ``Oasis VBM Testing dataset`` included in junifer.
+of coordinates, from the ``Oasis VBM Testing dataset`` included in ``junifer``.
 
 
 General Parameters
 ------------------
 
 The general parameters are the ones that are not specific to any of the sections
-of the pipeline, but configure junifer as a whole. These parameters are:
+of the pipeline, but configure ``junifer`` as a whole. These parameters are:
 
-* ``with``: A section used to specify modules and junifer extensions to use.
-* ``workdir``: The working directory where junifer will store temporary files.
+* ``with``: A section used to specify modules and ``junifer`` extensions to use.
+* ``workdir``: The working directory where ``junifer`` will store temporary files.
 
-Since the example uses a specific datagrabber for testing, we need to add
-``junifer.testing.registry`` to the ``with`` section. This will allow junifer
-to find the datagrabber. We will set the ``workdir`` to ``/tmp``.
+Since the example uses a specific DataGrabber for testing, we need to add
+``junifer.testing.registry`` to the ``with`` section. This will allow ``junifer``
+to find the DataGrabber. We will set the ``workdir`` to ``/tmp``.
 
 .. code-block:: yaml
 
   with: junifer.testing.registry
 
   workdir: /tmp
 
@@ -62,17 +62,17 @@
 * ``datareader``
 * ``preprocess``
 * ``markers``
 * ``storage``
 
 .. important::
 
-   The datareader step configuration is optional, as junifer only provides one
-   datareader. Nevertheless, it is possible to extend junifer with custom
-   datareaders, and thus, it is also possible to configure this step.
+   The ``datareader`` step configuration is optional, as ``junifer`` only
+   provides one DataReader. Nevertheless, it is possible to extend ``junifer``
+   with custom DataReaders, and thus, it is also possible to configure this step.
 
 
 Data Grabber
 ^^^^^^^^^^^^
 
 The ``datagrabber`` section must be configured using the ``kind`` key to specify
 the DataGrabber to use. Additional keys correspond to the parameters of the
@@ -103,17 +103,17 @@
   datagrabber:
     kind: OasisVBMTestingDataGrabber
 
 
 Data Reader
 ^^^^^^^^^^^
 
-As mentioned before, this section is entirely optional, as junifer only provides
-one DataReader (:class:`.DefaultDataReader`), which is the default in case the
-section is not specified.
+As mentioned before, this section is entirely optional, as ``junifer`` only
+provides one DataReader (:class:`.DefaultDataReader`), which is the default in
+case the section is not specified.
 
 In any case, the syntax of the section is the same as for the ``datagrabber``
 section, using the ``kind`` key to specify the DataReader to use, and additional
 keys to pass parameters to the DataReader constructor:
 
 .. code-block:: yaml
 
@@ -123,45 +123,46 @@
 
 For the ``Oasis VBM Testing dataset`` example, we will not specify a
 ``datareader`` step.
 
 Preprocess
 ^^^^^^^^^^
 
-Pre-processing is also an optional step, as it might be the case that no
-pre-processing is needed. In the case that pre-processing is needed, the section
-must be configured using the ``kind`` key to specify the preprocessor to use,
-and additional keys to pass parameters to the preprocessor.
+``preprocess`` is also an optional step, as it might be the case that no
+pre-processing is needed. As we can perform multiple preprocessing steps, it's
+passed as a list of Preprocessors. In the case that pre-processing is needed,
+each Preprocessord must be configured using the ``kind`` key to specify the
+Preprocessor to use, and additional keys to pass parameters to the Preprocessor.
 
-For example, to use the :class:`.fMRIPrepConfoundRemover` preprocessor, we just
+For example, to use the :class:`.fMRIPrepConfoundRemover` Preprocessor, we just
 need to specify its name as the ``kind`` key, as well as its parameters.
 
 .. code-block:: yaml
 
   preprocess:
-    kind: fMRIPrepConfoundRemover
-    strategy:
-      motion: full
-      wm_csf: full
-      global_signal: basic
-    spike: 0.2
-    detrend: false
-    standardize: true
+    - kind: fMRIPrepConfoundRemover
+      strategy:
+        motion: full
+        wm_csf: full
+        global_signal: basic
+      spike: 0.2
+      detrend: false
+      standardize: true
 
 
 For the ``Oasis VBM Testing dataset`` example, we will not specify a
 preprocessing step.
 
 
 Marker
 ^^^^^^
 
-The ``markers`` section diverges from the previous ones, as we need to specify
-a list of markers. Each marker has a name that we can use to refer to it later,
-and a set of parameters that will be passed to the marker.
+The ``markers`` section like the ``preprocess`` section expects a list of
+markers. Each Marker has a name that we can use to refer to it later,
+and a set of parameters that will be passed to the Marker.
 
 For the ``Oasis VBM Testing dataset`` example, we want to compute the mean
 ``VBM_GM`` value for each parcel using the ``Schaefer parcellation (100 parcels,
 7 networks)``, ``Schaefer parcellation (200 parcels, 7 networks)``, and the
 ``DMNBuckner`` network, using ``5mm`` spheres. Thus, we will configure the
 ``markers`` section as follows:
 
@@ -186,22 +187,22 @@
 Storage
 ^^^^^^^
 
 Finally, we need to define how and where the results will be stored. This is
 done using the ``storage`` section, which must be configured using the ``kind``
 key to specify the storage to use, and additional keys to pass parameters.
 
-For example, to use the :class:`.SQLiteFeatureStorage` storage, we just need to
+For example, to use the :class:`.HDF5FeatureStorage` storage, we just need to
 specify where we want to store the results:
 
 .. code-block:: yaml
 
     storage:
-      kind: SQLiteFeatureStorage
-      uri: /data/junifer/example/oasis_vbm_testing.sqlite
+      kind: HDF5FeatureStorage
+      uri: /data/junifer/example/oasis_vbm_testing.hdf5
 
 
 Complete Example
 ----------------
 
 This is how the full ``Oasis VBM Testing dataset`` example configuration file
 looks like:
@@ -227,9 +228,9 @@
     - name: DMNBuckner_5mm_mean
       kind: SphereAggregation
       coords: DMNBuckner
       radius: 5
       method: mean
 
   storage:
-    kind: SQLiteFeatureStorage
-    uri: /data/junifer/example/oasis_vbm_testing.sqlite
+    kind: HDF5FeatureStorage
+    uri: /data/junifer/example/oasis_vbm_testing.hdf5
```

### Comparing `junifer-0.0.4.dev90/docs/using/index.rst` & `junifer-0.0.5.dev11/docs/using/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .. include:: ../links.inc
 
 .. _using:
 
-Using junifer
-=============
+Using ``junifer``
+=================
 
-In this section, we will cover the main aspects behind using junifer. We will
-first explain the basics behind junifer's code-less configuration. Then we will
-show how to use the command line interface to ``run`` junifer and ``collect``
-the results. Finally, we will show how to use the ``queue`` command to interact
-with HPC and HTC systems.
+In this section, we will cover the main aspects behind using ``junifer``. We
+will first explain the basics behind junifer's code-less configuration. Then we
+will show how to use the command line interface to ``run`` the pipeline and
+``collect`` the results. Finally, we will show how to use the ``queue`` command
+to interact with HPC and HTC systems.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    codeless
    running
@@ -21,15 +21,15 @@
 
 
 .. _using_components:
 
 Using Common Components
 -----------------------
 
-The following sections explains common components of junifer that can be used
+The following sections explains common components of ``junifer`` that can be used
 across many steps of the pipeline.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    masks
```

### Comparing `junifer-0.0.4.dev90/docs/using/masks.rst` & `junifer-0.0.5.dev11/docs/using/masks.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 Masks are essentially boolean arrays that are used to constrain the extraction
 of features to voxels that are meaningful. For example, in an fMRI imaging
 study, a mask can be used to constrain the extraction of features to voxels that
 contain a certain ratio of gray matter to white matter / cerebrospinal fluid,
 ensuring that the features are not extracted from voxels that contain mostly
 white matter or cerebrospinal fluid, which could add noise to the BOLD signal.
 
-Junifer provides a number of built-in masks, which can be listed using
+``junifer`` provides a number of built-in masks, which can be listed using
 :func:`.list_masks`. Some masks are images, while other masks can be computed
 using :ref:`nilearn` functions.
 
 For markers and steps that accept ``masks`` as an argument, the mask can be
 specified as a string, which will be the name of a built-in mask, or as a
 dictionary in which the **only** key is the built-in mask name and the value is
 a dictionary of keyword arguments to pass to the mask function.
 
 For example, the following is a valid mask specification that specified the
-``GM_prob0.2`` mask.
+``GM_prob0.2`` mask:
 
 .. code-block:: yaml
 
     masks: GM_prob0.2
 
 The following is a valid mask specification that specifies the
-``compute_brain_mask``  mask (function from nilearn), with a threshold of
-``0.5``.
+``compute_brain_mask`` mask, with a threshold of ``0.5``.
 
 .. code-block:: yaml
 
     masks:
         compute_brain_mask:
             threshold: 0.5
```

### Comparing `junifer-0.0.4.dev90/docs/using/queueing.rst` & `junifer-0.0.5.dev11/docs/using/queueing.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 .. include:: ../links.inc
 
 .. _queueing:
 
 Queueing Jobs (HPC, HTC)
 ========================
 
-Yet another interesting feature of junifer is the ability to queue jobs on
+Yet another interesting feature of ``junifer`` is the ability to queue jobs on
 computational clusters. This is done by adding the ``queue`` section in the
 :ref:`codeless` file and executing the  ``junifer queue`` command.
 
 While junifer is meant to support `HTCondor`_, `SLURM`_ and local queueing
 using `GNU Parallel`_, only HTCondor is currently supported. This will be
-implemented in future releases of junifer. If you are in immediate need of any of
-these schedulers, please create an issue on the `junifer github`_ repository.
+implemented in future releases of ``junifer``. If you are in immediate need of
+any of these schedulers, please create an issue on the `junifer github`_
+repository.
 
 The ``queue`` section of the :ref:`codeless` must start by defining the
 following general parameters:
 
 * ``jobname``: Name of the job to be queued. This will be used to name the
   folder where the job files will be created, as well as any relevant file.
   Depending on the scheduler, it will also be listed in the queueing system
   with this name.
 * ``kind``: The kind of scheduler to be used. Currently, only ``HTCondor`` is
   supported.
 
-Example:
+Example in YAML:
 
 .. code-block:: yaml
 
   queue:
     jobname: TestHTCondorQueue
     kind: HTCondor
 
@@ -36,54 +37,57 @@
 The rest of the parameters depend on the scheduler you are using.
 
 .. _queueing_condor:
 
 HTCondor
 --------
 
-When using HTCondor, junifer will use a DAG to queue one job per element
+When using HTCondor, ``junifer`` will use a DAG to queue one job per element
 (``junifer run``). As an option, the DAG can include a final job
 (``junifer collect``) to collect the results once all of the individual element
 jobs are finished.
 
 The following parameters are available for HTCondor:
 
 * ``env``: Definition of the Python environment. It must provide two variables:
 
   * ``kind``: This is the kind of virtual environment to use:
 
     * ``conda``
-    * ``virtualenv`` (not yet supported)
+    * ``venv``
     * ``local`` (no virtual environment)
 
   * ``name``: This is the name of the environment to use in case a virtual
-    environment is used.
+    environment is used. It should be the name when ``conda`` is used and
+    the absolute or relative path to the virtualenv when ``venv`` is used.
+    If relative path is used then it should be relative to the YAML.
 
 * ``mem``: Memory to be used by the job. It must be provided as a string with
-  the units (e.g. ``2GB``).
-* ``cpus``: Number of CPUs to be used by the job. It must be provided as an int.
+  the units (e.g., ``"2GB"``).
+* ``cpus``: Number of CPUs to be used by the job. It must be provided as an
+  integer (e.g., ``1``).
 * ``disk``: Disk space to be used by the job. It must be provided as a string
-  with the units (e.g. ``2GB``). Keep in mind that junifer uses a local working
-  directory for each job, and datalad datasets might be cloned in this temporary
-  directory.
+  with the units (e.g., ``"2GB"``). Keep in mind that ``junifer`` uses a local
+  working directory for each job, and datalad datasets might be cloned in this
+  temporary directory.
 * ``extra_preamble``: Extra lines to be added to the HTCondor submit file. This
   can be used to add extra parameters to the job, such as ``requirements``.
 * ``collect``: This parameter allows to include a collect to the DAG to collect
   the results once all of the individual element jobs are finished. This is
   useful if you want to run a ``junifer collect`` job only once all of the
   individual element jobs are finished. Valid options are:
 
   * ``yes``: Include a collect job in the DAG that will be executed even if some
     of the individual element jobs fail.
   * ``on_success_only``: Include a collect job to the DAG, but will only run if
     all of the individual element jobs are successful.
   * ``no``: Do not include a collect job to the DAG.
 
 
-Example:
+Example in YAML:
 
 .. code-block:: yaml
 
   queue:
     jobname: TestHTCondorQueue
     kind: HTCondor
     env:
```

### Comparing `junifer-0.0.4.dev90/docs/using/running.rst` & `junifer-0.0.5.dev11/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/docs/whats_new.rst` & `junifer-0.0.5.dev11/docs/whats_new.rst`

 * *Files 25% similar despite different names*

```diff
@@ -4,16 +4,244 @@
 .. _whats_new:
 
 What's new
 ==========
 
 .. towncrier release notes start
 
+Junifer 0.0.4 (2024-04-05)
+--------------------------
+
+Bugfixes
+^^^^^^^^
+
+- Make copying of assets in ``with`` block of YAML, relative to YAML and not to
+  current working directory by `Fede Raimondo`_ and `Synchon Mandal`_
+  (:gh:`224`)
+- Adapt ``junifer queue`` to properly use HTCondor >=10.4.0
+  ``condor_submit_dag`` by `Fede Raimondo`_ and `Synchon Mandal`_ (:gh:`233`)
+- Use 1 instead of 0 for successful FSL commands in ``_check_fsl()`` by
+  `Synchon Mandal`_ (:gh:`272`)
+- Store native warped parcellations, coordinates and masks in element-scoped
+  tempdirs for the pipeline to work by `Synchon Mandal`_ (:gh:`274`)
+- Change interpolation scheme for parcel and mask native space transformation
+  to nearest neighbour by `Synchon Mandal`_ (:gh:`276`)
+- Bypass FSL ``std2imgcoord`` stdin bug and use recommended piped input for
+  coordinates transformation by `Synchon Mandal`_ (:gh:`278`)
+- Add ``-std`` to FSL ``std2imgcoord`` for coordinates transformation by
+  `Synchon Mandal`_ (:gh:`280`)
+- Replace FSL ``std2imgcoord`` with ``img2imgcoord`` as the former is incorrect
+  for coordinates transformation to other template spaces. (:gh:`281`)
+- Propagate ReHo and fALFF maps, for aggregation to convert to other template
+  spaces when required by `Synchon Mandal`_ (:gh:`282`)
+- Allow :class:`junifer.pipeline.WorkDirManager` to accept str via the
+  ``workdir`` parameter by `Synchon Mandal`_ (:gh:`283`)
+- Avoid warping mask preprocessed with :class:`.fMRIPrepConfoundRemover` and
+  used by markers with ``mask="inherit"`` in subject-native template space by
+  `Fede Raimondo`_ and `Synchon Mandal`_ (:gh:`284`)
+- Pass down input path if input space is "native" for ``ReHoEstimator`` and
+  ``ALFFEstimator``, else use respective compute maps by `Fede Raimondo`_ and
+  `Synchon Mandal`_ (:gh:`286`)
+- Fix :class:`.HTCondorAdapter`'s script generation to use double quotes
+  instead of single quotes for HTCondor's ``VARS`` by `Synchon Mandal`_
+  (:gh:`312`)
+- Fix element access for :class:`.DMCC13Benchmark` DataGrabber by `Synchon
+  Mandal`_ (:gh:`314`)
+- Add a validation step on the :func:`.run` function to validate the marker
+  collection by `Fede Raimondo`_ (:gh:`320`)
+- Add the executable flag to the ants docker scripts, fsl docker scripts and
+  other running scripts by `Fede Raimondo`_ (:gh:`321`)
+- Force ``str`` dtype when parsing elements from file by `Synchon Mandal`_
+  (:gh:`322`)
+
+
+API Changes
+^^^^^^^^^^^
+
+- Rename ``Power`` coordinates to ``Power2011`` by `Synchon Mandal`_
+  (:gh:`245`)
+- Add ``feature_md5`` argument to :func:`.read_transform()` by `Synchon
+  Mandal`_ (:gh:`248`)
+- Add ``native_t1w`` parameter to :class:`.DataladAOMICID1000`,
+  :class:`.DataladAOMICPIOP1`, :class:`.DataladAOMICPIOP2`, enabling fetching
+  of T1w data in subject-native space by `Synchon Mandal`_ (:gh:`252`)
+- Modify ``preprocessor`` to ``preprocessors`` in :func:`.run` and
+  ``preprocessing`` to ``preprocessors`` in :class:`.MarkerCollection` to
+  accept multiple preprocessors by `Synchon Mandal`_ (:gh:`263`)
+- Add ``space`` parameter to :func:`.register_coordinates`,
+  :func:`.register_parcellation` and :func:`.register_mask` and return space
+  from :func:`.load_coordinates`, :func:`.load_parcellation` and
+  :func:`.load_mask` by `Synchon Mandal`_ and `Fede Raimondo`_ (:gh:`268`)
+- Add ``template_type`` parameter to :func:`.get_template` by `Synchon Mandal`_
+  (:gh:`299`)
+- Change :meth:`.BasePreprocessor.preprocess` return values to preprocessed
+  target data and "helper" data types as a dictionary by `Synchon Mandal`_
+  (:gh:`310`)
+- Add a positional argument ``using`` for Markers and Preprocessors having
+  implementation-based variations, in particular :class:`.ReHoParcels`,
+  :class:`.ReHoSpheres`, :class:`.ALFFParcels`, :class:`.ALFFSpheres` and
+  :class:`.BOLDWarper` by `Synchon Mandal`_ (:gh:`311`)
+- Change all ``probseg_`` types to ``VBM_`` types by `Fede Raimondo`_
+  (:gh:`320`)
+- Change the subject and session patterns for :class:`.DataladAOMICID1000`,
+  :class:`.DataladAOMICPIOP1`, :class:`.DataladAOMICPIOP2` and
+  :class:`.DMCC13Benchmark` so that they are consistent with their own
+  ``"participants.tsv"`` file by `Fede Raimondo`_ (:gh:`325`)
+
+
+Improved Documentation
+^^^^^^^^^^^^^^^^^^^^^^
+
+- Add Zenodo badge in ``README`` and improve general documentation by `Synchon
+  Mandal`_ (:gh:`247`)
+- Rename ``extMDN`` to ``extDMN`` (extended default mode network) and fix
+  listing for ``eMDN`` (extended multiple-demand network) by `Synchon Mandal`_
+  (:gh:`251`)
+- Fixed typo in code example for adding masks from "register_custom_mask" to
+  "register_mask" by `Tobias Muganga`_ (:gh:`291`)
+- Rename ``Misc`` section to ``Miscellaneous`` in ``docs/whats_new.rst`` by
+  `Synchon Mandal`_ (:gh:`300`)
+- Improve documentation by adding information about space transformation and
+  writing custom Preprocessors by `Synchon Mandal`_ (:gh:`317`)
+
+
+Enhancements
+^^^^^^^^^^^^
+
+- Support element(s) to be specified via text file for ``--element`` option of
+  ``junifer run`` by `Synchon Mandal`_ (:gh:`182`)
+- Support element-scoped directory and temporary directories for
+  :class:`junifer.pipeline.WorkDirManager` by `Synchon Mandal`_ (:gh:`258`)
+- Improve element directory cleanup via
+  ``junifer.pipeline.WorkDirManager.cleanup_elementdir`` method by `Synchon
+  Mandal`_ (:gh:`259`)
+- Improve :class:`.BasePreprocessor` for easy subclassing and adapt
+  :class:`.fMRIPrepConfoundRemover` to it by `Synchon Mandal`_ (:gh:`260`)
+- Add ``space`` information to existing datagrabbers, masks, parcellations and
+  coordinates by `Synchon Mandal`_ and `Fede Raimondo`_ (:gh:`268`)
+- Add ``mode`` as an aggregation function option in
+  :func:`.get_aggfunc_by_name` by `Synchon Mandal`_ (:gh:`287`)
+- Adapt :class:`.BOLDWarper` to use FSL or ANTs depending on warp file
+  extension by `Synchon Mandal`_ (:gh:`293`)
+- Rewrite :func:`.compute_brain_mask` to allow variable template fetching via
+  templateflow, according to target data by `Synchon Mandal`_ (:gh:`299`)
+- Replace ``requests`` with ``httpx`` for fetching parcellations by `Synchon
+  Mandal`_ (:gh:`300`)
+- Allow :class:`.BOLDWarper` to warp BOLD data to other MNI spaces by `Synchon
+  Mandal`_ (:gh:`302`)
+- Add support for local ``junifer queue`` via GNU Parallel by `Synchon Mandal`_
+  (:gh:`306`)
+- Improve :class:`.PatternDataGrabber` and
+  :class:`.PatternDataladDataGrabber`'s ``patterns`` to enable ``space``,
+  ``format``, ``mask_item`` and other metadata description handling via YAML by
+  `Synchon Mandal`_ (:gh:`308`)
+- Improve :class:`.BasePreprocessor` by revamping
+  :meth:`.BasePreprocessor.preprocess` and ``BasePreprocessor._fit_transform``
+  to handle "helper" data types better and make the pipeline explicit where
+  data is being altered by `Synchon Mandal`_ (:gh:`310`)
+- Improve external dependency handling for :class:`.PipelineStepMixin`-derived
+  objects having implementation-based variations by `Synchon Mandal`_
+  (:gh:`311`)
+
+
+Features
+^^^^^^^^
+
+- Introduce complexity markers: :class:`.HurstExponent`,
+  :class:`.MultiscaleEntropyAUC`, :class:`.PermEntropy`,
+  :class:`.RangeEntropy`, :class:`.RangeEntropyAUC` and :class:`.SampleEntropy`
+  by `Amir Omidvarnia`_ (:gh:`145`)
+- Add ``junifer reset`` to reset storage and jobs directory by `Synchon
+  Mandal`_ (:gh:`240`)
+- Add support for ``Power2013`` coordinates by `Synchon Mandal`_ (:gh:`245`)
+- Support ``venv`` as environment kind for queueing jobs by `Synchon Mandal`_
+  (:gh:`249`)
+- Add support for ``AutobiographicalMemory`` coordinates by `Synchon Mandal`_
+  (:gh:`250`)
+- Add support for subject-native space by `Synchon Mandal`_ and `Fede
+  Raimondo`_ (:gh:`252`)
+- Introduce :class:`junifer.pipeline.WorkDirManager` singleton class to manage
+  working and temporary directories across pipeline by `Synchon Mandal`_
+  (:gh:`254`)
+- Introduce :func:`.get_parcellation` to fetch parcellation tailored for the
+  data by `Synchon Mandal`_ (:gh:`264`)
+- Introduce :func:`.get_coordinates` to fetch coordinates tailored for the data
+  by `Synchon Mandal`_ (:gh:`265`)
+- Introduce ``junifer.preprocess.fsl.apply_warper._ApplyWarper`` to wrap FSL's
+  ``applywarp`` by `Synchon Mandal`_ (:gh:`266`)
+- Introduce :class:`.BOLDWarper` for warping BOLD data via FSL's ``applywarp``
+  by `Synchon Mandal`_ (:gh:`267`)
+- Introduce :class:`.DMCC13Benchmark` to access `DMCC13benchmark dataset
+  <https://openneuro.org/datasets/ds003452/versions/1.0.1>`_ by `Synchon
+  Mandal`_ (:gh:`271`)
+- Add ``Brainnetome 246`` parcellation to ``junifer.data`` by `Synchon Mandal`_
+  (:gh:`275`)
+- Introduce
+  ``junifer.preprocess.ants.ants_apply_transforms_warper._AntsApplyTransformsWarper``
+  to wrap ANTs' ``antsApplyTransforms`` by `Synchon Mandal`_ (:gh:`293`)
+- Introduce :func:`.run_ext_cmd` to take care of the boilerplate code for
+  running external commands from FSL, ANTs and others by `Synchon Mandal`_
+  (:gh:`295`)
+- Introduce :func:`.get_xfm` to fetch transformation files for moving between
+  template spaces by `Synchon Mandal`_ (:gh:`297`)
+- Introduce :func:`.get_template` to fetch template space image tailored to a
+  target data by `Synchon Mandal`_ (:gh:`298`)
+- Add support for on-the-fly template space transformation in
+  :func:`.get_parcellation` and :func:`.get_mask` to allow parcellation and
+  mask in different template spaces to work with a ``DataGrabber``'s data in a
+  specified template space. (:gh:`299`)
+- Introduce :class:`.SpaceWarper` for warping ``T1w``, ``BOLD``, ``VBM_GM``,
+  ``VBM_WM``, ``fALFF``, ``GCOR`` and ``LCOR`` data to other spaces by `Synchon
+  Mandal`_ (:gh:`301`)
+- Introduce :class:`.QueueContextAdapter` as an abstract base class for job
+  queueing and :class:`.HTCondorAdapter` as its implementation for HTCondor by
+  `Synchon Mandal`_ (:gh:`309`)
+
+
+Miscellaneous
+^^^^^^^^^^^^^
+
+- Update dependencies requirements by `Fede Raimondo`_ (:gh:`253`)
+- Pin ``ruff`` to ``0.1.0`` as the lowest version and update ``pre-commit``
+  config by `Synchon Mandal`_ (:gh:`261`)
+- Add support for accessing FSL via Docker wrapper along with ``flirt``,
+  ``applywarp``  and ``std2imgcoord`` commands by `Synchon Mandal`_ (:gh:`262`)
+- Improve documentation, packaging and code style by `Synchon Mandal`_
+  (:gh:`269`)
+- Add support for Python 3.12 and make Python 3.11 the base for code coverage
+  and CI checks by `Synchon Mandal`_ (:gh:`270`)
+- Add support for accessing ANTs via Docker wrapper along with
+  ``antsApplyTransforms`` and ``antsApplyTransformsToPoints`` by `Synchon
+  Mandal`_ (:gh:`277`)
+- Make the external tool wrappers output to stderr instead of stdout by
+  `Synchon Mandal`_ (:gh:`279`)
+- Add support for accessing FSL ``img2imgcoord`` via Docker wrapper command by
+  `Synchon Mandal`_ (:gh:`281`)
+- Make :class:`.BOLDWarper` tool-agnostic by moving it from
+  ``junifer.preprocess.fsl`` to :mod:`junifer.preprocess` by `Synchon Mandal`_
+  (:gh:`288`)
+- Add support for accessing ANTs' ``ResampleImage`` via Docker wrapper by
+  `Synchon Mandal`_ (:gh:`293`)
+- Update ``pyproject.toml`` and add FAIR shield in ``README.md`` by `Synchon
+  Mandal`_ (:gh:`294`)
+- Update dependency listing in ``pyproject.toml``, add
+  ``.github/dependabot.yml`` to auto-update GitHub Actions, add ``ANTs`` and
+  ``FSL`` installation in CI and improve general code style by `Synchon
+  Mandal`_ (:gh:`300`)
+
+
+Deprecations and Removals
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+- Deprecate :class:`.BOLDWarper` and mark for removal in v0.0.4 by `Synchon
+  Mandal`_ (:gh:`301`)
+
+
 Junifer 0.0.3 (2023-07-21)
----------------------------------
+--------------------------
 
 Bugfixes
 ^^^^^^^^
 
 - Enable YAML 1.2 support and allow multiline strings in YAML which would not
   work earlier by `Synchon Mandal`_ (:gh:`223`)
 - Handle ``datalad.IncompleteResultsError`` exception for partial clone in
@@ -72,16 +300,16 @@
   ``junifer.data`` by `Synchon Mandal`_ (:gh:`184`)
 - Add ``Yan 2023`` parcellation to ``junifer.data`` by `Synchon Mandal`_
   (:gh:`225`)
 - Introduce :mod:`.onthefly` sub-module and :func:`.read_transform` for quick
   transform operations on stored data by `Synchon Mandal`_ (:gh:`237`)
 
 
-Misc
-^^^^
+Miscellaneous
+^^^^^^^^^^^^^
 
 - Consistent docstrings for pytest fixtures used in the test suite by `Synchon
   Mandal`_ (:gh:`228`)
 - Adopt ``ruff`` as the only linter for the codebase by `Synchon Mandal`_
   (:gh:`229`)
 - Improve ``codespell`` support by fixing typos in documentation by `Synchon
   Mandal`_ (:gh:`230`)
@@ -369,11 +597,11 @@
 - Implement :class:`.ReHoParcels` and :class:`.ReHoSpheres` markers by
   `Synchon Mandal`_ (:gh:`36`)
 
 - Implement :class:`.ALFFParcels` and :class:`.ALFFSpheres` markers by
   `Fede Raimondo`_ (:gh:`35`)
 
 
-Misc
-^^^^
+Miscellaneous
+^^^^^^^^^^^^^
 
 - Create the repository based on the mockup by `Fede Raimondo`_
```

### Comparing `junifer-0.0.4.dev90/examples/norun_hcpfc_pearson.py` & `junifer-0.0.5.dev11/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/norun_ukbvm_gmd.py` & `junifer-0.0.5.dev11/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.5.dev11/examples/run_datagrabber_bids_datalad.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 ###############################################################################
 # The BIDS DataGrabber requires three parameters: the types of data we want,
 # the specific pattern that matches each type, and the variables that will be
 # replaced in the patterns.
 types = ["T1w", "BOLD"]
 patterns = {
-    "T1w": "{subject}/anat/{subject}_T1w.nii.gz",
-    "BOLD": "{subject}/func/{subject}_task-rest_bold.nii.gz",
+    "T1w": {
+        "pattern": "{subject}/anat/{subject}_T1w.nii.gz",
+        "space": "native",
+    },
+    "BOLD": {
+        "pattern": "{subject}/func/{subject}_task-rest_bold.nii.gz",
+        "space": "MNI152NLin6Asym",
+    },
 }
 replacements = ["subject"]
 ###############################################################################
 # Additionally, a datalad-based DataGrabber requires the URI of the remote
 # sibling and the location of the dataset within the remote sibling.
 repo_uri = "https://gin.g-node.org/juaml/datalad-example-bids"
 rootdir = "example_bids"
```

### Comparing `junifer-0.0.4.dev90/examples/run_ets_rss_marker.py` & `junifer-0.0.5.dev11/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/run_junifer_julearn.py` & `junifer-0.0.5.dev11/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/run_run_gmd_mean.py` & `junifer-0.0.5.dev11/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/yamls/gmd_mean.yaml` & `junifer-0.0.5.dev11/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.5.dev11/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/api/cli.py` & `junifer-0.0.5.dev11/junifer/api/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     configure_logging,
     logger,
     raise_error,
     warn_with_log,
 )
 from .functions import collect as api_collect
 from .functions import queue as api_queue
+from .functions import reset as api_reset
 from .functions import run as api_run
 from .parser import parse_yaml
 from .utils import (
     _get_dependency_information,
     _get_environment_information,
     _get_junifer_version,
     _get_python_information,
@@ -109,22 +110,21 @@
 
     """
     # Read CSV into dataframe
     csv_df = pd.read_csv(
         filepath,
         header=None,  # no header  # type: ignore
         index_col=False,  # no index column
+        dtype=str,
         skipinitialspace=True,  # no leading space after delimiter
     )
     # Remove trailing whitespace in cell entries
-    csv_df_trimmed = csv_df.apply(
-        lambda x: x.str.strip() if x.dtype == "object" else x
-    )
+    csv_df_trimmed = csv_df.apply(lambda x: x.str.strip())
     # Convert to list of tuple of str
-    return list(map(tuple, csv_df_trimmed.to_numpy().astype(str)))
+    return list(map(tuple, csv_df_trimmed.to_numpy()))
 
 
 def _validate_verbose(
     ctx: click.Context, param: str, value: str
 ) -> Union[str, int]:
     """Validate verbose option.
 
@@ -137,14 +137,15 @@
     value : str
         The value to validate.
 
     Returns
     -------
     str or int
         The validated value.
+
     """
     if isinstance(value, int):
         return value
 
     valid_strings = ["error", "warning", "info", "debug"]
     if isinstance(value, str) and value.lower() in valid_strings:
         return value.upper()
@@ -196,29 +197,39 @@
     element : tuple of str
         The element to operate on.
     verbose : click.Choice
         The verbosity level: warning, info or debug (default "info").
 
     """
     configure_logging(level=verbose)
-    # TODO: add validation
+    # TODO(synchon): add validation
+    # Parse YAML
     config = parse_yaml(filepath)  # type: ignore
+    # Retrieve working directory
     workdir = config["workdir"]
+    # Fetch datagrabber
     datagrabber = config["datagrabber"]
+    # Fetch markers
     markers = config["markers"]
+    # Fetch storage
     storage = config["storage"]
-    preprocessor = config.get("preprocess")
+    # Fetch preprocessors
+    preprocessors = config.get("preprocess")
+    # Convert to list if single preprocessor
+    if preprocessors is not None and not isinstance(preprocessors, list):
+        preprocessors = [preprocessors]
+    # Parse elements
     elements = _parse_elements(element, config)
     # Perform operation
     api_run(
         workdir=workdir,
         datagrabber=datagrabber,
         markers=markers,
         storage=storage,
-        preprocessor=preprocessor,
+        preprocessors=preprocessors,
         elements=elements,
     )
 
 
 @cli.command()
 @click.argument(
     "filepath",
@@ -399,14 +410,51 @@
 
     if completed_process.returncode == 0:
         click.secho("Successful.", fg="green")
     else:
         click.secho("Failure.", fg="red")
 
 
+@cli.command()
+@click.argument(
+    "filepath",
+    type=click.Path(
+        exists=True, readable=True, dir_okay=False, path_type=pathlib.Path
+    ),
+)
+@click.option(
+    "-v",
+    "--verbose",
+    type=click.UNPROCESSED,
+    callback=_validate_verbose,
+    default="info",
+)
+def reset(
+    filepath: click.Path,
+    verbose: Union[str, int],
+) -> None:
+    """Reset command for CLI.
+
+    \f
+
+    Parameters
+    ----------
+    filepath : click.Path
+        The filepath to the configuration file.
+    verbose : click.Choice
+        The verbosity level: warning, info or debug (default "info").
+
+    """
+    configure_logging(level=verbose)
+    # Parse YAML
+    config = parse_yaml(filepath)
+    # Perform operation
+    api_reset(config)
+
+
 @cli.group()
 def setup() -> None:  # pragma: no cover
     """Configure commands for Junifer."""
     pass
 
 
 @setup.command("afni-docker")
@@ -426,7 +474,53 @@
         docker pull afni/afni
 
     3. Add this line to the ~/.bashrc or ~/.zshrc file:
 
     export PATH="$PATH:{afni_wrappers_path}"
     """
     click.secho(msg, fg="blue")
+
+
+@setup.command("fsl-docker")
+def fsl_docker() -> None:  # pragma: no cover
+    """Configure FSL-Docker wrappers."""
+    import junifer
+
+    pkg_path = Path(junifer.__path__[0])  # type: ignore
+    fsl_wrappers_path = pkg_path / "api" / "res" / "fsl"
+    msg = f"""
+    Installation instructions for FSL-Docker wrappers:
+
+    1. Install Docker: https://docs.docker.com/get-docker/
+
+    2. Get the FSL-Docker image by running this on the command line:
+
+        docker pull brainlife/fsl
+
+    3. Add this line to the ~/.bashrc or ~/.zshrc file:
+
+    export PATH="$PATH:{fsl_wrappers_path}"
+    """
+    click.secho(msg, fg="blue")
+
+
+@setup.command("ants-docker")
+def ants_docker() -> None:  # pragma: no cover
+    """Configure ANTs-Docker wrappers."""
+    import junifer
+
+    pkg_path = Path(junifer.__path__[0])  # type: ignore
+    ants_wrappers_path = pkg_path / "api" / "res" / "ants"
+    msg = f"""
+    Installation instructions for ANTs-Docker wrappers:
+
+    1. Install Docker: https://docs.docker.com/get-docker/
+
+    2. Get the ANTs-Docker image by running this on the command line:
+
+        docker pull antsx/ants
+
+    3. Add this line to the ~/.bashrc or ~/.zshrc file:
+
+    export PATH="$PATH:{ants_wrappers_path}"
+    """
+    click.secho(msg, fg="blue")
```

### Comparing `junifer-0.0.4.dev90/junifer/api/decorators.py` & `junifer-0.0.5.dev11/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/api/parser.py` & `junifer-0.0.5.dev11/junifer/api/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -46,14 +46,16 @@
             )
     # load modules
     if "with" in contents:
         to_load = contents["with"]
         # Convert load modules to list
         if not isinstance(to_load, list):
             to_load = [to_load]
+        # Initialize list to have absolute paths for custom modules
+        final_to_load = []
         for t_module in to_load:
             if t_module.endswith(".py"):
                 logger.debug(f"Importing file: {t_module}")
                 # This resolves both absolute and relative paths
                 file_path = filepath.parent / t_module
                 if not file_path.exists():
                     raise_error(
@@ -61,17 +63,26 @@
                     )
                 spec = importlib.util.spec_from_file_location(
                     t_module, file_path
                 )
                 module = importlib.util.module_from_spec(spec)  # type: ignore
                 sys.modules[t_module] = module
                 spec.loader.exec_module(module)  # type: ignore
+                # Add absolute path to final list
+                final_to_load.append(str(file_path.resolve()))
             else:
                 logger.info(f"Importing module: {t_module}")
                 importlib.import_module(t_module)
+                # Add module to final list
+                final_to_load.append(t_module)
+
+        # Replace modules to be loaded so that custom modules will take the
+        # absolute path. This was not the case as found in #224. Similar thing
+        # is done with the storage URI below.
+        contents["with"] = final_to_load
 
     # Compute path for the URI parameter in storage files that are relative
     # This is a tricky thing that appeared in #127. The problem is that
     # the path in the URI parameter is relative to YAML file, not to the
     # current working directory. If we leave it as is in the contents
     # dict, then it will be used later in the ``build`` function as is,
     # which will be computed relative to the current working directory.
@@ -84,8 +95,21 @@
             # Check if the storage file is relative
             uri_path = Path(contents["storage"]["uri"])
             if not uri_path.is_absolute():
                 # Compute the absolute path
                 contents["storage"]["uri"] = str(
                     (filepath.parent / uri_path).resolve()
                 )
+
+    # Allow relative path if queue env kind is venv; same motivation as above
+    if "queue" in contents:
+        if "env" in contents["queue"]:
+            if "venv" == contents["queue"]["env"]["kind"]:
+                # Check if the env name is relative
+                venv_path = Path(contents["queue"]["env"]["name"])
+                if not venv_path.is_absolute():
+                    # Compute the absolute path
+                    contents["queue"]["env"]["name"] = str(
+                        (filepath.parent / venv_path).resolve()
+                    )
+
     return contents
```

### Comparing `junifer-0.0.4.dev90/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.5.dev11/junifer/api/res/ants/run_ants_docker.sh`

 * *Files 16% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 corrected_args=()
 docker_args=()
 mounts=0
 for var in "$@"
 do
 if [ -d "${var}" ]; then
-        echo "$var is a directory"
+        echo "$var is a directory" >&2
         var=$(realpath "${var}")
         host_dir=$(dirname "${var}")
         ((mounts+=1))
         container_dir="/data/mount_${mounts}"
         docker_args+=("-v ${host_dir}:${container_dir}")
         var=${container_dir}
     elif [ -f "${var}" ] || [[ "${var}" == /* ]]; then
         if [ -f "${var}" ]; then
-            echo "$var is a file"
+            echo "$var is a file" >&2
             var=$(realpath "${var}")
         else
-            echo "$var is a prefix"
+            echo "$var is a prefix" >&2
         fi
         fname=$(basename "${var}")
         host_dir=$(dirname "${var}")
         ((mounts+=1))
         container_dir="/data/mount_${mounts}"
         docker_args+=("-v ${host_dir}:${container_dir}")
         var=${container_dir}/${fname}
     fi
     corrected_args+=("${var}")
 done
 
-echo "Docker args: ${docker_args[*]}"
-echo "Corrected args for afni: ${corrected_args[*]}"
+echo "Docker args: ${docker_args[*]}" >&2
+echo "Corrected args for fsl: ${corrected_args[*]}" >&2
 
 cwd=$(pwd)
-cmd="docker run --rm ${docker_args[*]} -v ${cwd}:${cwd} -w ${cwd} afni/afni_make_build ${corrected_args[*]}"
-echo "Running command: ${cmd}"
+cmd="docker run --rm ${docker_args[*]} -v ${cwd}:${cwd} -w ${cwd} antsx/ants ${corrected_args[*]}"
+echo "Running command: ${cmd}" >&2
 ${cmd}
```

### Comparing `junifer-0.0.4.dev90/junifer/api/tests/test_api_utils.py` & `junifer-0.0.5.dev11/junifer/api/tests/test_api_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,40 +28,58 @@
     assert python_information["version"] == pl.python_version()
     assert python_information["implementation"] == pl.python_implementation()
 
 
 def test_get_dependency_information_short() -> None:
     """Test short version of _get_dependency_information()."""
     dependency_information = _get_dependency_information(long_=False)
-    assert list(dependency_information.keys()) == [
+    dependency_list = [
         "click",
         "numpy",
+        "scipy",
         "datalad",
         "pandas",
         "nibabel",
         "nilearn",
         "sqlalchemy",
         "ruamel.yaml",
+        "httpx",
+        "tqdm",
+        "templateflow",
+        "looseversion",
     ]
 
+    python_minor_version = int(pl.python_version_tuple()[1])
+    if python_minor_version < 10:
+        dependency_list.append("importlib_metadata")
+
+    assert frozenset(dependency_information.keys()) == frozenset(
+        dependency_list
+    )
+
 
 def test_get_dependency_information_long() -> None:
     """Test long version of _get_dependency_information()."""
     dependency_information = _get_dependency_information(long_=True)
     dependency_information_keys = list(dependency_information.keys())
-    for key in [
+    dependency_list = [
         "click",
         "numpy",
+        "scipy",
         "datalad",
         "pandas",
         "nibabel",
         "nilearn",
         "sqlalchemy",
         "ruamel.yaml",
-    ]:
+        "httpx",
+        "tqdm",
+        "templateflow",
+    ]
+    for key in dependency_list:
         assert key in dependency_information_keys
 
 
 def test_get_system_information() -> None:
     """Test _get_system_information()."""
     system_information = _get_system_information()
     assert system_information["platform"] == pl.platform()
```

### Comparing `junifer-0.0.4.dev90/junifer/api/tests/test_parser.py` & `junifer-0.0.5.dev11/junifer/api/tests/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     fname = tmp_path / "test_parse_yaml_with_single_module_autoload.yaml"
     fname.write_text("foo: bar\nwith: numpy")
     # Check test file
     contents = parse_yaml(fname)
     assert "foo" in contents
     assert contents["foo"] == "bar"
     assert "with" in contents
-    assert contents["with"] == "numpy"
+    assert contents["with"] == ["numpy"]
     assert "numpy" in sys.modules
     assert "junifer.configs.wrong_config" not in sys.modules
 
 
 def test_parse_yaml_failure_with_multi_module_autoload(tmp_path: Path) -> None:
     """Test YAML parsing with multi module autoload failure.
```

### Comparing `junifer-0.0.4.dev90/junifer/api/utils.py` & `junifer-0.0.5.dev11/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     """
 
     def __init__(self, datadir: Union[str, Path, None] = None) -> None:
         uri = "https://gin.g-node.org/felixh/ds003097_ReproVBM"
         types = ["VBM_GM"]
         replacements = ["subject"]
         patterns = {
-            "VBM_GM": "sub-{subject}/mri/mwp1sub-{subject}_run-2_T1w.nii.gz",
+            "VBM_GM": {
+                "pattern": ("{subject}/mri/mwp1{subject}_run-2_T1w.nii.gz"),
+                "space": "IXI549Space",
+            },
         }
         super().__init__(
             types=types,
             datadir=datadir,
             uri=uri,
             replacements=replacements,
             patterns=patterns,
```

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-"""Provide concrete implementation for CamCAN VBM DataGrabber."""
+"""Provide concrete implementation for UKB VBM DataGrabber."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 from typing import Union
 
 from ....api.decorators import register_datagrabber
 from ....datagrabber import PatternDataladDataGrabber
 
 
 @register_datagrabber
-class JuselessDataladCamCANVBM(PatternDataladDataGrabber):
-    """Concrete implementation for Juseless CamCAN VBM data fetching.
+class JuselessDataladUKBVBM(PatternDataladDataGrabber):
+    """Concrete implementation for Juseless UKB VBM data fetching.
 
-    Implements a DataGrabber to access the CamCAN VBM data in Juseless.
+    Implements a DataGrabber to access the UKB VBM data in Juseless.
 
     Parameters
     ----------
     datadir : str or pathlib.Path or None, optional
         The directory where the datalad dataset will be cloned. If None,
         the datalad dataset will be cloned into a temporary directory
         (default None).
 
     """
 
     def __init__(self, datadir: Union[str, Path, None] = None) -> None:
-        uri = (
-            "ria+http://cat_12.5.ds.inm7.de"
-            "#a139b26a-8406-11ea-8f94-a0369f287950"
-        )
+        uri = "ria+http://ukb.ds.inm7.de#~cat_m0wp1"
+        rootdir = "m0wp1"
         types = ["VBM_GM"]
-        replacements = ["subject"]
-        patterns = {"VBM_GM": "sub-{subject}/mri/m0wp1sub-{subject}.nii.gz"}
+        replacements = ["subject", "session"]
+        patterns = {
+            "VBM_GM": {
+                "pattern": "m0wp1{subject}_ses-{session}_T1w.nii.gz",
+                "space": "IXI549Space",
+            },
+        }
         super().__init__(
             types=types,
             datadir=datadir,
             uri=uri,
+            rootdir=rootdir,
             replacements=replacements,
             patterns=patterns,
         )
```

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
         uri = (
             "ria+http://cat_12.5.ds.inm7.de"
             "#b7107c52-8408-11ea-89c6-a0369f287950"
         )
         types = ["VBM_GM"]
         replacements = ["site", "subject"]
         patterns = {
-            "VBM_GM": "{site}/sub-{subject}/mri/m0wp1sub-{subject}.nii.gz"
+            "VBM_GM": {
+                "pattern": ("{site}/{subject}/mri/m0wp1{subject}.nii.gz"),
+                "space": "IXI549Space",
+            },
         }
 
         # validate and/or transform 'site' input
         all_sites = ["HH", "Guys", "IOP"]
         if sites is None:
             sites = all_sites
```

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,36 +25,36 @@
         test_element = all_elements[0]
         out = dg[test_element]
 
         types = [
             "BOLD",
             "BOLD_confounds",
             "T1w",
-            "probseg_CSF",
-            "probseg_GM",
-            "probseg_WM",
+            "VBM_CSF",
+            "VBM_GM",
+            "VBM_WM",
         ]
 
         for t in types:
             assert t in out
             assert out[t]["path"].exists()
 
 
 @pytest.mark.parametrize(
     "types",
     [
         "BOLD",
         "BOLD_confounds",
         "T1w",
-        "probseg_CSF",
-        "probseg_GM",
-        "probseg_WM",
+        "VBM_CSF",
+        "VBM_GM",
+        "VBM_WM",
         ["BOLD", "BOLD_confounds"],
-        ["T1w", "probseg_CSF"],
-        ["probseg_GM", "probseg_WM"],
+        ["T1w", "VBM_CSF"],
+        ["VBM_GM", "VBM_WM"],
         ["BOLD", "T1w"],
     ],
 )
 def test_JuselessUCLA_partial_data_access(
     types: Union[str, List[str]],
 ) -> None:
     """Test JuselessUCLA DataGrabber partial data access.
```

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.5.dev11/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     Implements a DataGrabber to access the UCLA data in Juseless.
 
     Parameters
     ----------
     datadir : str or Path, optional
         The directory where the dataset is stored.
         (default "/data/project/psychosis_thalamus/data/fmriprep").
-    types: {"BOLD", "BOLD_confounds", "T1w", "probseg_CSF", "probseg_GM", \
-           "probseg_WM"} or a list of the options, optional
+    types: {"BOLD", "BOLD_confounds", "T1w", "VBM_CSF", "VBM_GM", \
+           "VBM_WM"} or a list of the options, optional
         UCLA data types. If None, all available data types are selected.
         (default None).
     tasks : {"rest", "bart", "bht", "pamenc", "pamret", \
             "scap", "taskswitch", "stopsignal"} or \
             list of the options or None, optional
         UCLA task sessions. If None, all available task sessions are
         selected (default None).
@@ -66,38 +66,56 @@
                 if t not in all_tasks:
                     raise_error(
                         f"{t} is not a valid task in the UCLA dataset!"
                     )
         self.tasks = tasks
         # The patterns
         patterns = {
-            "BOLD": (
-                "sub-{subject}/func/sub-{subject}_task-{task}_bold_space-"
-                "MNI152NLin2009cAsym_preproc.nii.gz"
-            ),
-            "BOLD_confounds": (
-                "sub-{subject}/func/sub-{subject}_"
-                "task-{task}_bold_confounds.tsv"
-            ),
-            "T1w": (
-                "sub-{subject}/anat/sub-{subject}_"
-                "T1w_space-MNI152NLin2009cAsym_preproc.nii.gz"
-            ),
-            "probseg_CSF": (
-                "sub-{subject}/anat/sub-{subject}_T1w_space-"
-                "MNI152NLin2009cAsym_class-CSF_probtissue.nii.gz"
-            ),
-            "probseg_GM": (
-                "sub-{subject}/anat/sub-{subject}_T1w_space-"
-                "MNI152NLin2009cAsym_class-GM_probtissue.nii.gz"
-            ),
-            "probseg_WM": (
-                "sub-{subject}/anat/sub-{subject}_T1w_space"
-                "-MNI152NLin2009cAsym_class-WM_probtissue.nii.gz"
-            ),
+            "BOLD": {
+                "pattern": (
+                    "{subject}/func/{subject}_task-{task}_bold_space-"
+                    "MNI152NLin2009cAsym_preproc.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "BOLD_confounds": {
+                "pattern": (
+                    "{subject}/func/{subject}_"
+                    "task-{task}_bold_confounds.tsv"
+                ),
+                "space": "fmriprep",
+            },
+            "T1w": {
+                "pattern": (
+                    "{subject}/anat/{subject}_"
+                    "T1w_space-MNI152NLin2009cAsym_preproc.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_CSF": {
+                "pattern": (
+                    "{subject}/anat/{subject}_T1w_space-"
+                    "MNI152NLin2009cAsym_class-CSF_probtissue.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_GM": {
+                "pattern": (
+                    "{subject}/anat/{subject}_T1w_space-"
+                    "MNI152NLin2009cAsym_class-GM_probtissue.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_WM": {
+                "pattern": (
+                    "{subject}/anat/{subject}_T1w_space"
+                    "-MNI152NLin2009cAsym_class-WM_probtissue.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
         }
         # Set default types
         if types is None:
             types = list(patterns.keys())
         # Convert single type into list
         else:
             if not isinstance(types, list):
```

### Comparing `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.5.dev11/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.5.dev11/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.5.dev11/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.5.dev11/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.5.dev11/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.5.dev11/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/data/parcellations.py` & `junifer-0.0.5.dev11/junifer/data/parcellations.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,141 +5,161 @@
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import io
 import shutil
 import tarfile
 import tempfile
+import typing
 import zipfile
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
+import httpx
 import nibabel as nib
 import numpy as np
 import pandas as pd
-import requests
 from nilearn import datasets, image
-from requests.exceptions import ConnectionError, HTTPError, ReadTimeout
 
-from ..utils.logging import logger, raise_error, warn_with_log
+from ..pipeline import WorkDirManager
+from ..utils import logger, raise_error, run_ext_cmd, warn_with_log
+from .template_spaces import get_template, get_xfm
 from .utils import closest_resolution
 
 
 if TYPE_CHECKING:
     from nibabel import Nifti1Image
 
 
 # A dictionary containing all supported parcellations and their respective
 # valid parameters.
 
 # Each entry is a dictionary that must contain at least the following keys:
 # * 'family': the parcellation's family name (e.g. 'Schaefer', 'SUIT')
+# * 'space': the parcellation's space (e.g., 'MNI', 'SUIT')
 
 # Optional keys:
 # * 'valid_resolutions': a list of valid resolutions for the parcellation
 # (e.g. [1, 2])
 
 # TODO: have separate dictionary for built-in
 _available_parcellations: Dict[str, Dict[Any, Any]] = {
     "SUITxSUIT": {"family": "SUIT", "space": "SUIT"},
-    "SUITxMNI": {"family": "SUIT", "space": "MNI"},
+    "SUITxMNI": {"family": "SUIT", "space": "MNI152NLin6Asym"},
 }
 
 # Add Schaefer parcellation info
 for n_rois in range(100, 1001, 100):
     for t_net in [7, 17]:
         t_name = f"Schaefer{n_rois}x{t_net}"
         _available_parcellations[t_name] = {
             "family": "Schaefer",
             "n_rois": n_rois,
             "yeo_networks": t_net,
+            "space": "MNI152NLin6Asym",
         }
 # Add Tian parcellation info
 for scale in range(1, 5):
     t_name = f"TianxS{scale}x7TxMNI6thgeneration"
     _available_parcellations[t_name] = {
         "family": "Tian",
         "scale": scale,
         "magneticfield": "7T",
-        "space": "MNI6thgeneration",
+        "space": "MNI152NLin6Asym",
     }
     t_name = f"TianxS{scale}x3TxMNI6thgeneration"
     _available_parcellations[t_name] = {
         "family": "Tian",
         "scale": scale,
         "magneticfield": "3T",
-        "space": "MNI6thgeneration",
+        "space": "MNI152NLin6Asym",
     }
     t_name = f"TianxS{scale}x3TxMNInonlinear2009cAsym"
     _available_parcellations[t_name] = {
         "family": "Tian",
         "scale": scale,
         "magneticfield": "3T",
-        "space": "MNInonlinear2009cAsym",
+        "space": "MNI152NLin2009cAsym",
     }
 # Add AICHA parcellation info
 for version in (1, 2):
     _available_parcellations[f"AICHA_v{version}"] = {
         "family": "AICHA",
         "version": version,
+        "space": "IXI549Space",
     }
 # Add Shen parcellation info
 for year in (2013, 2015, 2019):
     if year == 2013:
         for n_rois in (50, 100, 150):
             _available_parcellations[f"Shen_{year}_{n_rois}"] = {
                 "family": "Shen",
                 "year": 2013,
                 "n_rois": n_rois,
+                "space": "MNI152NLin2009cAsym",
             }
     elif year == 2015:
         _available_parcellations["Shen_2015_268"] = {
             "family": "Shen",
             "year": 2015,
             "n_rois": 268,
+            "space": "MNI152NLin2009cAsym",
         }
     elif year == 2019:
         _available_parcellations["Shen_2019_368"] = {
             "family": "Shen",
             "year": 2019,
             "n_rois": 368,
+            "space": "MNI152NLin2009cAsym",
         }
 # Add Yan parcellation info
 for n_rois in range(100, 1001, 100):
     # Add Yeo networks
     for yeo_network in [7, 17]:
         _available_parcellations[f"Yan{n_rois}xYeo{yeo_network}"] = {
             "family": "Yan",
             "n_rois": n_rois,
             "yeo_networks": yeo_network,
+            "space": "MNI152NLin6Asym",
         }
     # Add Kong networks
     _available_parcellations[f"Yan{n_rois}xKong17"] = {
         "family": "Yan",
         "n_rois": n_rois,
         "kong_networks": 17,
+        "space": "MNI152NLin6Asym",
+    }
+# Add Brainnetome parcellation info
+for threshold in [0, 25, 50]:
+    _available_parcellations[f"Brainnetome_thr{threshold}"] = {
+        "family": "Brainnetome",
+        "threshold": threshold,
+        "space": "MNI152NLin6Asym",
     }
 
 
 def register_parcellation(
     name: str,
     parcellation_path: Union[str, Path],
     parcels_labels: List[str],
+    space: str,
     overwrite: bool = False,
 ) -> None:
     """Register a custom user parcellation.
 
     Parameters
     ----------
     name : str
         The name of the parcellation.
     parcellation_path : str or pathlib.Path
         The path to the parcellation file.
     parcels_labels : list of str
         The list of labels for the parcellation.
+    space : str
+        The template space of the parcellation, for e.g., "MNI152NLin6Asym".
     overwrite : bool, optional
         If True, overwrite an existing parcellation with the same name.
         Does not apply to built-in parcellations (default False).
 
     Raises
     ------
     ValueError
@@ -157,25 +177,26 @@
             ):
                 raise_error(
                     f"Cannot overwrite {name} parcellation. "
                     "It is a built-in parcellation."
                 )
         else:
             raise_error(
-                f"Parcellation {name} already registered. Set `overwrite=True`"
-                "to update its value."
+                f"Parcellation {name} already registered. Set "
+                "`overwrite=True` to update its value."
             )
     # Convert str to Path
     if not isinstance(parcellation_path, Path):
         parcellation_path = Path(parcellation_path)
     # Add user parcellation info
     _available_parcellations[name] = {
         "path": str(parcellation_path.absolute()),
         "labels": parcels_labels,
         "family": "CustomUserParcellation",
+        "space": space,
     }
 
 
 def list_parcellations() -> List[str]:
     """List all the available parcellations.
 
     Returns
@@ -183,32 +204,230 @@
     list of str
         A list with all available parcellations.
 
     """
     return sorted(_available_parcellations.keys())
 
 
-# def _check_resolution(resolution, valid_resolution):
-#     if resolution is None:
-#         return None
-#     if resolution not in valid_resolution:
-#         raise ValueError(f'Invalid resolution: {resolution}')
-#     return resolution
+def get_parcellation(
+    parcellation: List[str],
+    target_data: Dict[str, Any],
+    extra_input: Optional[Dict[str, Any]] = None,
+) -> Tuple["Nifti1Image", List[str]]:
+    """Get parcellation, tailored for the target image.
+
+    Parameters
+    ----------
+    parcellation : list of str
+        The name(s) of the parcellation(s).
+    target_data : dict
+        The corresponding item of the data object to which the parcellation
+        will be applied.
+    extra_input : dict, optional
+        The other fields in the data object. Useful for accessing other data
+        kinds that needs to be used in the computation of parcellations
+        (default None).
+
+    Returns
+    -------
+    Nifti1Image
+        The parcellation image.
+    list of str
+        Parcellation labels.
+
+    Raises
+    ------
+    RuntimeError
+        If warp / transformation file extension is not ".mat" or ".h5".
+    ValueError
+        If ``extra_input`` is None when ``target_data``'s space is native.
+
+    """
+    # Check pre-requirements for space manipulation
+    target_space = target_data["space"]
+    # Set target standard space to target space
+    target_std_space = target_space
+    # Extra data type requirement check if target space is native
+    if target_space == "native":
+        # Check for extra inputs
+        if extra_input is None:
+            raise_error(
+                "No extra input provided, requires `Warp` and `T1w` "
+                "data types in particular for transformation to "
+                f"{target_data['space']} space for further computation."
+            )
+        # Set target standard space to warp file space source
+        target_std_space = extra_input["Warp"]["src"]
+
+    # Get the min of the voxels sizes and use it as the resolution
+    target_img = target_data["data"]
+    resolution = np.min(target_img.header.get_zooms()[:3])
+
+    # Create component-scoped tempdir
+    tempdir = WorkDirManager().get_tempdir(prefix="parcellations")
+    # Create element-scoped tempdir so that warped parcellation is
+    # available later as nibabel stores file path reference for
+    # loading on computation
+    element_tempdir = WorkDirManager().get_element_tempdir(
+        prefix="parcellations"
+    )
+
+    # Load the parcellations
+    all_parcellations = []
+    all_labels = []
+    for name in parcellation:
+        img, labels, _, space = load_parcellation(
+            name=name,
+            resolution=resolution,
+        )
+
+        # Convert parcellation spaces if required
+        if space != target_std_space:
+            # Get xfm file
+            xfm_file_path = get_xfm(src=space, dst=target_std_space)
+            # Get target standard space template
+            target_std_space_template_img = get_template(
+                space=target_std_space,
+                target_data=target_data,
+                extra_input=extra_input,
+            )
+
+            # Save parcellation image to a component-scoped tempfile
+            parcellation_path = tempdir / f"{name}.nii.gz"
+            nib.save(img, parcellation_path)
+
+            # Save template
+            target_std_space_template_path = (
+                tempdir / f"{target_std_space}_T1w_{resolution}.nii.gz"
+            )
+            nib.save(
+                target_std_space_template_img, target_std_space_template_path
+            )
+
+            # Set warped parcellation path
+            warped_parcellation_path = element_tempdir / (
+                f"{name}_warped_from_{space}_to_" f"{target_std_space}.nii.gz"
+            )
+
+            logger.debug(
+                f"Using ANTs to warp {name} "
+                f"from {space} to {target_std_space}"
+            )
+            # Set antsApplyTransforms command
+            apply_transforms_cmd = [
+                "antsApplyTransforms",
+                "-d 3",
+                "-e 3",
+                "-n 'GenericLabel[NearestNeighbor]'",
+                f"-i {parcellation_path.resolve()}",
+                f"-r {target_std_space_template_path.resolve()}",
+                f"-t {xfm_file_path.resolve()}",
+                f"-o {warped_parcellation_path.resolve()}",
+            ]
+            # Call antsApplyTransforms
+            run_ext_cmd(name="antsApplyTransforms", cmd=apply_transforms_cmd)
+
+            img = nib.load(warped_parcellation_path)
+
+        # Resample parcellation to target image
+        img_to_merge = image.resample_to_img(
+            source_img=img,
+            target_img=target_img,
+            interpolation="nearest",
+            copy=True,
+        )
+
+        all_parcellations.append(img_to_merge)
+        all_labels.append(labels)
+
+    # Avoid merging if there is only one parcellation
+    if len(all_parcellations) == 1:
+        resampled_parcellation_img = all_parcellations[0]
+        labels = all_labels[0]
+    # Parcellations are already transformed to target standard space
+    else:
+        resampled_parcellation_img, labels = merge_parcellations(
+            parcellations_list=all_parcellations,
+            parcellations_names=parcellation,
+            labels_lists=all_labels,
+        )
+
+    # Warp parcellation if target space is native
+    if target_space == "native":
+        # Save parcellation image to a component-scoped tempfile
+        prewarp_parcellation_path = tempdir / "prewarp_parcellation.nii.gz"
+        nib.save(resampled_parcellation_img, prewarp_parcellation_path)
+
+        # Create an element-scoped tempfile for warped output
+        warped_parcellation_path = (
+            element_tempdir / "parcellation_warped.nii.gz"
+        )
+
+        # Check for warp file type to use correct tool
+        warp_file_ext = extra_input["Warp"]["path"].suffix
+        if warp_file_ext == ".mat":
+            logger.debug("Using FSL for parcellation warping")
+            # Set applywarp command
+            applywarp_cmd = [
+                "applywarp",
+                "--interp=nn",
+                f"-i {prewarp_parcellation_path.resolve()}",
+                # use resampled reference
+                f"-r {target_data['reference_path'].resolve()}",
+                f"-w {extra_input['Warp']['path'].resolve()}",
+                f"-o {warped_parcellation_path.resolve()}",
+            ]
+            # Call applywarp
+            run_ext_cmd(name="applywarp", cmd=applywarp_cmd)
+
+        elif warp_file_ext == ".h5":
+            logger.debug("Using ANTs for parcellation warping")
+            # Set antsApplyTransforms command
+            apply_transforms_cmd = [
+                "antsApplyTransforms",
+                "-d 3",
+                "-e 3",
+                "-n 'GenericLabel[NearestNeighbor]'",
+                f"-i {prewarp_parcellation_path.resolve()}",
+                # use resampled reference
+                f"-r {target_data['reference_path'].resolve()}",
+                f"-t {extra_input['Warp']['path'].resolve()}",
+                f"-o {warped_parcellation_path.resolve()}",
+            ]
+            # Call antsApplyTransforms
+            run_ext_cmd(name="antsApplyTransforms", cmd=apply_transforms_cmd)
+
+        else:
+            raise_error(
+                msg=(
+                    "Unknown warp / transformation file extension: "
+                    f"{warp_file_ext}"
+                ),
+                klass=RuntimeError,
+            )
+
+        # Load nifti
+        resampled_parcellation_img = nib.load(warped_parcellation_path)
+
+    # Delete tempdir
+    WorkDirManager().delete_tempdir(tempdir)
+
+    return resampled_parcellation_img, labels  # type: ignore
 
 
 def load_parcellation(
     name: str,
     parcellations_dir: Union[str, Path, None] = None,
     resolution: Optional[float] = None,
     path_only: bool = False,
-) -> Tuple[Optional["Nifti1Image"], List[str], Path]:
+) -> Tuple[Optional["Nifti1Image"], List[str], Path, str]:
     """Load a brain parcellation (including a label file).
 
-    If it is a built-in parcellaions and file is not present in the
-    `parcellations_dir` directory, it will be downloaded.
+    If it is a built-in parcellation and the file is not present in the
+    ``parcellations_dir`` directory, it will be downloaded.
 
     Parameters
     ----------
     name : str
         The name of the parcellation. Check valid options by calling
         :func:`.list_parcellations`.
     parcellations_dir : str or pathlib.Path, optional
@@ -226,56 +445,78 @@
     -------
     Nifti1Image or None
         Loaded parcellation image.
     list of str
         Parcellation labels.
     pathlib.Path
         File path to the parcellation image.
+    str
+        The space of the parcellation.
+
+    Raises
+    ------
+    ValueError
+        If ``name`` is invalid or if the parcellation values and labels
+        don't have equal dimension or if the value range is invalid.
 
     """
-    # Invalid parcellation name
+    # Check for valid parcellation name
     if name not in _available_parcellations:
         raise_error(
             f"Parcellation {name} not found. "
             f"Valid options are: {list_parcellations()}"
         )
 
+    # Copy parcellation definition to avoid edits in original object
     parcellation_definition = _available_parcellations[name].copy()
     t_family = parcellation_definition.pop("family")
+    # Remove space conditionally
+    if t_family not in ["SUIT", "Tian"]:
+        space = parcellation_definition.pop("space")
+    else:
+        space = parcellation_definition["space"]
 
+    # Check if the parcellation family is custom or built-in
     if t_family == "CustomUserParcellation":
         parcellation_fname = Path(parcellation_definition["path"])
         parcellation_labels = parcellation_definition["labels"]
     else:
         parcellation_fname, parcellation_labels = _retrieve_parcellation(
             family=t_family,
             parcellations_dir=parcellations_dir,
             resolution=resolution,
             **parcellation_definition,
         )
 
+    # Load parcellation image and values
     logger.info(f"Loading parcellation {parcellation_fname.absolute()!s}")
-
     parcellation_img = None
     if path_only is False:
+        # Load image via nibabel
         parcellation_img = nib.load(parcellation_fname)
+        # Get unique values
         parcel_values = np.unique(parcellation_img.get_fdata())
+        # Check for dimension
         if len(parcel_values) - 1 != len(parcellation_labels):
             raise_error(
                 f"Parcellation {name} has {len(parcel_values) - 1} parcels "
                 f"but {len(parcellation_labels)} labels."
             )
+        # Sort values
         parcel_values.sort()
+        # Check if value range is invalid
         if np.any(np.diff(parcel_values) != 1):
             raise_error(
                 f"Parcellation {name} must have all the values in the range  "
                 f"[0, {len(parcel_values)}]."
             )
 
-    return parcellation_img, parcellation_labels, parcellation_fname
+    # Type-cast to remove errors
+    parcellation_img = typing.cast("Nifti1Image", parcellation_img)
+    return parcellation_img, parcellation_labels, parcellation_fname, space
 
 
 def _retrieve_parcellation(
     family: str,
     parcellations_dir: Union[str, Path, None] = None,
     resolution: Optional[float] = None,
     **kwargs,
@@ -308,21 +549,21 @@
       ``n_rois`` : {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
             Granularity of parcellation to be used.
        ``yeo_network`` : {7, 17}, optional
             Number of Yeo networks to use (default 7).
     * Tian :
         ``scale`` : {1, 2, 3, 4}
             Scale of parcellation (defines granularity).
-        ``space`` : {"MNI6thgeneration", "MNInonlinear2009cAsym"}, optional
-            Space of parcellation (default "MNI6thgeneration"). (For more
+        ``space`` : {"MNI152NLin6Asym", "MNI152NLin2009cAsym"}, optional
+            Space of parcellation (default "MNI152NLin6Asym"). (For more
             information see https://github.com/yetianmed/subcortex)
         ``magneticfield`` : {"3T", "7T"}, optional
             Magnetic field (default "3T").
     * SUIT :
-        ``space`` : {"MNI", "SUIT"}, optional
+        ``space`` : {"MNI152NLin6Asym", "SUIT"}, optional
             Space of parcellation (default "MNI"). (For more information
             see http://www.diedrichsenlab.org/imaging/suit.htm).
     * AICHA :
         ``version`` : {1, 2}, optional
             Version of parcellation (default 2).
     * Shen :
         ``year`` : {2013, 2015, 2019}, optional
@@ -334,14 +575,17 @@
     * Yan :
         ``n_rois`` : {100, 200, 300, 400, 500, 600, 700, 800, 900, 1000}
             Granularity of the parcellation to be used.
         ``yeo_networks`` : {7, 17}, optional
             Number of Yeo networks to use (default None).
         ``kong_networks`` : {17}, optional
             Number of Kong networks to use (default None).
+    * Brainnetome :
+        ``threshold`` : {0, 25, 50}
+            Threshold for the probabilistic maps of subregion.
 
     Returns
     -------
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
@@ -397,14 +641,20 @@
         )
     elif family == "Yan":
         parcellation_fname, parcellation_labels = _retrieve_yan(
             parcellations_dir=parcellations_dir,
             resolution=resolution,
             **kwargs,
         )
+    elif family == "Brainnetome":
+        parcellation_fname, parcellation_labels = _retrieve_brainnetome(
+            parcellations_dir=parcellations_dir,
+            resolution=resolution,
+            **kwargs,
+        )
     else:
         raise_error(
             f"The provided parcellation name {family} cannot be retrieved."
         )
 
     return parcellation_fname, parcellation_labels
 
@@ -447,64 +697,62 @@
 
     """
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tn_rois: {n_rois}")
     logger.info(f"\tyeo_networks: {yeo_networks}")
 
+    # Check n_rois value
     _valid_n_rois = [100, 200, 300, 400, 500, 600, 700, 800, 900, 1000]
-    _valid_networks = [7, 17]
-    _valid_resolutions = [1, 2]
-
     if n_rois not in _valid_n_rois:
         raise_error(
             f"The parameter `n_rois` ({n_rois}) needs to be one of the "
             f"following: {_valid_n_rois}"
         )
+
+    # Check networks
+    _valid_networks = [7, 17]
     if yeo_networks not in _valid_networks:
         raise_error(
             f"The parameter `yeo_networks` ({yeo_networks}) needs to be one "
             f"of the following: {_valid_networks}"
         )
 
+    # Check resolution
+    _valid_resolutions = [1, 2]
     resolution = closest_resolution(resolution, _valid_resolutions)
 
-    # define file names
+    # Define parcellation and label file names
     parcellation_fname = (
         parcellations_dir
         / "schaefer_2018"
         / (
             f"Schaefer2018_{n_rois}Parcels_{yeo_networks}Networks_order_"
             f"FSLMNI152_{resolution}mm.nii.gz"
         )
     )
     parcellation_lname = (
         parcellations_dir
         / "schaefer_2018"
         / (f"Schaefer2018_{n_rois}Parcels_{yeo_networks}Networks_order.txt")
     )
 
-    # check existence of parcellation
+    # Check existence of parcellation
     if not (parcellation_fname.exists() and parcellation_lname.exists()):
         logger.info(
             "At least one of the parcellation files are missing. "
             "Fetching using nilearn."
         )
         datasets.fetch_atlas_schaefer_2018(
             n_rois=n_rois,
             yeo_networks=yeo_networks,
             resolution_mm=resolution,  # type: ignore we know it's 1 or 2
-            data_dir=str(parcellations_dir.absolute()),
+            data_dir=parcellations_dir.resolve(),
         )
 
-        if not (
-            parcellation_fname.exists() and parcellation_lname.exists()
-        ):  # pragma: no cover
-            raise_error("There was a problem fetching the parcellations.")
-
     # Load labels
     labels = [
         "_".join(x.split("_")[1:])
         for x in pd.read_csv(parcellation_lname, sep="\t", header=None)
         .iloc[:, 1]
         .to_list()
     ]
@@ -512,15 +760,15 @@
     return parcellation_fname, labels
 
 
 def _retrieve_tian(
     parcellations_dir: Path,
     resolution: Optional[float] = None,
     scale: Optional[int] = None,
-    space: str = "MNI6thgeneration",
+    space: str = "MNI152NLin6Asym",
     magneticfield: str = "3T",
 ) -> Tuple[Path, List[str]]:
     """Retrieve Tian parcellation.
 
     Parameters
     ----------
     parcellations_dir : pathlib.Path
@@ -529,94 +777,95 @@
         The desired resolution of the parcellation to load. If it is not
         available, the closest resolution will be loaded. Preferably, use a
         resolution higher than the desired one. By default, will load the
         highest one (default None). Available resolutions for this
         parcellation depend on the space and magnetic field.
     scale : {1, 2, 3, 4}, optional
         Scale of parcellation (defines granularity) (default None).
-    space : {"MNI6thgeneration", "MNInonlinear2009cAsym"}, optional
-        Space of parcellation (default "MNI6thgeneration"). (For more
+    space : {"MNI152NLin6Asym", "MNI152NLin2009cAsym"}, optional
+        Space of parcellation (default "MNI152NLin6Asym"). (For more
         information see https://github.com/yetianmed/subcortex)
     magneticfield : {"3T", "7T"}, optional
         Magnetic field (default "3T").
 
     Returns
     -------
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem fetching files.
     ValueError
         If invalid value is provided for ``scale`` or ``magneticfield`` or
-        ``space`` or if there is a problem fetching the parcellation.
+        ``space``.
 
     """
-    # show parameters to user
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tscale: {scale}")
     logger.info(f"\tspace: {space}")
     logger.info(f"\tmagneticfield: {magneticfield}")
 
-    # check validity of parameters
+    # Check scale
     _valid_scales = [1, 2, 3, 4]
     if scale not in _valid_scales:
         raise_error(
             f"The parameter `scale` ({scale}) needs to be one of the "
             f"following: {_valid_scales}"
         )
 
+    # Check resolution
     _valid_resolutions = []  # avoid pylance error
     if magneticfield == "3T":
-        _valid_spaces = ["MNI6thgeneration", "MNInonlinear2009cAsym"]
-        if space == "MNI6thgeneration":
+        _valid_spaces = ["MNI152NLin6Asym", "MNI152NLin2009cAsym"]
+        if space == "MNI152NLin6Asym":
             _valid_resolutions = [1, 2]
-        elif space == "MNInonlinear2009cAsym":
+        elif space == "MNI152NLin2009cAsym":
             _valid_resolutions = [2]
         else:
             raise_error(
                 f"The parameter `space` ({space}) for 3T needs to be one of "
                 f"the following: {_valid_spaces}"
             )
     elif magneticfield == "7T":
         _valid_resolutions = [1.6]
-        if space != "MNI6thgeneration":
+        if space != "MNI152NLin6Asym":
             raise_error(
                 f"The parameter `space` ({space}) for 7T needs to be "
-                f"MNI6thgeneration"
+                f"MNI152NLin6Asym"
             )
     else:
         raise_error(
             f"The parameter `magneticfield` ({magneticfield}) needs to be "
             f"one of the following: 3T or 7T"
         )
-
     resolution = closest_resolution(resolution, _valid_resolutions)
 
-    # define file names
+    # Define parcellation and label file names
     if magneticfield == "3T":
         parcellation_fname_base_3T = (
             parcellations_dir / "Tian2020MSA_v1.1" / "3T" / "Subcortex-Only"
         )
         parcellation_lname = parcellation_fname_base_3T / (
             f"Tian_Subcortex_S{scale}_3T_label.txt"
         )
-        if space == "MNI6thgeneration":
+        if space == "MNI152NLin6Asym":
             parcellation_fname = parcellation_fname_base_3T / (
                 f"Tian_Subcortex_S{scale}_{magneticfield}.nii.gz"
             )
             if resolution == 1:
                 parcellation_fname = (
                     parcellation_fname_base_3T
                     / f"Tian_Subcortex_S{scale}_{magneticfield}_1mm.nii.gz"
                 )
-        elif space == "MNInonlinear2009cAsym":
+        elif space == "MNI152NLin2009cAsym":
             space = "2009cAsym"
             parcellation_fname = parcellation_fname_base_3T / (
                 f"Tian_Subcortex_S{scale}_{magneticfield}_{space}.nii.gz"
             )
     elif magneticfield == "7T":
         parcellation_fname_base_7T = (
             parcellations_dir / "Tian2020MSA_v1.1" / "7T"
@@ -640,149 +889,176 @@
             for listitem in labels:
                 filehandle.write("%s\n" % listitem)
         logger.info(
             "Currently there are no labels provided for the 7T Tian "
             "parcellation. A simple numbering scheme for distinction was "
             "therefore used."
         )
-    else:  # pragma: no cover
-        raise_error("This should not happen. Please report this error.")
 
-    # check existence of parcellation
+    # Check existence of parcellation
     if not (parcellation_fname.exists() and parcellation_lname.exists()):
         logger.info(
             "At least one of the parcellation files are missing, fetching."
         )
-
-        url_basis = (
+        # Set URL
+        url = (
             "https://www.nitrc.org/frs/download.php/12012/Tian2020MSA_v1.1.zip"
         )
 
-        logger.info(f"Downloading TIAN from {url_basis}")
+        logger.info(f"Downloading TIAN from {url}")
+        # Store initial download in a tempdir
         with tempfile.TemporaryDirectory() as tmpdir:
-            parcellation_download = requests.get(url_basis)
-            parcellation_zip_fname = Path(tmpdir) / "Tian2020MSA_v1.1.zip"
-            with open(parcellation_zip_fname, "wb") as f:
-                f.write(parcellation_download.content)
-            with zipfile.ZipFile(parcellation_zip_fname, "r") as zip_ref:
-                zip_ref.extractall(parcellations_dir.as_posix())
-            # clean after unzipping
-            if (parcellations_dir / "__MACOSX").exists():
-                shutil.rmtree((parcellations_dir / "__MACOSX").as_posix())
-
-        labels = pd.read_csv(parcellation_lname, sep=" ", header=None)[
-            0
-        ].to_list()
-
-        if not (parcellation_fname.exists() and parcellation_lname.exists()):
-            raise_error("There was a problem fetching the parcellations.")
+            # Make HTTP request
+            try:
+                resp = httpx.get(url)
+                resp.raise_for_status()
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
+            else:
+                # Set tempfile for storing initial content and unzipping
+                zip_fname = Path(tmpdir) / "Tian2020MSA_v1.1.zip"
+                # Open tempfile and write content
+                with open(zip_fname, "wb") as f:
+                    f.write(resp.content)
+                # Unzip tempfile
+                with zipfile.ZipFile(zip_fname, "r") as zip_ref:
+                    zip_ref.extractall(parcellations_dir.as_posix())
+                # Clean after unzipping
+                if (parcellations_dir / "__MACOSX").exists():
+                    shutil.rmtree((parcellations_dir / "__MACOSX").as_posix())
 
+    # Load labels
     labels = pd.read_csv(parcellation_lname, sep=" ", header=None)[0].to_list()
 
     return parcellation_fname, labels
 
 
 def _retrieve_suit(
-    parcellations_dir: Path, resolution: Optional[float], space: str = "MNI"
+    parcellations_dir: Path,
+    resolution: Optional[float],
+    space: str = "MNI152NLin6Asym",
 ) -> Tuple[Path, List[str]]:
     """Retrieve SUIT parcellation.
 
     Parameters
     ----------
     parcellations_dir : pathlib.Path
         The path to the parcellation data directory.
     resolution : float, optional
         The desired resolution of the parcellation to load. If it is not
         available, the closest resolution will be loaded. Preferably, use a
         resolution higher than the desired one. By default, will load the
         highest one (default None). Available resolutions for this parcellation
         are 1mm and 2mm.
-    space : {"MNI", "SUIT"}, optional
-        Space of parcellation (default "MNI"). (For more information
-        see http://www.diedrichsenlab.org/imaging/suit.htm).
+    space : {"MNI152NLin6Asym", "SUIT"}, optional
+        Space of parcellation (default "MNI152NLin6Asym"). (For more
+        information see http://www.diedrichsenlab.org/imaging/suit.htm).
 
     Returns
     -------
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem fetching files.
     ValueError
-        If invalid value is provided for ``space`` or if there is a problem
-        fetching the parcellation.
+        If invalid value is provided for ``space``.
 
     """
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tspace: {space}")
 
-    _valid_spaces = ["MNI", "SUIT"]
-
-    # check validity of parameters
+    # Check space
+    _valid_spaces = ["MNI152NLin6Asym", "SUIT"]
     if space not in _valid_spaces:
         raise_error(
             f"The parameter `space` ({space}) needs to be one of the "
             f"following: {_valid_spaces}"
         )
 
-    # TODO: Validate this with Vera
+    # Check resolution
     _valid_resolutions = [1]
-
     resolution = closest_resolution(resolution, _valid_resolutions)
 
-    # define file names
+    # Format space if MNI; required for the file name
+    if space == "MNI152NLin6Asym":
+        space = "MNI"
+
+    # Define parcellation and label file names
     parcellation_fname = (
         parcellations_dir / "SUIT" / (f"SUIT_{space}Space_{resolution}mm.nii")
     )
     parcellation_lname = (
         parcellations_dir / "SUIT" / (f"SUIT_{space}Space_{resolution}mm.tsv")
     )
 
-    # check existence of parcellation
+    # Check existence of parcellation
     if not (parcellation_fname.exists() and parcellation_lname.exists()):
-        parcellation_fname.parent.mkdir(exist_ok=True, parents=True)
         logger.info(
             "At least one of the parcellation files is missing, fetching."
         )
-
+        # Create local directory if not present
+        parcellation_fname.parent.mkdir(exist_ok=True, parents=True)
+        # Set URL
         url_basis = (
             "https://github.com/DiedrichsenLab/cerebellar_atlases/raw"
-            "/master/Diedrichsen_2009/"
+            "/master/Diedrichsen_2009"
         )
-        url_MNI = url_basis + "atl-Anatom_space-MNI_dseg.nii"
-        url_SUIT = url_basis + "atl-Anatom_space-SUIT_dseg.nii"
-        url_labels = url_basis + "atl-Anatom.tsv"
-
         if space == "MNI":
-            logger.info(f"Downloading {url_MNI}")
-            parcellation_download = requests.get(url_MNI)
-            with open(parcellation_fname, "wb") as f:
-                f.write(parcellation_download.content)
+            url = f"{url_basis}/atl-Anatom_space-MNI_dseg.nii"
         else:  # if not MNI, then SUIT
-            logger.info(f"Downloading {url_SUIT}")
-            parcellation_download = requests.get(url_SUIT)
-            with open(parcellation_fname, "wb") as f:
-                f.write(parcellation_download.content)
-
-        labels_download = requests.get(url_labels)
-        labels = pd.read_csv(
-            io.StringIO(labels_download.content.decode("utf-8")),
-            sep="\t",
-            usecols=["name"],
-        )
-
-        labels.to_csv(parcellation_lname, sep="\t", index=False)
-        if (
-            not parcellation_fname.exists() and parcellation_lname.exists()
-        ):  # pragma: no cover
-            raise_error("There was a problem fetching the parcellations.")
+            url = f"{url_basis}/atl-Anatom_space-SUIT_dseg.nii"
+        url_labels = f"{url_basis}/atl-Anatom.tsv"
 
+        # Make HTTP requests
+        with httpx.Client(follow_redirects=True) as client:
+            # Download parcellation file
+            logger.info(f"Downloading SUIT parcellation from {url}")
+            try:
+                img_resp = client.get(url)
+                img_resp.raise_for_status()
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
+            else:
+                with open(parcellation_fname, "wb") as f:
+                    f.write(img_resp.content)
+            # Download label file
+            logger.info(f"Downloading SUIT labels from {url_labels}")
+            try:
+                label_resp = client.get(url_labels)
+                label_resp.raise_for_status()
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
+            else:
+                # Load labels
+                labels = pd.read_csv(
+                    io.StringIO(label_resp.content.decode("utf-8")),
+                    sep="\t",
+                    usecols=["name"],
+                )
+                labels.to_csv(parcellation_lname, sep="\t", index=False)
+
+    # Load labels
     labels = pd.read_csv(parcellation_lname, sep="\t", usecols=["name"])[
         "name"
     ].to_list()
 
     return parcellation_fname, labels
 
 
@@ -811,46 +1087,57 @@
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem fetching files.
     ValueError
-        If invalid value is provided for ``version`` or if there is a problem
-        fetching the parcellation.
+        If invalid value is provided for ``version``.
+
+    Warns
+    -----
+    RuntimeWarning
+        Until the authors confirm the space, the warning will be issued.
 
     Notes
     -----
     The resolution of the parcellation is 2mm and although v2 provides
     1mm, it is only for display purpose as noted in the release document.
 
     """
-    # show parameters to user
+    # Issue warning until space is confirmed by authors
+    warn_with_log(
+        "The current space for AICHA parcellations are IXI549Space, but are "
+        "not confirmed by authors, until that this warning will be issued."
+    )
+
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tversion: {version}")
 
-    # Check version value
-    _valid_version = (1, 2)
+    # Check version
+    _valid_version = [1, 2]
     if version not in _valid_version:
         raise_error(
             f"The parameter `version` ({version}) needs to be one of the "
             f"following: {_valid_version}"
         )
 
+    # Check resolution
     _valid_resolutions = [1]
     resolution = closest_resolution(resolution, _valid_resolutions)
 
-    # Define image file
+    # Define parcellation and label file names
     parcellation_fname = (
         parcellations_dir / f"AICHA_v{version}" / "AICHA" / "AICHA.nii"
     )
-
-    # Define label file name according to version
+    parcellation_lname = Path()
     if version == 1:
         parcellation_lname = (
             parcellations_dir
             / f"AICHA_v{version}"
             / "AICHA"
             / "AICHA_vol1.txt"
         )
@@ -863,62 +1150,68 @@
         )
 
     # Check existence of parcellation
     if not (parcellation_fname.exists() and parcellation_lname.exists()):
         logger.info(
             "At least one of the parcellation files are missing, fetching."
         )
-
         # Set file name on server according to version
+        server_filename = ""
         if version == 1:
             server_filename = "aicha_v1.zip"
         elif version == 2:
             server_filename = "AICHA_v2.tar.zip"
-
         # Set URL
         url = f"http://www.gin.cnrs.fr/wp-content/uploads/{server_filename}"
 
         logger.info(f"Downloading AICHA v{version} from {url}")
+        # Store initial download in a tempdir
         with tempfile.TemporaryDirectory() as tmpdir:
             # Make HTTP request
             try:
-                resp = requests.get(url)
+                resp = httpx.get(url, follow_redirects=True)
                 resp.raise_for_status()
-            except (ConnectionError, ReadTimeout, HTTPError) as err:
+            except httpx.HTTPError as exc:
                 raise_error(
-                    f"Failed to download AICHA v{version} due to: {err}"
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
                 )
             else:
+                # Set tempfile for storing initial content and unzipping
                 parcellation_zip_path = Path(tmpdir) / server_filename
+                # Open tempfile and write content
                 with open(parcellation_zip_path, "wb") as f:
                     f.write(resp.content)
-
-            # Extract zipfile
-            with zipfile.ZipFile(parcellation_zip_path, "r") as zip_ref:
-                if version == 1:
-                    zip_ref.extractall(
-                        (parcellations_dir / "AICHA_v1").as_posix()
-                    )
-                elif version == 2:
-                    zip_ref.extractall(Path(tmpdir).as_posix())
-                    # Extract tarfile for v2
-                    with tarfile.TarFile(
-                        Path(tmpdir) / "aicha_v2.tar", "r"
-                    ) as tar_ref:
-                        tar_ref.extractall(
-                            (parcellations_dir / "AICHA_v2").as_posix()
+                # Unzip tempfile
+                with zipfile.ZipFile(parcellation_zip_path, "r") as zip_ref:
+                    if version == 1:
+                        zip_ref.extractall(
+                            (parcellations_dir / "AICHA_v1").as_posix()
                         )
-
-            # Cleanup after unzipping
-            if (parcellations_dir / f"AICHA_v{version}" / "__MACOSX").exists():
-                shutil.rmtree(
-                    (
-                        parcellations_dir / f"AICHA_v{version}" / "__MACOSX"
-                    ).as_posix()
-                )
+                    elif version == 2:
+                        zip_ref.extractall(Path(tmpdir).as_posix())
+                        # Extract tarfile for v2
+                        with tarfile.TarFile(
+                            Path(tmpdir) / "aicha_v2.tar", "r"
+                        ) as tar_ref:
+                            tar_ref.extractall(
+                                (parcellations_dir / "AICHA_v2").as_posix()
+                            )
+                # Cleanup after unzipping
+                if (
+                    parcellations_dir / f"AICHA_v{version}" / "__MACOSX"
+                ).exists():
+                    shutil.rmtree(
+                        (
+                            parcellations_dir
+                            / f"AICHA_v{version}"
+                            / "__MACOSX"
+                        ).as_posix()
+                    )
 
     # Load labels
     labels = pd.read_csv(
         parcellation_lname, sep="\t", header=None, skiprows=[0]  # type: ignore
     )[0].to_list()
 
     return parcellation_fname, labels
@@ -955,20 +1248,21 @@
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem fetching files.
     ValueError
-        If invalid value or combination is provided for ``year`` and ``n_rois``
-        or if there is a problem fetching the parcellation.
+        If invalid value or combination is provided for ``year`` and
+        ``n_rois``.
 
     """
-    # show parameters to user
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tyear: {year}")
     logger.info(f"\tn_rois: {n_rois}")
 
     # Check resolution
     _valid_resolutions = [1, 2]
@@ -1008,15 +1302,15 @@
         )
     if (n_rois == 268 and year == 2019) or (n_rois == 368 and year == 2015):
         raise_error(
             f"The parameter combination `resolution = {resolution}` and "
             f"`year = {year}` is invalid"
         )
 
-    # Define image file according to constraints
+    # Define parcellation and label file names
     if year == 2013:
         parcellation_fname = (
             parcellations_dir
             / "Shen_2013"
             / "shenetal_neuroimage2013"
             / f"fconn_atlas_{n_rois}_{resolution}mm.nii"
         )
@@ -1055,54 +1349,60 @@
                 url = "https://www.nitrc.org/frs/download.php/7976/shen_1mm_268_parcellation.nii.gz"
             elif resolution == 2:
                 url = "https://www.nitrc.org/frs/download.php/7977/shen_2mm_268_parcellation.nii.gz"
         elif year == 2019:
             url = "https://www.nitrc.org/frs/download.php/11629/shen_368.zip"
 
         logger.info(f"Downloading Shen {year} from {url}")
+        # Store initial download in a tempdir
         with tempfile.TemporaryDirectory() as tmpdir:
             # Make HTTP request
             try:
-                resp = requests.get(url)
+                resp = httpx.get(url)
                 resp.raise_for_status()
-            except (ConnectionError, ReadTimeout, HTTPError) as err:
-                raise_error(f"Failed to download Shen {year} due to {err}")
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
             else:
                 if year in (2013, 2019):
                     parcellation_zip_path = Path(tmpdir) / f"Shen{year}.zip"
+                    # Open tempfile and write content
                     with open(parcellation_zip_path, "wb") as f:
                         f.write(resp.content)
-
-                    # Extract zipfile
+                    # Unzip tempfile
                     with zipfile.ZipFile(
                         parcellation_zip_path, "r"
                     ) as zip_ref:
                         zip_ref.extractall(
                             (parcellations_dir / f"Shen_{year}").as_posix()
                         )
-
                     # Cleanup after unzipping
                     if (
                         parcellations_dir / f"Shen_{year}" / "__MACOSX"
                     ).exists():
                         shutil.rmtree(
                             (
                                 parcellations_dir / f"Shen_{year}" / "__MACOSX"
                             ).as_posix()
                         )
-
                 elif year == 2015:
                     img_dir_path = parcellations_dir / "Shen_2015"
+                    # Create local directory if not present
                     img_dir_path.mkdir(parents=True, exist_ok=True)
                     img_path = (
                         img_dir_path
                         / f"shen_{resolution}mm_268_parcellation.nii.gz"
                     )
+                    # Create local file if not present
                     img_path.touch(exist_ok=True)
-                    with open(img_path.as_posix(), "wb") as f:
+                    # Open tempfile and write content
+                    with open(img_path, "wb") as f:
                         f.write(resp.content)
 
     # Load labels based on year
     if year == 2013:
         labels = (
             pd.read_csv(
                 parcellation_lname,  # type: ignore
@@ -1152,17 +1452,19 @@
     pathlib.Path
         File path to the parcellation image.
     list of str
         Parcellation labels.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem fetching files.
     ValueError
         If invalid value is provided for ``n_rois``, ``yeo_networks`` or
-        ``kong_networks`` or if there is a problem fetching the parcellation.
+        ``kong_networks``.
 
     """
     logger.info("Parcellation parameters:")
     logger.info(f"\tresolution: {resolution}")
     logger.info(f"\tn_rois: {n_rois}")
     logger.info(f"\tyeo_networks: {yeo_networks}")
     logger.info(f"\tkong_networks: {kong_networks}")
@@ -1184,14 +1486,16 @@
     _valid_n_rois = list(range(100, 1001, 100))
     if n_rois not in _valid_n_rois:
         raise_error(
             f"The parameter `n_rois` ({n_rois}) needs to be one of the "
             f"following: {_valid_n_rois}"
         )
 
+    parcellation_fname = Path()
+    parcellation_lname = Path()
     if yeo_networks:
         # Check yeo_networks value
         _valid_yeo_networks = [7, 17]
         if yeo_networks not in _valid_yeo_networks:
             raise_error(
                 f"The parameter `yeo_networks` ({yeo_networks}) needs to be "
                 f"one of the following: {_valid_yeo_networks}"
@@ -1236,14 +1540,16 @@
     # Check for existence of parcellation:
     if not parcellation_fname.exists() and not parcellation_lname.exists():
         logger.info(
             "At least one of the parcellation files are missing, fetching."
         )
 
         # Set URL based on network
+        img_url = ""
+        label_url = ""
         if yeo_networks:
             img_url = (
                 "https://raw.githubusercontent.com/ThomasYeoLab/CBIG/"
                 "master/stable_projects/brain_parcellation/Yan2023_homotopic/"
                 f"parcellations/MNI/yeo{yeo_networks}/{n_rois}Parcels_Yeo2011"
                 f"_{yeo_networks}Networks_FSLMNI152_{resolution}mm.nii.gz"
             )
@@ -1263,46 +1569,173 @@
             label_url = (
                 "https://raw.githubusercontent.com/ThomasYeoLab/CBIG/"
                 "master/stable_projects/brain_parcellation/Yan2023_homotopic/"
                 f"parcellations/MNI/kong17/freeview_lut/{n_rois}Parcels_"
                 "Kong2022_17Networks_LUT.txt"
             )
 
-        # Initiate a session and make HTTP requests
-        session = requests.Session()
-        # Download parcellation file
-        logger.info(f"Downloading Yan 2023 parcellation from {img_url}")
+        # Make HTTP requests
+        with httpx.Client() as client:
+            # Download parcellation file
+            logger.info(f"Downloading Yan 2023 parcellation from {img_url}")
+            try:
+                img_resp = client.get(img_url)
+                img_resp.raise_for_status()
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
+            else:
+                parcellation_img_path = Path(parcellation_fname)
+                # Create local directory if not present
+                parcellation_img_path.parent.mkdir(parents=True, exist_ok=True)
+                # Create local file if not present
+                parcellation_img_path.touch(exist_ok=True)
+                # Open file and write content
+                with open(parcellation_img_path, "wb") as f:
+                    f.write(img_resp.content)
+            # Download label file
+            logger.info(f"Downloading Yan 2023 labels from {label_url}")
+            try:
+                label_resp = client.get(label_url)
+                label_resp.raise_for_status()
+            except httpx.HTTPError as exc:
+                raise_error(
+                    f"Error response {exc.response.status_code} while "
+                    f"requesting {exc.request.url!r}",
+                    klass=RuntimeError,
+                )
+            else:
+                parcellation_labels_path = Path(parcellation_lname)
+                # Create local file if not present
+                parcellation_labels_path.touch(exist_ok=True)
+                # Open file and write content
+                with open(parcellation_labels_path, "wb") as f:
+                    f.write(label_resp.content)
+
+    # Load label file
+    labels = pd.read_csv(parcellation_lname, sep=" ", header=None)[1].to_list()
+
+    return parcellation_fname, labels
+
+
+def _retrieve_brainnetome(
+    parcellations_dir: Path,
+    resolution: Optional[float] = None,
+    threshold: Optional[int] = None,
+) -> Tuple[Path, List[str]]:
+    """Retrieve Brainnetome parcellation.
+
+    Parameters
+    ----------
+    parcellations_dir : pathlib.Path
+        The path to the parcellation data directory.
+    resolution : {1.0, 1.25, 2.0}, optional
+        The desired resolution of the parcellation to load. If it is not
+        available, the closest resolution will be loaded. Preferably, use a
+        resolution higher than the desired one. By default, will load the
+        highest one (default None). Available resolutions for this
+        parcellation are 1mm, 1.25mm and 2mm.
+    threshold : {0, 25, 50}, optional
+        The threshold for the probabilistic maps of subregion (default None).
+
+    Returns
+    -------
+    pathlib.Path
+        File path to the parcellation image.
+    list of str
+        Parcellation labels.
+
+    Raises
+    ------
+    RuntimeError
+        If there is a problem fetching files.
+    ValueError
+        If invalid value is provided for ``threshold``.
+
+    """
+    logger.info("Parcellation parameters:")
+    logger.info(f"\tresolution: {resolution}")
+    logger.info(f"\tthreshold: {threshold}")
+
+    # Check resolution
+    _valid_resolutions = [1.0, 1.25, 2.0]
+    resolution = closest_resolution(resolution, _valid_resolutions)
+
+    # Check threshold value
+    _valid_threshold = [0, 25, 50]
+    if threshold not in _valid_threshold:
+        raise_error(
+            f"The parameter `threshold` ({threshold}) needs to be one of the "
+            f"following: {_valid_threshold}"
+        )
+    # Correct resolution for further stuff
+    if resolution in [1.0, 2.0]:
+        resolution = int(resolution)
+
+    parcellation_fname = (
+        parcellations_dir
+        / "BNA246"
+        / f"BNA-maxprob-thr{threshold}-{resolution}mm.nii.gz"
+    )
+
+    # Check for existence of parcellation
+    if not parcellation_fname.exists():
+        # Set URL
+        url = f"http://neurovault.org/media/images/1625/BNA-maxprob-thr{threshold}-{resolution}mm.nii.gz"
+
+        logger.info(f"Downloading Brainnetome from {url}")
+        # Make HTTP request
         try:
-            img_resp = session.get(img_url)
-            img_resp.raise_for_status()
-        except (ConnectionError, ReadTimeout, HTTPError) as err:
+            resp = httpx.get(url, follow_redirects=True)
+            resp.raise_for_status()
+        except httpx.HTTPError as exc:
             raise_error(
-                f"Failed to download Yan 2023 parcellation due to: {err}"
+                f"Error response {exc.response.status_code} while "
+                f"requesting {exc.request.url!r}",
+                klass=RuntimeError,
             )
         else:
-            parcellation_img_path = Path(parcellation_fname)
-            parcellation_img_path.parent.mkdir(parents=True, exist_ok=True)
-            parcellation_img_path.touch(exist_ok=True)
-            with open(parcellation_img_path, "wb") as f:
-                f.write(img_resp.content)
-        # Download label file
-        logger.info(f"Downloading Yan 2023 labels from {label_url}")
-        try:
-            label_resp = session.get(label_url)
-            label_resp.raise_for_status()
-        except (ConnectionError, ReadTimeout, HTTPError) as err:
-            raise_error(f"Failed to download Yan 2023 labels due to: {err}")
-        else:
-            parcellation_labels_path = Path(parcellation_lname)
-            parcellation_labels_path.touch(exist_ok=True)
-            with open(parcellation_labels_path, "wb") as f:
-                f.write(label_resp.content)
+            # Create local directory if not present
+            parcellation_fname.parent.mkdir(parents=True, exist_ok=True)
+            # Create file if not present
+            parcellation_fname.touch(exist_ok=True)
+            # Open file and write bytes
+            parcellation_fname.write_bytes(resp.content)
 
-    # Load label file
-    labels = pd.read_csv(parcellation_lname, sep=" ", header=None)[1].to_list()
+    # Load labels
+    labels = (
+        sorted([f"SFG_L(R)_7_{i}" for i in range(1, 8)] * 2)
+        + sorted([f"MFG_L(R)_7_{i}" for i in range(1, 8)] * 2)
+        + sorted([f"IFG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"OrG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"PrG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"PCL_L(R)_2_{i}" for i in range(1, 3)] * 2)
+        + sorted([f"STG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"MTG_L(R)_4_{i}" for i in range(1, 5)] * 2)
+        + sorted([f"ITG_L(R)_7_{i}" for i in range(1, 8)] * 2)
+        + sorted([f"FuG_L(R)_3_{i}" for i in range(1, 4)] * 2)
+        + sorted([f"PhG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"pSTS_L(R)_2_{i}" for i in range(1, 3)] * 2)
+        + sorted([f"SPL_L(R)_5_{i}" for i in range(1, 6)] * 2)
+        + sorted([f"IPL_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"PCun_L(R)_4_{i}" for i in range(1, 5)] * 2)
+        + sorted([f"PoG_L(R)_4_{i}" for i in range(1, 5)] * 2)
+        + sorted([f"INS_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"CG_L(R)_7_{i}" for i in range(1, 8)] * 2)
+        + sorted([f"MVOcC _L(R)_5_{i}" for i in range(1, 6)] * 2)
+        + sorted([f"LOcC_L(R)_4_{i}" for i in range(1, 5)] * 2)
+        + sorted([f"LOcC_L(R)_2_{i}" for i in range(1, 3)] * 2)
+        + sorted([f"Amyg_L(R)_2_{i}" for i in range(1, 3)] * 2)
+        + sorted([f"Hipp_L(R)_2_{i}" for i in range(1, 3)] * 2)
+        + sorted([f"BG_L(R)_6_{i}" for i in range(1, 7)] * 2)
+        + sorted([f"Tha_L(R)_8_{i}" for i in range(1, 9)] * 2)
+    )
 
     return parcellation_fname, labels
 
 
 def merge_parcellations(
     parcellations_list: List["Nifti1Image"],
     parcellations_names: List[str],
```

### Comparing `junifer-0.0.4.dev90/junifer/data/tests/test_data_utils.py` & `junifer-0.0.5.dev11/junifer/data/tests/test_data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,13 @@
     ----------
     resolution: float
         The resolution to test.
     valid_resolutions: list of float
         The valid resolutions.
     expected: float
         The expected result.
+
     """
     assert closest_resolution(resolution, valid_resolutions) == expected
     assert (
         closest_resolution(resolution, np.array(valid_resolutions)) == expected
     )
```

### Comparing `junifer-0.0.4.dev90/junifer/data/tests/test_masks.py` & `junifer-0.0.5.dev11/junifer/data/tests/test_masks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,129 @@
 """Provide tests for masks."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Vera Komeyer <v.komeyer@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
+import socket
 from pathlib import Path
-from typing import Callable, Dict, List, Union
+from typing import Callable, Dict, List, Optional, Union
 
+import nibabel as nib
 import numpy as np
 import pytest
-from nilearn.datasets import fetch_icbm152_brain_gm_mask
 from nilearn.image import resample_to_img
 from nilearn.masking import (
     compute_background_mask,
-    compute_brain_mask,
     compute_epi_mask,
     intersect_masks,
 )
 from numpy.testing import assert_array_almost_equal, assert_array_equal
 
 from junifer.data.masks import (
     _available_masks,
     _load_vickery_patil_mask,
+    compute_brain_mask,
     get_mask,
     list_masks,
     load_mask,
     register_mask,
 )
+from junifer.datagrabber import DMCC13Benchmark
 from junifer.datareader import DefaultDataReader
 from junifer.testing.datagrabbers import (
     OasisVBMTestingDataGrabber,
+    PartlyCloudyTestingDataGrabber,
     SPMAuditoryTestingDataGrabber,
 )
 
 
+@pytest.mark.parametrize(
+    "mask_type, threshold",
+    [
+        ("brain", 0.2),
+        ("brain", 0.5),
+        ("brain", 0.8),
+        ("gm", 0.2),
+        ("gm", 0.5),
+        ("gm", 0.8),
+        ("wm", 0.2),
+        ("wm", 0.5),
+        ("wm", 0.8),
+    ],
+)
+def test_compute_brain_mask(mask_type: str, threshold: float) -> None:
+    """Test compute_brain_mask().
+
+    Parameters
+    ----------
+    mask_type : str
+        The parametrized mask type.
+    threshold : float
+        The parametrized threshold.
+
+    """
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        mask = compute_brain_mask(
+            target_data=element_data["BOLD"],
+            extra_input=None,
+            mask_type=mask_type,
+        )
+        assert isinstance(mask, nib.Nifti1Image)
+
+
+@pytest.mark.skipif(
+    socket.gethostname() != "juseless",
+    reason="only for juseless",
+)
+@pytest.mark.parametrize(
+    "mask_type",
+    [
+        "brain",
+        "gm",
+        "wm",
+    ],
+)
+def test_compute_brain_mask_for_native(mask_type: str) -> None:
+    """Test compute_brain_mask().
+
+    Parameters
+    ----------
+    mask_type : str
+        The parametrized mask type.
+
+    """
+    with DMCC13Benchmark(
+        types=["BOLD"],
+        sessions=["ses-wave1bas"],
+        tasks=["Rest"],
+        phase_encodings=["AP"],
+        runs=["1"],
+        native_t1w=True,
+    ) as dg:
+        element_data = DefaultDataReader().fit_transform(
+            dg[("sub-f1031ax", "ses-wave1bas", "Rest", "AP", "1")]
+        )
+        mask = compute_brain_mask(
+            target_data=element_data["BOLD"],
+            extra_input=None,
+            mask_type=mask_type,
+        )
+        assert isinstance(mask, nib.Nifti1Image)
+
+
 def test_register_mask_built_in_check() -> None:
     """Test mask registration check for built-in masks."""
     with pytest.raises(ValueError, match=r"built-in mask"):
         register_mask(
             name="GM_prob0.2",
             mask_path="testmask.nii.gz",
+            space="MNI",
             overwrite=True,
         )
 
 
 def test_list_masks_incorrect() -> None:
     """Test incorrect information check for list masks."""
     masks = list_masks()
@@ -53,75 +132,83 @@
 
 def test_register_mask_already_registered() -> None:
     """Test mask registration check for already registered."""
     # Register custom mask
     register_mask(
         name="testmask",
         mask_path="testmask.nii.gz",
+        space="MNI",
     )
     out = load_mask("testmask", path_only=True)
     assert out[1] is not None
     assert out[1].name == "testmask.nii.gz"
 
     # Try registering again
     with pytest.raises(ValueError, match=r"already registered."):
         register_mask(
             name="testmask",
             mask_path="testmask.nii.gz",
+            space="MNI",
         )
     register_mask(
         name="testmask",
         mask_path="testmask2.nii.gz",
+        space="MNI",
         overwrite=True,
     )
 
     out = load_mask("testmask", path_only=True)
     assert out[1] is not None
     assert out[1].name == "testmask2.nii.gz"
 
 
 @pytest.mark.parametrize(
-    "name, mask_path, overwrite",
+    "name, mask_path, space, overwrite",
     [
-        ("testmask_1", "testmask_1.nii.gz", True),
-        ("testmask_2", "testmask_2.nii.gz", True),
-        ("testmask_3", Path("testmask_3.nii.gz"), True),
+        ("testmask_1", "testmask_1.nii.gz", "MNI", True),
+        ("testmask_2", "testmask_2.nii.gz", "MNI", True),
+        ("testmask_3", Path("testmask_3.nii.gz"), "MNI", True),
     ],
 )
 def test_register_mask(
     name: str,
     mask_path: str,
+    space: str,
     overwrite: bool,
 ) -> None:
     """Test mask registration.
 
     Parameters
     ----------
     name : str
         The parametrized mask name.
     mask_path : str or pathlib.Path
         The parametrized mask path.
+    space : str
+        The parametrized mask space.
     overwrite : bool
         The parametrized mask overwrite value.
 
     """
     # Register custom mask
     register_mask(
         name=name,
         mask_path=mask_path,
+        space=space,
         overwrite=overwrite,
     )
     # List available mask and check registration
     masks = list_masks()
     assert name in masks
     # Load registered mask
-    _, fname = load_mask(name=name, path_only=True)
+    _, fname, mask_space = load_mask(name=name, path_only=True)
     # Check values for registered mask
     assert fname is not None
     assert fname.name == f"{name}.nii.gz"
+    assert space == mask_space
 
 
 @pytest.mark.parametrize(
     "mask_name",
     [
         "GM_prob0.2",
         "GM_prob0.2_cortex",
@@ -142,60 +229,87 @@
 
 def test_load_mask_incorrect() -> None:
     """Test loading of invalid masks."""
     with pytest.raises(ValueError, match=r"not found"):
         load_mask("wrongmask")
 
 
-def test_vickery_patil() -> None:
-    """Test Vickery-Patil mask."""
-    mask, fname = load_mask("GM_prob0.2")
-    assert_array_almost_equal(
-        mask.header["pixdim"][1:4], [1.5, 1.5, 1.5]  # type: ignore
-    )
-
-    assert fname is not None
-    assert fname.name == "CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz"
-
-    mask, fname = load_mask("GM_prob0.2", resolution=3)
-    assert_array_almost_equal(
-        mask.header["pixdim"][1:4], [3.0, 3.0, 3.0]  # type: ignore
-    )
+@pytest.mark.parametrize(
+    "name, resolution, pixdim, fname",
+    [
+        (
+            "GM_prob0.2",
+            None,
+            [1.5, 1.5, 1.5],
+            "CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz",
+        ),
+        (
+            "GM_prob0.2",
+            3.0,
+            [3.0, 3.0, 3.0],
+            "CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz",
+        ),
+        (
+            "GM_prob0.2_cortex",
+            None,
+            [3.0, 3.0, 3.0],
+            "GMprob0.2_cortex_3mm_NA_rm.nii.gz",
+        ),
+    ],
+)
+def test_vickery_patil(
+    name: str,
+    resolution: Optional[float],
+    pixdim: List[float],
+    fname: str,
+) -> None:
+    """Test Vickery-Patil mask.
 
-    assert fname is not None
-    assert (
-        fname.name == "CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz"
-    )
+    Parameters
+    ----------
+    name : str
+        The parametrized name of the mask.
+    resolution : float or None
+        The parametrized resolution of the mask.
+    pixdim : list of float
+        The parametrized pixel dimensions of the mask.
+    fname : str
+        The parametrized name of the mask file.
 
-    mask, fname = load_mask("GM_prob0.2_cortex")
+    """
+    mask, mask_fname, space = load_mask(name, resolution=resolution)
     assert_array_almost_equal(
-        mask.header["pixdim"][1:4], [3.0, 3.0, 3.0]  # type: ignore
+        mask.header["pixdim"][1:4], pixdim  # type: ignore
     )
+    assert space == "IXI549Space"
+    assert mask_fname is not None
+    assert mask_fname.name == fname
 
-    assert fname is not None
-    assert fname.name == "GMprob0.2_cortex_3mm_NA_rm.nii.gz"
 
+def test_vickery_patil_error() -> None:
+    """Test error for Vickery-Patil mask."""
     with pytest.raises(ValueError, match=r"find a Vickery-Patil mask "):
-        _load_vickery_patil_mask("wrong", resolution=2)
+        _load_vickery_patil_mask(name="wrong", resolution=2.0)
 
 
 def test_get_mask() -> None:
     """Test the get_mask function."""
-    reader = DefaultDataReader()
     with OasisVBMTestingDataGrabber() as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        vbm_gm = input["VBM_GM"]
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        vbm_gm = element_data["VBM_GM"]
         vbm_gm_img = vbm_gm["data"]
-        mask = get_mask(masks="GM_prob0.2", target_data=vbm_gm)
+        mask = get_mask(masks="compute_brain_mask", target_data=vbm_gm)
 
         assert mask.shape == vbm_gm_img.shape
         assert_array_equal(mask.affine, vbm_gm_img.affine)
 
-        raw_mask_img, _ = load_mask("GM_prob0.2", resolution=1.5)
+        raw_mask_callable, _, _ = load_mask(
+            "compute_brain_mask", resolution=1.5
+        )
+        raw_mask_img = raw_mask_callable(vbm_gm)  # type: ignore
         res_mask_img = resample_to_img(
             raw_mask_img,
             vbm_gm_img,
             interpolation="nearest",
             copy=True,
         )
         assert_array_equal(mask.get_fdata(), res_mask_img.get_fdata())
@@ -203,35 +317,35 @@
 
 def test_mask_callable() -> None:
     """Test using a callable mask."""
 
     def ident(x):
         return x
 
-    _available_masks["identity"] = {"family": "Callable", "func": ident}
-    reader = DefaultDataReader()
+    _available_masks["identity"] = {
+        "family": "Callable",
+        "func": ident,
+        "space": "MNI152Lin",
+    }
     with OasisVBMTestingDataGrabber() as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        vbm_gm = input["VBM_GM"]
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        vbm_gm = element_data["VBM_GM"]
         vbm_gm_img = vbm_gm["data"]
         mask = get_mask(masks="identity", target_data=vbm_gm)
 
         assert_array_equal(mask.get_fdata(), vbm_gm_img.get_fdata())
 
     del _available_masks["identity"]
 
 
 def test_get_mask_errors() -> None:
     """Test passing wrong parameters to get_mask."""
-    reader = DefaultDataReader()
     with OasisVBMTestingDataGrabber() as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        vbm_gm = input["VBM_GM"]
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        vbm_gm = element_data["VBM_GM"]
         # Test wrong masks definitions (more than one key per dict)
         with pytest.raises(ValueError, match=r"only one key"):
             get_mask(masks={"GM_prob0.2": {}, "Other": {}}, target_data=vbm_gm)
 
         # Test wrong masks definitions (pass paramaeters to non-callable mask)
         with pytest.raises(ValueError, match=r"callable params"):
             get_mask(masks={"GM_prob0.2": {"param": 1}}, target_data=vbm_gm)
@@ -243,15 +357,16 @@
             get_mask(masks={"threshold": 1}, target_data=vbm_gm)
 
         # Pass parameters to the intersection function when only one mask
         with pytest.raises(
             ValueError, match=r"parameters to the intersection"
         ):
             get_mask(
-                masks=["GM_prob0.2", {"threshold": 1}], target_data=vbm_gm
+                masks=["compute_brain_mask", {"threshold": 1}],
+                target_data=vbm_gm,
             )
 
         # Test "inherited" masks errors
 
         # 1) No extra_data parameter
         with pytest.raises(ValueError, match=r"no extra data was passed"):
             get_mask(masks="inherit", target_data=vbm_gm)
@@ -267,27 +382,28 @@
         # 3) mask_item not in extra data
         with pytest.raises(ValueError, match=r"does not exist"):
             vbm_gm["mask_item"] = "wrong"
             get_mask(
                 masks="inherit", target_data=vbm_gm, extra_input=extra_input
             )
 
+        # Block fetch_icbm152_brain_gm_mask space transformation
+        with pytest.raises(RuntimeError, match="prohibited"):
+            get_mask(
+                masks="fetch_icbm152_brain_gm_mask",
+                target_data=vbm_gm,
+                extra_input=extra_input,
+            )
+
 
 @pytest.mark.parametrize(
     "mask_name,function,params,resample",
     [
-        ("compute_brain_mask", compute_brain_mask, {"threshold": 0.2}, False),
         ("compute_background_mask", compute_background_mask, None, False),
         ("compute_epi_mask", compute_epi_mask, None, False),
-        (
-            "fetch_icbm152_brain_gm_mask",
-            fetch_icbm152_brain_gm_mask,
-            None,
-            True,
-        ),
     ],
 )
 def test_nilearn_compute_masks(
     mask_name: str,
     function: Callable,
     params: Union[Dict, None],
     resample: bool,
@@ -300,20 +416,19 @@
         Name of the mask.
     function : callable
         Function to call.
     params : dict, optional
         Parameters to pass to the function.
     resample : bool
         Whether to resample the mask to the target data.
+
     """
-    reader = DefaultDataReader()
     with SPMAuditoryTestingDataGrabber() as dg:
-        input = dg["sub001"]
-        input = reader.fit_transform(input)
-        bold = input["BOLD"]
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
+        bold = element_data["BOLD"]
         bold_img = bold["data"]
 
         if params is None:
             params = {}
             mask_spec = mask_name
         else:
             mask_spec = {mask_name: params}
@@ -334,85 +449,80 @@
                 copy=True,
             )
         assert_array_equal(mask.get_fdata(), ni_mask.get_fdata())
 
 
 def test_get_mask_inherit() -> None:
     """Test using the inherit mask functionality."""
-    reader = DefaultDataReader()
     with SPMAuditoryTestingDataGrabber() as dg:
-        input = dg["sub001"]
-        input = reader.fit_transform(input)
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
         # Compute brain mask using nilearn
-        gm_mask = compute_brain_mask(input["BOLD"]["data"], threshold=0.2)
+        gm_mask = compute_brain_mask(element_data["BOLD"], threshold=0.2)
 
         # Get mask using the compute_brain_mask function
         mask1 = get_mask(
             masks={"compute_brain_mask": {"threshold": 0.2}},
-            target_data=input["BOLD"],
+            target_data=element_data["BOLD"],
         )
 
         # Now get the mask using the inherit functionality, passing the
         # computed mask as extra data
-        extra_input = {"BOLD_MASK": {"data": gm_mask}}
-        input["BOLD"]["mask_item"] = "BOLD_MASK"
+        extra_input = {
+            "BOLD_MASK": {
+                "data": gm_mask,
+                "space": element_data["BOLD"]["space"],
+            }
+        }
+        element_data["BOLD"]["mask_item"] = "BOLD_MASK"
         mask2 = get_mask(
-            masks="inherit", target_data=input["BOLD"], extra_input=extra_input
+            masks="inherit",
+            target_data=element_data["BOLD"],
+            extra_input=extra_input,
         )
 
         # Both masks should be equal
         assert_array_equal(mask1.get_fdata(), mask2.get_fdata())
 
 
 @pytest.mark.parametrize(
     "masks,params",
     [
-        (["GM_prob0.2", "compute_brain_mask"], {}),
-        (
-            ["GM_prob0.2", "compute_brain_mask"],
-            {"threshold": 0.2},
-        ),
-        (
-            [
-                "GM_prob0.2",
-                "compute_brain_mask",
-                "fetch_icbm152_brain_gm_mask",
-            ],
-            {"threshold": 1, "connected": True},
-        ),
+        (["compute_brain_mask", "compute_background_mask"], {}),
+        (["compute_brain_mask", "compute_epi_mask"], {}),
     ],
 )
 def test_get_mask_multiple(
     masks: Union[str, Dict, List[Union[Dict, str]]], params: Dict
 ) -> None:
     """Test getting multiple masks.
 
     Parameters
     ----------
     masks : str, dict, list of str or dict
         Masks to get, junifer style.
     params : dict
         Parameters to pass to the intersect_masks function.
+
     """
-    reader = DefaultDataReader()
     with SPMAuditoryTestingDataGrabber() as dg:
-        input = dg["sub001"]
-        input = reader.fit_transform(input)
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
         if not isinstance(masks, list):
             junifer_masks = [masks]
         else:
             junifer_masks = masks.copy()
         if len(params) > 0:
             # Convert params to junifer style (one dict per param)
             junifer_params = [{k: params[k]} for k in params.keys()]
             junifer_masks.extend(junifer_params)
-        target_img = input["BOLD"]["data"]
+        target_img = element_data["BOLD"]["data"]
         resolution = np.min(target_img.header.get_zooms()[:3])
 
-        computed = get_mask(masks=junifer_masks, target_data=input["BOLD"])
+        computed = get_mask(
+            masks=junifer_masks, target_data=element_data["BOLD"]
+        )
 
         masks_names = [
             next(iter(x.keys())) if isinstance(x, dict) else x for x in masks
         ]
 
         mask_funcs = [
             x
@@ -427,15 +537,21 @@
 
         mask_imgs = [
             load_mask(t_mask, path_only=False, resolution=resolution)[0]
             for t_mask in mask_files
         ]
 
         for t_func in mask_funcs:
-            mask_imgs.append(_available_masks[t_func]["func"](target_img))
+            # Bypass for custom mask
+            if t_func == "compute_brain_mask":
+                mask_imgs.append(
+                    _available_masks[t_func]["func"](element_data["BOLD"])
+                )
+            else:
+                mask_imgs.append(_available_masks[t_func]["func"](target_img))
 
         mask_imgs = [
             resample_to_img(
                 t_mask,
                 target_img,
                 interpolation="nearest",
                 copy=True,
```

### Comparing `junifer-0.0.4.dev90/junifer/data/tests/test_parcellations.py` & `junifer-0.0.5.dev11/junifer/data/tests/test_parcellations.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,39 +7,48 @@
 
 from pathlib import Path
 from typing import List
 
 import nibabel as nib
 import numpy as np
 import pytest
-from nilearn.image import new_img_like
+from nilearn.image import new_img_like, resample_to_img
 from numpy.testing import assert_array_almost_equal, assert_array_equal
 
 from junifer.data.parcellations import (
     _retrieve_aicha,
+    _retrieve_brainnetome,
     _retrieve_parcellation,
     _retrieve_schaefer,
     _retrieve_shen,
     _retrieve_suit,
     _retrieve_tian,
     _retrieve_yan,
+    get_parcellation,
     list_parcellations,
     load_parcellation,
     merge_parcellations,
     register_parcellation,
 )
+from junifer.datareader import DefaultDataReader
+from junifer.pipeline.utils import _check_ants
+from junifer.testing.datagrabbers import (
+    OasisVBMTestingDataGrabber,
+    PartlyCloudyTestingDataGrabber,
+)
 
 
 def test_register_parcellation_built_in_check() -> None:
     """Test parcellation registration check for built-in parcellations."""
     with pytest.raises(ValueError, match=r"built-in parcellation"):
         register_parcellation(
             name="SUITxSUIT",
             parcellation_path="testparc.nii.gz",
             parcels_labels=["1", "2", "3"],
+            space="SUIT",
             overwrite=True,
         )
 
 
 def test_list_parcellations_incorrect() -> None:
     """Test incorrect information check for list parcellations."""
     parcellations = list_parcellations()
@@ -49,31 +58,34 @@
 def test_register_parcellation_already_registered() -> None:
     """Test parcellation registration check for already registered."""
     # Register custom parcellation
     register_parcellation(
         name="testparc",
         parcellation_path="testparc.nii.gz",
         parcels_labels=["1", "2", "3"],
+        space="MNI152Lin",
     )
     assert (
         load_parcellation("testparc", path_only=True)[2].name
         == "testparc.nii.gz"
     )
 
     # Try registering again
     with pytest.raises(ValueError, match=r"already registered."):
         register_parcellation(
             name="testparc",
             parcellation_path="testparc.nii.gz",
             parcels_labels=["1", "2", "3"],
+            space="MNI152Lin",
         )
     register_parcellation(
         name="testparc",
         parcellation_path="testparc2.nii.gz",
         parcels_labels=["1", "2", "3"],
+        space="MNI152Lin",
         overwrite=True,
     )
 
     assert (
         load_parcellation("testparc", path_only=True)[2].name
         == "testparc2.nii.gz"
     )
@@ -82,94 +94,128 @@
 def test_parcellation_wrong_labels_values(tmp_path: Path) -> None:
     """Test parcellation with wrong labels and values.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
+
     """
-    schaefer, labels, schaefer_path = load_parcellation("Schaefer100x7")
+    schaefer, labels, schaefer_path, _ = load_parcellation("Schaefer100x7")
     assert schaefer is not None
 
     # Test wrong number of labels
-    register_parcellation("WrongLabels", schaefer_path, labels[:10])
+    register_parcellation(
+        "WrongLabels", schaefer_path, labels[:10], "MNI152Lin"
+    )
 
     with pytest.raises(ValueError, match=r"has 100 parcels but 10"):
         load_parcellation("WrongLabels")
 
     # Test wrong number of labels
-    register_parcellation("WrongLabels2", schaefer_path, [*labels, "wrong"])
+    register_parcellation(
+        "WrongLabels2", schaefer_path, [*labels, "wrong"], "MNI152Lin"
+    )
 
     with pytest.raises(ValueError, match=r"has 100 parcels but 101"):
         load_parcellation("WrongLabels2")
 
     schaefer_data = schaefer.get_fdata().copy()
     schaefer_data[schaefer_data == 50] = 0
     new_schaefer_path = tmp_path / "new_schaefer.nii.gz"
     new_schaefer_img = new_img_like(schaefer, schaefer_data)
     nib.save(new_schaefer_img, new_schaefer_path)
 
-    register_parcellation("WrongValues", new_schaefer_path, labels[:-1])
+    register_parcellation(
+        "WrongValues", new_schaefer_path, labels[:-1], "MNI152Lin"
+    )
     with pytest.raises(ValueError, match=r"the range [0, 99]"):
         load_parcellation("WrongValues")
 
     schaefer_data = schaefer.get_fdata().copy()
     schaefer_data[schaefer_data == 50] = 200
     new_schaefer_path = tmp_path / "new_schaefer2.nii.gz"
     new_schaefer_img = new_img_like(schaefer, schaefer_data)
     nib.save(new_schaefer_img, new_schaefer_path)
 
-    register_parcellation("WrongValues2", new_schaefer_path, labels)
+    register_parcellation(
+        "WrongValues2", new_schaefer_path, labels, "MNI152Lin"
+    )
     with pytest.raises(ValueError, match=r"the range [0, 100]"):
         load_parcellation("WrongValues2")
 
 
 @pytest.mark.parametrize(
-    "name, parcellation_path, parcels_labels, overwrite",
+    "name, parcellation_path, parcels_labels, space, overwrite",
     [
-        ("testparc_1", "testparc_1.nii.gz", ["1", "2", "3"], True),
-        ("testparc_2", "testparc_2.nii.gz", ["1", "2", "6"], True),
-        ("testparc_3", Path("testparc_3.nii.gz"), ["1", "2", "6"], True),
+        (
+            "testparc_1",
+            "testparc_1.nii.gz",
+            ["1", "2", "3"],
+            "MNI152Lin",
+            True,
+        ),
+        (
+            "testparc_2",
+            "testparc_2.nii.gz",
+            ["1", "2", "6"],
+            "MNI152Lin",
+            True,
+        ),
+        (
+            "testparc_3",
+            Path("testparc_3.nii.gz"),
+            ["1", "2", "6"],
+            "MNI152Lin",
+            True,
+        ),
     ],
 )
 def test_register_parcellation(
     name: str,
     parcellation_path: str,
     parcels_labels: List[str],
+    space: str,
     overwrite: bool,
 ) -> None:
     """Test parcellation registration.
 
     Parameters
     ----------
     name : str
         The parametrized parcellation name.
     parcellation_path : str or pathlib.Path
         The parametrized parcellation path.
     parcels_labels : list of str
         The parametrized parcellation labels.
+    space : str
+        The parametrized parcellation space.
     overwrite : bool
         The parametrized parcellation overwrite value.
 
     """
     # Register custom parcellation
     register_parcellation(
         name=name,
         parcellation_path=parcellation_path,
         parcels_labels=parcels_labels,
+        space=space,
         overwrite=overwrite,
     )
     # List available parcellation and check registration
     parcellations = list_parcellations()
     assert name in parcellations
     # Load registered parcellation
-    _, lbl, fname = load_parcellation(name=name, path_only=True)
+    _, lbl, fname, parcellation_space = load_parcellation(
+        name=name, path_only=True
+    )
     # Check values for registered parcellation
     assert lbl == parcels_labels
     assert fname.name == f"{name}.nii.gz"
+    assert parcellation_space == space
 
 
 @pytest.mark.parametrize(
     "parcellation_name",
     [
         "AICHA_v1",
         "AICHA_v2",
@@ -277,22 +323,23 @@
     assert parcellation_name in parcellations
 
     parcellation_file = (
         f"Schaefer2018_{n_rois}Parcels_{yeo_networks}Networks_order_FSLMNI152_"
         f"{int(resolution)}mm.nii.gz"
     )
     # Load parcellation
-    img, label, img_path = load_parcellation(
+    img, label, img_path, space = load_parcellation(
         name=parcellation_name,
         parcellations_dir=tmp_path,
         resolution=resolution,
     )
     assert img is not None
     assert img_path.name == parcellation_file
     assert len(label) == n_rois
+    assert space == "MNI152NLin6Asym"
     assert_array_equal(
         img.header["pixdim"][1:4], 3 * [resolution]  # type: ignore
     )
 
 
 def test_retrieve_schaefer_incorrect_n_rois(tmp_path: Path) -> None:
     """Test retrieve Schaefer with incorrect ROIs.
@@ -327,37 +374,40 @@
             resolution=1,
             n_rois=100,
             yeo_networks=8,
         )
 
 
 @pytest.mark.parametrize(
-    "space",
-    ["SUIT", "MNI"],
+    "space_key, space",
+    [("SUIT", "SUIT"), ("MNI", "MNI152NLin6Asym")],
 )
-def test_suit(tmp_path: Path, space: str) -> None:
+def test_suit(tmp_path: Path, space_key: str, space: str) -> None:
     """Test SUIT parcellation.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
+    space_key : str
+        The parametrized space values for the key.
     space : str
         The parametrized space values.
 
     """
     parcellations = list_parcellations()
-    assert f"SUITx{space}" in parcellations
+    assert f"SUITx{space_key}" in parcellations
     # Load parcellation
-    img, label, img_path = load_parcellation(
-        name=f"SUITx{space}",
+    img, label, img_path, parcellation_space = load_parcellation(
+        name=f"SUITx{space_key}",
         parcellations_dir=tmp_path,
     )
     assert img is not None
-    assert img_path.name == f"SUIT_{space}Space_1mm.nii"
+    assert img_path.name == f"SUIT_{space_key}Space_1mm.nii"
+    assert parcellation_space == space
     assert len(label) == 34
     assert_array_equal(img.header["pixdim"][1:4], [1, 1, 1])  # type: ignore
 
 
 def test_retrieve_suit_incorrect_space(tmp_path: Path) -> None:
     """Test retrieve SUIT with incorrect space.
 
@@ -393,31 +443,33 @@
     """
     parcellations = list_parcellations()
     assert "TianxS1x3TxMNI6thgeneration" in parcellations
     assert "TianxS2x3TxMNI6thgeneration" in parcellations
     assert "TianxS3x3TxMNI6thgeneration" in parcellations
     assert "TianxS4x3TxMNI6thgeneration" in parcellations
     # Load parcellation
-    img, lbl, fname = load_parcellation(
+    img, lbl, fname, parcellation_space_1 = load_parcellation(
         name=f"TianxS{scale}x3TxMNI6thgeneration", parcellations_dir=tmp_path
     )
     fname1 = f"Tian_Subcortex_S{scale}_3T_1mm.nii.gz"
     assert img is not None
     assert fname.name == fname1
+    assert parcellation_space_1 == "MNI152NLin6Asym"
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [1, 1, 1])  # type: ignore
     # Load parcellation
-    img, lbl, fname = load_parcellation(
+    img, lbl, fname, parcellation_space_2 = load_parcellation(
         name=f"TianxS{scale}x3TxMNI6thgeneration",
         parcellations_dir=tmp_path,
         resolution=2,
     )
     fname1 = f"Tian_Subcortex_S{scale}_3T.nii.gz"
     assert img is not None
     assert fname.name == fname1
+    assert parcellation_space_2 == "MNI152NLin6Asym"
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
 
 
 @pytest.mark.parametrize(
     "scale, n_label", [(1, 16), (2, 32), (3, 50), (4, 54)]
 )
@@ -438,21 +490,22 @@
     """
     parcellations = list_parcellations()
     assert "TianxS1x3TxMNInonlinear2009cAsym" in parcellations
     assert "TianxS2x3TxMNInonlinear2009cAsym" in parcellations
     assert "TianxS3x3TxMNInonlinear2009cAsym" in parcellations
     assert "TianxS4x3TxMNInonlinear2009cAsym" in parcellations
     # Load parcellation
-    img, lbl, fname = load_parcellation(
+    img, lbl, fname, space = load_parcellation(
         name=f"TianxS{scale}x3TxMNInonlinear2009cAsym",
         parcellations_dir=tmp_path,
     )
     fname1 = f"Tian_Subcortex_S{scale}_3T_2009cAsym.nii.gz"
     assert img is not None
     assert fname.name == fname1
+    assert space == "MNI152NLin2009cAsym"
     assert len(lbl) == n_label
     assert_array_equal(img.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
 
 
 @pytest.mark.parametrize(
     "scale, n_label", [(1, 16), (2, 34), (3, 54), (4, 62)]
 )
@@ -473,20 +526,21 @@
     """
     parcellations = list_parcellations()
     assert "TianxS1x7TxMNI6thgeneration" in parcellations
     assert "TianxS2x7TxMNI6thgeneration" in parcellations
     assert "TianxS3x7TxMNI6thgeneration" in parcellations
     assert "TianxS4x7TxMNI6thgeneration" in parcellations
     # Load parcellation
-    img, lbl, fname = load_parcellation(
+    img, lbl, fname, space = load_parcellation(
         name=f"TianxS{scale}x7TxMNI6thgeneration", parcellations_dir=tmp_path
     )
     fname1 = f"Tian_Subcortex_S{scale}_7T.nii.gz"
     assert img is not None
     assert fname.name == fname1
+    assert space == "MNI152NLin6Asym"
     assert len(lbl) == n_label
     assert_array_almost_equal(
         img.header["pixdim"][1:4], [1.6, 1.6, 1.6]  # type: ignore
     )
 
 
 def test_retrieve_tian_incorrect_space(tmp_path: Path) -> None:
@@ -499,21 +553,21 @@
 
     """
     with pytest.raises(ValueError, match=r"The parameter `space`"):
         _retrieve_tian(
             parcellations_dir=tmp_path, resolution=1, scale=1, space="wrong"
         )
 
-    with pytest.raises(ValueError, match=r"MNI6thgeneration"):
+    with pytest.raises(ValueError, match=r"MNI152NLin6Asym"):
         _retrieve_tian(
             parcellations_dir=tmp_path,
             resolution=1,
             scale=1,
             magneticfield="7T",
-            space="MNInonlinear2009cAsym",
+            space="MNI152NLin2009cAsym",
         )
 
 
 def test_retrieve_tian_incorrect_magneticfield(tmp_path: Path) -> None:
     """Test retrieve tian with incorrect magneticfield.
 
     Parameters
@@ -541,15 +595,15 @@
 
     """
     with pytest.raises(ValueError, match=r"The parameter `scale`"):
         _retrieve_tian(
             parcellations_dir=tmp_path,
             resolution=1,
             scale=5,
-            space="MNI6thgeneration",
+            space="MNI152NLin6Asym",
         )
 
 
 @pytest.mark.parametrize("version", [1, 2])
 def test_aicha(tmp_path: Path, version: int) -> None:
     """Test AICHA parcellation.
 
@@ -560,19 +614,20 @@
     version : int
         The parametrized version values.
 
     """
     parcellations = list_parcellations()
     assert f"AICHA_v{version}" in parcellations
     # Load parcellation
-    img, label, img_path = load_parcellation(
+    img, label, img_path, space = load_parcellation(
         name=f"AICHA_v{version}", parcellations_dir=tmp_path
     )
     assert img is not None
     assert img_path.name == "AICHA.nii"
+    assert space == "IXI549Space"
     assert len(label) == 384
     assert_array_equal(img.header["pixdim"][1:4], [2, 2, 2])  # type: ignore
 
 
 def test_retrieve_aicha_incorrect_version(tmp_path: Path) -> None:
     """Test retrieve AICHA with incorrect version.
 
@@ -628,21 +683,22 @@
     img_name : str
         The parametrized partial file names.
 
     """
     parcellations = list_parcellations()
     assert f"Shen_{year}_{n_rois}" in parcellations
     # Load parcellation
-    img, label, img_path = load_parcellation(
+    img, label, img_path, space = load_parcellation(
         name=f"Shen_{year}_{n_rois}",
         parcellations_dir=tmp_path,
         resolution=resolution,
     )
     assert img is not None
     assert img_name in img_path.name
+    assert space == "MNI152NLin2009cAsym"
     assert len(label) == n_labels
     assert_array_equal(
         img.header["pixdim"][1:4], 3 * [resolution]  # type: ignore
     )
 
 
 def test_retrieve_shen_incorrect_year(tmp_path: Path) -> None:
@@ -823,21 +879,22 @@
         parcellation_name = f"Yan{n_rois}xKong{kong_networks}"
         assert parcellation_name in parcellations
         parcellation_file = (
             f"{n_rois}Parcels_Kong2022_{kong_networks}Networks_FSLMNI152_"
             f"{int(resolution)}mm.nii.gz"
         )
     # Load parcellation
-    img, label, img_path = load_parcellation(
+    img, label, img_path, space = load_parcellation(
         name=parcellation_name,  # type: ignore
         parcellations_dir=tmp_path,
         resolution=resolution,
     )
     assert img is not None
     assert img_path.name == parcellation_file  # type: ignore
+    assert space == "MNI152NLin6Asym"
     assert len(label) == n_rois
     assert_array_equal(
         img.header["pixdim"][1:4], 3 * [resolution]  # type: ignore
     )
 
 
 def test_retrieve_yan_incorrect_networks(tmp_path: Path) -> None:
@@ -917,21 +974,92 @@
         _retrieve_yan(
             parcellations_dir=tmp_path,
             n_rois=100,
             kong_networks=27,
         )
 
 
+@pytest.mark.parametrize(
+    "resolution, threshold",
+    [
+        (1.0, 0),
+        (1.0, 25),
+        (1.0, 50),
+        (1.25, 0),
+        (1.25, 25),
+        (1.25, 50),
+        (2, 0),
+        (2, 25),
+        (2, 50),
+    ],
+)
+def test_brainnetome(
+    tmp_path: Path,
+    resolution: float,
+    threshold: int,
+) -> None:
+    """Test Brainnetome parcellation.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+    resolution : float
+        The parametrized resolution values.
+    threshold : int
+        The parametrized threshold values.
+
+    """
+    parcellations = list_parcellations()
+    parcellation_name = f"Brainnetome_thr{threshold}"
+    assert parcellation_name in parcellations
+
+    # Fix resolution
+    if resolution in [1.0, 2.0]:
+        resolution = int(resolution)
+
+    parcellation_file = f"BNA-maxprob-thr{threshold}-{resolution}mm.nii.gz"
+    # Load parcellation
+    img, label, img_path, space = load_parcellation(
+        name=parcellation_name,
+        parcellations_dir=tmp_path,
+        resolution=resolution,
+    )
+    assert img is not None
+    assert img_path.name == parcellation_file
+    assert space == "MNI152NLin6Asym"
+    assert len(label) == 246
+    assert_array_equal(
+        img.header["pixdim"][1:4], 3 * [resolution]  # type: ignore
+    )
+
+
+def test_retrieve_brainnetome_incorrect_threshold(tmp_path: Path) -> None:
+    """Test retrieve Brainnetome with incorrect threshold.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+    with pytest.raises(ValueError, match="The parameter `threshold`"):
+        _retrieve_brainnetome(
+            parcellations_dir=tmp_path,
+            threshold=100,
+        )
+
+
 def test_merge_parcellations() -> None:
     """Test merging parcellations."""
     # load some parcellations for testing
-    schaefer_parcellation, schaefer_labels, _ = load_parcellation(
+    schaefer_parcellation, schaefer_labels, _, _ = load_parcellation(
         "Schaefer100x17"
     )
-    tian_parcellation, tian_labels, _ = load_parcellation(
+    tian_parcellation, tian_labels, _, _ = load_parcellation(
         "TianxS2x3TxMNInonlinear2009cAsym"
     )
     # prepare the list of the actual parcellations
     parcellation_list = [schaefer_parcellation, tian_parcellation]
     # prepare a list of names
     names = ["Schaefer100x17", "TianxS2x3TxMNInonlinear2009cAsym"]
     # prepare a list of label lists
@@ -956,15 +1084,15 @@
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
     # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+    parcellation, labels, _, _ = load_parcellation("Schaefer100x7")
 
     assert parcellation is not None
 
     # Create two parcellations from it
     parcellation_data = parcellation.get_fdata()
     parcellation1_data = parcellation_data.copy()
     parcellation1_data[parcellation1_data > 50] = 0
@@ -977,36 +1105,29 @@
     parcellation1_img = new_img_like(parcellation, parcellation1_data)
     parcellation2_img = new_img_like(parcellation, parcellation2_data)
 
     parcellation_list = [parcellation1_img, parcellation2_img]
     names = ["high", "low"]
     labels_lists = [labels1, labels2]
 
-    merged_parc, merged_labels = merge_parcellations(
+    merged_parc, _ = merge_parcellations(
         parcellation_list, names, labels_lists
     )
 
     parc_data = parcellation.get_fdata()
     assert_array_equal(parc_data, merged_parc.get_fdata())
     assert len(labels) == 100
     assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
 
 
-def test_merge_parcellations_3D_multiple_overlapping(tmp_path: Path) -> None:
-    """Test merge_parcellations with multiple overlapping parcellations.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The path to the test directory.
-
-    """
+def test_merge_parcellations_3D_multiple_overlapping() -> None:
+    """Test merge_parcellations with multiple overlapping parcellations."""
 
     # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+    parcellation, labels, _, _ = load_parcellation("Schaefer100x7")
 
     assert parcellation is not None
 
     # Create two parcellations from it
     parcellation_data = parcellation.get_fdata()
     parcellation1_data = parcellation_data.copy()
     parcellation1_data[parcellation1_data > 50] = 0
@@ -1031,28 +1152,19 @@
         )
 
     parc_data = parcellation.get_fdata()
     assert len(labels) == 100
     assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
 
 
-def test_merge_parcellations_3D_multiple_duplicated_labels(
-    tmp_path: Path,
-) -> None:
-    """Test merge_parcellations with two parcellations with duplicated labels.
-
-    Parameters
-    ----------
-    tmp_path : pathlib.Path
-        The path to the test directory.
-
-    """
+def test_merge_parcellations_3D_multiple_duplicated_labels() -> None:
+    """Test merge_parcellations with duplicated labels."""
 
     # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+    parcellation, labels, _, _ = load_parcellation("Schaefer100x7")
 
     assert parcellation is not None
 
     # Create two parcellations from it
     parcellation_data = parcellation.get_fdata()
     parcellation1_data = parcellation_data.copy()
     parcellation1_data[parcellation1_data > 50] = 0
@@ -1074,7 +1186,106 @@
             parcellation_list, names, labels_lists
         )
 
     parc_data = parcellation.get_fdata()
     assert_array_equal(parc_data, merged_parc.get_fdata())
     assert len(labels) == 100
     assert len(np.unique(parc_data)) == 101  # 100 + 1 because background 0
+
+
+def test_get_parcellation_single() -> None:
+    """Test tailored single parcellation fetch."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        bold = element_data["BOLD"]
+        bold_img = bold["data"]
+        # Get tailored parcellation
+        tailored_parcellation, tailored_labels = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=bold,
+        )
+        # Check shape and affine with original element data
+        assert tailored_parcellation.shape == bold_img.shape[:3]
+        assert_array_equal(tailored_parcellation.affine, bold_img.affine)
+        # Get raw parcellation
+        raw_parcellation, raw_labels, _, _ = load_parcellation(
+            "TianxS1x3TxMNInonlinear2009cAsym",
+            resolution=1.5,
+        )
+        resampled_raw_parcellation = resample_to_img(
+            source_img=raw_parcellation,
+            target_img=bold_img,
+            interpolation="nearest",
+            copy=True,
+        )
+        # Check resampled data with tailored data
+        assert_array_equal(
+            tailored_parcellation.get_fdata(),
+            resampled_raw_parcellation.get_fdata(),
+        )
+        assert tailored_labels == raw_labels
+
+
+def test_get_parcellation_multi_same_space() -> None:
+    """Test tailored multi parcellation fetch in same space."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        bold = element_data["BOLD"]
+        bold_img = bold["data"]
+        # Get tailored parcellation
+        tailored_parcellation, tailored_labels = get_parcellation(
+            parcellation=[
+                "Shen_2015_268",
+                "TianxS1x3TxMNInonlinear2009cAsym",
+            ],
+            target_data=bold,
+        )
+        # Check shape and affine with original element data
+        assert tailored_parcellation.shape == bold_img.shape[:3]
+        assert_array_equal(tailored_parcellation.affine, bold_img.affine)
+        # Get raw parcellations
+        raw_parcellations = []
+        raw_labels = []
+        parcellations_names = [
+            "Shen_2015_268",
+            "TianxS1x3TxMNInonlinear2009cAsym",
+        ]
+        for name in parcellations_names:
+            img, labels, _, _ = load_parcellation(name=name, resolution=1.5)
+            # Resample raw parcellations
+            resampled_img = resample_to_img(
+                source_img=img,
+                target_img=bold_img,
+                interpolation="nearest",
+                copy=True,
+            )
+            raw_parcellations.append(resampled_img)
+            raw_labels.append(labels)
+        # Merge resampled parcellations
+        merged_resampled_parcellations, merged_labels = merge_parcellations(
+            parcellations_list=raw_parcellations,
+            parcellations_names=parcellations_names,
+            labels_lists=raw_labels,
+        )
+        # Check resampled data with tailored data
+        assert_array_equal(
+            tailored_parcellation.get_fdata(),
+            merged_resampled_parcellations.get_fdata(),
+        )
+        assert tailored_labels == merged_labels
+
+
+@pytest.mark.skipif(
+    _check_ants() is False, reason="requires ANTs to be in PATH"
+)
+def test_get_parcellation_multi_different_space() -> None:
+    """Test tailored multi parcellation fetch in different space."""
+    with OasisVBMTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        # Get tailored parcellation
+        get_parcellation(
+            parcellation=[
+                "Schaefer100x7",
+                "TianxS1x3TxMNInonlinear2009cAsym",
+            ],
+            target_data=element_data["VBM_GM"],
+        )
```

### Comparing `junifer-0.0.4.dev90/junifer/data/utils.py` & `junifer-0.0.5.dev11/junifer/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 """Provide utilities for data module."""
+
 from typing import List, Optional, Union
 
 import numpy as np
 
 from ..utils.logging import logger
 
 
 def closest_resolution(
-    resolution: Optional[float],
+    resolution: Optional[Union[float, int]],
     valid_resolution: Union[List[float], List[int], np.ndarray],
 ) -> Union[float, int]:
     """Find the closest resolution.
 
     Parameters
     ----------
-    resolution : float, optional
+    resolution : float or int, optional
         The given resolution. If None, will return the highest resolution
         (default None).
     valid_resolution : list of float or int, or np.ndarray
         The array of valid resolutions.
 
     Returns
     -------
     float or int
         The closest valid resolution.
+
     """
     # Convert list of int to numpy.ndarray
     if not isinstance(valid_resolution, np.ndarray):
         valid_resolution = np.array(valid_resolution)
 
     if resolution is None:
         logger.info("Resolution set to None, using highest resolution.")
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/__init__.py` & `junifer-0.0.5.dev11/junifer/datagrabber/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 from .datalad_base import DataladDataGrabber
 from .pattern import PatternDataGrabber
 from .pattern_datalad import PatternDataladDataGrabber
 
 from .aomic import DataladAOMICID1000, DataladAOMICPIOP1, DataladAOMICPIOP2
 from .hcp1200 import HCP1200, DataladHCP1200
 from .multiple import MultipleDataGrabber
+from .dmcc13_benchmark import DMCC13Benchmark
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.5.dev11/junifer/datagrabber/aomic/piop1.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,30 +22,38 @@
 
     Parameters
     ----------
     datadir : str or Path or None, optional
         The directory where the datalad dataset will be cloned. If None,
         the datalad dataset will be cloned into a temporary directory
         (default None).
-    types: {"BOLD", "BOLD_confounds", "T1w", "probseg_CSF", "probseg_GM", \
-           "probseg_WM", "DWI"} or a list of the options, optional
+    types: {"BOLD", "BOLD_confounds", "T1w", "VBM_CSF", "VBM_GM", \
+           "VBM_WM", "DWI"} or a list of the options, optional
         AOMIC data types. If None, all available data types are selected.
         (default None).
     tasks : {"restingstate", "anticipation", "emomatching", "faces", \
             "gstroop", "workingmemory"} or list of the options, optional
         AOMIC PIOP1 task sessions. If None, all available task sessions are
         selected (default None).
+    native_t1w : bool, optional
+        Whether to use T1w in native space (default False).
+
+    Raises
+    ------
+    ValueError
+        If invalid value is passed for ``tasks``.
 
     """
 
     def __init__(
         self,
         datadir: Union[str, Path, None] = None,
         types: Union[str, List[str], None] = None,
         tasks: Union[str, List[str], None] = None,
+        native_t1w: bool = False,
     ) -> None:
         # Declare all tasks
         all_tasks = [
             "restingstate",
             "anticipation",
             "emomatching",
             "faces",
@@ -65,59 +73,119 @@
                     raise_error(
                         f"{t} is not a valid task in the AOMIC PIOP1"
                         " dataset!"
                     )
         self.tasks = tasks
         # The patterns
         patterns = {
-            "BOLD": (
-                "derivatives/fmriprep/sub-{subject}/func/"
-                "sub-{subject}_task-{task}_"
-                "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
-            ),
-            "BOLD_confounds": (
-                "derivatives/fmriprep/sub-{subject}/func/"
-                "sub-{subject}_task-{task}_"
-                "desc-confounds_regressors.tsv"
-            ),
-            "BOLD_mask": (
-                "derivatives/fmriprep/sub-{subject}/func/"
-                "sub-{subject}_task-{task}_"
-                "space-MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
-            ),
-            "T1w": (
-                "derivatives/fmriprep/sub-{subject}/anat/"
-                "sub-{subject}_space-MNI152NLin2009cAsym_"
-                "desc-preproc_T1w.nii.gz"
-            ),
-            "T1w_mask": (
-                "derivatives/fmriprep/sub-{subject}/anat/"
-                "sub-{subject}_space-MNI152NLin2009cAsym_"
-                "desc-brain_mask.nii.gz"
-            ),
-            "probseg_CSF": (
-                "derivatives/fmriprep/sub-{subject}/anat/"
-                "sub-{subject}_space-MNI152NLin2009cAsym_label-"
-                "CSF_probseg.nii.gz"
-            ),
-            "probseg_GM": (
-                "derivatives/fmriprep/sub-{subject}/anat/"
-                "sub-{subject}_space-MNI152NLin2009cAsym_label-"
-                "GM_probseg.nii.gz"
-            ),
-            "probseg_WM": (
-                "derivatives/fmriprep/sub-{subject}/anat/"
-                "sub-{subject}_space-MNI152NLin2009cAsym_label-"
-                "WM_probseg.nii.gz"
-            ),
-            "DWI": (
-                "derivatives/dwipreproc/sub-{subject}/dwi/"
-                "sub-{subject}_desc-preproc_dwi.nii.gz"
-            ),
+            "BOLD": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/func/"
+                    "{subject}_task-{task}_"
+                    "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+                "mask_item": "BOLD_mask",
+            },
+            "BOLD_confounds": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/func/"
+                    "{subject}_task-{task}_"
+                    "desc-confounds_regressors.tsv"
+                ),
+                "format": "fmriprep",
+            },
+            "BOLD_mask": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/func/"
+                    "{subject}_task-{task}_"
+                    "space-MNI152NLin2009cAsym_desc-brain_mask.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "T1w": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/anat/"
+                    "{subject}_space-MNI152NLin2009cAsym_"
+                    "desc-preproc_T1w.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+                "mask_item": "T1w_mask",
+            },
+            "T1w_mask": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/anat/"
+                    "{subject}_space-MNI152NLin2009cAsym_"
+                    "desc-brain_mask.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_CSF": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/anat/"
+                    "{subject}_space-MNI152NLin2009cAsym_label-"
+                    "CSF_probseg.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_GM": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/anat/"
+                    "{subject}_space-MNI152NLin2009cAsym_label-"
+                    "GM_probseg.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "VBM_WM": {
+                "pattern": (
+                    "derivatives/fmriprep/{subject}/anat/"
+                    "{subject}_space-MNI152NLin2009cAsym_label-"
+                    "WM_probseg.nii.gz"
+                ),
+                "space": "MNI152NLin2009cAsym",
+            },
+            "DWI": {
+                "pattern": (
+                    "derivatives/dwipreproc/{subject}/dwi/"
+                    "{subject}_desc-preproc_dwi.nii.gz"
+                ),
+            },
         }
+        # Use native T1w assets
+        self.native_t1w = False
+        if native_t1w:
+            self.native_t1w = True
+            patterns.update(
+                {
+                    "T1w": {
+                        "pattern": (
+                            "derivatives/fmriprep/{subject}/anat/"
+                            "{subject}_desc-preproc_T1w.nii.gz"
+                        ),
+                        "space": "native",
+                        "mask_item": "T1w_mask",
+                    },
+                    "T1w_mask": {
+                        "pattern": (
+                            "derivatives/fmriprep/{subject}/anat/"
+                            "{subject}_desc-brain_mask.nii.gz"
+                        ),
+                        "space": "native",
+                    },
+                    "Warp": {
+                        "pattern": (
+                            "derivatives/fmriprep/{subject}/anat/"
+                            "{subject}_from-MNI152NLin2009cAsym_to-T1w_"
+                            "mode-image_xfm.h5"
+                        ),
+                        "src": "MNI152NLin2009cAsym",
+                        "dst": "native",
+                    },
+                }
+            )
         # Set default types
         if types is None:
             types = list(patterns.keys())
         # Convert single type into list
         else:
             if not isinstance(types, list):
                 types = [types]
@@ -159,29 +227,24 @@
             "gstroop": "seq",
             "restingstate": "mb3",
             "workingmemory": "seq",
         }
         acq = task_acqs[task]
         new_task = f"{task}_acq-{acq}"
 
-        out = super().get_item(subject=subject, task=new_task)
-        if out.get("BOLD"):
-            out["BOLD"]["mask_item"] = "BOLD_mask"
-        if out.get("T1w"):
-            out["T1w"]["mask_item"] = "T1w_mask"
-        return out
+        return super().get_item(subject=subject, task=new_task)
 
     def get_elements(self) -> List:
         """Implement fetching list of subjects in the dataset.
 
         Returns
         -------
         list of str
             The list of subjects in the dataset.
 
         """
-        subjects = [f"{x:04d}" for x in range(1, 217)]
+        subjects = [f"sub-{x:04d}" for x in range(1, 217)]
         elems = []
         for subject, task in product(subjects, self.tasks):
             elems.append((subject, task))
 
         return elems
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,94 +29,93 @@
 
         out = dg[test_element]
 
         # asserts type "BOLD"
         assert "BOLD" in out
 
         assert (
-            out["BOLD"]["path"].name
-            == f"sub-{test_element}_task-moviewatching_"
+            out["BOLD"]["path"].name == f"{test_element}_task-moviewatching_"
             "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
         )
 
         assert out["BOLD"]["path"].exists()
         assert out["BOLD"]["path"].is_file()
 
         # asserts type "BOLD_confounds"
         assert "BOLD_confounds" in out
 
         assert (
             out["BOLD_confounds"]["path"].name
-            == f"sub-{test_element}_task-moviewatching_"
+            == f"{test_element}_task-moviewatching_"
             "desc-confounds_regressors.tsv"
         )
 
         assert out["BOLD_confounds"]["path"].exists()
         assert out["BOLD_confounds"]["path"].is_file()
 
         # assert BOLD_mask
         assert out["BOLD_mask"]["path"].exists()
 
         # asserts type "T1w"
         assert "T1w" in out
 
         assert (
             out["T1w"]["path"].name
-            == f"sub-{test_element}_space-MNI152NLin2009cAsym_"
+            == f"{test_element}_space-MNI152NLin2009cAsym_"
             "desc-preproc_T1w.nii.gz"
         )
 
         assert out["T1w"]["path"].exists()
         assert out["T1w"]["path"].is_file()
 
         # asserts T1w_mask
         assert out["T1w_mask"]["path"].exists()
 
-        # asserts type "probseg_CSF"
-        assert "probseg_CSF" in out
+        # asserts type "VBM_CSF"
+        assert "VBM_CSF" in out
 
         assert (
-            out["probseg_CSF"]["path"].name
-            == f"sub-{test_element}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_CSF"]["path"].name
+            == f"{test_element}_space-MNI152NLin2009cAsym_label-"
             "CSF_probseg.nii.gz"
         )
 
-        assert out["probseg_CSF"]["path"].exists()
-        assert out["probseg_CSF"]["path"].is_file()
+        assert out["VBM_CSF"]["path"].exists()
+        assert out["VBM_CSF"]["path"].is_file()
 
-        # asserts type "probseg_GM"
-        assert "probseg_GM" in out
+        # asserts type "VBM_GM"
+        assert "VBM_GM" in out
 
         assert (
-            out["probseg_GM"]["path"].name
-            == f"sub-{test_element}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_GM"]["path"].name
+            == f"{test_element}_space-MNI152NLin2009cAsym_label-"
             "GM_probseg.nii.gz"
         )
 
-        assert out["probseg_GM"]["path"].exists()
-        assert out["probseg_GM"]["path"].is_file()
+        assert out["VBM_GM"]["path"].exists()
+        assert out["VBM_GM"]["path"].is_file()
 
-        # asserts type "probseg_WM"
-        assert "probseg_WM" in out
+        # asserts type "VBM_WM"
+        assert "VBM_WM" in out
 
         assert (
-            out["probseg_WM"]["path"].name
-            == f"sub-{test_element}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_WM"]["path"].name
+            == f"{test_element}_space-MNI152NLin2009cAsym_label-"
             "WM_probseg.nii.gz"
         )
 
-        assert out["probseg_WM"]["path"].exists()
-        assert out["probseg_WM"]["path"].is_file()
+        assert out["VBM_WM"]["path"].exists()
+        assert out["VBM_WM"]["path"].is_file()
 
         # asserts type "DWI"
         assert "DWI" in out
 
         assert (
             out["DWI"]["path"].name
-            == f"sub-{test_element}_desc-preproc_dwi.nii.gz"
+            == f"{test_element}_desc-preproc_dwi.nii.gz"
         )
 
         assert out["DWI"]["path"].exists()
         assert out["DWI"]["path"].is_file()
 
         # asserts meta
         assert "meta" in out["BOLD"]
@@ -128,21 +127,21 @@
 
 @pytest.mark.parametrize(
     "types",
     [
         "BOLD",
         "BOLD_confounds",
         "T1w",
-        "probseg_CSF",
-        "probseg_GM",
-        "probseg_WM",
+        "VBM_CSF",
+        "VBM_GM",
+        "VBM_WM",
         "DWI",
         ["BOLD", "BOLD_confounds"],
-        ["T1w", "probseg_CSF"],
-        ["probseg_GM", "probseg_WM"],
+        ["T1w", "VBM_CSF"],
+        ["VBM_GM", "VBM_WM"],
         ["DWI", "BOLD"],
     ],
 )
 def test_DataladAOMICID1000_partial_data_access(
     types: Union[str, List[str]],
 ) -> None:
     """Test DataladAOMICID1000 DataGrabber partial data access.
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,89 +52,89 @@
             "gstroop": "seq",
             "restingstate": "mb3",
             "workingmemory": "seq",
         }
         acq = task_acqs[task]
         new_task = f"{task}_acq-{acq}"
         assert (
-            out["BOLD"]["path"].name == f"sub-{sub}_task-{new_task}_"
+            out["BOLD"]["path"].name == f"{sub}_task-{new_task}_"
             "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
         )
 
         assert out["BOLD"]["path"].exists()
         assert out["BOLD"]["path"].is_file()
 
         # asserts type "BOLD_confounds"
         assert "BOLD_confounds" in out
 
         assert (
-            out["BOLD_confounds"]["path"].name == f"sub-{sub}_task-{new_task}_"
+            out["BOLD_confounds"]["path"].name == f"{sub}_task-{new_task}_"
             "desc-confounds_regressors.tsv"
         )
 
         assert out["BOLD_confounds"]["path"].exists()
         assert out["BOLD_confounds"]["path"].is_file()
 
         # assert BOLD_mask
         assert out["BOLD_mask"]["path"].exists()
 
         # asserts type "T1w"
         assert "T1w" in out
 
         assert (
-            out["T1w"]["path"].name == f"sub-{sub}_space-MNI152NLin2009cAsym_"
+            out["T1w"]["path"].name == f"{sub}_space-MNI152NLin2009cAsym_"
             "desc-preproc_T1w.nii.gz"
         )
 
         assert out["T1w"]["path"].exists()
         assert out["T1w"]["path"].is_file()
 
         # asserts T1w_mask
         assert out["T1w_mask"]["path"].exists()
 
-        # asserts type "probseg_CSF"
-        assert "probseg_CSF" in out
+        # asserts type "VBM_CSF"
+        assert "VBM_CSF" in out
 
         assert (
-            out["probseg_CSF"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_CSF"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "CSF_probseg.nii.gz"
         )
 
-        assert out["probseg_CSF"]["path"].exists()
-        assert out["probseg_CSF"]["path"].is_file()
+        assert out["VBM_CSF"]["path"].exists()
+        assert out["VBM_CSF"]["path"].is_file()
 
-        # asserts type "probseg_GM"
-        assert "probseg_GM" in out
+        # asserts type "VBM_GM"
+        assert "VBM_GM" in out
 
         assert (
-            out["probseg_GM"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_GM"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "GM_probseg.nii.gz"
         )
 
-        assert out["probseg_GM"]["path"].exists()
-        assert out["probseg_GM"]["path"].is_file()
+        assert out["VBM_GM"]["path"].exists()
+        assert out["VBM_GM"]["path"].is_file()
 
-        # asserts type "probseg_WM"
-        assert "probseg_WM" in out
+        # asserts type "VBM_WM"
+        assert "VBM_WM" in out
 
         assert (
-            out["probseg_WM"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_WM"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "WM_probseg.nii.gz"
         )
 
-        assert out["probseg_WM"]["path"].exists()
-        assert out["probseg_WM"]["path"].is_file()
+        assert out["VBM_WM"]["path"].exists()
+        assert out["VBM_WM"]["path"].is_file()
 
         # asserts type "DWI"
         assert "DWI" in out
 
-        assert out["DWI"]["path"].name == f"sub-{sub}_desc-preproc_dwi.nii.gz"
+        assert out["DWI"]["path"].name == f"{sub}_desc-preproc_dwi.nii.gz"
 
         assert out["DWI"]["path"].exists()
         assert out["DWI"]["path"].is_file()
 
         # asserts meta
         assert "meta" in out["BOLD"]
         meta = out["BOLD"]["meta"]
@@ -145,21 +145,21 @@
 
 @pytest.mark.parametrize(
     "types",
     [
         "BOLD",
         "BOLD_confounds",
         "T1w",
-        "probseg_CSF",
-        "probseg_GM",
-        "probseg_WM",
+        "VBM_CSF",
+        "VBM_GM",
+        "VBM_WM",
         "DWI",
         ["BOLD", "BOLD_confounds"],
-        ["T1w", "probseg_CSF"],
-        ["probseg_GM", "probseg_WM"],
+        ["T1w", "VBM_CSF"],
+        ["VBM_GM", "VBM_WM"],
         ["DWI", "BOLD"],
     ],
 )
 def test_DataladAOMICPIOP1_partial_data_access(
     types: Union[str, List[str]],
 ) -> None:
     """Test DataladAOMICPIOP1 DataGrabber partial data access.
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.5.dev11/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,89 +46,89 @@
         out = dg[test_element]
 
         # asserts type "BOLD"
         assert "BOLD" in out
 
         new_task = f"{task}_acq-seq"
         assert (
-            out["BOLD"]["path"].name == f"sub-{sub}_task-{new_task}_"
+            out["BOLD"]["path"].name == f"{sub}_task-{new_task}_"
             "space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"
         )
 
         assert out["BOLD"]["path"].exists()
         assert out["BOLD"]["path"].is_file()
 
         # asserts type "BOLD_confounds"
         assert "BOLD_confounds" in out
 
         assert (
-            out["BOLD_confounds"]["path"].name == f"sub-{sub}_task-{new_task}_"
+            out["BOLD_confounds"]["path"].name == f"{sub}_task-{new_task}_"
             "desc-confounds_regressors.tsv"
         )
 
         assert out["BOLD_confounds"]["path"].exists()
         assert out["BOLD_confounds"]["path"].is_file()
 
         # assert BOLD_mask
         assert out["BOLD_mask"]["path"].exists()
 
         # asserts type "T1w"
         assert "T1w" in out
 
         assert (
-            out["T1w"]["path"].name == f"sub-{sub}_space-MNI152NLin2009cAsym_"
+            out["T1w"]["path"].name == f"{sub}_space-MNI152NLin2009cAsym_"
             "desc-preproc_T1w.nii.gz"
         )
 
         assert out["T1w"]["path"].exists()
         assert out["T1w"]["path"].is_file()
 
         # asserts T1w_mask
         assert out["T1w_mask"]["path"].exists()
 
-        # asserts type "probseg_CSF"
-        assert "probseg_CSF" in out
+        # asserts type "VBM_CSF"
+        assert "VBM_CSF" in out
 
         assert (
-            out["probseg_CSF"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_CSF"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "CSF_probseg.nii.gz"
         )
 
-        assert out["probseg_CSF"]["path"].exists()
-        assert out["probseg_CSF"]["path"].is_file()
+        assert out["VBM_CSF"]["path"].exists()
+        assert out["VBM_CSF"]["path"].is_file()
 
-        # asserts type "probseg_GM"
-        assert "probseg_GM" in out
+        # asserts type "VBM_GM"
+        assert "VBM_GM" in out
 
         assert (
-            out["probseg_GM"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_GM"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "GM_probseg.nii.gz"
         )
 
-        assert out["probseg_GM"]["path"].exists()
-        assert out["probseg_GM"]["path"].is_file()
+        assert out["VBM_GM"]["path"].exists()
+        assert out["VBM_GM"]["path"].is_file()
 
-        # asserts type "probseg_WM"
-        assert "probseg_WM" in out
+        # asserts type "VBM_WM"
+        assert "VBM_WM" in out
 
         assert (
-            out["probseg_WM"]["path"].name
-            == f"sub-{sub}_space-MNI152NLin2009cAsym_label-"
+            out["VBM_WM"]["path"].name
+            == f"{sub}_space-MNI152NLin2009cAsym_label-"
             "WM_probseg.nii.gz"
         )
 
-        assert out["probseg_WM"]["path"].exists()
-        assert out["probseg_WM"]["path"].is_file()
+        assert out["VBM_WM"]["path"].exists()
+        assert out["VBM_WM"]["path"].is_file()
 
         # asserts type "DWI"
         assert "DWI" in out
 
-        assert out["DWI"]["path"].name == f"sub-{sub}_desc-preproc_dwi.nii.gz"
+        assert out["DWI"]["path"].name == f"{sub}_desc-preproc_dwi.nii.gz"
 
         assert out["DWI"]["path"].exists()
         assert out["DWI"]["path"].is_file()
 
         # asserts meta
         assert "meta" in out["BOLD"]
         meta = out["BOLD"]["meta"]
@@ -139,21 +139,21 @@
 
 @pytest.mark.parametrize(
     "types",
     [
         "BOLD",
         "BOLD_confounds",
         "T1w",
-        "probseg_CSF",
-        "probseg_GM",
-        "probseg_WM",
+        "VBM_CSF",
+        "VBM_GM",
+        "VBM_WM",
         "DWI",
         ["BOLD", "BOLD_confounds"],
-        ["T1w", "probseg_CSF"],
-        ["probseg_GM", "probseg_WM"],
+        ["T1w", "VBM_CSF"],
+        ["VBM_GM", "VBM_WM"],
         ["DWI", "BOLD"],
     ],
 )
 def test_DataladAOMICPIOP2_partial_data_access(
     types: Union[str, List[str]],
 ) -> None:
     """Test DataladAOMICPIOP2 DataGrabber partial data access.
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/base.py` & `junifer-0.0.5.dev11/junifer/datagrabber/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,36 +33,39 @@
         The directory where the data is / will be stored.
 
     """
 
     def __init__(self, types: List[str], datadir: Union[str, Path]) -> None:
         # Validate types
         validate_types(types)
+        self.types = types
+
         # Convert str to Path
         if not isinstance(datadir, Path):
             datadir = Path(datadir)
+        self._datadir = datadir
 
         logger.debug("Initializing BaseDataGrabber")
         logger.debug(f"\t_datadir = {datadir}")
         logger.debug(f"\ttypes = {types}")
-        self._datadir = datadir
-        self.types = types
 
     def __iter__(self) -> Iterator:
         """Enable iterable support.
 
         Yields
         ------
         object
             An element that can be indexed by the DataGrabber.
 
         """
         yield from self.get_elements()
 
-    def __getitem__(self, element: Union[str, Tuple[str]]) -> Dict[str, Dict]:
+    def __getitem__(
+        self, element: Union[str, Tuple[str, ...]]
+    ) -> Dict[str, Dict]:
         """Enable indexing support.
 
         Parameters
         ----------
         element : str or tuple of str
             The element to be indexed.
 
@@ -70,20 +73,24 @@
         -------
         dict
             Dictionary of paths for each type of data required for the
             specified element.
 
         """
         logger.info(f"Getting element {element}")
+        # Convert element to tuple if not already
         if not isinstance(element, tuple):
             element = (element,)
-        named_element = dict(zip(self.get_element_keys(), element))
+        # Zip through element keys and actual values to construct element
+        # access dictionary
+        named_element: Dict = dict(zip(self.get_element_keys(), element))
         logger.debug(f"Named element: {named_element}")
+        # Fetch element
         out = self.get_item(**named_element)
-
+        # Update metadata
         for _, t_val in out.items():
             self.update_meta(t_val, "datagrabber")
             t_val["meta"]["element"] = named_element
 
         return out
 
     def __enter__(self) -> "BaseDataGrabber":
@@ -174,15 +181,15 @@
         list of str
             The element keys.
 
         """
         raise_error(
             msg="Concrete classes need to implement get_element_keys().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
 
     @abstractmethod
     def get_elements(self) -> List[Union[str, Tuple[str]]]:
         """Get elements.
 
         Returns
         -------
@@ -191,15 +198,15 @@
             tuples or any object that will be then used as a key to index the
             DataGrabber.
 
         """
         raise_error(
             msg="Concrete classes need to implement get_elements().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
 
     @abstractmethod
     def get_item(self, **element: Dict) -> Dict[str, Dict]:
         """Get the specified item from the dataset.
 
         Parameters
         ----------
@@ -212,8 +219,8 @@
             Dictionary of paths for each type of data required for the
             specified element.
 
         """
         raise_error(
             msg="Concrete classes need to implement get_item().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/datalad_base.py` & `junifer-0.0.5.dev11/junifer/datagrabber/datalad_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 from typing import Dict, Optional, Tuple, Union
 
 import datalad
 import datalad.api as dl
 from datalad.support.exceptions import IncompleteResultsError
 from datalad.support.gitrepo import GitRepo
 
-from ..api.decorators import register_datagrabber
 from ..utils import logger, raise_error, warn_with_log
 from .base import BaseDataGrabber
 
 
-@register_datagrabber
 class DataladDataGrabber(BaseDataGrabber):
     """Abstract base class for datalad-based data fetching.
 
     Defines a DataGrabber that gets data from a datalad sibling.
 
     Parameters
     ----------
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,19 @@
         HCP phase encoding directions. If None, both will be used
         (default None).
     ica_fix : bool, optional
         Whether to retrieve data that was processed with ICA+FIX.
         Only "REST1" and "REST2" tasks are available with ICA+FIX (default
         False).
 
+    Raises
+    ------
+    ValueError
+        If invalid value is passed for ``tasks`` or ``phase_encodings``.
+
     """
 
     def __init__(
         self,
         datadir: Union[str, Path, None] = None,
         tasks: Union[str, List[str], None] = None,
         phase_encodings: Union[str, List[str], None] = None,
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,26 +30,28 @@
     phase_encodings : {"LR", "RL"} or list of the options or None, optional
         HCP phase encoding directions. If None, both will be used
         (default None).
     ica_fix : bool, optional
         Whether to retrieve data that was processed with ICA+FIX.
         Only "REST1" and "REST2" tasks are available with ICA+FIX (default
         False).
-    **kwargs
-        Keyword arguments passed to superclass.
+
+    Raises
+    ------
+    ValueError
+        If invalid value is passed for ``tasks`` or ``phase_encodings``.
 
     """
 
     def __init__(
         self,
         datadir: Union[str, Path],
         tasks: Union[str, List[str], None] = None,
         phase_encodings: Union[str, List[str], None] = None,
         ica_fix: bool = False,
-        **kwargs,
     ) -> None:
         # All tasks
         all_tasks = [
             "REST1",
             "REST2",
             "SOCIAL",
             "WM",
@@ -70,14 +72,15 @@
             for task in tasks:
                 if task not in all_tasks:
                     raise_error(
                         f"'{task}' is not a valid HCP-YA fMRI task input. "
                         f"Valid task values can be any or all of {all_tasks}."
                     )
             self.tasks: List[str] = tasks
+
         # All phase encodings
         all_phase_encodings = ["LR", "RL"]
         # Set phase encodings
         if phase_encodings is None:
             phase_encodings = all_phase_encodings
         # Convert single phase encoding into list
         if isinstance(phase_encodings, str):
@@ -86,41 +89,56 @@
         for pe in phase_encodings:
             if pe not in all_phase_encodings:
                 raise_error(
                     f"'{pe}' is not a valid HCP-YA phase encoding. "
                     "Valid phase encoding can be any or all of "
                     f"{all_phase_encodings}."
                 )
+        self.phase_encodings = phase_encodings
 
         if ica_fix:
             if not all(task in ["REST1", "REST2"] for task in self.tasks):
                 raise_error(
                     "ICA+FIX is only available for 'REST1' and 'REST2' tasks."
                 )
         suffix = "_hp2000_clean" if ica_fix else ""
+
         # The types of data
-        types = ["BOLD"]
+        types = ["BOLD", "T1w", "Warp"]
         # The patterns
         patterns = {
-            "BOLD": (
-                "{subject}/MNINonLinear/Results/"
-                "{task}_{phase_encoding}/"
-                "{task}_{phase_encoding}"
-                f"{suffix}.nii.gz"
-            )
+            "BOLD": {
+                "pattern": (
+                    "{subject}/MNINonLinear/Results/"
+                    "{task}_{phase_encoding}/"
+                    "{task}_{phase_encoding}"
+                    f"{suffix}.nii.gz"
+                ),
+                "space": "MNI152NLin6Asym",
+            },
+            "T1w": {
+                "pattern": "{subject}/T1w/T1w_acpc_dc_restore.nii.gz",
+                "space": "native",
+            },
+            "Warp": {
+                "pattern": (
+                    "{subject}/MNINonLinear/xfms/standard2acpc_dc.nii.gz"
+                ),
+                "src": "MNI152NLin6Asym",
+                "dst": "native",
+            },
         }
         # The replacements
         replacements = ["subject", "task", "phase_encoding"]
         super().__init__(
             types=types,
             datadir=datadir,
             patterns=patterns,
             replacements=replacements,
         )
-        self.phase_encodings = phase_encodings
 
     def get_item(self, subject: str, task: str, phase_encoding: str) -> Dict:
         """Implement single element indexing in the database.
 
         Parameters
         ----------
         subject : str
@@ -140,18 +158,17 @@
         """
         # Resting task
         if "REST" in task:
             new_task = f"rfMRI_{task}"
         else:
             new_task = f"tfMRI_{task}"
 
-        out = super().get_item(
+        return super().get_item(
             subject=subject, task=new_task, phase_encoding=phase_encoding
         )
-        return out
 
     def get_elements(self) -> List:
         """Implement fetching list of elements in the dataset.
 
         Returns
         -------
         list
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.5.dev11/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/multiple.py` & `junifer-0.0.5.dev11/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/pattern.py` & `junifer-0.0.5.dev11/junifer/datagrabber/pattern.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,56 +28,153 @@
     Implements a DataGrabber that understands patterns to grab data.
 
     Parameters
     ----------
     types : list of str
         The types of data to be grabbed.
     patterns : dict
-        Patterns for each type of data as a dictionary. The keys are the types
-        and the values are the patterns. Each occurrence of the string
-        ``{subject}`` in the pattern will be replaced by the indexed element.
+        Data type patterns as a dictionary. It has the following schema:
+
+        * ``"T1w"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "space"],
+              "optional": []
+            }
+
+        * ``"T2w"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "space"],
+              "optional": []
+            }
+
+        * ``"BOLD"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "space"],
+              "optional": ["mask_item"]
+            }
+
+        * ``"Warp"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "src", "dst"],
+              "optional": []
+            }
+
+        * ``"BOLD_confounds"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "format"],
+              "optional": []
+            }
+
+        * ``"VBM_GM"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "space"],
+              "optional": []
+            }
+
+        * ``"VBM_WM"`` :
+
+          .. code-block:: none
+
+            {
+              "mandatory": ["pattern", "space"],
+              "optional": []
+            }
+
+        Basically, for each data type, one needs to provide ``mandatory`` keys
+        and can choose to also provide ``optional`` keys. The value for each
+        key is a string. So, one needs to provide necessary data types as a
+        dictionary, for example:
+
+        .. code-block:: none
+
+          {
+              "BOLD": {
+                "pattern": "...",
+                "space": "...",
+              },
+              "T1w": {
+                "pattern": "...",
+                "space": "...",
+              },
+              "Warp": {
+                "pattern": "...",
+                "src": "...",
+                "dst": "...",
+              }
+          }
+
+        taken from :class:`.HCP1200`.
     replacements : str or list of str
-        Replacements in the patterns for each item in the "element" tuple.
+        Replacements in the ``pattern`` key of each data type. The value needs
+        to be a list of all possible replacements.
     datadir : str or pathlib.Path
         The directory where the data is / will be stored.
     confounds_format : {"fmriprep", "adhoc"} or None, optional
         The format of the confounds for the dataset (default None).
 
+    Raises
+    ------
+    ValueError
+        If ``confounds_format`` is invalid.
+
     """
 
     def __init__(
         self,
         types: List[str],
-        patterns: Dict[str, str],
+        patterns: Dict[str, Dict[str, str]],
         replacements: Union[List[str], str],
         datadir: Union[str, Path],
         confounds_format: Optional[str] = None,
     ) -> None:
         # Validate patterns
         validate_patterns(types=types, patterns=patterns)
+        self.patterns = patterns
 
+        # Convert replacements to list if not already
         if not isinstance(replacements, list):
             replacements = [replacements]
         # Validate replacements
         validate_replacements(replacements=replacements, patterns=patterns)
+        self.replacements = replacements
 
         # Validate confounds format
-        if confounds_format and confounds_format not in _CONFOUNDS_FORMATS:
+        if (
+            confounds_format is not None
+            and confounds_format not in _CONFOUNDS_FORMATS
+        ):
             raise_error(
                 "Invalid value for `confounds_format`, should be one of "
                 f"{_CONFOUNDS_FORMATS}."
             )
         self.confounds_format = confounds_format
 
         super().__init__(types=types, datadir=datadir)
         logger.debug("Initializing PatternDataGrabber")
         logger.debug(f"\tpatterns = {patterns}")
         logger.debug(f"\treplacements = {replacements}")
-        self.patterns = patterns
-        self.replacements = replacements
+        logger.debug(f"\tconfounds_format = {confounds_format}")
 
     @property
     def skip_file_check(self) -> bool:
         """Skip file check existence."""
         return False
 
     def _replace_patterns_regex(
@@ -132,14 +229,19 @@
             The pattern to be replaced.
 
         Returns
         -------
         str
             The pattern with the element replaced.
 
+        Raises
+        ------
+        ValueError
+            If element keys do not match with replacements.
+
         """
         if list(element.keys()) != self.replacements:
             raise_error(
                 f"The element keys must be {self.replacements}, "
                 f"element has {list(element.keys())}."
             )
         return pattern.format(**element)
@@ -156,15 +258,15 @@
         list of str
             The element keys.
 
         """
         return self.replacements
 
     def get_item(self, **element: str) -> Dict[str, Dict]:
-        """Implement single element indexing in the database.
+        """Implement single element indexing for the datagrabber.
 
         This method constructs a real path to the requested item's data, by
         replacing the ``patterns`` with actual values passed via ``**element``.
 
         Parameters
         ----------
         element : dict
@@ -173,51 +275,55 @@
 
         Returns
         -------
         dict
             Dictionary of dictionaries for each type of data required for the
             specified element.
 
+        Raises
+        ------
+        RuntimeError
+            If more than one file matches for a data type's pattern or
+            if no file matches for a data type's pattern or
+            if file cannot be accessed for an element.
+
         """
         out = {}
         for t_type in self.types:
             t_pattern = self.patterns[t_type]
-            t_replace = self._replace_patterns_glob(element, t_pattern)
+            t_replace = self._replace_patterns_glob(
+                element, t_pattern["pattern"]
+            )
             if "*" in t_replace:
                 t_matches = list(self.datadir.absolute().glob(t_replace))
                 if len(t_matches) > 1:
                     raise_error(
                         f"More than one file matches for {element} / {t_type}:"
-                        f" {t_matches}"
+                        f" {t_matches}",
+                        klass=RuntimeError,
                     )
                 elif len(t_matches) == 0:
-                    raise_error(f"No file matches for {element} / {t_type}")
+                    raise_error(
+                        f"No file matches for {element} / {t_type}",
+                        klass=RuntimeError,
+                    )
                 t_out = t_matches[0]
             else:
                 t_out = self.datadir / t_replace
                 if not self.skip_file_check:
                     if not t_out.exists() and not t_out.is_symlink():
                         raise_error(
                             f"Cannot access {t_type} for {element}: "
-                            f"File {t_out} does not exist"
+                            f"File {t_out} does not exist",
+                            klass=RuntimeError,
                         )
             # Update path for the element
-            out[t_type] = {"path": t_out}
-            # Update confounds format for BOLD_confounds
-            # (if found in the datagrabber)
-            if t_type == "BOLD_confounds":
-                if not self.confounds_format:
-                    raise_error(
-                        "`confounds_format` needs to be one of "
-                        f"{_CONFOUNDS_FORMATS}, None provided. "
-                        "As the DataGrabber used specifies "
-                        "'BOLD_confounds', None is invalid."
-                    )
-                # Set the format
-                out[t_type].update({"format": self.confounds_format})
+            out[t_type] = t_pattern.copy()  # copy data type dictionary
+            out[t_type].pop("pattern")  # remove pattern key
+            out[t_type].update({"path": t_out})  # add path key
 
         return out
 
     def get_elements(self) -> List:
         """Implement fetching list of elements in the dataset.
 
         It will use regex to search for "replacements" in the "patterns" and
@@ -248,15 +354,15 @@
             # Get the pattern
             t_pattern = self.patterns[t_type]
             # Replace the pattern
             (
                 re_pattern,
                 glob_pattern,
                 t_replacements,
-            ) = self._replace_patterns_regex(t_pattern)
+            ) = self._replace_patterns_regex(t_pattern["pattern"])
             for fname in self.datadir.glob(glob_pattern):
                 suffix = fname.relative_to(self.datadir).as_posix()
                 m = re.match(re_pattern, suffix)
                 if m is not None:
                     # Find the groups of replacements present in the pattern
                     # If one replacement is not present, set it to None.
                     # We will take care of this in the intersection
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.5.dev11/junifer/datagrabber/tests/test_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,14 @@
 from pathlib import Path
 
 import pytest
 
 from junifer.datagrabber import BaseDataGrabber
 
 
-def test_BaseDataGrabber_abstractness() -> None:
-    """Test BaseDataGrabber is abstract base class."""
-    with pytest.raises(TypeError, match=r"abstract"):
-        BaseDataGrabber(datadir="/tmp", types=["func"])  # type: ignore
-
-
 def test_BaseDataGrabber() -> None:
     """Test BaseDataGrabber."""
 
     # Create concrete class.
     class MyDataGrabber(BaseDataGrabber):
         def get_item(self, subject):
             return {"BOLD": {}}
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.5.dev11/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,14 @@
         "uri": "https://gin.g-node.org/juaml/datalad-example-bids-ses",
         "commit": "3d08d55d1faad4f12ab64ac9497544a0d924d47a",
         "id": "c83500d0-532f-45be-baf1-0dab703bdc2a",
     },
 }
 
 
-def test_DataladDataGrabber_abstractness() -> None:
-    """Test DataladDataGrabber is abstract base class."""
-    with pytest.raises(TypeError, match=r"abstract"):
-        DataladDataGrabber()  # type: ignore
-
-
 @pytest.fixture
 def concrete_datagrabber() -> Type[DataladDataGrabber]:
     """Return a concrete datalad-based DataGrabber.
 
     Returns
     -------
     DataladDataGrabber
```

### Comparing `junifer-0.0.4.dev90/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.5.dev11/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,16 +39,22 @@
 
 def test_bids_PatternDataladDataGrabber() -> None:
     """Test subject-based BIDS PatternDataladDataGrabber."""
     # Define types
     types = ["T1w", "BOLD"]
     # Define patterns
     patterns = {
-        "T1w": "{subject}/anat/{subject}_T1w.nii.gz",
-        "BOLD": "{subject}/func/{subject}_task-rest_bold.nii.gz",
+        "T1w": {
+            "pattern": "{subject}/anat/{subject}_T1w.nii.gz",
+            "space": "MNI152NLin6Asym",
+        },
+        "BOLD": {
+            "pattern": "{subject}/func/{subject}_task-rest_bold.nii.gz",
+            "space": "MNI152NLin6Asym",
+        },
     }
     # Define replacements
     replacements = ["subject"]
 
     repo_uri = _testing_dataset["example_bids"]["uri"]
     rootdir = "example_bids"
     repo_commit = _testing_dataset["example_bids"]["commit"]
@@ -88,39 +94,36 @@
 
             with open(t_sub["T1w"]["path"]) as f:
                 assert f.readlines()[0].startswith("placeholder")
 
 
 def test_bids_PatternDataladDataGrabber_datadir() -> None:
     """Test PatternDataladDataGrabber with a datadir set to a relative path."""
-    # Define types
-    types = ["T1w", "BOLD"]
     # Define patterns
     patterns = {
-        "T1w": "{subject}/anat/{subject}_T1w.nii.gz",
-        "BOLD": "{subject}/func/{subject}_task-rest_bold.nii.gz",
+        "T1w": {
+            "pattern": "{subject}/anat/{subject}_T*w.nii.gz",
+            "space": "MNI152NLin6Asym",
+        },
+        "BOLD": {
+            "pattern": "{subject}/func/{subject}_task-rest_*.nii.gz",
+            "space": "MNI152NLin6Asym",
+        },
     }
-    # Define replacements
-    replacements = ["subject"]
-
-    repo_uri = _testing_dataset["example_bids"]["uri"]
-
+    # Define datadir
     datadir = "dataset"  # use string and not absolute path
-    patterns = {
-        "T1w": "example_bids/{subject}/anat/{subject}_T*w.nii.gz",
-        "BOLD": "example_bids/{subject}/func/{subject}_task-rest_*.nii.gz",
-    }
     with PatternDataladDataGrabber(
-        uri=repo_uri,
-        types=types,
+        uri=_testing_dataset["example_bids"]["uri"],
+        types=["T1w", "BOLD"],
         patterns=patterns,
         datadir=datadir,
-        replacements=replacements,
+        rootdir="example_bids",
+        replacements=["subject"],
     ) as dg:
-        assert dg.datadir == Path(datadir)
+        assert dg.datadir == Path(datadir) / "example_bids"
         for elem in dg:
             t_sub = dg[elem]
             assert "path" in t_sub["T1w"]
             assert t_sub["T1w"]["path"] == (
                 dg.datadir / f"{elem}/anat/{elem}_T1w.nii.gz"
             )
             assert "path" in t_sub["BOLD"]
@@ -129,52 +132,68 @@
             )
 
 
 def test_bids_PatternDataladDataGrabber_session():
     """Test a subject and session-based BIDS PatternDataladDataGrabber."""
     types = ["T1w", "BOLD"]
     patterns = {
-        "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
-        "BOLD": "{subject}/{session}/func/"
-        "{subject}_{session}_task-rest_bold.nii.gz",
+        "T1w": {
+            "pattern": (
+                "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz"
+            ),
+            "space": "MNI152NLin6Asym",
+        },
+        "BOLD": {
+            "pattern": (
+                "{subject}/{session}/func/"
+                "{subject}_{session}_task-rest_bold.nii.gz"
+            ),
+            "space": "MNI152NLin6Asym",
+        },
     }
     replacements = ["subject", "session"]
 
+    # Check error
     with pytest.raises(ValueError, match=r"`uri` must be provided"):
         PatternDataladDataGrabber(
             datadir=None,
             types=types,
             patterns=patterns,
             replacements=replacements,
         )
 
+    # Set parameters
     repo_uri = _testing_dataset["example_bids_ses"]["uri"]
     rootdir = "example_bids_ses"
-    # repo_commit =  _testing_dataset['example_bids_ses']['id']
 
     # With T1W and bold, only 2 sessions are available
     with PatternDataladDataGrabber(
         rootdir=rootdir,
         uri=repo_uri,
         types=types,
         patterns=patterns,
         replacements=replacements,
     ) as dg:
-        subs = list(dg)
+        subs = list(dg.get_elements())
         expected_subs = [
             (f"sub-{i:02d}", f"ses-{j:02d}")
             for j in range(1, 3)
             for i in range(1, 10)
         ]
         assert set(subs) == set(expected_subs)
 
     # Test with a different T1w only, it should have 3 sessions
     types = ["T1w"]
     patterns = {
-        "T1w": "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz",
+        "T1w": {
+            "pattern": (
+                "{subject}/{session}/anat/{subject}_{session}_T1w.nii.gz"
+            ),
+            "space": "MNI152NLin6Asym",
+        },
     }
     with PatternDataladDataGrabber(
         rootdir=rootdir,
         uri=repo_uri,
         types=types,
         patterns=patterns,
         replacements=replacements,
```

### Comparing `junifer-0.0.4.dev90/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.5.dev11/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.5.dev11/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.5.dev11/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.5.dev11/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev11/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     -------
     X : 2D numpy.ndarray
         Signal for each brain voxel in the (masked) niimgs.
         shape: (number of scans, number of voxels)
     A : scipy.sparse.lil_matrix
         Contains the boolean indices for each sphere.
         shape: (number of seeds, number of voxels)
+
     """
     seeds = list(seeds)
 
     # Compute world coordinates of all in-mask voxels.
     if niimg is None:
         mask, affine = masking._load_mask_img(mask_img)
         # Get coordinate for all voxels inside of mask
@@ -200,14 +201,15 @@
         Indicates, in millimeters, the radius for the sphere around the seed.
     allow_overlap: boolean
         If False, an error is raised if the maps overlaps (ie at least two
         maps have a non-zero value for the same voxel).
     mask_img : Niimg-like object, optional
         See :ref:`extracting_data`.
         Mask to apply to regions before extracting signals.
+
     """
     X, A = _apply_mask_and_get_affinity(
         seeds, niimg, radius, allow_overlap, mask_img=mask_img
     )
     for _, row in enumerate(A.rows):
         yield X[:, row]
```

### Comparing `junifer-0.0.4.dev90/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev11/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/__init__.py` & `junifer-0.0.5.dev11/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/base.py` & `junifer-0.0.5.dev11/junifer/markers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,46 +23,40 @@
     on : str or list of str
         The kind of data to apply the marker to. By default, will work on all
         available data.
     name : str, optional
         The name of the marker. By default, it will use the class name as the
         name of the marker (default None).
 
+    Raises
+    ------
+    ValueError
+        If required input data type(s) is(are) not found.
+
     """
 
     def __init__(
         self,
         on: Optional[Union[List[str], str]] = None,
         name: Optional[str] = None,
     ) -> None:
+        # Use all data types if not provided
         if on is None:
             on = self.get_valid_inputs()
+        # Convert data types to list
         if not isinstance(on, list):
             on = [on]
+        # Set default name if not provided
         self.name = self.__class__.__name__ if name is None else name
-
+        # Check if required inputs are found
         if any(x not in self.get_valid_inputs() for x in on):
             wrong_on = [x for x in on if x not in self.get_valid_inputs()]
-            raise ValueError(f"{self.name} cannot be computed on {wrong_on}")
+            raise_error(f"{self.name} cannot be computed on {wrong_on}")
         self._on = on
 
-    @abstractmethod
-    def get_valid_inputs(self) -> List[str]:
-        """Get valid data types for input.
-
-        Returns
-        -------
-        list of str
-            The list of data types that can be used as input for this marker.
-        """
-        raise_error(
-            msg="Concrete classes need to implement get_valid_inputs().",
-            klass=NotImplementedError,
-        )
-
     def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step. The list must contain the
@@ -85,14 +79,29 @@
                 "Input does not have the required data."
                 f"\t Input: {input}"
                 f"\t Required (any of): {self._on}"
             )
         return [x for x in self._on if x in input]
 
     @abstractmethod
+    def get_valid_inputs(self) -> List[str]:
+        """Get valid data types for input.
+
+        Returns
+        -------
+        list of str
+            The list of data types that can be used as input for this marker.
+
+        """
+        raise_error(
+            msg="Concrete classes need to implement get_valid_inputs().",
+            klass=NotImplementedError,
+        )
+
+    @abstractmethod
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
         input_type : str
             The data type input to the marker.
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/collection.py` & `junifer-0.0.5.dev11/junifer/markers/collection.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 # License: AGPL
 
 from collections import Counter
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 from ..datareader.default import DefaultDataReader
 from ..markers.base import BaseMarker
-from ..pipeline import PipelineStepMixin
+from ..pipeline import PipelineStepMixin, WorkDirManager
+from ..preprocess.base import BasePreprocessor
 from ..storage.base import BaseFeatureStorage
-from ..utils import logger
+from ..utils import logger, raise_error
 
 
 if TYPE_CHECKING:
     from junifer.datagrabber import BaseDataGrabber
 
 
 class MarkerCollection:
@@ -23,41 +24,46 @@
 
     Parameters
     ----------
     markers : list of marker-like
         The markers to compute.
     datareader : DataReader-like object, optional
         The DataReader to use (default None).
-    preprocessing : preprocessing-like, optional
-        The preprocessing steps to apply.
+    preprocessors : list of preprocessing-like, optional
+        The preprocessors to apply (default None).
     storage : storage-like, optional
         The storage to use (default None).
 
+    Raises
+    ------
+    ValueError
+        If ``markers`` have same names.
+
     """
 
     def __init__(
         self,
         markers: List[BaseMarker],
         datareader: Optional[PipelineStepMixin] = None,
-        preprocessing: Optional[PipelineStepMixin] = None,
+        preprocessors: Optional[List[BasePreprocessor]] = None,
         storage: Optional[BaseFeatureStorage] = None,
     ):
         # Check that the markers have different names
         marker_names = [m.name for m in markers]
         if len(set(marker_names)) != len(marker_names):
             counts = Counter(marker_names)
-            raise ValueError(
+            raise_error(
                 "Markers must have different names. "
                 f"Current names are: {counts}"
             )
         self._markers = markers
         if datareader is None:
             datareader = DefaultDataReader()
         self._datareader = datareader
-        self._preprocessing = preprocessing
+        self._preprocessors = preprocessors
         self._storage = storage
 
     def fit(self, input: Dict[str, Dict]) -> Optional[Dict]:
         """Fit the pipeline.
 
         Parameters
         ----------
@@ -75,36 +81,44 @@
         """
         logger.info("Fitting pipeline")
 
         # Fetch actual data using datareader
         data = self._datareader.fit_transform(input)
 
         # Apply preprocessing steps
-        if self._preprocessing is not None:
-            logger.info("Preprocessing data")
-            data = self._preprocessing.fit_transform(data)
+        if self._preprocessors is not None:
+            for preprocessor in self._preprocessors:
+                logger.info(
+                    "Preprocessing data with "
+                    f"{preprocessor.__class__.__name__}"
+                )
+                # Mutate data after every iteration
+                data = preprocessor.fit_transform(data)
 
         # Compute markers
         out = {}
         for marker in self._markers:
             logger.info(f"Fitting marker {marker.name}")
             m_value = marker.fit_transform(data, storage=self._storage)
             if self._storage is None:
                 out[marker.name] = m_value
         logger.info("Marker collection fitting done")
 
+        # Cleanup element directory
+        WorkDirManager().cleanup_elementdir()
+
         return None if self._storage else out
 
     def validate(self, datagrabber: "BaseDataGrabber") -> None:
         """Validate the pipeline.
 
         Without doing any computation, check if the marker collection can
-        be fit without problems. That is, the data required for each marker is
+        be fitted without problems i.e., the data required for each marker is
         present and streamed down the steps. Also, if a storage is configured,
-        check that the storage can handle the markers output.
+        check that the storage can handle the markers' output.
 
         Parameters
         ----------
         datagrabber : DataGrabber-like
             The DataGrabber to validate.
 
         """
@@ -112,18 +126,23 @@
         t_data = datagrabber.get_types()
         logger.info(f"DataGrabber output type: {t_data}")
 
         logger.info("Validating Data Reader:")
         t_data = self._datareader.validate(t_data)
         logger.info(f"Data Reader output type: {t_data}")
 
-        if self._preprocessing is not None:
-            logger.info("Validating Preprocessor:")
-            t_data = self._preprocessing.validate(t_data)
-            logger.info(f"Preprocess output type: {t_data}")
+        if self._preprocessors is not None:
+            for preprocessor in self._preprocessors:
+                logger.info(
+                    "Validating Preprocessor: "
+                    f"{preprocessor.__class__.__name__}"
+                )
+                # Validate preprocessor
+                t_data = preprocessor.validate(t_data)
+                logger.info(f"Preprocess output type: {t_data}")
 
         for marker in self._markers:
             logger.info(f"Validating Marker: {marker.name}")
             # Validate marker
             m_data = marker.validate(input=t_data)
             logger.info(f"Marker output type: {m_data}")
             # Check storage for the marker
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/ets_rss.py` & `junifer-0.0.5.dev11/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/falff/falff_base.py` & `junifer-0.0.5.dev11/junifer/markers/falff/falff_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,116 @@
-"""Provide abstract class for computing fALFF."""
+"""Provide base class for ALFF / fALFF."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from abc import abstractmethod
-from typing import ClassVar, Dict, List, Optional, Union
+from pathlib import Path
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
-from ...utils.logging import raise_error
+from ...utils.logging import logger, raise_error
 from ..base import BaseMarker
-from .falff_estimator import ALFFEstimator
+from ._afni_falff import AFNIALFF
+from ._junifer_falff import JuniferALFF
+
+
+if TYPE_CHECKING:
+    from nibabel import Nifti1Image
 
 
 class ALFFBase(BaseMarker):
     """Base class for (fractional) Amplitude Low Frequency Fluctuation.
 
     Parameters
     ----------
     fractional : bool
         Whether to compute fractional ALFF.
     highpass : positive float
         Highpass cutoff frequency.
     lowpass : positive float
         Lowpass cutoff frequency.
+    using : {"junifer", "afni"}
+        Implementation to use for computing ALFF:
+
+        * "junifer" : Use ``junifer``'s own ALFF implementation
+        * "afni" : Use AFNI's ``3dRSFC``
+
     tr : positive float, optional
         The Repetition Time of the BOLD data. If None, will extract
-        the TR from NIFTI header (default None).
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
+        the TR from NIfTI header (default None).
     name : str, optional
         The name of the marker. If None, it will use the class name
         (default None).
 
     Notes
     -----
-        The `tr` parameter is crucial for the correctness of fALFF/ALFF
-        computation. If a dataset is correctly preprocessed, the TR should be
-        extracted from the NIFTI without any issue. However, it has been
-        reported that some preprocessed data might not have the correct TR in
-        the NIFTI header.
+    The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
+    computation. If a dataset is correctly preprocessed, the ``tr`` should be
+    extracted from the NIfTI without any issue. However, it has been
+    reported that some preprocessed data might not have the correct ``tr`` in
+    the NIfTI header.
+
+    Raises
+    ------
+    ValueError
+        If ``highpass`` is not positive or zero or
+        if ``lowpass`` is not positive or
+        if ``highpass`` is higher than ``lowpass`` or
+        if ``using`` is invalid.
 
     """
 
-    _EXT_DEPENDENCIES: ClassVar[
-        List[Dict[str, Union[str, bool, List[str]]]]
-    ] = [
+    _CONDITIONAL_DEPENDENCIES: ClassVar[List[Dict[str, Union[str, Type]]]] = [
+        {
+            "using": "afni",
+            "depends_on": AFNIALFF,
+        },
         {
-            "name": "afni",
-            "optional": True,
-            "commands": ["3dRSFC", "3dAFNItoNIFTI"],
+            "using": "junifer",
+            "depends_on": JuniferALFF,
         },
     ]
 
     def __init__(
         self,
         fractional: bool,
         highpass: float,
         lowpass: float,
+        using: str,
         tr: Optional[float] = None,
-        use_afni: Optional[bool] = None,
         name: Optional[str] = None,
     ) -> None:
         if highpass < 0:
             raise_error("Highpass must be positive or 0")
         if lowpass <= 0:
             raise_error("Lowpass must be positive")
         if highpass >= lowpass:
             raise_error("Highpass must be lower than lowpass")
         self.highpass = highpass
         self.lowpass = lowpass
+        # Validate `using` parameter
+        valid_using = [dep["using"] for dep in self._CONDITIONAL_DEPENDENCIES]
+        if using not in valid_using:
+            raise_error(
+                f"Invalid value for `using`, should be one of: {valid_using}"
+            )
+        self.using = using
         self.tr = tr
-        self.use_afni = use_afni
         self.fractional = fractional
 
         # Create a name based on the class name if none is provided
         if name is None:
             suffix = "_fractional" if fractional else ""
             name = f"{self.__class__.__name__}{suffix}"
         super().__init__(on="BOLD", name=name)
@@ -104,83 +138,56 @@
         -------
         str
             The storage type output by the marker.
 
         """
         return "vector"
 
-    def compute(
+    def _compute(
         self,
-        input: Dict[str, Dict],
-        extra_input: Optional[Dict] = None,
-    ) -> Dict:
-        """Compute.
+        input_data: Dict[str, Any],
+    ) -> Tuple["Nifti1Image", Path]:
+        """Compute ALFF and fALFF.
 
         Parameters
         ----------
-        input : dict
-            A single input from the pipeline data object in which to compute
-            the marker.
+        input_data : dict
+            The input to the marker.
         extra_input : dict, optional
-            The other fields in the pipeline data object. Useful for accessing
-            other data kind that needs to be used in the computation. For
-            example, the functional connectivity markers can make use of the
-            confounds if available (default None).
+            The other fields in the pipeline data object (default None).
 
         Returns
         -------
-        dict
-            The computed result as dictionary. This will be either returned
-            to the user or stored in the storage by calling the store method
-            with this as a parameter. The dictionary has the following keys:
-
-            * ``data`` : the actual computed values as a numpy.ndarray
-            * ``col_names`` : the column labels for the computed values as list
+        Niimg-like object
+            The ALFF / fALFF as NIfTI.
+        pathlib.Path
+            The path to the ALFF / fALFF as NIfTI.
 
         """
-        if self.use_afni is None:
-            raise_error(
-                "Parameter `use_afni` must be set to True or False in order "
-                "to compute this marker. It is currently set to None (default "
-                "behaviour). This is intended to be for auto-detection. In "
-                "order for that to happen, please call the `validate` method "
-                "before calling the `compute` method."
-            )
+        logger.debug("Calculating ALFF and fALFF")
 
-        estimator = ALFFEstimator()
-
-        alff, falff = estimator.fit_transform(
-            use_afni=self.use_afni,
-            input_data=input,
+        # Conditional estimator
+        if self.using == "afni":
+            estimator = AFNIALFF()
+        elif self.using == "junifer":
+            estimator = JuniferALFF()
+        # Compute ALFF + fALFF
+        alff, falff, alff_path, falff_path = estimator.compute(  # type: ignore
+            data=input_data["data"],
             highpass=self.highpass,
             lowpass=self.lowpass,
             tr=self.tr,
         )
-        post_data = falff if self.fractional else alff
-
-        post_input = dict(input.items())
-        post_input["data"] = post_data
-        post_input["path"] = None
-
-        out = self._postprocess(post_input, extra_input=extra_input)
-
-        return out
-
-    @abstractmethod
-    def _postprocess(
-        self, input: Dict, extra_input: Optional[Dict] = None
-    ) -> Dict:
-        """Postprocess the output of the estimator.
 
-        Parameters
-        ----------
-        input : dict
-            The output of the estimator. It must have the following
-        extra_input : dict, optional
-            The other fields in the pipeline data object. Useful for accessing
-            other data kind that needs to be used in the computation. For
-            example, the functional connectivity markers can make use of the
-            confounds if available (default None).
-        """
-        raise_error(
-            "_postprocess must be implemented", klass=NotImplementedError
-        )
+        # If the input data space is native already, the original path should
+        # be propagated down as it might be required for transforming
+        # parcellation / coordinates to native space, else the
+        # path should be passed for use later if required.
+        # TODO(synchon): will be taken care in #292
+        if input_data["space"] == "native" and self.fractional:
+            return falff, input_data["path"]
+        elif input_data["space"] == "native" and not self.fractional:
+            return alff, input_data["path"]
+        elif input_data["space"] != "native" and self.fractional:
+            return falff, falff_path
+        else:
+            return alff, alff_path
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/falff/falff_parcels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,143 @@
-"""Provide class for computing fALFF on parcels."""
+"""Provide class for ALFF / fALFF on parcels."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
-from .. import ParcelAggregation
+from ...utils import logger
+from ..parcel_aggregation import ParcelAggregation
 from .falff_base import ALFFBase
 
 
 @register_marker
 class ALFFParcels(ALFFBase):
-    """Class for computing fALFF/ALFF on parcels.
+    """Class for ALFF / fALFF on parcels.
 
     Parameters
     ----------
     parcellation : str or list of str
         The name(s) of the parcellation(s). Check valid options by calling
         :func:`.list_parcellations`.
     fractional : bool
         Whether to compute fractional ALFF.
+    using : {"junifer", "afni"}
+        Implementation to use for computing ALFF:
+
+        * "junifer" : Use ``junifer``'s own ALFF implementation
+        * "afni" : Use AFNI's ``3dRSFC``
+
     highpass : positive float, optional
         The highpass cutoff frequency for the bandpass filter. If 0,
         it will not apply a highpass filter (default 0.01).
     lowpass : positive float, optional
         The lowpass cutoff frequency for the bandpass filter (default 0.1).
     tr : positive float, optional
         The Repetition Time of the BOLD data. If None, will extract
-        the TR from NIFTI header (default None).
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
+        the TR from NIfTI header (default None).
+    agg_method : str, optional
+        The method to perform aggregation using. Check valid options in
+        :func:`.get_aggfunc_by_name` (default "mean").
+    agg_method_params : dict, optional
+        Parameters to pass to the aggregation function. Check valid options in
+        :func:`.get_aggfunc_by_name` (default None).
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
-    method : str, optional
-        The method to perform aggregation using. Check valid options in
-        :func:`.get_aggfunc_by_name` (default "mean").
-    method_params : dict, optional
-        Parameters to pass to the aggregation function. Check valid options in
-        :func:`.get_aggfunc_by_name`.
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
 
     Notes
     -----
     The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
-    computation. If a dataset is correctly preprocessed, the TR should be
-    extracted from the NIFTI without any issue. However, it has been
-    reported that some preprocessed data might not have the correct TR in
-    the NIFTI header.
+    computation. If a dataset is correctly preprocessed, the ``tr`` should be
+    extracted from the NIfTI without any issue. However, it has been
+    reported that some preprocessed data might not have the correct ``tr`` in
+    the NIfTI header.
 
     ALFF/fALFF are computed using a bandpass butterworth filter. See
     :func:`scipy.signal.butter` and :func:`scipy.signal.filtfilt` for more
     details.
+
     """
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
         fractional: bool,
+        using: str,
         highpass: float = 0.01,
         lowpass: float = 0.1,
         tr: Optional[float] = None,
-        use_afni: Optional[bool] = None,
+        agg_method: str = "mean",
+        agg_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
-        method: str = "mean",
-        method_params: Optional[Dict] = None,
         name: Optional[str] = None,
     ) -> None:
-        self.parcellation = parcellation
-        self.masks = masks
-        self.method = method
-        self.method_params = method_params
+        # Superclass init first to validate `using` parameter
         super().__init__(
             fractional=fractional,
             highpass=highpass,
             lowpass=lowpass,
+            using=using,
             tr=tr,
             name=name,
-            use_afni=use_afni,
         )
+        self.parcellation = parcellation
+        self.agg_method = agg_method
+        self.agg_method_params = agg_method_params
+        self.masks = masks
 
-    def _postprocess(
-        self, input: Dict, extra_input: Optional[Dict] = None
-    ) -> Dict:
-        """Compute ALFF and fALFF.
+    def compute(
+        self,
+        input: Dict[str, Any],
+        extra_input: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Compute.
 
         Parameters
         ----------
         input : dict
-            A single input from the pipeline data object in which to compute
-            the marker.
+            The BOLD data as dictionary.
         extra_input : dict, optional
-            The other fields in the pipeline data object. Useful for accessing
-            other data kind that needs to be used in the computation. For
-            example, the functional connectivity markers can make use of the
-            confounds if available (default None).
+            The other fields in the pipeline data object (default None).
 
         Returns
         -------
         dict
-            The computed ALFF as dictionary. The dictionary has the following
+            The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
 
         """
-        pa = ParcelAggregation(
+        logger.info("Calculating ALFF / fALFF for parcels")
+
+        # Compute ALFF / fALFF
+        output_data, output_file_path = self._compute(input_data=input)
+
+        # Initialize parcel aggregation
+        parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
-            method=self.method,
-            method_params=self.method_params,
+            method=self.agg_method,
+            method_params=self.agg_method_params,
             masks=self.masks,
-            on="fALFF",
+            on="BOLD",
+        )
+        # Perform aggregation on ALFF / fALFF
+        parcel_aggregation_input = dict(input.items())
+        parcel_aggregation_input["data"] = output_data
+        parcel_aggregation_input["path"] = output_file_path
+        output = parcel_aggregation.compute(
+            input=parcel_aggregation_input,
+            extra_input=extra_input,
         )
 
-        # get the 2D timeseries after parcel aggregation
-        out = pa.compute(input, extra_input=extra_input)
-
-        return out
+        return output
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,97 @@
-"""Provide class for computing fALFF on spheres."""
+"""Provide class for edge-centric functional connectivity using spheres."""
 
-# Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
-#          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
-#          Kaustubh R. Patil <k.patil@fz-juelich.de>
+# Authors: Leonard Sasse <l.sasse@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
-from .. import SphereAggregation
-from .falff_base import ALFFBase
+from ..sphere_aggregation import SphereAggregation
+from ..utils import _ets, raise_error
+from .functional_connectivity_base import FunctionalConnectivityBase
 
 
 @register_marker
-class ALFFSpheres(ALFFBase):
-    """Class for computing fALFF/ALFF on spheres.
+class EdgeCentricFCSpheres(FunctionalConnectivityBase):
+    """Class for edge-centric FC using coordinates (spheres).
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
         :func:`.list_coordinates` for options.
     radius : float, optional
         The radius of the sphere in mm. If None, the signal will be extracted
         from a single voxel. See :class:`nilearn.maskers.NiftiSpheresMasker`
         for more information (default None).
     allow_overlap : bool, optional
         Whether to allow overlapping spheres. If False, an error is raised if
         the spheres overlap (default is False).
-    fractional : bool
-        Whether to compute fractional ALFF.
-    highpass : positive float, optional
-        The highpass cutoff frequency for the bandpass filter. If 0,
-        it will not apply a highpass filter (default 0.01).
-    lowpass : positive float, optional
-        The lowpass cutoff frequency for the bandpass filter (default 0.1).
-    tr : positive float, optional
-        The Repetition Time of the BOLD data. If None, will extract
-        the TR from NIFTI header (default None).
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
+    agg_method : str, optional
+        The aggregation method to use.
+        See :func:`.get_aggfunc_by_name` for more information
+        (default None).
+    agg_method_params : dict, optional
+        The parameters to pass to the aggregation method (default None).
+    cor_method : str, optional
+        The method to perform correlation using. Check valid options in
+        :class:`nilearn.connectome.ConnectivityMeasure` (default "covariance").
+    cor_method_params : dict, optional
+        Parameters to pass to the correlation function. Check valid options in
+        :class:`nilearn.connectome.ConnectivityMeasure` (default None).
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
-    method : str, optional
-        The method to perform aggregation using. Check valid options in
-        :func:`.get_aggfunc_by_name` (default "mean").
-    method_params : dict, optional
-        Parameters to pass to the aggregation function. Check valid options in
-        :func:`.get_aggfunc_by_name`.
     name : str, optional
-        The name of the marker. If None, will use the class name (default
-        None).
+        The name of the marker. By default, it will use
+        KIND_EdgeCentricFCSpheres where KIND is the kind of data it
+        was applied to (default None).
+
+    References
+    ----------
+    .. [1] Jo et al. (2021)
+            Subject identification using
+            edge-centric functional connectivity
+            doi: https://doi.org/10.1016/j.neuroimage.2021.118204
 
-    Notes
-    -----
-    The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
-    computation. If a dataset is correctly preprocessed, the TR should be
-    extracted from the NIFTI without any issue. However, it has been
-    reported that some preprocessed data might not have the correct TR in
-    the NIFTI header.
-
-    ALFF/fALFF are computed using a bandpass butterworth filter. See
-    :func:`scipy.signal.butter` and :func:`scipy.signal.filtfilt` for more
-    details.
     """
 
     def __init__(
         self,
         coords: str,
-        fractional: bool,
         radius: Optional[float] = None,
         allow_overlap: bool = False,
-        highpass: float = 0.01,
-        lowpass: float = 0.1,
-        tr: Optional[float] = None,
-        use_afni: Optional[bool] = None,
+        agg_method: str = "mean",
+        agg_method_params: Optional[Dict] = None,
+        cor_method: str = "covariance",
+        cor_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
-        method: str = "mean",
-        method_params: Optional[Dict] = None,
         name: Optional[str] = None,
     ) -> None:
         self.coords = coords
         self.radius = radius
         self.allow_overlap = allow_overlap
-        self.masks = masks
-        self.method = method
-        self.method_params = method_params
+        if radius is None or radius <= 0:
+            raise_error(f"radius should be > 0: provided {radius}")
         super().__init__(
-            fractional=fractional,
-            highpass=highpass,
-            lowpass=lowpass,
-            tr=tr,
+            agg_method=agg_method,
+            agg_method_params=agg_method_params,
+            cor_method=cor_method,
+            cor_method_params=cor_method_params,
+            masks=masks,
             name=name,
-            use_afni=use_afni,
         )
 
-    def _postprocess(
-        self, input: Dict, extra_input: Optional[Dict] = None
+    def aggregate(
+        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
     ) -> Dict:
-        """Compute ALFF and fALFF.
+        """Perform sphere aggregation and ETS computation.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
             the marker.
         extra_input : dict, optional
@@ -113,28 +99,32 @@
             other data kind that needs to be used in the computation. For
             example, the functional connectivity markers can make use of the
             confounds if available (default None).
 
         Returns
         -------
         dict
-            The computed ALFF as dictionary. The dictionary has the following
-            keys:
+            The computed result as dictionary. This will be either returned
+            to the user or stored in the storage by calling the store method
+            with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
 
         """
-        pa = SphereAggregation(
+        sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
             allow_overlap=self.allow_overlap,
-            method=self.method,
-            method_params=self.method_params,
+            method=self.agg_method,
+            method_params=self.agg_method_params,
             masks=self.masks,
-            on="fALFF",
+            on="BOLD",
+        )
+        bold_aggregated = sphere_aggregation.compute(
+            input, extra_input=extra_input
+        )
+        ets, edge_names = _ets(
+            bold_aggregated["data"], bold_aggregated["col_names"]
         )
 
-        # get the 2D timeseries after sphere aggregation
-        out = pa.compute(input, extra_input=extra_input)
-
-        return out
+        return {"data": ets, "col_names": edge_names}
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. If None, will use the class name
         (default None).
+
     """
 
     _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn"}
 
     def __init__(
         self,
         parcellation_one: str,
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
         dict
             The computed result as dictionary. This will be either returned
             to the user or stored in the storage by calling the store method
             with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
+
         """
         parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-"""Provide class for edge-centric functional connectivity using spheres."""
+"""Provide class for functional connectivity using spheres."""
 
-# Authors: Leonard Sasse <l.sasse@fz-juelich.de>
+# Authors: Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
+#          Kaustubh R. Patil <k.patil@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
 from ..sphere_aggregation import SphereAggregation
-from ..utils import _ets, raise_error
+from ..utils import raise_error
 from .functional_connectivity_base import FunctionalConnectivityBase
 
 
 @register_marker
-class EdgeCentricFCSpheres(FunctionalConnectivityBase):
-    """Class for edge-centric FC using coordinates (spheres).
+class FunctionalConnectivitySpheres(FunctionalConnectivityBase):
+    """Class for functional connectivity using coordinates (spheres).
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
         :func:`.list_coordinates` for options.
     radius : float, optional
@@ -42,24 +43,17 @@
         :class:`nilearn.connectome.ConnectivityMeasure` (default None).
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
     name : str, optional
         The name of the marker. By default, it will use
-        KIND_EdgeCentricFCSpheres where KIND is the kind of data it
+        KIND_FunctionalConnectivitySpheres where KIND is the kind of data it
         was applied to (default None).
 
-    References
-    ----------
-    .. [1] Jo et al. (2021)
-            Subject identification using
-            edge-centric functional connectivity
-            doi: https://doi.org/10.1016/j.neuroimage.2021.118204
-
     """
 
     def __init__(
         self,
         coords: str,
         radius: Optional[float] = None,
         allow_overlap: bool = False,
@@ -83,15 +77,15 @@
             masks=masks,
             name=name,
         )
 
     def aggregate(
         self, input: Dict[str, Any], extra_input: Optional[Dict] = None
     ) -> Dict:
-        """Perform sphere aggregation and ETS computation.
+        """Perform sphere aggregation.
 
         Parameters
         ----------
         input : dict
             A single input from the pipeline data object in which to compute
             the marker.
         extra_input : dict, optional
@@ -116,15 +110,9 @@
             radius=self.radius,
             allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
-        bold_aggregated = sphere_aggregation.compute(
-            input, extra_input=extra_input
-        )
-        ets, edge_names = _ets(
-            bold_aggregated["data"], bold_aggregated["col_names"]
-        )
-
-        return {"data": ets, "col_names": edge_names}
+        # Return the 2D timeseries after sphere aggregation
+        return sphere_aggregation.compute(input, extra_input=extra_input)
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
+
         """
         return ["BOLD"]
 
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/falff/falff_spheres.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,156 @@
-"""Provide class for functional connectivity using spheres."""
+"""Provide class for ALFF / fALFF on spheres."""
 
-# Authors: Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
+# Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
+#          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, Dict, List, Optional, Union
 
 from ...api.decorators import register_marker
+from ...utils import logger
 from ..sphere_aggregation import SphereAggregation
-from ..utils import raise_error
-from .functional_connectivity_base import FunctionalConnectivityBase
+from .falff_base import ALFFBase
 
 
 @register_marker
-class FunctionalConnectivitySpheres(FunctionalConnectivityBase):
-    """Class for functional connectivity using coordinates (spheres).
+class ALFFSpheres(ALFFBase):
+    """Class for computing ALFF / fALFF on spheres.
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
         :func:`.list_coordinates` for options.
+    fractional : bool
+        Whether to compute fractional ALFF.
+    using : {"junifer", "afni"}
+        Implementation to use for computing ALFF:
+
+        * "junifer" : Use ``junifer``'s own ALFF implementation
+        * "afni" : Use AFNI's ``3dRSFC``
+
     radius : float, optional
         The radius of the sphere in mm. If None, the signal will be extracted
         from a single voxel. See :class:`nilearn.maskers.NiftiSpheresMasker`
         for more information (default None).
     allow_overlap : bool, optional
         Whether to allow overlapping spheres. If False, an error is raised if
         the spheres overlap (default is False).
+    highpass : positive float, optional
+        The highpass cutoff frequency for the bandpass filter. If 0,
+        it will not apply a highpass filter (default 0.01).
+    lowpass : positive float, optional
+        The lowpass cutoff frequency for the bandpass filter (default 0.1).
+    tr : positive float, optional
+        The Repetition Time of the BOLD data. If None, will extract
+        the TR from NIfTI header (default None).
     agg_method : str, optional
-        The aggregation method to use.
-        See :func:`.get_aggfunc_by_name` for more information
-        (default None).
+        The method to perform aggregation using. Check valid options in
+        :func:`.get_aggfunc_by_name` (default "mean").
     agg_method_params : dict, optional
-        The parameters to pass to the aggregation method (default None).
-    cor_method : str, optional
-        The method to perform correlation using. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure` (default "covariance").
-    cor_method_params : dict, optional
-        Parameters to pass to the correlation function. Check valid options in
-        :class:`nilearn.connectome.ConnectivityMeasure` (default None).
+        Parameters to pass to the aggregation function. Check valid options in
+        :func:`.get_aggfunc_by_name`.
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
     name : str, optional
-        The name of the marker. By default, it will use
-        KIND_FunctionalConnectivitySpheres where KIND is the kind of data it
-        was applied to (default None).
+        The name of the marker. If None, will use the class name (default
+        None).
+
+    Notes
+    -----
+    The ``tr`` parameter is crucial for the correctness of fALFF/ALFF
+    computation. If a dataset is correctly preprocessed, the ``tr`` should be
+    extracted from the NIfTI without any issue. However, it has been
+    reported that some preprocessed data might not have the correct ``tr`` in
+    the NIFTI header.
+
+    ALFF/fALFF are computed using a bandpass butterworth filter. See
+    :func:`scipy.signal.butter` and :func:`scipy.signal.filtfilt` for more
+    details.
 
     """
 
     def __init__(
         self,
         coords: str,
+        fractional: bool,
+        using: str,
         radius: Optional[float] = None,
         allow_overlap: bool = False,
+        highpass: float = 0.01,
+        lowpass: float = 0.1,
+        tr: Optional[float] = None,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
-        cor_method: str = "covariance",
-        cor_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
-        self.coords = coords
-        self.radius = radius
-        self.allow_overlap = allow_overlap
-        if radius is None or radius <= 0:
-            raise_error(f"radius should be > 0: provided {radius}")
+        # Superclass init first to validate `using` parameter
         super().__init__(
-            agg_method=agg_method,
-            agg_method_params=agg_method_params,
-            cor_method=cor_method,
-            cor_method_params=cor_method_params,
-            masks=masks,
+            fractional=fractional,
+            highpass=highpass,
+            lowpass=lowpass,
+            using=using,
+            tr=tr,
             name=name,
         )
+        self.coords = coords
+        self.radius = radius
+        self.allow_overlap = allow_overlap
+        self.agg_method = agg_method
+        self.agg_method_params = agg_method_params
+        self.masks = masks
 
-    def aggregate(
-        self, input: Dict[str, Any], extra_input: Optional[Dict] = None
-    ) -> Dict:
-        """Perform sphere aggregation.
+    def compute(
+        self,
+        input: Dict[str, Any],
+        extra_input: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Compute.
 
         Parameters
         ----------
         input : dict
-            A single input from the pipeline data object in which to compute
-            the marker.
+            The BOLD data as dictionary.
         extra_input : dict, optional
-            The other fields in the pipeline data object. Useful for accessing
-            other data kind that needs to be used in the computation. For
-            example, the functional connectivity markers can make use of the
-            confounds if available (default None).
+            The other fields in the pipeline data object (default None).
 
         Returns
         -------
         dict
-            The computed result as dictionary. This will be either returned
-            to the user or stored in the storage by calling the store method
-            with this as a parameter. The dictionary has the following keys:
+            The computed result as dictionary. The dictionary has the following
+            keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
 
         """
+        logger.info("Calculating ALFF / fALFF for spheres")
+
+        # Compute ALFF / fALFF
+        output_data, output_file_path = self._compute(input_data=input)
+
+        # Initialize sphere aggregation
         sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
             allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
-        # Return the 2D timeseries after sphere aggregation
-        return sphere_aggregation.compute(input, extra_input=extra_input)
+        # Perform aggregation on ALFF / fALFF
+        sphere_aggregation_input = dict(input.items())
+        sphere_aggregation_input["data"] = output_data
+        sphere_aggregation_input["path"] = output_file_path
+        output = sphere_aggregation.compute(
+            input=sphere_aggregation_input,
+            extra_input=extra_input,
+        )
+
+        return output
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,96 @@
 """Provide tests for marker class to calculate cross-parcellation FC."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
 import pytest
-from nilearn import image
 
+from junifer.datareader import DefaultDataReader
 from junifer.markers.functional_connectivity import CrossParcellationFC
+from junifer.pipeline import WorkDirManager
+from junifer.pipeline.utils import _check_ants
 from junifer.storage import SQLiteFeatureStorage
 from junifer.testing.datagrabbers import SPMAuditoryTestingDataGrabber
 
 
 parcellation_one = "Schaefer100x17"
 parcellation_two = "Schaefer200x17"
 
 
-def test_compute() -> None:
-    """Test CrossParcellationFC compute()."""
+def test_init() -> None:
+    """Test CrossParcellationFC init()."""
+    with pytest.raises(ValueError, match="must be different"):
+        CrossParcellationFC(
+            parcellation_one="a",
+            parcellation_two="a",
+            correlation_method="pearson",
+        )
 
-    with SPMAuditoryTestingDataGrabber() as dg:
-        out = dg["sub001"]
-        niimg = image.load_img(str(out["BOLD"]["path"].absolute()))
-        input_dict = {
-            "BOLD": {
-                "data": niimg,
-                "path": out["BOLD"]["path"],
-                "meta": {"element": "sub001"},
-            }
-        }
 
+def test_get_output_type() -> None:
+    """Test CrossParcellationFC get_output_type()."""
+    crossparcellation = CrossParcellationFC(
+        parcellation_one=parcellation_one, parcellation_two=parcellation_two
+    )
+    assert "matrix" == crossparcellation.get_output_type("BOLD")
+
+
+@pytest.mark.skipif(
+    _check_ants() is False, reason="requires ANTs to be in PATH"
+)
+def test_compute(tmp_path: Path) -> None:
+    """Test CrossParcellationFC compute().
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+
+    """
+    with SPMAuditoryTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
+        WorkDirManager().workdir = tmp_path
         crossparcellation = CrossParcellationFC(
             parcellation_one=parcellation_one,
             parcellation_two=parcellation_two,
             correlation_method="spearman",
         )
-        out = crossparcellation.compute(input_dict["BOLD"])
+        out = crossparcellation.compute(element_data["BOLD"])
         assert out["data"].shape == (200, 100)
         assert len(out["col_names"]) == 100
         assert len(out["row_names"]) == 200
 
 
+@pytest.mark.skipif(
+    _check_ants() is False, reason="requires ANTs to be in PATH"
+)
 def test_store(tmp_path: Path) -> None:
     """Test CrossParcellationFC store().
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-
     with SPMAuditoryTestingDataGrabber() as dg:
-        input_dict = dg["sub001"]
-        niimg = image.load_img(str(input_dict["BOLD"]["path"].absolute()))
-
-        input_dict["BOLD"]["data"] = niimg
-
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
+        WorkDirManager().workdir = tmp_path
         crossparcellation = CrossParcellationFC(
             parcellation_one=parcellation_one,
             parcellation_two=parcellation_two,
             correlation_method="spearman",
         )
-        uri = tmp_path / "test_crossparcellation.sqlite"
-        storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-        crossparcellation.fit_transform(input_dict, storage=storage)
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_crossparcellation.sqlite", upsert="ignore"
+        )
+        # Fit transform marker on data with storage
+        crossparcellation.fit_transform(input=element_data, storage=storage)
         features = storage.list_features()
         assert any(
             x["name"] == "BOLD_CrossParcellationFC" for x in features.values()
         )
-
-
-def test_get_output_type() -> None:
-    """Test CrossParcellationFC get_output_type()."""
-
-    crossparcellation = CrossParcellationFC(
-        parcellation_one=parcellation_one, parcellation_two=parcellation_two
-    )
-    input_ = "BOLD"
-    output = crossparcellation.get_output_type(input_)
-    assert output == "matrix"
-
-
-def test_init_() -> None:
-    """Test CrossParcellationFC init()."""
-    with pytest.raises(ValueError, match="must be different"):
-        CrossParcellationFC(
-            parcellation_one="a",
-            parcellation_two="a",
-            correlation_method="pearson",
-        )
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,59 +2,54 @@
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
-from nilearn import datasets, image
-
+from junifer.datareader import DefaultDataReader
 from junifer.markers.functional_connectivity import EdgeCentricFCParcels
 from junifer.storage import SQLiteFeatureStorage
+from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
 
 
 def test_EdgeCentricFCParcels(tmp_path: Path) -> None:
     """Test EdgeCentricFCParcels.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    # get a dataset
-    ni_data = datasets.fetch_spm_auditory(subject_id="sub001")
-    fmri_img = image.concat_imgs(ni_data.func)  # type: ignore
-
-    # Check empirical correlation method parameters
-    efc = EdgeCentricFCParcels(
-        parcellation="TianxS1x3TxMNInonlinear2009cAsym",
-        cor_method_params={"empirical": True},
-    )
-    all_out = efc.fit_transform({"BOLD": {"data": fmri_img, "meta": {}}})
-
-    out = all_out["BOLD"]
-
-    # for 16 ROIs we should get (16 * (16 -1) / 2) edges in the ETS
-    n_edges = int(16 * (16 - 1) / 2)
-    assert "data" in out
-    assert "row_names" in out
-    assert "col_names" in out
-    assert out["data"].shape[0] == n_edges
-    assert out["data"].shape[1] == n_edges
-    assert len(set(out["row_names"])) == n_edges
-    assert len(set(out["col_names"])) == n_edges
-
-    # check correct output
-    assert efc.get_output_type("BOLD") == "matrix"
-
-    uri = tmp_path / "test_fc_parcellation.sqlite"
-    # Single storage, must be the uri
-    storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-    meta = {"element": {"subject": "test"}, "dependencies": {"numpy"}}
-    input = {"BOLD": {"data": fmri_img, "meta": meta}}
-    all_out = efc.fit_transform(input, storage=storage)
-
-    features = storage.list_features()
-    assert any(
-        x["name"] == "BOLD_EdgeCentricFCParcels" for x in features.values()
-    )
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        marker = EdgeCentricFCParcels(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            cor_method_params={"empirical": True},
+        )
+        # Check correct output
+        assert marker.get_output_type("BOLD") == "matrix"
+
+        # Fit-transform the data
+        edge_fc = marker.fit_transform(element_data)
+        edge_fc_bold = edge_fc["BOLD"]
+
+        # For 16 ROIs we should get (16 * (16 -1) / 2) edges in the ETS
+        n_edges = int(16 * (16 - 1) / 2)
+        assert "data" in edge_fc_bold
+        assert "row_names" in edge_fc_bold
+        assert "col_names" in edge_fc_bold
+        assert edge_fc_bold["data"].shape[0] == n_edges
+        assert edge_fc_bold["data"].shape[1] == n_edges
+        assert len(set(edge_fc_bold["row_names"])) == n_edges
+        assert len(set(edge_fc_bold["col_names"])) == n_edges
+
+        # Store
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_edge_fc_parcels.sqlite", upsert="ignore"
+        )
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_EdgeCentricFCParcels" for x in features.values()
+        )
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,72 +2,60 @@
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
-from nilearn import datasets, image
-
+from junifer.datareader import DefaultDataReader
 from junifer.markers.functional_connectivity import EdgeCentricFCSpheres
 from junifer.storage import SQLiteFeatureStorage
+from junifer.testing.datagrabbers import SPMAuditoryTestingDataGrabber
 
 
 def test_EdgeCentricFCSpheres(tmp_path: Path) -> None:
     """Test EdgeCentricFCSpheres.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    # get a dataset
-    ni_data = datasets.fetch_spm_auditory(subject_id="sub001")
-    fmri_img = image.concat_imgs(ni_data.func)  # type: ignore
-
-    efc = EdgeCentricFCSpheres(
-        coords="DMNBuckner", radius=5.0, cor_method="correlation"
-    )
-    all_out = efc.fit_transform({"BOLD": {"data": fmri_img, "meta": {}}})
-
-    out = all_out["BOLD"]
-
-    # There are six DMNBuckner coordinates, so
-    # for 6 ROIs we should get (6 * (6 -1) / 2) edges in the ETS
-    n_edges = int(6 * (6 - 1) / 2)
-    assert "data" in out
-    assert "row_names" in out
-    assert "col_names" in out
-    assert out["data"].shape[0] == n_edges
-    assert out["data"].shape[1] == n_edges
-    assert len(set(out["row_names"])) == n_edges
-    assert len(set(out["col_names"])) == n_edges
-
-    # check correct output
-    assert efc.get_output_type("BOLD") == "matrix"
-
-    # Check empirical correlation method parameters
-    efc = EdgeCentricFCSpheres(
-        coords="DMNBuckner",
-        radius=5.0,
-        cor_method="correlation",
-        cor_method_params={"empirical": True},
-    )
-
-    meta = {
-        "element": {"subject": "sub001"},
-        "dependencies": {"nilearn"},
-    }
-    all_out = efc.fit_transform({"BOLD": {"data": fmri_img, "meta": meta}})
-
-    uri = tmp_path / "test_fc_parcellation.sqlite"
-    # Single storage, must be the uri
-    storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-    meta = {"element": {"subject": "test"}, "dependencies": {"numpy"}}
-    input = {"BOLD": {"data": fmri_img, "meta": meta}}
-    all_out = efc.fit_transform(input, storage=storage)
-
-    features = storage.list_features()
-    assert any(
-        x["name"] == "BOLD_EdgeCentricFCSpheres" for x in features.values()
-    )
+    with SPMAuditoryTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub001"])
+        marker = EdgeCentricFCSpheres(
+            coords="DMNBuckner", radius=5.0, cor_method="correlation"
+        )
+        # Check correct output
+        assert marker.get_output_type("BOLD") == "matrix"
+
+        # Fit-transform the data
+        edge_fc = marker.fit_transform(element_data)
+        edge_fc_bold = edge_fc["BOLD"]
+
+        # There are six DMNBuckner coordinates, so
+        # for 6 ROIs we should get (6 * (6 -1) / 2) edges in the ETS
+        n_edges = int(6 * (6 - 1) / 2)
+        assert "data" in edge_fc_bold
+        assert "row_names" in edge_fc_bold
+        assert "col_names" in edge_fc_bold
+        assert edge_fc_bold["data"].shape == (n_edges, n_edges)
+        assert len(set(edge_fc_bold["row_names"])) == n_edges
+        assert len(set(edge_fc_bold["col_names"])) == n_edges
+
+        # Check empirical correlation method parameters
+        marker = EdgeCentricFCSpheres(
+            coords="DMNBuckner",
+            radius=5.0,
+            cor_method="correlation",
+            cor_method_params={"empirical": True},
+        )
+        # Store
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_edge_fc_spheres.sqlite", upsert="ignore"
+        )
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_EdgeCentricFCSpheres" for x in features.values()
+        )
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,88 @@
 """Provide tests for functional connectivity using parcellation."""
 
 # Authors: Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 #          Kaustubh R. Patil <k.patil@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
-from nilearn import datasets, image
 from nilearn.connectome import ConnectivityMeasure
 from nilearn.maskers import NiftiLabelsMasker
-from numpy.testing import assert_array_almost_equal, assert_array_equal
+from numpy.testing import assert_array_almost_equal
 
+from junifer.data import get_parcellation
+from junifer.datareader import DefaultDataReader
 from junifer.markers.functional_connectivity import (
     FunctionalConnectivityParcels,
 )
-from junifer.markers.parcel_aggregation import ParcelAggregation
 from junifer.storage import SQLiteFeatureStorage
+from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
 
 
 def test_FunctionalConnectivityParcels(tmp_path: Path) -> None:
     """Test FunctionalConnectivityParcels.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    # get a dataset
-    ni_data = datasets.fetch_spm_auditory(subject_id="sub001")
-    fmri_img = image.concat_imgs(ni_data.func)  # type: ignore
-
-    fc = FunctionalConnectivityParcels(parcellation="Schaefer100x7")
-    all_out = fc.fit_transform({"BOLD": {"data": fmri_img, "meta": {}}})
-
-    out = all_out["BOLD"]
-
-    assert "data" in out
-    assert "row_names" in out
-    assert "col_names" in out
-    assert out["data"].shape[0] == 100
-    assert out["data"].shape[1] == 100
-    assert len(set(out["row_names"])) == 100
-    assert len(set(out["col_names"])) == 100
-
-    # get the timeseries using pa
-    pa = ParcelAggregation(
-        parcellation="Schaefer100x7", method="mean", on="BOLD"
-    )
-    meta = {
-        "element": {"subject": "sub001"},
-        "dependencies": {"nilearn"},
-    }
-    ts = pa.compute({"data": fmri_img, "meta": meta})
-
-    # compare with nilearn
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(
-        n_rois=100, yeo_networks=7, resolution_mm=2
-    )
-    masker = NiftiLabelsMasker(
-        labels_img=parcellation["maps"], standardize=False
-    )
-    ts_ni = masker.fit_transform(fmri_img)
-
-    # check the TS are almost equal
-    assert_array_equal(ts_ni, ts["data"])
-
-    # Check that FC are almost equal
-    cm = ConnectivityMeasure(kind="covariance")
-    out_ni = cm.fit_transform([ts_ni])[0]
-    assert_array_almost_equal(out_ni, out["data"], decimal=3)
-
-    # check correct output
-    assert fc.get_output_type("BOLD") == "matrix"
-
-    # Check empirical correlation method parameters
-    fc = FunctionalConnectivityParcels(
-        parcellation="Schaefer100x7", cor_method_params={"empirical": True}
-    )
-
-    all_out = fc.fit_transform({"BOLD": {"data": fmri_img, "meta": meta}})
-
-    uri = tmp_path / "test_fc_parcellation.sqlite"
-    # Single storage, must be the uri
-    storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-    meta = {"element": {"subject": "test"}, "dependencies": {"numpy"}}
-    input = {"BOLD": {"data": fmri_img, "meta": meta}}
-    all_out = fc.fit_transform(input, storage=storage)
-
-    features = storage.list_features()
-    assert any(
-        x["name"] == "BOLD_FunctionalConnectivityParcels"
-        for x in features.values()
-    )
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        marker = FunctionalConnectivityParcels(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym"
+        )
+        # Check correct output
+        assert marker.get_output_type("BOLD") == "matrix"
+
+        # Fit-transform the data
+        fc = marker.fit_transform(element_data)
+        fc_bold = fc["BOLD"]
+
+        assert "data" in fc_bold
+        assert "row_names" in fc_bold
+        assert "col_names" in fc_bold
+        assert fc_bold["data"].shape == (16, 16)
+        assert len(set(fc_bold["row_names"])) == 16
+        assert len(set(fc_bold["col_names"])) == 16
+
+        # Compare with nilearn
+        # Load testing parcellation for the target data
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Extract timeseries
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation, standardize=False
+        )
+        extracted_timeseries = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"]
+        )
+        # Compute the connectivity measure
+        connectivity_measure = ConnectivityMeasure(
+            kind="covariance"
+        ).fit_transform([extracted_timeseries])[0]
+
+        # Check that FC are almost equal
+        assert_array_almost_equal(
+            connectivity_measure, fc_bold["data"], decimal=3
+        )
+
+        # Check empirical correlation method parameters
+        marker = FunctionalConnectivityParcels(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            cor_method_params={"empirical": True},
+        )
+        # Store
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_fc_parcels.sqlite", upsert="ignore"
+        )
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_FunctionalConnectivityParcels"
+            for x in features.values()
+        )
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/parcel_aggregation.py` & `junifer-0.0.5.dev11/junifer/markers/parcel_aggregation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 import numpy as np
-from nilearn.image import math_img, resample_to_img
+from nilearn.image import math_img
 from nilearn.maskers import NiftiMasker
 
 from ..api.decorators import register_marker
-from ..data import get_mask, load_parcellation, merge_parcellations
+from ..data import get_mask, get_parcellation
 from ..stats import get_aggfunc_by_name
 from ..utils import logger, raise_error, warn_with_log
 from .base import BaseMarker
 
 
 @register_marker
 class ParcelAggregation(BaseMarker):
@@ -38,21 +38,28 @@
         it will not operate on the time dimension (default None).
     time_method_params : dict, optional
         The parameters to pass to the time aggregation method (default None).
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
-    on : {"T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"} \
-         or list of the options, optional
+    on : {"T1w", "T2w", "BOLD", "VBM_GM", "VBM_WM", "VBM_CSF", "fALFF", \
+        "GCOR", "LCOR"} or list of the options, optional
         The data types to apply the marker to. If None, will work on all
         available data (default None).
     name : str, optional
         The name of the marker. If None, will use the class name (default
         None).
+
+    Raises
+    ------
+    ValueError
+        If ``time_method`` is specified for non-BOLD data or if
+        ``time_method_params`` is not None when ``time_method`` is None.
+
     """
 
     _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn", "numpy"}
 
     def __init__(
         self,
         parcellation: Union[str, List[str]],
@@ -91,37 +98,59 @@
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
 
         """
-        return ["T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]
+        return [
+            "T1w",
+            "T2w",
+            "BOLD",
+            "VBM_GM",
+            "VBM_WM",
+            "VBM_CSF",
+            "fALFF",
+            "GCOR",
+            "LCOR",
+        ]
 
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
         input_type : str
             The data type input to the marker.
 
         Returns
         -------
         str
             The storage type output by the marker.
 
+        Raises
+        ------
+        ValueError
+            If the ``input_type`` is invalid.
+
         """
 
-        if input_type in ["VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]:
+        if input_type in [
+            "VBM_GM",
+            "VBM_WM",
+            "VBM_CSF",
+            "fALFF",
+            "GCOR",
+            "LCOR",
+        ]:
             return "vector"
         elif input_type == "BOLD":
             return "timeseries"
         else:
-            raise ValueError(f"Unknown input kind for {input_type}")
+            raise_error(f"Unknown input kind for {input_type}")
 
     def compute(
         self, input: Dict[str, Any], extra_input: Optional[Dict] = None
     ) -> Dict:
         """Compute.
 
         Parameters
@@ -141,90 +170,83 @@
             The computed result as dictionary. This will be either returned
             to the user or stored in the storage by calling the store method
             with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
 
+        Warns
+        -----
+        RuntimeWarning
+            If time aggregation is required but only time point is available.
+
         """
         t_input_img = input["data"]
         logger.debug(f"Parcel aggregation using {self.method}")
+        # Get aggregation function
         agg_func = get_aggfunc_by_name(
             name=self.method, func_params=self.method_params
         )
-        # Get the min of the voxels sizes and use it as the resolution
-        resolution = np.min(t_input_img.header.get_zooms()[:3])
-
-        # Load the parcellations
-        all_parcelations = []
-        all_labels = []
-        for t_parc_name in self.parcellation:
-            t_parcellation, t_labels, _ = load_parcellation(
-                name=t_parc_name, resolution=resolution
-            )
-            # Resample all of them to the image
-            t_parcellation_img_res = resample_to_img(
-                t_parcellation, t_input_img, interpolation="nearest", copy=True
-            )
-            all_parcelations.append(t_parcellation_img_res)
-            all_labels.append(t_labels)
 
-        # Avoid merging if there is only one parcellation
-        if len(all_parcelations) == 1:
-            parcellation_img_res = all_parcelations[0]
-            labels = all_labels[0]
-        else:
-            # Merge the parcellations
-            parcellation_img_res, labels = merge_parcellations(
-                all_parcelations, self.parcellation, all_labels
-            )
+        # Get parcellation tailored to target image
+        parcellation_img, labels = get_parcellation(
+            parcellation=self.parcellation,
+            target_data=input,
+            extra_input=extra_input,
+        )
 
-        parcellation_bin = math_img("img != 0", img=parcellation_img_res)
+        # Get binarized parcellation image for masking
+        parcellation_bin = math_img("img != 0", img=parcellation_img)
 
+        # Load mask
         if self.masks is not None:
             logger.debug(f"Masking with {self.masks}")
+            # Get tailored mask
             mask_img = get_mask(
                 masks=self.masks, target_data=input, extra_input=extra_input
             )
-
+            # Get "logical and" version of parcellation and mask
             parcellation_bin = math_img(
                 "np.logical_and(img, mask)",
                 img=parcellation_bin,
                 mask=mask_img,
             )
 
+        # Initialize masker
         logger.debug("Masking")
         masker = NiftiMasker(
             parcellation_bin, target_affine=t_input_img.affine
-        )  # type: ignore
-
+        )
         # Mask the input data and the parcellation
         data = masker.fit_transform(t_input_img)
-        parcellation_values = masker.transform(parcellation_img_res)
-        parcellation_values = np.squeeze(parcellation_values).astype(int)
+        parcellation_values = np.squeeze(
+            masker.transform(parcellation_img)
+        ).astype(int)
 
         # Get the values for each parcel and apply agg function
         logger.debug("Computing ROI means")
         out_values = []
         # Iterate over the parcels (existing)
         for t_v in range(1, len(labels) + 1):
             t_values = agg_func(data[:, parcellation_values == t_v], axis=-1)
             out_values.append(t_values)
             # Update the labels just in case a parcel has no voxels
             # in it
 
         out_values = np.array(out_values).T
 
+        # Apply time dimension aggregation if required
         if self.time_method is not None:
             if out_values.shape[0] > 1:
                 logger.debug("Aggregating time dimension")
                 time_agg_func = get_aggfunc_by_name(
                     self.time_method, func_params=self.time_method_params
                 )
                 out_values = time_agg_func(out_values, axis=0)
             else:
                 warn_with_log(
                     "No time dimension to aggregate as only one time point is "
                     "available."
                 )
+        # Format the output
         out = {"data": out_values, "col_names": labels}
         return out
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/reho/reho_base.py` & `junifer-0.0.5.dev11/junifer/markers/reho/reho_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,82 @@
 """Provide base class for regional homogeneity (ReHo)."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional, Union
+from pathlib import Path
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
 
 from ...utils import logger, raise_error
 from ..base import BaseMarker
-from .reho_estimator import ReHoEstimator
+from ._afni_reho import AFNIReHo
+from ._junifer_reho import JuniferReHo
 
 
 if TYPE_CHECKING:
     from nibabel import Nifti1Image
 
 
 class ReHoBase(BaseMarker):
     """Base class for regional homogeneity computation.
 
     Parameters
     ----------
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
+    using : {"junifer", "afni"}
+        Implementation to use for computing ReHo:
+
+        * "junifer" : Use ``junifer``'s own ReHo implementation
+        * "afni" : Use AFNI's ``3dReHo``
+
     name : str, optional
         The name of the marker. If None, it will use the class name
         (default None).
 
+    Raises
+    ------
+    ValueError
+        If ``using`` is invalid.
+
     """
 
-    _EXT_DEPENDENCIES: ClassVar[
-        List[Dict[str, Union[str, bool, List[str]]]]
-    ] = [
+    _CONDITIONAL_DEPENDENCIES: ClassVar[List[Dict[str, Union[str, Type]]]] = [
         {
-            "name": "afni",
-            "optional": True,
-            "commands": ["3dReHo", "3dAFNItoNIFTI"],
+            "using": "afni",
+            "depends_on": AFNIReHo,
+        },
+        {
+            "using": "junifer",
+            "depends_on": JuniferReHo,
         },
     ]
 
     def __init__(
         self,
-        use_afni: Optional[bool] = None,
+        using: str,
         name: Optional[str] = None,
     ) -> None:
+        # Validate `using` parameter
+        valid_using = [dep["using"] for dep in self._CONDITIONAL_DEPENDENCIES]
+        if using not in valid_using:
+            raise_error(
+                f"Invalid value for `using`, should be one of: {valid_using}"
+            )
+        self.using = using
         super().__init__(on="BOLD", name=name)
-        self.use_afni = use_afni
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
@@ -70,59 +97,67 @@
         -------
         str
             The storage type output by the marker.
 
         """
         return "vector"
 
-    def compute_reho_map(
+    def _compute(
         self,
-        input: Dict[str, Any],
+        input_data: Dict[str, Any],
         **reho_params: Any,
-    ) -> "Nifti1Image":
-        """Compute.
+    ) -> Tuple["Nifti1Image", Path]:
+        """Compute voxel-wise ReHo.
 
         Calculates Kendall's W per voxel using neighborhood voxels.
         Instead of the time series values themselves, Kendall's W uses the
         relative rank ordering of a hood over all time points to evaluate
         a parameter W in range 0-1, with 0 reflecting no trend of agreement
         between time series and 1 reflecting perfect agreement. For more
         information about the method, please check [1]_.
 
         Parameters
         ----------
-        input : dict
+        input_data : dict
             The BOLD data as dictionary.
         **reho_params : dict
             Extra keyword arguments for ReHo.
 
         Returns
         -------
         Niimg-like object
+            The ReHo map as NIfTI.
+        pathlib.Path
+            The path to the ReHo map as NIfTI or the input data path if the
+            input data space is "native".
 
         References
         ----------
         .. [1] Jiang, L., & Zuo, X. N. (2016).
                Regional Homogeneity: A Multimodal, Multiscale Neuroimaging
                Marker of the Human Connectome.
                The Neuroscientist, Volume 22(5), Pages 486-505.
                https://doi.org/10.1177/1073858415595004
 
         """
-        if self.use_afni is None:
-            raise_error(
-                "Parameter `use_afni` must be set to True or False in order "
-                "to compute this marker. It is currently set to None (default "
-                "behaviour). This is intended to be for auto-detection. In "
-                "order for that to happen, please call the `validate` method "
-                "before calling the `compute` method."
-            )
-        logger.info("Calculating ReHO map.")
-        # Initialize reho estimator
-        reho_estimator = ReHoEstimator()
-        # Fit-transform reho estimator
-        reho_map = reho_estimator.fit_transform(
-            use_afni=self.use_afni,
-            input_data=input,
+        logger.debug("Calculating voxel-wise ReHo")
+
+        # Conditional estimator
+        if self.using == "afni":
+            estimator = AFNIReHo()
+        elif self.using == "junifer":
+            estimator = JuniferReHo()
+        # Compute reho
+        reho_map, reho_map_path = estimator.compute(  # type: ignore
+            data=input_data["data"],
             **reho_params,
         )
-        return reho_map
+
+        # If the input data space is native already, the original path should
+        # be propagated down as it might be required for transforming
+        # parcellation / coordinates to native space, else the reho map
+        # path should be passed for use later if required.
+        # TODO(synchon): will be taken care in #292
+        if input_data["space"] == "native":
+            return reho_map, input_data["path"]
+
+        return reho_map, reho_map_path
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/reho/reho_parcels.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 
 @register_marker
 class ReHoParcels(ReHoBase):
     """Class for regional homogeneity on parcels.
 
     Parameters
     ----------
-    parcellation : str
-        The name of the parcellation. Check valid options by calling
+    parcellation : str or list of str
+        The name(s) of the parcellation(s). Check valid options by calling
         :func:`.list_parcellations`.
-    use_afni : bool, optional
-        Whether to use AFNI for computing. If None, will use AFNI only
-        if available (default None).
+    using : {"junifer", "afni"}
+        Implementation to use for computing ReHo:
+
+        * "junifer" : Use ``junifer``'s own ReHo implementation
+        * "afni" : Use AFNI's ``3dReHo``
+
     reho_params : dict, optional
         Extra parameters for computing ReHo map as a dictionary (default None).
-        If ``use_afni = True``, then the valid keys are:
+        If ``using="afni"``, then the valid keys are:
 
         * ``nneigh`` : {7, 19, 27}, optional (default 27)
             Number of voxels in the neighbourhood, inclusive. Can be:
 
             - 7 : for facewise neighbours only
             - 19 : for face- and edge-wise nieghbours
             - 27 : for face-, edge-, and node-wise neighbors
@@ -54,15 +57,15 @@
         * ``box_y`` : positive int, optional
             The number of voxels for +/- y-axis of cuboidal volumes
             (default None).
         * ``box_z`` : positive int, optional
             The number of voxels for +/- z-axis of cuboidal volumes
             (default None).
 
-        else if ``use_afni = False``, then the valid keys are:
+        else if ``using="junifer"``, then the valid keys are:
 
         * ``nneigh`` : {7, 19, 27, 125}, optional (default 27)
             Number of voxels in the neighbourhood, inclusive. Can be:
 
             * 7 : for facewise neighbours only
             * 19 : for face- and edge-wise nieghbours
             * 27 : for face-, edge-, and node-wise neighbors
@@ -82,28 +85,29 @@
         The name of the marker. If None, it will use the class name
         (default None).
 
     """
 
     def __init__(
         self,
-        parcellation: str,
-        use_afni: Optional[bool] = None,
+        parcellation: Union[str, List[str]],
+        using: str,
         reho_params: Optional[Dict] = None,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
+        # Superclass init first to validate `using` parameter
+        super().__init__(using=using, name=name)
         self.parcellation = parcellation
         self.reho_params = reho_params
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
         self.masks = masks
-        super().__init__(use_afni=use_afni, name=name)
 
     def compute(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         """Compute.
@@ -121,33 +125,39 @@
             The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a 1D numpy.ndarray
             * ``col_names`` : the column labels for the parcels as a list
 
         """
-        logger.info("Calculating ReHo for parcels.")
-        # Calculate reho map
+        logger.info("Calculating ReHo for parcels")
+
+        # Compute voxelwise reho
+        # If the input data space is "native", then reho_file_path points to
+        # the input data path as it might be required for parcellation
+        # transformation to native space.
         if self.reho_params is not None:
-            reho_map = self.compute_reho_map(input=input, **self.reho_params)
+            reho_map, reho_file_path = self._compute(
+                input_data=input, **self.reho_params
+            )
         else:
-            reho_map = self.compute_reho_map(input=input)
+            reho_map, reho_file_path = self._compute(input_data=input)
+
         # Initialize parcel aggregation
         parcel_aggregation = ParcelAggregation(
             parcellation=self.parcellation,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
         parcel_aggregation_input = dict(input.items())
         parcel_aggregation_input["data"] = reho_map
-        parcel_aggregation_input["path"] = None
-
+        parcel_aggregation_input["path"] = reho_file_path
         output = parcel_aggregation.compute(
             input=parcel_aggregation_input,
             extra_input=extra_input,
         )
         # Only use the first row and expand row dimension
         output["data"] = output["data"][0][np.newaxis, :]
         return output
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/reho/reho_spheres.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,28 +19,34 @@
     """Class for regional homogeneity on spheres.
 
     Parameters
     ----------
     coords : str
         The name of the coordinates list to use. See
         :func:`.list_coordinates` for options.
+    using : {"junifer", "afni"}
+        Implementation to use for computing ReHo:
+
+        * "junifer" : Use ``junifer``'s own ReHo implementation
+        * "afni" : Use AFNI's ``3dReHo``
+
     radius : float, optional
         The radius of the sphere in millimeters. If None, the signal will be
         extracted from a single voxel. See
         :class:`nilearn.maskers.NiftiSpheresMasker` for more information
         (default None).
     allow_overlap : bool, optional
         Whether to allow overlapping spheres. If False, an error is raised if
         the spheres overlap (default is False).
     use_afni : bool, optional
         Whether to use AFNI for computing. If None, will use AFNI only
         if available (default None).
     reho_params : dict, optional
         Extra parameters for computing ReHo map as a dictionary (default None).
-        If ``use_afni = True``, then the valid keys are:
+        If ``using="afni"``, then the valid keys are:
 
         * ``nneigh`` : {7, 19, 27}, optional (default 27)
             Number of voxels in the neighbourhood, inclusive. Can be:
 
             - 7 : for facewise neighbours only
             - 19 : for face- and edge-wise nieghbours
             - 27 : for face-, edge-, and node-wise neighbors
@@ -62,15 +68,15 @@
         * ``box_y`` : positive int, optional
             The number of voxels for +/- y-axis of cuboidal volumes
             (default None).
         * ``box_z`` : positive int, optional
             The number of voxels for +/- z-axis of cuboidal volumes
             (default None).
 
-        else if ``use_afni = False``, then the valid keys are:
+        else if ``using="junifer"``, then the valid keys are:
 
         * ``nneigh`` : {7, 19, 27, 125}, optional (default 27)
             Number of voxels in the neighbourhood, inclusive. Can be:
 
             * 7 : for facewise neighbours only
             * 19 : for face- and edge-wise nieghbours
             * 27 : for face-, edge-, and node-wise neighbors
@@ -91,31 +97,32 @@
         (default None).
 
     """
 
     def __init__(
         self,
         coords: str,
+        using: str,
         radius: Optional[float] = None,
         allow_overlap: bool = False,
-        use_afni: Optional[bool] = None,
         reho_params: Optional[Dict] = None,
         agg_method: str = "mean",
         agg_method_params: Optional[Dict] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
         name: Optional[str] = None,
     ) -> None:
+        # Superclass init first to validate `using` parameter
+        super().__init__(using=using, name=name)
         self.coords = coords
         self.radius = radius
         self.allow_overlap = allow_overlap
         self.reho_params = reho_params
         self.agg_method = agg_method
         self.agg_method_params = agg_method_params
         self.masks = masks
-        super().__init__(use_afni=use_afni, name=name)
 
     def compute(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         """Compute.
@@ -133,33 +140,40 @@
             The computed result as dictionary. The dictionary has the following
             keys:
 
             * ``data`` : the actual computed values as a 1D numpy.ndarray
             * ``col_names`` : the column labels for the spheres as a list
 
         """
-        logger.info("Calculating ReHo for spheres.")
-        # Calculate reho map
+        logger.info("Calculating ReHo for spheres")
+
+        # Compute voxelwise reho
+        # If the input data space is "native", then reho_file_path points to
+        # the input data path as it might be required for coordinates
+        # transformation to native space.
         if self.reho_params is not None:
-            reho_map = self.compute_reho_map(input=input, **self.reho_params)
+            reho_map, reho_file_path = self._compute(
+                input_data=input, **self.reho_params
+            )
         else:
-            reho_map = self.compute_reho_map(input=input)
+            reho_map, reho_file_path = self._compute(input_data=input)
+
         # Initialize sphere aggregation
         sphere_aggregation = SphereAggregation(
             coords=self.coords,
             radius=self.radius,
             allow_overlap=self.allow_overlap,
             method=self.agg_method,
             method_params=self.agg_method_params,
             masks=self.masks,
             on="BOLD",
         )
         # Perform aggregation on reho map
         sphere_aggregation_input = dict(input.items())
         sphere_aggregation_input["data"] = reho_map
-        sphere_aggregation_input["path"] = None
+        sphere_aggregation_input["path"] = reho_file_path
         output = sphere_aggregation.compute(
             input=sphere_aggregation_input, extra_input=extra_input
         )
         # Only use the first row and expand row dimension
         output["data"] = output["data"][0][np.newaxis, :]
         return output
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/sphere_aggregation.py` & `junifer-0.0.5.dev11/junifer/markers/sphere_aggregation.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, ClassVar, Dict, List, Optional, Set, Union
 
 from ..api.decorators import register_marker
-from ..data import get_mask, load_coordinates
+from ..data import get_coordinates, get_mask
 from ..external.nilearn import JuniferNiftiSpheresMasker
 from ..stats import get_aggfunc_by_name
 from ..utils import logger, raise_error, warn_with_log
 from .base import BaseMarker
 
 
 @register_marker
@@ -43,22 +43,28 @@
         it will not operate on the time dimension (default None).
     time_method_params : dict, optional
         The parameters to pass to the time aggregation method (default None).
     masks : str, dict or list of dict or str, optional
         The specification of the masks to apply to regions before extracting
         signals. Check :ref:`Using Masks <using_masks>` for more details.
         If None, will not apply any mask (default None).
-    on : {"T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"} or \
-         list of the options, optional
+    on : {"T1w", "T2w", "BOLD", "VBM_GM", "VBM_WM", "VBM_CSF", "fALFF", \
+        "GCOR", "LCOR"} or list of the options, optional
         The data types to apply the marker to. If None, will work on all
         available data (default None).
     name : str, optional
         The name of the marker. By default, it will use KIND_SphereAggregation
         where KIND is the kind of data it was applied to (default None).
 
+    Raises
+    ------
+    ValueError
+        If ``time_method`` is specified for non-BOLD data or if
+        ``time_method_params`` is not None when ``time_method`` is None.
+
     """
 
     _DEPENDENCIES: ClassVar[Set[str]] = {"nilearn", "numpy"}
 
     def __init__(
         self,
         coords: str,
@@ -99,37 +105,59 @@
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
 
         """
-        return ["T1w", "BOLD", "VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]
+        return [
+            "T1w",
+            "T2w",
+            "BOLD",
+            "VBM_GM",
+            "VBM_WM",
+            "VBM_CSF",
+            "fALFF",
+            "GCOR",
+            "LCOR",
+        ]
 
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
         input_type : str
             The data type input to the marker.
 
         Returns
         -------
         str
             The storage type output by the marker.
 
+        Raises
+        ------
+        ValueError
+            If the ``input_type`` is invalid.
+
         """
 
-        if input_type in ["VBM_GM", "VBM_WM", "fALFF", "GCOR", "LCOR"]:
+        if input_type in [
+            "VBM_GM",
+            "VBM_WM",
+            "VBM_CSF",
+            "fALFF",
+            "GCOR",
+            "LCOR",
+        ]:
             return "vector"
         elif input_type == "BOLD":
             return "timeseries"
         else:
-            raise ValueError(f"Unknown input kind for {input_type}")
+            raise_error(f"Unknown input kind for {input_type}")
 
     def compute(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict] = None,
     ) -> Dict:
         """Compute.
@@ -151,47 +179,64 @@
             The computed result as dictionary. This will be either returned
             to the user or stored in the storage by calling the store method
             with this as a parameter. The dictionary has the following keys:
 
             * ``data`` : the actual computed values as a numpy.ndarray
             * ``col_names`` : the column labels for the computed values as list
 
+        Warns
+        -----
+        RuntimeWarning
+            If time aggregation is required but only time point is available.
+
         """
         t_input_img = input["data"]
         logger.debug(f"Sphere aggregation using {self.method}")
         # Get aggregation function
         agg_func = get_aggfunc_by_name(
             self.method, func_params=self.method_params
         )
+
+        # Get seeds and labels tailored to target image
+        coords, labels = get_coordinates(
+            coords=self.coords,
+            target_data=input,
+            extra_input=extra_input,
+        )
+
         # Load mask
         mask_img = None
         if self.masks is not None:
             logger.debug(f"Masking with {self.masks}")
+            # Get tailored mask
             mask_img = get_mask(
                 masks=self.masks, target_data=input, extra_input=extra_input
             )
-        # Get seeds and labels
-        coords, out_labels = load_coordinates(name=self.coords)
+
+        # Initialize masker
+        logger.debug("Masking")
         masker = JuniferNiftiSpheresMasker(
             seeds=coords,
             radius=self.radius,
             allow_overlap=self.allow_overlap,
             mask_img=mask_img,
             agg_func=agg_func,
         )
         # Fit and transform the marker on the data
         out_values = masker.fit_transform(t_input_img)
+
+        # Apply time dimension aggregation if required
         if self.time_method is not None:
             if out_values.shape[0] > 1:
                 logger.debug("Aggregating time dimension")
                 time_agg_func = get_aggfunc_by_name(
                     self.time_method, func_params=self.time_method_params
                 )
                 out_values = time_agg_func(out_values, axis=0)
             else:
                 warn_with_log(
                     "No time dimension to aggregate as only one time point is "
                     "available."
                 )
         # Format the output
-        out = {"data": out_values, "col_names": out_labels}
+        out = {"data": out_values, "col_names": labels}
         return out
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     def get_valid_inputs(self) -> List[str]:
         """Get valid data types for input.
 
         Returns
         -------
         list of str
             The list of data types that can be used as input for this marker.
+
         """
         return ["BOLD"]
 
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.5.dev11/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.5.dev11/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """Provide tests for temporal signal-to-noise ratio using parcellation."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
+#          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from pathlib import Path
 
-from nilearn import datasets, image
-
+from junifer.datareader import DefaultDataReader
 from junifer.markers.temporal_snr import TemporalSNRParcels
-from junifer.storage import SQLiteFeatureStorage
+from junifer.storage import HDF5FeatureStorage
+from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
+
+
+def test_TemporalSNRParcels_computation() -> None:
+    """Test TemporalSNRParcels fit-transform."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        marker = TemporalSNRParcels(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym"
+        )
+        # Check correct output
+        assert marker.get_output_type("BOLD") == "vector"
+
+        # Fit-transform the data
+        tsnr_parcels = marker.fit_transform(element_data)
+        tsnr_parcels_bold = tsnr_parcels["BOLD"]
+
+        assert "data" in tsnr_parcels_bold
+        assert "col_names" in tsnr_parcels_bold
+        assert tsnr_parcels_bold["data"].shape == (1, 16)
+        assert len(set(tsnr_parcels_bold["col_names"])) == 16
 
 
-def test_TemporalSNRParcels(tmp_path: Path) -> None:
-    """Test TemporalSNRParcels.
+def test_TemporalSNRParcels_storage(tmp_path: Path) -> None:
+    """Test TemporalSNRParcels store.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    # get a dataset
-    ni_data = datasets.fetch_spm_auditory(subject_id="sub001")
-    fmri_img = image.concat_imgs(ni_data.func)  # type: ignore
-
-    tsnr_parcels = TemporalSNRParcels(parcellation="Schaefer100x7")
-    all_out = tsnr_parcels.fit_transform(
-        {"BOLD": {"data": fmri_img, "meta": {}}}
-    )
-
-    out = all_out["BOLD"]
-
-    assert "data" in out
-    assert "col_names" in out
-
-    assert out["data"].shape[0] == 1
-    assert out["data"].shape[1] == 100
-    assert len(set(out["col_names"])) == 100
-
-    # check correct output
-    assert tsnr_parcels.get_output_type("BOLD") == "vector"
-
-    uri = tmp_path / "test_tsnr_parcellation.sqlite"
-    # Single storage, must be the uri
-    storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-    meta = {"element": {"subject": "test"}, "dependencies": {"numpy"}}
-    input = {"BOLD": {"data": fmri_img, "meta": meta}}
-    all_out = tsnr_parcels.fit_transform(input, storage=storage)
-
-    features = storage.list_features()
-    assert any(
-        x["name"] == "BOLD_TemporalSNRParcels" for x in features.values()
-    )
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        marker = TemporalSNRParcels(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym"
+        )
+        # Store
+        storage = HDF5FeatureStorage(tmp_path / "test_tsnr_parcels.hdf5")
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_TemporalSNRParcels" for x in features.values()
+        )
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/tests/test_collection.py` & `junifer-0.0.5.dev11/junifer/markers/tests/test_collection.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     MarkerCollection,
     ParcelAggregation,
 )
 from junifer.pipeline import PipelineStepMixin
 from junifer.preprocess import fMRIPrepConfoundRemover
 from junifer.storage import SQLiteFeatureStorage
 from junifer.testing.datagrabbers import (
-    OasisVBMTestingDataGrabber,
     PartlyCloudyTestingDataGrabber,
 )
 
 
 def test_marker_collection_incorrect_markers() -> None:
     """Test incorrect markers for MarkerCollection."""
     wrong_markers = [
@@ -42,77 +41,77 @@
         MarkerCollection(wrong_markers)  # type: ignore
 
 
 def test_marker_collection() -> None:
     """Test MarkerCollection."""
     markers = [
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="mean",
-            name="gmd_schaefer100x7_mean",
+            name="tian_mean",
         ),
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="std",
-            name="gmd_schaefer100x7_std",
+            name="tian_std",
         ),
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="trim_mean",
             method_params={"proportiontocut": 0.1},
-            name="gmd_schaefer100x7_trim_mean90",
+            name="tian_trim_mean90",
         ),
     ]
     mc = MarkerCollection(markers=markers)  # type: ignore
     assert mc._markers == markers
-    assert mc._preprocessing is None
+    assert mc._preprocessors is None
     assert mc._storage is None
     assert isinstance(mc._datareader, DefaultDataReader)
 
     # Create testing datagrabber
-    dg = OasisVBMTestingDataGrabber()
+    dg = PartlyCloudyTestingDataGrabber()
     mc.validate(dg)
 
     with dg:
         input = dg["sub-01"]
         out = mc.fit(input)
         assert out is not None
         assert isinstance(out, dict)
         assert len(out) == 3
-        assert "gmd_schaefer100x7_mean" in out
-        assert "gmd_schaefer100x7_std" in out
-        assert "gmd_schaefer100x7_trim_mean90" in out
+        assert "tian_mean" in out
+        assert "tian_std" in out
+        assert "tian_trim_mean90" in out
 
         for t_marker in markers:
             t_name = t_marker.name
-            assert "VBM_GM" in out[t_name]
-            t_vbm = out[t_name]["VBM_GM"]
-            assert "data" in t_vbm
-            assert "col_names" in t_vbm
-            assert "meta" in t_vbm
+            assert "BOLD" in out[t_name]
+            t_bold = out[t_name]["BOLD"]
+            assert "data" in t_bold
+            assert "col_names" in t_bold
+            assert "meta" in t_bold
 
     # Test preprocessing
     class BypassPreprocessing(PipelineStepMixin):
         def fit_transform(self, input):
             return input
 
     mc2 = MarkerCollection(
         markers=markers,  # type: ignore
-        preprocessing=BypassPreprocessing(),
+        preprocessors=[BypassPreprocessing()],  # type: ignore
         datareader=DefaultDataReader(),
     )
     assert isinstance(mc2._datareader, DefaultDataReader)
     with dg:
         input = dg["sub-01"]
         out2 = mc2.fit(input)
         assert out2 is not None
         for t_marker in markers:
             t_name = t_marker.name
             assert_array_equal(
-                out[t_name]["VBM_GM"]["data"], out2[t_name]["VBM_GM"]["data"]
+                out[t_name]["BOLD"]["data"], out2[t_name]["BOLD"]["data"]
             )
 
 
 def test_marker_collection_with_preprocessing() -> None:
     """Test MarkerCollection with preprocessing."""
     markers = [
         FunctionalConnectivityParcels(
@@ -124,18 +123,18 @@
             parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             agg_method="mean",
             name="TianxS2x3TxMNInonlinear2009cAsym_mean_FC",
         ),
     ]
     mc = MarkerCollection(
         markers=markers,  # type: ignore
-        preprocessing=fMRIPrepConfoundRemover(),
+        preprocessors=[fMRIPrepConfoundRemover()],
     )
     assert mc._markers == markers
-    assert mc._preprocessing is not None
+    assert mc._preprocessors is not None
     assert mc._storage is None
     assert isinstance(mc._datareader, DefaultDataReader)
 
     # Create testing datagrabber
     dg = PartlyCloudyTestingDataGrabber(reduce_confounds=False)
     mc.validate(dg)
 
@@ -147,35 +146,36 @@
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
     markers = [
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="mean",
-            name="gmd_schaefer100x7_mean",
+            name="tian_mean",
         ),
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="std",
-            name="gmd_schaefer100x7_std",
+            name="tian_std",
         ),
         ParcelAggregation(
-            parcellation="Schaefer100x7",
+            parcellation="TianxS2x3TxMNInonlinear2009cAsym",
             method="trim_mean",
             method_params={"proportiontocut": 0.1},
-            name="gmd_schaefer100x7_trim_mean90",
+            name="tian_trim_mean90",
         ),
     ]
-    # Test storage
-    dg = OasisVBMTestingDataGrabber()
-
-    uri = tmp_path / "test_marker_collection_storage.sqlite"
-    storage = SQLiteFeatureStorage(uri=uri)
+    # Setup datagrabber
+    dg = PartlyCloudyTestingDataGrabber()
+    # Setup storage
+    storage = SQLiteFeatureStorage(
+        tmp_path / "test_marker_collection_storage.sqlite"
+    )
     mc = MarkerCollection(
         markers=markers,  # type: ignore
         storage=storage,
         datareader=DefaultDataReader(),
     )
     mc.validate(dg)
     assert mc._storage is not None
@@ -193,27 +193,28 @@
 
     with dg:
         input = dg["sub-01"]
         out = mc2.fit(input)
 
     features = storage.list_features()
     assert len(features) == 3
+
     feature_md5 = next(iter(features.keys()))
     t_feature = storage.read_df(feature_md5=feature_md5)
-    fname = "gmd_schaefer100x7_mean"
-    t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
+    fname = "tian_mean"
+    t_data = out[fname]["BOLD"]["data"]  # type: ignore
+    cols = out[fname]["BOLD"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
 
     feature_md5 = list(features.keys())[1]
     t_feature = storage.read_df(feature_md5=feature_md5)
-    fname = "gmd_schaefer100x7_std"
-    t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
+    fname = "tian_std"
+    t_data = out[fname]["BOLD"]["data"]  # type: ignore
+    cols = out[fname]["BOLD"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
 
     feature_md5 = list(features.keys())[2]
     t_feature = storage.read_df(feature_md5=feature_md5)
-    fname = "gmd_schaefer100x7_trim_mean90"
-    t_data = out[fname]["VBM_GM"]["data"]  # type: ignore
-    cols = out[fname]["VBM_GM"]["col_names"]  # type: ignore
+    fname = "tian_trim_mean90"
+    t_data = out[fname]["BOLD"]["data"]  # type: ignore
+    cols = out[fname]["BOLD"]["col_names"]  # type: ignore
     assert_array_equal(t_feature[cols].values, t_data)  # type: ignore
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.5.dev11/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.5.dev11/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.5.dev11/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 import warnings
 from pathlib import Path
 
 import nibabel as nib
 import numpy as np
 import pytest
-from nilearn import datasets
-from nilearn.image import concat_imgs, math_img, new_img_like, resample_to_img
+from nilearn.image import math_img, new_img_like
 from nilearn.maskers import NiftiLabelsMasker, NiftiMasker
 from nilearn.masking import compute_brain_mask
 from numpy.testing import assert_array_almost_equal, assert_array_equal
 from scipy.stats import trim_mean
 
-from junifer.data import load_mask, load_parcellation, register_parcellation
+from junifer.data import get_mask, get_parcellation, register_parcellation
+from junifer.datareader import DefaultDataReader
 from junifer.markers.parcel_aggregation import ParcelAggregation
 from junifer.storage import SQLiteFeatureStorage
+from junifer.testing.datagrabbers import PartlyCloudyTestingDataGrabber
 
 
 def test_ParcelAggregation_input_output() -> None:
     """Test ParcelAggregation input and output types."""
     marker = ParcelAggregation(
         parcellation="Schaefer100x7", method="mean", on="VBM_GM"
     )
@@ -32,578 +33,680 @@
 
     with pytest.raises(ValueError, match="Unknown input"):
         marker.get_output_type("unknown")
 
 
 def test_ParcelAggregation_3D() -> None:
     """Test ParcelAggregation object on 3D images."""
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(n_rois=100)
-
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Mask parcellation manually
-    parcellation_img_res = resample_to_img(
-        parcellation.maps,
-        img,
-        interpolation="nearest",
-    )
-    parcellation_bin = math_img(
-        "img != 0",
-        img=parcellation_img_res,
-    )
-
-    # Create NiftiMasker
-    masker = NiftiMasker(parcellation_bin, target_affine=img.affine)
-    data = masker.fit_transform(img)
-    parcellation_values = masker.transform(parcellation_img_res)
-    parcellation_values = np.squeeze(parcellation_values).astype(int)
-
-    # Compute the mean manually
-    manual = []
-    for t_v in sorted(np.unique(parcellation_values)):
-        t_values = np.mean(data[:, parcellation_values == t_v])
-        manual.append(t_values)
-    manual = np.array(manual)[np.newaxis, :]
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(labels_img=parcellation.maps)
-    auto = nifti_masker.fit_transform(img)
-
-    # Check that arrays are almost equal
-    assert_array_almost_equal(auto, manual)
-
-    # Use the ParcelAggregation object
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    jun_values3d_mean = marker.fit_transform(input)["VBM_GM"]["data"]
-
-    assert jun_values3d_mean.ndim == 2
-    assert jun_values3d_mean.shape[0] == 1
-    assert_array_equal(manual, jun_values3d_mean)
-
-    # Test using another function (std)
-    manual = []
-    for t_v in sorted(np.unique(parcellation_values)):
-        t_values = np.std(data[:, parcellation_values == t_v])
-        manual.append(t_values)
-    manual = np.array(manual)[np.newaxis, :]
-
-    # Use the ParcelAggregation object
-    marker = ParcelAggregation(parcellation="Schaefer100x7", method="std")
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    jun_values3d_std = marker.fit_transform(input)["VBM_GM"]["data"]
-
-    assert jun_values3d_std.ndim == 2
-    assert jun_values3d_std.shape[0] == 1
-    assert_array_equal(manual, jun_values3d_std)
-
-    # Test using another function with parameters
-    manual = []
-    for t_v in sorted(np.unique(parcellation_values)):
-        t_values = trim_mean(
-            data[:, parcellation_values == t_v],
-            proportiontocut=0.1,
-            axis=None,  # type: ignore
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            on="BOLD",
+        )
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+
+        # Compare with nilearn
+        # Load testing parcellation
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Binarize parcellation
+        testing_parcellation_bin = math_img(
+            "img != 0",
+            img=testing_parcellation,
+        )
+        # Create NiftiMasker
+        masker = NiftiMasker(
+            testing_parcellation_bin,
+            target_affine=element_data["BOLD"]["data"].affine,
+        )
+        data = masker.fit_transform(element_data["BOLD"]["data"])
+        parcellation_values = np.squeeze(
+            masker.transform(testing_parcellation)
+        ).astype(int)
+        # Compute the mean manually
+        manual = []
+        for t_v in sorted(np.unique(parcellation_values)):
+            t_values = np.mean(data[:, parcellation_values == t_v])
+            manual.append(t_values)
+        manual = np.array(manual)[np.newaxis, :]
+
+        # Create NiftiLabelsMasker
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation
+        )
+        nifti_labels_masked_bold = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"].slicer[..., 0:1]
         )
-        manual.append(t_values)
-    manual = np.array(manual)[np.newaxis, :]
 
-    # Use the ParcelAggregation object
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="trim_mean",
-        method_params={"proportiontocut": 0.1},
-    )
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    jun_values3d_tm = marker.fit_transform(input)["VBM_GM"]["data"]
+        parcel_agg_mean_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+        # Check that arrays are almost equal
+        assert_array_equal(parcel_agg_mean_bold_data, manual)
+        assert_array_almost_equal(nifti_labels_masked_bold, manual)
+
+        # Check further
+        assert parcel_agg_mean_bold_data.ndim == 2
+        assert parcel_agg_mean_bold_data.shape[0] == 1
+        assert_array_equal(
+            nifti_labels_masked_bold.shape, parcel_agg_mean_bold_data.shape
+        )
+        assert_array_equal(nifti_labels_masked_bold, parcel_agg_mean_bold_data)
 
-    assert jun_values3d_tm.ndim == 2
-    assert jun_values3d_tm.shape[0] == 1
-    assert_array_equal(manual, jun_values3d_tm)
+        # Compute std manually
+        manual = []
+        for t_v in sorted(np.unique(parcellation_values)):
+            t_values = np.std(data[:, parcellation_values == t_v])
+            manual.append(t_values)
+        manual = np.array(manual)[np.newaxis, :]
+
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="std",
+            on="BOLD",
+        )
+        parcel_agg_std_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+        assert parcel_agg_std_bold_data.ndim == 2
+        assert parcel_agg_std_bold_data.shape[0] == 1
+        assert_array_equal(parcel_agg_std_bold_data, manual)
+
+        # Test using another function with parameters
+        manual = []
+        for t_v in sorted(np.unique(parcellation_values)):
+            t_values = trim_mean(
+                data[:, parcellation_values == t_v],
+                proportiontocut=0.1,
+                axis=None,  # type: ignore
+            )
+            manual.append(t_values)
+        manual = np.array(manual)[np.newaxis, :]
+
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="trim_mean",
+            method_params={"proportiontocut": 0.1},
+            on="BOLD",
+        )
+        parcel_agg_trim_mean_bold_data = marker.fit_transform(element_data)[
+            "BOLD"
+        ]["data"]
+        assert parcel_agg_trim_mean_bold_data.ndim == 2
+        assert parcel_agg_trim_mean_bold_data.shape[0] == 1
+        assert_array_equal(parcel_agg_trim_mean_bold_data, manual)
 
 
 def test_ParcelAggregation_4D():
     """Test ParcelAggregation object on 4D images."""
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(
-        n_rois=100, yeo_networks=7, resolution_mm=2
-    )
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym", method="mean"
+        )
+        parcel_agg_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+
+        # Compare with nilearn
+        # Load testing parcellation
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Extract data
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation
+        )
+        nifti_labels_masked_bold = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"]
+        )
 
-    # Get the SPM auditory data:
-    subject_data = datasets.fetch_spm_auditory()
-    fmri_img = concat_imgs(subject_data.func)  # type: ignore
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(labels_img=parcellation.maps)
-    auto4d = nifti_masker.fit_transform(fmri_img)
-
-    # Create ParcelAggregation object
-    marker = ParcelAggregation(parcellation="Schaefer100x7", method="mean")
-    input = {"BOLD": {"data": fmri_img, "meta": {}}}
-    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
-
-    assert jun_values4d.ndim == 2
-    assert_array_equal(auto4d.shape, jun_values4d.shape)
-    assert_array_equal(auto4d, jun_values4d)
+        assert parcel_agg_bold_data.ndim == 2
+        assert_array_equal(
+            nifti_labels_masked_bold.shape, parcel_agg_bold_data.shape
+        )
+        assert_array_equal(nifti_labels_masked_bold, parcel_agg_bold_data)
 
 
 def test_ParcelAggregation_storage(tmp_path: Path) -> None:
     """Test ParcelAggregation storage.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-    uri = tmp_path / "test_sphere_storage_3D.sqlite"
-
-    storage = SQLiteFeatureStorage(uri=uri, upsert="ignore")
-    meta = {
-        "element": {"subject": "sub-01", "session": "ses-01"},
-        "dependencies": {"nilearn", "nibabel"},
-    }
-    input = {"VBM_GM": {"data": img, "meta": meta}}
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7", method="mean", on="VBM_GM"
-    )
-
-    marker.fit_transform(input, storage=storage)
-
-    features = storage.list_features()
-    assert any(
-        x["name"] == "VBM_GM_ParcelAggregation" for x in features.values()
-    )
-
-    meta = {
-        "element": {"subject": "sub-01", "session": "ses-01"},
-        "dependencies": {"nilearn", "nibabel"},
-    }
-    # Get the SPM auditory data
-    subject_data = datasets.fetch_spm_auditory()
-    fmri_img = concat_imgs(subject_data.func)  # type: ignore
-    input = {"BOLD": {"data": fmri_img, "meta": meta}}
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7", method="mean", on="BOLD"
-    )
+    # Store 3D
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_parcel_storage_3D.sqlite", upsert="ignore"
+        )
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            on="BOLD",
+        )
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_ParcelAggregation" for x in features.values()
+        )
 
-    marker.fit_transform(input, storage=storage)
-    features = storage.list_features()
-    assert any(
-        x["name"] == "BOLD_ParcelAggregation" for x in features.values()
-    )
+    # Store 4D
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        storage = SQLiteFeatureStorage(
+            uri=tmp_path / "test_parcel_storage_4D.sqlite", upsert="ignore"
+        )
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            on="BOLD",
+        )
+        marker.fit_transform(input=element_data, storage=storage)
+        features = storage.list_features()
+        assert any(
+            x["name"] == "BOLD_ParcelAggregation" for x in features.values()
+        )
 
 
 def test_ParcelAggregation_3D_mask() -> None:
     """Test ParcelAggregation object on 3D images with mask."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+            masks="compute_brain_mask",
+        )
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+        parcel_agg_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+
+        # Compare with nilearn
+        # Load testing parcellation
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Load mask
+        mask_img = get_mask(
+            "compute_brain_mask", target_data=element_data["BOLD"]
+        )
+        # Extract data
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation, mask_img=mask_img
+        )
+        nifti_labels_masked_bold = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"].slicer[..., 0:1]
+        )
 
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(n_rois=100)
-
-    # Get one mask
-    mask_img, _ = load_mask("GM_prob0.2")
-
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(
-        labels_img=parcellation.maps, mask_img=mask_img
-    )
-    auto = nifti_masker.fit_transform(img)
-
-    # Use the ParcelAggregation object
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        masks="GM_prob0.2",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    jun_values3d_mean = marker.fit_transform(input)["VBM_GM"]["data"]
-
-    assert jun_values3d_mean.ndim == 2
-    assert jun_values3d_mean.shape[0] == 1
-    assert_array_almost_equal(auto, jun_values3d_mean)
+        assert parcel_agg_bold_data.ndim == 2
+        assert_array_equal(
+            nifti_labels_masked_bold.shape, parcel_agg_bold_data.shape
+        )
+        assert_array_equal(nifti_labels_masked_bold, parcel_agg_bold_data)
 
 
 def test_ParcelAggregation_3D_mask_computed() -> None:
     """Test ParcelAggregation object on 3D images with computed masks."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+
+        # Compare with nilearn
+        # Load testing parcellation
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Get a mask
+        mask_img = compute_brain_mask(
+            element_data["BOLD"]["data"], threshold=0.2
+        )
+        # Create NiftiLabelsMasker
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation, mask_img=mask_img
+        )
+        nifti_labels_masked_bold_good = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"]
+        )
 
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(n_rois=100)
-
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Get one mask
-    mask_img = compute_brain_mask(img, threshold=0.2)
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(
-        labels_img=parcellation.maps, mask_img=mask_img
-    )
-    auto = nifti_masker.fit_transform(img)
-
-    # Get one mask
-    mask_img = compute_brain_mask(img, threshold=0.5)
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(
-        labels_img=parcellation.maps, mask_img=mask_img
-    )
-    auto_bad = nifti_masker.fit_transform(img)
+        # Get another mask
+        mask_img = compute_brain_mask(
+            element_data["BOLD"]["data"], threshold=0.5
+        )
+        # Create NiftiLabelsMasker
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation, mask_img=mask_img
+        )
+        nifti_labels_masked_bold_bad = nifti_labels_masker.fit_transform(
+            mask_img
+        )
 
-    # Use the ParcelAggregation object
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        masks={"compute_brain_mask": {"threshold": 0.2}},
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    jun_values3d_mean = marker.fit_transform(input)["VBM_GM"]["data"]
-
-    assert jun_values3d_mean.ndim == 2
-    assert jun_values3d_mean.shape[0] == 1
-    assert_array_almost_equal(auto, jun_values3d_mean)
+        # Use the ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            masks={"compute_brain_mask": {"threshold": 0.2}},
+            name="tian_mean",
+            on="BOLD",
+        )
+        parcel_agg_mean_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+
+        assert parcel_agg_mean_bold_data.ndim == 2
+        assert parcel_agg_mean_bold_data.shape[0] == 1
+        assert_array_almost_equal(
+            nifti_labels_masked_bold_good, parcel_agg_mean_bold_data
+        )
 
-    with pytest.raises(AssertionError):
-        assert_array_almost_equal(jun_values3d_mean, auto_bad)
+        with pytest.raises(AssertionError):
+            assert_array_almost_equal(
+                parcel_agg_mean_bold_data, nifti_labels_masked_bold_bad
+            )
 
 
 def test_ParcelAggregation_3D_multiple_non_overlapping(tmp_path: Path) -> None:
     """Test ParcelAggregation with multiple non-overlapping parcellations.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+
+        # Load testing parcellation
+        testing_parcellation, labels = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
 
-    # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+        # Create two parcellations from it
+        parcellation_data = testing_parcellation.get_fdata()
+        parcellation1_data = parcellation_data.copy()
+        parcellation1_data[parcellation1_data > 8] = 0
+        parcellation2_data = parcellation_data.copy()
+        parcellation2_data[parcellation2_data <= 8] = 0
+        parcellation2_data[parcellation2_data > 0] -= 8
+        labels1 = labels[:8]
+        labels2 = labels[8:]
 
-    assert parcellation is not None
+        parcellation1_img = new_img_like(
+            testing_parcellation, parcellation1_data
+        )
+        parcellation2_img = new_img_like(
+            testing_parcellation, parcellation2_data
+        )
 
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Create two parcellations from it
-    parcellation_data = parcellation.get_fdata()
-    parcellation1_data = parcellation_data.copy()
-    parcellation1_data[parcellation1_data > 50] = 0
-    parcellation2_data = parcellation_data.copy()
-    parcellation2_data[parcellation2_data <= 50] = 0
-    parcellation2_data[parcellation2_data > 0] -= 50
-    labels1 = labels[:50]
-    labels2 = labels[50:]
-
-    parcellation1_img = new_img_like(parcellation, parcellation1_data)
-    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+        parcellation1_path = tmp_path / "parcellation1.nii.gz"
+        parcellation2_path = tmp_path / "parcellation2.nii.gz"
 
-    parcellation1_path = tmp_path / "parcellation1.nii.gz"
-    parcellation2_path = tmp_path / "parcellation2.nii.gz"
+        nib.save(parcellation1_img, parcellation1_path)
+        nib.save(parcellation2_img, parcellation2_path)
 
-    nib.save(parcellation1_img, parcellation1_path)
-    nib.save(parcellation2_img, parcellation2_path)
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_low",
+            parcellation_path=parcellation1_path,
+            parcels_labels=labels1,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_high",
+            parcellation_path=parcellation2_path,
+            parcels_labels=labels2,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
 
-    register_parcellation(
-        "Schaefer100x7_low", parcellation1_path, labels1, overwrite=True
-    )
-    register_parcellation(
-        "Schaefer100x7_high", parcellation2_path, labels2, overwrite=True
-    )
+        # Use the ParcelAggregation object on the original parcellation
+        marker_original = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+        orig_mean = marker_original.fit_transform(element_data)["BOLD"]
 
-    # Use the ParcelAggregation object on the original parcellation
-    marker_original = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    orig_mean = marker_original.fit_transform(input)["VBM_GM"]
-
-    orig_mean_data = orig_mean["data"]
-    assert orig_mean_data.ndim == 2
-    assert orig_mean_data.shape[0] == 1
-    assert orig_mean_data.shape[1] == 100
-    # assert_array_almost_equal(auto, jun_values3d_mean)
-
-    # Use the ParcelAggregation object on the two parcellations
-    marker_split = ParcelAggregation(
-        parcellation=["Schaefer100x7_low", "Schaefer100x7_high"],
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-
-    # No warnings should be raised
-    with warnings.catch_warnings():
-        warnings.simplefilter("error", category=UserWarning)
-        split_mean = marker_split.fit_transform(input)["VBM_GM"]
-    split_mean_data = split_mean["data"]
-
-    assert split_mean_data.ndim == 2
-    assert split_mean_data.shape[0] == 1
-    assert split_mean_data.shape[1] == 100
-
-    # Data and labels should be the same
-    assert_array_equal(orig_mean_data, split_mean_data)
-    assert orig_mean["col_names"] == split_mean["col_names"]
+        orig_mean_data = orig_mean["data"]
+        assert orig_mean_data.ndim == 2
+        assert orig_mean_data.shape == (1, 16)
+
+        # Use the ParcelAggregation object on the two parcellations
+        marker_split = ParcelAggregation(
+            parcellation=[
+                "TianxS1x3TxMNInonlinear2009cAsym_low",
+                "TianxS1x3TxMNInonlinear2009cAsym_high",
+            ],
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+
+        # No warnings should be raised
+        with warnings.catch_warnings():
+            warnings.simplefilter("error", category=UserWarning)
+            split_mean = marker_split.fit_transform(element_data)["BOLD"]
+
+        split_mean_data = split_mean["data"]
+
+        assert split_mean_data.ndim == 2
+        assert split_mean_data.shape == (1, 16)
+
+        # Data and labels should be the same
+        assert_array_equal(orig_mean_data, split_mean_data)
+        assert orig_mean["col_names"] == split_mean["col_names"]
 
 
 def test_ParcelAggregation_3D_multiple_overlapping(tmp_path: Path) -> None:
     """Test ParcelAggregation with multiple overlapping parcellations.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+
+        # Load testing parcellation
+        testing_parcellation, labels = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
 
-    # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+        # Create two parcellations from it
+        parcellation_data = testing_parcellation.get_fdata()
+        parcellation1_data = parcellation_data.copy()
+        parcellation1_data[parcellation1_data > 8] = 0
+        parcellation2_data = parcellation_data.copy()
+
+        # Make the second parcellation overlap with the first
+        parcellation2_data[parcellation2_data <= 6] = 0
+        parcellation2_data[parcellation2_data > 0] -= 6
+        labels1 = [f"low_{x}" for x in labels[:8]]  # Change the labels
+        labels2 = [f"high_{x}" for x in labels[6:]]  # Change the labels
 
-    assert parcellation is not None
+        parcellation1_img = new_img_like(
+            testing_parcellation, parcellation1_data
+        )
+        parcellation2_img = new_img_like(
+            testing_parcellation, parcellation2_data
+        )
 
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Create two parcellations from it
-    parcellation_data = parcellation.get_fdata()
-    parcellation1_data = parcellation_data.copy()
-    parcellation1_data[parcellation1_data > 50] = 0
-    parcellation2_data = parcellation_data.copy()
-
-    # Make the second parcellation overlap with the first
-    parcellation2_data[parcellation2_data <= 45] = 0
-    parcellation2_data[parcellation2_data > 0] -= 45
-    labels1 = [f"low_{x}" for x in labels[:50]]  # Change the labels
-    labels2 = [f"high_{x}" for x in labels[45:]]  # Change the labels
-
-    parcellation1_img = new_img_like(parcellation, parcellation1_data)
-    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+        parcellation1_path = tmp_path / "parcellation1.nii.gz"
+        parcellation2_path = tmp_path / "parcellation2.nii.gz"
 
-    parcellation1_path = tmp_path / "parcellation1.nii.gz"
-    parcellation2_path = tmp_path / "parcellation2.nii.gz"
+        nib.save(parcellation1_img, parcellation1_path)
+        nib.save(parcellation2_img, parcellation2_path)
 
-    nib.save(parcellation1_img, parcellation1_path)
-    nib.save(parcellation2_img, parcellation2_path)
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_low",
+            parcellation_path=parcellation1_path,
+            parcels_labels=labels1,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_high",
+            parcellation_path=parcellation2_path,
+            parcels_labels=labels2,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
 
-    register_parcellation(
-        "Schaefer100x7_low2", parcellation1_path, labels1, overwrite=True
-    )
-    register_parcellation(
-        "Schaefer100x7_high2", parcellation2_path, labels2, overwrite=True
-    )
+        # Use the ParcelAggregation object on the original parcellation
+        marker_original = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+        orig_mean = marker_original.fit_transform(element_data)["BOLD"]
 
-    # Use the ParcelAggregation object on the original parcellation
-    marker_original = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    orig_mean = marker_original.fit_transform(input)["VBM_GM"]
-
-    orig_mean_data = orig_mean["data"]
-    assert orig_mean_data.ndim == 2
-    assert orig_mean_data.shape[0] == 1
-    assert orig_mean_data.shape[1] == 100
-    # assert_array_almost_equal(auto, jun_values3d_mean)
-
-    # Use the ParcelAggregation object on the two parcellations
-    marker_split = ParcelAggregation(
-        parcellation=["Schaefer100x7_low2", "Schaefer100x7_high2"],
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    with pytest.warns(RuntimeWarning, match="overlapping voxels"):
-        split_mean = marker_split.fit_transform(input)["VBM_GM"]
-    split_mean_data = split_mean["data"]
-
-    assert split_mean_data.ndim == 2
-    assert split_mean_data.shape[0] == 1
-    assert split_mean_data.shape[1] == 105
-
-    # Overlapping voxels should be NaN
-    assert np.isnan(split_mean_data[:, 50:55]).all()
-
-    non_nan = split_mean_data[~np.isnan(split_mean_data)]
-    # Data should be the same
-    assert_array_equal(orig_mean_data, non_nan[None, :])
-
-    # Labels should be "low" for the first 50 and "high" for the second 50
-    assert all(x.startswith("low") for x in split_mean["col_names"][:50])
-    assert all(x.startswith("high") for x in split_mean["col_names"][50:])
+        orig_mean_data = orig_mean["data"]
+        assert orig_mean_data.ndim == 2
+        assert orig_mean_data.shape == (1, 16)
+
+        # Use the ParcelAggregation object on the two parcellations
+        marker_split = ParcelAggregation(
+            parcellation=[
+                "TianxS1x3TxMNInonlinear2009cAsym_low",
+                "TianxS1x3TxMNInonlinear2009cAsym_high",
+            ],
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+        # Warning should be raised
+        with pytest.warns(RuntimeWarning, match="overlapping voxels"):
+            split_mean = marker_split.fit_transform(element_data)["BOLD"]
+
+        split_mean_data = split_mean["data"]
+
+        assert split_mean_data.ndim == 2
+        assert split_mean_data.shape == (1, 18)
+
+        # Overlapping voxels should be NaN
+        assert np.isnan(split_mean_data[:, 8:10]).all()
+
+        non_nan = split_mean_data[~np.isnan(split_mean_data)]
+        # Data should be the same
+        assert_array_equal(orig_mean_data, non_nan[None, :])
+
+        # Labels should be "low" for the first 8 and "high" for the second 8
+        assert all(x.startswith("low") for x in split_mean["col_names"][:8])
+        assert all(x.startswith("high") for x in split_mean["col_names"][8:])
 
 
 def test_ParcelAggregation_3D_multiple_duplicated_labels(
     tmp_path: Path,
 ) -> None:
     """Test ParcelAggregation with two parcellations with duplicated labels.
 
     Parameters
     ----------
     tmp_path : pathlib.Path
         The path to the test directory.
 
     """
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+            ..., 0:1
+        ]
+
+        # Load testing parcellation
+        testing_parcellation, labels = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
 
-    # Get the testing parcellation
-    parcellation, labels, _ = load_parcellation("Schaefer100x7")
+        # Create two parcellations from it
+        parcellation_data = testing_parcellation.get_fdata()
+        parcellation1_data = parcellation_data.copy()
+        parcellation1_data[parcellation1_data > 8] = 0
+        parcellation2_data = parcellation_data.copy()
+        parcellation2_data[parcellation2_data <= 8] = 0
+        parcellation2_data[parcellation2_data > 0] -= 8
+        labels1 = labels[:8]
+        labels2 = labels[7:-1]  # One label is duplicated
 
-    assert parcellation is not None
+        parcellation1_img = new_img_like(
+            testing_parcellation, parcellation1_data
+        )
+        parcellation2_img = new_img_like(
+            testing_parcellation, parcellation2_data
+        )
 
-    # Get the oasis VBM data
-    oasis_dataset = datasets.fetch_oasis_vbm(n_subjects=1)
-    vbm = oasis_dataset.gray_matter_maps[0]
-    img = nib.load(vbm)
-
-    # Create two parcellations from it
-    parcellation_data = parcellation.get_fdata()
-    parcellation1_data = parcellation_data.copy()
-    parcellation1_data[parcellation1_data > 50] = 0
-    parcellation2_data = parcellation_data.copy()
-    parcellation2_data[parcellation2_data <= 50] = 0
-    parcellation2_data[parcellation2_data > 0] -= 50
-    labels1 = labels[:50]
-    labels2 = labels[49:-1]  # One label is duplicated
-
-    parcellation1_img = new_img_like(parcellation, parcellation1_data)
-    parcellation2_img = new_img_like(parcellation, parcellation2_data)
+        parcellation1_path = tmp_path / "parcellation1.nii.gz"
+        parcellation2_path = tmp_path / "parcellation2.nii.gz"
 
-    parcellation1_path = tmp_path / "parcellation1.nii.gz"
-    parcellation2_path = tmp_path / "parcellation2.nii.gz"
+        nib.save(parcellation1_img, parcellation1_path)
+        nib.save(parcellation2_img, parcellation2_path)
 
-    nib.save(parcellation1_img, parcellation1_path)
-    nib.save(parcellation2_img, parcellation2_path)
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_low",
+            parcellation_path=parcellation1_path,
+            parcels_labels=labels1,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
+        register_parcellation(
+            name="TianxS1x3TxMNInonlinear2009cAsym_high",
+            parcellation_path=parcellation2_path,
+            parcels_labels=labels2,
+            space="MNI152NLin2009cAsym",
+            overwrite=True,
+        )
 
-    register_parcellation(
-        "Schaefer100x7_low", parcellation1_path, labels1, overwrite=True
-    )
-    register_parcellation(
-        "Schaefer100x7_high", parcellation2_path, labels2, overwrite=True
-    )
+        # Use the ParcelAggregation object on the original parcellation
+        marker_original = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+        orig_mean = marker_original.fit_transform(element_data)["BOLD"]
 
-    # Use the ParcelAggregation object on the original parcellation
-    marker_original = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-    orig_mean = marker_original.fit_transform(input)["VBM_GM"]
-
-    orig_mean_data = orig_mean["data"]
-    assert orig_mean_data.ndim == 2
-    assert orig_mean_data.shape[0] == 1
-    assert orig_mean_data.shape[1] == 100
-    # assert_array_almost_equal(auto, jun_values3d_mean)
-
-    # Use the ParcelAggregation object on the two parcellations
-    marker_split = ParcelAggregation(
-        parcellation=["Schaefer100x7_low", "Schaefer100x7_high"],
-        method="mean",
-        name="gmd_schaefer100x7_mean",
-        on="VBM_GM",
-    )  # Test passing "on" as a keyword argument
-    input = {"VBM_GM": {"data": img, "meta": {}}}
-
-    with pytest.warns(RuntimeWarning, match="duplicated labels."):
-        split_mean = marker_split.fit_transform(input)["VBM_GM"]
-    split_mean_data = split_mean["data"]
-
-    assert split_mean_data.ndim == 2
-    assert split_mean_data.shape[0] == 1
-    assert split_mean_data.shape[1] == 100
-
-    # Data should be the same
-    assert_array_equal(orig_mean_data, split_mean_data)
-
-    # Labels should be prefixed with the parcellation name
-    col_names = [f"Schaefer100x7_low_{x}" for x in labels1]
-    col_names += [f"Schaefer100x7_high_{x}" for x in labels2]
-    assert col_names == split_mean["col_names"]
+        orig_mean_data = orig_mean["data"]
+        assert orig_mean_data.ndim == 2
+        assert orig_mean_data.shape == (1, 16)
+
+        # Use the ParcelAggregation object on the two parcellations
+        marker_split = ParcelAggregation(
+            parcellation=[
+                "TianxS1x3TxMNInonlinear2009cAsym_low",
+                "TianxS1x3TxMNInonlinear2009cAsym_high",
+            ],
+            method="mean",
+            name="tian_mean",
+            on="BOLD",
+        )
+
+        # Warning should be raised
+        with pytest.warns(RuntimeWarning, match="duplicated labels."):
+            split_mean = marker_split.fit_transform(element_data)["BOLD"]
+
+        split_mean_data = split_mean["data"]
+
+        assert split_mean_data.ndim == 2
+        assert split_mean_data.shape == (1, 16)
+
+        # Data should be the same
+        assert_array_equal(orig_mean_data, split_mean_data)
+
+        # Labels should be prefixed with the parcellation name
+        col_names = [
+            f"TianxS1x3TxMNInonlinear2009cAsym_low_{x}" for x in labels1
+        ]
+        col_names += [
+            f"TianxS1x3TxMNInonlinear2009cAsym_high_{x}" for x in labels2
+        ]
+        assert col_names == split_mean["col_names"]
 
 
 def test_ParcelAggregation_4D_agg_time():
     """Test ParcelAggregation object on 4D images, aggregating time."""
-    # Get the testing parcellation (for nilearn)
-    parcellation = datasets.fetch_atlas_schaefer_2018(
-        n_rois=100, yeo_networks=7, resolution_mm=2
-    )
-
-    # Get the SPM auditory data:
-    subject_data = datasets.fetch_spm_auditory()
-    fmri_img = concat_imgs(subject_data.func)  # type: ignore
-
-    # Create NiftiLabelsMasker
-    nifti_masker = NiftiLabelsMasker(labels_img=parcellation.maps)
-    auto4d = nifti_masker.fit_transform(fmri_img)
-    auto_mean = auto4d.mean(axis=0)
-
-    # Create ParcelAggregation object
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7", method="mean", time_method="mean"
-    )
-    input = {"BOLD": {"data": fmri_img, "meta": {}}}
-    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
-
-    assert jun_values4d.ndim == 1
-    assert_array_equal(auto_mean.shape, jun_values4d.shape)
-    assert_array_almost_equal(auto_mean, jun_values4d, decimal=2)
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        # Create ParcelAggregation object
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            time_method="mean",
+            on="BOLD",
+        )
+        parcel_agg_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+
+        # Compare with nilearn
+        # Loading testing parcellation
+        testing_parcellation, _ = get_parcellation(
+            parcellation=["TianxS1x3TxMNInonlinear2009cAsym"],
+            target_data=element_data["BOLD"],
+        )
+        # Extract data
+        nifti_labels_masker = NiftiLabelsMasker(
+            labels_img=testing_parcellation
+        )
+        nifti_labels_masked_bold = nifti_labels_masker.fit_transform(
+            element_data["BOLD"]["data"]
+        )
+        nifti_labels_masked_bold_mean = nifti_labels_masked_bold.mean(axis=0)
 
-    auto_pick_0 = auto4d[:1, :]
-    marker = ParcelAggregation(
-        parcellation="Schaefer100x7",
-        method="mean",
-        time_method="select",
-        time_method_params={"pick": [0]},
-    )
+        assert parcel_agg_bold_data.ndim == 1
+        assert_array_equal(
+            nifti_labels_masked_bold_mean.shape, parcel_agg_bold_data.shape
+        )
+        assert_array_almost_equal(
+            nifti_labels_masked_bold_mean, parcel_agg_bold_data, decimal=2
+        )
 
-    input = {"BOLD": {"data": fmri_img, "meta": {}}}
-    jun_values4d = marker.fit_transform(input)["BOLD"]["data"]
+        # Test picking first time point
+        nifti_labels_masked_bold_pick_0 = nifti_labels_masked_bold[:1, :]
+        marker = ParcelAggregation(
+            parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+            method="mean",
+            time_method="select",
+            time_method_params={"pick": [0]},
+            on="BOLD",
+        )
+        parcel_agg_bold_data = marker.fit_transform(element_data)["BOLD"][
+            "data"
+        ]
+
+        assert parcel_agg_bold_data.ndim == 2
+        assert_array_equal(
+            nifti_labels_masked_bold_pick_0.shape, parcel_agg_bold_data.shape
+        )
+        assert_array_equal(
+            nifti_labels_masked_bold_pick_0, parcel_agg_bold_data
+        )
 
-    assert jun_values4d.ndim == 2
-    assert_array_equal(auto_pick_0.shape, jun_values4d.shape)
-    assert_array_equal(auto_pick_0, jun_values4d)
 
+def test_ParcelAggregation_errors() -> None:
+    """Test errors for ParcelAggregation."""
     with pytest.raises(ValueError, match="can only be used with BOLD data"):
         ParcelAggregation(
             parcellation="Schaefer100x7",
             method="mean",
             time_method="select",
             time_method_params={"pick": [0]},
             on="VBM_GM",
@@ -615,10 +718,26 @@
         ParcelAggregation(
             parcellation="Schaefer100x7",
             method="mean",
             time_method_params={"pick": [0]},
             on="VBM_GM",
         )
 
-    with pytest.warns(RuntimeWarning, match="No time dimension to aggregate"):
-        input = {"BOLD": {"data": fmri_img.slicer[..., 0:1], "meta": {}}}
-        marker.fit_transform(input)
+
+def test_ParcelAggregation_warning() -> None:
+    """Test warning for ParcelAggregation."""
+    with PartlyCloudyTestingDataGrabber() as dg:
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        with pytest.warns(
+            RuntimeWarning, match="No time dimension to aggregate"
+        ):
+            marker = ParcelAggregation(
+                parcellation="TianxS1x3TxMNInonlinear2009cAsym",
+                method="mean",
+                time_method="select",
+                time_method_params={"pick": [0]},
+                on="BOLD",
+            )
+            element_data["BOLD"]["data"] = element_data["BOLD"]["data"].slicer[
+                ..., 0:1
+            ]
+            marker.fit_transform(element_data)
```

### Comparing `junifer-0.0.4.dev90/junifer/markers/utils.py` & `junifer-0.0.5.dev11/junifer/markers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Provide utility functions shared by different markers."""
 
 # Authors: Leonard Sasse <l.sasse@fz-juelich.de>
 #          Nicolás Nieto <n.nieto@fz-juelich.de>
 #          Sami Hamdan <s.hamdan@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 #          Federico Raimondo <f.raimondo@fz-juelich.de>
+#          Amir Omidvarnia <a.omidvarnia@fz-juelich.de>
 # License: AGPL
 
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import zscore
```

### Comparing `junifer-0.0.4.dev90/junifer/onthefly/read_transform.py` & `junifer-0.0.5.dev11/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.5.dev11/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.5.dev11/junifer/pipeline/pipeline_step_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         ValueError
             If the input does not have the required data.
 
         """
         raise_error(
             msg="Concrete classes need to implement validate_input().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
 
     def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
         input_type : str
@@ -59,90 +59,154 @@
         str
             The storage type output by the marker.
 
         """
         raise_error(
             msg="Concrete classes need to implement get_output_type().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
 
     def _fit_transform(
-        self, input: Dict[str, Dict], **kwargs: Any
+        self,
+        input: Dict[str, Dict],
     ) -> Dict[str, Dict]:
         """Fit and transform.
 
         Parameters
         ----------
         input : dict
             The Junifer Data object.
-        **kwargs : dict
-            Extra keyword arguments.
 
         Returns
         -------
         dict
             The processed output of the pipeline step.
 
         """
         raise_error(
             msg="Concrete classes need to implement _fit_transform().",
             klass=NotImplementedError,
-        )
+        )  # pragma: no cover
 
     def validate(self, input: List[str]) -> List[str]:
         """Validate the the pipeline step.
 
         Parameters
         ----------
         input : list of str
             The input to the pipeline step.
 
         Returns
         -------
         list of str
             The output of the pipeline step.
 
-        Raises
-        ------
-        ValueError
-            If the pipeline step object is missing dependencies required for
-            its working or if the input does not have the required data.
-
         """
-        # Check if _DEPENDENCIES attribute is found;
-        # (markers and preprocessors will have them but not datareaders
-        # as of now)
-        dependencies_not_found = []
-        if hasattr(self, "_DEPENDENCIES"):
-            # Check if dependencies are importable
-            for dependency in self._DEPENDENCIES:  # type: ignore
-                # First perform an easy check
-                if find_spec(dependency) is None:
-                    # Then check mapped names
-                    if dependency not in list(
-                        chain.from_iterable(packages_distributions().values())
-                    ):
-                        dependencies_not_found.append(dependency)
-        # Raise error if any dependency is not found
-        if dependencies_not_found:
-            raise_error(
-                msg=f"{dependencies_not_found} are not installed but are "
-                "required for using {self.name}.",
-                klass=ImportError,
-            )
-        # Check if _EXT_DEPENDENCIES attribute is found;
-        # (some markers might have them like ReHo-family)
-        if hasattr(self, "_EXT_DEPENDENCIES"):
-            for dependency in self._EXT_DEPENDENCIES:  # type: ignore
-                out = check_ext_dependencies(**dependency)
-                if getattr(self, f"use_{dependency['name']}", None) is None:
-                    # Set attribute for using external tools
-                    setattr(self, f"use_{dependency['name']}", out)
 
+        def _check_dependencies(obj) -> None:
+            """Check obj._DEPENDENCIES.
+
+            Parameters
+            ----------
+            obj : object
+                Object to check _DEPENDENCIES of.
+
+            Raises
+            ------
+            ImportError
+                If the pipeline step object is missing dependencies required
+                for its working.
+
+            """
+            # Check if _DEPENDENCIES attribute is found;
+            # (markers and preprocessors will have them but not datareaders
+            # as of now)
+            dependencies_not_found = []
+            if hasattr(obj, "_DEPENDENCIES"):
+                # Check if dependencies are importable
+                for dependency in obj._DEPENDENCIES:
+                    # First perform an easy check
+                    if find_spec(dependency) is None:
+                        # Then check mapped names
+                        if dependency not in list(
+                            chain.from_iterable(
+                                packages_distributions().values()
+                            )
+                        ):
+                            dependencies_not_found.append(dependency)
+            # Raise error if any dependency is not found
+            if dependencies_not_found:
+                raise_error(
+                    msg=(
+                        f"{dependencies_not_found} are not installed but are "
+                        f"required for using {obj.__class__.__name__}."
+                    ),
+                    klass=ImportError,
+                )
+
+        def _check_ext_dependencies(obj) -> None:
+            """Check obj._EXT_DEPENDENCIES.
+
+            Parameters
+            ----------
+            obj : object
+                Object to check _EXT_DEPENDENCIES of.
+
+            """
+            # Check if _EXT_DEPENDENCIES attribute is found;
+            # (some markers and preprocessors might have them)
+            if hasattr(obj, "_EXT_DEPENDENCIES"):
+                for dependency in obj._EXT_DEPENDENCIES:
+                    check_ext_dependencies(**dependency)
+
+        def _check_conditional_dependencies(obj) -> None:
+            """Check obj._CONDITIONAL_DEPENDENCIES.
+
+            Parameters
+            ----------
+            obj : object
+                Object to check _CONDITIONAL_DEPENDENCIES of.
+
+            Raises
+            ------
+            AttributeError
+                If the pipeline step object does not have `using` as a
+                constructor parameter.
+
+            """
+            # Check if _CONDITIONAL_DEPENDENCIES attribute is found;
+            # (some markers and preprocessors might have them)
+            if hasattr(obj, "_CONDITIONAL_DEPENDENCIES"):
+                if not hasattr(obj, "using"):
+                    raise_error(
+                        msg=(
+                            f"The pipeline step: {obj.__class__.__name__} has "
+                            "`_CONDITIONAL_DEPENDENCIES` but does not have "
+                            "`using` as a constructor parameter"
+                        ),
+                        klass=AttributeError,
+                    )
+                else:
+                    for dependency in obj._CONDITIONAL_DEPENDENCIES:
+                        if dependency["using"] == obj.using:
+                            depends_on = dependency["depends_on"]
+                            # Check dependencies
+                            _check_dependencies(depends_on)
+                            # Check external dependencies
+                            _check_ext_dependencies(depends_on)
+
+        # Check dependencies
+        _check_dependencies(self)
+        # Check external dependencies
+        _check_ext_dependencies(self)
+        # Check conditional dependencies
+        _check_conditional_dependencies(self)
+        # Validate input
         fit_input = self.validate_input(input=input)
+        # Validate output type
         outputs = [self.get_output_type(t_input) for t_input in fit_input]
         return outputs
 
     def fit_transform(
         self, input: Dict[str, Dict], **kwargs: Any
     ) -> Dict[str, Dict]:
         """Fit and transform.
```

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/registry.py` & `junifer-0.0.5.dev11/junifer/pipeline/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,19 @@
     step : str
         Name of the step.
     name : str
         Name of the function.
     klass : class
         Class to be registered.
 
+    Raises
+    ------
+    ValueError
+        If the ``step`` is invalid.
+
     """
     # Verify step
     if step not in _VALID_STEPS:
         raise_error(msg=f"Invalid step: {step}", klass=ValueError)
 
     logger.info(f"Registering {name} in {step}")
     _REGISTRY[step][name] = klass
@@ -59,14 +64,19 @@
         Name of the step.
 
     Returns
     -------
     list
         List of registered function names.
 
+    Raises
+    ------
+    ValueError
+        If the ``step`` is invalid.
+
     """
     # Verify step
     if step not in _VALID_STEPS:
         raise_error(msg=f"Invalid step: {step}", klass=ValueError)
 
     return list(_REGISTRY[step].keys())
 
@@ -82,14 +92,19 @@
         Name of the function.
 
     Returns
     -------
     class
         Registered function class.
 
+    Raises
+    ------
+    ValueError
+        If the ``step`` or ``name`` is invalid.
+
     """
     # Verify step
     if step not in _VALID_STEPS:
         raise_error(msg=f"Invalid step: {step}", klass=ValueError)
     # Verify step name
     if name not in _REGISTRY[step]:
         raise_error(msg=f"Invalid name: {name}", klass=ValueError)
@@ -119,14 +134,16 @@
     Returns
     -------
     object
         An instance of the given base class.
 
     Raises
     ------
+    RuntimeError
+        If there is a problem creating the instance.
     ValueError
         If the created object with the given name is not an instance of the
         base class.
 
     """
     # Set default init parameters
     if init_params is None:
```

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/singleton.py` & `junifer-0.0.5.dev11/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.5.dev11/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.5.dev11/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         The data object to update.
     step_name : str
         The name of the pipeline step.
     dependencies : set, list, None, str
         The dependencies of the pipeline step.
     expected : set
         The expected dependencies.
+
     """
 
     class TestUpdateMetaMixin(UpdateMetaMixin):
         """Test UpdateMetaMixin."""
 
         _DEPENDENCIES = dependencies
```

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.5.dev11/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.5.dev11/junifer/pipeline/update_meta_mixin.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,25 +19,31 @@
 
         Parameters
         ----------
         input : dict
             The data object to update.
         step_name : str
             The name of the pipeline step.
+
         """
+        # Initialize empty dictionary for the step's metadata
         t_meta = {}
+        # Set class name for the step
         t_meta["class"] = self.__class__.__name__
+        # Add object variables to metadata if name doesn't start with "_"
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 t_meta[k] = v
-
+        # Add "meta" to the step's local context dict
         if "meta" not in input:
             input["meta"] = {}
+        # Add step name
         input["meta"][step_name] = t_meta
+        # Add step dependencies
         if "dependencies" not in input["meta"]:
             input["meta"]["dependencies"] = set()
-
+        # Update step dependencies
         dependencies = getattr(self, "_DEPENDENCIES", set())
         if dependencies is not None:
             if not isinstance(dependencies, (set, list)):
                 dependencies = {dependencies}
             input["meta"]["dependencies"].update(dependencies)
```

### Comparing `junifer-0.0.4.dev90/junifer/pipeline/workdir_manager.py` & `junifer-0.0.5.dev11/junifer/pipeline/workdir_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     root_tempdir : pathlib.Path or None
         The path to the root temporary directory.
 
     """
 
     def __init__(self, workdir: Optional[Union[str, Path]] = None) -> None:
         """Initialize the class."""
-        self._workdir = workdir
+        self._workdir = Path(workdir) if isinstance(workdir, str) else workdir
         self._elementdir = None
         self._root_tempdir = None
 
         self._set_default_workdir()
 
     def _set_default_workdir(self) -> None:
         """Set the default working directory if not set already."""
```

### Comparing `junifer-0.0.4.dev90/junifer/preprocess/base.py` & `junifer-0.0.5.dev11/junifer/preprocess/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,58 @@
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from ..pipeline import PipelineStepMixin, UpdateMetaMixin
 from ..utils import logger, raise_error
 
 
 class BasePreprocessor(ABC, PipelineStepMixin, UpdateMetaMixin):
-    """Provide abstract base class for all preprocessors.
+    """Abstract base class for all preprocessors.
+
+    For every interface that is required, one needs to provide a concrete
+    implementation of this abstract class.
 
     Parameters
     ----------
-    on : str or list of str, optional
-        The kind of data to apply the preprocessor to. If None,
-        will work on all available data (default None).
+    on : str or list of str or None, optional
+        The data type to apply the preprocessor on. If None,
+        will work on all available data types (default None).
+    required_data_types : str or list of str, optional
+        The data types needed for computation. If None,
+        will be equal to ``on`` (default None).
+
+    Raises
+    ------
+    ValueError
+        If required input data type(s) is(are) not found.
+
     """
 
     def __init__(
         self,
         on: Optional[Union[List[str], str]] = None,
+        required_data_types: Optional[Union[List[str], str]] = None,
     ) -> None:
+        """Initialize the class."""
+        # Use all data types if not provided
         if on is None:
             on = self.get_valid_inputs()
+        # Convert data types to list
         if not isinstance(on, list):
             on = [on]
-
+        # Check if required inputs are found
         if any(x not in self.get_valid_inputs() for x in on):
             name = self.__class__.__name__
             wrong_on = [x for x in on if x not in self.get_valid_inputs()]
-            raise ValueError(f"{name} cannot be computed on {wrong_on}")
+            raise_error(f"{name} cannot be computed on {wrong_on}")
         self._on = on
+        # Set required data types for validation
+        if required_data_types is None:
+            self._required_data_types = on
+        else:
+            self._required_data_types = required_data_types
 
     def validate_input(self, input: List[str]) -> List[str]:
         """Validate input.
 
         Parameters
         ----------
         input : list of str
@@ -51,57 +72,90 @@
             The actual elements of the input that will be processed by this
             pipeline step.
 
         Raises
         ------
         ValueError
             If the input does not have the required data.
+
         """
-        if not any(x in input for x in self._on):
+        if any(x not in input for x in self._required_data_types):
             raise_error(
                 "Input does not have the required data."
                 f"\t Input: {input}"
-                f"\t Required (any of): {self._on}"
+                f"\t Required (all of): {self._required_data_types}"
             )
         return [x for x in self._on if x in input]
 
     @abstractmethod
-    def get_output_type(self, input: List[str]) -> List[str]:
+    def get_valid_inputs(self) -> List[str]:
+        """Get valid data types for input.
+
+        Returns
+        -------
+        list of str
+            The list of data types that can be used as input for this
+            preprocessor.
+
+        """
+        raise_error(
+            msg="Concrete classes need to implement get_valid_inputs().",
+            klass=NotImplementedError,
+        )
+
+    @abstractmethod
+    def get_output_type(self, input_type: str) -> str:
         """Get output type.
 
         Parameters
         ----------
-        input : list of str
-            The input to the preprocessor. The list must contain the
-            available Junifer Data dictionary keys.
+        input_type : str
+            The data type input to the preprocessor.
 
         Returns
         -------
-        list of str
-            The updated list of available Junifer Data object keys after
-            the pipeline step.
+        str
+            The data type output by the preprocessor.
 
         """
         raise_error(
             msg="Concrete classes need to implement get_output_type().",
             klass=NotImplementedError,
         )
 
     @abstractmethod
-    def get_valid_inputs(self) -> List[str]:
-        """Get valid data types for input.
+    def preprocess(
+        self,
+        input: Dict[str, Any],
+        extra_input: Optional[Dict[str, Any]] = None,
+    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Dict[str, Any]]]]:
+        """Preprocess.
+
+        Parameters
+        ----------
+        input : dict
+            A single input from the Junifer Data object to preprocess.
+        extra_input : dict, optional
+            The other fields in the Junifer Data object. Useful for accessing
+            other data kind that needs to be used in the computation. For
+            example, the confound removers can make use of the
+            confounds if available (default None).
 
         Returns
         -------
-        list of str
-            The list of data types that can be used as input for this
-            preprocessor.
+        dict
+            The computed result as dictionary.
+        dict or None
+            Extra "helper" data types as dictionary to add to the Junifer Data
+            object. For example, computed BOLD mask can be passed via this.
+            If no new "helper" data types is created, None is to be passed.
+
         """
         raise_error(
-            msg="Concrete classes need to implement get_valid_inputs().",
+            msg="Concrete classes need to implement preprocess().",
             klass=NotImplementedError,
         )
 
     def _fit_transform(
         self,
         input: Dict[str, Dict],
     ) -> Dict:
@@ -114,67 +168,40 @@
 
         Returns
         -------
         dict
             The processed output as a dictionary.
 
         """
-        out = input
+        # Copy input to not modify the original
+        out = input.copy()
+        # For each data type, run preprocessing
         for type_ in self._on:
+            # Check if data type is available
             if type_ in input.keys():
                 logger.info(f"Preprocessing {type_}")
+                # Get data dict for data type
                 t_input = input[type_]
-
                 # Pass the other data types as extra input, removing
                 # the current type
-                extra_input = input
+                extra_input = input.copy()
                 extra_input.pop(type_)
                 logger.debug(
-                    f"Extra input for preprocess: {extra_input.keys()}"
+                    f"Extra data type for preprocess: {extra_input.keys()}"
                 )
-                key, t_out = self.preprocess(
+                # Preprocess data
+                t_out, t_extra_input = self.preprocess(
                     input=t_input, extra_input=extra_input
                 )
-
-                # Add the output to the Junifer Data object
-                logger.debug(f"Adding {key} to output")
-                out[key] = t_out
-
-                # In case we are creating a new type, re-add the original input
-                if key != type_:
-                    logger.debug("Adding original input back to output")
-                    out[type_] = t_input
-
-                self.update_meta(out[key], "preprocess")
+                # Set output to the Junifer Data object
+                logger.debug(f"Adding {type_} to output")
+                out[type_] = t_out
+                # Check if helper data types are to be added
+                if t_extra_input is not None:
+                    logger.debug(
+                        f"Adding helper data types: {t_extra_input.keys()} "
+                        "to output"
+                    )
+                    out.update(t_extra_input)
+                # Update metadata for step
+                self.update_meta(out[type_], "preprocess")
         return out
-
-    @abstractmethod
-    def preprocess(
-        self,
-        input: Dict[str, Any],
-        extra_input: Optional[Dict[str, Any]] = None,
-    ) -> Tuple[str, Dict[str, Any]]:
-        """Preprocess.
-
-        Parameters
-        ----------
-        input : dict
-            A single input from the Junifer Data object to preprocess.
-        extra_input : dict, optional
-            The other fields in the Junifer Data object. Useful for accessing
-            other data kind that needs to be used in the computation. For
-            example, the confound removers can make use of the
-            confounds if available (default None).
-
-        Returns
-        -------
-        key : str
-            The key to store the output in the Junifer Data object.
-        object : dict
-            The computed result as dictionary. This will be stored in the
-            Junifer Data object under the key 'key'.
-
-        """
-        raise_error(
-            msg="Concrete classes need to implement preprocess().",
-            klass=NotImplementedError,
-        )
```

### Comparing `junifer-0.0.4.dev90/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.5.dev11/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,40 +2,35 @@
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import (
-    TYPE_CHECKING,
     Any,
     ClassVar,
     Dict,
     List,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
 import numpy as np
 import pandas as pd
+from nilearn import image as nimg
 from nilearn._utils.niimg_conversions import check_niimg_4d
-from nilearn.image import clean_img
 
 from ...api.decorators import register_preprocessor
 from ...data import get_mask
 from ...utils import logger, raise_error
 from ..base import BasePreprocessor
 
 
-if TYPE_CHECKING:
-    from nibabel import MGHImage, Nifti1Image, Nifti2Image
-
-
 FMRIPREP_BASICS = {
     "motion": [
         "trans_x",
         "trans_y",
         "trans_z",
         "rot_x",
         "rot_y",
@@ -160,15 +155,15 @@
         detrend: bool = True,
         standardize: bool = True,
         low_pass: Optional[float] = None,
         high_pass: Optional[float] = None,
         t_r: Optional[float] = None,
         masks: Union[str, Dict, List[Union[Dict, str]], None] = None,
     ) -> None:
-        """Initialise the class."""
+        """Initialize the class."""
         if strategy is None:
             strategy = {
                 "motion": "full",
                 "wm_csf": "full",
                 "global_signal": "full",
             }
         self.strategy = strategy
@@ -204,77 +199,46 @@
                 msg=f"Invalid confound types {list(strategy.values())}. "
                 f"Valid confound types are {self._valid_confounds}.\n"
                 f"If any of them is a valid parameter in "
                 "nilearn.interfaces.fmriprep.load_confounds we may "
                 "include it in the future",
                 klass=ValueError,
             )
-        super().__init__()
-
-    def validate_input(self, input: List[str]) -> List[str]:
-        """Validate the input to the pipeline step.
+        super().__init__(
+            on="BOLD", required_data_types=["BOLD", "BOLD_confounds"]
+        )
 
-        Parameters
-        ----------
-        input : list of str
-            The input to the pipeline step. The list must contain the
-            available Junifer Data object keys.
+    def get_valid_inputs(self) -> List[str]:
+        """Get valid data types for input.
 
         Returns
         -------
         list of str
-            The actual elements of the input that will be processed by this
-            pipeline step.
-
-        Raises
-        ------
-        ValueError
-            If the input does not have the required data.
+            The list of data types that can be used as input for this
+            preprocessor.
 
         """
-        _required_inputs = ["BOLD", "BOLD_confounds"]
-        if any(x not in input for x in _required_inputs):
-            raise_error(
-                msg="Input does not have the required data. \n"
-                f"Input: {input} \n"
-                f"Required (all off): {_required_inputs} \n",
-                klass=ValueError,
-            )
-
-        return [x for x in self._on if x in input]
+        return ["BOLD"]
 
-    def get_output_type(self, input: List[str]) -> List[str]:
-        """Get the kind of the pipeline step.
+    def get_output_type(self, input_type: str) -> str:
+        """Get output type.
 
         Parameters
         ----------
-        input : list of str
-            The input to the pipeline step. The list must contain the
-            available Junifer Data object keys.
+        input_type : str
+            The input to the preprocessor.
 
         Returns
         -------
-        list of str
-            The updated list of available Junifer Data object keys after
-            the pipeline step.
+        str
+            The data type output by the preprocessor.
 
         """
         # Does not add any new keys
-        return input
-
-    def get_valid_inputs(self) -> List[str]:
-        """Get the valid inputs for the pipeline step.
-
-        Returns
-        -------
-        list of str
-            The valid inputs for the pipeline step.
-
-        """
-        return ["BOLD"]
+        return input_type
 
     def _map_adhoc_to_fmriprep(self, input: Dict[str, Any]) -> None:
         """Map the adhoc format to the fmpriprep format spec.
 
         Based on the spec, map the column names to match the fmriprep format.
 
         It assumes that the data is valid, meaning that all the mapping
@@ -329,29 +293,34 @@
         derivatives_to_compute : dict
             Dictionary containing the missing derivatives confounds to compute
             (keys) and the corresponding confounds to compute the derivative
             from (values)
         spike_name : str
             Name of the confound to use for spike detection
 
+        Raises
+        ------
+        ValueError
+            If invalid confounds file is found.
+
         """
         confounds_df = input["data"]
         available_vars = confounds_df.columns
 
         # This function should build this 3 variables
         to_select = []  # the list of confounds to select
         squares_to_compute = {}  # the dictionary of missing squares
         derivatives_to_compute = {}  # the dictionary of missing derivatives
 
         for t_kind, t_strategy in self.strategy.items():
             t_basics = FMRIPREP_BASICS[t_kind]
 
             if any(x not in available_vars for x in t_basics):
                 missing = [x for x in t_basics if x not in available_vars]
-                raise ValueError(
+                raise_error(
                     "Invalid confounds file. Missing basic confounds: "
                     f"{missing}. "
                     "Check if this file is really an fmriprep confounds file. "
                     "You can also modify the confound removal strategy."
                 )
 
             to_select.extend(t_basics)
@@ -373,15 +342,15 @@
                         x_derivative_2 = f"{x_derivative}_power2"
                         to_select.append(x_derivative_2)
                         if x_derivative_2 not in available_vars:
                             squares_to_compute[x_derivative_2] = x_derivative
         spike_name = "framewise_displacement"
         if self.spike is not None:
             if spike_name not in available_vars:
-                raise ValueError(
+                raise_error(
                     "Invalid confounds file. Missing framewise_displacement "
                     "(spike) confound. "
                     "Check if this file is really an fmriprep confounds file. "
                     "You can also deactivate spike (set spike = None)."
                 )
         out = to_select, squares_to_compute, derivatives_to_compute, spike_name
         return out
@@ -456,178 +425,166 @@
         input : dict
             Dictionary containing the ``BOLD`` value from the
             Junifer Data object.
         extra_input : dict, optional
             Dictionary containing the rest of the Junifer Data object. Must
             include the ``BOLD_confounds`` key.
 
-        """
+        Raises
+        ------
+        ValueError
+            If ``extra_input`` is None or
+            if ``"BOLD_confounds"`` is not found in ``extra_input`` or
+            if ``"data"`` key is not found in ``"BOLD_confounds"`` or
+            if ``"data"`` is not pandas.DataFrame or
+            if image time series and confounds have different lengths or
+            if ``"format"`` is not found in ``"BOLD_confounds"`` or
+            if ``format = "adhoc"`` and ``"mappings"`` key or ``"fmriprep"``
+            key or correct fMRIPrep mappings or required fMRIPrep mappings are
+            not found or if invalid confounds format is found.
 
-        # Bold must be 4D niimg
+        """
+        # BOLD must be 4D niimg
         check_niimg_4d(input["data"])
-
+        # Check for extra inputs
         if extra_input is None:
-            raise_error("No extra input provided", ValueError)
+            raise_error(
+                "No extra input provided, requires `BOLD_confounds` data type "
+                "in particular"
+            )
         if "BOLD_confounds" not in extra_input:
-            raise_error("No BOLD_confounds provided", ValueError)
+            raise_error("`BOLD_confounds` data type not provided")
         if "data" not in extra_input["BOLD_confounds"]:
-            raise_error("No BOLD_confounds data provided", ValueError)
-        # Confounds must be a dataframe
+            raise_error("`BOLD_confounds.data` not provided")
+        # Confounds must be a pandas.DataFrame
         if not isinstance(extra_input["BOLD_confounds"]["data"], pd.DataFrame):
-            raise_error(
-                "Confounds data must be a pandas dataframe", ValueError
-            )
+            raise_error("`BOLD_confounds.data` must be a `pandas.DataFrame`")
 
         confound_df = extra_input["BOLD_confounds"]["data"]
         bold_img = input["data"]
         if bold_img.get_fdata().shape[3] != len(confound_df):
             raise_error(
                 "Image time series and confounds have different length!\n"
                 f"\tImage time series: { bold_img.get_fdata().shape[3]}\n"
                 f"\tConfounds: {len(confound_df)}"
             )
 
+        # Check format
         if "format" not in extra_input["BOLD_confounds"]:
-            raise_error(
-                "Confounds format must be specified in "
-                'input["BOLD_confounds"]'
-            )
-
+            raise_error("`BOLD_confounds.format` not provided")
         t_format = extra_input["BOLD_confounds"]["format"]
-
         if t_format == "adhoc":
             if "mappings" not in extra_input["BOLD_confounds"]:
                 raise_error(
-                    "When using adhoc format, you must specify "
-                    "the variables names mappings in "
-                    'input["BOLD_confounds"]["mappings"]'
+                    "`BOLD_confounds.mappings` need to be set when "
+                    "`BOLD_confounds.format == 'adhoc'`"
                 )
             if "fmriprep" not in extra_input["BOLD_confounds"]["mappings"]:
                 raise_error(
-                    "When using adhoc format, you must specify "
-                    "the variables names mappings to fmriprep format in "
-                    'input["BOLD_confounds"]["mappings"]["fmriprep"]'
+                    "`BOLD_confounds.mappings.fmriprep` need to be set when "
+                    "`BOLD_confounds.format == 'adhoc'`"
                 )
             fmriprep_mappings = extra_input["BOLD_confounds"]["mappings"][
                 "fmriprep"
             ]
             wrong_names = [
                 x
                 for x in fmriprep_mappings.values()
                 if x not in FMRIPREP_VALID_NAMES
             ]
             if len(wrong_names) > 0:
                 raise_error(
-                    "The following mapping values are not valid fmriprep "
+                    "The following mapping values are not valid fMRIPrep "
                     f"names: {wrong_names}"
                 )
             # Check that all the required columns are present
             missing = [
                 x
                 for x in fmriprep_mappings.keys()
                 if x not in confound_df.columns
             ]
 
             if len(missing) > 0:
-                raise ValueError(
+                raise_error(
                     "Invalid confounds file. Missing columns: "
                     f"{missing}. "
                     "Check if this file matches the adhoc specification for "
                     "this dataset."
                 )
         elif t_format != "fmriprep":
-            raise ValueError(f"Invalid confounds format {t_format}")
+            raise_error(f"Invalid confounds format {t_format}")
 
-    def _remove_confounds(
+    def preprocess(
         self,
         input: Dict[str, Any],
         extra_input: Optional[Dict[str, Any]] = None,
-    ) -> Union["Nifti1Image", "Nifti2Image", "MGHImage", List]:
-        """Remove confounds from the BOLD image.
+    ) -> Tuple[Dict[str, Any], Optional[Dict[str, Dict[str, Any]]]]:
+        """Preprocess.
 
         Parameters
         ----------
         input : dict
-            Dictionary containing the ``BOLD`` value from the
-            Junifer Data object.
+            A single input from the Junifer Data object to preprocess.
         extra_input : dict, optional
-            Dictionary containing the rest of the Junifer Data object. Must
-            include the ``BOLD_confounds`` key.
+            The other fields in the Junifer Data object. Must include the
+            ``BOLD_confounds`` key.
 
         Returns
         -------
-        Niimg-like object
-            Input image with confounds removed.
+        dict
+            The computed result as dictionary.
+        dict or None
+            If `self.masks` is not None, then the target data computed mask is
+            returned else None.
 
         """
-        assert extra_input is not None  # Not the case, data is validated
-        confounds_df = self._pick_confounds(extra_input["BOLD_confounds"])
-        confounds_array = confounds_df.values
-
+        # Validate data
+        self._validate_data(input, extra_input)
+        # Pick confounds
+        confounds_df = self._pick_confounds(extra_input["BOLD_confounds"])  # type: ignore
+        # Get BOLD data
         bold_img = input["data"]
+        # Set t_r
         t_r = self.t_r
         if t_r is None:
-            logger.info("No `t_r` specified, using t_r from nifti header")
-            zooms = bold_img.header.get_zooms()  # type: ignore
-            t_r = zooms[3]
+            logger.info("No `t_r` specified, using t_r from NIfTI header")
+            t_r = bold_img.header.get_zooms()[3]  # type: ignore
             logger.info(
-                f"Read t_r from nifti header: {t_r}",
+                f"Read t_r from NIfTI header: {t_r}",
             )
-
+        # Set mask data
         mask_img = None
+        bold_mask_dict = None
         if self.masks is not None:
             logger.debug(f"Masking with {self.masks}")
             mask_img = get_mask(
                 masks=self.masks, target_data=input, extra_input=extra_input
             )
-            # Save the mask in the extra input and link it to the bold data
+            # Return the BOLD mask and link it to the BOLD data type dict;
             # this allows to use "inherit" down the pipeline
             if extra_input is not None:
-                logger.debug("Setting mask_item")
-                extra_input["BOLD_mask"] = {"data": mask_img}
+                logger.debug("Setting `BOLD.mask_item`")
                 input["mask_item"] = "BOLD_mask"
-
-        logger.info("Cleaning image")
+                bold_mask_dict = {
+                    "BOLD_mask": {
+                        "data": mask_img,
+                        "space": input["space"],
+                    }
+                }
+        # Clean image
+        logger.info("Cleaning image using nilearn")
         logger.debug(f"\tdetrend: {self.detrend}")
         logger.debug(f"\tstandardize: {self.standardize}")
         logger.debug(f"\tlow_pass: {self.low_pass}")
         logger.debug(f"\thigh_pass: {self.high_pass}")
-        clean_bold = clean_img(
+        input["data"] = nimg.clean_img(
             imgs=bold_img,
             detrend=self.detrend,
             standardize=self.standardize,
-            confounds=confounds_array,
+            confounds=confounds_df.values,
             low_pass=self.low_pass,
             high_pass=self.high_pass,
             t_r=t_r,
             mask_img=mask_img,
         )
 
-        return clean_bold
-
-    def preprocess(
-        self,
-        input: Dict[str, Any],
-        extra_input: Optional[Dict[str, Any]] = None,
-    ) -> Tuple[str, Dict[str, Any]]:
-        """Preprocess.
-
-        Parameters
-        ----------
-        input : dict
-            A single input from the Junifer Data object in which to preprocess.
-        extra_input : dict, optional
-            The other fields in the Junifer Data object. Must include the
-            ``BOLD_confounds`` key.
-
-        Returns
-        -------
-        key : str
-            The key to store the output in the Junifer Data object.
-        object : dict
-            The computed result as dictionary. This will be stored in the
-            Junifer Data object under the key ``key``.
-
-        """
-        self._validate_data(input, extra_input)
-        input["data"] = self._remove_confounds(input, extra_input=extra_input)
-        return "BOLD", input
+        return input, bold_mask_dict
```

### Comparing `junifer-0.0.4.dev90/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.5.dev11/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Provide tests for fMRIPrepConfoundRemover."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
-import typing
+from typing import List
 
-import nibabel as nib
 import numpy as np
 import pandas as pd
 import pytest
 from nilearn._utils.exceptions import DimensionError
 from numpy.testing import assert_array_equal, assert_raises
 from pandas.testing import assert_frame_equal
 
@@ -36,47 +35,70 @@
     with pytest.raises(ValueError, match="component names"):
         fMRIPrepConfoundRemover(strategy={"wrong": "full"})
 
     with pytest.raises(ValueError, match="confound types"):
         fMRIPrepConfoundRemover(strategy={"motion": "wrong"})
 
 
-def test_fMRIPrepConfoundRemover_validate_input() -> None:
-    """Test fMRIPrepConfoundRemover validate_input."""
-    confound_remover = fMRIPrepConfoundRemover()
+@pytest.mark.parametrize(
+    "input_",
+    [
+        ["T1w"],
+        ["BOLD"],
+        ["T1w", "BOLD"],
+    ],
+)
+def test_fMRIPrepConfoundRemover_validate_input_errors(
+    input_: List[str],
+) -> None:
+    """Test errors for fMRIPrepConfoundRemover validate_input.
+
+    Parameters
+    ----------
+    input_ : list of str
+        The input data types.
 
-    # Input is valid when both BOLD and BOLD_confounds are present
+    """
+    confound_remover = fMRIPrepConfoundRemover()
 
-    input = ["T1w"]
     with pytest.raises(ValueError, match="not have the required data"):
-        confound_remover.validate_input(input)
+        confound_remover.validate_input(input_)
 
-    input = ["BOLD"]
-    with pytest.raises(ValueError, match="not have the required data"):
-        confound_remover.validate_input(input)
 
-    input = ["BOLD", "T1w"]
-    with pytest.raises(ValueError, match="not have the required data"):
-        confound_remover.validate_input(input)
+@pytest.mark.parametrize(
+    "input_",
+    [
+        ["BOLD", "BOLD_confounds"],
+        ["T1w", "BOLD", "BOLD_confounds"],
+    ],
+)
+def test_fMRIPrepConfoundRemover_validate_input(input_: List[str]) -> None:
+    """Test fMRIPrepConfoundRemover validate_input.
 
-    input = ["BOLD", "T1w", "BOLD_confounds"]
-    confound_remover.validate_input(input)
+    Parameters
+    ----------
+    input_ : list of str
+        The input data types.
+
+    """
+    confound_remover = fMRIPrepConfoundRemover()
+    confound_remover.validate_input(input_)
+
+
+def test_fMRIPrepConfoundRemover_get_valid_inputs() -> None:
+    """Test fMRIPrepConfoundRemover get_valid_inputs."""
+    confound_remover = fMRIPrepConfoundRemover()
+    assert confound_remover.get_valid_inputs() == ["BOLD"]
 
 
 def test_fMRIPrepConfoundRemover_get_output_type() -> None:
-    """Test fMRIPrepConfoundRemover validate_input."""
+    """Test fMRIPrepConfoundRemover get_output_type."""
     confound_remover = fMRIPrepConfoundRemover()
-    inputs = [
-        ["BOLD", "T1w", "BOLD_confounds"],
-        ["BOLD", "VBM_GM", "BOLD_confounds"],
-        ["BOLD", "BOLD_confounds"],
-    ]
     # Confound remover works in place
-    for input in inputs:
-        assert confound_remover.get_output_type(input) == input
+    assert confound_remover.get_output_type("BOLD") == "BOLD"
 
 
 def test_fMRIPrepConfoundRemover__map_adhoc_to_fmriprep() -> None:
     """Test fMRIPrepConfoundRemover adhoc to fmriprep spec mapping."""
     confound_remover = fMRIPrepConfoundRemover()
     # Use non fmriprep variable names
     adhoc_names = [f"var{i}" for i in range(6)]
@@ -255,15 +277,15 @@
         "format": "adhoc",
     }
 
     out = confound_remover._pick_confounds(input)
     assert set(out.columns) == set(fmriprep_all_vars)
 
 
-def test_FMRIPRepConfoundRemover__pick_confounds_fmriprep() -> None:
+def test_fMRIPRepConfoundRemover__pick_confounds_fmriprep() -> None:
     """Test fMRIPrepConfoundRemover pick confounds on fmriprep confounds."""
     confound_remover = fMRIPrepConfoundRemover(
         strategy={"wm_csf": "full"}, spike=0.2
     )
     fmriprep_all_vars = [
         "csf",
         "white_matter",
@@ -288,15 +310,15 @@
         input = reader.fit_transform(input)
         out2 = confound_remover._pick_confounds(input["BOLD_confounds"])
         assert set(out2.columns) == {*fmriprep_all_vars, "spike"}
 
     assert_frame_equal(out1, out2)
 
 
-def test_FMRIPRepConfoundRemover__pick_confounds_fmriprep_compute() -> None:
+def test_fMRIPRepConfoundRemover__pick_confounds_fmriprep_compute() -> None:
     """Test if fmriprep returns the same derivatives/power2 as we compute."""
 
     confound_remover = fMRIPrepConfoundRemover(strategy={"wm_csf": "full"})
     fmriprep_all_vars = [
         "csf",
         "white_matter",
         "csf_power2",
@@ -322,200 +344,173 @@
     assert np.all(out_fmriprep.values != np.nan)
     assert_frame_equal(out_junifer, out_fmriprep)
 
 
 def test_fMRIPrepConfoundRemover__validate_data() -> None:
     """Test fMRIPrepConfoundRemover validate data."""
     confound_remover = fMRIPrepConfoundRemover(strategy={"wm_csf": "full"})
-    reader = DefaultDataReader()
+
     with OasisVBMTestingDataGrabber() as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        new_input = input["VBM_GM"]
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        vbm = element_data["VBM_GM"]
         with pytest.raises(
             DimensionError, match="incompatible dimensionality"
         ):
-            confound_remover._validate_data(new_input, None)
+            confound_remover._validate_data(vbm, None)
 
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        new_input = input["BOLD"]
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        bold = element_data["BOLD"]
 
         with pytest.raises(ValueError, match="No extra input"):
-            confound_remover._validate_data(new_input, None)
-        with pytest.raises(ValueError, match="No BOLD_confounds provided"):
-            confound_remover._validate_data(new_input, {})
+            confound_remover._validate_data(bold, None)
         with pytest.raises(
-            ValueError, match="No BOLD_confounds data provided"
+            ValueError, match="`BOLD_confounds` data type not provided"
         ):
-            confound_remover._validate_data(new_input, {"BOLD_confounds": {}})
+            confound_remover._validate_data(bold, {})
+        with pytest.raises(
+            ValueError, match="`BOLD_confounds.data` not provided"
+        ):
+            confound_remover._validate_data(bold, {"BOLD_confounds": {}})
 
         extra_input = {
             "BOLD_confounds": {"data": "wrong"},
         }
-        msg = "must be a pandas dataframe"
+        msg = "must be a `pandas.DataFrame`"
         with pytest.raises(ValueError, match=msg):
-            confound_remover._validate_data(new_input, extra_input)
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {"BOLD_confounds": {"data": pd.DataFrame()}}
         with pytest.raises(ValueError, match="Image time series and"):
-            confound_remover._validate_data(new_input, extra_input)
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
-            "BOLD_confounds": {"data": input["BOLD_confounds"]["data"]}
+            "BOLD_confounds": {"data": element_data["BOLD_confounds"]["data"]}
         }
-        with pytest.raises(ValueError, match="format must be specified"):
-            confound_remover._validate_data(new_input, extra_input)
+        with pytest.raises(
+            ValueError, match="`BOLD_confounds.format` not provided"
+        ):
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "wrong",
             }
         }
-        with pytest.raises(ValueError, match="Invalid confounds format wrong"):
-            confound_remover._validate_data(new_input, extra_input)
+        with pytest.raises(ValueError, match="Invalid confounds format"):
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "adhoc",
             }
         }
-        with pytest.raises(ValueError, match="variables names mappings"):
-            confound_remover._validate_data(new_input, extra_input)
+        with pytest.raises(ValueError, match="need to be set"):
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "adhoc",
                 "mappings": {},
             }
         }
-        with pytest.raises(ValueError, match="mappings to fmriprep"):
-            confound_remover._validate_data(new_input, extra_input)
+        with pytest.raises(ValueError, match="need to be set"):
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "adhoc",
                 "mappings": {
                     "fmriprep": {
                         "rot_x": "wrong",
                         "rot_y": "rot_z",
                         "rot_z": "rot_y",
                     }
                 },
             }
         }
         with pytest.raises(ValueError, match=r"names: \['wrong'\]"):
-            confound_remover._validate_data(new_input, extra_input)
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "adhoc",
                 "mappings": {
                     "fmriprep": {
                         "wrong": "rot_x",
                         "rot_y": "rot_z",
                         "rot_z": "rot_y",
                     }
                 },
             }
         }
         with pytest.raises(ValueError, match=r"Missing columns: \['wrong'\]"):
-            confound_remover._validate_data(new_input, extra_input)
+            confound_remover._validate_data(bold, extra_input)
 
         extra_input = {
             "BOLD_confounds": {
-                "data": input["BOLD_confounds"]["data"],
+                "data": element_data["BOLD_confounds"]["data"],
                 "format": "adhoc",
                 "mappings": {
                     "fmriprep": {
                         "rot_x": "rot_x",
                         "rot_y": "rot_z",
                         "rot_z": "rot_y",
                     }
                 },
             }
         }
-        confound_remover._validate_data(new_input, extra_input)
-
-
-def test_fMRIPrepConfoundRemover__remove_confounds() -> None:
-    """Test fMRIPrepConfoundRemover remove confounds."""
-    confound_remover = fMRIPrepConfoundRemover(
-        strategy={"wm_csf": "full"}, spike=0.2
-    )
-    reader = DefaultDataReader()
-    with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        raw_bold = input["BOLD"]["data"]
-        extra_input = {k: v for k, v in input.items() if k != "BOLD"}
-        clean_bold = confound_remover._remove_confounds(
-            input=input["BOLD"], extra_input=extra_input
-        )
-        clean_bold = typing.cast(nib.Nifti1Image, clean_bold)
-        # TODO: Find a better way to test functionality here
-        assert (
-            clean_bold.header.get_zooms()  # type: ignore
-            == raw_bold.header.get_zooms()  # type: ignore
-        )
-        assert clean_bold.get_fdata().shape == raw_bold.get_fdata().shape
-    # TODO: Test confound remover with mask, needs #79 to be implemented
+        confound_remover._validate_data(bold, extra_input)
 
 
 def test_fMRIPrepConfoundRemover_preprocess() -> None:
     """Test fMRIPrepConfoundRemover with all confounds present."""
-
-    # need reader for the data
-    reader = DefaultDataReader()
     # All strategies full, no spike
     confound_remover = fMRIPrepConfoundRemover()
 
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        orig_bold = input["BOLD"]["data"].get_fdata().copy()
-        pre_input = input["BOLD"]
-        pre_extra_input = {"BOLD_confounds": input["BOLD_confounds"]}
-        key, output = confound_remover.preprocess(pre_input, pre_extra_input)
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        orig_bold = element_data["BOLD"]["data"].get_fdata().copy()
+        pre_input = element_data["BOLD"]
+        pre_extra_input = {"BOLD_confounds": element_data["BOLD_confounds"]}
+        output, _ = confound_remover.preprocess(pre_input, pre_extra_input)
         trans_bold = output["data"].get_fdata()
         # Transformation is in place
-        assert_array_equal(trans_bold, input["BOLD"]["data"].get_fdata())
+        assert_array_equal(
+            trans_bold, element_data["BOLD"]["data"].get_fdata()
+        )
 
         # Data should have the same shape
         assert orig_bold.shape == trans_bold.shape
 
         # but be different
         assert_raises(
             AssertionError, assert_array_equal, orig_bold, trans_bold
         )
-        assert key == "BOLD"
 
 
 def test_fMRIPrepConfoundRemover_fit_transform() -> None:
     """Test fMRIPrepConfoundRemover with all confounds present."""
-
-    # need reader for the data
-    reader = DefaultDataReader()
     # All strategies full, no spike
     confound_remover = fMRIPrepConfoundRemover()
 
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        orig_bold = input["BOLD"]["data"].get_fdata().copy()
-        output = confound_remover.fit_transform(input)
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        orig_bold = element_data["BOLD"]["data"].get_fdata().copy()
+        output = confound_remover.fit_transform(element_data)
         trans_bold = output["BOLD"]["data"].get_fdata()
         # Transformation is in place
-        assert_array_equal(trans_bold, input["BOLD"]["data"].get_fdata())
+        assert_array_equal(
+            trans_bold, element_data["BOLD"]["data"].get_fdata()
+        )
 
         # Data should have the same shape
         assert orig_bold.shape == trans_bold.shape
 
         # but be different
         assert_raises(
             AssertionError, assert_array_equal, orig_bold, trans_bold
@@ -531,37 +526,37 @@
         assert t_meta["detrend"] is True
         assert t_meta["standardize"] is True
         assert t_meta["low_pass"] is None
         assert t_meta["high_pass"] is None
         assert t_meta["t_r"] is None
         assert t_meta["masks"] is None
 
+        assert "BOLD_mask" not in output
+
         assert "dependencies" in output["BOLD"]["meta"]
         dependencies = output["BOLD"]["meta"]["dependencies"]
         assert dependencies == {"numpy", "nilearn"}
 
 
 def test_fMRIPrepConfoundRemover_fit_transform_masks() -> None:
     """Test fMRIPrepConfoundRemover with all confounds present."""
-
-    # need reader for the data
-    reader = DefaultDataReader()
     # All strategies full, no spike
     confound_remover = fMRIPrepConfoundRemover(
         masks={"compute_brain_mask": {"threshold": 0.2}}
     )
 
     with PartlyCloudyTestingDataGrabber(reduce_confounds=False) as dg:
-        input = dg["sub-01"]
-        input = reader.fit_transform(input)
-        orig_bold = input["BOLD"]["data"].get_fdata().copy()
-        output = confound_remover.fit_transform(input)
+        element_data = DefaultDataReader().fit_transform(dg["sub-01"])
+        orig_bold = element_data["BOLD"]["data"].get_fdata().copy()
+        output = confound_remover.fit_transform(element_data)
         trans_bold = output["BOLD"]["data"].get_fdata()
         # Transformation is in place
-        assert_array_equal(trans_bold, input["BOLD"]["data"].get_fdata())
+        assert_array_equal(
+            trans_bold, element_data["BOLD"]["data"].get_fdata()
+        )
 
         # Data should have the same shape
         assert orig_bold.shape == trans_bold.shape
 
         # but be different
         assert_raises(
             AssertionError, assert_array_equal, orig_bold, trans_bold
```

### Comparing `junifer-0.0.4.dev90/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.5.dev11/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         def __init__(self, on):
             self.parameter = 1
             super().__init__(on=on)
 
         def get_valid_inputs(self):
             return ["BOLD", "T1w"]
 
-        def get_output_type(self, input):
-            return ["timeseries"]
+        def get_output_type(self, input_type):
+            return input_type
 
-        def preprocess(self, input, extra_input):
-            input["data"] = f"mofidied_{input['data']}"
-            return "BOLD", input
+        def preprocess(self, input, extra_input=None):
+            input["data"] = f"modified_{input['data']}"
+            return input, extra_input
 
     with pytest.raises(ValueError, match=r"cannot be computed on \['T2w'\]"):
         MyBasePreprocessor(on=["BOLD", "T2w"])
 
     with pytest.raises(ValueError, match=r"cannot be computed on \['T2w'\]"):
         MyBasePreprocessor(on="T2w")
 
@@ -66,15 +66,15 @@
     with pytest.raises(ValueError, match="not have the required data"):
         prep.validate_input(["T1w"])
 
     output = prep.fit_transform(input=input_)  # process
     # Check output
     assert "BOLD" in output
     assert "data" in output["BOLD"]
-    assert output["BOLD"]["data"] == "mofidied_data"
+    assert output["BOLD"]["data"] == "modified_data"
     assert "path" in output["BOLD"]
     assert "meta" in output["BOLD"]
 
     meta = output["BOLD"]["meta"]
     assert "preprocess" in meta
     assert "class" in meta["preprocess"]
     assert "MyBasePreprocessor" == meta["preprocess"]["class"]
```

### Comparing `junifer-0.0.4.dev90/junifer/stats.py` & `junifer-0.0.5.dev11/junifer/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from typing import Any, Callable, Dict, List, Optional
 
 import numpy as np
-from scipy.stats import trim_mean
+from scipy.stats import mode, trim_mean
 from scipy.stats.mstats import winsorize
 
 from .utils import logger, raise_error
 
 
 def get_aggfunc_by_name(
     name: str, func_params: Optional[Dict[str, Any]] = None
@@ -20,41 +20,44 @@
 
     Parameters
     ----------
     name : str
         Name to identify the function. Currently supported names and
         corresponding functions are:
 
-        * ``winsorized_mean`` -> :func:`scipy.stats.mstats.winsorize`
         * ``mean`` -> :func:`numpy.mean`
-        * ``std`` -> :func:`numpy.std`
+        * ``winsorized_mean`` -> :func:`scipy.stats.mstats.winsorize`
         * ``trim_mean`` -> :func:`scipy.stats.trim_mean`
+        * ``mode`` -> :func:`scipy.stats.mode`
+        * ``std`` -> :func:`numpy.std`
         * ``count`` -> :func:`.count`
         * ``select`` -> :func:`.select`
 
     func_params : dict, optional
         Parameters to pass to the function.
         E.g. for ``winsorized_mean``: ``func_params = {'limits': [0.1, 0.1]}``
         (default None).
 
     Returns
     -------
     function
         Respective function with ``func_params`` parameter set.
+
     """
     from functools import partial  # local import to avoid sphinx error
 
     # check validity of names
     _valid_func_names = {
         "winsorized_mean",
         "mean",
         "std",
         "trim_mean",
         "count",
         "select",
+        "mode",
     }
     if func_params is None:
         func_params = {}
     # apply functions
     if name == "winsorized_mean":
         # check validity of func_params
         limits = func_params.get("limits")
@@ -89,14 +92,16 @@
         pick = func_params.get("pick", None)
         drop = func_params.get("drop", None)
         if pick is None and drop is None:
             raise_error("Either pick or drop must be specified.")
         elif pick is not None and drop is not None:
             raise_error("Either pick or drop must be specified, not both.")
         func = partial(select, **func_params)
+    elif name == "mode":
+        func = partial(mode, **func_params)
     else:
         raise_error(
             f"Function {name} unknown. Please provide any of "
             f"{_valid_func_names}"
         )
     return func
 
@@ -111,14 +116,15 @@
     axis : int, optional
         The axis to count elements on (default 0).
 
     Returns
     -------
     numpy.ndarray
         Number of elements along the given axis.
+
     """
     ax_size = data.shape[axis]
     if axis < 0:
         axis = data.ndim + axis
     # keep the shape on the other axes
     out = np.ones([x for i, x in enumerate(data.shape) if i != axis]) * ax_size
     return out
@@ -133,26 +139,27 @@
     ----------
     data : numpy.ndarray
         Data to calculate winsorized mean on.
     axis : int, optional
         The axis to calculate winsorized mean on (default None).
     **win_params : dict
         Dictionary containing the keyword arguments for the winsorize function.
-        E.g. ``{'limits': [0.1, 0.1]}``.
+        E.g., ``{'limits': [0.1, 0.1]}``.
 
     Returns
     -------
     numpy.ndarray
         Winsorized mean of the inputted data with the winsorize settings
         applied as specified in ``win_params``.
 
     See Also
     --------
     scipy.stats.mstats.winsorize :
         The winsorize function used in this function.
+
     """
     win_dat = winsorize(data, axis=axis, **win_params)
     win_mean = win_dat.mean(axis=axis)
 
     return win_mean
 
 
@@ -176,14 +183,21 @@
         List of indices to drop (default None).
 
     Returns
     -------
     numpy.ndarray
         Subset of the inputted data with the select settings
         applied as specified in ``select_params``.
+
+    Raises
+    ------
+    ValueError
+        If both ``pick`` and ``drop`` are None or
+        if both ``pick`` and ``drop`` are not None.
+
     """
 
     if pick is None and drop is None:
         raise_error("Either pick or drop must be specified.")
     elif pick is not None and drop is not None:
         raise_error("Either pick or drop must be specified, not both.")
     elif drop is not None:
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/base.py` & `junifer-0.0.5.dev11/junifer/storage/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,30 +26,37 @@
     uri : str or pathlib.Path
         The path to the storage.
     storage_types : str or list of str
         The available storage types for the class.
     single_output : bool, optional
         Whether to have single output (default True).
 
+    Raises
+    ------
+    ValueError
+        If required storage type(s) is(are) missing from ``storage_types``.
+
     """
 
     def __init__(
         self,
         uri: Union[str, Path],
         storage_types: Union[List[str], str],
         single_output: bool = True,
     ) -> None:
         self.uri = uri
+        # Convert storage_types to list
         if not isinstance(storage_types, list):
             storage_types = [storage_types]
+        # Check if required inputs are found
         if any(x not in self.get_valid_inputs() for x in storage_types):
             wrong_storage_types = [
                 x for x in storage_types if x not in self.get_valid_inputs()
             ]
-            raise ValueError(
+            raise_error(
                 f"{self.__class__.__name__} cannot store {wrong_storage_types}"
             )
         self._valid_inputs = storage_types
         self.single_output = single_output
 
     def get_valid_inputs(self) -> List[str]:
         """Get valid storage types for input.
@@ -166,14 +173,15 @@
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         meta : dict
             The metadata as a dictionary.
+
         """
         raise_error(
             msg="Concrete classes need to implement store_metadata().",
             klass=NotImplementedError,
         )
 
     def store(self, kind: str, **kwargs) -> None:
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/hdf5.py` & `junifer-0.0.5.dev11/junifer/storage/hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     ChunkedArray or ChunkedList
         The chunked array or list.
 
     Raises
     ------
     ValueError
         If `kind` is not one of ['vector', 'matrix', 'timeseries'].
+
     """
     if kind in ["vector", "matrix"]:
         features_data = np.concatenate(chunk_data, axis=-1)
         array_shape = [features_data.shape[0]]
         array_chunk_size = [features_data.shape[0]]
         # Append second dimension for 3D
         if features_data.ndim == 3:
@@ -674,17 +675,21 @@
             if data.dtype == np.dtype("float64") and self.force_float32:
                 data = data.astype(
                     dtype=np.dtype("float32"), casting="same_kind"
                 )
         elif isinstance(data, list):
             if self.force_float32:
                 data = [
-                    x.astype(dtype=np.dtype("float32"), casting="same_kind")
-                    if x.dtype == np.dtype("float64")
-                    else x
+                    (
+                        x.astype(
+                            dtype=np.dtype("float32"), casting="same_kind"
+                        )
+                        if x.dtype == np.dtype("float64")
+                        else x
+                    )
                     for x in data
                 ]
         # Handle cases for existing and new entry
         if not stored_data:
             logger.debug(f"Writing new data for {meta_md5} ...")
             # New entry; add as is
             data_to_write.update(
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/pandas_base.py` & `junifer-0.0.5.dev11/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/storage/sqlite.py` & `junifer-0.0.5.dev11/junifer/storage/sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,15 @@
         ----------
         meta_md5 : str
             The metadata MD5 hash.
         element : dict
             The element as a dictionary.
         meta : dict
             The metadata as a dictionary.
+
         """
         # Get sqlalchemy engine
         engine = self.get_engine(element=element)
         table_name = f"meta_{meta_md5}"
         if table_name not in inspect(engine).get_table_names():
             # Convert metadata to dataframe
             meta_df = self._meta_row(meta=meta, meta_md5=meta_md5)
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.5.dev11/junifer/storage/tests/test_hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -834,14 +834,15 @@
 
     Returns
     -------
     str
         The meta md5.
     dict
         The data to store.
+
     """
     all_data = []
     t_md5 = None
     if kind == "vector":
         data_to_store = {
             "data": np.arange(10),
             "col_names": [f"col-{i}" for i in range(10)],
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.5.dev11/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.5.dev11/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.5.dev11/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/storage/tests/test_utils.py` & `junifer-0.0.5.dev11/junifer/storage/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 )
 
 
 @pytest.mark.parametrize(
     "dependency, max_version",
     [
         ("click", "8.2"),
-        ("numpy", "1.26"),
-        ("datalad", "0.19"),
-        ("pandas", "1.6"),
-        ("nibabel", "4.1"),
-        ("nilearn", "0.10.0"),
-        ("sqlalchemy", "1.5.0"),
+        ("numpy", "1.27"),
+        ("datalad", "0.20"),
+        ("pandas", "2.2"),
+        ("nibabel", "5.11"),
+        ("nilearn", "0.11.0"),
+        ("sqlalchemy", "2.1.0"),
         ("ruamel.yaml", "0.18.0"),
     ],
 )
 def test_get_dependency_version(dependency: str, max_version: str) -> None:
     """Test dependency resolution for installed dependencies.
 
     Parameters
```

### Comparing `junifer-0.0.4.dev90/junifer/storage/utils.py` & `junifer-0.0.5.dev11/junifer/storage/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     element : dict
         The element to convert to prefix.
 
     Returns
     -------
     str
         The element converted to prefix.
+
     """
     logger.debug(f"Converting element {element} to prefix.")
     prefix = "element"
     if not isinstance(element, dict):
         raise_error(msg="`element` must be a dict")
 
     prefix = f"{prefix}_{'_'.join([f'{x}' for x in element.values()])}"
```

### Comparing `junifer-0.0.4.dev90/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.5.dev11/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/datagrabbers.py` & `junifer-0.0.5.dev11/junifer/testing/datagrabbers.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         -------
         dict
             The data along with the metadata.
 
         """
         out = {}
         i_sub = int(subject.split("-")[1]) - 1
-        out["VBM_GM"] = {"path": Path(self._dataset.gray_matter_maps[i_sub])}
+        out["VBM_GM"] = {
+            "path": Path(self._dataset.gray_matter_maps[i_sub]),
+            "space": "MNI152Lin",
+        }
 
         return out
 
     def __enter__(self) -> "OasisVBMTestingDataGrabber":
         """Implement context entry.
 
         Returns
@@ -137,16 +140,16 @@
         fmri_img = image.concat_imgs(nilearn_data.func)  # type: ignore
         anat_img = image.concat_imgs(nilearn_data.anat)  # type: ignore
 
         fmri_fname = self.datadir / f"{subject}_bold.nii.gz"
         anat_fname = self.datadir / f"{subject}_T1w.nii.gz"
         nib.save(fmri_img, fmri_fname)
         nib.save(anat_img, anat_fname)
-        out["BOLD"] = {"path": fmri_fname}
-        out["T1w"] = {"path": anat_fname}
+        out["BOLD"] = {"path": fmri_fname, "space": "MNI152Lin"}
+        out["T1w"] = {"path": anat_fname, "space": "native"}
         return out
 
 
 class PartlyCloudyTestingDataGrabber(BaseDataGrabber):
     """DataGrabber for Partly Cloudy dataset.
 
     Wrapper for :func:`nilearn.datasets.fetch_development_fmri`.
@@ -232,16 +235,17 @@
         -------
         dict
             The data along with the metadata.
 
         """
         out = {}
         i_sub = int(subject.split("-")[1]) - 1
-        out["BOLD"] = {"path": Path(self._dataset["func"][i_sub])}
-        conf_format = "fmriprep"
-
+        out["BOLD"] = {
+            "path": Path(self._dataset["func"][i_sub]),
+            "space": "MNI152NLin2009cAsym",
+        }
         out["BOLD_confounds"] = {
             "path": Path(self._dataset["confounds"][i_sub]),
-            "format": conf_format,
+            "format": "fmriprep",
         }
 
         return out
```

### Comparing `junifer-0.0.4.dev90/junifer/testing/registry.py` & `junifer-0.0.5.dev11/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.5.dev11/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.5.dev11/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.5.dev11/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.5.dev11/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/testing/utils.py` & `junifer-0.0.5.dev11/junifer/testing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,13 @@
     fname : str
         The name of the file.
 
     Returns
     -------
     pathlib.Path
         The absolute path to the file.
+
     """
     t_path = Path(__file__).parent / "data" / fname
     if not t_path.exists():
         raise FileNotFoundError(f"File {fname} not found in testing data")
     return t_path.resolve()
```

### Comparing `junifer-0.0.4.dev90/junifer/tests/test_stats.py` & `junifer-0.0.5.dev11/junifer/tests/test_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     [
         ("winsorized_mean", {"limits": [0.2, 0.7]}),
         ("mean", None),
         ("std", None),
         ("count", None),
         ("trim_mean", None),
         ("trim_mean", {"proportiontocut": 0.1}),
+        ("mode", None),
+        ("mode", {"keepdims": True}),
     ],
 )
 def test_get_aggfunc_by_name(name: str, params: Optional[Dict]) -> None:
     """Test aggregation function retrieval by name.
 
     Parameters
     ----------
```

### Comparing `junifer-0.0.4.dev90/junifer/utils/logging.py` & `junifer-0.0.5.dev11/junifer/utils/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Provide class and functions for logging."""
 
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
+try:
+    from distutils.version import LooseVersion
+except ImportError:  # pragma: no cover
+    from looseversion import LooseVersion
+
 import logging
 import sys
-from distutils.version import LooseVersion
 from pathlib import Path
 from subprocess import PIPE, Popen, TimeoutExpired
 from typing import Dict, NoReturn, Optional, Type, Union
 from warnings import warn
 
 import datalad
 
@@ -56,17 +60,24 @@
 
     Returns
     -------
     str
         Empty string if timeout expired for subprocess command execution else
         git HEAD information.
 
+    Raises
+    ------
+    FileNotFoundError
+        If ``path`` is invalid.
+
     """
     if not path.exists():
-        raise ValueError(f"This path does not exist: {path}")
+        raise_error(
+            msg=f"This path does not exist: {path}", klass=FileNotFoundError
+        )
     command = f"cd {path}; git rev-parse --verify HEAD"
     process = Popen(
         args=command,
         stdout=PIPE,
         shell=True,
     )
     try:
@@ -84,15 +95,15 @@
     Returns
     -------
     module_versions : dict
         The module names and corresponding versions.
 
     """
     module_versions = {}
-    for name, module in sys.modules.items():
+    for name, module in sys.modules.copy().items():
         # Bypassing sub-modules of packages and
         # allowing ruamel.yaml
         if "." in name and name != "ruamel.yaml":
             continue
         if name in ["_curses"]:
             continue
         vstring = str(getattr(module, "__version__", None))
```

### Comparing `junifer-0.0.4.dev90/junifer/utils/tests/test_fs.py` & `junifer-0.0.5.dev11/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer/utils/tests/test_logging.py` & `junifer-0.0.5.dev11/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/junifer.egg-info/PKG-INFO` & `junifer-0.0.5.dev11/junifer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.4.dev90
+Version: 0.0.5.dev11
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
-Project-URL: homepage, https://juaml.github.io/junifer
-Project-URL: documentation, https://juaml.github.io/junifer
-Project-URL: repository, https://github.com/juaml/junifer
+Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
+Project-URL: Documentation, https://juaml.github.io/junifer
+Project-URL: Homepage, https://juaml.github.io/junifer
+Project-URL: Source, https://github.com/juaml/junifer
 Keywords: neuroimaging
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 Requires-Dist: click<8.2,>=8.1.3
 Requires-Dist: numpy<1.27,>=1.24
+Requires-Dist: scipy<=1.11.4,>=1.9.0
 Requires-Dist: datalad<0.20,>=0.15.4
 Requires-Dist: pandas<2.2,>=1.4.0
 Requires-Dist: nibabel<5.11,>=3.2.0
-Requires-Dist: nilearn<=0.11.0,>=0.9.0
+Requires-Dist: nilearn<=0.10.2,>=0.9.0
 Requires-Dist: sqlalchemy<=2.1.0,>=1.4.27
 Requires-Dist: ruamel.yaml<0.18,>=0.17
+Requires-Dist: h5py>=3.10
+Requires-Dist: httpx[http2]==0.26.0
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: templateflow>=23.0.0
 Requires-Dist: importlib_metadata; python_version < "3.10"
-Requires-Dist: h5py<3.10,>=3.8.0
+Requires-Dist: looseversion==1.3.0; python_version >= "3.12"
+Provides-Extra: all
+Requires-Dist: bctpy==0.6.0; extra == "all"
+Requires-Dist: neurokit2>=0.1.7; extra == "all"
+Provides-Extra: bct
+Requires-Dist: bctpy==0.6.0; extra == "bct"
+Provides-Extra: onthefly
+Requires-Dist: bctpy==0.6.0; extra == "onthefly"
+Provides-Extra: neurokit2
+Requires-Dist: neurokit2>=0.1.7; extra == "neurokit2"
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: seaborn<0.13,>=0.11.2; extra == "docs"
 Requires-Dist: sphinx<7.3,>=5.3.0; extra == "docs"
 Requires-Dist: sphinx-gallery<0.15.0,>=0.11.0; extra == "docs"
 Requires-Dist: furo<2023.10.0,>=2022.9.29; extra == "docs"
 Requires-Dist: numpydoc<1.6,>=1.5.0; extra == "docs"
 Requires-Dist: julearn<0.4,>=0.3.0; extra == "docs"
 Requires-Dist: sphinx-copybutton<0.5.3,>=0.5.1; extra == "docs"
 Requires-Dist: towncrier<23.7,>=22.12.0; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid<0.10,>=0.8.1; extra == "docs"
-Provides-Extra: onthefly
-Requires-Dist: bctpy==0.6.0; extra == "onthefly"
 
 ![Junifer logo](docs/images/junifer_logo.png "junifer logo")
 
 # junifer - JUelich NeuroImaging FEature extractoR
 
 ![PyPI](https://img.shields.io/pypi/v/junifer?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/junifer?style=flat-square)
@@ -62,14 +76,15 @@
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/junifer/badges/version.svg)](https://anaconda.org/conda-forge/junifer)
 ![GitHub](https://img.shields.io/github/license/juaml/junifer?style=flat-square)
 ![Codecov](https://img.shields.io/codecov/c/github/juaml/junifer?style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8176570.svg)](https://doi.org/10.5281/zenodo.8176570)
+[![FAIR checklist badge](https://fairsoftwarechecklist.net/badge.svg)](https://fairsoftwarechecklist.net/v0.2?f=31&a=32113&i=32322&r=133)
 
 ## About
 
 `junifer` is a data handling and feature extraction library targeted towards neuroimaging data specifically functional MRI data.
 
 It is currently being developed and maintained at the [Applied Machine Learning](https://www.fz-juelich.de/en/inm/inm-7/research-groups/applied-machine-learning-aml) group at [Forschungszentrum Juelich](https://www.fz-juelich.de/en), Germany. Although the library is designed for people working at [Institute of Neuroscience and Medicine - Brain and Behaviour (INM-7)](https://www.fz-juelich.de/en/inm/inm-7), it is designed to be as modular as possible thus enabling others to extend it easily.
 
@@ -88,15 +103,15 @@
   * `external`: Module for external libraries and tools.
   * `markers`: Markers module.
   * `onthefly`: Transformation components (on-the-fly) module.
   * `pipeline`: Pipeline module.
   * `preprocess`: Preprocessing module.
   * `storage`: Storage module.
   * `testing`: Testing components module.
-  * `utils`: Utilities module (e.g. logging)
+  * `utils`: Utilities module (e.g. logging).
 
 ## Installation
 
 Use `pip` to install from PyPI like so:
 
 ```
 pip install junifer
@@ -104,14 +119,29 @@
 
 You can also install via `conda`, like so:
 
 ```
 conda install -c conda-forge junifer
 ```
 
+### Optional dependencies
+
+`junifer` supports a few optional dependencies to enable certain features. You can
+install them by specifying a comma separated list within square brackets, like so:
+
+```
+pip install "junifer[bct,dev]"
+```
+
+* `bct` installs [bctpy](https://github.com/aestrivex/bctpy) to enable use of `onthefly` module.
+* `neurokit2` installs [neurokit2](https://github.com/neuropsychology/NeuroKit) to enable use of [complexity markers](https://juaml.github.io/junifer/main/api/markers.html#module-junifer.markers.complexity).
+* `all` includes all of the above.
+* `dev` installs packages needed for development.
+* `docs` installs packages needed for building documentation.
+
 ## Citation
 
 If you use `junifer` in a scientific publication, we would appreciate if you cite our work. Currently, we do not have a publication, so feel free to use the project's [Zenodo URL](https://doi.org/10.5281/zenodo.8176569).
 
 ## Funding
 
 We thank the [Helmholtz Imaging Platform](https://helmholtz-imaging.de/) and
```

### Comparing `junifer-0.0.4.dev90/junifer.egg-info/SOURCES.txt` & `junifer-0.0.5.dev11/junifer.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.md
 codecov.yml
 conda-env.yml
 ignore_words.txt
 pyproject.toml
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug-report.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/dataset-request.yml
 .github/ISSUE_TEMPLATE/documention-request.yml
 .github/ISSUE_TEMPLATE/feature-request.yml
 .github/ISSUE_TEMPLATE/marker-request.yml
@@ -52,33 +53,24 @@
 docs/api/preprocessing.rst
 docs/api/stats.rst
 docs/api/storage.rst
 docs/api/testing.rst
 docs/api/utils.rst
 docs/changes/contributors.inc
 docs/changes/newsfragments/.gitignore
-docs/changes/newsfragments/182.enh
-docs/changes/newsfragments/233.bugfix
-docs/changes/newsfragments/245.change
-docs/changes/newsfragments/245.feature
-docs/changes/newsfragments/247.doc
-docs/changes/newsfragments/248.change
-docs/changes/newsfragments/251.doc
-docs/changes/newsfragments/253.misc
-docs/changes/newsfragments/254.feature
-docs/changes/newsfragments/258.enh
-docs/changes/newsfragments/259.enh
-docs/changes/newsfragments/261.misc
+docs/changes/newsfragments/273.feature
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
+docs/extending/dependencies.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
 docs/extending/masks.rst
 docs/extending/parcellations.rst
+docs/extending/preprocessor.rst
 docs/images/junifer_logo.png
 docs/sphinxext/gh_substitutions.py
 docs/understanding/data.rst
 docs/understanding/datagrabber.rst
 docs/understanding/datareader.rst
 docs/understanding/index.rst
 docs/understanding/marker.rst
@@ -96,14 +88,15 @@
 examples/run_compute_parcel_mean.py
 examples/run_datagrabber_bids_datalad.py
 examples/run_ets_rss_marker.py
 examples/run_junifer_julearn.py
 examples/run_run_gmd_mean.py
 examples/yamls/gmd_mean.yaml
 examples/yamls/gmd_mean_htcondor.yaml
+examples/yamls/partly_cloudy_agg_mean_tian.yml
 examples/yamls/ukb_gmd_mean.yaml
 junifer/__init__.py
 junifer/_version.py
 junifer/stats.py
 junifer.egg-info/PKG-INFO
 junifer.egg-info/SOURCES.txt
 junifer.egg-info/dependency_links.txt
@@ -112,26 +105,45 @@
 junifer.egg-info/top_level.txt
 junifer/api/__init__.py
 junifer/api/cli.py
 junifer/api/decorators.py
 junifer/api/functions.py
 junifer/api/parser.py
 junifer/api/utils.py
-junifer/api/res/run_conda.sh
+junifer/api/queue_context/__init__.py
+junifer/api/queue_context/gnu_parallel_local_adapter.py
+junifer/api/queue_context/htcondor_adapter.py
+junifer/api/queue_context/queue_context_adapter.py
+junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+junifer/api/queue_context/tests/test_htcondor_adapter.py
+junifer/api/res/run_conda.bash
+junifer/api/res/run_conda.zsh
+junifer/api/res/run_venv.bash
+junifer/api/res/run_venv.zsh
 junifer/api/res/afni/3dAFNItoNIFTI
 junifer/api/res/afni/3dRSFC
 junifer/api/res/afni/3dReHo
 junifer/api/res/afni/afni
 junifer/api/res/afni/run_afni_docker.sh
+junifer/api/res/ants/ResampleImage
+junifer/api/res/ants/antsApplyTransforms
+junifer/api/res/ants/antsApplyTransformsToPoints
+junifer/api/res/ants/run_ants_docker.sh
+junifer/api/res/fsl/applywarp
+junifer/api/res/fsl/flirt
+junifer/api/res/fsl/img2imgcoord
+junifer/api/res/fsl/run_fsl_docker.sh
+junifer/api/res/fsl/std2imgcoord
 junifer/api/tests/test_api_utils.py
 junifer/api/tests/test_cli.py
 junifer/api/tests/test_functions.py
 junifer/api/tests/test_parser.py
 junifer/api/tests/data/gmd_mean.yaml
 junifer/api/tests/data/gmd_mean_htcondor.yaml
+junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
 junifer/configs/__init__.py
 junifer/configs/juseless/__init__.py
 junifer/configs/juseless/datagrabbers/__init__.py
 junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
 junifer/configs/juseless/datagrabbers/camcan_vbm.py
 junifer/configs/juseless/datagrabbers/ixi_vbm.py
 junifer/configs/juseless/datagrabbers/ucla.py
@@ -141,15 +153,17 @@
 junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
 junifer/configs/juseless/datagrabbers/tests/test_ucla.py
 junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
 junifer/data/__init__.py
 junifer/data/coordinates.py
 junifer/data/masks.py
 junifer/data/parcellations.py
+junifer/data/template_spaces.py
 junifer/data/utils.py
+junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
 junifer/data/VOIs/meta/CogAC_VOIs.txt
 junifer/data/VOIs/meta/CogAR_VOIs.txt
 junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
 junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
 junifer/data/VOIs/meta/Empathy_VOIs.txt
 junifer/data/VOIs/meta/Motor_VOIs.txt
 junifer/data/VOIs/meta/MultiTask_VOIs.txt
@@ -167,17 +181,19 @@
 junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
 junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
 junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
 junifer/data/tests/test_coordinates.py
 junifer/data/tests/test_data_utils.py
 junifer/data/tests/test_masks.py
 junifer/data/tests/test_parcellations.py
+junifer/data/tests/test_template_spaces.py
 junifer/datagrabber/__init__.py
 junifer/datagrabber/base.py
 junifer/datagrabber/datalad_base.py
+junifer/datagrabber/dmcc13_benchmark.py
 junifer/datagrabber/multiple.py
 junifer/datagrabber/pattern.py
 junifer/datagrabber/pattern_datalad.py
 junifer/datagrabber/utils.py
 junifer/datagrabber/aomic/__init__.py
 junifer/datagrabber/aomic/id1000.py
 junifer/datagrabber/aomic/piop1.py
@@ -188,14 +204,15 @@
 junifer/datagrabber/hcp1200/__init__.py
 junifer/datagrabber/hcp1200/datalad_hcp1200.py
 junifer/datagrabber/hcp1200/hcp1200.py
 junifer/datagrabber/hcp1200/tests/test_hcp1200.py
 junifer/datagrabber/tests/test_base.py
 junifer/datagrabber/tests/test_datagrabber_utils.py
 junifer/datagrabber/tests/test_datalad_base.py
+junifer/datagrabber/tests/test_dmcc13_benchmark.py
 junifer/datagrabber/tests/test_multiple.py
 junifer/datagrabber/tests/test_pattern.py
 junifer/datagrabber/tests/test_pattern_datalad.py
 junifer/datareader/__init__.py
 junifer/datareader/default.py
 junifer/datareader/tests/test_default_reader.py
 junifer/external/__init__.py
@@ -210,20 +227,37 @@
 junifer/markers/__init__.py
 junifer/markers/base.py
 junifer/markers/collection.py
 junifer/markers/ets_rss.py
 junifer/markers/parcel_aggregation.py
 junifer/markers/sphere_aggregation.py
 junifer/markers/utils.py
+junifer/markers/complexity/__init__.py
+junifer/markers/complexity/complexity_base.py
+junifer/markers/complexity/hurst_exponent.py
+junifer/markers/complexity/multiscale_entropy_auc.py
+junifer/markers/complexity/perm_entropy.py
+junifer/markers/complexity/range_entropy.py
+junifer/markers/complexity/range_entropy_auc.py
+junifer/markers/complexity/sample_entropy.py
+junifer/markers/complexity/weighted_perm_entropy.py
+junifer/markers/complexity/tests/test_complexity_base.py
+junifer/markers/complexity/tests/test_hurst_exponent.py
+junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+junifer/markers/complexity/tests/test_perm_entropy.py
+junifer/markers/complexity/tests/test_range_entropy.py
+junifer/markers/complexity/tests/test_range_entropy_auc.py
+junifer/markers/complexity/tests/test_sample_entropy.py
+junifer/markers/complexity/tests/test_weighted_perm_entropy.py
 junifer/markers/falff/__init__.py
+junifer/markers/falff/_afni_falff.py
+junifer/markers/falff/_junifer_falff.py
 junifer/markers/falff/falff_base.py
-junifer/markers/falff/falff_estimator.py
 junifer/markers/falff/falff_parcels.py
 junifer/markers/falff/falff_spheres.py
-junifer/markers/falff/tests/test_falff_estimator.py
 junifer/markers/falff/tests/test_falff_parcels.py
 junifer/markers/falff/tests/test_falff_spheres.py
 junifer/markers/functional_connectivity/__init__.py
 junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
 junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
 junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
 junifer/markers/functional_connectivity/functional_connectivity_base.py
@@ -232,19 +266,19 @@
 junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
 junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
 junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
 junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
 junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
 junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
 junifer/markers/reho/__init__.py
+junifer/markers/reho/_afni_reho.py
+junifer/markers/reho/_junifer_reho.py
 junifer/markers/reho/reho_base.py
-junifer/markers/reho/reho_estimator.py
 junifer/markers/reho/reho_parcels.py
 junifer/markers/reho/reho_spheres.py
-junifer/markers/reho/tests/test_reho_estimator.py
 junifer/markers/reho/tests/test_reho_parcels.py
 junifer/markers/reho/tests/test_reho_spheres.py
 junifer/markers/temporal_snr/__init__.py
 junifer/markers/temporal_snr/temporal_snr_base.py
 junifer/markers/temporal_snr/temporal_snr_parcels.py
 junifer/markers/temporal_snr/temporal_snr_spheres.py
 junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
@@ -268,18 +302,31 @@
 junifer/pipeline/workdir_manager.py
 junifer/pipeline/tests/test_pipeline_step_mixin.py
 junifer/pipeline/tests/test_registry.py
 junifer/pipeline/tests/test_update_meta_mixin.py
 junifer/pipeline/tests/test_workdir_manager.py
 junifer/preprocess/__init__.py
 junifer/preprocess/base.py
+junifer/preprocess/bold_warper.py
+junifer/preprocess/ants/__init__.py
+junifer/preprocess/ants/ants_apply_transforms_warper.py
+junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py
 junifer/preprocess/confounds/__init__.py
 junifer/preprocess/confounds/fmriprep_confound_remover.py
 junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+junifer/preprocess/fsl/__init__.py
+junifer/preprocess/fsl/apply_warper.py
+junifer/preprocess/fsl/tests/test_apply_warper.py
+junifer/preprocess/tests/test_bold_warper.py
 junifer/preprocess/tests/test_preprocess_base.py
+junifer/preprocess/warping/__init__.py
+junifer/preprocess/warping/_ants_warper.py
+junifer/preprocess/warping/_fsl_warper.py
+junifer/preprocess/warping/space_warper.py
+junifer/preprocess/warping/tests/test_space_warper.py
 junifer/storage/__init__.py
 junifer/storage/base.py
 junifer/storage/hdf5.py
 junifer/storage/pandas_base.py
 junifer/storage/sqlite.py
 junifer/storage/utils.py
 junifer/storage/tests/test_hdf5.py
@@ -296,16 +343,19 @@
 junifer/testing/tests/test_partlycloudytesting_datagrabber.py
 junifer/testing/tests/test_spmauditory_datagrabber.py
 junifer/testing/tests/test_testing_registry.py
 junifer/tests/test_main.py
 junifer/tests/test_stats.py
 junifer/utils/__init__.py
 junifer/utils/fs.py
+junifer/utils/helpers.py
 junifer/utils/logging.py
 junifer/utils/tests/test_fs.py
+junifer/utils/tests/test_helpers.py
 junifer/utils/tests/test_logging.py
 tools/create_aomic1000_example_dataset.py
 tools/create_aomicpiop1_example_dataset.py
 tools/create_aomicpiop2_example_dataset.py
 tools/create_bids_example_dataset.py
 tools/create_bids_example_dataset_sessions.py
+tools/create_dmcc13_benchmark_example_dataset.py
 tools/create_hcp1200_example_dataset.py
```

### Comparing `junifer-0.0.4.dev90/pyproject.toml` & `junifer-0.0.5.dev11/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 [build-system]
-requires = [
-  "setuptools >= 61.0.0",
-  "wheel",
-  "setuptools_scm[toml] >= 6.2"
-]
+requires = ["setuptools>=64", "setuptools_scm>=8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "junifer"
 description = "JUelich NeuroImaging FEature extractoR"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -33,51 +29,66 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "click>=8.1.3,<8.2",
     "numpy>=1.24,<1.27",
+    "scipy>=1.9.0,<=1.11.4",
     "datalad>=0.15.4,<0.20",
     "pandas>=1.4.0,<2.2",
     "nibabel>=3.2.0,<5.11",
-    "nilearn>=0.9.0,<=0.11.0",
-    "sqlalchemy>=1.4.27,<= 2.1.0",
+    "nilearn>=0.9.0,<=0.10.2",
+    "sqlalchemy>=1.4.27,<=2.1.0",
     "ruamel.yaml>=0.17,<0.18",
-    "importlib_metadata; python_version < '3.10'",
-    "h5py>=3.8.0,<3.10",
+    "h5py>=3.10",
+    "httpx[http2]==0.26.0",
+    "tqdm==4.66.1",
+    "templateflow>=23.0.0",
+    "importlib_metadata; python_version<'3.10'",
+    "looseversion==1.3.0; python_version>='3.12'",
 ]
 dynamic = ["version"]
 
 [project.urls]
-homepage = "https://juaml.github.io/junifer"
-documentation = "https://juaml.github.io/junifer"
-repository = "https://github.com/juaml/junifer"
+Changelog = "https://juaml.github.io/junifer/main/whats_new.html"
+Documentation = "https://juaml.github.io/junifer"
+Homepage = "https://juaml.github.io/junifer"
+Source = "https://github.com/juaml/junifer"
 
 [project.scripts]
 junifer = "junifer.api.cli:cli"
 
 [project.optional-dependencies]
+all = [
+    "bctpy==0.6.0",
+    "neurokit2>=0.1.7",
+]
+bct = ["bctpy==0.6.0"]
+onthefly = [
+    "bctpy==0.6.0"
+]
+neurokit2 = ["neurokit2>=0.1.7"]
 dev = ["tox", "pre-commit"]
 docs = [
     "seaborn>=0.11.2,<0.13",
     "sphinx>=5.3.0,<7.3",
     "sphinx-gallery>=0.11.0,<0.15.0",
     "furo>=2022.9.29,<2023.10.0",
     "numpydoc>=1.5.0,<1.6",
     "julearn>=0.3.0,<0.4",
     "sphinx-copybutton>=0.5.1,<0.5.3",
     "towncrier>=22.12.0,<23.7",
     "sphinxcontrib-mermaid>=0.8.1,<0.10",
 ]
-onthefly = ["bctpy==0.6.0"]
 
 ################
 # Tool configs #
 ################
 
 [tool.setuptools]
 packages = ["junifer", "junifer.external.h5io.h5io"]
@@ -85,15 +96,15 @@
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "no-local-version"
 write_to = "junifer/_version.py"
 
 [tool.black]
 line-length = 79
-target-version = ["py38", "py39", "py310", "py311"]
+target-version = ["py38", "py39", "py310", "py311", "py312"]
 extend-exclude = """
 (
   junifer/external/h5io
 )
 """
 
 [tool.codespell]
@@ -141,15 +152,15 @@
 extend-exclude = [
     "__init__.py",
     "junifer/external/h5io",
     "docs",
     "examples",
     "tools",
 ]
-extend-ignore = [
+ignore = [
     # Use of `functools.lru_cache` or `functools.cache` on methods can lead to
     # memory leaks. The cache may retain instance references, preventing garbage
     # collection.
     "B019",
     # abstract class with no abstract methods
     "B024",
     "D202",
@@ -169,20 +180,27 @@
 
 [tool.ruff.isort]
 lines-after-imports = 2
 known-first-party = ["junifer"]
 known-third-party =[
     "click",
     "numpy",
+    "scipy",
     "datalad",
     "pandas",
     "nibabel",
     "nilearn",
     "sqlalchemy",
     "yaml",
+    "importlib_metadata",
+    "httpx",
+    "tqdm",
+    "templateflow",
+    "bct",
+    "neurokit2",
     "pytest",
 ]
 
 [tool.ruff.mccabe]
 max-complexity = 20
 
 [tool.pytest.ini_options]
@@ -211,15 +229,15 @@
 showcontent = true
 
 [tool.towncrier.fragment.feature]
 name = "Features"
 showcontent = true
 
 [tool.towncrier.fragment.misc]
-name = "Misc"
+name = "Miscellaneous"
 showcontent = true
 
 [tool.towncrier.fragment.removal]
 name = "Deprecations and Removals"
 showcontent = true
 
 # Add custom towncrier fragment for enhancements
```

### Comparing `junifer-0.0.4.dev90/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.5.dev11/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.5.dev11/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.5.dev11/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/tools/create_bids_example_dataset.py` & `junifer-0.0.5.dev11/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.5.dev11/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.4.dev90/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.5.dev11/tools/create_hcp1200_example_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 """Script to generate example dataset for HCP1200."""
 
 # Authors: Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 from itertools import product
-from tempfile import TemporaryDirectory
 from pathlib import Path
+from tempfile import TemporaryDirectory
 
 import datalad.api as dl
 
 
 # Set destination URL
 DST = "git@gin.g-node.org:/juaml/datalad-example-hcp1200.git"
 
 
 if __name__ == "__main__":
-
     with TemporaryDirectory() as tmpdir:
         # Convert str to Path
         tmpdir_path = Path(tmpdir)
         # Set base directory
         basedir = tmpdir_path / "example_hcp1200"
         # Create new datalad dataset
         dataset = dl.create(path=str(basedir.absolute()))  # type: ignore
         # Generate subject directories
         for sub in range(1, 10):
             subdir = basedir / f"sub-{sub:02d}"
             # Create subject directory
             subdir.mkdir()
 
-            for (task, phase_encoding) in product(
+            # T1w data
+            # Set subject data directory
+            sub_t1w_datadir = subdir / "T1w"
+            # Create subject data directory
+            sub_t1w_datadir.mkdir(parents=True)
+            # Set subject data file
+            sub_t1w_datafile = sub_t1w_datadir / "T1w_acpc_dc_restore.nii.gz"
+            # Write subject data file
+            with open(sub_t1w_datafile, "w") as f:
+                f.write("placeholder")
+
+            # Warp data
+            # Set subject data directory
+            sub_warp_datadir = subdir / "MNINonLinear" / "xfms"
+            # Create subject data directory
+            sub_warp_datadir.mkdir(parents=True)
+            # Set subject data file
+            sub_warp_datafile = sub_warp_datadir / "standard2acpc_dc.nii.gz"
+            # Write subject data file
+            with open(sub_warp_datafile, "w") as f:
+                f.write("placeholder")
+
+            # BOLD data
+            for task, phase_encoding in product(
                 [
                     "REST1",
                     "REST2",
                     "SOCIAL",
                     "WM",
                     "RELATIONAL",
                     "EMOTION",
@@ -45,40 +67,39 @@
             ):
                 # Proper formatting of task name
                 if "REST" in task:
                     new_task = f"rfMRI_{task}"
                 else:
                     new_task = f"tfMRI_{task}"
                 # Set subject data directory
-                sub_datadir = (
+                sub_bold_datadir = (
                     subdir
                     / "MNINonLinear"
                     / "Results"
                     / f"{new_task}_{phase_encoding}"
                 )
                 # Create subject data directory
-                sub_datadir.mkdir(parents=True)
+                sub_bold_datadir.mkdir(parents=True)
 
                 # Set subject data file
-                sub_datafile = (
-                    sub_datadir
-                    / f"{new_task}_{phase_encoding}.nii.gz"
+                sub_bold_datafile = (
+                    sub_bold_datadir / f"{new_task}_{phase_encoding}.nii.gz"
                 )
                 # Create subject data file
-                with open(sub_datafile, "w") as f:
+                with open(sub_bold_datafile, "w") as f:
                     f.write("placeholder")
 
                 if "REST" in task:
                     # Set subject data file with ICA+FIX
-                    sub_datafile = (
-                        sub_datadir
+                    sub_bold_datafile = (
+                        sub_bold_datadir
                         / f"{new_task}_{phase_encoding}_hp2000_clean.nii.gz"
                     )
                     # Create subject data file with ICA+FIX
-                    with open(sub_datafile, "w") as f:
+                    with open(sub_bold_datafile, "w") as f:
                         f.write("placeholder")
 
         # Save datalad dataset
         dataset.save(recursive=True)
         # Add datalad sibling
         dataset.siblings(action="add", name="gin", url=DST)
         # Push dataset to sibling
```

### Comparing `junifer-0.0.4.dev90/tox.ini` & `junifer-0.0.5.dev11/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tox]
-envlist = ruff, black, test, coverage, codespell, py3{8,9,10,11}
+envlist = ruff, black, test, coverage, codespell, py3{8,9,10,11,12}
 isolated_build = true
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
-    3.10: coverage
-    3.11: py311
+    3.10: py310
+    3.11: coverage
+    3.12: py312
 
 [testenv]
 skip_install = false
 # Required for git-annex
 passenv =
     HOME
 deps =
@@ -42,14 +43,15 @@
 commands =
     pytest
 
 [testenv:coverage]
 skip_install = false
 deps =
     bctpy==0.6.0
+    neurokit2>=0.1.7
     pytest
     pytest-cov
 commands =
     pytest --cov={envsitepackagesdir}/junifer --cov-report=xml --cov-report=term
 
 [testenv:codespell]
 skip_install = true
```

