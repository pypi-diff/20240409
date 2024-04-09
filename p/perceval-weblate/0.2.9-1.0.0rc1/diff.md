# Comparing `tmp/perceval_weblate-0.2.9.tar.gz` & `tmp/perceval_weblate-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_weblate-0.2.9.tar", max compression
+gzip compressed data, was "perceval_weblate-1.0.0rc1.tar", max compression
```

## Comparing `perceval_weblate-0.2.9.tar` & `perceval_weblate-1.0.0rc1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      119 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/LICENSE
--rw-r--r--   0        0        0     1104 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/NEWS
--rw-r--r--   0        0        0     2187 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/README.md
--rw-r--r--   0        0        0        0 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/__init__.py
--rw-r--r--   0        0        0       86 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/_version.py
--rw-r--r--   0        0        0    14043 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/perceval/backends/weblate/weblate.py
--rw-r--r--   0        0        0     1385 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0     1832 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/base.py
--rw-r--r--   0        0        0      981 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes.json
--rw-r--r--   0        0        0     1922 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_archived.json
--rw-r--r--   0        0        0     8490 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_expected.json
--rw-r--r--   0        0        0     1086 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_page_2.json
--rw-r--r--   0        0        0      719 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_unit.json
--rw-r--r--   0        0        0      359 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_1.json
--rw-r--r--   0        0        0      354 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_2.json
--rw-r--r--   0        0        0       31 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/data/weblate/weblate_user_no_permission.json
--rw-r--r--   0        0        0     1007 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/run_tests.py
--rw-r--r--   0        0        0    16895 2023-04-26 14:45:56.183194 perceval_weblate-0.2.9/tests/test_weblate.py
--rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 perceval_weblate-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      196 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2653 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0     2187 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/_version.py
+-rw-r--r--   0        0        0    14043 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/perceval/backends/weblate/weblate.py
+-rw-r--r--   0        0        0     1403 2024-04-09 16:15:58.085415 perceval_weblate-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     1832 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/base.py
+-rw-r--r--   0        0        0      981 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes.json
+-rw-r--r--   0        0        0     1922 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_archived.json
+-rw-r--r--   0        0        0     8490 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_expected.json
+-rw-r--r--   0        0        0     1086 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_page_2.json
+-rw-r--r--   0        0        0      719 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_unit.json
+-rw-r--r--   0        0        0      359 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_1.json
+-rw-r--r--   0        0        0      354 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_2.json
+-rw-r--r--   0        0        0       31 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_user_no_permission.json
+-rw-r--r--   0        0        0     1007 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    16895 2024-04-09 16:15:58.089415 perceval_weblate-1.0.0rc1/tests/test_weblate.py
+-rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 perceval_weblate-1.0.0rc1/PKG-INFO
```

### Comparing `perceval_weblate-0.2.9/LICENSE` & `perceval_weblate-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/README.md` & `perceval_weblate-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Weblate
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-weblate on your system: packages or source
```

### Comparing `perceval_weblate-0.2.9/perceval/backends/weblate/weblate.py` & `perceval_weblate-1.0.0rc1/perceval/backends/weblate/weblate.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     :param sleep_for_rate: sleep until rate limit is reset
     :param min_rate_to_sleep: minimum rate needed to sleep until
          it will be reset
     :param sleep_time: time (in seconds) to sleep in case
         of connection problems
     :param ssl_verify: enable/disable SSL verification
     """
-    version = '0.1.0'
+    version = '1.0.0'
 
     CATEGORIES = [CATEGORY_CHANGE]
 
     def __init__(self, url, project=None, api_token=None, tag=None, archive=None,
                  sleep_for_rate=False, min_rate_to_sleep=MIN_RATE_LIMIT,
                  max_retries=MAX_RETRIES, sleep_time=DEFAULT_SLEEP_TIME, ssl_verify=True):
```

### Comparing `perceval_weblate-0.2.9/pyproject.toml` & `perceval_weblate-1.0.0rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-weblate"
-version = "0.2.9"
+version = "1.0.0-rc.1"
 description = "Bundle of Perceval backends for Weblate."
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
 "Bug Tracker" = "https://github.com/chaoss/grimoirelab-perceval-weblate/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
 requests = "^2.7.0"
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 perceval = { version = ">=0.19", allow-prereleases = true }
 
 [tool.poetry.dev-dependencies]
 httpretty = "1.0.2"
```

### Comparing `perceval_weblate-0.2.9/tests/base.py` & `perceval_weblate-1.0.0rc1/tests/base.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes.json` & `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_archived.json` & `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_archived.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_expected.json` & `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_expected.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/data/weblate/weblate_changes_page_2.json` & `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_changes_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/data/weblate/weblate_unit.json` & `perceval_weblate-1.0.0rc1/tests/data/weblate/weblate_unit.json`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/run_tests.py` & `perceval_weblate-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/tests/test_weblate.py` & `perceval_weblate-1.0.0rc1/tests/test_weblate.py`

 * *Files identical despite different names*

### Comparing `perceval_weblate-0.2.9/PKG-INFO` & `perceval_weblate-1.0.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: perceval-weblate
-Version: 0.2.9
+Version: 1.0.0rc1
 Summary: Bundle of Perceval backends for Weblate.
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
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-perceval-weblate/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-perceval-weblate
 Description-Content-Type: text/markdown
@@ -34,15 +32,15 @@
 
 The backends currently managed by this package support the next repositories:
 
 * Weblate
 
 ## Requirements
 
- * Python >= 3.7
+ * Python >= 3.8
 
 You will also need some other libraries for running the tool, you can find the
 whole list of dependencies in [pyproject.toml](pyproject.toml) file.
 
 ## Installation
 
 There are several ways to install perceval-weblate on your system: packages or source
```

