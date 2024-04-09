# Comparing `tmp/edwh_uptime_plugin-0.3.4.tar.gz` & `tmp/edwh_uptime_plugin-0.3.5.tar.gz`

## Comparing `edwh_uptime_plugin-0.3.4.tar` & `edwh_uptime_plugin-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/__about__.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/__init__.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/dumpers.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/helpers.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/tasks.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/uptimerobot.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/tests/test_api.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/README.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/__about__.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/__init__.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/dumpers.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/helpers.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/tasks.py
+-rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/uptimerobot.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/tests/test_api.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/LICENSE.txt
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/PKG-INFO
```

### Comparing `edwh_uptime_plugin-0.3.4/CHANGELOG.md` & `edwh_uptime_plugin-0.3.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.5 (2024-04-09)
+
+### Fix
+
+* **deps:** Include two missing dependencies ([`09fb42e`](https://github.com/educationwarehouse/edwh-uptime-plugin/commit/09fb42e88c5c79dc02fc8cf80e31173a1d03b14f))
+
 ## v0.3.4 (2024-03-15)
 ### Fix
 * Delayed init of UptimeRobot instance, since this depends on TomlConfig which is not always available ([`c73daee`](https://github.com/educationwarehouse/edwh-uptime-plugin/commit/c73daeed3ffec5766247795c1b97e44b84773e9b))
 
 ## v0.3.3 (2024-02-09)
```

### Comparing `edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/dumpers.py` & `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/dumpers.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/tasks.py` & `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/src/edwh_uptime_plugin/uptimerobot.py` & `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/uptimerobot.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/tests/test_api.py` & `edwh_uptime_plugin-0.3.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/LICENSE.txt` & `edwh_uptime_plugin-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/README.md` & `edwh_uptime_plugin-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.4/pyproject.toml` & `edwh_uptime_plugin-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     'edwh>=0.38.0',
     'yayarl',
     'termcolor',
+    'tomli-w',
+    'typing-extensions',
 ]
 
 [project.optional-dependencies]
 dev = [
     "hatch",
     # "python-semantic-release",
     "black",
```

### Comparing `edwh_uptime_plugin-0.3.4/PKG-INFO` & `edwh_uptime_plugin-0.3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: edwh-uptime-plugin
-Version: 0.3.4
+Version: 0.3.5
 Summary: UptimeRobot plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-uptime-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-uptime-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-uptime-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: edwh>=0.38.0
 Requires-Dist: termcolor
+Requires-Dist: tomli-w
+Requires-Dist: typing-extensions
 Requires-Dist: yayarl
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
```

