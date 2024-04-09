# Comparing `tmp/pygsdata-0.1.0.tar.gz` & `tmp/pygsdata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygsdata-0.1.0.tar", last modified: Fri Feb  9 12:14:47 2024, max compression
+gzip compressed data, was "pygsdata-0.2.0.tar", last modified: Tue Apr  9 13:23:48 2024, max compression
```

## Comparing `pygsdata-0.1.0.tar` & `pygsdata-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.648941 pygsdata-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/release-draft.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-09 12:14:26.000000 pygsdata-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-02-09 12:14:26.000000 pygsdata-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-09 12:14:26.000000 pygsdata-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-09 12:14:26.000000 pygsdata-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-09 12:14:47.648941 pygsdata-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-09 12:14:26.000000 pygsdata-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/codeofconduct.md
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/docs/faqs/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/faqs/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.644941 pygsdata-0.1.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-09 12:14:26.000000 pygsdata-0.1.0/docs/workflow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-09 12:14:26.000000 pygsdata-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 12:14:47.648941 pygsdata-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.640941 pygsdata-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.648941 pygsdata-0.1.0/src/pygsdata/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    27350 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/gsdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/gsflag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-02-09 12:14:26.000000 pygsdata-0.1.0/src/pygsdata/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.648941 pygsdata-0.1.0/src/pygsdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-09 12:14:47.000000 pygsdata-0.1.0/src/pygsdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-09 12:14:47.000000 pygsdata-0.1.0/src/pygsdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 12:14:47.000000 pygsdata-0.1.0/src/pygsdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-09 12:14:47.000000 pygsdata-0.1.0/src/pygsdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-09 12:14:47.000000 pygsdata-0.1.0/src/pygsdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 12:14:47.648941 pygsdata-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-02-09 12:14:26.000000 pygsdata-0.1.0/tests/mock_gsdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-02-09 12:14:26.000000 pygsdata-0.1.0/tests/test_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-02-09 12:14:26.000000 pygsdata-0.1.0/tests/test_gsdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.597834 pygsdata-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.585834 pygsdata-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.585834 pygsdata-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-09 13:23:41.000000 pygsdata-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-09 13:23:41.000000 pygsdata-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-09 13:23:41.000000 pygsdata-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 13:23:41.000000 pygsdata-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 13:23:48.597834 pygsdata-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-09 13:23:41.000000 pygsdata-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.589834 pygsdata-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.589834 pygsdata-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/codeofconduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.589834 pygsdata-0.2.0/docs/faqs/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/faqs/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.589834 pygsdata-0.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-09 13:23:41.000000 pygsdata-0.2.0/docs/workflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-09 13:23:41.000000 pygsdata-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:23:48.597834 pygsdata-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.581834 pygsdata-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.593834 pygsdata-0.2.0/src/pygsdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24684 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/gsdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/gsflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/telescope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-09 13:23:41.000000 pygsdata-0.2.0/src/pygsdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.593834 pygsdata-0.2.0/src/pygsdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-09 13:23:48.000000 pygsdata-0.2.0/src/pygsdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-09 13:23:48.000000 pygsdata-0.2.0/src/pygsdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:23:48.000000 pygsdata-0.2.0/src/pygsdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 13:23:48.000000 pygsdata-0.2.0/src/pygsdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 13:23:48.000000 pygsdata-0.2.0/src/pygsdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:23:48.593834 pygsdata-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/mock_gsdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_gsdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_gsflag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_gsh5_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_telescope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 13:23:41.000000 pygsdata-0.2.0/tests/test_utils.py
```

### Comparing `pygsdata-0.1.0/.coveragerc` & `pygsdata-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/.github/labels.yml` & `pygsdata-0.2.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/.github/release-drafter.yml` & `pygsdata-0.2.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/.github/workflows/check-build.yml` & `pygsdata-0.2.0/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/.github/workflows/deploy.yaml` & `pygsdata-0.2.0/.github/workflows/deploy.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
         run: pip install build
 
       - name: Build a binary wheel
         run: |
           python -m build -s .
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.12
```

### Comparing `pygsdata-0.1.0/.github/workflows/test_suite.yaml` & `pygsdata-0.2.0/.github/workflows/test_suite.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -70,31 +70,28 @@
 
       - name: Get downstream package
         run: |
           cd ..
           git clone https://github.com/edges-collab/${{ matrix.package }}
           cd ${{ matrix.package }}
           pip install .[dev]
-      # - name: Install ipykernel
-      #   if: matrix.package == 'edges-cal'
-      #   run: python -m ipykernel install --user --name edges --display-name "edges"
 
       - name: Run Tests
         run: |
           coverage run --parallel-mode -m pytest ../${{ matrix.package}}
 
       - name: Upload coverage data
         uses: actions/upload-artifact@v4
         with:
           name: coverage-data-downstream-${{ matrix.package }}
           path: ".coverage.*"
           if-no-files-found: error
 
   codecov:
-    needs: [downstream, tests]
+    needs: [tests]
     name: Codecov Reporting
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
       - name: Download coverage data.
         uses: actions/download-artifact@v4
@@ -117,7 +114,9 @@
           coverage xml
 
       - uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           verbose: true
           file: ./coverage.xml
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `pygsdata-0.1.0/.pre-commit-config.yaml` & `pygsdata-0.2.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,20 @@
   - id: mixed-line-ending
     args: ['--fix=no']
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
   rev: v0.1.4
   hooks:
-    # Run the formatter.
-    - id: ruff-format
-
     # Run the linter.
     - id: ruff
+      args: [--fix]
+
+    # Run the formatter.
+    - id: ruff-format
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
```

### Comparing `pygsdata-0.1.0/CODE_OF_CONDUCT.md` & `pygsdata-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/CONTRIBUTING.md` & `pygsdata-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/LICENSE` & `pygsdata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/PKG-INFO` & `pygsdata-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygsdata
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python interface for 21cm Global Signal Data.
 Author-email: Steven Murray <steven.murray@sns.it>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -18,25 +18,25 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: attrs
 Requires-Dist: matplotlib
 Requires-Dist: hickleable
-Requires-Dist: read_acq
 Requires-Dist: h5py
 Requires-Dist: typing_extensions
 Requires-Dist: pytz
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pygsdata[docs,tests]; extra == "dev"
 
 # pygsdata
```

### Comparing `pygsdata-0.1.0/README.md` & `pygsdata-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/docs/Makefile` & `pygsdata-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/docs/conf.py` & `pygsdata-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/docs/usage.md` & `pygsdata-0.2.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/docs/workflow.yaml` & `pygsdata-0.2.0/docs/workflow.yaml`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/pyproject.toml` & `pygsdata-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,30 +28,30 @@
 dependencies = [
     "numpy",
     "scipy",
     "astropy",
     "attrs",
     "matplotlib",
     "hickleable",
-    "read_acq",
     "h5py",
     "typing_extensions",
     "pytz",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 docs = [
     "sphinx",
     "furo",
     "myst-parser"
 ]
 tests = [
     "pytest",
-    "pytest-cov"
+    "pytest-cov",
+    "pytest-xdist",
 ]
 dev = [
     "pre-commit",
     "ruff",
     "pygsdata[docs,tests]"
 ]
 
@@ -84,14 +84,16 @@
   "NPY",  # numpy-specific rules
   "PERF", # performance
   # "FURB", # refurb
   "RUF",  # ruff-specific rules
 ]
 ignore = [
     "DTZ007",   # use %z in strptime
+    "A003",     # class attribute shadows python builtin
+    "B008",     # function call in argument defaults
 ]
 [tool.ruff.lint.per-file-ignores]
 "tests/*.py" = [
     "D103",  # ignore missing docstring in tests
     "DTZ",   # ignore datetime in tests
     "T",     # print statements
 ]
@@ -103,14 +105,14 @@
 [tool.ruff.lint.pydocstyle]
 convention = 'numpy'
 
 [tool.ruff.lint.mccabe]
 max-complexity = 15
 
 [tool.pytest.ini_options]
-addopts = "--verbose --durations=25"
+addopts = "--verbose --durations=10"
 norecursedirs = [
     "dist",
     "build",
     ".tox",
 ]
 testpaths = "tests"
```

### Comparing `pygsdata-0.1.0/src/pygsdata/attrs.py` & `pygsdata-0.2.0/src/pygsdata/attrs.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
 def shape_validator(shape: tuple[int | None, ...]):
     """Validate that an array has a given shape."""
     if isinstance(shape, int):
         shape = (shape,)
 
     def validator(inst, att, value):
+        if len(shape) != len(value.shape):
+            raise ValueError(f"{att.name} must have shape {shape}, got {value.shape}")
+
         for i, (d0, d1) in enumerate(zip(shape, value.shape)):
             if d0 is not None and d0 != d1:
                 raise ValueError(
                     f"Axis {i} of {att.name} must have size {d0}, got {d1}"
                 )
 
     return validator
@@ -85,15 +88,15 @@
 
 def _cmp_num_array(x, y):
     if x is None and y is None:
         return True
     elif x is None or y is None:
         return False
     else:
-        return x.shape == y.shape and np.allclose(x, y)
+        return (x.shape == y.shape or x.size == 1 or y.size == 1) and np.allclose(x, y)
 
 
 def npfield(
     dtype=None,
     possible_ndims: tuple[int] | None = None,
     shape: tuple[int | None] | None = None,
     unit: un.Unit | None | str = None,
@@ -124,44 +127,83 @@
     if validator:
         if required:
             kwargs["validator"] = validator
         else:
             kwargs["validator"] = attrs.validators.optional(validator)
 
     return field(
-        eq=cmp_using(_cmp_bool_array if dtype == bool else _cmp_num_array),
+        eq=cmp_using(_cmp_bool_array if dtype is bool else _cmp_num_array),
         converter=array_converter(dtype=dtype, allow_none=not required),
         **kwargs,
     )
 
 
-def timefield(
+def _astropy_subclass_field(
+    cls,
+    defining_attr,
     possible_ndims: tuple[int] | None = None,
     shape: tuple[int] | None = None,
     validator=None,
     **kwargs,
 ):
-    """Construct an attrs field for an astropy Time."""
-
     def cmp(x, y):
-        if isinstance(x, Time) and isinstance(y, Time):
-            return x.shape == y.shape and np.allclose(x.jd, y.jd)
-        elif isinstance(x, Longitude) and isinstance(y, Longitude):
-            return x.shape == y.shape and np.allclose(x.deg, y.deg)
-        else:
-            return False
+        return x.shape == y.shape and np.allclose(
+            getattr(x, defining_attr), getattr(y, defining_attr), rtol=0, atol=1e-8
+        )
 
     if validator is None:
-        validator = []
+        validator = [attrs.validators.instance_of(cls)]
     elif callable(validator):
-        validator = [validator]
+        validator = [validator, attrs.validators.instance_of(cls)]
 
     if possible_ndims is not None:
         validator.append(ndim_validator(possible_ndims))
 
     if shape is not None:
         validator.append(shape_validator(shape))
 
-    if validator:
-        kwargs["validator"] = validator
+    kwargs["validator"] = validator
 
     return field(eq=cmp_using(cmp), **kwargs)
+
+
+def timefield(
+    possible_ndims: tuple[int] | None = None,
+    shape: tuple[int] | None = None,
+    validator=None,
+    **kwargs,
+):
+    """Construct an attrs field for an astropy Time."""
+    return _astropy_subclass_field(
+        Time, "jd", possible_ndims, shape, validator, **kwargs
+    )
+
+
+def lstfield(
+    possible_ndims: tuple[int] | None = None,
+    shape: tuple[int] | None = None,
+    validator=None,
+    **kwargs,
+):
+    """Construct an attrs field for an astropy Time."""
+    return _astropy_subclass_field(
+        Longitude, "rad", possible_ndims, shape, validator, **kwargs
+    )
+
+
+def cmp_qtable(x, y):
+    """Compare two QTable objects."""
+    if x is None and y is None:
+        return True
+    elif x is None or y is None:
+        return False
+    else:
+        if type(x) != type(y):
+            return False
+        if x.columns.keys() != y.columns.keys():
+            return False
+
+        for key in x.columns:
+            if not np.all(x[key] == y[key]):
+                return False
+
+    return True
```

### Comparing `pygsdata-0.1.0/src/pygsdata/gsflag.py` & `pygsdata-0.2.0/src/pygsdata/gsflag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """An object to hold flag information."""
 
 from __future__ import annotations
 
+from collections.abc import Sequence
 from functools import cached_property
 from pathlib import Path
 from typing import Protocol
 
 import hickle
 import numpy as np
 from attrs import converters as cnv
@@ -38,15 +39,15 @@
     ----------
     flags
         The flags as a boolean array. The array may have up to 4 dimensions -- load,
         pol, time, and freq -- but need not have all of the dimensions.
     axes
         A tuple of strings specifying the axes of the data array. The possible axes are
         "load", "pol", "time", and "freq". They must be in that order, but not all
-        must be present.
+        must be present, only as many as flags has dimensions.
     history
         A tuple of dictionaries, each of which is a record of a previous processing
         step.
     filename
         The filename from which the data was read (if any). Used for writing additional
         data if more is added (eg. flags, data model).
     """
@@ -63,24 +64,30 @@
     @flags.validator
     def _flags_vld(self, _, value):
         if value.ndim > 4:
             raise ValueError("Flag array must have at most 4 dimensions")
 
     @axes.validator
     def _axes_vld(self, _, value):
-        if not len(set(value)) == len(value):
+        if len(set(value)) != len(value):
             raise ValueError(f"Axes must be unique, got {value}")
 
-        if not all(ax in ("load", "pol", "time", "freq") for ax in value):
+        if len(value) != self.flags.ndim:
+            raise ValueError(
+                f"Number of axes must match number of dimensions in flags. "
+                f"Got {len(value)} axes and {self.flags.ndim} dimensions"
+            )
+
+        if any(ax not in self._axes for ax in value):
             raise ValueError("Axes must be a subset of load, pol, time, freq")
 
-        idx = [value.index(ax) for ax in ("load", "pol", "time", "freq") if ax in value]
+        idx = [value.index(ax) for ax in self._axes if ax in value]
 
-        if not idx == sorted(idx):
-            raise ValueError("Axes must be in order load, pol, time, freq")
+        if idx != sorted(idx):
+            raise ValueError(f"Axes must be in order {self._axes}")
 
     @axes.default
     def _axes_default(self):
         if self.flags.ndim == 4:
             return self._axes
         else:
             raise ValueError(
@@ -94,31 +101,27 @@
             return None
 
         return self.flags.shape[self.axes.index("freq")]
 
     @cached_property
     def nloads(self) -> int | None:
         """The number of loads."""
-        if "load" not in self.axes:
-            return None
-        return self.flags.shape[0]
+        return None if "load" not in self.axes else self.flags.shape[0]
 
     @property
     def ntimes(self) -> int | None:
         """The number of times."""
         if "time" not in self.axes:
             return None
         return self.flags.shape[self.axes.index("time")]
 
     @property
     def npols(self) -> int | None:
         """The number of polarizations."""
-        if "pol" not in self.axes:
-            return None
-        return self.flags.shape[self.axes.index("pol")]
+        return self.flags.shape[self.axes.index("pol")] if "pol" in self.axes else None
 
     @classmethod
     def from_file(cls, filename: str | Path, filetype: str | None = None, **kw) -> Self:
         """Create a GSFlag instance from a file.
 
         This method attempts to auto-detect the file type and read it.
         """
@@ -146,26 +149,15 @@
         return new.update(filename=filename)
 
     def update(self, **kwargs) -> Self:
         """Return a new GSFlag object with updated attributes."""
         # If the user passes a single dictionary as history, append it.
         # Otherwise raise an error, unless it's not passed at all.
         history = kwargs.pop("history", None)
-        if isinstance(history, Stamp):
-            history = self.history.add(history)
-        elif isinstance(history, dict):
-            history = self.history.add(Stamp(**history))
-        elif isinstance(history, History):
-            history = self.history
-        elif history is not None:
-            raise ValueError(
-                f"History must be a Stamp object or dictionary, got {history}"
-            )
-        else:
-            history = self.history
+        history = self.history if history is None else self.history.add(history)
 
         return evolve(self, history=history, **kwargs)
 
     @property
     def full_rank_flags(self) -> np.ndarray:
         """Return a full-rank flag array."""
         flg = self.flags.copy()
@@ -187,58 +179,56 @@
     def _check_compat(self, other: _GSDataSized) -> None:
         if (
             self.nloads is not None
             and other.nloads is not None
             and self.nloads != other.nloads
         ):
             raise ValueError(
-                "Cannot multiply GSFlag objects with different loads. Got "
-                f"{self.nloads} and {other.nloads}."
+                "Objects have different nloads. Got "
+                f"this={self.nloads} and that={other.nloads}."
             )
 
         if (
             self.npols is not None
             and other.npols is not None
             and self.npols != other.npols
         ):
             raise ValueError(
-                "Cannot multiply GSFlag objects with different polarizations. Got "
-                f"{self.npols} and {other.npols}"
+                "Objects have different npols. Got "
+                f"this={self.npols} and that={other.npols}"
             )
 
         if (
             self.ntimes is not None
             and other.ntimes is not None
             and self.ntimes != other.ntimes
         ):
             raise ValueError(
-                "Cannot multiply GSFlag objects with different times. Got "
-                f"{self.ntimes} and {other.ntimes}"
+                "Objects have different ntimes. Got "
+                f"this={self.ntimes} and that={other.ntimes}"
             )
 
         if (
             self.nfreqs is not None
             and other.nfreqs is not None
             and self.nfreqs != other.nfreqs
         ):
             raise ValueError(
-                "Cannot multiply GSFlag objects with different frequencies. Got "
-                f"{self.nfreqs} and {other.nfreqs}"
+                "Objects have different nfreqs. Got "
+                f"this={self.nfreqs} and that={other.nfreqs}"
             )
 
     def __or__(self, other: GSFlag) -> Self:
         """Take the product of two GSFlag objects and return a new one."""
         if not isinstance(other, GSFlag):
             raise TypeError("can only 'or' GSFlag objects")
 
         self._check_compat(other)
         new_flags = np.squeeze(self.full_rank_flags | other.full_rank_flags)
-        axes = tuple(
-            ax for ax in ("load", "pol", "time", "freq") if ax in self.axes + other.axes
-        )
+        axes = tuple(ax for ax in self._axes if ax in self.axes + other.axes)
 
         return self.update(
             flags=new_flags,
             axes=axes,
             history=self.history.add(other.history).add(
                 Stamp("Multiplied GSFlag objects")
             ),
@@ -248,30 +238,29 @@
     def __and__(self, other: GSFlag) -> Self:
         """Take the product of two GSFlag objects and return a new one."""
         if not isinstance(other, GSFlag):
             raise TypeError("can only 'and' GSFlag objects")
 
         self._check_compat(other)
         new_flags = np.squeeze(self.full_rank_flags & other.full_rank_flags)
-        axes = tuple(
-            ax for ax in ("load", "pol", "time", "freq") if ax in self.axes + other.axes
-        )
+
+        axes = tuple(ax for ax in self._axes if ax in self.axes + other.axes)
 
         return self.update(
             flags=new_flags,
             axes=axes,
             history=self.history.add(other.history).add(
                 Stamp("Multiplied GSFlag objects")
             ),
             filename=None,
         )
 
     def select(self, idx: np.ndarray | slice, axis: str, squeeze: bool = False) -> Self:
         """Select a subset of the data along the given axis."""
-        if axis not in ("load", "pol", "time", "freq"):
+        if axis not in self._axes:
             raise ValueError(f"Axis {axis} not recognized")
 
         if isinstance(idx, slice):
             idx = np.arange(*idx.indices(self.flags.shape[self.axes.index(axis)]))
         elif idx.dtype == bool:
             idx = np.where(idx)[0]
 
@@ -319,15 +308,41 @@
         else:
             axes = self.axes
 
         return self.update(
             flags=new_flags,
             axes=axes,
             history=self.history.add(
-                Stamp("Applied operation to data", axis=axis, op=op)
+                Stamp("Applied operation to data", parameters={"axis": axis, "op": op})
             ),
             filename=None,
         )
 
-    def any(self, axis: str | None = None) -> bool | Self:  # noqa: A003
+    def any(self, axis: str | None = None) -> bool | Self:
         """Return True if any of the flags are True."""
         return self.flags.any() if axis is None else self.op_on_axis(np.any, axis)
+
+    def all(self, axis: str | None = None) -> bool | Self:
+        """Return True if any of the flags are True."""
+        return self.flags.all() if axis is None else self.op_on_axis(np.all, axis)
+
+    def concat(self, others: GSFlag | Sequence[GSFlag], axis: str) -> GSFlag:
+        """Get a new GSFlag by concatenating other flags to this one."""
+        if isinstance(others, GSFlag):
+            others = [others]
+
+        if axis not in ("load", "pol", "time", "freq"):
+            raise ValueError(f"Axis {axis} not recognized")
+
+        if axis not in self.axes:
+            raise ValueError(f"Axis {axis} not present in this GSFlag object")
+
+        new_flags = np.concatenate(
+            [self.flags] + [o.flags for o in others], axis=self.axes.index(axis)
+        )
+        return self.update(
+            flags=new_flags,
+            history=self.history.add(
+                Stamp("Concatenated GSFlag objects", parameters={"axis": axis})
+            ),
+            filename=None,
+        )
```

### Comparing `pygsdata-0.1.0/src/pygsdata/history.py` & `pygsdata-0.2.0/src/pygsdata/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Classes for defining the history of a GSData / GSFlag object."""
 
 from __future__ import annotations
 
 import contextlib
 import datetime
+from importlib.metadata import PackageNotFoundError, version
 
 import yaml
 from attrs import asdict, define, evolve, field
 from attrs import validators as vld
 from hickleable import hickleable
-from pkg_resources import get_distribution
+
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
 
 @hickleable()
 @define(frozen=True, slots=False)
 class Stamp:
     """Class representing a historical record of a process applying to an object.
 
@@ -55,16 +60,16 @@
             "edges-io",
             "edges-analysis",
             "read_acq",
             "numpy",
             "astropy",
             "pygsdata",
         ):
-            with contextlib.suppress(Exception):
-                out[pkg] = get_distribution(__name__).version
+            with contextlib.suppress(PackageNotFoundError):
+                out[pkg] = version(pkg)
         return out
 
     def _to_yaml_dict(self):
         dct = asdict(self)
         dct["timestamp"] = dct["timestamp"].isoformat()
         return dct
 
@@ -105,17 +110,22 @@
         """Create a Stamp object from a string representation."""
         dct = yaml.load(repr_string, Loader=yaml.FullLoader)
         return cls.from_yaml_dict(dct)
 
     @classmethod
     def from_yaml_dict(cls, d: dict) -> Stamp:
         """Create a Stamp object from a dictionary representing a history record."""
-        d["timestamp"] = datetime.datetime.strptime(
-            d["timestamp"], "%Y-%m-%dT%H:%M:%S.%f"
-        )
+        try:
+            d["timestamp"] = datetime.datetime.strptime(
+                d["timestamp"], "%Y-%m-%dT%H:%M:%S.%f"
+            )
+        except ValueError:
+            d["timestamp"] = datetime.datetime.strptime(
+                d["timestamp"], "%Y-%m-%dT%H:%M:%S.%f%z"
+            )
         return cls(**d)
 
 
 @hickleable()
 @define(slots=False)
 class History:
     """A collection of Stamp objects defining the history."""
@@ -165,22 +175,29 @@
 
     @classmethod
     def from_repr(cls, repr_string: str):
         """Create a History object from a string representation."""
         d = yaml.load(repr_string, Loader=yaml.FullLoader)
         return cls(stamps=[Stamp.from_yaml_dict(s) for s in d])
 
-    def add(self, stamp: Stamp | dict):
+    def add(self, stamp: Stamp | dict | tuple[Stamp] | tuple[dict] | Self):
         """Add a stamp to the history."""
         if isinstance(stamp, dict):
-            stamp = Stamp(**stamp)
-        if not isinstance(stamp, Stamp):
-            raise TypeError("stamp must be a Stamp or a dictionary")
+            stamp = (Stamp(**stamp),)
+
+        if isinstance(stamp, Stamp):
+            return evolve(self, stamps=(*self.stamps, stamp))
+
+        if all(isinstance(s, (Stamp, dict)) for s in stamp):
+            a = self
+            for s in stamp:
+                a = a.add(s)
+            return a
 
-        return evolve(self, stamps=(*self.stamps, stamp))
+        raise TypeError("stamp must be a Stamp or a dictionary")
 
     def __len__(self):
         """Return the number of stamps."""
         return len(self.stamps)
 
     def __iter__(self):
         """Iterate over the stamps."""
```

### Comparing `pygsdata-0.1.0/src/pygsdata/plots.py` & `pygsdata-0.2.0/src/pygsdata/plots.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,51 +60,56 @@
             "the same shape as data."
         )
 
     q = np.where(data.get_flagged_nsamples(which_flags, ignore_flags) == 0, np.nan, q)
     q = q[load, pol, :, :]
 
     if ax is None:
-        ax = plt.subplots(1, 1)[1]
+        ax = plt.subplots(1, 1, layout="constrained")[1]
 
-    if attribute == "resids":
+    if attribute == "residuals":
         cmap = imshow_kwargs.pop("cmap", "coolwarm")
     else:
         cmap = imshow_kwargs.pop("cmap", "magma")
 
-    times = data.time_array
+    times = data.times
 
     img = ax.imshow(
         q,
         origin="lower",
         extent=(
-            data.freq_array.min().to_value("MHz"),
-            data.freq_array.max().to_value("MHz"),
-            0,
-            (
-                (times.max() - times.min()).hour
-                if data.in_lst
-                else (times.max() - times.min()).to_value("hour")
-            ),
+            data.freqs.min().to_value("MHz"),
+            data.freqs.max().to_value("MHz"),
+            times.jd.min(),
+            times.jd.max(),
         ),
         cmap=cmap,
         aspect="auto",
         interpolation="none",
         **imshow_kwargs,
     )
 
     if xlab:
         ax.set_xlabel("Frequency [MHz]")
     if ylab:
-        if data.in_lst:
-            ax.set_ylabel("LST")
-        else:
-            ax.set_ylabel("Hours into Observation")
-
-    if title and not isinstance(title, str) and not data.in_lst:
-        ax.set_title(f"{data.get_initial_yearday()}. LST0={data.lst_array[0][0]:.2f}")
-
-    if cbar:
-        cb = plt.colorbar(img, ax=ax)
-        cb.set_label(data.loads[load])
+        ax.set_ylabel("JD")
 
-    return ax
+    dlst = data.times.jd[0, 0] * 24.0 - data.lsts.hourangle[0, 0]
+
+    def jd2lst(jd):
+        return jd * 24 - dlst  # spl_jd2lst(jd) % 24
+
+    def lst2jd(lst):
+        return lst + dlst
+
+    v2 = ax.secondary_yaxis("right", functions=(jd2lst, lst2jd))
+    v2.set_ylabel("LST [hour]")
+    v2.yaxis.set_major_formatter(lambda x, pos: str(x % 24))
+
+    if title and not isinstance(title, str):
+        ax.set_title(f"{data.get_initial_yearday()}")
+    if title and isinstance(title, str):
+        ax.set_title(title)
+
+    cb = plt.colorbar(img, ax=ax, pad=0.1) if cbar else None
+
+    return ax, cb
```

### Comparing `pygsdata-0.1.0/src/pygsdata/register.py` & `pygsdata-0.2.0/src/pygsdata/register.py`

 * *Files identical despite different names*

### Comparing `pygsdata-0.1.0/src/pygsdata.egg-info/PKG-INFO` & `pygsdata-0.2.0/src/pygsdata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygsdata
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python interface for 21cm Global Signal Data.
 Author-email: Steven Murray <steven.murray@sns.it>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -18,25 +18,25 @@
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: astropy
 Requires-Dist: attrs
 Requires-Dist: matplotlib
 Requires-Dist: hickleable
-Requires-Dist: read_acq
 Requires-Dist: h5py
 Requires-Dist: typing_extensions
 Requires-Dist: pytz
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pygsdata[docs,tests]; extra == "dev"
 
 # pygsdata
```

### Comparing `pygsdata-0.1.0/tests/test_gsdata.py` & `pygsdata-0.2.0/tests/test_gsdata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,146 +1,56 @@
 """Tests of the GSData object."""
 
-from datetime import datetime, timedelta
+import pickle
+import re
+from datetime import timedelta
+from pathlib import Path
 
 import attrs
 import numpy as np
 import pytest
 from astropy import units as un
-from astropy.coordinates import EarthLocation
+from astropy.coordinates import Longitude
 from astropy.time import Time
 from pygsdata import (
     GSData,
     GSFlag,
-    History,
     Stamp,
-    gsregister,
     select_freqs,
     select_lsts,
     select_times,
 )
 
 
-@pytest.fixture(scope="module")
-def simple_gsdata():
-    return GSData(
-        data=np.zeros((1, 1, 50, 100)),
-        freq_array=np.linspace(50, 100, 100) * un.MHz,
-        time_array=Time(np.linspace(2459811, 2459812, 50)[:, np.newaxis], format="jd"),
-        telescope_location=EarthLocation(lat=0, lon=0),
-    )
-
-
-@pytest.fixture(scope="module")
-def power_gsdata():
-    return GSData(
-        data=np.zeros((3, 1, 50, 100)),
-        freq_array=np.linspace(50, 100, 100) * un.MHz,
-        time_array=Time(
-            np.array(
-                [
-                    np.linspace(2459811, 2459812, 50),
-                    np.linspace(2459811.001, 2459812.001, 50),
-                    np.linspace(2459811.002, 2459812.002, 50),
-                ]
-            ).T,
-            format="jd",
-        ),
-        telescope_location=EarthLocation(lat=0, lon=0),
-    )
-
-
 def test_default_power_load_names(power_gsdata):
     assert power_gsdata.loads == (
         "ant",
         "internal_load",
         "internal_load_plus_noise_source",
     )
 
 
-def test_bad_load_names():
+def test_bad_load_names(edges):
     with pytest.raises(ValueError, match="If data has more than one source"):
         GSData(
             data=np.zeros((2, 1, 50, 100)),
-            freq_array=np.linspace(50, 100, 100) * un.MHz,
-            time_array=Time(
+            freqs=np.linspace(50, 100, 100) * un.MHz,
+            times=Time(
                 np.array(
                     [
                         np.linspace(2459811, 2459812, 50),
                         np.linspace(2459811.001, 2459812.001, 50),
                     ]
                 ).T,
                 format="jd",
             ),
-            telescope_location=EarthLocation(lat=0, lon=0),
+            telescope=edges,
         )
 
 
-@gsregister("calibrate")
-def bad_gsfunc(data):
-    return 3
-
-
-def test_bad_gsfunc_return(simple_gsdata):
-    with pytest.raises(TypeError, match="bad_gsfunc returned <class 'int'>"):
-        bad_gsfunc(simple_gsdata)
-
-
-def test_bad_stamp_init():
-    with pytest.raises(
-        ValueError, match="History record must have a message or a function"
-    ):
-        Stamp()
-
-
-def test_str_and_pretty():
-    s = Stamp(message="dummy")
-    assert str(s) != s.pretty()
-
-
-def test_from_yaml_roundtrip():
-    s = Stamp(message="dummy", parameters={"a": 1, "b": "hey"})
-    xx = repr(s)
-
-    s2 = Stamp.from_repr(xx)
-
-    assert s2 == s
-
-
-def test_history():
-    history = History(
-        (
-            Stamp(message="hello"),
-            Stamp(function="a_function", parameters={"a": 1, "b": "hey"}),
-        )
-    )
-
-    assert len(history) == 2
-
-    history2 = history.add({"message": "hey", "versions": {"some_package": "1.2.3"}})
-    assert len(history2) == 3
-    assert str(history) != history.pretty()
-
-    # Ensure that we can index by int, str or datetime.
-    assert (
-        history[1]
-        == history[history[1].timestamp]
-        == history[history[1].timestamp.isoformat()]
-    )
-
-    with pytest.raises(KeyError):
-        history["not_a_key"]
-
-    with pytest.raises(KeyError):
-        history[datetime.now()]
-
-    with pytest.raises(KeyError):
-        history[(1, 2)]
-
-
 def test_bad_gsdata_init(simple_gsdata: GSData):
     with pytest.raises(ValueError, match="data must have ndim in"):
         simple_gsdata.update(data=np.zeros((3, 4, 5)))
 
     with pytest.raises(ValueError, match="nsamples must have the same shape as data"):
         simple_gsdata.update(nsamples=np.zeros((2, 1, 50, 100)))
 
@@ -153,76 +63,106 @@
                 1: GSFlag(
                     flags=np.zeros(simple_gsdata.data.shape, dtype=bool),
                     axes=("load", "pol", "time", "freq"),
                 )
             }
         )
 
-    with pytest.raises(TypeError, match="freq_array must be a Quantity"):
-        simple_gsdata.update(freq_array=np.linspace(50, 100, 100))
+    with pytest.raises(TypeError, match="freqs must be a Quantity"):
+        simple_gsdata.update(freqs=np.linspace(50, 100, 100))
 
-    with pytest.raises(
-        ValueError, match="freq_array must have units compatible with MHz"
-    ):
-        simple_gsdata.update(freq_array=np.linspace(50, 100, 100) * un.m)
+    with pytest.raises(ValueError, match="freqs must have units compatible with MHz"):
+        simple_gsdata.update(freqs=np.linspace(50, 100, 100) * un.m)
 
-    with pytest.raises(ValueError, match="freq_array must have the size nfreqs"):
-        simple_gsdata.update(freq_array=simple_gsdata.freq_array[:-1])
+    with pytest.raises(ValueError, match="freqs must have the size nfreqs"):
+        simple_gsdata.update(freqs=simple_gsdata.freqs[:-1])
 
-    with pytest.raises(ValueError, match="time_array must have ndim in "):
-        simple_gsdata.update(time_array=simple_gsdata.time_array[:, 0])
+    with pytest.raises(ValueError, match="times must have ndim in "):
+        simple_gsdata.update(times=simple_gsdata.times[:, 0])
 
     with pytest.raises(ValueError, match="loads must have the same length as"):
         simple_gsdata.update(loads=("ant", "another_one"))
 
     with pytest.raises(ValueError, match="loads must be a tuple of strings"):
         simple_gsdata.update(loads=(38,))
 
     with pytest.raises(
-        TypeError, match="effective_integration_time must be a Quantity"
+        ValueError,
+        match="auxiliary_measurements must be length ntimes",
+    ):
+        simple_gsdata.update(auxiliary_measurements={"hey": np.linspace(50, 100, 75)})
+
+    with pytest.raises(ValueError, match="data_unit must be one of"):
+        simple_gsdata.update(data_unit="my_custom_string")
+
+    with pytest.raises(TypeError, match="flags values must be GSFlag instances"):
+        simple_gsdata.update(
+            flags={"new": np.zeros(simple_gsdata.data.shape, dtype=bool)}
+        )
+
+    with pytest.raises(ValueError, match="residuals must have the same shape as data"):
+        simple_gsdata.update(residuals=np.zeros((2, 1, 50, 100)))
+
+    with pytest.raises(
+        ValueError, match=re.escape("times must have the size (ntimes, nloads)")
     ):
-        simple_gsdata.update(effective_integration_time=10.0)
+        simple_gsdata.update(times=simple_gsdata.times[:-1])
 
     with pytest.raises(
-        ValueError, match="effective_integration_time must be in seconds"
+        ValueError,
+        match=re.escape("time_ranges must have the size (ntimes, nloads, 2)"),
     ):
-        simple_gsdata.update(effective_integration_time=10.0 * un.MHz)
+        simple_gsdata.update(time_ranges=simple_gsdata.time_ranges[:-1])
 
-    with pytest.raises(TypeError, match="auxiliary_measurements must be a dictionary"):
-        simple_gsdata.update(auxiliary_measurements=3)
+    with pytest.raises(
+        ValueError, match=re.escape("time_ranges must all be greater than zero")
+    ):
+        simple_gsdata.update(time_ranges=simple_gsdata.time_ranges[..., ::-1])
 
     with pytest.raises(
         ValueError,
-        match="If times are LSTs, auxiliary_measurements cannot be specified",
+        match=re.escape("effective_integration_time must be greater than zero"),
     ):
-        simple_gsdata.update(
-            auxiliary_measurements={"hey": np.linspace(50, 100, 50)},
-            time_array=simple_gsdata.lst_array,
-        )
+        simple_gsdata.update(effective_integration_time=-1 * un.s)
 
-    with pytest.raises(TypeError, match="auxiliary_measurements keys must be strings"):
-        simple_gsdata.update(auxiliary_measurements={1: np.linspace(50, 100, 50)})
-
-    with pytest.raises(TypeError, match="auxiliary_measurements values must be arrays"):
-        simple_gsdata.update(auxiliary_measurements={"hey": 3})
+    with pytest.raises(
+        ValueError, match=re.escape("effective_integration_time must be a scalar")
+    ):
+        simple_gsdata.update(effective_integration_time=np.ones((50, 273, 3)) * un.s)
 
     with pytest.raises(
-        ValueError, match="auxiliary_measurements values must have the size ntimes"
+        ValueError, match=re.escape("lsts must have the size (ntimes, nloads)")
     ):
-        simple_gsdata.update(auxiliary_measurements={"hey": np.linspace(50, 100, 75)})
+        simple_gsdata.update(lsts=simple_gsdata.lsts[:-1])
 
-    with pytest.raises(ValueError, match="data_unit must be one of"):
-        simple_gsdata.update(data_unit="my_custom_string")
+    with pytest.raises(
+        ValueError, match=re.escape("lst_ranges must have the size (ntimes, nloads, 2)")
+    ):
+        simple_gsdata.update(lst_ranges=simple_gsdata.lst_ranges[:-1])
 
 
 def test_read_bad_filetype():
     with pytest.raises(ValueError, match="Unrecognized file type"):
         GSData.from_file("a_bad_file.txt")
 
 
+def test_aux_none_is_ok(simple_gsdata):
+    new = simple_gsdata.update(auxiliary_measurements=None)
+    assert new.auxiliary_measurements is None
+
+
+def test_effective_integration_time_array(simple_gsdata):
+    new = simple_gsdata.update(
+        effective_integration_time=simple_gsdata.effective_integration_time
+    )
+    assert np.all(
+        new.effective_integration_time == simple_gsdata.effective_integration_time
+    )
+
+
 def test_update_history(simple_gsdata):
     assert len(simple_gsdata.history) == 0
 
     new = simple_gsdata.update(data=simple_gsdata.data + 1)
     assert len(new.history) == 0
 
     new = new.update(history=Stamp(message="just tagging a point in time"))
@@ -234,82 +174,71 @@
     with pytest.raises(
         ValueError, match="History must be a Stamp object or dictionary"
     ):
         new.update(history="bad message")
 
 
 def test_select_lsts_and_times(power_gsdata):
-    indx = np.zeros(50, dtype=bool)
+    indx = np.zeros(power_gsdata.ntimes, dtype=bool)
     indx[::2] = True
 
     lst = select_lsts(power_gsdata, indx=indx)
     tm = select_times(power_gsdata, indx=indx)
 
     assert lst == tm
 
     stime = select_times(power_gsdata, time_range=(2459811.5, 2459811.7))
     assert stime != power_gsdata
 
 
 def test_select_lsts(power_gsdata: GSData):
-    rng = (power_gsdata.lst_array.min().hour, power_gsdata.lst_array.max().hour)
+    rng = (power_gsdata.lsts.min().hour, power_gsdata.lsts.max().hour)
 
     new = select_lsts(power_gsdata, lst_range=rng, load="all")
     # even though they're the same, the _file_appendable is switched off now
     assert new != power_gsdata
     assert np.allclose(new.data, power_gsdata.data)
 
     new = select_lsts(power_gsdata, lst_range=rng, load="ant")
     assert new != power_gsdata
-    assert np.allclose(new.data, power_gsdata.data[0])
+    assert np.allclose(new.data, power_gsdata.data)
 
     with pytest.raises(ValueError, match="range must be a length-2 tuple"):
         select_lsts(power_gsdata, lst_range=[0, 2, 3])
 
     # Use different order of range
     new = select_lsts(power_gsdata, lst_range=(-2, 4))
     new2 = select_lsts(power_gsdata, lst_range=(22, 4))
+
     assert new == new2
 
     # Test with both indx and range
     new = select_lsts(power_gsdata, lst_range=rng, indx=np.arange(0, 50, 2))
     new2 = select_lsts(power_gsdata, indx=np.arange(0, 50, 2))
 
-    flds = attrs.fields(GSData)
-    for fld in flds:
-        v1 = getattr(new, fld.name)
-        v2 = getattr(new2, fld.name)
-
-        if not fld.eq:
-            continue
-        if fld.eq_key is not None:
-            if fld.eq_key(v1) != fld.eq_key(v2):
-                print(fld)
-        elif v1 != v2:
-            print(fld)
     assert new == new2
 
 
 def test_select_freqs(simple_gsdata):
     new = select_freqs(simple_gsdata, freq_range=(50 * un.MHz, 70 * un.MHz))
-    assert new.freq_array.max() <= 70 * un.MHz
+    assert new.freqs.max() <= 70 * un.MHz
 
 
 def test_add(simple_gsdata):
     with pytest.raises(TypeError, match="can only add GSData objects"):
         simple_gsdata + 3
 
     new_times = simple_gsdata.update(
-        time_array=simple_gsdata.time_array + timedelta(days=1),
+        times=simple_gsdata.times + timedelta(days=1),
         time_ranges=simple_gsdata.time_ranges + 1 * un.day,
     )
 
-    new_freqs = simple_gsdata.update(freq_array=simple_gsdata.freq_array + 50 * un.MHz)
+    new_freqs = simple_gsdata.update(freqs=simple_gsdata.freqs + 50 * un.MHz)
 
-    new_timefreq = new_times.update(freq_array=new_freqs.freq_array)
+    new_timefreq = new_times.update(freqs=new_freqs.freqs)
 
     with pytest.raises(
         ValueError,
         match="Cannot add GSData objects with different frequencies",
     ):
         simple_gsdata + new_timefreq
 
@@ -317,27 +246,14 @@
     assert np.allclose(doubled.data, simple_gsdata.data * 2)
 
 
 def test_moon_sun(simple_gsdata: GSData):
     az, el = simple_gsdata.get_moon_azel()
     assert len(az) == len(el) == simple_gsdata.ntimes
 
-    in_lst = simple_gsdata.to_lsts()
-    with pytest.raises(
-        ValueError,
-        match="Cannot compute Moon positions when time array is not a Time object",
-    ):
-        in_lst.get_moon_azel()
-
-    with pytest.raises(
-        ValueError,
-        match="Cannot compute Sun positions when time array is not a Time object",
-    ):
-        in_lst.get_sun_azel()
-
 
 def test_cumulative_flags(simple_gsdata: GSData):
     # Add a few flags in...
 
     flg0 = np.zeros(simple_gsdata.data.shape, dtype=bool)
     no_flags = simple_gsdata.add_flags("zeros", flg0)
 
@@ -360,41 +276,170 @@
 
     assert np.array_equal(freq_flags.get_cumulative_flags(), freq_flags.complete_flags)
 
     with pytest.raises(ValueError, match="Flags for filter"):
         # can't add the same flags twice
         no_flags.add_flags("zeros", flg0)
 
-    with pytest.raises(ValueError, match="Cannot multiply GSFlag objects"):
-        no_flags.add_flags("new", np.zeros((1, 2, 3)))
+    with pytest.raises(ValueError, match="Objects have different npols"):
+        no_flags.add_flags("new", np.zeros((1, 2, 3, 4)))
 
     with pytest.raises(ValueError, match="Cannot append to file without a filename"):
         no_flags.add_flags("time", flg1, append_to_file=True)
 
     new_no_flags = time_flags.remove_flags("time")
+
+    flds = attrs.fields(GSData)
+    for fld in flds:
+        v1 = getattr(new_no_flags, fld.name)
+        v2 = getattr(no_flags, fld.name)
+
+        if not fld.eq:
+            continue
+        if fld.eq_key is not None:
+            if fld.eq_key(v1) != fld.eq_key(v2):
+                print(fld)
+        elif v1 != v2:
+            print(fld)
+
     assert new_no_flags == no_flags
 
     with pytest.raises(ValueError, match="No flags for filter"):
         no_flags.remove_flags("nonexistent")
 
 
 def test_initial_yearday(simple_gsdata):
-    assert simple_gsdata.get_initial_yearday() == "2022:231"
+    assert simple_gsdata.get_initial_yearday() == "2022:320"
 
     with pytest.raises(ValueError, match="Cannot return minutes without hours"):
         simple_gsdata.get_initial_yearday(minutes=True)
 
-    lst = simple_gsdata.to_lsts()
-
-    with pytest.raises(ValueError, match="Cannot represent times as year-days"):
-        lst.get_initial_yearday()
-
 
 def test_iterators(simple_gsdata):
     for slc in simple_gsdata.time_iter():
         assert simple_gsdata.data[slc].shape == simple_gsdata.data[:, :, 0].shape
 
     for slc in simple_gsdata.load_iter():
         assert simple_gsdata.data[slc].shape == simple_gsdata.data[0].shape
 
     for slc in simple_gsdata.freq_iter():
         assert simple_gsdata.data[slc].shape == simple_gsdata.data[:, :, :, 0].shape
+
+
+def test_trivial_model(simple_gsdata):
+    new = simple_gsdata.update(residuals=np.zeros_like(simple_gsdata.data))
+    assert np.all(new.residuals == 0)
+    assert np.array_equal(new.model, simple_gsdata.data)
+
+    assert simple_gsdata.model is None
+
+
+def test_partial_io_gspkl(simple_gsdata, tmp_path):
+    pth = tmp_path / "test.pkl"
+    with Path(pth).open("wb") as fl:
+        pickle.dump(simple_gsdata, fl)
+
+    new = GSData.from_file(
+        pth,
+        reader="gspkl",
+        selectors={
+            "time_selector": {"indx": np.arange(0, 10, 2)},
+            "lst_selector": {"lst_range": (0, 24)},
+            "freq_selector": {"freq_range": (50 * un.MHz, 70 * un.MHz)},
+            "load_selector": {"loads": ("ant",)},
+        },
+    )
+
+    assert new != simple_gsdata
+
+
+def test_multifile_read(simple_gsdata, tmp_path):
+    part1 = select_times(simple_gsdata, indx=list(range(5)))
+    part2 = select_times(simple_gsdata, indx=list(range(5, 10)))
+
+    part1.write_gsh5(tmp_path / "part1.gsh5")
+    part2.write_gsh5(tmp_path / "part2.gsh5")
+
+    new = GSData.from_file(
+        [tmp_path / "part1.gsh5", tmp_path / "part2.gsh5"], concat_axis="time"
+    )
+    assert np.all(new.data == simple_gsdata.data)
+
+
+def test_add_errors(
+    simple_gsdata, simple_gsdata_noaux, flagged_gsdata, modelled_gsdata
+):
+    new = simple_gsdata + simple_gsdata
+    assert np.all(new.data == simple_gsdata.data * 2)
+
+    with pytest.raises(
+        ValueError, match="Cannot add GSData objects with different shapes"
+    ):
+        simple_gsdata + select_freqs(
+            simple_gsdata, freq_range=(50 * un.MHz, 70 * un.MHz)
+        )
+
+    new = simple_gsdata + simple_gsdata_noaux
+    assert new.auxiliary_measurements is not None
+
+    new = simple_gsdata_noaux + simple_gsdata
+    assert new.auxiliary_measurements is not None
+
+    with pytest.warns(UserWarning, match="Overlapping auxiliary measurements exist"):
+        new = simple_gsdata + flagged_gsdata
+
+    assert new.auxiliary_measurements is not None
+
+    with pytest.raises(
+        ValueError, match="Cannot add GSData objects with different times"
+    ):
+        simple_gsdata + simple_gsdata.update(times=simple_gsdata.times + 1 * un.day)
+
+    modelled = modelled_gsdata + modelled_gsdata
+    assert np.all(modelled.residuals == 0)
+    assert np.all(modelled.data == simple_gsdata.data * 2)
+
+
+def test_gha(simple_gsdata):
+    assert simple_gsdata.gha.shape == simple_gsdata.times.shape
+    assert isinstance(simple_gsdata.gha, Longitude)
+
+
+def test_get_moon_sun(simple_gsdata):
+    az, el = simple_gsdata.get_moon_azel()
+    assert az.size == el.size == simple_gsdata.times.size
+
+    az, el = simple_gsdata.get_sun_azel()
+    assert az.size == el.size == simple_gsdata.times.size
+
+
+@pytest.mark.parametrize("which_flags", [None, (), "all", "twice"])
+@pytest.mark.parametrize("ignore_flags", [(), "all"])
+@pytest.mark.parametrize("data", ["simple_gsdata", "flagged_gsdata"])
+def test_cumulative_flags_cases(data, which_flags, request, ignore_flags):
+    data = request.getfixturevalue(data)
+
+    if which_flags == "all":
+        which_flags = tuple(data.flags.keys())
+    elif which_flags == "twice":
+        which_flags = 2 * tuple(data.flags.keys())
+
+    if ignore_flags == "all":
+        ignore_flags = tuple(data.flags.keys())
+
+    flags = data.get_cumulative_flags(
+        which_flags=which_flags, ignore_flags=ignore_flags
+    )
+    assert np.all(flags == 0)
+
+
+def test_get_initial_yearday(simple_gsdata):
+    yd = simple_gsdata.get_initial_yearday(hours=True, minutes=True)
+
+    yd1 = simple_gsdata.get_initial_yearday(hours=True, minutes=False)
+    assert yd.startswith(yd1)
+
+    yd2 = simple_gsdata.get_initial_yearday(hours=False, minutes=False)
+    assert yd1.startswith(yd2)
+
+    with pytest.raises(ValueError, match="Cannot return minutes without hours"):
+        simple_gsdata.get_initial_yearday(minutes=True)
```

