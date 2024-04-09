# Comparing `tmp/Geopypi-0.0.2.tar.gz` & `tmp/Geopypi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Geopypi-0.0.2.tar", last modified: Tue Apr  9 16:37:38 2024, max compression
+gzip compressed data, was "Geopypi-0.0.3.tar", last modified: Tue Apr  9 19:57:16 2024, max compression
```

## Comparing `Geopypi-0.0.2.tar` & `Geopypi-0.0.3.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.608256 Geopypi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.596256 Geopypi-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.600256 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.600256 Geopypi-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 16:37:27.000000 Geopypi-0.0.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.608256 Geopypi-0.0.2/Geopypi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 16:37:38.000000 Geopypi-0.0.2/Geopypi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:37:27.000000 Geopypi-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 16:37:27.000000 Geopypi-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 16:37:38.608256 Geopypi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 16:37:27.000000 Geopypi-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    30850 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    47264 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/europe_110.geo.json
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/geopypi.md
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 16:37:27.000000 Geopypi-0.0.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/geopypi/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-09 16:37:27.000000 Geopypi-0.0.2/geopypi/geopypi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-09 16:37:27.000000 Geopypi-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 16:37:27.000000 Geopypi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:37:27.000000 Geopypi-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 16:37:27.000000 Geopypi-0.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:37:38.608256 Geopypi-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:37:38.604256 Geopypi-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 16:37:27.000000 Geopypi-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 16:37:27.000000 Geopypi-0.0.2/tests/test_geopypi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.838397 Geopypi-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.842397 Geopypi-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.842397 Geopypi-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-09 19:57:03.000000 Geopypi-0.0.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/Geopypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 19:57:16.000000 Geopypi-0.0.3/Geopypi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:57:03.000000 Geopypi-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 19:57:03.000000 Geopypi-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-09 19:57:16.846397 Geopypi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-09 19:57:03.000000 Geopypi-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    30850 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47264 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab6.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/geopypi.md
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 19:57:03.000000 Geopypi-0.0.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/geopypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 19:57:03.000000 Geopypi-0.0.3/geopypi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 19:57:03.000000 Geopypi-0.0.3/geopypi/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-09 19:57:03.000000 Geopypi-0.0.3/geopypi/geopypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 19:57:03.000000 Geopypi-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 19:57:03.000000 Geopypi-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 19:57:03.000000 Geopypi-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 19:57:03.000000 Geopypi-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:57:16.846397 Geopypi-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:57:16.846397 Geopypi-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 19:57:03.000000 Geopypi-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-09 19:57:03.000000 Geopypi-0.0.3/tests/test_geopypi.py
```

### Comparing `Geopypi-0.0.2/.github/workflows/docs-build.yml` & `Geopypi-0.0.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/docs.yml` & `Geopypi-0.0.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/installation.yml` & `Geopypi-0.0.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/macos.yml` & `Geopypi-0.0.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/pypi.yml` & `Geopypi-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/ubuntu.yml` & `Geopypi-0.0.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.github/workflows/windows.yml` & `Geopypi-0.0.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/.gitignore` & `Geopypi-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/Geopypi.egg-info/PKG-INFO` & `Geopypi-0.0.3/Geopypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Geopypi-0.0.2/Geopypi.egg-info/SOURCES.txt` & `Geopypi-0.0.3/Geopypi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 docs/faq.md
 docs/geopypi.md
 docs/index.md
 docs/installation.md
 docs/usage.md
 docs/examples/KH_Shakibul_Islam_lab4.ipynb
 docs/examples/KH_Shakibul_Islam_lab5.ipynb
+docs/examples/KH_Shakibul_Islam_lab6.ipynb
 docs/examples/europe_110.geo.json
 docs/examples/examples.ipynb
 docs/examples/intro.ipynb
+docs/examples/vector.ipynb
 docs/overrides/main.html
 geopypi/__init__.py
 geopypi/common.py
 geopypi/geopypi.py
 tests/__init__.py
 tests/test_geopypi.py
```

### Comparing `Geopypi-0.0.2/PKG-INFO` & `Geopypi-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geopypi
-Version: 0.0.2
+Version: 0.0.3
 Summary: This is a python package for batch geoprocessing.
 Author-email: KH Shakibul Islam <kshakibu@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/Metaliguns77/Geopypi
 Keywords: Geopypi
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Geopypi-0.0.2/docs/contributing.md` & `Geopypi-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab4.ipynb` & `Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab4.ipynb`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/docs/examples/KH_Shakibul_Islam_lab5.ipynb` & `Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab5.ipynb`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/docs/examples/europe_110.geo.json` & `Geopypi-0.0.3/docs/examples/europe_110.geo.json`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/docs/examples/examples.ipynb` & `Geopypi-0.0.3/docs/examples/KH_Shakibul_Islam_lab6.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883463541666666%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, "*

 * *            "'[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/examples.ipynb#scrollTo=vsp9e6EfuWz6)\\n')], "*

 * *            "delete: [0]}}, 1: {'execution_count': 3, 'outputs': {0: {'data': "*

 * *            "{'application/vnd.jupyter.widget-view+json': {'model_id': "*

 * *            "'5e628a63273f40f3a39de3cb40a449c9'}}, 'execution_count': 3}}}, 2: {'execution_count':  […]*

```diff
@@ -1,50 +1,50 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/KH_Shakibul_Islam_lab5.ipynb)\n",
+                "[![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Metaliguns77/Geopypi/blob/main/docs/examples/examples.ipynb#scrollTo=vsp9e6EfuWz6)\n",
                 "\n",
                 "## A basic python package for CNN networking model\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "1aafdb20184145ac8503801b4ad0d856",
+                            "model_id": "5e628a63273f40f3a39de3cb40a449c9",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
                             "Map(center=[40, -100], controls=(ZoomControl(options=['position', 'zoom_in_text', 'zoom_in_title', 'zoom_out_t\u2026"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import geopypi\n",
                 "m = geopypi.Map()\n",
                 "m.add_basemap(\"OpenTopoMap\")\n",
                 "m"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Requirement already satisfied: geopypi in c:\\users\\shaki\\anaconda3\\envs\\geo\\lib\\site-packages (0.0.1)\n",
```

### Comparing `Geopypi-0.0.2/docs/installation.md` & `Geopypi-0.0.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `Geopypi-0.0.2/mkdocs.yml` & `Geopypi-0.0.3/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,16 @@
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Metaliguns77/Geopypi/issues
     - Examples:
         - examples/intro.ipynb
         - examples/KH_Shakibul_Islam_lab4.ipynb
         - examples/KH_Shakibul_Islam_lab5.ipynb
+        - examples/KH_Shakibul_Islam_lab6.ipynb
+        - examples/vector.ipynb
     - Labs:
         -labs/KH_Shakibul_Islam_lab4.ipynb
         -labs/KH_Shakibul_Islam_lab5.ipynb
         
     - API Reference:
           - geopypi module: geopypi.md
           - common module: common.md
```

### Comparing `Geopypi-0.0.2/pyproject.toml` & `Geopypi-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Geopypi"
-version = "0.0.2"
+version = "0.0.3"
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
-current_version = "0.0.2"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

