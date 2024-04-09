# Comparing `tmp/galcheat-1.0.0.tar.gz` & `tmp/galcheat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galcheat-1.0.0.tar", last modified: Fri May  6 14:08:33 2022, max compression
+gzip compressed data, was "dist/galcheat-1.1.0.tar", last modified: Tue Apr  9 17:46:02 2024, max compression
```

## Comparing `galcheat-1.0.0.tar` & `galcheat-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2128 2022-05-06 14:08:25.000000 galcheat-1.0.0/.all-contributorsrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-06 14:08:25.000000 galcheat-1.0.0/.github/workflows/check_style.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-05-06 14:08:25.000000 galcheat-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-05-06 14:08:25.000000 galcheat-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-05-06 14:08:25.000000 galcheat-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-05-06 14:08:25.000000 galcheat-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3097 2022-05-06 14:08:25.000000 galcheat-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-05-06 14:08:25.000000 galcheat-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8330 2022-05-06 14:08:33.000000 galcheat-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6588 2022-05-06 14:08:25.000000 galcheat-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/api/filter.md
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/api/helpers.md
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/api/survey.md
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/api/utilities.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/guides/create-galaxy.md
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/guides/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/guides/heritage.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)   159096 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/images/galaxy.png
--rw-r--r--   0 runner    (1001) docker     (121)    89915 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/images/galcheat_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     8870 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/parameters.md
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-06 14:08:25.000000 galcheat-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/CFHTLS.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/COSMOS.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2153 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/DES.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/Euclid_VIS.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/HSC.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2727 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/data/LSST.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/survey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-05-06 14:08:25.000000 galcheat-1.0.0/galcheat/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8330 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-06 14:08:33.000000 galcheat-1.0.0/galcheat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-05-06 14:08:25.000000 galcheat-1.0.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-05-06 14:08:25.000000 galcheat-1.0.0/scripts/check_effective_wavelengths.py
--rw-r--r--   0 runner    (1001) docker     (121)     2071 2022-05-06 14:08:25.000000 galcheat-1.0.0/scripts/check_zeropoints.py
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-06 14:08:25.000000 galcheat-1.0.0/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-05-06 14:08:33.000000 galcheat-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-05-06 14:08:25.000000 galcheat-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-06 14:08:33.000000 galcheat-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-05-06 14:08:25.000000 galcheat-1.0.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-09 17:45:52.000000 galcheat-1.1.0/.all-contributorsrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/check_style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 17:45:52.000000 galcheat-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-09 17:45:52.000000 galcheat-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-09 17:45:52.000000 galcheat-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 17:45:52.000000 galcheat-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 17:45:52.000000 galcheat-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-09 17:46:02.000000 galcheat-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-04-09 17:45:52.000000 galcheat-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/helpers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/survey.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/api/utilities.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/create-galaxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/guides/heritage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   159096 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/images/galaxy.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89915 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/images/galcheat_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/parameters.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 17:45:52.000000 galcheat-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/CFHTLS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/COSMOS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/DES.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/Euclid_VIS.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/HSC.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/data/LSST.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/rich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 17:45:52.000000 galcheat-1.1.0/galcheat/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-09 17:46:02.000000 galcheat-1.1.0/galcheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:46:01.000000 galcheat-1.1.0/galcheat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-09 17:45:52.000000 galcheat-1.1.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/check_effective_wavelengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/check_zeropoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:45:52.000000 galcheat-1.1.0/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 17:46:02.000000 galcheat-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-09 17:45:52.000000 galcheat-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:46:02.000000 galcheat-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-09 17:45:52.000000 galcheat-1.1.0/tests/test_utilities.py
```

### Comparing `galcheat-1.0.0/.all-contributorsrc` & `galcheat-1.1.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/.github/workflows/python-package.yml` & `galcheat-1.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/.github/workflows/python-publish.yml` & `galcheat-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/.gitignore` & `galcheat-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/.pre-commit-config.yaml` & `galcheat-1.1.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.2.0
+  rev: v4.6.0
   hooks:
     - id: check-merge-conflict
     - id: check-yaml
     - id: debug-statements
     - id: end-of-file-fixer
     - id: no-commit-to-branch
       args: [--branch, main]
     - id: requirements-txt-fixer
     - id: trailing-whitespace
       args: [--markdown-linebreak-ext=md]
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.13.2
   hooks:
     - id: isort
       args: [--profile, black]
 - repo: https://github.com/asottile/pyupgrade
-  rev: v2.31.1
+  rev: v3.15.2
   hooks:
     - id: pyupgrade
       args: [--py37-plus]
 - repo: https://github.com/PyCQA/flake8
-  rev: 4.0.1
+  rev: 7.0.0
   hooks:
    - id: flake8
-     additional_dependencies: [flake8-typing-imports==1.7.0]
      args: ['--ignore=E501,E203,E731,W503']
 - repo: https://github.com/psf/black
-  rev: 22.3.0
+  rev: 24.3.0
   hooks:
     - id: black
```

### Comparing `galcheat-1.0.0/CONTRIBUTING.md` & `galcheat-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/LICENSE` & `galcheat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/PKG-INFO` & `galcheat-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galcheat
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tiny library of galaxy surveys most useful parameters with units
 Home-page: https://github.com/aboucaud/galcheat
 Author: Alexandre Boucaud
 Author-email: aboucaud@apc.in2p3.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aboucaud/galcheat/issues
 Description: [**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
@@ -48,21 +48,23 @@
         ```sh
         galcheat
         ```
         
         ### Options
         - **`-s <survey>`**: print information for a given survey
         - **`--refs`**: print the source for each parameter
+        - **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
         - **`-h, --help`**: get help
         
         ### Examples
         ```sh
-        galcheat -s LSST        # LSST info
-        galcheat --refs         # all surveys info with refs
-        galcheat --refs -s HSC  # HSC info with refs
+        galcheat -s LSST         # LSST info
+        galcheat --refs          # all surveys info with refs
+        galcheat --refs -s HSC   # HSC info with refs
+        galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
         ```
         
         API
         ---
         ```python
         import galcheat
```

### Comparing `galcheat-1.0.0/README.md` & `galcheat-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,21 +39,23 @@
 ```sh
 galcheat
 ```
 
 ### Options
 - **`-s <survey>`**: print information for a given survey
 - **`--refs`**: print the source for each parameter
+- **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
 - **`-h, --help`**: get help
 
 ### Examples
 ```sh
-galcheat -s LSST        # LSST info
-galcheat --refs         # all surveys info with refs
-galcheat --refs -s HSC  # HSC info with refs
+galcheat -s LSST         # LSST info
+galcheat --refs          # all surveys info with refs
+galcheat --refs -s HSC   # HSC info with refs
+galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
 ```
 
 API
 ---
 ```python
 import galcheat
```

#### html2text {}

```diff
@@ -18,18 +18,20 @@
 information tends to be scattered in many places or is often copy/pasted
 without all of the relevant information like units or sources. The current
 parameters and the corresponding units are specified in the [documentation]
 (https://aboucaud.github.io/galcheat/parameters.html) Getting started ---------
 ------ Install the latest version of the library ```sh pip install -U galcheat
 ``` CLI --- Print the available surveys and associated filters ```sh galcheat
 ``` ### Options - **`-s `**: print information for a given survey - **`--
-refs`**: print the source for each parameter - **`-h, --help`**: get help ###
-Examples ```sh galcheat -s LSST # LSST info galcheat --refs # all surveys info
-with refs galcheat --refs -s HSC # HSC info with refs ``` API --- ```python
-import galcheat # Start with the list of available surveys
+refs`**: print the source for each parameter - **`--rich`**: use pretty
+printing for the terminal (needs the `rich` library installed) - **`-h, --
+help`**: get help ### Examples ```sh galcheat -s LSST # LSST info galcheat --
+refs # all surveys info with refs galcheat --refs -s HSC # HSC info with refs
+galcheat -s LSST --rich # pretty print rich terminal output for LSST info ```
+API --- ```python import galcheat # Start with the list of available surveys
 galcheat.available_surveys # Retrieve a Survey instance LSST =
 galcheat.get_survey("LSST") # List the available survey filters
 LSST.available_filters # Pick a Filter instance u_band = LSST.get_filter("u") #
 Both Survey and Filter objects have physical attributes LSST.mirror_diameter
 u_band.full_exposure_time # These attributes are Astropy Quantity objects #
 whose value can be retrieved in any desired unit u_band.psf_fwhm.to_value
 ('arcmin') ``` ## Contributing â¨ This project was started in the context of
```

### Comparing `galcheat-1.0.0/docs/guides/create-galaxy.md` & `galcheat-1.1.0/docs/guides/create-galaxy.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/docs/guides/getting-started.md` & `galcheat-1.1.0/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/docs/guides/heritage.md` & `galcheat-1.1.0/docs/guides/heritage.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/docs/images/galaxy.png` & `galcheat-1.1.0/docs/images/galaxy.png`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/docs/images/galcheat_logo.png` & `galcheat-1.1.0/docs/images/galcheat_logo.png`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/docs/index.md` & `galcheat-1.1.0/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 galcheat
 ```
 
 ### Options
 
 - **`-s <survey>`**: print information for a given survey
 - **`--refs`**: print the source for each parameter
+- **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
 - **`-h, --help`**: get help
 
 ### Examples
 
 ```sh
-galcheat -s LSST        # LSST info
-galcheat --refs         # all surveys info with refs
-galcheat --refs -s HSC  # HSC info with refs
+galcheat -s LSST         # LSST info
+galcheat --refs          # all surveys info with refs
+galcheat --refs -s HSC   # HSC info with refs
+galcheat -s LSST --rich  # pretty print rich terminal output for LSST survey info
 ```
 
 ## Installation
 
 ```sh
 python -m pip install -U galcheat
 ```
@@ -45,7 +47,15 @@
 ### Developers
 
 The developer tools needed to perform tests and linting and compile the docs locally can be installed with
 
 ```sh
 python -m pip install -U galcheat[dev]
 ```
+
+### Rich display (new in v1.1)
+
+For a better terminal experience, install the `rich` library and use it together with the `--rich` option from `galcheat`
+
+```sh
+python -m pip install rich
+```
```

### Comparing `galcheat-1.0.0/docs/parameters.md` & `galcheat-1.1.0/docs/parameters.md`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/__init__.py` & `galcheat-1.1.0/galcheat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,9 @@
     0.014316666666666667
 
 Feel free to contribute by submitting
 parameter values for your surveys of
 interest or reporting inconsistent values.
 
 """
+
 from galcheat.helpers import available_surveys, get_survey  # noqa
```

### Comparing `galcheat-1.0.0/galcheat/data/CFHTLS.yaml` & `galcheat-1.1.0/galcheat/data/CFHTLS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/data/COSMOS.yaml` & `galcheat-1.1.0/galcheat/data/COSMOS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/data/DES.yaml` & `galcheat-1.1.0/galcheat/data/DES.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/data/Euclid_VIS.yaml` & `galcheat-1.1.0/galcheat/data/Euclid_VIS.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/data/HSC.yaml` & `galcheat-1.1.0/galcheat/data/HSC.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/data/LSST.yaml` & `galcheat-1.1.0/galcheat/data/LSST.yaml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/filter.py` & `galcheat-1.1.0/galcheat/filter.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/helpers.py` & `galcheat-1.1.0/galcheat/helpers.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/survey.py` & `galcheat-1.1.0/galcheat/survey.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat/utilities.py` & `galcheat-1.1.0/galcheat/utilities.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/galcheat.egg-info/PKG-INFO` & `galcheat-1.1.0/galcheat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galcheat
-Version: 1.0.0
+Version: 1.1.0
 Summary: Tiny library of galaxy surveys most useful parameters with units
 Home-page: https://github.com/aboucaud/galcheat
 Author: Alexandre Boucaud
 Author-email: aboucaud@apc.in2p3.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aboucaud/galcheat/issues
 Description: [**Main documentation**](https://aboucaud.github.io/galcheat/) | [**Getting started**](#getting-started) | [**CLI**](#cli) | [**API**](#api) | [**Contributing**](#contributing) | [**License**](#license)
@@ -48,21 +48,23 @@
         ```sh
         galcheat
         ```
         
         ### Options
         - **`-s <survey>`**: print information for a given survey
         - **`--refs`**: print the source for each parameter
+        - **`--rich`**: use pretty printing for the terminal (needs the `rich` library installed)
         - **`-h, --help`**: get help
         
         ### Examples
         ```sh
-        galcheat -s LSST        # LSST info
-        galcheat --refs         # all surveys info with refs
-        galcheat --refs -s HSC  # HSC info with refs
+        galcheat -s LSST         # LSST info
+        galcheat --refs          # all surveys info with refs
+        galcheat --refs -s HSC   # HSC info with refs
+        galcheat -s LSST --rich  # pretty print rich terminal output for LSST info
         ```
         
         API
         ---
         ```python
         import galcheat
```

### Comparing `galcheat-1.0.0/galcheat.egg-info/SOURCES.txt` & `galcheat-1.1.0/galcheat.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/guides/heritage.md
 docs/images/galaxy.png
 docs/images/galcheat_logo.png
 galcheat/__init__.py
 galcheat/__main__.py
 galcheat/filter.py
 galcheat/helpers.py
+galcheat/rich.py
 galcheat/survey.py
 galcheat/utilities.py
 galcheat.egg-info/PKG-INFO
 galcheat.egg-info/SOURCES.txt
 galcheat.egg-info/dependency_links.txt
 galcheat.egg-info/entry_points.txt
 galcheat.egg-info/not-zip-safe
```

### Comparing `galcheat-1.0.0/mkdocs.yml` & `galcheat-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/scripts/check_effective_wavelengths.py` & `galcheat-1.1.0/scripts/check_effective_wavelengths.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/scripts/check_zeropoints.py` & `galcheat-1.1.0/scripts/check_zeropoints.py`

 * *Files identical despite different names*

### Comparing `galcheat-1.0.0/setup.cfg` & `galcheat-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 	pytest>=6.0
 	pytest-cov>=3.0
 	pytest_astropy_header>=0.2
 	mkdocs>=1.2
 	mkdocs-material>=8.2
 	mkdocstrings>=0.18
 	pytkdocs[numpy-style]>=0.16
+	rich>=13.7
 scripts = 
 	speclite>=0.15
 
 [options.package_data]
 galcheat = data/*
 
 [bdist_wheel]
```

### Comparing `galcheat-1.0.0/tests/test_utilities.py` & `galcheat-1.1.0/tests/test_utilities.py`

 * *Files identical despite different names*

