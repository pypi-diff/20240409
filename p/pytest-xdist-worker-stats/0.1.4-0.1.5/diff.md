# Comparing `tmp/pytest_xdist_worker_stats-0.1.4.tar.gz` & `tmp/pytest_xdist_worker_stats-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xdist_worker_stats-0.1.4.tar", max compression
+gzip compressed data, was "pytest_xdist_worker_stats-0.1.5.tar", max compression
```

## Comparing `pytest_xdist_worker_stats-0.1.4.tar` & `pytest_xdist_worker_stats-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/LICENSE
--rw-r--r--   0        0        0     2305 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/README.md
--rw-r--r--   0        0        0     2855 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       75 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/pytest_xdist_worker_stats/__init__.py
--rw-r--r--   0        0        0      937 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/pytest_xdist_worker_stats/options.py
--rw-r--r--   0        0        0     3639 2023-09-29 20:46:40.591765 pytest_xdist_worker_stats-0.1.4/pytest_xdist_worker_stats/plugin.py
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2305 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/README.md
+-rw-r--r--   0        0        0     2857 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       75 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/options.py
+-rw-r--r--   0        0        0     3639 2024-04-09 12:21:21.071665 pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/plugin.py
+-rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 pytest_xdist_worker_stats-0.1.5/PKG-INFO
```

### Comparing `pytest_xdist_worker_stats-0.1.4/LICENSE` & `pytest_xdist_worker_stats-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.4/README.md` & `pytest_xdist_worker_stats-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.4/pyproject.toml` & `pytest_xdist_worker_stats-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xdist-worker-stats"
-version = "0.1.4"
+version = "0.1.5"
 description = "A pytest plugin to list worker statistics after a xdist run."
 authors = ["Mikuláš Poul <mikulaspoul@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pytest_xdist_worker_stats"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
 keywords = ["pytest", "xdist", "pytest-xdist"]
 
 [tool.poetry.plugins."pytest11"]
 pytest-xdist-worker-stats = "pytest_xdist_worker_stats"
 
 [tool.poetry.dependencies]
 python = ">3.9"
-pytest = "^7.3"
+pytest = ">7.3.2"
 pytest-xdist = "^3.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 ruff = "^0.0.291"
 
 [build-system]
```

### Comparing `pytest_xdist_worker_stats-0.1.4/pytest_xdist_worker_stats/options.py` & `pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/options.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.4/pytest_xdist_worker_stats/plugin.py` & `pytest_xdist_worker_stats-0.1.5/pytest_xdist_worker_stats/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_xdist_worker_stats-0.1.4/PKG-INFO` & `pytest_xdist_worker_stats-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist-worker-stats
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pytest plugin to list worker statistics after a xdist run.
 Home-page: https://github.com/mikicz/pytest-xdist-worker-stats
 License: MIT
 Keywords: pytest,xdist,pytest-xdist
 Author: Mikuláš Poul
 Author-email: mikulaspoul@gmail.com
 Requires-Python: >3.9
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest (>=7.3,<8.0)
+Requires-Dist: pytest (>7.3.2)
 Requires-Dist: pytest-xdist (>=3.3,<4.0)
 Project-URL: Repository, https://github.com/mikicz/pytest-xdist-worker-stats
 Description-Content-Type: text/markdown
 
 # pytest-xdist-worker-stats
 
 A pytest plugin to list worker statistics after a xdist run.
```

