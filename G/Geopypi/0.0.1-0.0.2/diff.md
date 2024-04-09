# Comparing `tmp/Geopypi-0.0.1.tar.gz` & `tmp/Geopypi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Geopypi-0.0.1.tar", last modified: Wed Feb 14 19:16:31 2024, max compression
+gzip compressed data, was "Geopypi-0.0.2.tar", last modified: Tue Apr  9 16:37:38 2024, max compression
```

## Comparing `Geopypi-0.0.1.tar` & `Geopypi-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.258241 Geopypi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.246241 Geopypi-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.250241 Geopypi-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-14 19:16:11.000000 Geopypi-0.0.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/Geopypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-14 19:16:31.000000 Geopypi-0.0.1/Geopypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 19:16:11.000000 Geopypi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-14 19:16:11.000000 Geopypi-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-14 19:16:31.258241 Geopypi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-14 19:16:11.000000 Geopypi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/geopypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-14 19:16:11.000000 Geopypi-0.0.1/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/geopypi/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-14 19:16:11.000000 Geopypi-0.0.1/geopypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-14 19:16:11.000000 Geopypi-0.0.1/geopypi/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-14 19:16:11.000000 Geopypi-0.0.1/geopypi/geopypi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-02-14 19:16:11.000000 Geopypi-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-14 19:16:11.000000 Geopypi-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-14 19:16:11.000000 Geopypi-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-14 19:16:11.000000 Geopypi-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 19:16:31.258241 Geopypi-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 19:16:31.254241 Geopypi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-14 19:16:11.000000 Geopypi-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-14 19:16:11.000000 Geopypi-0.0.1/tests/test_geopypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.608256 Geopypi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.596256 Geopypi-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.600256 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.600256 Geopypi-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.608256 Geopypi-0.0.2/Geopypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:37:27.000000 Geopypi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 16:37:27.000000 Geopypi-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 16:37:38.608256 Geopypi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 16:37:27.000000 Geopypi-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    30850 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47264 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/geopypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/geopypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/geopypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-09 16:37:27.000000 Geopypi-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 16:37:27.000000 Geopypi-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:37:27.000000 Geopypi-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 16:37:27.000000 Geopypi-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:37:38.608256 Geopypi-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 16:37:27.000000 Geopypi-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 16:37:27.000000 Geopypi-0.0.2/tests/test_geopypi.py
```

### Comparing `Geopypi-0.0.1/.github/workflows/docs-build.yml` & `Geopypi-0.0.2/.github/workflows/docs-build.yml`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                   gdalinfo --version
             - name: Install dependencies
               run: |
                   pip install --no-cache-dir Cython
                   pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
-              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git" --ignore-words-list="aci,acount,hist"
+              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git, *data_types.ipynb" --ignore-words-list="aci,acount,hist,meni,Pakages"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
             # - name: Deploy to Netlify
```

### Comparing `Geopypi-0.0.1/.github/workflows/docs.yml` & `Geopypi-0.0.2/.github/workflows/docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,13 @@
               run: |
                   python -m pip install --upgrade pip
                   pip install --user --no-cache-dir Cython
                   pip install --user -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
               run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
+                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git, *data_types.ipynb" --ignore-words-list="aci,hist,meni,Pakages"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - run: mkdocs gh-deploy --force
```

### Comparing `Geopypi-0.0.1/.github/workflows/installation.yml` & `Geopypi-0.0.2/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/.github/workflows/macos.yml` & `Geopypi-0.0.2/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/.github/workflows/pypi.yml` & `Geopypi-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/.github/workflows/ubuntu.yml` & `Geopypi-0.0.2/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/.github/workflows/windows.yml` & `Geopypi-0.0.2/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/.gitignore` & `Geopypi-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/Geopypi.egg-info/PKG-INFO` & `Geopypi-0.0.2/Geopypi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
 Provides-Extra: all
 Requires-Dist: Geopypi[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # Geopypi
```

### Comparing `Geopypi-0.0.1/PKG-INFO` & `Geopypi-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
 Provides-Extra: all
 Requires-Dist: Geopypi[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # Geopypi
```

### Comparing `Geopypi-0.0.1/docs/contributing.md` & `Geopypi-0.0.2/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/docs/installation.md` & `Geopypi-0.0.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.1/mkdocs.yml` & `Geopypi-0.0.2/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -43,18 +43,18 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: True
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["*ignore.ipynb"]
+          execute_ignore: ["examples/KH_Shakibul_Islam_lab4.ipynb","examples/KH_Shakibul_Islam_lab5.ipynb" ]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -77,10 +77,18 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Metaliguns77/Geopypi/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/KH_Shakibul_Islam_lab4.ipynb
+        - examples/KH_Shakibul_Islam_lab5.ipynb
+    - Labs:
+        -labs/KH_Shakibul_Islam_lab4.ipynb
+        -labs/KH_Shakibul_Islam_lab5.ipynb
+        
     - API Reference:
           - geopypi module: geopypi.md
           - common module: common.md
+
+
```

### Comparing `Geopypi-0.0.1/pyproject.toml` & `Geopypi-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Geopypi"
-version = "0.0.1"
+version = "0.0.2"
 dynamic = [
     "dependencies",
 ]
 description = "This is a python package for batch geoprocessing."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.2"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

