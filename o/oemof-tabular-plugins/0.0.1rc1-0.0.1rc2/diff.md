# Comparing `tmp/oemof-tabular-plugins-0.0.1rc1.tar.gz` & `tmp/oemof-tabular-plugins-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oemof-tabular-plugins-0.0.1rc1.tar", last modified: Fri Apr  5 11:22:59 2024, max compression
+gzip compressed data, was "oemof-tabular-plugins-0.0.1rc2.tar", last modified: Tue Apr  9 12:31:25 2024, max compression
```

## Comparing `oemof-tabular-plugins-0.0.1rc1.tar` & `oemof-tabular-plugins-0.0.1rc2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.945780 oemof-tabular-plugins-0.0.1rc1/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1080 2024-02-06 15:46:18.000000 oemof-tabular-plugins-0.0.1rc1/LICENSE.txt
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)     4049 2024-04-05 11:22:59.945780 oemof-tabular-plugins-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3387 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/README.rst
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      999 2024-02-28 09:24:58.000000 oemof-tabular-plugins-0.0.1rc1/pyproject.toml
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/requirements/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      192 2024-02-28 09:41:26.000000 oemof-tabular-plugins-0.0.1rc1/requirements/build_requirements.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-05 11:22:59.945780 oemof-tabular-plugins-0.0.1rc1/setup.cfg
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      239 2024-02-27 14:26:41.000000 oemof-tabular-plugins-0.0.1rc1/setup.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/src/
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      271 2024-02-27 14:40:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       48 2024-04-05 11:22:33.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/_version.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:35:06.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1000 2024-02-27 15:06:09.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/constraint_facades.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1051 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25058 2024-03-28 13:07:08.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/post_processing.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9235 2024-03-28 14:28:43.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/pre_processing.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/hydrogen/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/hydrogen/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       24 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/hydrogen/constraint_facades.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/hydrogen/constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       47 2024-03-08 08:27:12.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/hydrogen/post_processing.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.941780 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/wefe/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/wefe/__init__.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       24 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/wefe/constraint_facades.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/wefe/constraints.py
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       85 2024-03-08 08:27:12.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/wefe/post_processing.py
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.945780 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/
--rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)     4049 2024-04-05 11:22:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/PKG-INFO
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1091 2024-04-05 11:22:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-05 11:22:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-04-05 11:22:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/entry_points.txt
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2024-04-05 11:22:59.000000 oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/top_level.txt
-drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-05 11:22:59.945780 oemof-tabular-plugins-0.0.1rc1/tests/
--rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      903 2024-03-28 14:28:14.000000 oemof-tabular-plugins-0.0.1rc1/tests/test_pre_processing.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1080 2024-02-06 15:46:18.000000 oemof-tabular-plugins-0.0.1rc2/LICENSE.txt
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)     4078 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     3387 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/README.rst
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      999 2024-02-28 09:24:58.000000 oemof-tabular-plugins-0.0.1rc2/pyproject.toml
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.717639 oemof-tabular-plugins-0.0.1rc2/requirements/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      133 2024-04-09 12:29:44.000000 oemof-tabular-plugins-0.0.1rc2/requirements/build_requirements.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       38 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      239 2024-02-27 14:26:41.000000 oemof-tabular-plugins-0.0.1rc2/setup.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.717639 oemof-tabular-plugins-0.0.1rc2/src/
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.717639 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      271 2024-02-27 14:40:59.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       48 2024-04-09 12:31:00.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/_version.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.717639 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:35:06.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1000 2024-02-27 15:06:09.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/constraint_facades.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1051 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)    25058 2024-03-28 13:07:08.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/post_processing.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     9235 2024-03-28 14:28:43.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/pre_processing.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/hydrogen/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/hydrogen/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       24 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/hydrogen/constraint_facades.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/hydrogen/constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       47 2024-03-08 08:27:12.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/hydrogen/post_processing.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/wefe/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/wefe/__init__.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       24 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/wefe/constraint_facades.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-02-27 14:32:54.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/wefe/constraints.py
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       85 2024-03-08 08:27:12.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/wefe/post_processing.py
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/
+-rw-r--r--   0 pierre-francois  (1000) pierre-francois  (1000)     4078 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)     1139 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)        1 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       54 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/entry_points.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       14 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/requires.txt
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)       22 2024-04-09 12:31:25.000000 oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/top_level.txt
+drwxrwxr-x   0 pierre-francois  (1000) pierre-francois  (1000)        0 2024-04-09 12:31:25.721639 oemof-tabular-plugins-0.0.1rc2/tests/
+-rw-rw-r--   0 pierre-francois  (1000) pierre-francois  (1000)      903 2024-03-28 14:28:14.000000 oemof-tabular-plugins-0.0.1rc2/tests/test_pre_processing.py
```

### Comparing `oemof-tabular-plugins-0.0.1rc1/LICENSE.txt` & `oemof-tabular-plugins-0.0.1rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/PKG-INFO` & `oemof-tabular-plugins-0.0.1rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: oemof-tabular-plugins
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A package that contains various constraint facades to be used with oemof-tabular
 Author-email: Ciara Dunks <ciara.dunks@rl-institut.de>, Pierre-François Duc <pierre-francois.duc@rl-institut.de>
 Project-URL: Homepage, https://github.com/rl-institut/oemof-tabular-plugins
 Project-URL: Issues, https://github.com/rl-institut/oemof-tabular-plugins/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: oemof-tabular
 
 
 .. figure:: https://user-images.githubusercontent.com/14353512/185425447-85dbcde9-f3a2-4f06-a2db-0dee43af2f5f.png
     :align: left
     :target: https://github.com/rl-institut/super-repo/
     :alt: Repo logo
```

### Comparing `oemof-tabular-plugins-0.0.1rc1/README.rst` & `oemof-tabular-plugins-0.0.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/pyproject.toml` & `oemof-tabular-plugins-0.0.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/constraint_facades.py` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/constraint_facades.py`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/constraints.py` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/constraints.py`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/post_processing.py` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/post_processing.py`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins/general/pre_processing.py` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins/general/pre_processing.py`

 * *Files identical despite different names*

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/PKG-INFO` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: oemof-tabular-plugins
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A package that contains various constraint facades to be used with oemof-tabular
 Author-email: Ciara Dunks <ciara.dunks@rl-institut.de>, Pierre-François Duc <pierre-francois.duc@rl-institut.de>
 Project-URL: Homepage, https://github.com/rl-institut/oemof-tabular-plugins
 Project-URL: Issues, https://github.com/rl-institut/oemof-tabular-plugins/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: oemof-tabular
 
 
 .. figure:: https://user-images.githubusercontent.com/14353512/185425447-85dbcde9-f3a2-4f06-a2db-0dee43af2f5f.png
     :align: left
     :target: https://github.com/rl-institut/super-repo/
     :alt: Repo logo
```

### Comparing `oemof-tabular-plugins-0.0.1rc1/src/oemof_tabular_plugins.egg-info/SOURCES.txt` & `oemof-tabular-plugins-0.0.1rc2/src/oemof_tabular_plugins.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements/build_requirements.txt
 src/oemof_tabular_plugins/__init__.py
 src/oemof_tabular_plugins/_version.py
 src/oemof_tabular_plugins.egg-info/PKG-INFO
 src/oemof_tabular_plugins.egg-info/SOURCES.txt
 src/oemof_tabular_plugins.egg-info/dependency_links.txt
 src/oemof_tabular_plugins.egg-info/entry_points.txt
+src/oemof_tabular_plugins.egg-info/requires.txt
 src/oemof_tabular_plugins.egg-info/top_level.txt
 src/oemof_tabular_plugins/general/__init__.py
 src/oemof_tabular_plugins/general/constraint_facades.py
 src/oemof_tabular_plugins/general/constraints.py
 src/oemof_tabular_plugins/general/post_processing.py
 src/oemof_tabular_plugins/general/pre_processing.py
 src/oemof_tabular_plugins/hydrogen/__init__.py
```

### Comparing `oemof-tabular-plugins-0.0.1rc1/tests/test_pre_processing.py` & `oemof-tabular-plugins-0.0.1rc2/tests/test_pre_processing.py`

 * *Files identical despite different names*

