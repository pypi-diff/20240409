# Comparing `tmp/circuitpython-jepler-udecimal-1.0.10.tar.gz` & `tmp/circuitpython-jepler-udecimal-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-jepler-udecimal-1.0.10.tar", last modified: Tue Apr  9 19:05:27 2024, max compression
+gzip compressed data, was "circuitpython-jepler-udecimal-1.0.9.tar", last modified: Tue Oct  3 15:44:05 2023, max compression
```

## Comparing `circuitpython-jepler-udecimal-1.0.10.tar` & `circuitpython-jepler-udecimal-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.212314 circuitpython-jepler-udecimal-1.0.10/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.212314 circuitpython-jepler-udecimal-1.0.10/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.216314 circuitpython-jepler-udecimal-1.0.10/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.216314 circuitpython-jepler-udecimal-1.0.10/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (127)     1814 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-09 19:05:27.000000 circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 19:05:27.000000 circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:05:27.000000 circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 19:05:27.000000 circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.216314 circuitpython-jepler-udecimal-1.0.10/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.216314 circuitpython-jepler-udecimal-1.0.10/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/api.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.212314 circuitpython-jepler-udecimal-1.0.10/docs/autoapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.212314 circuitpython-jepler-udecimal-1.0.10/docs/autoapi/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/docs/autoapi/templates/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/autoapi/templates/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/autoapi/templates/python/module.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/examples/test_udecimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/examples/udecimal_moneyfmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/examples/udecimal_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/
--rw-r--r--   0 runner    (1001) docker     (127)   186127 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-09 19:05:27.000000 circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/utrig.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-09 19:05:24.000000 circuitpython-jepler-udecimal-1.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 19:05:18.000000 circuitpython-jepler-udecimal-1.0.10/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:05:27.220314 circuitpython-jepler-udecimal-1.0.10/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.529153 circuitpython-jepler-udecimal-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.517153 circuitpython-jepler-udecimal-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.521153 circuitpython-jepler-udecimal-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.521153 circuitpython-jepler-udecimal-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.521153 circuitpython-jepler-udecimal-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1814 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.521153 circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-10-03 15:44:05.000000 circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-10-03 15:44:05.000000 circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-03 15:44:05.000000 circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-03 15:44:05.000000 circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/api.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.517153 circuitpython-jepler-udecimal-1.0.9/docs/autoapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.517153 circuitpython-jepler-udecimal-1.0.9/docs/autoapi/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/docs/autoapi/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/autoapi/templates/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/autoapi/templates/python/module.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/examples/test_udecimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/examples/udecimal_moneyfmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/examples/udecimal_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-03 15:44:05.525153 circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/
+-rw-r--r--   0 runner    (1001) docker     (127)   186127 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2023-10-03 15:44:05.000000 circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/utrig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-10-03 15:43:55.000000 circuitpython-jepler-udecimal-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-03 15:43:43.000000 circuitpython-jepler-udecimal-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-03 15:44:05.529153 circuitpython-jepler-udecimal-1.0.9/setup.cfg
```

### Comparing `circuitpython-jepler-udecimal-1.0.10/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-jepler-udecimal-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/.github/workflows/release_gh.yml` & `circuitpython-jepler-udecimal-1.0.9/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/.pre-commit-config.yaml` & `circuitpython-jepler-udecimal-1.0.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
 -   repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 23.9.1
     hooks:
     - id: black
 -   repo: https://github.com/fsfe/reuse-tool
-    rev: v3.0.2
+    rev: v2.1.0
     hooks:
     - id: reuse
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.6.0
+    rev: v4.4.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/pylint
-    rev: v3.1.0
+    rev: v3.0.0
     hooks:
     -   id: pylint
         name: lint (examples)
         types: [python]
         files: ^examples/
         args:
         - --disable=missing-docstring,invalid-name,bad-whitespace
```

### Comparing `circuitpython-jepler-udecimal-1.0.10/.pylintrc` & `circuitpython-jepler-udecimal-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/CODE_OF_CONDUCT.md` & `circuitpython-jepler-udecimal-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSE` & `circuitpython-jepler-udecimal-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/Apache-2.0.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/BSD-2-Clause.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/CC-BY-4.0.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/MIT.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/Python-2.0.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/LICENSES/Unlicense.txt` & `circuitpython-jepler-udecimal-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/PKG-INFO` & `circuitpython-jepler-udecimal-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-jepler-udecimal
-Version: 1.0.10
+Version: 1.0.9
 Summary: Reduced version of the decimal library for CircuitPython
 Author-email: Jeff Epler <jepler@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/jepler/Jepler_CircuitPython_udecimal
 Project-URL: Documentation, https://jepler-udecimal.readthedocs.io/en/latest/api/jepler_udecimal/index.html
 Project-URL: Tracker, https://github.com/jepler/Jepler_CircuitPython_udecimal/issues
 Keywords: adafruit,blinka,circuitpython,micropython,udecimal,numeric,helper,arbitraryprecision,math
```

### Comparing `circuitpython-jepler-udecimal-1.0.10/README.rst` & `circuitpython-jepler-udecimal-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/build.sh` & `circuitpython-jepler-udecimal-1.0.9/build.sh`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/PKG-INFO` & `circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-jepler-udecimal
-Version: 1.0.10
+Version: 1.0.9
 Summary: Reduced version of the decimal library for CircuitPython
 Author-email: Jeff Epler <jepler@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/jepler/Jepler_CircuitPython_udecimal
 Project-URL: Documentation, https://jepler-udecimal.readthedocs.io/en/latest/api/jepler_udecimal/index.html
 Project-URL: Tracker, https://github.com/jepler/Jepler_CircuitPython_udecimal/issues
 Keywords: adafruit,blinka,circuitpython,micropython,udecimal,numeric,helper,arbitraryprecision,math
```

### Comparing `circuitpython-jepler-udecimal-1.0.10/circuitpython_jepler_udecimal.egg-info/SOURCES.txt` & `circuitpython-jepler-udecimal-1.0.9/circuitpython_jepler_udecimal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/docs/_static/favicon.ico` & `circuitpython-jepler-udecimal-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/docs/autoapi/templates/python/module.rst` & `circuitpython-jepler-udecimal-1.0.9/docs/autoapi/templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/docs/conf.py` & `circuitpython-jepler-udecimal-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/docs/index.rst` & `circuitpython-jepler-udecimal-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/examples/test_udecimal.py` & `circuitpython-jepler-udecimal-1.0.9/examples/test_udecimal.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/examples/udecimal_moneyfmt.py` & `circuitpython-jepler-udecimal-1.0.9/examples/udecimal_moneyfmt.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/examples/udecimal_simpletest.py` & `circuitpython-jepler-udecimal-1.0.9/examples/udecimal_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/__init__.py` & `circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/__init__.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/test.py` & `circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/test.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/jepler_udecimal/utrig.py` & `circuitpython-jepler-udecimal-1.0.9/jepler_udecimal/utrig.py`

 * *Files identical despite different names*

### Comparing `circuitpython-jepler-udecimal-1.0.10/pyproject.toml` & `circuitpython-jepler-udecimal-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-jepler-udecimal"
 description = "Reduced version of the decimal library for CircuitPython"
-version = "1.0.10"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Jeff Epler", email = "jepler@gmail.com"}
 ]
 urls = { Source = "https://github.com/jepler/Jepler_CircuitPython_udecimal", Documentation = "https://jepler-udecimal.readthedocs.io/en/latest/api/jepler_udecimal/index.html", Tracker = "https://github.com/jepler/Jepler_CircuitPython_udecimal/issues" }
 #    "Pull Requests" = "https://github.com/jepler/Jepler_CircuitPython_udecimal/pulls",
 keywords = [
```

