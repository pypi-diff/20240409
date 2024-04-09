# Comparing `tmp/priority-search-tree-0.0.2.tar.gz` & `tmp/priority-search-tree-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "priority-search-tree-0.0.2.tar", last modified: Tue Mar 26 12:20:48 2024, max compression
+gzip compressed data, was "priority-search-tree-0.1.0.tar", last modified: Tue Apr  9 11:39:45 2024, max compression
```

## Comparing `priority-search-tree-0.0.2.tar` & `priority-search-tree-0.1.0.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.095275 priority-search-tree-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.bumpversion.toml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.083275 priority-search-tree-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.087275 priority-search-tree-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-26 12:20:48.095275 priority-search-tree-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.087275 priority-search-tree-0.0.2/ci/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/ci/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/ci/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.083275 priority-search-tree-0.0.2/ci/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.083275 priority-search-tree-0.0.2/ci/templates/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.087275 priority-search-tree-0.0.2/ci/templates/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.091275 priority-search-tree-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.091275 priority-search-tree-0.0.2/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/reference/priority_search_tree.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/reference/priority_search_tree_print.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:20:48.095275 priority-search-tree-0.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2998 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.083275 priority-search-tree-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.091275 priority-search-tree-0.0.2/src/priority_search_tree/
--rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/src/priority_search_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/src/priority_search_tree/pst_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/src/priority_search_tree/pst_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.095275 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-26 12:20:48.000000 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-26 12:20:48.000000 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:20:48.000000 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:20:47.000000 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-26 12:20:48.000000 priority-search-tree-0.0.2/src/priority_search_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:20:48.095275 priority-search-tree-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    31674 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     7377 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/test_priority_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/test_pst_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-03-26 12:20:43.000000 priority-search-tree-0.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.bumpversion.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.459295 priority-search-tree-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.467295 priority-search-tree-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43669 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.467295 priority-search-tree-0.1.0/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.463295 priority-search-tree-0.1.0/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.463295 priority-search-tree-0.1.0/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.467295 priority-search-tree-0.1.0/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/ci/templates/.github/workflows/github-actions.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.467295 priority-search-tree-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.467295 priority-search-tree-0.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/reference/priority_search_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/reference/priority_search_tree_print.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2998 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.463295 priority-search-tree-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/src/priority_search_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/src/priority_search_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/src/priority_search_tree/print_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/src/priority_search_tree/ps_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/src/priority_search_tree/ps_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/src/priority_search_tree/ps_tree_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 11:39:45.000000 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-09 11:39:45.000000 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:39:45.000000 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:39:45.000000 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:39:45.000000 priority-search-tree-0.1.0/src/priority_search_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24784 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:39:45.471295 priority-search-tree-0.1.0/tests/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/manual/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/manual/stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/test_print_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/test_priority_search_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/test_priority_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/test_pst_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-09 11:39:41.000000 priority-search-tree-0.1.0/tox.ini
```

### Comparing `priority-search-tree-0.0.2/.bumpversion.toml` & `priority-search-tree-0.1.0/.bumpversion.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.0.2"
+current_version = "0.1.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 ignore_missing_files = false
```

### Comparing `priority-search-tree-0.0.2/.github/workflows/build.yml` & `priority-search-tree-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/.github/workflows/publish.yml` & `priority-search-tree-0.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/.pre-commit-config.yaml` & `priority-search-tree-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/CONTRIBUTING.rst` & `priority-search-tree-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/LICENSE` & `priority-search-tree-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/PKG-INFO` & `priority-search-tree-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: priority-search-tree
-Version: 0.0.2
+Version: 0.1.0
 Summary: Priority search tree data structure
 Home-page: https://github.com/yusinv/priority-search-tree
 Author: Valentin Yusin
 Author-email: yusinv@gmail.com
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://priority-search-tree.readthedocs.io/
 Project-URL: Changelog, https://priority-search-tree.readthedocs.io/en/latest/changelog.html
@@ -33,34 +33,32 @@
 
 ========
 Overview
 ========
 
 
 
-The priority search tree (PST) is data structure with the following properties:
+The priority search tree (PST) is data structure (mutable mapping {**key**: **priority**}) with the following properties:
 
-* Items are stored in binary search tree (red-black tree in this case) using ``tree_key(value)``  function as a key.
-* Maintains max heap properties using ``heap_key(value)`` function as key.
-* Ability to perform efficient  *O(log(N)+K)* 3-sided search (finds items with ``tree_key`` in interval **[min_tree_key,max_tree_key]** and ``heap_key`` is grater or equal to **bottom_heap_key**).
+* Keys are stored in binary search tree (red-black tree in this case).
+* Maintains max heap properties (can return **key** with max **priority** in constant time).
+* Ability to perform efficient 3-sided search (finds items with **key** in interval `[min_tree_key,max_tree_key]` and **priority** is grater or equal to `bottom_priority`).
 
-For example PST can store 2 dimensional points P(X,Y) using X coordinate as ``tree_key`` and Y coordinate as ``heap_key``.  Such PST can perform 3 sided search to find points with X in [X_MIN,X_MAX] and Y >= Y_BOTTOM.
-
-Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
+For example PST can store 2 dimensional points `P(X,Y)` using X coordinate as **key** and Y coordinate as **priority**.  Such PST can perform 3 sided search to find points with `X in [X_MIN,X_MAX]` and `Y >= Y_BOTTOM`.
 
 Installation
 ============
 
 ::
 
     pip install priority-search-tree
 
 You can also install the in-development version with::
 
-    pip install https://github.com/yusinv/priority-search-tree/archive/main.zip
+    pip install https://github.com/yusinv/priority-search-tree/archive/develop.zip
 
 
 Documentation
 =============
 
 
 https://priority-search-tree.readthedocs.io/
@@ -70,14 +68,20 @@
 ===========
 
 To run all the tests run::
 
     tox
 
 
+Licence
+=======
+
+Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
+
+
 Changelog
 =========
 
 0.0.0 (2024-03-04)
 ------------------
 
 * First release on PyPI.
@@ -92,7 +96,15 @@
 0.0.2 (2024-03-26)
 ------------------
 
 * Added sorted_query method.
 * Added __len__ and __contains__ methods.
 * Added clear method.
 * Fixed issue with not unique heap keys
+
+
+0.1.0 (2024-04-08)
+------------------
+
+* Refactoring
+* Added PrioritySearchSet class
+* Added __iter__ method
```

### Comparing `priority-search-tree-0.0.2/README.rst` & `priority-search-tree-0.1.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -37,42 +37,40 @@
     :alt: Supported versions
     :target: https://pypi.org/project/priority-search-tree
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/priority-search-tree.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/priority-search-tree
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/yusinv/priority-search-tree/v0.0.2.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/yusinv/priority-search-tree/v0.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/yusinv/priority-search-tree/compare/v0.0.2...main
+    :target: https://github.com/yusinv/priority-search-tree/compare/v0.1.0...main
 
 
 
 .. end-badges
 
-The priority search tree (PST) is data structure with the following properties:
+The priority search tree (PST) is data structure (mutable mapping {**key**: **priority**}) with the following properties:
 
-* Items are stored in binary search tree (red-black tree in this case) using ``tree_key(value)``  function as a key.
-* Maintains max heap properties using ``heap_key(value)`` function as key.
-* Ability to perform efficient  *O(log(N)+K)* 3-sided search (finds items with ``tree_key`` in interval **[min_tree_key,max_tree_key]** and ``heap_key`` is grater or equal to **bottom_heap_key**).
+* Keys are stored in binary search tree (red-black tree in this case).
+* Maintains max heap properties (can return **key** with max **priority** in constant time).
+* Ability to perform efficient 3-sided search (finds items with **key** in interval `[min_tree_key,max_tree_key]` and **priority** is grater or equal to `bottom_priority`).
 
-For example PST can store 2 dimensional points P(X,Y) using X coordinate as ``tree_key`` and Y coordinate as ``heap_key``.  Such PST can perform 3 sided search to find points with X in [X_MIN,X_MAX] and Y >= Y_BOTTOM.
-
-Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
+For example PST can store 2 dimensional points `P(X,Y)` using X coordinate as **key** and Y coordinate as **priority**.  Such PST can perform 3 sided search to find points with `X in [X_MIN,X_MAX]` and `Y >= Y_BOTTOM`.
 
 Installation
 ============
 
 ::
 
     pip install priority-search-tree
 
 You can also install the in-development version with::
 
-    pip install https://github.com/yusinv/priority-search-tree/archive/main.zip
+    pip install https://github.com/yusinv/priority-search-tree/archive/develop.zip
 
 
 Documentation
 =============
 
 
 https://priority-search-tree.readthedocs.io/
@@ -80,7 +78,13 @@
 
 Development
 ===========
 
 To run all the tests run::
 
     tox
+
+
+Licence
+=======
+
+Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `priority-search-tree-0.0.2/ci/bootstrap.py` & `priority-search-tree-0.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/ci/templates/.github/workflows/github-actions.yml` & `priority-search-tree-0.1.0/ci/templates/.github/workflows/github-actions.yml.j2`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/docs/conf.py` & `priority-search-tree-0.1.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "priority-search-tree"
 year = "2024"
 author = "Valentin Yusin"
 copyright = f"{year}, {author}"
-version = release = "0.0.2"
+version = release = "0.1.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/yusinv/priority-search-tree/issues/%s", "#"),
     "pr": ("https://github.com/yusinv/priority-search-tree/pull/%s", "PR #"),
 }
```

### Comparing `priority-search-tree-0.0.2/pyproject.toml` & `priority-search-tree-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `priority-search-tree-0.0.2/pytest.ini` & `priority-search-tree-0.1.0/pytest.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [pytest]
 # If a pytest section is found in one of the possible config files
 # (pytest.ini, tox.ini or setup.cfg), then pytest will not look for any others,
 # so if you add a pytest config section elsewhere,
 # you will need to delete this section from setup.cfg.
 norecursedirs =
     migrations
+    manual
 
 python_files =
     test_*.py
     *_test.py
     tests.py
 addopts =
     -ra
```

### Comparing `priority-search-tree-0.0.2/setup.py` & `priority-search-tree-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="priority-search-tree",
-    version="0.0.2",
+    version="0.1.0",
     license="LGPL-3.0-or-later",
     description="Priority search tree data structure",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Valentin Yusin",
```

### Comparing `priority-search-tree-0.0.2/src/priority_search_tree/__init__.py` & `priority-search-tree-0.1.0/src/priority_search_tree/ps_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,191 @@
-__version__ = "0.0.2"
-
-from collections import deque
-from typing import Callable
 from typing import Iterable
+from typing import Iterator
+from typing import MutableMapping
 from typing import Optional
+from typing import Tuple
 from typing import TypeVar
 
-from .pst_node import Node
+from .ps_tree_node import Node
 
-_V = TypeVar("_V")
-_SupportsRichComparisonT = TypeVar("_SupportsRichComparisonT")
+_KEY = TypeVar("_KEY")
+_PRIORITY = TypeVar("_PRIORITY")
 
 
-class PrioritySearchTree:
-    """
-    Class that represents Priority search tree.
+class PrioritySearchTree(MutableMapping):
+    """Class that represents Priority search tree.
+
+    PrioritySearchTree is a mutable mapping that stores **keys** and corresponding **priorities**.
+
+    * Keys are stored in balanced binary search tree (red/black tree) that allow to effectively perform next operations:
+
+            * in order traversal
+            * find min/max keys
+            * find next/previous keys
+
+    * Priorities and keys form max priority queue, that allow to effectively perform next operations:
+
+            * find element with max priority
+            * remove element with max priority
+            * update priority for a given key
+
+    * It is capable to perform 3 sided queries
 
     Example::
 
         # create new tree
         pst = PrioritySearchTree([(1,1),(2,2)])
-        # add item to the tree
-        pst.add((3,3))
+        # add key 3 to the tree with priority 5
+        pst[3] = 5
         # perform 3 sided query
-        result = pst.query((0,0),(4,0),(0,2))
+        result = pst.query(0,4,2)
 
     Args:
-        iterable (Iterable): Initial values to build priority search tree. The default value is ``None``.
-        tree_key (Callable): Specifies a function of one argument that is used to extract a *tree* comparison key
-            from each element (for example, ``tree_key=str.lower``). The default value is ``tree_key=lambda x: x``
-        heap_key (Callable): Specifies a function of one argument that is used to extract a *heap* comparison key
-            from each element (for example, ``tree_key=str.lower``). The default value is ``tree_key=lambda x: x[1:]``
+        iterable (Iterable): Initial values to build priority search tree.
+            Each item in the iterable must itself be an iterable with exactly two objects.
+            The first object of each item becomes a **key** in the new pst, and the second object the corresponding
+            **priority**. The default value is ``None``.
 
     Raises:
-        ValueError: in case if iterable contains values with not unique tree_key
+        KeyError: in case if iterable contains values with not unique **key**
 
     Complexity:
-        O(N*log(N)) where **N** is number of items to be added to new PST
+        `O(N*log(N))` where **N** is number of items to be added to new PST
     """
 
-    def _push_down(self, node: Node, value: _V) -> None:
-        if node == Node.NULL_NODE:
-            return
-        if node.heap_value is None:
-            node.heap_value = value
-            return
-
-        if self.tree_key(node.heap_value) < self.tree_key(node.tree_value):
-            self._push_down(node.left, node.heap_value)
-        else:
-            self._push_down(node.right, node.heap_value)
-
-        if node.placeholder:
-            node.placeholder = False
-        else:
-            node.heap_value = value
+    __slots__ = ["_root", "_len"]
 
-    def _sieve_down(self, node: Node, value: _V) -> None:
+    def _push_down(self, node: Node, heap_key: Tuple[_PRIORITY, _KEY]) -> None:
 
-        if node.heap_value is None:
-            node.heap_value = value
+        if node.heap_key[0] == Node.PLACEHOLDER_VALUE:
+            node.heap_key = heap_key
             return
 
-        if node.placeholder:
-            node.placeholder = False
-            return
+        if node.heap_key[1] < node.tree_key:
+            self._push_down(node.left, node.heap_key)
+        else:
+            self._push_down(node.right, node.heap_key)
 
-        heap_key_value = self.heap_key(value)
-        tree_key_value = self.tree_key(value)
+        node.heap_key = heap_key
 
-        if heap_key_value > self.heap_key(node.heap_value):
-            self._push_down(node, value)
+    def _sift_down(self, node: Node, heap_key: Tuple[_PRIORITY, _KEY]) -> None:
+
+        if node.heap_key[0] == Node.PLACEHOLDER_VALUE:
+            node.heap_key = heap_key
             return
 
-        if heap_key_value == self.heap_key(node.heap_value) and tree_key_value < self.tree_key(node.heap_value):
-            self._push_down(node, value)
+        if heap_key > node.heap_key:
+            self._push_down(node, heap_key)
             return
 
-        if tree_key_value < self.tree_key(node.tree_value):
-            self._sieve_down(node.left, value)
+        if heap_key[1] < node.tree_key:
+            self._sift_down(node.left, heap_key)
         else:
-            self._sieve_down(node.right, value)
+            self._sift_down(node.right, heap_key)
 
     def _push_up(self, node: Node) -> None:
-        vl, vr = None, None
+        if node.heap_key[0] == Node.PLACEHOLDER_VALUE:
+            return
 
-        if not node.left.placeholder:
-            vl = node.left.heap_value
+        if node.left.heap_key[0] == Node.PLACEHOLDER_VALUE:
+            node.heap_key = node.right.heap_key
+            self._push_up(node.right)
+            return
 
-        if not node.right.placeholder:
-            vr = node.right.heap_value
+        if node.right.heap_key[0] == Node.PLACEHOLDER_VALUE:
+            node.heap_key = node.left.heap_key
+            self._push_up(node.left)
+            return
 
-        if vl and vr:
-            if self.heap_key(vl) >= self.heap_key(vr):
-                node.heap_value = vl
-                self._push_up(node.left)
-            else:
-                node.heap_value = vr
-                self._push_up(node.right)
-        elif vl:
-            node.heap_value = vl
+        if node.left.heap_key >= node.right.heap_key:
+            node.heap_key = node.left.heap_key
             self._push_up(node.left)
-        elif vr:
-            node.heap_value = vr
-            self._push_up(node.right)
         else:
-            if node.left == Node.NULL_NODE and node.right == Node.NULL_NODE:
-                node.placeholder = True
-            else:
-                node.heap_value = None
+            node.heap_key = node.right.heap_key
+            self._push_up(node.right)
 
-    def __init__(
-        self,
-        iterable: Optional[Iterable[_V]] = None,
-        tree_key: Callable[[_V], _SupportsRichComparisonT] = lambda x: x,
-        heap_key: Callable[[_V], _SupportsRichComparisonT] = lambda x: x[1:],
-    ) -> None:
+    def __init__(self, iterable: Optional[Iterable[Tuple[_KEY, _PRIORITY]]] = None) -> None:
         self._root: Node = Node.NULL_NODE
-        self.tree_key = tree_key
-        self.heap_key = heap_key
         self._len: int = 0
 
         if iterable:
-            sn = sorted(iterable, key=self.tree_key)
-
-            current_key = self.tree_key(sn[0])
-            for next_key in map(self.tree_key, sn[1:]):
-                if current_key == next_key:
-                    raise ValueError(f"More than one item with tree_key:{current_key}")
+            sn = sorted(iterable)
+            current_key = sn[0]
+            for next_key in sn[1:]:
+                if current_key[0] == next_key[0]:
+                    raise KeyError(f"More than one item with key:{current_key[0]}")
                 current_key = next_key
 
             sn_len = len(sn)
             sn_iter = iter(sn)
             tree_nodes = []
             lvl = sn_len.bit_length()
             for _ in range(sn_len - 2 ** (lvl - 1)):
-                value = next(sn_iter)
-                ln = Node(heap_value=value, tree_value=value)
-                value = next(sn_iter)
-                rn = Node(heap_value=value, tree_value=value)
-                pn = Node(tree_value=rn.tree_value, color=0)
+                keys = next(sn_iter)
+                ln = Node(tree_key=keys[0], heap_key=(keys[1], keys[0]))
+                keys = next(sn_iter)
+                rn = Node(tree_key=keys[0], heap_key=(keys[1], keys[0]))
+                pn = Node(tree_key=rn.tree_key, heap_key=(keys[1], keys[0]), color=0)
                 pn.set_left(ln)
                 pn.set_right(rn)
                 self._push_up(pn)
-                tree_nodes.append((pn, ln.tree_value, rn.tree_value))
+                tree_nodes.append((pn, ln.tree_key, rn.tree_key))
 
-            for value in sn_iter:
-                pn = Node(heap_value=value, tree_value=value, color=0)
-                tree_nodes.append((pn, pn.tree_value, pn.tree_value))
+            for keys in sn_iter:
+                pn = Node(tree_key=keys[0], heap_key=(keys[1], keys[0]), color=0)
+                tree_nodes.append((pn, pn.tree_key, pn.tree_key))
 
             while len(tree_nodes) > 1:
                 new_nodes = []
                 for i in range(0, len(tree_nodes), 2):
                     ln, ln_min, ln_max = tree_nodes[i]
                     rn, rn_min, rn_max = tree_nodes[i + 1]
-                    pn = Node(tree_value=rn_min, color=0)
+                    pn = Node(tree_key=rn_min, heap_key=ln.heap_key, color=0)
                     pn.set_left(ln)
                     pn.set_right(rn)
                     self._push_up(pn)
                     new_nodes.append((pn, ln_min, rn_max))
                 tree_nodes = new_nodes
 
             self._root = tree_nodes[0][0]
             self._len = sn_len
 
-    def heap_get_max(self) -> _V:
-        """
-        Return the item with the largest **heap_key** from the PST.
+    def get_with_max_priority(self) -> _KEY:
+        """Returns the **key** with the largest **priority** in PST.
 
         Returns:
-            item with the largest **heap_key**
+            **key** with the largest **priority**
 
         Raises:
-            IndexError: If the PST is empty
+            KeyError: If the PST is empty
 
         Complexity:
-            O(1)
+            `O(1)`
         """
         if self._root == Node.NULL_NODE:
-            raise IndexError
-        return self._root.heap_value
+            raise KeyError
+        return self._root.heap_key[1]
 
-    def heap_pop(self) -> _V:
-        """
-        Remove and return the item with the largest **heap_key** from the PST.
+    def popitem(self) -> Tuple[_KEY, _PRIORITY]:
+        """Remove and return (key, priority) pair from the PST. Pair with max **priority** will be removed.
 
         Returns:
-            item with the largest **heap_key**
+            Tuple: **key** and **priority** pair
 
         Raises:
-            IndexError: If the PST is empty
+            KeyError: If the PST is empty
 
         Complexity:
-            O(log(N)) where **N** is number of items in PST
+            `O(log(N))` where **N** is number of items in PST
         """
         if self._root == Node.NULL_NODE:
-            raise IndexError
-        result = self._root.heap_value
-        self.remove(result)
-        return result
-
-    def add(self, value: _V) -> None:
-        """
-        Add new item to PST.
-
-        Args:
-            value: Value to insert into PST
-
-        Raises:
-            ValueError: in case if value with **tree_key** already exists in PST
-
-        Complexity:
-            O(log(N)) where **N** is number of items in PST
-        """
-        if self._root == Node.NULL_NODE:
-            self._root = Node(heap_value=value, tree_value=value, color=0)
-            self._len = 1
-            return
-
-        value_tree_key = self.tree_key(value)
-
-        prev = None
-        node = self._root
-        while node != Node.NULL_NODE:
-            prev = node
-            if value_tree_key < self.tree_key(node.tree_value):
-                node = node.left
-            elif value_tree_key == self.tree_key(node.tree_value):
-                raise ValueError(f"Value with tree_key:{value_tree_key} already in tree")
-            else:
-                node = node.right
-
-        new_internal_node = Node(color=prev.color)
-        new_leaf_node = Node(tree_value=value, heap_value=value, placeholder=True)
-        prev.color = 1
-
-        if prev.parent:
-            if prev.parent.left == prev:
-                prev.parent.set_left(new_internal_node)
-            else:
-                prev.parent.set_right(new_internal_node)
-        else:
-            self._root = new_internal_node
-            new_internal_node.color = 0
-
-        if value_tree_key < self.tree_key(prev.tree_value):
-            new_internal_node.tree_value = prev.tree_value
-            new_internal_node.set_right(prev)
-            new_internal_node.set_left(new_leaf_node)
-        else:
-            new_internal_node.tree_value = value
-            new_internal_node.set_right(new_leaf_node)
-            new_internal_node.set_left(prev)
-
-        if not prev.placeholder:
-            new_internal_node.heap_value = prev.heap_value
-            prev.placeholder = True
-
-        self._sieve_down(self._root, value)
-        self._fix_insert(new_leaf_node)
-        self._len += 1
-
-    def remove(self, value: _V) -> None:
-        """
-        Remove item from PST.
-
-        Args:
-            value: Value to remove from PST
-
-        Raises:
-            ValueError: in case if value not exists in PST
-
-        Complexity:
-            O(log(N)) where **N** is number of items in PST
-
-        Note:
-            this function is using ``tree_key(value)`` to compare the items
-        """
-        node = self._root
-        value_tree_key = self.tree_key(value)
-        heap_node = None
-        tree_node = None
-        leaf_node = None
-
-        while node != Node.NULL_NODE:
-            leaf_node = node
-            if heap_node is None and self.tree_key(node.heap_value) == value_tree_key:
-                heap_node = node
-            if tree_node is None and self.tree_key(node.tree_value) == value_tree_key:
-                tree_node = node
-            if value_tree_key < self.tree_key(node.tree_value):
-                node = node.left
-            else:
-                node = node.right
-
-        if heap_node is None:
-            raise ValueError(f"Value not found:{value}")
-
-        if leaf_node == self._root:
-            self._root = Node.NULL_NODE
-            self._len = 0
-            return
-
-        self._push_up(heap_node)
-
-        if tree_node.left == Node.NULL_NODE:  # left node
-            cut_node = tree_node.parent
-            fix_node = tree_node.parent.right
-        elif tree_node.right == leaf_node:  # leaf children
-            cut_node = tree_node
-            fix_node = tree_node.left
-        else:  # subtree case
-            tree_node.tree_value = leaf_node.parent.tree_value
-            cut_node = leaf_node.parent
-            fix_node = leaf_node.parent.right
-
-        self._push_down(cut_node, None)
-        self._transplant(cut_node, fix_node)
-
-        if cut_node.color == 0:
-            self._fix_delete(fix_node)
-
-        self._len -= 1
+            raise KeyError
+        result = self._root.heap_key
+        del self[result[1]]
+        return result[1], result[0]
 
     def _fix_delete(self, node: Node) -> None:
         while node != self._root and node.color == 0:
             if node == node.parent.left:
                 s_node = node.parent.right
                 if s_node.color == 1:
                     s_node.color = 0
@@ -378,125 +238,118 @@
             self._root = v
             self._root.parent = None
         elif u == u.parent.left:
             u.parent.set_left(v)
         else:
             u.parent.set_right(v)
 
-    def query(self, tree_left: _V, tree_right: _V, heap_bottom: _V) -> [_V]:
+    def query(self, key_left: _KEY, key_right: _KEY, priority_bottom: _PRIORITY) -> list:
         """Performs 3 sided query on PST.
 
         This function returns list of items that meet the following criteria:
-            1. items have **tree_key** grater or equal to **tree_key** of tree_left argument
-            2. items have **tree_key** smaller or equal to **tree_key** of tree_right argument
-            3. items have **heap_key** grater or equal to **heap_key** of heap_bottom argument
+            1. items have **key** grater or equal to `key_left` argument
+            2. items have **key** smaller or equal to `key_right` argument
+            3. items have **priority** grater or equal to `priority_bottom` argument
 
         Args:
-            tree_left: Left bound for query (**tree_key** is used).
-            tree_right: Right bound for query (**tree_key** is used).
-            heap_bottom: Bottom bound for query (**heap_key** is used).
+            key_left: Left bound for query (**key** is used to compare).
+            key_right: Right bound for query (**key** is used to compare).
+            priority_bottom: Bottom bound for query (**priority** is used to compare).
 
         Returns:
-            List: list of items that satisfy criteria, or empty list if no items found
+            List: list of **keys** that satisfy criteria, or empty list if no items found
 
         Complexity:
-            O(log(N)+K) where **N** is number of items in PST and **K** is number of reported items
+            `O(log(N)+K)` where **N** is number of items in PST and **K** is number of reported items
         """
         result = []
-        queue = deque()
-        queue.append(self._root)
-        while queue:
-            node = queue.popleft()
-
-            if node == Node.NULL_NODE or node.placeholder:
-                continue
-
-            if node.heap_value:
-                if self.heap_key(node.heap_value) >= self.heap_key(heap_bottom):
-                    if self.tree_key(tree_left) <= self.tree_key(node.heap_value) <= self.tree_key(tree_right):
-                        result.append(node.heap_value)
-                else:
-                    continue
 
-            if self.tree_key(tree_right) < self.tree_key(node.tree_value):
-                queue.append(node.left)
-            elif self.tree_key(tree_left) >= self.tree_key(node.tree_value):
-                queue.append(node.right)
+        def _query_node(node) -> None:
+            if node == Node.NULL_NODE or node.heap_key[0] == Node.PLACEHOLDER_VALUE:
+                return
+
+            if node.heap_key[0] >= priority_bottom:
+                if key_left <= node.heap_key[1] <= key_right:
+                    result.append(node.heap_key[1])
+            else:
+                return
+
+            if key_right < node.tree_key:
+                _query_node(node.left)
+            elif key_left >= node.tree_key:
+                _query_node(node.right)
             else:
-                queue.append(node.left)
-                queue.append(node.right)
+                _query_node(node.left)
+                _query_node(node.right)
 
+        _query_node(self._root)
         return result
 
-    def sorted_query(self, tree_left: _V, tree_right: _V, heap_bottom: _V, items_limit: int = 0) -> [_V]:
+    def sorted_query(self, key_left: _KEY, key_right: _KEY, priority_bottom: _PRIORITY, items_limit: int = 0) -> list:
         """Performs 3 sided query on PST.
 
         This function returns list of items that meet the following criteria:
-            1. items have **tree_key** grater or equal to **tree_key** of tree_left argument
-            2. items have **tree_key** smaller or equal to **tree_key** of tree_right argument
-            3. items have **heap_key** grater or equal to **heap_key** of heap_bottom argument
+            1. items have **key** grater or equal to `key_left` argument
+            2. items have **key** smaller or equal to `key_right` argument
+            3. items have **priority** grater or equal to `priority_bottom` argument
 
         Args:
-            tree_left: Left bound for query (**tree_key** is used).
-            tree_right: Right bound for query (**tree_key** is used).
-            heap_bottom: Bottom bound for query (**heap_key** is used).
+            key_left: Left bound for query (**key** is used to compare).
+            key_right: Right bound for query (**key** is used to compare).
+            priority_bottom: Bottom bound for query (**priority** is used to compare).
             items_limit (int): Number of items to return. Default value is ``0`` - no limit.
 
         Returns:
-            List: list of items that satisfy criteria and sorted by **heap_key**
-            (in case of limit, items with largest **heap_key** will be returned), or empty list if no items found
+            List: list of items that satisfy criteria and sorted by **priority**
+            (in case of limit, items with largest **priority** will be returned), or empty list if no items found
 
         Complexity:
-            O(log(N)+K*log(K)) where **N** is number of items in PST and **K** is number of returned items
+            `O(log(N)+K*log(K))` where **N** is number of items in PST and **K** is number of returned items
         """
-        tree_left_key = self.tree_key(tree_left)
-        tree_right_key = self.tree_key(tree_right)
-        heap_bottom_key = self.heap_key(heap_bottom)
         if items_limit <= 0:
             items_limit = self._len
 
-        def _query_node(node, limit):
+        def _sorted_query_node(node, limit) -> list:
             result = []
-            if node == Node.NULL_NODE or node.placeholder or limit == 0:
+            if node == Node.NULL_NODE or node.heap_key[0] == Node.PLACEHOLDER_VALUE or limit == 0:
                 return result
 
-            if node.heap_value:
-                if self.heap_key(node.heap_value) >= heap_bottom_key:
-                    if tree_left_key <= self.tree_key(node.heap_value) <= tree_right_key:
-                        result.append(node.heap_value)
-                        limit -= 1
-                else:
-                    return result
+            if node.heap_key[0] >= priority_bottom:
+                if key_left <= node.heap_key[1] <= key_right:
+                    result.append(node.heap_key)
+                    limit -= 1
+            else:
+                return result
 
-            if tree_right_key < self.tree_key(node.tree_value):
-                result.extend(_query_node(node.left, limit))
-            elif tree_left_key >= self.tree_key(node.tree_value):
-                result.extend(_query_node(node.right, limit))
+            if key_right < node.tree_key:
+                result.extend(_sorted_query_node(node.left, limit))
+            elif key_left >= node.tree_key:
+                result.extend(_sorted_query_node(node.right, limit))
             else:
-                left = _query_node(node.left, limit)
-                right = _query_node(node.right, limit)
+                left = _sorted_query_node(node.left, limit)
+                right = _sorted_query_node(node.right, limit)
                 # merge
                 i, j = 0, 0
                 while i < len(left) and j < len(right) and len(result) < items_limit:
-                    if self.heap_key(left[i]) >= self.heap_key(right[j]):
+                    if left[i] >= right[j]:
                         result.append(left[i])
                         i += 1
                     else:
                         result.append(right[j])
                         j += 1
                 while i < len(left) and len(result) < items_limit:
                     result.append(left[i])
                     i += 1
                 while j < len(right) and len(result) < items_limit:
                     result.append(right[j])
                     j += 1
 
             return result
 
-        return _query_node(self._root, items_limit)
+        return [x[1] for x in _sorted_query_node(self._root, items_limit)]
 
     def _fix_insert(self, node: Node) -> None:
         while node.parent.color == 1:
             if node.parent.parent.right == node.parent:
                 u = node.parent.parent.left
                 if u.color == 1:
                     u.color = 0
@@ -528,15 +381,15 @@
             if node == self._root:
                 break
 
         self._root.color = 0
 
     def _rotate_right(self, x: Node) -> None:
         y = x.left
-        self._push_down(y, x.heap_value)
+        self._push_down(y, x.heap_key)
         x.set_left(y.right)
 
         if not x.parent:
             self._root = y
             y.parent = None
 
         elif x == x.parent.left:
@@ -545,15 +398,15 @@
             x.parent.set_right(y)
 
         y.set_right(x)
         self._push_up(x)
 
     def _rotate_left(self, x: Node) -> None:
         y = x.right
-        self._push_down(y, x.heap_value)
+        self._push_down(y, x.heap_key)
         x.set_right(y.left)
 
         if not x.parent:
             self._root = y
             y.parent = None
 
         elif x == x.parent.left:
@@ -561,56 +414,224 @@
         else:
             x.parent.set_right(y)
 
         y.set_left(x)
         self._push_up(x)
 
     def __len__(self) -> int:
-        """
-        Implements the built-in function len()
+        """Implements the built-in function len()
 
         Returns:
             int: Number of items in PST.
 
         Complexity:
-            O(1)
+            `O(1)`
         """
         return self._len
 
-    def __contains__(self, value) -> bool:
+    def clear(self) -> None:
+        """Removes **all** items from PST.
+
+        Complexity:
+            `O(1)`
         """
-        Implements membership test operator.
+        self._root = Node.NULL_NODE
+        self._len = 0
+
+    def update_priority(self, key: _KEY, priority: _PRIORITY) -> _PRIORITY:
+        """Updates priority for the given key.
 
         Args:
-            value: Value to test for membership
+            key: **key** to update
+            priority: new **priority** value
 
         Returns:
-            bool:  ``True`` if value is in ``self``, ``False`` otherwise.
+            old **priority** value
+
+        Raises:
+            KeyError: in case if **key** not exists in PST
 
         Complexity:
-            O(log(N)) where **N** is number of items in PST
+            `O(log(N))` where **N** is number of items in PST
 
-        Note:
-            this function is using ``tree_key(value)`` to compare the items
         """
-        value_tree_key = self.tree_key(value)
+        node = self._root
+        heap_node = None
+        while node.heap_key[0] != Node.PLACEHOLDER_VALUE:
+
+            if key == node.heap_key[1]:
+                heap_node = node
+                break
+
+            if key < node.tree_key:
+                node = node.left
+            else:
+                node = node.right
+
+        if not heap_node:
+            raise KeyError(f"Key not found:{key}")
+
+        result = heap_node.heap_key[0]
+        self._push_up(heap_node)
+        self._sift_down(self._root, (priority, key))
+        return result
+
+    def __setitem__(self, key: _KEY, priority: _PRIORITY) -> None:
+        """implements assignment operation.
+
+        Args:
+            key: **key** to add/update
+            priority: new **priority**
+
+        Complexity:
+            `O(log(N))` where **N** is number of items in PST
 
+        """
+        if self._root == Node.NULL_NODE:
+            self._root = Node(tree_key=key, heap_key=(priority, key), color=0)
+            self._len = 1
+            return
+
+        prev = None
         node = self._root
         while node != Node.NULL_NODE:
-            if value_tree_key < self.tree_key(node.tree_value):
+            prev = node
+            if key < node.tree_key:
                 node = node.left
-            elif value_tree_key == self.tree_key(node.tree_value):
-                return True
+            elif key == node.tree_key:
+                self.update_priority(key, priority)
+                return
             else:
                 node = node.right
 
-        return False
+        new_placeholder = Node(tree_key=key, heap_key=(Node.PLACEHOLDER_VALUE, Node.PLACEHOLDER_VALUE))
+        prev_placeholder = Node(tree_key=prev.tree_key, heap_key=(Node.PLACEHOLDER_VALUE, Node.PLACEHOLDER_VALUE))
 
-    def clear(self) -> None:
+        if key < prev.tree_key:
+            prev.set_right(prev_placeholder)
+            prev.set_left(new_placeholder)
+        else:
+            prev.tree_key = key
+            prev.set_right(new_placeholder)
+            prev.set_left(prev_placeholder)
+
+        self._sift_down(self._root, (priority, key))
+        self._fix_insert(new_placeholder)
+        self._len += 1
+
+    def __delitem__(self, key: _KEY) -> None:
+        """Remove **key** from PST.
+
+        Args:
+            key: **key** to remove
+
+        Raises:
+            KeyError: in case if **key** not exists in PST
+
+        Complexity:
+            `O(log(N))` where **N** is number of items in PST
         """
-        Removes **all** items from PST.
+        tree_node = None
+        node = self._root
+        while node != Node.NULL_NODE:
+            if key == node.tree_key:
+                tree_node = node
+                break
+            elif key < node.tree_key:
+                node = node.left
+            else:
+                node = node.right
+
+        if tree_node is None:
+            raise KeyError(f"Key not found:{key}")
+
+        leaf_node = None
+        node = tree_node
+        while node != Node.NULL_NODE:
+            leaf_node = node
+            if key < node.tree_key:
+                node = node.left
+            else:
+                node = node.right
+
+        if leaf_node == self._root:
+            self._root = Node.NULL_NODE
+            self._len = 0
+            return
+
+        # remove heap value
+        node = leaf_node
+        while node.heap_key[1] != key:
+            node = node.parent
+        self._push_up(node)
+
+        if tree_node.left == Node.NULL_NODE:  # left node
+            cut_node = tree_node.parent
+            fix_node = tree_node.parent.right
+        elif tree_node.right == leaf_node:  # leaf children
+            cut_node = tree_node
+            fix_node = tree_node.left
+        else:  # subtree case
+            tree_node.tree_key = leaf_node.parent.tree_key
+            cut_node = leaf_node.parent
+            fix_node = leaf_node.parent.right
+
+        self._push_down(cut_node, cut_node.heap_key)
+        self._transplant(cut_node, fix_node)
+
+        if cut_node.color == 0:
+            self._fix_delete(fix_node)
+
+        self._len -= 1
+
+    def __getitem__(self, key: _KEY) -> _PRIORITY:
+        """Returns **priority** of given **key** in PST.
+
+        Args:
+            key: **key** to find
+
+        Returns:
+            **priority** value if the given **key**
+
+        Raises:
+            KeyError: in case if **key** not exists in PST
 
         Complexity:
-            O(1)
+            `O(log(N))` where **N** is number of items in PST
         """
-        self._root = Node.NULL_NODE
-        self._len = 0
+        node = self._root
+        heap_node = None
+        while node.heap_key[0] != Node.PLACEHOLDER_VALUE:
+            if key == node.heap_key[1]:
+                heap_node = node
+                break
+            if key < node.tree_key:
+                node = node.left
+            else:
+                node = node.right
+
+        if not heap_node:
+            raise KeyError(f"Key not found:{key}")
+
+        return heap_node.heap_key[0]
+
+    def __iter__(self) -> Iterator:
+        """Create an iterator that iterates **keys** in sorted order
+
+        Returns:
+            Iterator: in order iterator
+        """
+        stack = []
+        current = self._root
+        yielded_key = None
+        while True:
+            if current != Node.NULL_NODE:
+                stack.append(current)
+                current = current.left
+            elif stack:
+                current = stack.pop()
+                if current.tree_key != yielded_key:
+                    yielded_key = current.tree_key
+                    yield yielded_key
+                current = current.right
+            else:
+                break
```

### Comparing `priority-search-tree-0.0.2/src/priority_search_tree/pst_node.py` & `priority-search-tree-0.1.0/src/priority_search_tree/ps_tree_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from typing import Any
 from typing import Optional
+from typing import Tuple
 from typing import TypeVar
 
 _Self = TypeVar("_Self")
 
 
 class Node:
+    __slots__ = ["parent", "left", "right", "color", "heap_key", "tree_key"]
+
     NULL_NODE: _Self = None
+    PLACEHOLDER_VALUE: object = None
 
-    def __init__(self, heap_value: Any = None, tree_value: Any = None, placeholder: bool = False, color: int = 1) -> None:
+    def __init__(self, tree_key: Any, heap_key: Tuple[Any, Any], color: int = 1) -> None:
         self.parent: Optional[_Self] = None
         self.left: _Self = self.NULL_NODE
         self.right: _Self = self.NULL_NODE
-        self.placeholder: bool = placeholder
         self.color: int = color
-        self.heap_value: Any = heap_value
-        self.tree_value: Any = tree_value
+        self.tree_key: Any = tree_key
+        self.heap_key: Tuple[Any, Any] = heap_key
 
     def set_left(self, left_node: _Self) -> None:
         if left_node and left_node != self.NULL_NODE:
             left_node.parent = self
         self.left = left_node
 
     def set_right(self, right_node: _Self) -> None:
         if right_node and right_node != self.NULL_NODE:
             right_node.parent = self
         self.right = right_node
 
 
-Node.NULL_NODE = Node(color=0, placeholder=True)
+Node.PLACEHOLDER_VALUE = object()
+Node.NULL_NODE = Node(tree_key=Node.PLACEHOLDER_VALUE, heap_key=(Node.PLACEHOLDER_VALUE, Node.PLACEHOLDER_VALUE), color=0)
```

### Comparing `priority-search-tree-0.0.2/src/priority_search_tree.egg-info/PKG-INFO` & `priority-search-tree-0.1.0/src/priority_search_tree.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: priority-search-tree
-Version: 0.0.2
+Version: 0.1.0
 Summary: Priority search tree data structure
 Home-page: https://github.com/yusinv/priority-search-tree
 Author: Valentin Yusin
 Author-email: yusinv@gmail.com
 License: LGPL-3.0-or-later
 Project-URL: Documentation, https://priority-search-tree.readthedocs.io/
 Project-URL: Changelog, https://priority-search-tree.readthedocs.io/en/latest/changelog.html
@@ -33,34 +33,32 @@
 
 ========
 Overview
 ========
 
 
 
-The priority search tree (PST) is data structure with the following properties:
+The priority search tree (PST) is data structure (mutable mapping {**key**: **priority**}) with the following properties:
 
-* Items are stored in binary search tree (red-black tree in this case) using ``tree_key(value)``  function as a key.
-* Maintains max heap properties using ``heap_key(value)`` function as key.
-* Ability to perform efficient  *O(log(N)+K)* 3-sided search (finds items with ``tree_key`` in interval **[min_tree_key,max_tree_key]** and ``heap_key`` is grater or equal to **bottom_heap_key**).
+* Keys are stored in binary search tree (red-black tree in this case).
+* Maintains max heap properties (can return **key** with max **priority** in constant time).
+* Ability to perform efficient 3-sided search (finds items with **key** in interval `[min_tree_key,max_tree_key]` and **priority** is grater or equal to `bottom_priority`).
 
-For example PST can store 2 dimensional points P(X,Y) using X coordinate as ``tree_key`` and Y coordinate as ``heap_key``.  Such PST can perform 3 sided search to find points with X in [X_MIN,X_MAX] and Y >= Y_BOTTOM.
-
-Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
+For example PST can store 2 dimensional points `P(X,Y)` using X coordinate as **key** and Y coordinate as **priority**.  Such PST can perform 3 sided search to find points with `X in [X_MIN,X_MAX]` and `Y >= Y_BOTTOM`.
 
 Installation
 ============
 
 ::
 
     pip install priority-search-tree
 
 You can also install the in-development version with::
 
-    pip install https://github.com/yusinv/priority-search-tree/archive/main.zip
+    pip install https://github.com/yusinv/priority-search-tree/archive/develop.zip
 
 
 Documentation
 =============
 
 
 https://priority-search-tree.readthedocs.io/
@@ -70,14 +68,20 @@
 ===========
 
 To run all the tests run::
 
     tox
 
 
+Licence
+=======
+
+Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
+
+
 Changelog
 =========
 
 0.0.0 (2024-03-04)
 ------------------
 
 * First release on PyPI.
@@ -92,7 +96,15 @@
 0.0.2 (2024-03-26)
 ------------------
 
 * Added sorted_query method.
 * Added __len__ and __contains__ methods.
 * Added clear method.
 * Fixed issue with not unique heap keys
+
+
+0.1.0 (2024-04-08)
+------------------
+
+* Refactoring
+* Added PrioritySearchSet class
+* Added __iter__ method
```

### Comparing `priority-search-tree-0.0.2/src/priority_search_tree.egg-info/SOURCES.txt` & `priority-search-tree-0.1.0/src/priority_search_tree.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,35 +13,39 @@
 pytest.ini
 setup.py
 tox.ini
 .github/workflows/build.yml
 .github/workflows/publish.yml
 ci/bootstrap.py
 ci/requirements.txt
-ci/templates/.github/workflows/github-actions.yml
+ci/templates/.github/workflows/github-actions.yml.j2
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/index.rst
 docs/reference/priority_search_tree.rst
 docs/reference/priority_search_tree_print.rst
 src/priority_search_tree/__init__.py
-src/priority_search_tree/pst_node.py
-src/priority_search_tree/pst_print.py
+src/priority_search_tree/print_helpers.py
+src/priority_search_tree/ps_set.py
+src/priority_search_tree/ps_tree.py
+src/priority_search_tree/ps_tree_node.py
 src/priority_search_tree.egg-info/PKG-INFO
 src/priority_search_tree.egg-info/SOURCES.txt
 src/priority_search_tree.egg-info/dependency_links.txt
 src/priority_search_tree.egg-info/not-zip-safe
 src/priority_search_tree.egg-info/top_level.txt
 tests/data.py
-tests/stress.py
-tests/test_print.py
+tests/test_print_helpers.py
+tests/test_priority_search_set.py
 tests/test_priority_search_tree.py
 tests/test_pst_node.py
-tests/utils.py
+tests/utils.py
+tests/manual/performance.py
+tests/manual/stress.py
```

### Comparing `priority-search-tree-0.0.2/tests/test_pst_node.py` & `priority-search-tree-0.1.0/tests/test_pst_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from priority_search_tree import Node
+from priority_search_tree.ps_tree_node import Node
 
 
 def test_node_init():
-    node = Node(1, 2, False)
-    assert node.heap_value == 1
-    assert node.tree_value == 2
-    assert node.placeholder is False
+    node = Node(1, (2, 1))
+    assert node.tree_key == 1
+    assert node.heap_key == (2, 1)
     assert node.color == 1
 
 
 def test_node_set_left():
-    p_node: Node = Node(1, 1)
-    c_node: Node = Node(2, 2)
+    p_node: Node = Node(1, (4, 1))
+    c_node: Node = Node(2, (7, 2))
     p_node.set_left(c_node)
     assert p_node.left == c_node
     assert c_node.parent == p_node
     p_node.set_left(Node.NULL_NODE)
     assert p_node.left == Node.NULL_NODE
 
 
 def test_node_set_right():
-    p_node: Node = Node(1, 1)
-    c_node: Node = Node(2, 2)
+    p_node: Node = Node(1, (3, 1))
+    c_node: Node = Node(2, (5, 2))
     p_node.set_right(c_node)
     assert p_node.right == c_node
     assert c_node.parent == p_node
     p_node.set_right(Node.NULL_NODE)
     assert p_node.right == Node.NULL_NODE
```

### Comparing `priority-search-tree-0.0.2/tox.ini` & `priority-search-tree-0.1.0/tox.ini`

 * *Files identical despite different names*

