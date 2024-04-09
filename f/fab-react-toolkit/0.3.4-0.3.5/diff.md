# Comparing `tmp/fab-react-toolkit-0.3.4.tar.gz` & `tmp/fab-react-toolkit-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.3.4.tar", last modified: Fri Apr  5 13:09:48 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.3.5.tar", last modified: Tue Apr  9 12:58:52 2024, max compression
```

## Comparing `fab-react-toolkit-0.3.4.tar` & `fab-react-toolkit-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.852508 fab-react-toolkit-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-05 13:09:48.852508 fab-react-toolkit-0.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.848508 fab-react-toolkit-0.3.4/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.848508 fab-react-toolkit-0.3.4/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.848508 fab-react-toolkit-0.3.4/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.852508 fab-react-toolkit-0.3.4/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:09:48.852508 fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-05 13:09:48.000000 fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 13:09:48.000000 fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:09:48.000000 fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 13:09:48.000000 fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 13:09:40.000000 fab-react-toolkit-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-05 13:09:48.852508 fab-react-toolkit-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 12:58:52.000000 fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-09 12:58:52.000000 fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:58:52.000000 fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 12:58:52.000000 fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 12:58:43.000000 fab-react-toolkit-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 12:58:52.241665 fab-react-toolkit-0.3.5/setup.cfg
```

### Comparing `fab-react-toolkit-0.3.4/LICENSE` & `fab-react-toolkit-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/PKG-INFO` & `fab-react-toolkit-0.3.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.3.4/example/app/__init__.py` & `fab-react-toolkit-0.3.5/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/example/app/apis.py` & `fab-react-toolkit-0.3.5/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/example/app/config.py` & `fab-react-toolkit-0.3.5/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/example/app/models.py` & `fab-react-toolkit-0.3.5/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/example/run.py` & `fab-react-toolkit-0.3.5/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit/views.py` & `fab-react-toolkit-0.3.5/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.4
+Version: 0.3.5
 Summary: A small example package
 Home-page: https://github.com/dttctcs/fab-react-toolkit
 Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fab-react-toolkit-0.3.4/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.3.5/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.4/pyproject.toml` & `fab-react-toolkit-0.3.5/pyproject.toml`

 * *Files identical despite different names*

