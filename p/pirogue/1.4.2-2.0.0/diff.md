# Comparing `tmp/pirogue-1.4.2.tar.gz` & `tmp/pirogue-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pirogue-1.4.2.tar", last modified: Wed Oct 25 12:21:10 2023, max compression
+gzip compressed data, was "pirogue-2.0.0.tar", last modified: Tue Apr  9 05:29:39 2024, max compression
```

## Comparing `pirogue-1.4.2.tar` & `pirogue-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.817330 pirogue-1.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.809331 pirogue-1.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-25 12:20:51.000000 pirogue-1.4.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.809331 pirogue-1.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-25 12:20:51.000000 pirogue-1.4.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-10-25 12:20:51.000000 pirogue-1.4.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-10-25 12:20:51.000000 pirogue-1.4.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-10-25 12:20:51.000000 pirogue-1.4.2/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-10-25 12:20:51.000000 pirogue-1.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-10-25 12:20:51.000000 pirogue-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-10-25 12:21:10.817330 pirogue-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-25 12:20:51.000000 pirogue-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.813331 pirogue-1.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-10-25 12:20:51.000000 pirogue-1.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2023-10-25 12:20:51.000000 pirogue-1.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-25 12:20:51.000000 pirogue-1.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-25 12:20:51.000000 pirogue-1.4.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.813331 pirogue-1.4.2/pirogue/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/information_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26707 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/simple_joins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/single_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18328 2023-10-25 12:20:51.000000 pirogue-1.4.2/pirogue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.813331 pirogue-1.4.2/pirogue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-25 12:21:10.000000 pirogue-1.4.2/pirogue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-10-25 12:20:51.000000 pirogue-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-25 12:20:51.000000 pirogue-1.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-25 12:20:51.000000 pirogue-1.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.813331 pirogue-1.4.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 12:20:51.000000 pirogue-1.4.2/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4652 2023-10-25 12:20:51.000000 pirogue-1.4.2/scripts/pirogue.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 12:21:10.817330 pirogue-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-10-25 12:20:51.000000 pirogue-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 12:21:10.813331 pirogue-1.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/demo_data.sql
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/multiple_inheritance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/simple_joins.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/simple_joins_based_on_view.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/test_multiple_inheritance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/test_simple_inheritance.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-10-25 12:20:51.000000 pirogue-1.4.2/test/test_simple_joins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.180911 pirogue-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.176911 pirogue-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 05:29:26.000000 pirogue-2.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.176911 pirogue-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-09 05:29:26.000000 pirogue-2.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 05:29:26.000000 pirogue-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 05:29:26.000000 pirogue-2.0.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 05:29:26.000000 pirogue-2.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 05:29:26.000000 pirogue-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 05:29:26.000000 pirogue-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-09 05:29:26.000000 pirogue-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 05:29:39.180911 pirogue-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 05:29:26.000000 pirogue-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.176911 pirogue-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 05:29:26.000000 pirogue-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-09 05:29:26.000000 pirogue-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 05:29:26.000000 pirogue-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 05:29:26.000000 pirogue-2.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.176911 pirogue-2.0.0/pirogue/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4482 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/information_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24940 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/simple_joins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/single_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-09 05:29:26.000000 pirogue-2.0.0/pirogue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.180911 pirogue-2.0.0/pirogue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 05:29:39.000000 pirogue-2.0.0/pirogue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 05:29:26.000000 pirogue-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:29:26.000000 pirogue-2.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 05:29:26.000000 pirogue-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:29:39.180911 pirogue-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:39.180911 pirogue-2.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/demo_data.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/multiple_inheritance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/simple_joins.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/simple_joins_based_on_view.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/test_multiple_inheritance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/test_simple_inheritance.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 05:29:26.000000 pirogue-2.0.0/test/test_simple_joins.py
```

### Comparing `pirogue-1.4.2/.github/workflows/docs.yml` & `pirogue-2.0.0/.github/workflows/docs.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 name: Build and deploy docs
 
 
 on:
-  push:
-    branches:
-      - master
+  release:
 
 jobs:
   docs:
     name: Deploy documentation
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/heads/master')
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
 
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+    - name: Set up Python
+      uses: actions/setup-python@v5
       with:
-        python-version: 3.8
+        python-version: 3.9
 
     - name: Install requirements
       run: |
         pip install -r requirements.txt
         pip install -r docs/requirements.txt
 
     - name: Cache pip
-      uses: actions/cache@v2
+      uses: actions/cache@v4
       with:
         path: ~/.cache/pip
         key: pip-${{ hashFiles('requirements.txt') }}-${{ hashFiles('docs/requirements.txt') }}
         restore-keys: |
           pip-${{ hashFiles('requirements.txt') }}
           pip-
 
     - name: Setup pirogue
       run: |
-        VERSION=${GITHUB_REF:-0.0.0}
-        VERSION=${VERSION##*/}
-        sed -i "s/__VERSION__/${VERSION}/g" setup.py
-        python setup.py install
+        python -m pip install -e .
         pirogue -v
 
     - name: Build docs
       run: |
         VERSION=${GITHUB_REF:-0.0.0}
         export VERSION=${VERSION##*/}
         cd docs
         sed -i "s/__VERSION__/${VERSION}/" conf.py
         make html
 
     - name: Deploy to GitHub Pages
       run: |
         python -m pip install ghp-import
-        ghp-import --force --no-jekyll --push docs/_build/html
+        ghp-import --force --no-jekyll --push docs/_build/html
```

### Comparing `pirogue-1.4.2/.github/workflows/release.yml` & `pirogue-2.0.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,21 @@
     name: "Release on tag 🚀"
     runs-on: ubuntu-latest
     needs: [build-python-wheel, tests]
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
 
     steps:
       - name: Retrieve artifact from Python build
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python_wheel
           path: dist/
 
       - name: Create/update release on GitHub
-        uses: ncipollo/release-action@v1.13.0
+        uses: ncipollo/release-action@v1.14.0
         with:
           allowUpdates: true
           artifacts: "builds**/*"
           generateReleaseNotes: true
           omitNameDuringUpdate: true
           token: ${{ secrets.GITHUB_TOKEN }}
 
@@ -49,28 +49,28 @@
     name: "🐍 Release on PyPI"
     runs-on: ubuntu-latest
     needs: [build-python-wheel, tests]
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags/')
 
     steps:
       - name: Retrieve artifact from Python build
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: python_wheel
           path: dist/
 
       # -- FROM HERE, A TAG IS REQUIRED ---
       - name: Deploy to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
 
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
       - name: Create/update release on GitHub
-        uses: ncipollo/release-action@v1.13.0
+        uses: ncipollo/release-action@v1.14.0
         with:
           allowUpdates: true
           artifacts: "dist/*.tar.gz"
           generateReleaseNotes: true
           omitNameDuringUpdate: true
-          token: ${{ secrets.GITHUB_TOKEN }}
+          token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pirogue-1.4.2/.github/workflows/test.yml` & `pirogue-2.0.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
       PGUSER: postgres
 
     steps:
       - name: Get source code
         uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.8"
+          python-version: "3.9"
           cache: "pip"
           cache-dependency-path: "requirements*.txt"
 
       - name: Install requirements
         run: |
           pip install -r requirements.txt
           pip install -r requirements-test.txt
@@ -69,9 +69,7 @@
           PGSERVICE=pirogue_test psql --quiet -v ON_ERROR_STOP=on -f test/demo_data.sql
 
       - name: Run bash tests
         run: ./test/test_simple_inheritance.sh
 
       - name: Run Python tests
         run: nose2 -v
-
-
```

### Comparing `pirogue-1.4.2/.github/workflows/wheel.yml` & `pirogue-2.0.0/.github/workflows/wheel.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   tests:
     runs-on: ubuntu-latest
     steps:
       - name: Get source code
         uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.9"
           cache: "pip"
           cache-dependency-path: "requirements*.txt"
 
       - name: Install project requirements
         run: |
@@ -33,12 +33,12 @@
       - name: Install project as a package
         run: python -m pip install -e .
 
       - name: Build a binary wheel and a source tarball
         run: >-
           python -m build --sdist --wheel --outdir dist/ .
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: python_wheel
           path: dist/*
           if-no-files-found: error
```

### Comparing `pirogue-1.4.2/LICENSE` & `pirogue-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pirogue-1.4.2/PKG-INFO` & `pirogue-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.1
 Name: pirogue
-Version: 1.4.2
+Version: 2.0.0
 Summary: pirogue let you dynamically and easily create views in PostgreSQL for inheritance or join scenarios.
-Home-page: https://github.com/opengisch/pirogue
-Download-URL: https://github.com/opengisch/pirogue/archive/__VERSION__.tar.gz
-Author: Denis Rouzaud
 Author-email: Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pirogue/
 Project-URL: repository, https://github.com/opengisch/pirogue
 Project-URL: tracker, https://github.com/opengisch/pirogue/issues
 Keywords: postgres
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psycopg2-binary
-Requires-Dist: pyyaml
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: psycopg>=3.1.18
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
 
 # pirogue
 A tool to automatically create views and triggers on PostgreSQL databases
 
 Read the docs: https://opengisch.github.io/pirogue
-
-
```

### Comparing `pirogue-1.4.2/docs/Makefile` & `pirogue-2.0.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `pirogue-1.4.2/docs/conf.py` & `pirogue-2.0.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
@@ -10,97 +9,98 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
-sys.path.insert(0, os.path.abspath('..'))
+
+sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
-project = 'pirogue'
-copyright = '2019-2021, Denis Rouzaud'
-author = 'Denis Rouzaud'
+project = "pirogue"
+copyright = "2019-2021, Denis Rouzaud"
+author = "Denis Rouzaud"
 
 # The short X.Y version
-version = '__VERSION__'
+version = "__VERSION__"
 # The full version, including alpha/beta/rc tags
-release = '__VERSION__'
+release = "__VERSION__"
 
 
 # -- General configuration ---------------------------------------------------
 
 autoclass_content = "class"
 autodoc_default_flags = [
-         "members",
-         "show-inheritance",
+    "members",
+    "show-inheritance",
 ]
 autosummary_generate = True  # Make _autosummary files and include them
 napoleon_numpy_docstring = True  # Force consistency, leave only Google
 napoleon_use_rtype = False  # More legible
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.coverage',
-    'sphinx.ext.viewcode',
-    'sphinx.ext.githubpages',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.autosummary'
+    "sphinx.ext.autodoc",
+    "sphinx.ext.coverage",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.githubpages",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autosummary",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = None
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # The default sidebars (for documents that don't match any pattern) are
 # defined by theme itself.  Builtin themes are using these templates by
 # default: ``['localtoc.html', 'relations.html', 'sourcelink.html',
@@ -108,65 +108,64 @@
 #
 # html_sidebars = {}
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'piroguedoc'
+htmlhelp_basename = "piroguedoc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'pirogue.tex', 'pirogue Documentation',
-     'Denis Rouzaud', 'manual'),
+    (master_doc, "pirogue.tex", "pirogue Documentation", "Denis Rouzaud", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'pirogue', 'pirogue Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "pirogue", "pirogue Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'pirogue', 'pirogue Documentation',
-     author, 'pirogue', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "pirogue",
+        "pirogue Documentation",
+        author,
+        "pirogue",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
 epub_title = project
@@ -177,11 +176,11 @@
 # epub_identifier = ''
 
 # A unique identification for the text.
 #
 # epub_uid = ''
 
 # A list of files that should not be packed into the epub file.
-epub_exclude_files = ['search.html']
+epub_exclude_files = ["search.html"]
 
 
 # -- Extension configuration -------------------------------------------------
```

### Comparing `pirogue-1.4.2/docs/index.rst` & `pirogue-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pirogue-1.4.2/pirogue/information_schema.py` & `pirogue-2.0.0/pirogue/information_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-# -*- coding: utf-8 -*-
-from pirogue.exceptions import TableHasNoPrimaryKey, NoReferenceFound, InvalidSkipColumns
-from psycopg2.extensions import cursor
+from psycopg import Cursor
 
+from pirogue.exceptions import (
+    InvalidSkipColumns,
+    NoReferenceFound,
+    TableHasNoPrimaryKey,
+)
 
-def primary_key(pg_cur: cursor, schema_name: str, table_name: str) -> str:
+
+def primary_key(pg_cur: Cursor, schema_name: str, table_name: str) -> str:
     """
     Returns the primary of a table
 
     Parameters
     ----------
     pg_cur
         psycopg cursor
     schema_name
         the schema name
     table_name
         the table name
     """
-    sql = "SELECT c.column_name"\
-          " FROM information_schema.key_column_usage AS c "\
-          " LEFT JOIN information_schema.table_constraints AS t"\
-          " ON t.constraint_name = c.constraint_name"\
-          " WHERE t.table_name = '{t}'"\
-          " AND t.table_schema = '{s}'"\
-          " AND t.constraint_type = 'PRIMARY KEY'".format(s=schema_name, t=table_name)
+    sql = (
+        "SELECT c.column_name"
+        " FROM information_schema.key_column_usage AS c "
+        " LEFT JOIN information_schema.table_constraints AS t"
+        " ON t.constraint_name = c.constraint_name"
+        " WHERE t.table_name = '{t}'"
+        " AND t.table_schema = '{s}'"
+        " AND t.constraint_type = 'PRIMARY KEY'".format(s=schema_name, t=table_name)
+    )
     pg_cur.execute(sql)
     try:
         pkey = pg_cur.fetchone()[0]
     except Exception:
         raise TableHasNoPrimaryKey(sql)
     return pkey
 
 
-def columns(pg_cur: cursor, table_schema: str, table_name: str, table_type: str = 'table',
-            remove_pkey: bool=False, skip_columns: list=[]) -> list:
+def columns(
+    pg_cur: Cursor,
+    table_schema: str,
+    table_name: str,
+    table_type: str = "table",
+    remove_pkey: bool = False,
+    skip_columns: list = [],
+) -> list:
     """
     Returns the list of columns of a table
 
     Parameters
     ----------
     pg_cur
         psycopg cursor
@@ -47,52 +59,63 @@
     table_type
         the type of table, i.e. view or table
     remove_pkey
         if True, the primary key is dropped
     skip_columns
         list of columns to be skipped
     """
-    assert table_type.lower() in ('table', 'view')
-    if table_type.lower() == 'table':
+    assert table_type.lower() in ("table", "view")
+    if table_type.lower() == "table":
         sql = """SELECT attname
-                    FROM pg_attribute 
+                    FROM pg_attribute
                     WHERE attrelid = '{s}.{t}'::regclass
-                    AND attisdropped IS NOT TRUE 
-                    AND attnum > 0 
-                    ORDER BY attnum ASC""".format(s=table_schema, t=table_name)
+                    AND attisdropped IS NOT TRUE
+                    AND attnum > 0
+                    ORDER BY attnum ASC""".format(
+            s=table_schema, t=table_name
+        )
     else:
         sql = """
             SELECT c.column_name
                 FROM information_schema.tables t
                     LEFT JOIN information_schema.columns c
                               ON t.table_schema = c.table_schema
                               AND t.table_name = c.table_name
                 WHERE table_type = 'VIEW'
                       AND t.table_schema = '{s}'
                       AND t.table_name = '{t}'
-                ORDER BY ordinal_position""".format(s=table_schema, t=table_name)
+                ORDER BY ordinal_position""".format(
+            s=table_schema, t=table_name
+        )
 
     pg_cur.execute(sql)
     pg_fields = pg_cur.fetchall()
     pg_fields = [field[0] for field in pg_fields if field[0]]
     for col in skip_columns:
         try:
             pg_fields.remove(col)
         except ValueError:
-            raise InvalidSkipColumns('Cannot skip unexisting column "{col}" in "{s}.{t}"'.format(col=col, s=table_schema,
-                                                                                                 t=table_name))
+            raise InvalidSkipColumns(
+                'Cannot skip unexisting column "{col}" in "{s}.{t}"'.format(
+                    col=col, s=table_schema, t=table_name
+                )
+            )
     if remove_pkey:
         pkey = primary_key(pg_cur, table_schema, table_name)
         pg_fields.remove(pkey)
     return pg_fields
 
 
-def reference_columns(pg_cur: cursor,
-                      table_schema: str, table_name: str,
-                      foreign_table_schema: str, foreign_table_name: str) -> (str, str):
+def reference_columns(
+    pg_cur: Cursor,
+    table_schema: str,
+    table_name: str,
+    foreign_table_schema: str,
+    foreign_table_name: str,
+) -> (str, str):
     """
     Returns the columns use in a reference constraint
 
     Parameters
     ----------
     pg_cur
         the psycopg cursor
@@ -102,41 +125,43 @@
         the table name
     foreign_table_schema
         the schema of the foreign table
     foreign_table_name
         the name of the foreign table
     """
     # see https://stackoverflow.com/a/1152321/1548052
-    sql = "SELECT kcu.column_name, ccu.column_name AS foreign_column_name " \
-          "FROM information_schema.table_constraints AS tc " \
-          "JOIN information_schema.key_column_usage AS kcu " \
-          "ON tc.constraint_name = kcu.constraint_name " \
-          "AND tc.table_schema = kcu.table_schema " \
-          "JOIN information_schema.constraint_column_usage AS ccu " \
-          "ON ccu.constraint_name = tc.constraint_name " \
-          "AND ccu.table_schema = tc.table_schema " \
-          "WHERE tc.constraint_type = 'FOREIGN KEY' " \
-          "AND tc.table_name='{tn}' " \
-          "AND tc.table_schema='{ts}' " \
-          "AND ccu.table_name = '{ftn}' " \
-          "AND ccu.table_schema = '{fts}';".format(tn=table_name,
-                                                   ts=table_schema,
-                                                   ftn=foreign_table_name,
-                                                   fts=foreign_table_schema)
+    sql = (
+        "SELECT kcu.column_name, ccu.column_name AS foreign_column_name "
+        "FROM information_schema.table_constraints AS tc "
+        "JOIN information_schema.key_column_usage AS kcu "
+        "ON tc.constraint_name = kcu.constraint_name "
+        "AND tc.table_schema = kcu.table_schema "
+        "JOIN information_schema.constraint_column_usage AS ccu "
+        "ON ccu.constraint_name = tc.constraint_name "
+        "AND ccu.table_schema = tc.table_schema "
+        "WHERE tc.constraint_type = 'FOREIGN KEY' "
+        "AND tc.table_name='{tn}' "
+        "AND tc.table_schema='{ts}' "
+        "AND ccu.table_name = '{ftn}' "
+        "AND ccu.table_schema = '{fts}';".format(
+            tn=table_name, ts=table_schema, ftn=foreign_table_name, fts=foreign_table_schema
+        )
+    )
     pg_cur.execute(sql)
     cols = pg_cur.fetchone()
     if not cols:
-        raise NoReferenceFound('{ts}.{tn} has no reference to {fts}.{ftn}'.format(tn=table_name,
-                                                                                  ts=table_schema,
-                                                                                  ftn=foreign_table_name,
-                                                                                  fts=foreign_table_schema))
+        raise NoReferenceFound(
+            "{ts}.{tn} has no reference to {fts}.{ftn}".format(
+                tn=table_name, ts=table_schema, ftn=foreign_table_name, fts=foreign_table_schema
+            )
+        )
     return cols
 
 
-def default_value(pg_cur: cursor, table_schema: str, table_name: str, column: str) -> str:
+def default_value(pg_cur: Cursor, table_schema: str, table_name: str, column: str) -> str:
     """
     Returns the default value of the column
 
     Parameters
     ----------
     pg_cur
         the psycopg cursor
@@ -145,50 +170,50 @@
     table_name
         the table name
     column
         the column name
     """
     # see https://stackoverflow.com/a/8148177/1548052
 
-    sql = "SELECT pg_get_expr(d.adbin, d.adrelid) AS default_value\n" \
-          "FROM pg_catalog.pg_attribute a\n" \
-          "LEFT JOIN pg_catalog.pg_attrdef d ON (a.attrelid, a.attnum) = (d.adrelid,  d.adnum)\n" \
-          "WHERE  NOT a.attisdropped   -- no dropped (dead) columns\n" \
-          "AND    a.attnum > 0         -- no system columns\n" \
-          "AND    a.attrelid = '{ts}.{tn}'::regclass\n" \
-          "AND    a.attname = '{col}';" \
-        .format(ts=table_schema,
-                tn=table_name,
-                col=column)
+    sql = (
+        "SELECT pg_get_expr(d.adbin, d.adrelid) AS default_value\n"
+        "FROM pg_catalog.pg_attribute a\n"
+        "LEFT JOIN pg_catalog.pg_attrdef d ON (a.attrelid, a.attnum) = (d.adrelid,  d.adnum)\n"
+        "WHERE  NOT a.attisdropped   -- no dropped (dead) columns\n"
+        "AND    a.attnum > 0         -- no system columns\n"
+        "AND    a.attrelid = '{ts}.{tn}'::regclass\n"
+        "AND    a.attname = '{col}';".format(ts=table_schema, tn=table_name, col=column)
+    )
     pg_cur.execute(sql)
-    return pg_cur.fetchone()[0] or 'NULL'
+    return pg_cur.fetchone()[0] or "NULL"
 
 
-def geometry_type(pg_cur: cursor, table_schema: str, table_name: str, column: str = 'geometry') -> (str,int):
+def geometry_type(
+    pg_cur: Cursor, table_schema: str, table_name: str, column: str = "geometry"
+) -> (str, int):
     """
     Returns the geometry type of a column as a tuple (type, srid)
 
     Parameters
     ----------
     pg_cur
         the psycopg cursor
     table_schema
         the table schema
     table_name
         the table name
     column:
         the geometry column name, defaults to "geometry"
     """
-    sql = "SELECT type, srid " \
-          "FROM geometry_columns " \
-          "WHERE f_table_schema = '{s}' " \
-          "AND f_table_name = '{t}' " \
-          "AND f_geometry_column = '{c}';".format(s=table_schema,
-                                                  t=table_name,
-                                                  c=column)
+    sql = (
+        "SELECT type, srid "
+        "FROM geometry_columns "
+        "WHERE f_table_schema = '{s}' "
+        "AND f_table_name = '{t}' "
+        "AND f_geometry_column = '{c}';".format(s=table_schema, t=table_name, c=column)
+    )
     pg_cur.execute(sql)
     res = pg_cur.fetchone()
     if res:
         return res[0], res[1]
     else:
         return None
-
```

### Comparing `pirogue-1.4.2/pirogue/multiple_inheritance.py` & `pirogue-2.0.0/pirogue/multiple_inheritance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-# -*- coding: utf-8 -*-
-
 import os
-import psycopg2
-import psycopg2.extras
 
-from pirogue.utils import table_parts, select_columns, insert_command, update_command, default_value
-from pirogue.information_schema import reference_columns, primary_key, columns, geometry_type
-from pirogue.exceptions import TableHasNoPrimaryKey, VariableError, InvalidDefinition
+import psycopg
+
+from pirogue.exceptions import InvalidDefinition, TableHasNoPrimaryKey, VariableError
+from pirogue.information_schema import (
+    columns,
+    geometry_type,
+    primary_key,
+    reference_columns,
+)
 from pirogue.single_inheritance import SingleInheritance
+from pirogue.utils import (
+    default_value,
+    insert_command,
+    select_columns,
+    table_parts,
+    update_command,
+)
 
 
 class MultipleInheritance:
     """
     Creates a view for multiple inheritance objects with associated triggers to edit data.
     """
 
-    def __init__(self,
-                 definition: dict,
-                 pg_service: str = None,
-                 variables: dict = {},
-                 create_joins: bool = False,
-                 drop: bool = False):
+    def __init__(
+        self,
+        definition: dict,
+        pg_service: str = None,
+        variables: dict = {},
+        create_joins: bool = False,
+        drop: bool = False,
+    ):
         """
         Produces the SQL code of the join table and triggers
 
         Parameters
         ----------
         definition
             the YAML definition of the multiple inheritance
@@ -40,100 +51,129 @@
 
         self.variables = variables
         self.create_joins = create_joins
         self.drop = drop
 
         self.pg_service = pg_service
         if self.pg_service is None:
-            self.pg_service = os.getenv('PGSERVICE')
-        self.conn = psycopg2.connect("service={0}".format(self.pg_service))
+            self.pg_service = os.getenv("PGSERVICE")
+        self.conn = psycopg.connect(f"service={self.pg_service}")
         self.cursor = self.conn.cursor()
 
         # check definition validity
         for key in definition.keys():
-            if key not in ('table', 'view_schema',
-                           'view_name', 'alias', 'short_alias',
-                           'type_name', 'joins',
-                           'insert_trigger', 'update_trigger',
-                           'allow_type_change', 'allow_parent_only',
-                           'additional_columns', 'additional_joins',
-                           'merge_columns', 'merge_geometry_columns',
-                           'pkey_default_value'):
-                raise InvalidDefinition('key {k} is not a valid'.format(k=key))
+            if key not in (
+                "table",
+                "view_schema",
+                "view_name",
+                "alias",
+                "short_alias",
+                "type_name",
+                "joins",
+                "insert_trigger",
+                "update_trigger",
+                "allow_type_change",
+                "allow_parent_only",
+                "additional_columns",
+                "additional_joins",
+                "merge_columns",
+                "merge_geometry_columns",
+                "pkey_default_value",
+            ):
+                raise InvalidDefinition(f"key {key} is not a valid")
         # check joins validity
-        for alias, table_def in definition['joins'].items():
+        for alias, table_def in definition["joins"].items():
             for key in table_def.keys():
-                if key not in ('table', 'short_alias',
-                               'skip_columns', 'fkey',
-                               'remap_columns', 'prefix', 'insert_values', 'update_values'):
-                    raise InvalidDefinition('in join {a} key "{k}" is not valid'.format(a=alias, k=key))
-        for mandatory_key in ['joins']:
+                if key not in (
+                    "table",
+                    "short_alias",
+                    "skip_columns",
+                    "fkey",
+                    "remap_columns",
+                    "prefix",
+                    "insert_values",
+                    "update_values",
+                ):
+                    raise InvalidDefinition(f'in join {alias} key "{key}" is not valid')
+        for mandatory_key in ["joins"]:
             if mandatory_key not in definition:
-                raise InvalidDefinition('Missing key: "{k}" should be provided.'.format(k=mandatory_key))
+                raise InvalidDefinition(f'Missing key: "{mandatory_key}" should be provided.')
         # check trigger modifiers validity
-        for trigger in ('insert_trigger', 'update_trigger'):
+        for trigger in ("insert_trigger", "update_trigger"):
             for key in definition.get(trigger, {}):
-                if key not in ('declare', 'pre', 'post'):
-                    raise InvalidDefinition('key {k} is not valid in trigger definitions'.format(k=key))
+                if key not in ("declare", "pre", "post"):
+                    raise InvalidDefinition(f"key {key} is not valid in trigger definitions")
 
-        (self.master_schema, self.master_table) = table_parts(definition.get('table', None))
-        self.master_skip_colums = definition.get('skip_columns', [])
-        self.master_prefix = definition.get('prefix', None)
-        self.master_remap_columns = definition.get('remap_columns', {})
-        self.pkey_default_value = definition.get('pkey_default_value', False)
+        (self.master_schema, self.master_table) = table_parts(definition.get("table", None))
+        self.master_skip_colums = definition.get("skip_columns", [])
+        self.master_prefix = definition.get("prefix", None)
+        self.master_remap_columns = definition.get("remap_columns", {})
+        self.pkey_default_value = definition.get("pkey_default_value", False)
 
         # global options:
-        self.view_schema = definition.get('view_schema', self.master_schema)
-        self.view_name = definition.get('view_name', "vw_merge_{t}".format(t=self.master_table))
-        self.view_alias = definition.get('alias', self.master_table)
-        self.short_alias = definition.get('short_alias', self.view_alias)
-        self.type_name = definition.get('type_name', '{al}_type'.format(al=self.view_alias))
-        self.insert_trigger = definition.get('insert_trigger', {})
-        self.update_trigger = definition.get('update_trigger', {})
-        self.allow_parent_only = definition.get('allow_parent_only', True)
-        self.allow_type_change = definition.get('allow_type_change', True)
-        self.additional_joins = definition.get('additional_joins', None)
-        self.additional_columns = definition.get('additional_columns', {})
+        self.view_schema = definition.get("view_schema", self.master_schema)
+        self.view_name = definition.get("view_name", f"vw_merge_{self.master_table}")
+        self.view_alias = definition.get("alias", self.master_table)
+        self.short_alias = definition.get("short_alias", self.view_alias)
+        self.type_name = definition.get("type_name", f"{self.view_alias}_type")
+        self.insert_trigger = definition.get("insert_trigger", {})
+        self.update_trigger = definition.get("update_trigger", {})
+        self.allow_parent_only = definition.get("allow_parent_only", True)
+        self.allow_type_change = definition.get("allow_type_change", True)
+        self.additional_joins = definition.get("additional_joins", None)
+        self.additional_columns = definition.get("additional_columns", {})
 
         try:
             self.master_pkey = primary_key(self.cursor, self.master_schema, self.master_table)
         except TableHasNoPrimaryKey:
-            raise TableHasNoPrimaryKey('{vn} has no primary key, specify it with "key"'.format(vn=self.view_alias))
+            raise TableHasNoPrimaryKey(
+                f'{self.view_alias} has no primary key, specify it with "key"'
+            )
 
         # parse the joins definition
-        self.joins = definition['joins']
+        self.joins = definition["joins"]
         self.joined_ref_master_key = []
         for alias, table_def in self.joins.items():
-            (table_def['table_schema'], table_def['table_name']) = table_parts(table_def['table'])
-            table_def['short_alias'] = table_def.get('short_alias', alias)
+            (table_def["table_schema"], table_def["table_name"]) = table_parts(table_def["table"])
+            table_def["short_alias"] = table_def.get("short_alias", alias)
 
-            if 'fkey' in table_def:
-                table_def['ref_master_key'] = table_def['fkey']
+            if "fkey" in table_def:
+                table_def["ref_master_key"] = table_def["fkey"]
             else:
-                table_def['ref_master_key'] = reference_columns(self.cursor,
-                                                                table_def['table_schema'], table_def['table_name'],
-                                                                self.master_schema, self.master_table)[0]
+                table_def["ref_master_key"] = reference_columns(
+                    self.cursor,
+                    table_def["table_schema"],
+                    table_def["table_name"],
+                    self.master_schema,
+                    self.master_table,
+                )[0]
             try:
-                table_def['pkey'] = primary_key(self.cursor, table_def['table_schema'], table_def['table_name'])
+                table_def["pkey"] = primary_key(
+                    self.cursor, table_def["table_schema"], table_def["table_name"]
+                )
             except TableHasNoPrimaryKey:
-                table_def['pkey'] = table_def['ref_master_key']
+                table_def["pkey"] = table_def["ref_master_key"]
 
         # pre-process merged columns
         self.merge_column_cast = {}
         # for geometry columns, we need to get the type to cast the NULL value
-        merge_geometry_columns = definition.get('merge_geometry_columns', [])
+        merge_geometry_columns = definition.get("merge_geometry_columns", [])
         for col in merge_geometry_columns:
             for table_def in self.joins.values():
-                gt = geometry_type(self.cursor, table_def['table_schema'], table_def['table_name'], col)
+                gt = geometry_type(
+                    self.cursor, table_def["table_schema"], table_def["table_name"], col
+                )
                 if gt:
-                    self.merge_column_cast[col] = '::geometry({type},{srid})'.format(type=gt[0],srid=gt[1])
+                    self.merge_column_cast[col] = "::geometry({type},{srid})".format(
+                        type=gt[0], srid=gt[1]
+                    )
                     break
             if col not in self.merge_column_cast:
-                raise InvalidDefinition('There is no geometry column "{col}" in joined tables'.format(col=col))
-        self.merge_columns = definition.get('merge_columns', []) + merge_geometry_columns
+                raise InvalidDefinition(f'There is no geometry column "{col}" in joined tables')
+        self.merge_columns = definition.get("merge_columns", []) + merge_geometry_columns
 
     def create(self) -> bool:
         """
         Creates the merge view on the specified service
         Returns True in case of success
         """
         queries = []
@@ -148,59 +188,64 @@
         queries.append(self.__extras())
 
         for sql in queries:
             if not sql:
                 continue
             try:
                 if self.variables:
-                    self.cursor.execute(sql, self.variables)
+                    self.cursor.execute(psycopg.sql.SQL(sql).format(self.variables))
                 else:
                     self.cursor.execute(sql)
-            except TypeError as e:
+            except TypeError:
                 success = False
-                print("*** Failing:\n{}\n***".format(sql))
-                raise VariableError("An error in a SQL variable is probable. "
-                                    "Check the variables in the SQL code "
-                                    "(were given: {svars}). "
-                                    "Also, any % character shall be escaped with %%"
-                                    .format(svars=list(self.variables.keys())))
-            except psycopg2.Error as e:
-                print("*** Failing:\n{}\n***".format(sql))
+                print(f"*** Failing:\n{sql}\n***")
+                raise VariableError(
+                    "An error in a SQL variable is probable. "
+                    "Check the variables in the SQL code "
+                    "(were given: {svars}). "
+                    "Also, any % character shall be escaped with %%".format(
+                        svars=list(self.variables.keys())
+                    )
+                )
+            except psycopg.Error as e:
+                print(f"*** Failing:\n{sql}\n***")
                 raise e
         self.conn.commit()
         self.conn.close()
 
         if self.create_joins:
             for alias, table_def in self.joins.items():
-                success &= SingleInheritance(pg_service=self.pg_service,
-                                             parent_table='{s}.{t}'.format(s=self.master_schema, t=self.master_table),
-                                             child_table='{s}.{t}'.format(s=table_def['table_schema'], t=table_def['table_name']),
-                                             view_name='vw_{a}'.format(a=alias),
-                                             view_schema=self.view_schema,
-                                             ).create()
+                success &= SingleInheritance(
+                    pg_service=self.pg_service,
+                    parent_table=f"{self.master_schema}.{self.master_table}",
+                    child_table="{s}.{t}".format(
+                        s=table_def["table_schema"], t=table_def["table_name"]
+                    ),
+                    view_name=f"vw_{alias}",
+                    view_schema=self.view_schema,
+                ).create()
         return success
 
     def __drops(self) -> str:
-        sql = "DROP VIEW IF EXISTS {vs}.{vn};" \
-              "DROP TYPE IF EXISTS {vs}.{tn};" \
-                  .format(vs=self.view_schema,
-                    tn=self.type_name,
-                    vn=self.view_name)
+        sql = "DROP VIEW IF EXISTS {vs}.{vn};" "DROP TYPE IF EXISTS {vs}.{tn};".format(
+            vs=self.view_schema, tn=self.type_name, vn=self.view_name
+        )
         return sql
 
     def __type(self) -> str:
         """
 
         :return:
         """
-        sql = "CREATE TYPE {vs}.{tn} AS ENUM ('{pt}', {ct} );"\
-            .format(vs=self.view_schema,
-                    tn=self.type_name,
-                    pt=self.view_alias if self.allow_parent_only else 'unknown',
-                    ct=', '.join(["'{al}'".format(al=alias) for alias in self.joins]))
+        sql = "CREATE TYPE {vs}.{tn} AS ENUM ('{pt}', {ct} );".format(
+            vs=self.view_schema,
+            tn=self.type_name,
+            pt=self.view_alias if self.allow_parent_only else "unknown",
+            ct=", ".join([f"'{alias}'" for alias in self.joins]),
+        )
         return sql
 
     def __view(self) -> str:
         """
         :return:
         """
 
@@ -212,69 +257,115 @@
     CASE
       {types}
       ELSE {no_subtype}
     END AS {type_name}
     {master_columns}{merge_columns}
     {joined_columns}{additional_columns}
   FROM {mt}.{ms} {sa}
-    {joined_tables}{additional_joins};        
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           types='\n      '.join(["WHEN {shal}.{mrf} IS NOT NULL THEN '{al}'::{vs}.{tn}"
-                                 .format(shal=table_def['short_alias'], mrf=table_def['ref_master_key'],
-                                         al=alias, vs=self.view_schema, tn=self.type_name)
-                                  for alias, table_def in sorted_joins]),
-           no_subtype="'{type}'::{vs}.{tn}".format(type=self.view_alias if self.allow_parent_only else 'unknown',
-                                                   vs=self.view_schema, tn=self.type_name),
-           type_name=self.type_name,
-           master_columns=select_columns(self.cursor, self.master_schema, self.master_table,
-                                         table_alias=self.view_alias,
-                                         skip_columns=self.master_skip_colums,
-                                         prefix=self.master_prefix,
-                                         remap_columns=self.master_remap_columns,
-                                         indent=4,
-                                         separate_first=True),
-           merge_columns='\n      , '.join(['\n    , CASE'
-                                            '\n      {conditions}'
-                                            '\n      ELSE NULL{cast}'
-                                            '\n    END AS {col}'
-                                            .format(col=col,
-                                                    conditions='\n      '.join(['WHEN {ta}.{rmk} IS NOT NULL THEN {ta}.{col}'
-                                                                .format(ta=table_def['short_alias'],
-                                                                        rmk=table_def['ref_master_key'],
-                                                                        col=col)
-                                                                for alias, table_def in sorted_joins
-                                                                if col in columns(self.cursor, table_def['table_schema'], table_def['table_name'], skip_columns=table_def.get('skip_columns', []))]),
-                                                    cast=self.merge_column_cast.get(col, '')
-                                                    )
-                                            for col in self.merge_columns]),
-           joined_columns='\n    '.join([select_columns(self.cursor, table_def['table_schema'], table_def['table_name'],
-                                                        table_alias=table_def['short_alias'],
-                                                        skip_columns=table_def.get('skip_columns', [])+[table_def['ref_master_key']],
-                                                        safe_skip_columns=self.merge_columns,
-                                                        prefix=table_def.get('prefix', None),
-                                                        remove_pkey=False,
-                                                        remap_columns=table_def.get('remap_columns', {}),
-                                                        indent=4,
-                                                        separate_first=True)
-                                         for alias, table_def in sorted_joins]),
-           additional_columns=''.join([',\n    {cdef} AS {alias}'.format(cdef=cdef,alias=alias)
-                                       for alias, cdef in self.additional_columns.items()]),
-           mt=self.master_schema,
-           ms=self.master_table,
-           sa=self.short_alias,
-           joined_tables='\n    '.join(["LEFT JOIN {tbl} {tal} ON {tal}.{rmk} = {msa}.{mpk}"
-                                            .format(tbl=table_def[1]['table'],
-                                                    tal=table_def[1]['short_alias'],
-                                                    rmk=table_def[1]['ref_master_key'],
-                                                    msa=self.short_alias,
-                                                    mpk=self.master_pkey)
-                                            for table_def in sorted_joins]),
-           additional_joins='\n    {ad}'.format(ad=self.additional_joins) if self.additional_joins else ''
-           )
+    {joined_tables}{additional_joins};
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            types="\n      ".join(
+                [
+                    "WHEN {shal}.{mrf} IS NOT NULL THEN '{al}'::{vs}.{tn}".format(
+                        shal=table_def["short_alias"],
+                        mrf=table_def["ref_master_key"],
+                        al=alias,
+                        vs=self.view_schema,
+                        tn=self.type_name,
+                    )
+                    for alias, table_def in sorted_joins
+                ]
+            ),
+            no_subtype="'{type}'::{vs}.{tn}".format(
+                type=self.view_alias if self.allow_parent_only else "unknown",
+                vs=self.view_schema,
+                tn=self.type_name,
+            ),
+            type_name=self.type_name,
+            master_columns=select_columns(
+                self.cursor,
+                self.master_schema,
+                self.master_table,
+                table_alias=self.view_alias,
+                skip_columns=self.master_skip_colums,
+                prefix=self.master_prefix,
+                remap_columns=self.master_remap_columns,
+                indent=4,
+                separate_first=True,
+            ),
+            merge_columns="\n      , ".join(
+                [
+                    "\n    , CASE"
+                    "\n      {conditions}"
+                    "\n      ELSE NULL{cast}"
+                    "\n    END AS {col}".format(
+                        col=col,
+                        conditions="\n      ".join(
+                            [
+                                "WHEN {ta}.{rmk} IS NOT NULL THEN {ta}.{col}".format(
+                                    ta=table_def["short_alias"],
+                                    rmk=table_def["ref_master_key"],
+                                    col=col,
+                                )
+                                for alias, table_def in sorted_joins
+                                if col
+                                in columns(
+                                    self.cursor,
+                                    table_def["table_schema"],
+                                    table_def["table_name"],
+                                    skip_columns=table_def.get("skip_columns", []),
+                                )
+                            ]
+                        ),
+                        cast=self.merge_column_cast.get(col, ""),
+                    )
+                    for col in self.merge_columns
+                ]
+            ),
+            joined_columns="\n    ".join(
+                [
+                    select_columns(
+                        self.cursor,
+                        table_def["table_schema"],
+                        table_def["table_name"],
+                        table_alias=table_def["short_alias"],
+                        skip_columns=table_def.get("skip_columns", [])
+                        + [table_def["ref_master_key"]],
+                        safe_skip_columns=self.merge_columns,
+                        prefix=table_def.get("prefix", None),
+                        remove_pkey=False,
+                        remap_columns=table_def.get("remap_columns", {}),
+                        indent=4,
+                        separate_first=True,
+                    )
+                    for alias, table_def in sorted_joins
+                ]
+            ),
+            additional_columns="".join(
+                [f",\n    {cdef} AS {alias}" for alias, cdef in self.additional_columns.items()]
+            ),
+            mt=self.master_schema,
+            ms=self.master_table,
+            sa=self.short_alias,
+            joined_tables="\n    ".join(
+                [
+                    "LEFT JOIN {tbl} {tal} ON {tal}.{rmk} = {msa}.{mpk}".format(
+                        tbl=table_def[1]["table"],
+                        tal=table_def[1]["short_alias"],
+                        rmk=table_def[1]["ref_master_key"],
+                        msa=self.short_alias,
+                        mpk=self.master_pkey,
+                    )
+                    for table_def in sorted_joins
+                ]
+            ),
+            additional_joins=f"\n    {self.additional_joins}" if self.additional_joins else "",
+        )
         return sql
 
     def __insert_trigger(self) -> str:
         """
 
         :return:
         """
@@ -286,15 +377,15 @@
 $BODY$
 DECLARE
   {declare}
 BEGIN
   {insert_trigger_pre}
   {insert_master}
 
-  CASE 
+  CASE
     {insert_joins}
   ELSE
     {raise_notice}
   END CASE;
 
   {insert_trigger_post}
 RETURN NEW;
@@ -303,50 +394,78 @@
 LANGUAGE plpgsql;
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_insert ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_insert
     INSTEAD OF INSERT ON {vs}.{vn}
     FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_insert();
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           declare='\n  '.join(['{d};'.format(d=declare) for declare in self.insert_trigger.get('declare', [])]),
-           insert_trigger_pre=self.insert_trigger.get('pre', ''),
-           insert_master=insert_command(self.cursor, self.master_schema, self.master_table,
-                                        skip_columns=self.master_skip_colums,
-                                        prefix=self.master_prefix,
-                                        remap_columns=self.master_remap_columns,
-                                        remove_pkey=False,
-                                        indent=8,
-                                        coalesce_pkey_default=True,
-                                        returning='{mpk} INTO NEW.{mpk}'.format(mpk=self.master_pkey)),
-           insert_joins='\n    '.join(["WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} THEN"
-                                       "\n      {insert_join}".format(type_name=self.type_name,
-                                                                      alias=alias,
-                                                                      vs=self.view_schema,
-                                                                      insert_join=insert_command(self.cursor,
-                                                                                                 table_def['table_schema'],
-                                                                                                 table_def['table_name'],
-                                                                                                 table_alias=table_def['short_alias'],
-                                                                                                 skip_columns=table_def.get('skip_columns', []),
-                                                                                                 prefix=table_def.get('prefix', None),
-                                                                                                 insert_values={**{table_def['ref_master_key']: 'NEW.{c}'.format(c=self.master_pkey)},
-                                                                                                                **table_def.get('insert_values', {})},
-                                                                                                 remap_columns=table_def.get('remap_columns', {}),
-                                                                                                 remove_pkey=False,
-                                                                                                 indent=4))
-                                      for alias, table_def in sorted_joins]),
-           raise_notice='NULL;' if self.allow_parent_only else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR"
-                            .format(vn=self.view_name,
-                                    percent_char='%%' if self.variables else '%',  # if variables, % should be escaped because cursor.execute is run with variables
-                                    type_name=self.type_name),
-           insert_trigger_post=self.insert_trigger.get('post', ''))
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            declare="\n  ".join(
+                [f"{declare};" for declare in self.insert_trigger.get("declare", [])]
+            ),
+            insert_trigger_pre=self.insert_trigger.get("pre", ""),
+            insert_master=insert_command(
+                self.cursor,
+                self.master_schema,
+                self.master_table,
+                skip_columns=self.master_skip_colums,
+                prefix=self.master_prefix,
+                remap_columns=self.master_remap_columns,
+                remove_pkey=False,
+                indent=8,
+                coalesce_pkey_default=True,
+                returning="{mpk} INTO NEW.{mpk}".format(mpk=self.master_pkey),
+            ),
+            insert_joins="\n    ".join(
+                [
+                    "WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} THEN"
+                    "\n      {insert_join}".format(
+                        type_name=self.type_name,
+                        alias=alias,
+                        vs=self.view_schema,
+                        insert_join=insert_command(
+                            self.cursor,
+                            table_def["table_schema"],
+                            table_def["table_name"],
+                            table_alias=table_def["short_alias"],
+                            skip_columns=table_def.get("skip_columns", []),
+                            prefix=table_def.get("prefix", None),
+                            insert_values={
+                                **{
+                                    table_def["ref_master_key"]: "NEW.{c}".format(
+                                        c=self.master_pkey
+                                    )
+                                },
+                                **table_def.get("insert_values", {}),
+                            },
+                            remap_columns=table_def.get("remap_columns", {}),
+                            remove_pkey=False,
+                            indent=4,
+                        ),
+                    )
+                    for alias, table_def in sorted_joins
+                ]
+            ),
+            raise_notice=(
+                "NULL;"
+                if self.allow_parent_only
+                else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR".format(
+                    vn=self.view_name,
+                    percent_char=(
+                        "%%" if self.variables else "%"
+                    ),  # if variables, % should be escaped because cursor.execute is run with variables
+                    type_name=self.type_name,
+                )
+            ),
+            insert_trigger_post=self.insert_trigger.get("post", ""),
+        )
         return sql
 
-
     def __update_trigger(self):
         sorted_joins = sorted(self.joins.items())
         sql = """-- UPDATE TRIGGER
 CREATE OR REPLACE FUNCTION {vs}.ft_{vn}_update() RETURNS trigger AS
 $BODY$
 DECLARE
   {declare}
@@ -369,78 +488,118 @@
 LANGUAGE plpgsql;
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_update ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_update
     INSTEAD OF update ON {vs}.{vn}
     FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_update();
-        """.format(vs=self.view_schema,
-                   vn=self.view_name,
-                   declare='\n  '.join(['{d};'.format(d=declare) for declare in self.update_trigger.get('declare', [])]),
-                   update_trigger_pre=self.update_trigger.get('pre', ''),
-                   update_master=update_command(self.cursor, self.master_schema, self.master_table,
-                                                skip_columns=self.master_skip_colums,
-                                                prefix=self.master_prefix,
-                                                remap_columns=self.master_remap_columns,
-                                                indent=8),
-                   type_name=self.type_name,
-                   type_change="RAISE EXCEPTION 'Type change not allowed for {alias}'"
-                               "\n      USING HINT = 'You cannot switch from ' "
-                               "|| OLD.{type_name} || ' to ' || NEW.{type_name};"
-                                .format(alias=self.view_alias, type_name=self.type_name)
-                               if not self.allow_type_change else
-                               "CASE"
-                               "\n      {deletes}"
-                               "\n    END CASE;"
-                               "\n    CASE"
-                               "\n      {inserts}"
-                               "\n      ELSE -- do nothing"
-                               "\n    END CASE;"
-                               .format(deletes='\n      '.join(["WHEN OLD.{type_name} = '{alias}'::{vs}.{type_name} "
-                                                                "THEN DELETE FROM {ts}.{tn} "
-                                                                "WHERE {rmk} = OLD.{mpk};"
-                                                                .format(type_name=self.type_name,
-                                                                        alias=alias,
-                                                                        vs=self.view_schema,
-                                                                        ts=table_def['table_schema'],
-                                                                        tn=table_def['table_name'],
-                                                                        rmk=table_def['ref_master_key'],
-                                                                        mpk=self.master_pkey)
-                                                                for alias, table_def in sorted_joins]),
-                                       inserts='\n      '.join(["WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} "
-                                                                "THEN INSERT INTO {ts}.{tn} "
-                                                                "({rmk}) VALUES (OLD.{mpk});"
-                                                               .format(type_name=self.type_name,
-                                                                       alias=alias,
-                                                                       vs=self.view_schema,
-                                                                       ts=table_def['table_schema'],
-                                                                       tn=table_def['table_name'],
-                                                                       rmk=table_def['ref_master_key'],
-                                                                       mpk=self.master_pkey)
-                                                                for alias, table_def in sorted_joins])),
-                   update_joins='\n    '.join(["WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} THEN"
-                                               "\n      {update_join}".format(type_name=self.type_name,
-                                                                              alias=alias,
-                                                                              vs=self.view_schema,
-                                                                              update_join=update_command(self.cursor, table_def['table_schema'], table_def['table_name'],
-                                                                                                         table_alias=table_def['short_alias'],
-                                                                                                         pkey=table_def['pkey'],
-                                                                                                         skip_columns=table_def.get('skip_columns', []),
-                                                                                                         prefix=table_def.get('prefix', None),
-                                                                                                         remap_columns=table_def.get('remap_columns', {}),
-                                                                                                         update_values={**{table_def['pkey']: 'OLD.{c}'.format(c=self.master_pkey)},
-                                                                                                                        **table_def.get('update_values', {})},
-                                                                                                         indent=4))
-                                   for alias, table_def in sorted_joins]),
-                   raise_notice='NULL;' if self.allow_parent_only
-                                else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR"
-                                     .format(vn=self.view_name,
-                                             percent_char='%%' if self.variables else '%',  # if variables, % should be escaped because cursor.execute is run with variables
-                                             type_name=self.type_name),
-                   update_trigger_post=self.update_trigger.get('post', ''))
+        """.format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            declare="\n  ".join(
+                [f"{declare};" for declare in self.update_trigger.get("declare", [])]
+            ),
+            update_trigger_pre=self.update_trigger.get("pre", ""),
+            update_master=update_command(
+                self.cursor,
+                self.master_schema,
+                self.master_table,
+                skip_columns=self.master_skip_colums,
+                prefix=self.master_prefix,
+                remap_columns=self.master_remap_columns,
+                indent=8,
+            ),
+            type_name=self.type_name,
+            type_change=(
+                "RAISE EXCEPTION 'Type change not allowed for {alias}'"
+                "\n      USING HINT = 'You cannot switch from ' "
+                "|| OLD.{type_name} || ' to ' || NEW.{type_name};".format(
+                    alias=self.view_alias, type_name=self.type_name
+                )
+                if not self.allow_type_change
+                else "CASE"
+                "\n      {deletes}"
+                "\n    END CASE;"
+                "\n    CASE"
+                "\n      {inserts}"
+                "\n      ELSE -- do nothing"
+                "\n    END CASE;".format(
+                    deletes="\n      ".join(
+                        [
+                            "WHEN OLD.{type_name} = '{alias}'::{vs}.{type_name} "
+                            "THEN DELETE FROM {ts}.{tn} "
+                            "WHERE {rmk} = OLD.{mpk};".format(
+                                type_name=self.type_name,
+                                alias=alias,
+                                vs=self.view_schema,
+                                ts=table_def["table_schema"],
+                                tn=table_def["table_name"],
+                                rmk=table_def["ref_master_key"],
+                                mpk=self.master_pkey,
+                            )
+                            for alias, table_def in sorted_joins
+                        ]
+                    ),
+                    inserts="\n      ".join(
+                        [
+                            "WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} "
+                            "THEN INSERT INTO {ts}.{tn} "
+                            "({rmk}) VALUES (OLD.{mpk});".format(
+                                type_name=self.type_name,
+                                alias=alias,
+                                vs=self.view_schema,
+                                ts=table_def["table_schema"],
+                                tn=table_def["table_name"],
+                                rmk=table_def["ref_master_key"],
+                                mpk=self.master_pkey,
+                            )
+                            for alias, table_def in sorted_joins
+                        ]
+                    ),
+                )
+            ),
+            update_joins="\n    ".join(
+                [
+                    "WHEN NEW.{type_name} = '{alias}'::{vs}.{type_name} THEN"
+                    "\n      {update_join}".format(
+                        type_name=self.type_name,
+                        alias=alias,
+                        vs=self.view_schema,
+                        update_join=update_command(
+                            self.cursor,
+                            table_def["table_schema"],
+                            table_def["table_name"],
+                            table_alias=table_def["short_alias"],
+                            pkey=table_def["pkey"],
+                            skip_columns=table_def.get("skip_columns", []),
+                            prefix=table_def.get("prefix", None),
+                            remap_columns=table_def.get("remap_columns", {}),
+                            update_values={
+                                **{table_def["pkey"]: f"OLD.{self.master_pkey}"},
+                                **table_def.get("update_values", {}),
+                            },
+                            indent=4,
+                        ),
+                    )
+                    for alias, table_def in sorted_joins
+                ]
+            ),
+            raise_notice=(
+                "NULL;"
+                if self.allow_parent_only
+                else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR".format(
+                    vn=self.view_name,
+                    percent_char=(
+                        "%%" if self.variables else "%"
+                    ),  # if variables, % should be escaped because cursor.execute is run with variables
+                    type_name=self.type_name,
+                )
+            ),
+            update_trigger_post=self.update_trigger.get("post", ""),
+        )
         return sql
 
     def __delete_trigger(self):
         sorted_joins = sorted(self.joins.items())
         sql = """
 CREATE OR REPLACE FUNCTION {vs}.ft_{vn}_delete() RETURNS trigger AS
     $BODY$
@@ -455,34 +614,44 @@
     LANGUAGE 'plpgsql';
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_delete ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_delete
     INSTEAD OF DELETE ON {vs}.{vn}
     FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_delete();
-""".format(vn=self.view_name,
-           deletes='\n      '.join(["WHEN OLD.{type_name} = '{alias}'::{vs}.{type_name} "
-                                    "THEN DELETE FROM {ts}.{tn} "
-                                    "WHERE {rmk} = OLD.{mpk};"
-                                   .format(type_name=self.type_name,
-                                           alias=alias,
-                                           vs=self.view_schema,
-                                           ts=table_def['table_schema'],
-                                           tn=table_def['table_name'],
-                                           rmk=table_def['ref_master_key'],
-                                           mpk=self.master_pkey)
-                                    for alias, table_def in sorted_joins]),
-           ts=self.master_schema,
-           tn=self.master_table,
-           mpk=self.master_pkey,
-           vs=self.view_schema)
+""".format(
+            vn=self.view_name,
+            deletes="\n      ".join(
+                [
+                    "WHEN OLD.{type_name} = '{alias}'::{vs}.{type_name} "
+                    "THEN DELETE FROM {ts}.{tn} "
+                    "WHERE {rmk} = OLD.{mpk};".format(
+                        type_name=self.type_name,
+                        alias=alias,
+                        vs=self.view_schema,
+                        ts=table_def["table_schema"],
+                        tn=table_def["table_name"],
+                        rmk=table_def["ref_master_key"],
+                        mpk=self.master_pkey,
+                    )
+                    for alias, table_def in sorted_joins
+                ]
+            ),
+            ts=self.master_schema,
+            tn=self.master_table,
+            mpk=self.master_pkey,
+            vs=self.view_schema,
+        )
         return sql
 
     def __extras(self):
-        sql = ''
+        sql = ""
         if self.pkey_default_value:
-            sql += "ALTER VIEW {vs}.{vn} ALTER {master_pkey} SET DEFAULT {dv};"\
-                .format(vs=self.view_schema,
-                        vn=self.view_name,
-                        master_pkey=self.master_pkey,
-                        dv=default_value(self.cursor, self.master_schema, self.master_table, self.master_pkey))
-        return sql
+            sql += "ALTER VIEW {vs}.{vn} ALTER {master_pkey} SET DEFAULT {dv};".format(
+                vs=self.view_schema,
+                vn=self.view_name,
+                master_pkey=self.master_pkey,
+                dv=default_value(
+                    self.cursor, self.master_schema, self.master_table, self.master_pkey
+                ),
+            )
+        return sql
```

### Comparing `pirogue-1.4.2/pirogue/simple_joins.py` & `pirogue-2.0.0/pirogue/simple_joins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,109 @@
-# -*- coding: utf-8 -*-
-
 import os
-import psycopg2
-import psycopg2.extras
 
-from pirogue.utils import table_parts, select_columns
-from pirogue.information_schema import reference_columns, primary_key
-from pirogue.exceptions import InvalidDefinition, TableHasNoPrimaryKey, NoReferenceFound
+import psycopg
+
+from pirogue.exceptions import InvalidDefinition, NoReferenceFound, TableHasNoPrimaryKey
+from pirogue.information_schema import primary_key, reference_columns
+from pirogue.utils import select_columns, table_parts
 
 
 class SimpleJoins:
     """
     Creates a view made of simple joins, without any edit triggers.
     """
-    def __init__(self,
-                 definition: dict,
-                 pg_service: str = None):
+
+    def __init__(self, definition: dict, pg_service: str = None):
         """
         Produces the SQL code of the join table and triggers
 
         Parameters
         ----------
         definition
             the YAML definition of the multiple inheritance
         pg_service
             if not given, it is determined using environment variable PGSERVICE
         """
 
         # check definition validity
         for key in definition.keys():
-            if key not in ('table', 'view_schema', 'joins', 'pkey', 'view_name'):
-                raise InvalidDefinition('key {k} is not a valid'.format(k=key))
+            if key not in ("table", "view_schema", "joins", "pkey", "view_name"):
+                raise InvalidDefinition(f"key {key} is not a valid")
         # check joins validity
-        for alias, table_def in definition['joins'].items():
+        for alias, table_def in definition["joins"].items():
             for key in table_def.keys():
-                if key not in ('table', 'short_alias',
-                               'fkey', 'prefix',
-                               'skip_columns', 'remap_columns'):
-                    raise InvalidDefinition('in join {a} key "{k}" is not valid'.format(a=alias, k=key))
+                if key not in (
+                    "table",
+                    "short_alias",
+                    "fkey",
+                    "prefix",
+                    "skip_columns",
+                    "remap_columns",
+                ):
+                    raise InvalidDefinition(f'in join {alias} key "{key}" is not valid')
 
         if pg_service is None:
-            pg_service = os.getenv('PGSERVICE')
-        self.conn = psycopg2.connect("service={0}".format(pg_service))
+            pg_service = os.getenv("PGSERVICE")
+        self.conn = psycopg.connect(f"service={pg_service}")
         self.cursor = self.conn.cursor()
 
-        (self.parent_schema, self.parent_table) = table_parts(definition['table'])
-        self.view_schema = definition.get('view_schema', self.parent_schema)
-        self.view_name = definition.get('view_name', "vw_{pt}".format(pt=self.parent_table))
+        (self.parent_schema, self.parent_table) = table_parts(definition["table"])
+        self.view_schema = definition.get("view_schema", self.parent_schema)
+        self.view_name = definition.get("view_name", f"vw_{self.parent_table}")
 
         try:
             self.parent_pkey = primary_key(self.cursor, self.parent_schema, self.parent_table)
         except TableHasNoPrimaryKey:
-            self.parent_pkey = definition['pkey']
+            self.parent_pkey = definition["pkey"]
 
         class Table:
             def __init__(self):
                 self.schema_name = None
                 self.table_name = None
                 self.pkey = None
                 self.ref_parent_key = None
                 self.parent_referenced_key = None
                 self.skip_columns = None
                 self.remap_columns = None
                 self.prefix = None
 
         self.child_tables = {}
-        for alias, table_def in definition['joins'].items():
+        for alias, table_def in definition["joins"].items():
             child = Table()
-            (child.schema_name, child.table_name) = table_parts(table_def['table'])
+            (child.schema_name, child.table_name) = table_parts(table_def["table"])
             child.pkey = primary_key(self.cursor, child.schema_name, child.table_name)
             try:
-                (child.parent_referenced_key, child.ref_parent_key) = reference_columns(self.cursor,
-                                                                                        self.parent_schema,
-                                                                                        self.parent_table,
-                                                                                        child.schema_name,
-                                                                                        child.table_name)
+                (child.parent_referenced_key, child.ref_parent_key) = reference_columns(
+                    self.cursor,
+                    self.parent_schema,
+                    self.parent_table,
+                    child.schema_name,
+                    child.table_name,
+                )
                 assert child.pkey == child.ref_parent_key
             except NoReferenceFound:
-                child.parent_referenced_key = table_def['fkey']
+                child.parent_referenced_key = table_def["fkey"]
 
-            child.skip_columns = table_def.get('skip_columns', {})
-            child.remap_columns = table_def.get('remap_columns', {})
-            child.prefix = table_def.get('prefix', None)
+            child.skip_columns = table_def.get("skip_columns", {})
+            child.remap_columns = table_def.get("remap_columns", {})
+            child.prefix = table_def.get("prefix", None)
             self.child_tables[alias] = child
 
     def create(self) -> bool:
         """
         Creates the merge view on the specified service
         Returns True in case of success
         """
         sql = self.__view()
         success = True
         try:
             self.cursor.execute(sql)
-        except psycopg2.Error as e:
+        except psycopg.Error as e:
             success = False
-            print("*** Failing:\n{}\n***".format(sql))
+            print(f"*** Failing:\n{sql}\n***")
             raise e
         self.conn.commit()
         self.conn.close()
         return success
 
     def __view(self) -> str:
         """
@@ -108,26 +112,49 @@
         """
         sql = """
 CREATE OR REPLACE VIEW {vs}.{vn} AS SELECT
   {parent_cols}
   {child_cols}
   FROM {ps}.{pt}
   {joins};
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           parent_cols=select_columns(self.cursor, self.parent_schema, self.parent_table, table_alias=self.parent_table, remove_pkey=False),
-           child_cols='\n  '.join([select_columns(self.cursor, child_def.schema_name, child_def.table_name,
-                                                   table_alias=alias, remap_columns=child_def.remap_columns,
-                                                   prefix=child_def.prefix, separate_first=True)
-                                    for alias, child_def in self.child_tables.items()]),
-           ps=self.parent_schema,
-           pt=self.parent_table,
-           joins='\n  '.join(["LEFT JOIN {cs}.{ct} {alias} ON {alias}.{cpk} = {pt}.{rpk}".format(cs=child.schema_name,
-                                                                                                 ct=child.table_name,
-                                                                                                 alias=alias,
-                                                                                                 cpk=child.pkey,
-                                                                                                 pt=self.parent_table,
-                                                                                                 rpk=child.parent_referenced_key)
-                            for alias, child in self.child_tables.items()])
-           )
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            parent_cols=select_columns(
+                self.cursor,
+                self.parent_schema,
+                self.parent_table,
+                table_alias=self.parent_table,
+                remove_pkey=False,
+            ),
+            child_cols="\n  ".join(
+                [
+                    select_columns(
+                        self.cursor,
+                        child_def.schema_name,
+                        child_def.table_name,
+                        table_alias=alias,
+                        remap_columns=child_def.remap_columns,
+                        prefix=child_def.prefix,
+                        separate_first=True,
+                    )
+                    for alias, child_def in self.child_tables.items()
+                ]
+            ),
+            ps=self.parent_schema,
+            pt=self.parent_table,
+            joins="\n  ".join(
+                [
+                    "LEFT JOIN {cs}.{ct} {alias} ON {alias}.{cpk} = {pt}.{rpk}".format(
+                        cs=child.schema_name,
+                        ct=child.table_name,
+                        alias=alias,
+                        cpk=child.pkey,
+                        pt=self.parent_table,
+                        rpk=child.parent_referenced_key,
+                    )
+                    for alias, child in self.child_tables.items()
+                ]
+            ),
+        )
 
-        return sql
+        return sql
```

### Comparing `pirogue-1.4.2/pirogue/single_inheritance.py` & `pirogue-2.0.0/pirogue/single_inheritance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# -*- coding: utf-8 -*-
-
 import os
-import psycopg2
-import psycopg2.extras
 
-from pirogue.utils import table_parts, select_columns, insert_command, update_command
-from pirogue.information_schema import reference_columns, primary_key, default_value
+import psycopg
+
 from pirogue.exceptions import TableHasNoPrimaryKey
+from pirogue.information_schema import default_value, primary_key, reference_columns
+from pirogue.utils import insert_command, select_columns, table_parts, update_command
 
 
 class SingleInheritance:
     """
     Creates a join view with associated triggers to edit for a single inheritance.
     """
 
-    def __init__(self, parent_table: str, child_table: str,
-                 pg_service: str = None,
-                 view_schema: str = None,
-                 view_name: str = None,
-                 pkey_default_value: bool = False,
-                 inner_defaults: dict = {}):
+    def __init__(
+        self,
+        parent_table: str,
+        child_table: str,
+        pg_service: str = None,
+        view_schema: str = None,
+        view_name: str = None,
+        pkey_default_value: bool = False,
+        inner_defaults: dict = {},
+    ):
         """
         Produces the SQL code of the join table and triggers
 
         Parameters
         ----------
         pg_service
             if not given, it is determined using environment variable PGSERVICE
@@ -38,63 +40,68 @@
         pkey_default_value
             the primary key column of the view will have a default value according to the child primary key table
         inner_defaults
             dictionary of other columns to default to in case the provided value is null or empty
         """
 
         if pg_service is None:
-            pg_service = os.getenv('PGSERVICE')
-        self.conn = psycopg2.connect("service={0}".format(pg_service))
+            pg_service = os.getenv("PGSERVICE")
+        self.conn = psycopg.connect(f"service={pg_service}")
         self.cursor = self.conn.cursor()
 
         self.pkey_default_value = pkey_default_value
         self.inner_defaults = inner_defaults
 
         (self.parent_schema, self.parent_table) = table_parts(parent_table)
         (self.child_schema, self.child_table) = table_parts(child_table)
 
         if view_schema is None:
             if self.parent_schema != self.child_schema:
-                raise ValueError('Destination schema cannot be guessed if different on sources tables.')
+                raise ValueError(
+                    "Destination schema cannot be guessed if different on sources tables."
+                )
             else:
                 self.view_schema = self.parent_schema
         else:
             self.view_schema = view_schema
 
-        self.view_name = view_name or "vw_{pt}_{ct}".format(pt=self.parent_table, ct=self.child_table)
-
-        (self.ref_parent_key, parent_referenced_key) = reference_columns(self.cursor,
-                                                                         self.child_schema, self.child_table,
-                                                                         self.parent_schema, self.parent_table)
+        self.view_name = view_name or "vw_{pt}_{ct}".format(
+            pt=self.parent_table, ct=self.child_table
+        )
+
+        (self.ref_parent_key, parent_referenced_key) = reference_columns(
+            self.cursor, self.child_schema, self.child_table, self.parent_schema, self.parent_table
+        )
         try:
             self.child_pkey = primary_key(self.cursor, self.child_schema, self.child_table)
         except TableHasNoPrimaryKey:
             self.child_pkey = self.ref_parent_key
         self.parent_pkey = primary_key(self.cursor, self.parent_schema, self.parent_table)
 
         assert self.parent_pkey == parent_referenced_key
 
     def create(self) -> bool:
         """
         Creates the merge view on the specified service
         Returns True in case of success
         """
         success = True
-        for sql in [self.__view(),
-                    self.__insert_trigger(),
-                    self.__update_trigger(),
-                    self.__delete_trigger(),
-                    self.__extras()
-                    ]:
+        for sql in [
+            self.__view(),
+            self.__insert_trigger(),
+            self.__update_trigger(),
+            self.__delete_trigger(),
+            self.__extras(),
+        ]:
             try:
                 if sql:
                     self.cursor.execute(sql)
-            except psycopg2.Error as e:
+            except psycopg.Error as e:
                 success = False
-                print("*** Failing:\n{}\n***".format(sql))
+                print(f"*** Failing:\n{sql}\n***")
                 raise e
         self.conn.commit()
         self.conn.close()
         return success
 
     def __view(self) -> str:
         """
@@ -103,24 +110,34 @@
         """
         sql = """
 CREATE OR REPLACE VIEW {vs}.{vn} AS SELECT
   {child_cols},
   {parent_cols}
   FROM {cs}.{ct}
   LEFT JOIN {ps}.{pt} ON {pt}.{prk} = {ct}.{rpk};
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           parent_cols=select_columns(self.cursor, self.parent_schema, self.parent_table, table_alias=self.parent_table, remove_pkey=True),
-           child_cols=select_columns(self.cursor, self.child_schema, self.child_table, table_alias=self.child_table),
-           cs=self.child_schema,
-           ct=self.child_table,
-           ps=self.parent_schema,
-           pt=self.parent_table,
-           rpk=self.ref_parent_key,
-           prk=self.parent_pkey)
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            parent_cols=select_columns(
+                self.cursor,
+                self.parent_schema,
+                self.parent_table,
+                table_alias=self.parent_table,
+                remove_pkey=True,
+            ),
+            child_cols=select_columns(
+                self.cursor, self.child_schema, self.child_table, table_alias=self.child_table
+            ),
+            cs=self.child_schema,
+            ct=self.child_table,
+            ps=self.parent_schema,
+            pt=self.parent_table,
+            rpk=self.ref_parent_key,
+            prk=self.parent_pkey,
+        )
 
         return sql
 
     def __insert_trigger(self) -> str:
         """
 
         :return:
@@ -139,26 +156,37 @@
 LANGUAGE plpgsql;
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_insert ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_insert
   INSTEAD OF INSERT ON {vs}.{vn}
   FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_insert();
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           insert_parent=insert_command(self.cursor, self.parent_schema, self.parent_table,
-                                        remove_pkey=False,
-                                        coalesce_pkey_default=True,
-                                        remap_columns={self.parent_pkey: self.ref_parent_key},
-                                        inner_defaults=self.inner_defaults,
-                                        returning='{ppk} INTO NEW.{prk}'.format(ppk=self.parent_pkey, prk=self.ref_parent_key)),
-           insert_child=insert_command(self.cursor, self.child_schema, self.child_table,
-                                       remove_pkey=False,
-                                       pkey=self.child_pkey)
-           )
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            insert_parent=insert_command(
+                self.cursor,
+                self.parent_schema,
+                self.parent_table,
+                remove_pkey=False,
+                coalesce_pkey_default=True,
+                remap_columns={self.parent_pkey: self.ref_parent_key},
+                inner_defaults=self.inner_defaults,
+                returning="{ppk} INTO NEW.{prk}".format(
+                    ppk=self.parent_pkey, prk=self.ref_parent_key
+                ),
+            ),
+            insert_child=insert_command(
+                self.cursor,
+                self.child_schema,
+                self.child_table,
+                remove_pkey=False,
+                pkey=self.child_pkey,
+            ),
+        )
         return sql
 
     def __update_trigger(self):
         sql = """
 -- UPDATE TRIGGER
 CREATE OR REPLACE FUNCTION {vs}.ft_{vn}_update() RETURNS trigger AS
 $BODY$
@@ -172,20 +200,31 @@
 LANGUAGE plpgsql;
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_update ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_update
   INSTEAD OF UPDATE ON {vs}.{vn}
   FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_update();
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           update_master=update_command(self.cursor, self.parent_schema, self.parent_table,
-                                        remap_columns={self.parent_pkey: self.ref_parent_key}),
-           update_child=update_command(self.cursor, self.child_schema, self.child_table, pkey=self.child_pkey, remove_pkey=False)
-           )
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            update_master=update_command(
+                self.cursor,
+                self.parent_schema,
+                self.parent_table,
+                remap_columns={self.parent_pkey: self.ref_parent_key},
+            ),
+            update_child=update_command(
+                self.cursor,
+                self.child_schema,
+                self.child_table,
+                pkey=self.child_pkey,
+                remove_pkey=False,
+            ),
+        )
         return sql
 
     def __delete_trigger(self):
         sql = """
 CREATE OR REPLACE FUNCTION {vs}.ft_{vn}_delete() RETURNS trigger AS
 $BODY$
 BEGIN
@@ -197,26 +236,31 @@
 LANGUAGE plpgsql;
 
 DROP TRIGGER IF EXISTS tr_{vn}_on_delete ON {vs}.{vn};
 
 CREATE TRIGGER tr_{vn}_on_delete
   INSTEAD OF DELETE ON {vs}.{vn}
   FOR EACH ROW EXECUTE PROCEDURE {vs}.ft_{vn}_delete();
-""".format(vs=self.view_schema,
-           vn=self.view_name,
-           cs=self.child_schema,
-           ct=self.child_table,
-           rpk=self.ref_parent_key,
-           ppk=self.parent_pkey,
-           ps=self.parent_schema,
-           pt=self.parent_table)
+""".format(
+            vs=self.view_schema,
+            vn=self.view_name,
+            cs=self.child_schema,
+            ct=self.child_table,
+            rpk=self.ref_parent_key,
+            ppk=self.parent_pkey,
+            ps=self.parent_schema,
+            pt=self.parent_table,
+        )
         return sql
 
     def __extras(self):
-        sql = ''
+        sql = ""
         if self.pkey_default_value:
-            sql += "ALTER VIEW {vs}.{vn} ALTER {rpk} SET DEFAULT {dv};"\
-                .format(vs=self.view_schema,
-                        vn=self.view_name,
-                        rpk=self.child_pkey,
-                        dv=default_value(self.cursor, self.child_schema, self.child_table, self.child_pkey))
-        return sql
+            sql += "ALTER VIEW {vs}.{vn} ALTER {rpk} SET DEFAULT {dv};".format(
+                vs=self.view_schema,
+                vn=self.view_name,
+                rpk=self.child_pkey,
+                dv=default_value(
+                    self.cursor, self.child_schema, self.child_table, self.child_pkey
+                ),
+            )
+        return sql
```

### Comparing `pirogue-1.4.2/pirogue/utils.py` & `pirogue-2.0.0/pirogue/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-# -*- coding: utf-8 -*-
-from psycopg2.extensions import cursor
+from psycopg import Cursor
 
 from pirogue.exceptions import InvalidColumn, TableHasNoPrimaryKey
-from pirogue.information_schema import columns, primary_key, default_value
+from pirogue.information_schema import columns, default_value, primary_key
 
 
 def table_parts(name: str) -> (str, str):
     """
     Returns a tuple with schema and table names
 
     Parameters
     ----------
     name
         the schema specified name of the table or view.
     """
-    if name and '.' in name:
-        return name.split('.', 1)
+    if name and "." in name:
+        return name.split(".", 1)
     else:
-        return 'public', name
+        return "public", name
 
 
-def select_columns(pg_cur: cursor,
-                   table_schema: str,
-                   table_name: str,
-                   table_type: str = 'table',
-                   table_alias: str = None,
-                   remove_pkey: bool = False,
-                   skip_columns: list = [],
-                   safe_skip_columns: list = [],
-                   columns_list: list = None,
-                   comment_skipped: bool = True,
-                   remap_columns: dict = {},
-                   columns_on_top: list = [],
-                   columns_at_end: list = [],
-                   prefix: str = None,
-                   indent: int = 2,
-                   separate_first: bool = False) -> str:
+def select_columns(
+    pg_cur: Cursor,
+    table_schema: str,
+    table_name: str,
+    table_type: str = "table",
+    table_alias: str = None,
+    remove_pkey: bool = False,
+    skip_columns: list = [],
+    safe_skip_columns: list = [],
+    columns_list: list = None,
+    comment_skipped: bool = True,
+    remap_columns: dict = {},
+    columns_on_top: list = [],
+    columns_at_end: list = [],
+    prefix: str = None,
+    indent: int = 2,
+    separate_first: bool = False,
+) -> str:
     """
     Returns the list of columns to be used in a SELECT command
 
     Parameters
     ----------
     pg_cur
         the psycopg cursor
@@ -75,81 +76,99 @@
     separate_first
         separate the first column with a comma
     """
     try:
         pk_for_sort = primary_key(pg_cur, table_schema, table_name)
     except TableHasNoPrimaryKey:
         pk_for_sort = None
-    cols = sorted(columns_list or columns(pg_cur,
-                                          table_schema=table_schema,
-                                          table_name=table_name,
-                                          table_type=table_type,
-                                          remove_pkey=remove_pkey),
-                  key=lambda col, pk_for_sort=pk_for_sort: __column_priority(col, primary_key=pk_for_sort))
+    cols = sorted(
+        columns_list
+        or columns(
+            pg_cur,
+            table_schema=table_schema,
+            table_name=table_name,
+            table_type=table_type,
+            remove_pkey=remove_pkey,
+        ),
+        key=lambda col, pk_for_sort=pk_for_sort: __column_priority(col, primary_key=pk_for_sort),
+    )
     cols = [col for col in cols if col not in safe_skip_columns]
 
     # check arguments
-    for param, dict_or_list in {'skip_columns': skip_columns,
-                                'remap_columns': remap_columns,
-                                'columns_on_top': columns_on_top,
-                                'columns_at_end': columns_at_end}.items():
+    for param, dict_or_list in {
+        "skip_columns": skip_columns,
+        "remap_columns": remap_columns,
+        "columns_on_top": columns_on_top,
+        "columns_at_end": columns_at_end,
+    }.items():
         for col in dict_or_list:
             if col not in cols:
-                raise InvalidColumn('Invalid column in {param} paramater: "{tab}" has no column "{col}"'
-                                    .format(param=param, tab=table_name, col=col))
+                raise InvalidColumn(
+                    'Invalid column in {param} paramater: "{tab}" has no column "{col}"'.format(
+                        param=param, tab=table_name, col=col
+                    )
+                )
 
     first_column_printed = [separate_first]
 
     def print_comma(first_column_printed, print: bool) -> str:
         if first_column_printed[0]:
             # we can print in any case
-            return ', '
+            return ", "
         elif print:
             # we start printing commas (i.e. not commenting anymore)
             if not first_column_printed[0]:
                 # this is the first column to be printed => no comma
                 first_column_printed[0] = True
-                return ''
+                return ""
             else:
-                return ', '
+                return ", "
         else:
-            return ''
+            return ""
 
-    return '\n{indent}'\
-        .format(indent=indent*' ')\
-        .join(['{skip}{comma}{table_alias}.{column}{col_alias}'
-              .format(comma=print_comma(first_column_printed, col not in skip_columns),
-                      skip='-- ' if col in skip_columns else '',
-                      table_alias=table_alias or table_name,
-                      column=col,
-                      col_alias=__column_alias(col, remap_columns=remap_columns, prefix=prefix, prepend_as=True))
-               for col in cols if (comment_skipped or col not in skip_columns)])
-
-
-def insert_command(pg_cur: cursor,
-                   table_schema: str,
-                   table_name: str,
-                   table_type: str = "table",
-                   table_alias: str = None,
-                   remove_pkey: bool = True,
-                   pkey: str = None,
-                   coalesce_pkey_default: bool = False,
-                   skip_columns: list = [],
-                   comment_skipped: bool = True,
-                   remap_columns: dict = {},
-                   insert_values: dict = {},
-                   columns_on_top: list = [],
-                   columns_at_end: list = [],
-                   prefix: str = None,
-                   returning: str = None,
-                   indent: int = 2,
-                   inner_defaults: dict = {}) -> str:
+    return "\n{indent}".format(indent=indent * " ").join(
+        [
+            "{skip}{comma}{table_alias}.{column}{col_alias}".format(
+                comma=print_comma(first_column_printed, col not in skip_columns),
+                skip="-- " if col in skip_columns else "",
+                table_alias=table_alias or table_name,
+                column=col,
+                col_alias=__column_alias(
+                    col, remap_columns=remap_columns, prefix=prefix, prepend_as=True
+                ),
+            )
+            for col in cols
+            if (comment_skipped or col not in skip_columns)
+        ]
+    )
+
+
+def insert_command(
+    pg_cur: Cursor,
+    table_schema: str,
+    table_name: str,
+    table_type: str = "table",
+    table_alias: str = None,
+    remove_pkey: bool = True,
+    pkey: str = None,
+    coalesce_pkey_default: bool = False,
+    skip_columns: list = [],
+    comment_skipped: bool = True,
+    remap_columns: dict = {},
+    insert_values: dict = {},
+    columns_on_top: list = [],
+    columns_at_end: list = [],
+    prefix: str = None,
+    returning: str = None,
+    indent: int = 2,
+    inner_defaults: dict = {},
+) -> str:
     """
     Creates an INSERT command
-    
+
     Parameters
     ----------
     pg_cur
         the psycopg cursor
     table_schema
         the schema
     table_name
@@ -176,114 +195,139 @@
          bring the columns to the front of the list
     columns_at_end
         bring the columns to the end of the list
     prefix
         add a prefix to the columns (do not applied to remapped columns)
     returning
         returning command
-    indent add
-         an indent in front
+    indent
+         add an indent in front
     inner_defaults
         dictionary of other columns to default to in case the provided value is null (can be used instead of insert_values to make it easier to reuse other columns definitions)
     """
     remove_pkey = remove_pkey and pkey is None
 
     # get columns
     try:
         pk_for_sort = primary_key(pg_cur, table_schema, table_name)
     except TableHasNoPrimaryKey:
         pk_for_sort = None
-    cols = sorted(columns(pg_cur,
-                          table_schema=table_schema,
-                          table_name=table_name,
-                          table_type=table_type,
-                          remove_pkey=remove_pkey),
-                  key=lambda col, pk_for_sort=pk_for_sort: __column_priority(col, primary_key=pk_for_sort))
+    cols = sorted(
+        columns(
+            pg_cur,
+            table_schema=table_schema,
+            table_name=table_name,
+            table_type=table_type,
+            remove_pkey=remove_pkey,
+        ),
+        key=lambda col, pk_for_sort=pk_for_sort: __column_priority(col, primary_key=pk_for_sort),
+    )
 
     if pkey and remove_pkey:
         cols.remove(pkey)
 
     # if no columns, return NULL
     if len([col for col in cols if col not in skip_columns]) == 0:
-        return "-- Do not insert for {} since all columns are skipped".format(table_name)
+        return f"-- Do not insert for {table_name} since all columns are skipped"
 
     if not pkey and coalesce_pkey_default:
         pkey = primary_key(pg_cur, table_schema, table_name)
 
     # check arguments
-    for param, dict_or_list in {'skip_columns': skip_columns,
-                                'remap_columns': remap_columns,
-                                'insert_values': insert_values,
-                                'columns_on_top': columns_on_top,
-                                'columns_at_end': columns_at_end}.items():
+    for param, dict_or_list in {
+        "skip_columns": skip_columns,
+        "remap_columns": remap_columns,
+        "insert_values": insert_values,
+        "columns_on_top": columns_on_top,
+        "columns_at_end": columns_at_end,
+    }.items():
         for col in dict_or_list:
             if col not in cols:
-                raise InvalidColumn('Invalid column in {param} paramater: "{tab}" has no column "{col}"'
-                                    .format(param=param, tab=table_name, col=col))
+                raise InvalidColumn(
+                    'Invalid column in {param} paramater: "{tab}" has no column "{col}"'.format(
+                        param=param, tab=table_name, col=col
+                    )
+                )
 
     def value(col):
         if col in insert_values:
-            return '{val} -- {ori_col}'.format(val=insert_values[col], ori_col=col)
-        cal = __column_alias(col, remap_columns=remap_columns, prefix=prefix, field_if_no_alias=True)
+            return f"{insert_values[col]} -- {col}"
+        cal = __column_alias(
+            col, remap_columns=remap_columns, prefix=prefix, field_if_no_alias=True
+        )
         if coalesce_pkey_default and col == pkey:
-            return 'COALESCE( NEW.{cal}, {pk_def} )'.format(cal=cal,
-                                                            pk_def=default_value(pg_cur, table_schema, table_name, pkey))
+            return "COALESCE( NEW.{cal}, {pk_def} )".format(
+                cal=cal, pk_def=default_value(pg_cur, table_schema, table_name, pkey)
+            )
         elif col in inner_defaults:
             def_col = inner_defaults[col]
             # we don't use COALESCE to deal with empt strings too
             # we use recursion in case we need to call default to obj_id which may be calculated as just above
-            return 'CASE WHEN NEW.{cal} IS NOT NULL AND NEW.{cal}::text <> \'\' THEN NEW.{cal} ELSE {default} END'.format(cal=cal, default=value(def_col))
+            return "CASE WHEN NEW.{cal} IS NOT NULL AND NEW.{cal}::text <> '' THEN NEW.{cal} ELSE {default} END".format(
+                cal=cal, default=value(def_col)
+            )
         else:
-            return 'NEW.{cal}'.format(cal=cal)
+            return f"NEW.{cal}"
 
     next_comma_printed_1 = [False]
     next_comma_printed_2 = [False]
     return """INSERT INTO {s}.{t} (
-{indent}      {cols} 
-{indent}  ) VALUES ( 
+{indent}      {cols}
+{indent}  ) VALUES (
 {indent}      {new_cols}
 {indent}  ){returning};
-""".format(indent=indent*' ',
-           s=table_schema,
-           t=table_name,
-           cols='\n{indent}    '
-                .format(indent=indent*' ')
-                .join(['{skip}{comma}{col}'
-                      .format(indent=indent*' ',
-                              skip='-- ' if col in skip_columns else '',
-                              comma=', ' if __print_comma(next_comma_printed_1, col in skip_columns) else '',
-                              col=col)
-                       for col in cols if (comment_skipped or col not in skip_columns)]),
-           new_cols='\n{indent}    '
-                    .format(indent=indent*' ')
-                    .join(['{skip}{comma}{value}'
-                          .format(skip='-- ' if col in skip_columns else '',
-                                  comma=', ' if __print_comma(next_comma_printed_2, col in skip_columns) else '',
-                                  value=value(col))
-                           for col in cols if (comment_skipped or col not in skip_columns)]),
-           returning=' RETURNING {returning}'.format(indent=4*' ', returning=returning) if returning else '')
-
-
-def update_command(pg_cur: cursor,
-                   table_schema: str,
-                   table_name: str,
-                   table_alias: str = None,
-                   table_type: str = 'table',
-                   remove_pkey: bool = True,
-                   pkey: str = None,
-                   skip_columns: list=[],
-                   comment_skipped: bool = True,
-                   remap_columns: dict = {},
-                   update_values: dict = {},
-                   columns_on_top: list=[],
-                   columns_at_end: list=[],
-                   prefix: str= None,
-                   where_clause: str = None,
-                   indent: int=2,
-                   inner_defaults: dict = {}) -> str:
+""".format(
+        indent=indent * " ",
+        s=table_schema,
+        t=table_name,
+        cols="\n{indent}    ".format(indent=indent * " ").join(
+            [
+                "{skip}{comma}{col}".format(
+                    skip="-- " if col in skip_columns else "",
+                    comma=", " if __print_comma(next_comma_printed_1, col in skip_columns) else "",
+                    col=col,
+                )
+                for col in cols
+                if (comment_skipped or col not in skip_columns)
+            ]
+        ),
+        new_cols="\n{indent}    ".format(indent=indent * " ").join(
+            [
+                "{skip}{comma}{value}".format(
+                    skip="-- " if col in skip_columns else "",
+                    comma=", " if __print_comma(next_comma_printed_2, col in skip_columns) else "",
+                    value=value(col),
+                )
+                for col in cols
+                if (comment_skipped or col not in skip_columns)
+            ]
+        ),
+        returning=f" RETURNING {returning}" if returning else "",
+    )
+
+
+def update_command(
+    pg_cur: Cursor,
+    table_schema: str,
+    table_name: str,
+    table_alias: str = None,
+    table_type: str = "table",
+    remove_pkey: bool = True,
+    pkey: str = None,
+    skip_columns: list = [],
+    comment_skipped: bool = True,
+    remap_columns: dict = {},
+    update_values: dict = {},
+    columns_on_top: list = [],
+    columns_at_end: list = [],
+    prefix: str = None,
+    where_clause: str = None,
+    indent: int = 2,
+    inner_defaults: dict = {},
+) -> str:
     """
     Creates an UPDATE command
 
     Parameters
     ----------
     pg_cur
          the psycopg cursor
@@ -327,106 +371,133 @@
 
     remove_pkey = remove_pkey and pkey is None and where_clause is None
     # get columns
     try:
         pk_for_sort = primary_key(pg_cur, table_schema, table_name)
     except TableHasNoPrimaryKey:
         pk_for_sort = None
-    cols = sorted(columns(pg_cur,
-                          table_schema=table_schema,
-                          table_name=table_name,
-                          table_type=table_type,
-                          remove_pkey=remove_pkey),
-                  key=lambda _col, pk_for_sort=pk_for_sort: __column_priority(_col, primary_key=pk_for_sort))
+    cols = sorted(
+        columns(
+            pg_cur,
+            table_schema=table_schema,
+            table_name=table_name,
+            table_type=table_type,
+            remove_pkey=remove_pkey,
+        ),
+        key=lambda _col, pk_for_sort=pk_for_sort: __column_priority(_col, primary_key=pk_for_sort),
+    )
 
     if pkey and remove_pkey:
         cols.remove(pkey)
 
     # if no columns, return NULL
     if len([col for col in cols if col not in skip_columns]) == 0:
-        return "-- Do not update for {} since all columns are skipped".format(table_name)
+        return f"-- Do not update for {table_name} since all columns are skipped"
 
     if not pkey and not where_clause:
         pkey = primary_key(pg_cur, table_schema, table_name)
 
     # check arguments
-    for param, dict_or_list in {'skip_columns': skip_columns,
-                                'remap_columns': remap_columns,
-                                'update_values': update_values,
-                                'columns_on_top': columns_on_top,
-                                'columns_at_end': columns_at_end}.items():
+    for param, dict_or_list in {
+        "skip_columns": skip_columns,
+        "remap_columns": remap_columns,
+        "update_values": update_values,
+        "columns_on_top": columns_on_top,
+        "columns_at_end": columns_at_end,
+    }.items():
         for col in dict_or_list:
             if col not in cols and col != pkey:
-                raise InvalidColumn('Invalid column in {param} paramater: "{tab}" has no column "{col}"'
-                                    .format(param=param, tab=table_name, col=col))
+                raise InvalidColumn(
+                    'Invalid column in {param} paramater: "{tab}" has no column "{col}"'.format(
+                        param=param, tab=table_name, col=col
+                    )
+                )
 
     next_comma_printed = [False]
 
     def value(col):
         if col in update_values:
             return update_values[col]
-        cal = __column_alias(col, remap_columns=remap_columns, prefix=prefix, field_if_no_alias=True)
+        cal = __column_alias(
+            col, remap_columns=remap_columns, prefix=prefix, field_if_no_alias=True
+        )
         if col in inner_defaults:
             def_col = inner_defaults[col]
             # we don't use COALESCE to deal with empt strings too
             # we use recursion in case we need to call default to obj_id which may be calculated as just above
-            return 'CASE WHEN NEW.{cal} IS NOT NULL AND NEW.{cal}::text <> \'\' THEN NEW.{cal} ELSE {default} END'.format(cal=cal, default=value(def_col))
+            return "CASE WHEN NEW.{cal} IS NOT NULL AND NEW.{cal}::text <> '' THEN NEW.{cal} ELSE {default} END".format(
+                cal=cal, default=value(def_col)
+            )
         else:
-            return 'NEW.{cal}'.format(cal=cal)
+            return f"NEW.{cal}"
 
     return """UPDATE {s}.{t}{a} SET
 {indent}    {cols}
-{indent}  WHERE {where_clause};"""\
-        .format(indent=indent*' ',
-                s=table_schema,
-                t=table_name,
-                a=' {alias}'.format(alias=table_alias) if table_alias else '',
-                cols='\n{indent}    '
-                     .format(indent=indent*' ')
-                     .join(['{skip}{comma}{col} = {new_col}'
-                                .format(indent=indent*' ',
-                                        skip='-- ' if col in skip_columns else '',
-                                        comma=', ' if __print_comma(next_comma_printed, col in skip_columns) else '',
-                                        col=col,
-                                        new_col=value(col))
-                                for col in cols if (comment_skipped or col not in skip_columns)]),
-                where_clause=where_clause or '{pkey} = {pkal}'.format(pkey=pkey,
-                                                                      pkal=update_values.get(pkey,
-                                                                                             'OLD.{cal}'.format(cal=__column_alias(pkey,
-                                                                                                                                   remap_columns=remap_columns,
-                                                                                                                                   prefix=prefix,
-                                                                                                                                   field_if_no_alias=True)))))
-
-
-def __column_alias(column: str,
-                   remap_columns: dict = {},
-                   prefix: str= None,
-                   field_if_no_alias: bool = False,
-                   prepend_as: bool = False) -> list:
+{indent}  WHERE {where_clause};""".format(
+        indent=indent * " ",
+        s=table_schema,
+        t=table_name,
+        a=f" {table_alias}" if table_alias else "",
+        cols="\n{indent}    ".format(indent=indent * " ").join(
+            [
+                "{skip}{comma}{col} = {new_col}".format(
+                    skip="-- " if col in skip_columns else "",
+                    comma=", " if __print_comma(next_comma_printed, col in skip_columns) else "",
+                    col=col,
+                    new_col=value(col),
+                )
+                for col in cols
+                if (comment_skipped or col not in skip_columns)
+            ]
+        ),
+        where_clause=where_clause
+        or "{pkey} = {pkal}".format(
+            pkey=pkey,
+            pkal=update_values.get(
+                pkey,
+                "OLD.{cal}".format(
+                    cal=__column_alias(
+                        pkey, remap_columns=remap_columns, prefix=prefix, field_if_no_alias=True
+                    )
+                ),
+            ),
+        ),
+    )
+
+
+def __column_alias(
+    column: str,
+    remap_columns: dict = {},
+    prefix: str = None,
+    field_if_no_alias: bool = False,
+    prepend_as: bool = False,
+) -> list:
     """
 
     table_alias
     column
     field_if_no_alias if True, return the field if the alias doesn't exist. If False return an empty string
     prepend_as prepend " AS " to the alias
     :return: empty string if there is no alias and (i.e = field name)
     """
-    col_alias = ''
+    col_alias = ""
     if column in remap_columns:
         col_alias = remap_columns[column]
     elif prefix:
         col_alias = prefix + column
     elif field_if_no_alias:
         col_alias = column
     if prepend_as and col_alias:
-        col_alias = ' AS {al}'.format(al=col_alias)
+        col_alias = f" AS {col_alias}"
     return col_alias
 
 
-def __column_priority(column: str, columns_on_top: list=[], columns_at_end: list=[], primary_key: str=None):
+def __column_priority(
+    column: str, columns_on_top: list = [], columns_at_end: list = [], primary_key: str = None
+):
     """
     Returns a value to sort columns first the primary key, then by priority (on top / at end), then alphabetically
     """
     if primary_key is not None and primary_key == column:
         return [-1, column]
     if column in columns_on_top:
         return [0, column]
@@ -445,8 +516,8 @@
     """
     if is_skipped:
         return next_comma_printed[0]
     elif not next_comma_printed[0]:
         next_comma_printed[0] = True
         return False
     else:
-        return True
+        return True
```

### Comparing `pirogue-1.4.2/pirogue.egg-info/PKG-INFO` & `pirogue-2.0.0/pirogue.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.1
 Name: pirogue
-Version: 1.4.2
+Version: 2.0.0
 Summary: pirogue let you dynamically and easily create views in PostgreSQL for inheritance or join scenarios.
-Home-page: https://github.com/opengisch/pirogue
-Download-URL: https://github.com/opengisch/pirogue/archive/__VERSION__.tar.gz
-Author: Denis Rouzaud
 Author-email: Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pirogue/
 Project-URL: repository, https://github.com/opengisch/pirogue
 Project-URL: tracker, https://github.com/opengisch/pirogue/issues
 Keywords: postgres
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: psycopg2-binary
-Requires-Dist: pyyaml
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: psycopg>=3.1.18
 Provides-Extra: test
 Requires-Dist: nose2; extra == "test"
 
 # pirogue
 A tool to automatically create views and triggers on PostgreSQL databases
 
 Read the docs: https://opengisch.github.io/pirogue
-
-
```

### Comparing `pirogue-1.4.2/pirogue.egg-info/SOURCES.txt` & `pirogue-2.0.0/pirogue.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 requirements-test.txt
 requirements.txt
-setup.py
 .github/dependabot.yml
 .github/workflows/docs.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 .github/workflows/wheel.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 pirogue/__init__.py
+pirogue/cli.py
 pirogue/exceptions.py
 pirogue/information_schema.py
 pirogue/multiple_inheritance.py
 pirogue/simple_joins.py
 pirogue/single_inheritance.py
 pirogue/utils.py
 pirogue.egg-info/PKG-INFO
 pirogue.egg-info/SOURCES.txt
 pirogue.egg-info/dependency_links.txt
 pirogue.egg-info/entry_points.txt
 pirogue.egg-info/requires.txt
 pirogue.egg-info/top_level.txt
-scripts/__init__.py
-scripts/pirogue.py
 test/__init__.py
 test/demo_data.sql
 test/multiple_inheritance.yaml
 test/simple_joins.yaml
 test/simple_joins_based_on_view.yaml
 test/test_multiple_inheritance.py
 test/test_simple_inheritance.sh
```

### Comparing `pirogue-1.4.2/pyproject.toml` & `pirogue-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 dynamic = ["version", "readme", "dependencies", "optional-dependencies"]
 
 [project.urls]
 homepage = "https://opengisch.github.io/pirogue/"
 repository = "https://github.com/opengisch/pirogue"
 tracker = "https://github.com/opengisch/pirogue/issues"
 
+[project.scripts]
+pirogue = "pirogue.cli:main"
+
 [tool.setuptools-git-versioning]
 enabled = true
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"], content-type = "text/markdown"}
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies.test = {file = ["requirements-test.txt"]}
```

### Comparing `pirogue-1.4.2/scripts/pirogue.py` & `pirogue-2.0.0/pirogue/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,137 @@
 #!/usr/bin/env python3
 
 import argparse
 import os
+
 import yaml
 
-from pirogue.single_inheritance import SingleInheritance
 from pirogue.multiple_inheritance import MultipleInheritance
 from pirogue.simple_joins import SimpleJoins
+from pirogue.single_inheritance import SingleInheritance
 
 
 def main():
-
     # create the top-level parser
     parser = argparse.ArgumentParser()
-    parser.add_argument("-v", "--version", help="print the version and exit", action='store_true')
+    parser.add_argument("-v", "--version", help="print the version and exit", action="store_true")
 
-    subparsers = parser.add_subparsers(title='commands', description='pirogue command', dest='command')
+    subparsers = parser.add_subparsers(
+        title="commands", description="pirogue command", dest="command"
+    )
 
     # single inheritance view
-    single_inheritance_parser = subparsers.add_parser('single_inheritance', help='create a single inheritance view')
-    single_inheritance_parser.add_argument('parent_table')
-    single_inheritance_parser.add_argument('child_table')
-    single_inheritance_parser.add_argument('-s', '--view-schema', help='schema for the created join view')
-    single_inheritance_parser.add_argument('-v', '--view-name', help='name for the created join view')
-    single_inheritance_parser.add_argument('-d', '--pkey-default-value', action='store_true',
-                                           help='The primary key column of the view will have a default value'
-                                                ' according to the child primary key table')
-    single_inheritance_parser.add_argument('-p', '--pg_service', help='postgres service')
-
+    single_inheritance_parser = subparsers.add_parser(
+        "single_inheritance", help="create a single inheritance view"
+    )
+    single_inheritance_parser.add_argument("parent_table")
+    single_inheritance_parser.add_argument("child_table")
+    single_inheritance_parser.add_argument(
+        "-s", "--view-schema", help="schema for the created join view"
+    )
+    single_inheritance_parser.add_argument(
+        "-v", "--view-name", help="name for the created join view"
+    )
+    single_inheritance_parser.add_argument(
+        "-d",
+        "--pkey-default-value",
+        action="store_true",
+        help="The primary key column of the view will have a default value"
+        " according to the child primary key table",
+    )
+    single_inheritance_parser.add_argument("-p", "--pg_service", help="postgres service")
 
     # multiple inheritance view
-    multiple_inheritance_parser = subparsers.add_parser('multiple_inheritance', help='create a multiple inheritance view')
-    multiple_inheritance_parser.add_argument('definition_file', help='YAML definition of the merge view', type=argparse.FileType('r'))
-    multiple_inheritance_parser.add_argument('-j', '--create-joins', action='store_true',
-                                             help='Create simple join view for all joined tables.')
-    multiple_inheritance_parser.add_argument('-d', '--drop', action='store_true',
-                                             help='Drop existing views, type and triggers.')
-    multiple_inheritance_parser.add_argument('-v', '--var', nargs=3,
-                                             help='Assign variable for running SQL deltas. '
-                                                  'Format is: (string|float|int) name value. ',
-                                             action='append', default=[])
-    multiple_inheritance_parser.add_argument('-p', '--pg_service', help='postgres service')
-
+    multiple_inheritance_parser = subparsers.add_parser(
+        "multiple_inheritance", help="create a multiple inheritance view"
+    )
+    multiple_inheritance_parser.add_argument(
+        "definition_file", help="YAML definition of the merge view", type=argparse.FileType("r")
+    )
+    multiple_inheritance_parser.add_argument(
+        "-j",
+        "--create-joins",
+        action="store_true",
+        help="Create simple join view for all joined tables.",
+    )
+    multiple_inheritance_parser.add_argument(
+        "-d", "--drop", action="store_true", help="Drop existing views, type and triggers."
+    )
+    multiple_inheritance_parser.add_argument(
+        "-v",
+        "--var",
+        nargs=3,
+        help="Assign variable for running SQL deltas. "
+        "Format is: (string|float|int) name value. ",
+        action="append",
+        default=[],
+    )
+    multiple_inheritance_parser.add_argument("-p", "--pg_service", help="postgres service")
 
     # multiple inheritance view
-    simple_joins = subparsers.add_parser('simple_joins', help='create a view for simple joins without any editing capability')
-    simple_joins.add_argument('definition_file', help='YAML definition of the merge view', type=argparse.FileType('r'))
-    simple_joins.add_argument('-p', '--pg_service', help='postgres service')
+    simple_joins = subparsers.add_parser(
+        "simple_joins", help="create a view for simple joins without any editing capability"
+    )
+    simple_joins.add_argument(
+        "definition_file", help="YAML definition of the merge view", type=argparse.FileType("r")
+    )
+    simple_joins.add_argument("-p", "--pg_service", help="postgres service")
 
     args = parser.parse_args()
 
     # print the version and exit
     if args.version:
         import pkg_resources
-        print('pirogue version: {}'.format(pkg_resources.get_distribution('pirogue').version))
+
+        print("pirogue version: {}".format(pkg_resources.get_distribution("pirogue").version))
         parser.exit()
 
     # if no command is passed, print the help and exit
     if not args.command:
         parser.print_help()
         parser.exit()
 
     exit_val = 0
 
     if args.pg_service:
         pg_service = args.pg_service
     else:
-        pg_service = os.getenv('PGSERVICE')
+        pg_service = os.getenv("PGSERVICE")
 
-    if args.command == 'single_inheritance':
-        success = SingleInheritance(parent_table=args.parent_table,
-                                    child_table=args.child_table,
-                                    pg_service=pg_service,
-                                    view_schema=args.view_schema,
-                                    view_name=args.view_name,
-                                    pkey_default_value=args.pkey_default_value).create()
+    if args.command == "single_inheritance":
+        success = SingleInheritance(
+            parent_table=args.parent_table,
+            child_table=args.child_table,
+            pg_service=pg_service,
+            view_schema=args.view_schema,
+            view_name=args.view_name,
+            pkey_default_value=args.pkey_default_value,
+        ).create()
         if not success:
             exit_val = 1
 
-    elif args.command == 'multiple_inheritance':
+    elif args.command == "multiple_inheritance":
         yaml_definition = yaml.safe_load(args.definition_file)
         variables = {}
         for v in args.var or ():
-            if v[0] == 'float':
+            if v[0] == "float":
                 variables[v[1]] = float(v[2])
-            elif v[0] == 'int':
+            elif v[0] == "int":
                 variables[v[1]] = int(v[2])
             else:
                 variables[v[1]] = v[2]
-        MultipleInheritance(yaml_definition,
-                            variables=variables,
-                            create_joins=args.create_joins,
-                            pg_service=pg_service).create()
+        MultipleInheritance(
+            yaml_definition,
+            variables=variables,
+            create_joins=args.create_joins,
+            pg_service=pg_service,
+        ).create()
 
-    elif args.command == 'simple_joins':
+    elif args.command == "simple_joins":
         yaml_definition = yaml.safe_load(args.definition_file)
         SimpleJoins(yaml_definition, pg_service=pg_service).create()
 
-
     exit(exit_val)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pirogue-1.4.2/test/demo_data.sql` & `pirogue-2.0.0/test/demo_data.sql`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -49,8 +49,8 @@
    	fk_animal integer REFERENCES pirogue_test.animal,
 	weight double precision);
 
 
 INSERT INTO pirogue_test.cat_breed (id, breed_name) VALUES (1, 'Abyssinian');
 INSERT INTO pirogue_test.cat_breed (id, breed_name) VALUES (2, 'American Bobtail');
 INSERT INTO pirogue_test.dog_breed (id, breed_name) VALUES (1, 'Afghan Hound');
-INSERT INTO pirogue_test.dog_breed (id, breed_name) VALUES (2, 'Barbet');
+INSERT INTO pirogue_test.dog_breed (id, breed_name) VALUES (2, 'Barbet');
```

### Comparing `pirogue-1.4.2/test/test_multiple_inheritance.py` & `pirogue-2.0.0/test/test_multiple_inheritance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,100 @@
 #! /usr/bin/env python
 
 import unittest
+
+import psycopg
 import yaml
-import psycopg2
-import psycopg2.extras
+
 from pirogue import MultipleInheritance
-from pirogue.utils import default_value
 from pirogue.exceptions import InvalidDefinition
+from pirogue.utils import default_value
 
-pg_service = 'pirogue_test'
+pg_service = "pirogue_test"
 
 
 class TestMultipleInheritance(unittest.TestCase):
-
     def setUp(self):
-        self.conn = psycopg2.connect("service={0}".format(pg_service))
+        self.conn = psycopg.connect(f"service={pg_service}")
         self.cur = self.conn.cursor()
 
         sql = open("test/demo_data.sql").read()
         self.cur.execute(sql)
         self.conn.commit()
 
     def tearDown(self):
         self.conn.close()
 
     def test_insert_update_delete(self):
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
         MultipleInheritance(yaml_definition, pg_service=pg_service).create()
 
         # insert
-        self.cur.execute("INSERT INTO pirogue_test.vw_merge_animal (animal_type,name,year,fk_cat_breed,eye_color) VALUES ('cat','felix',1985,2,'black');")
-        self.cur.execute("SELECT animal_type, year, fk_cat_breed FROM pirogue_test.vw_merge_animal WHERE name = 'felix';")
+        self.cur.execute(
+            "INSERT INTO pirogue_test.vw_merge_animal (animal_type,name,year,fk_cat_breed,eye_color) VALUES ('cat','felix',1985,2,'black');"
+        )
+        self.cur.execute(
+            "SELECT animal_type, year, fk_cat_breed FROM pirogue_test.vw_merge_animal WHERE name = 'felix';"
+        )
         res = self.cur.fetchone()
-        self.assertEqual(res[0], 'cat')
+        self.assertEqual(res[0], "cat")
         self.assertEqual(res[1], 1985)
         self.assertEqual(res[2], 2)
         # update
         self.cur.execute("SELECT * FROM pirogue_test.cat WHERE eye_color = 'black';")
         self.assertIsNotNone(self.cur.fetchone())
-        self.cur.execute("UPDATE pirogue_test.vw_merge_animal SET animal_type = 'dog' WHERE name = 'felix';")
+        self.cur.execute(
+            "UPDATE pirogue_test.vw_merge_animal SET animal_type = 'dog' WHERE name = 'felix';"
+        )
         self.cur.execute("SELECT * FROM pirogue_test.cat WHERE eye_color = 'black';")
         self.assertIsNone(self.cur.fetchone())
         # delete
         self.cur.execute("SELECT * FROM pirogue_test.vw_merge_animal WHERE name = 'felix';")
         self.assertIsNotNone(self.cur.fetchone())
         self.cur.execute("DELETE FROM pirogue_test.vw_merge_animal WHERE name = 'felix';")
         self.cur.execute("SELECT * FROM pirogue_test.vw_merge_animal WHERE name = 'felix';")
         self.assertIsNone(self.cur.fetchone())
 
     def test_type_change_not_allowed(self):
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
-        yaml_definition['view_name'] = 'vw_animal_no_type_change'
-        yaml_definition['allow_type_change'] = False
+        yaml_definition["view_name"] = "vw_animal_no_type_change"
+        yaml_definition["allow_type_change"] = False
         MultipleInheritance(yaml_definition, pg_service=pg_service).create()
-        self.cur.execute("INSERT INTO pirogue_test.vw_animal_no_type_change (animal_type,name,year,fk_cat_breed,eye_color) VALUES ('dog','albert',1933,2,'yellow');")
+        self.cur.execute(
+            "INSERT INTO pirogue_test.vw_animal_no_type_change (animal_type,name,year,fk_cat_breed,eye_color) VALUES ('dog','albert',1933,2,'yellow');"
+        )
         error_caught = False
         try:
-            self.cur.execute("UPDATE pirogue_test.vw_animal_no_type_change SET animal_type = 'cat';")
-        except psycopg2.errors.RaiseException:
+            self.cur.execute(
+                "UPDATE pirogue_test.vw_animal_no_type_change SET animal_type = 'cat';"
+            )
+        except psycopg.errors.RaiseException:
             error_caught = True
         self.assertTrue(error_caught)
 
     def test_invalid_definition(self):
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
-        yaml_definition['MyBadKey'] = 'Ouch'
+        yaml_definition["MyBadKey"] = "Ouch"
         error_caught = False
         try:
             MultipleInheritance(yaml_definition, pg_service=pg_service).create()
         except InvalidDefinition:
             error_caught = True
             self.assertTrue(error_caught)
 
     def test_pkey_default_value(self):
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
-        yaml_definition['pkey_default_value'] = True
+        yaml_definition["pkey_default_value"] = True
         MultipleInheritance(yaml_definition, pg_service=pg_service).create()
-        self.assertEqual(default_value(self.cur, 'pirogue_test', 'animal', 'aid'), default_value(self.cur, 'pirogue_test', 'vw_merge_animal', 'aid'))
+        self.assertEqual(
+            default_value(self.cur, "pirogue_test", "animal", "aid"),
+            default_value(self.cur, "pirogue_test", "vw_merge_animal", "aid"),
+        )
 
     def test_merge_no_columns(self):
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
-        yaml_definition['joins']['aardvark']['skip_columns'] = ['aid', 'father']
+        yaml_definition["joins"]["aardvark"]["skip_columns"] = ["aid", "father"]
         MultipleInheritance(yaml_definition, pg_service=pg_service).create()
 
 
-
-
-
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pirogue-1.4.2/test/test_simple_inheritance.sh` & `pirogue-2.0.0/test/test_simple_inheritance.sh`

 * *Files identical despite different names*

### Comparing `pirogue-1.4.2/test/test_simple_joins.py` & `pirogue-2.0.0/test/test_simple_joins.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #! /usr/bin/env python
 
 import unittest
+
+import psycopg
 import yaml
-import psycopg2
-import psycopg2.extras
-from pirogue import SimpleJoins, MultipleInheritance
+
+from pirogue import MultipleInheritance, SimpleJoins
 from pirogue.exceptions import InvalidDefinition
 
-pg_service = 'pirogue_test'
+pg_service = "pirogue_test"
 
 
 class TestSimpleJoins(unittest.TestCase):
-
     def setUp(self):
-        self.conn = psycopg2.connect("service={0}".format(pg_service))
+        self.conn = psycopg.connect(f"service={pg_service}")
         self.cur = self.conn.cursor()
 
         sql = open("test/demo_data.sql").read()
         self.cur.execute(sql)
         self.conn.commit()
 
     def tearDown(self):
@@ -31,18 +31,18 @@
         yaml_definition = yaml.safe_load(open("test/multiple_inheritance.yaml"))
         MultipleInheritance(yaml_definition, pg_service=pg_service).create()
         yaml_definition = yaml.safe_load(open("test/simple_joins_based_on_view.yaml"))
         SimpleJoins(yaml_definition, pg_service=pg_service).create()
 
     def test_invalid_definition(self):
         yaml_definition = yaml.safe_load(open("test/simple_joins.yaml"))
-        yaml_definition['MyBadKey'] = 'Ouch'
+        yaml_definition["MyBadKey"] = "Ouch"
         error_caught = False
         try:
             SimpleJoins(yaml_definition, pg_service=pg_service).create()
         except InvalidDefinition:
             error_caught = True
         self.assertTrue(error_caught)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

