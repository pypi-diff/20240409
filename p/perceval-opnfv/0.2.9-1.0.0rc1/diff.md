# Comparing `tmp/perceval_opnfv-0.2.9.tar.gz` & `tmp/perceval_opnfv-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_opnfv-0.2.9.tar", max compression
+gzip compressed data, was "perceval_opnfv-1.0.0rc1.tar", max compression
```

## Comparing `perceval_opnfv-0.2.9.tar` & `perceval_opnfv-1.0.0rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      292 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/LICENSE
--rw-r--r--   0        0        0      964 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/NEWS
--rw-r--r--   0        0        0     2250 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/README.md
--rw-r--r--   0        0        0        0 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/perceval/backends/opnfv/__init__.py
--rw-r--r--   0        0        0       86 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/perceval/backends/opnfv/_version.py
--rw-r--r--   0        0        0     7996 2023-04-26 14:45:43.086613 perceval_opnfv-0.2.9/perceval/backends/opnfv/functest.py
--rw-r--r--   0        0        0     1387 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/base.py
--rw-r--r--   0        0        0    46769 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/data/functest/functest_results.json
--rw-r--r--   0        0        0      101 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/data/functest/functest_results_empty.json
--rw-r--r--   0        0        0    41641 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/data/functest/functest_results_page_1.json
--rw-r--r--   0        0        0     5312 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/data/functest/functest_results_page_2.json
--rwxr-xr-x   0        0        0     1017 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/run_tests.py
--rw-r--r--   0        0        0    13686 2023-04-26 14:45:43.090613 perceval_opnfv-0.2.9/tests/test_functest.py
--rw-r--r--   0        0        0     3463 1970-01-01 00:00:00.000000 perceval_opnfv-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      329 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2481 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0     2250 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/perceval/backends/opnfv/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/perceval/backends/opnfv/_version.py
+-rw-r--r--   0        0        0     7996 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/perceval/backends/opnfv/functest.py
+-rw-r--r--   0        0        0     1405 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1887 2024-04-09 16:14:50.334790 perceval_opnfv-1.0.0rc1/tests/base.py
+-rw-r--r--   0        0        0    46769 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results.json
+-rw-r--r--   0        0        0      101 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results_empty.json
+-rw-r--r--   0        0        0    41641 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results_page_1.json
+-rw-r--r--   0        0        0     5312 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results_page_2.json
+-rwxr-xr-x   0        0        0     1017 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    13686 2024-04-09 16:14:50.338790 perceval_opnfv-1.0.0rc1/tests/test_functest.py
+-rw-r--r--   0        0        0     3381 1970-01-01 00:00:00.000000 perceval_opnfv-1.0.0rc1/PKG-INFO
```

### Comparing `perceval_opnfv-0.2.9/LICENSE` & `perceval_opnfv-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/README.md` & `perceval_opnfv-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Functest
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-opnfv on your system: packages or source
```

### Comparing `perceval_opnfv-0.2.9/perceval/backends/opnfv/functest.py` & `perceval_opnfv-1.0.0rc1/perceval/backends/opnfv/functest.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     The `url` will be set as the origin of the data.
 
     :param url: Functest URL
     :param tag: label used to mark the data
     :param archive: archive to store/retrieve items
     :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.6.0'
+    version = '1.0.0'
 
     CATEGORIES = [CATEGORY_FUNCTEST]
     EXTRA_SEARCH_FIELDS = {
         'project_name': ['project_name']
     }
 
     def __init__(self, url, tag=None, archive=None, ssl_verify=True):
```

### Comparing `perceval_opnfv-0.2.9/pyproject.toml` & `perceval_opnfv-1.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-opnfv"
-version = "0.2.9"
+version = "1.0.0-rc.1"
 description = "Bundle of Perceval backends for OPNFV ecosystem."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -25,27 +25,27 @@
 include = [
     { path = "AUTHORS", format = "sdist" },
     { path = "NEWS", format = "sdist" },
     { path = "README.md", format = "sdist" },
 ]
 
 classifiers = [
-   "Development Status :: 4 - Beta",
+   "Development Status :: 5 - Production/Stable",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Topic :: Software Development",
    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
    "Programming Language :: Python :: 3"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chaoss/grimoirelab-perceval-opnfv/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 requests = "^2.7.0"
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 perceval = { version = ">=0.19", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 httpretty = "1.0.2"
```

### Comparing `perceval_opnfv-0.2.9/tests/base.py` & `perceval_opnfv-1.0.0rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/tests/data/functest/functest_results.json` & `perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/tests/data/functest/functest_results_page_1.json` & `perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/tests/data/functest/functest_results_page_2.json` & `perceval_opnfv-1.0.0rc1/tests/data/functest/functest_results_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/tests/run_tests.py` & `perceval_opnfv-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/tests/test_functest.py` & `perceval_opnfv-1.0.0rc1/tests/test_functest.py`

 * *Files identical despite different names*

### Comparing `perceval_opnfv-0.2.9/PKG-INFO` & `perceval_opnfv-1.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: perceval-opnfv
-Version: 0.2.9
+Version: 1.0.0rc1
 Summary: Bundle of Perceval backends for OPNFV ecosystem.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: grimoirelab-toolkit (>=0.3)
 Requires-Dist: perceval (>=0.19)
 Requires-Dist: requests (>=2.7.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-perceval-opnfv/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-perceval-opnfv
 Description-Content-Type: text/markdown
@@ -34,15 +32,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Functest
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-opnfv on your system: packages or source
```

