# Comparing `tmp/flake8_builtins-2.4.0.tar.gz` & `tmp/flake8_builtins-2.5.0.tar.gz`

## Comparing `flake8_builtins-2.4.0.tar` & `flake8_builtins-2.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.flake8
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/CHANGES.rst
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/MANIFEST.in
--rw-r--r--   0        0        0    10967 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/flake8_builtins.py
--rw-r--r--   0        0        0    11332 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/run_tests.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/tox.ini
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/.gitignore
--rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/LICENSE
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/README.rst
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 flake8_builtins-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/.flake8
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/CHANGES.rst
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/MANIFEST.in
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/flake8_builtins.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/run_tests.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/tox.ini
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/.gitignore
+-rw-r--r--   0        0        0    18092 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/README.rst
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 flake8_builtins-2.5.0/PKG-INFO
```

### Comparing `flake8_builtins-2.4.0/.pre-commit-config.yaml` & `flake8_builtins-2.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.4.0/CHANGES.rst` & `flake8_builtins-2.5.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 .. -*- coding: utf-8 -*-
 
 Changelog
 =========
 
+2.5.0 (2024-04-09)
+------------------
+
+- Support detecting a shadowing folder as module name (as part of `A005`).
+  [asfaltboy]
+
+
 2.4.0 (2024-04-01)
 ------------------
 
 - Add rule for lambda argument shadowing (`A006`).
   [cielavenir]
```

### Comparing `flake8_builtins-2.4.0/flake8_builtins.py` & `flake8_builtins-2.5.0/flake8_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,17 @@
             type(self),
         )
 
     def check_module_name(self, filename: str):
         if not self.module_names:
             return
         path = Path(filename)
-        module_name = path.name.removesuffix('.py')
+        if path.name == '__init__.py':
+            module_name = path.parent.name
+        else:
+            module_name = path.name.removesuffix('.py')
         if module_name in self.module_names:
             yield self.error(
                 None,
                 module_name,
                 message=self.module_name_msg,
             )
```

### Comparing `flake8_builtins-2.4.0/run_tests.py` & `flake8_builtins-2.5.0/run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,14 +506,15 @@
 @pytest.mark.skipif(
     sys.version_info < (3, 10),
     reason='Skip A005, module testing is only supported in Python 3.10 and above',
 )
 def test_module_name():
     source = ''
     check_code(source, expected_codes='A005', filename='./temp/logging.py')
+    check_code(source, expected_codes='A005', filename='./temp/typing/__init__.py')
 
 
 @pytest.mark.skipif(
     sys.version_info < (3, 10),
     reason='Skip A005, module testing is only supported in Python 3.10 and above',
 )
 def test_module_name_ignore_module():
```

### Comparing `flake8_builtins-2.4.0/tox.ini` & `flake8_builtins-2.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.4.0/.github/workflows/testing.yml` & `flake8_builtins-2.5.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.4.0/LICENSE` & `flake8_builtins-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.4.0/README.rst` & `flake8_builtins-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `flake8_builtins-2.4.0/pyproject.toml` & `flake8_builtins-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flake8-builtins"
-version = "2.4.0"
+version = "2.5.0"
 authors = [
   { name="Gil Forcada Codinachs", email="gil.gnome@gmail.com" },
 ]
 description = "Check for python builtins being used as variables or parameters"
 keywords = ["pep8", "flake8", "python", ]
 readme = "README.rst"
 requires-python = ">=3.8"
```

### Comparing `flake8_builtins-2.4.0/PKG-INFO` & `flake8_builtins-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-builtins
-Version: 2.4.0
+Version: 2.5.0
 Summary: Check for python builtins being used as variables or parameters
 Project-URL: Homepage, https://github.com/gforcada/flake8-builtins
 Project-URL: Bug Tracker, https://github.com/gforcada/flake8-builtins/issues
 Project-URL: Changelog, https://github.com/gforcada/flake8-builtins/blob/main/CHANGES.rst
 Author-email: Gil Forcada Codinachs <gil.gnome@gmail.com>
 License-File: LICENSE
 Keywords: flake8,pep8,python
```

