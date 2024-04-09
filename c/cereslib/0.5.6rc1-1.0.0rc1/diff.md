# Comparing `tmp/cereslib-0.5.6rc1.tar.gz` & `tmp/cereslib-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereslib-0.5.6rc1.tar", max compression
+gzip compressed data, was "cereslib-1.0.0rc1.tar", max compression
```

## Comparing `cereslib-0.5.6rc1.tar` & `cereslib-1.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      166 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/AUTHORS
--rw-r--r--   0        0        0     7651 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/LICENSE
--rw-r--r--   0        0        0     2631 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/NEWS
--rw-r--r--   0        0        0     4872 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/README.md
--rw-r--r--   0        0        0      759 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/__init__.py
--rw-r--r--   0        0        0       91 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/_version.py
--rw-r--r--   0        0        0        0 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/dfutils/__init__.py
--rw-r--r--   0        0        0     2586 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/dfutils/filter.py
--rw-r--r--   0        0        0     3595 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/dfutils/format.py
--rw-r--r--   0        0        0        0 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/enrich/__init__.py
--rw-r--r--   0        0        0    31928 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/enrich/enrich.py
--rw-r--r--   0        0        0        0 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/events/__init__.py
--rw-r--r--   0        0        0    35285 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/cereslib/events/events.py
--rw-r--r--   0        0        0     1357 2024-03-27 10:58:58.272218 cereslib-0.5.6rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/__init__.py
--rw-r--r--   0        0        0      379 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/enrich/authors.csv
--rw-r--r--   0        0        0      106 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/enrich/onion.csv
--rw-r--r--   0        0        0      111 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/enrich/pairprogramming.csv
--rw-r--r--   0        0        0      292 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/enrich/timedifference.csv
--rw-r--r--   0        0        0      610 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/enrich/uuids.csv
--rw-r--r--   0        0        0     9538 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/events/git.json
--rw-r--r--   0        0        0       97 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/data/projects_map.json
--rw-r--r--   0        0        0     3982 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/manual_test_events.py
--rwxr-xr-x   0        0        0     1075 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/run_tests.py
--rw-r--r--   0        0        0    11014 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/test_enrich.py
--rw-r--r--   0        0        0     2433 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/test_filter.py
--rw-r--r--   0        0        0     1894 2024-03-27 10:58:58.276218 cereslib-0.5.6rc1/tests/test_format.py
--rw-r--r--   0        0        0     6056 1970-01-01 00:00:00.000000 cereslib-0.5.6rc1/PKG-INFO
+-rw-r--r--   0        0        0      166 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0     7651 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2711 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0     4872 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      759 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/_version.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/dfutils/__init__.py
+-rw-r--r--   0        0        0     2586 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/dfutils/filter.py
+-rw-r--r--   0        0        0     3595 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/dfutils/format.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/enrich/__init__.py
+-rw-r--r--   0        0        0    31928 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/enrich/enrich.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/events/__init__.py
+-rw-r--r--   0        0        0    35285 2024-04-09 16:09:45.965047 cereslib-1.0.0rc1/cereslib/events/events.py
+-rw-r--r--   0        0        0     1370 2024-04-09 16:09:45.969047 cereslib-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0      379 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/enrich/authors.csv
+-rw-r--r--   0        0        0      106 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/enrich/onion.csv
+-rw-r--r--   0        0        0      111 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/enrich/pairprogramming.csv
+-rw-r--r--   0        0        0      292 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/enrich/timedifference.csv
+-rw-r--r--   0        0        0      610 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/enrich/uuids.csv
+-rw-r--r--   0        0        0     9538 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/events/git.json
+-rw-r--r--   0        0        0       97 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/data/projects_map.json
+-rw-r--r--   0        0        0     3982 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/manual_test_events.py
+-rwxr-xr-x   0        0        0     1075 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    11014 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/test_enrich.py
+-rw-r--r--   0        0        0     2433 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/test_filter.py
+-rw-r--r--   0        0        0     1894 2024-04-09 16:09:45.973047 cereslib-1.0.0rc1/tests/test_format.py
+-rw-r--r--   0        0        0     6069 1970-01-01 00:00:00.000000 cereslib-1.0.0rc1/PKG-INFO
```

### Comparing `cereslib-0.5.6rc1/LICENSE` & `cereslib-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/NEWS` & `cereslib-1.0.0rc1/NEWS`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## cereslib 0.5.6 - (2024-03-27)
+  
+  * Update Poetry's package dependencies
+
   ## cereslib 0.5.5 - (2024-03-12)
   
   * Update Poetry's package dependencies
 
   ## cereslib 0.5.4 - (2024-03-01)
   
   * Update Poetry's package dependencies
```

### Comparing `cereslib-0.5.6rc1/README.md` & `cereslib-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/cereslib/__init__.py` & `cereslib-1.0.0rc1/cereslib/__init__.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/cereslib/dfutils/filter.py` & `cereslib-1.0.0rc1/cereslib/dfutils/filter.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/cereslib/dfutils/format.py` & `cereslib-1.0.0rc1/cereslib/dfutils/format.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/cereslib/enrich/enrich.py` & `cereslib-1.0.0rc1/cereslib/enrich/enrich.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/cereslib/events/events.py` & `cereslib-1.0.0rc1/cereslib/events/events.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/pyproject.toml` & `cereslib-1.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cereslib"
-version = "0.5.6-rc.1"
+version = "1.0.0-rc.1"
 description = "GrimoireLab: Unify, eventize and enrich information from Perceval"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -25,15 +25,15 @@
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
```

### Comparing `cereslib-0.5.6rc1/tests/data/enrich/uuids.csv` & `cereslib-1.0.0rc1/tests/data/enrich/uuids.csv`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/data/events/git.json` & `cereslib-1.0.0rc1/tests/data/events/git.json`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/manual_test_events.py` & `cereslib-1.0.0rc1/tests/manual_test_events.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/run_tests.py` & `cereslib-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/test_enrich.py` & `cereslib-1.0.0rc1/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/test_filter.py` & `cereslib-1.0.0rc1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/tests/test_format.py` & `cereslib-1.0.0rc1/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `cereslib-0.5.6rc1/PKG-INFO` & `cereslib-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: cereslib
-Version: 0.5.6rc1
+Version: 1.0.0rc1
 Summary: GrimoireLab: Unify, eventize and enrich information from Perceval
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
