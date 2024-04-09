# Comparing `tmp/pyramid_formencode_classic-0.5.1.tar.gz` & `tmp/pyramid_formencode_classic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyramid_formencode_classic-0.5.1.tar", last modified: Wed Jul 26 19:32:17 2023, max compression
+gzip compressed data, was "pyramid_formencode_classic-0.6.0.tar", last modified: Tue Apr  9 20:24:51 2024, max compression
```

## Comparing `pyramid_formencode_classic-0.5.1.tar` & `pyramid_formencode_classic-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.299528 pyramid_formencode_classic-0.5.1/
--rw-r--r--   0 jvanasco   (501) admin       (80)     8177 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.5.1/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)    21773 2023-07-26 19:32:17.299937 pyramid_formencode_classic-0.5.1/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)    20888 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       82 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      583 2023-07-26 19:32:17.301509 pyramid_formencode_classic-0.5.1/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     2032 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.240047 pyramid_formencode_classic-0.5.1/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.263735 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/
--rw-r--r--   0 jvanasco   (501) admin       (80)     2071 2023-07-26 19:32:05.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      144 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/_defaults.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      208 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/_utils.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    14242 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/api.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.275559 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      422 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.277864 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1371 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.279227 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
--rw-r--r--   0 jvanasco   (501) admin       (80)     2057 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/exceptions.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1691 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/formatters.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    16571 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/objects.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/py.typed
--rw-r--r--   0 jvanasco   (501) admin       (80)     1542 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.272593 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)    21773 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     1351 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)       68 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       27 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.282225 pyramid_formencode_classic-0.5.1/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.5.1/tests/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.297868 pyramid_formencode_classic-0.5.1/tests/fixtures/
--rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-alt.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-default.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-explicit.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-none.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_b-multi.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)   119760 2023-06-16 19:20:00.000000 pyramid_formencode_classic-0.5.1/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.668855 pyramid_formencode_classic-0.6.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     8752 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.6.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)    22703 2024-04-09 20:24:51.669320 pyramid_formencode_classic-0.6.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)    21747 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       82 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      593 2024-04-09 20:24:51.670899 pyramid_formencode_classic-0.6.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2082 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.620450 pyramid_formencode_classic-0.6.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.647603 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2399 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      144 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/_defaults.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      208 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/_utils.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    15073 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/api.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.655045 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      422 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.657094 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/
+-rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1371 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.658181 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2057 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/exceptions.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1691 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/formatters.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16571 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/objects.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1542 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.654115 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    22703 2024-04-09 20:24:51.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1351 2024-04-09 20:24:51.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2024-04-09 20:24:51.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       68 2024-04-09 20:24:51.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       27 2024-04-09 20:24:51.000000 pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.660205 pyramid_formencode_classic-0.6.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.6.0/tests/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2024-04-09 20:24:51.667594 pyramid_formencode_classic-0.6.0/tests/fixtures/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.6.0/tests/fixtures/form_a-html_error_placeholder-alt.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.6.0/tests/fixtures/form_a-html_error_placeholder-default.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.6.0/tests/fixtures/form_a-html_error_placeholder-explicit.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.6.0/tests/fixtures/form_a-html_error_placeholder-none.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.6.0/tests/fixtures/form_b-multi.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)   120106 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      155 2024-04-09 20:24:30.000000 pyramid_formencode_classic-0.6.0/tox.ini
```

### Comparing `pyramid_formencode_classic-0.5.1/CHANGES.txt` & `pyramid_formencode_classic-0.6.0/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+0.6.0
+    BACKWARDS INCOMPATIBLE CHANGE
+    * `form_validate` now requires `return_stash=True` - which is enabled by default.
+      To support `return_stash=False`, please call `form_validate_simple` instead.
+      This change was required to streamline typing and better standardize the library.
+      Background:
+        `form_validate` was renamed to `_form_validate_core`
+        the new `form_validate` ensures `return_stash==True` and invokes `_form_validate_core`
+        the new `form_validate_simple` ensures `return_stash==False` and invokes `_form_validate_core`
+
 0.5.0
     * drop py2
     * mypy support
     * reorganized a lot of code/functions into new files.
       the relevant imports should be unchanged.
 
 0.4.5
```

### Comparing `pyramid_formencode_classic-0.5.1/PKG-INFO` & `pyramid_formencode_classic-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: pyramid_formencode_classic
-Version: 0.5.1
+Version: 0.6.0
 Summary: ('An implementation of the classic Pylons formencode validation, for Pyramid',)
 Home-page: https://github.com/jvanasco/pyramid_formencode_classic
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
 
 ## Current Recommended Version
 
+`v 0.6.0 (2024.04.09)`
+
+This is backwards compatible due to the following change:
+
+    * `form_validate` now requires `return_stash=True` - which is enabled by default.
+      To support `return_stash=False`, please call `form_validate_simple` instead.
+      This change was required to streamline typing and better standardize the library.
+      Background:
+        `form_validate` was renamed to `_form_validate_core`
+        the new `form_validate` ensures `return_stash==True` and invokes `_form_validate_core`
+        the new `form_validate_simple` ensures `return_stash==False` and invokes `_form_validate_core`
+
+## Current EOL version
+
 `v 0.5.0 (2023.06.xx)`
 
 New Features:
 * mypy support
 * drop python2
 * project reorganized
 
@@ -43,14 +59,21 @@
 * python3 support
 * pyramid debugtoolbar support
 * automatic handling of edge cases with ForEach validator errors
 
 
 ### Backwards Compatible?
 
+### 0.6.0
+
+A backwards incompatible change was introduced.
+
+form_validate` now requires `return_stash=True` - which is enabled by default.
+To support `return_stash=False`, please call `form_validate_simple` instead.
+
 ### 0.5.0
 
 The library was reorganized to implement typing.
 Most uses should be backwards compatible.
 It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
 The default values were moved to a separate file. Those should never have been referenced in code.
 
@@ -590,7 +613,9 @@
 ### v0.3.x to v0.4.x
 
 * `FormStash.set_error()` the `raise_FieldInvalid` kwarg was removed. instead, use `FormStash.fatal_field()`
 * `FormStash.set_error()` the `raise_FormInvalid` kwarg was removed. instead, use `FormStash.fatal_form()`
 * import formatters from `pyramid_formencode_classic.formatters` not the main namespace
 
 
+
+
```

### Comparing `pyramid_formencode_classic-0.5.1/README.md` & `pyramid_formencode_classic-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
 
 ## Current Recommended Version
 
+`v 0.6.0 (2024.04.09)`
+
+This is backwards compatible due to the following change:
+
+    * `form_validate` now requires `return_stash=True` - which is enabled by default.
+      To support `return_stash=False`, please call `form_validate_simple` instead.
+      This change was required to streamline typing and better standardize the library.
+      Background:
+        `form_validate` was renamed to `_form_validate_core`
+        the new `form_validate` ensures `return_stash==True` and invokes `_form_validate_core`
+        the new `form_validate_simple` ensures `return_stash==False` and invokes `_form_validate_core`
+
+## Current EOL version
+
 `v 0.5.0 (2023.06.xx)`
 
 New Features:
 * mypy support
 * drop python2
 * project reorganized
 
@@ -21,14 +35,21 @@
 * python3 support
 * pyramid debugtoolbar support
 * automatic handling of edge cases with ForEach validator errors
 
 
 ### Backwards Compatible?
 
+### 0.6.0
+
+A backwards incompatible change was introduced.
+
+form_validate` now requires `return_stash=True` - which is enabled by default.
+To support `return_stash=False`, please call `form_validate_simple` instead.
+
 ### 0.5.0
 
 The library was reorganized to implement typing.
 Most uses should be backwards compatible.
 It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
 The default values were moved to a separate file. Those should never have been referenced in code.
```

### Comparing `pyramid_formencode_classic-0.5.1/setup.cfg` & `pyramid_formencode_classic-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 	src/pyramid_formencode_classic/__init__.py: E501
 	src/pyramid_formencode_classic/api.py: E501
 	src/pyramid_formencode_classic/exceptions.py: E501
 	src/pyramid_formencode_classic/formatters.py: E501
 	src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py: E501
 	src/pyramid_formencode_classic/objects.py: E501
 	src/pyramid_formencode_classic/utils.py: E501
-	tests/core.py:W293,E722
+	tests/test_core.py:W293,E501,E722
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyramid_formencode_classic-0.5.1/setup.py` & `pyramid_formencode_classic-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: BSD License",
     ],
 )
```

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/__init__.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 # pypi
 import webob.compat
 
 # local
 from .api import form_reprint  # noqa: F401 ; maintain API
 from .api import form_validate  # noqa: F401 ; maintain API
+from .exceptions import BaseException  # noqa: F401 ; maintain API
+from .exceptions import CsrfInvalid  # noqa: F401 ; maintain API
+from .exceptions import FormFieldInvalid  # noqa: F401 ; maintain API
 from .exceptions import FormInvalid  # noqa: F401 ; maintain API
-from .objects import FormStash
-from .objects import FormStashList
+from .exceptions import ValidationStop  # noqa: F401 ; maintain API
+from .objects import FormStash  # noqa: F401 ; maintain API
+from .objects import FormStashList  # noqa: F401 ; maintain API
 
 if TYPE_CHECKING:
     from pyramid.config import Configurator
     from pyramid.request import Request
 
 # ==============================================================================
 
@@ -29,15 +33,15 @@
 
 def warn_user(message):
     warnings.warn(message, UserWarning, stacklevel=2)
 """
 
 
 # defaults
-__VERSION__ = "0.5.1"
+__VERSION__ = "0.6.0"
 
 AUTOMATIC_CLEANUP = True
 
 log = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/api.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # pypi
 import formencode
 import formencode.htmlfill
 from pyramid.interfaces import IResponse
 from pyramid.renderers import render as pyramid_render
 from pyramid.response import Response as PyramidResponse
+from webob.multidict import MultiDict
 
 # local
 from ._defaults import DEFAULT_ERROR_MAIN_KEY
 from ._defaults import DEFAULT_ERROR_MAIN_TEXT
 from ._defaults import DEFAULT_FORM_STASH
 from .exceptions import FormFieldInvalid
 from .exceptions import FormInvalid
@@ -27,31 +28,30 @@
 from .utils import determine_response_charset
 from .utils import encode_formencode_errors
 
 if TYPE_CHECKING:
     from formencode import Schema
     from pyramid.request import Request
     from pyramid.response import Response
-    from webob.multidict import MultiDict
 
 # ==============================================================================
 
 log = logging.getLogger(__name__)
 
 # ------------------------------------------------------------------------------
 
 
-def form_validate(
+def _form_validate_core(
     request: "Request",
     schema: Optional["Schema"] = None,
     form_stash: str = DEFAULT_FORM_STASH,
     form_stash_object: Optional[FormStash] = None,
     validate_post: bool = True,
     validate_get: bool = False,
-    validate_params: Optional["MultiDict"] = None,
+    validate_params: Optional[MultiDict] = None,
     variable_decode: bool = False,
     dict_char: str = ".",
     list_char: str = "-",
     state: Optional[Any] = None,  # passthrough to formencode
     error_main_text: str = DEFAULT_ERROR_MAIN_TEXT,
     error_main_key: str = DEFAULT_ERROR_MAIN_KEY,
     error_string_key: str = "Error_String",
@@ -173,25 +173,26 @@
             elif not validate_post and validate_get:
                 validate_params = request.GET
             elif not validate_post and not validate_get:
                 formStash.set_error(
                     field=formStash.error_main_key, message="Nothing submitted."
                 )
                 raise ValidationStop("no `validate_params`")
-
-        validate_params = validate_params.mixed()
+        if TYPE_CHECKING:
+            assert isinstance(validate_params, MultiDict)
+        _validate_params: Dict = validate_params.mixed()
 
         if variable_decode:
             if __debug__:
                 log.debug("form_validate - running variable_decode on params")
             decoded_params = formencode.variabledecode.variable_decode(
-                validate_params, dict_char, list_char
+                _validate_params, dict_char, list_char
             )
         else:
-            decoded_params = validate_params
+            decoded_params = _validate_params
 
         # if there are no params to validate against, then just stop
         if not decoded_params:
             formStash.is_submitted_vars = False
             formStash.set_error(
                 field=formStash.error_main_key, message="Nothing submitted."
             )
@@ -262,14 +263,34 @@
             raise FormFieldInvalid()
 
     if return_stash:
         return (not formStash.is_error, formStash)
     return not formStash.is_error
 
 
+def form_validate(request: "Request", **kwargs) -> Tuple[bool, FormStash]:
+    if "return_stash" in kwargs:
+        if kwargs["return_stash"] is not True:
+            raise ValueError("`form_validate` REQUIRES `return_stash=True`")
+    result = _form_validate_core(request, **kwargs)
+    if TYPE_CHECKING:
+        assert isinstance(result, tuple)
+    return result
+
+
+def form_validate_simple(request: "Request", **kwargs) -> bool:
+    if "return_stash" in kwargs:
+        if kwargs["return_stash"] not in (False, None):
+            raise ValueError("`form_validate_simple` REQUIRES `return_stash=False`")
+    result = _form_validate_core(request, **kwargs)
+    if TYPE_CHECKING:
+        assert isinstance(result, bool)
+    return result
+
+
 def form_reprint(
     request: "Request",
     form_print_method: Optional[Callable],
     form_stash=DEFAULT_FORM_STASH,
     render_view: Optional[Callable] = None,
     render_view_template: Optional[str] = None,
     auto_error_formatter: Callable = formatter_nobr,
```

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/exceptions.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/formatters.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/formatters.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/objects.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/objects.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/utils.py` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic/utils.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/PKG-INFO` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 Metadata-Version: 2.1
 Name: pyramid-formencode-classic
-Version: 0.5.1
+Version: 0.6.0
 Summary: ('An implementation of the classic Pylons formencode validation, for Pyramid',)
 Home-page: https://github.com/jvanasco/pyramid_formencode_classic
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: BSD
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 
 ![Python package](https://github.com/jvanasco/pyramid_formencode_classic/workflows/Python%20package/badge.svg)
 
 ## Current Recommended Version
 
+`v 0.6.0 (2024.04.09)`
+
+This is backwards compatible due to the following change:
+
+    * `form_validate` now requires `return_stash=True` - which is enabled by default.
+      To support `return_stash=False`, please call `form_validate_simple` instead.
+      This change was required to streamline typing and better standardize the library.
+      Background:
+        `form_validate` was renamed to `_form_validate_core`
+        the new `form_validate` ensures `return_stash==True` and invokes `_form_validate_core`
+        the new `form_validate_simple` ensures `return_stash==False` and invokes `_form_validate_core`
+
+## Current EOL version
+
 `v 0.5.0 (2023.06.xx)`
 
 New Features:
 * mypy support
 * drop python2
 * project reorganized
 
@@ -43,14 +59,21 @@
 * python3 support
 * pyramid debugtoolbar support
 * automatic handling of edge cases with ForEach validator errors
 
 
 ### Backwards Compatible?
 
+### 0.6.0
+
+A backwards incompatible change was introduced.
+
+form_validate` now requires `return_stash=True` - which is enabled by default.
+To support `return_stash=False`, please call `form_validate_simple` instead.
+
 ### 0.5.0
 
 The library was reorganized to implement typing.
 Most uses should be backwards compatible.
 It is possible an object you used moved. If so, please file a ticket to see if we can pull it back in.
 The default values were moved to a separate file. Those should never have been referenced in code.
 
@@ -590,7 +613,9 @@
 ### v0.3.x to v0.4.x
 
 * `FormStash.set_error()` the `raise_FieldInvalid` kwarg was removed. instead, use `FormStash.fatal_field()`
 * `FormStash.set_error()` the `raise_FormInvalid` kwarg was removed. instead, use `FormStash.fatal_form()`
 * import formatters from `pyramid_formencode_classic.formatters` not the main namespace
 
 
+
+
```

### Comparing `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/SOURCES.txt` & `pyramid_formencode_classic-0.6.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/tests/fixtures/form_b-multi.mako` & `pyramid_formencode_classic-0.6.0/tests/fixtures/form_b-multi.mako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.1/tests/test_core.py` & `pyramid_formencode_classic-0.6.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from __future__ import print_function
-
 """
 IMPORTANT
 
 whitespace in the this file IS SIGNIFICANT AND IMPORTANT.
 the test-cases check for specific whitespace
 """
 
-import pyramid_formencode_classic
-from pyramid_formencode_classic import formatters
-
 # stdblib
+from typing import Dict
+from typing import Optional
 import unittest
-import pytest
 
 # pypi
 import formencode
 from pyramid import testing
-from pyramid.renderers import render_to_response
 from pyramid.interfaces import IRequestExtensions
+from pyramid.renderers import render_to_response
+from pyramid.request import Request
 from webob.multidict import MultiDict
 
-DEBUG_PRINT = True
+# local
+import pyramid_formencode_classic
+from pyramid_formencode_classic import formatters
 
 # ==============================================================================
 
+DEBUG_PRINT = True
+
 
 class _Schema_Base(formencode.Schema):
     allow_extra_fields = True
     filter_extra_fields = True
 
 
 class Form_Email(_Schema_Base):
@@ -44,14 +45,17 @@
 
 
 class DummyRequest(testing.DummyRequest):
     """
     extend `testing.DummyRequest` with a closer represtantion
     """
 
+    GET: MultiDict
+    POST: MultiDict
+
     def __init__(self):
         super(DummyRequest, self).__init__()
         self.GET = MultiDict()
         self.POST = MultiDict()
 
 
 class _TestHarness(object):
@@ -83,18 +87,19 @@
 
     python -munittest pyramid_formencode_classic.tests.core.TestRenderSimple_FormA_HtmlErrorPlaceholder_Default \
                       pyramid_formencode_classic.tests.core.TestRenderSimple_FormA_HtmlErrorPlaceholder_Explicit \
                       pyramid_formencode_classic.tests.core.TestRenderSimple_FormA_HtmlErrorPlaceholder_Alt \
                       pyramid_formencode_classic.tests.core.TestRenderSimple_FormA_HtmlErrorPlaceholder_None
     """
 
-    template = None
+    template: str
+    _test_render_simple__data: Dict
+    request: Request
 
     def test_render_simple(self):
-
         _template = self.template
         _response_text = self._test_render_simple__data["response_text"]
 
         def _print_form_simple():
             rendered = render_to_response(_template, {"request": self.request})
             return rendered
 
@@ -120,49 +125,49 @@
                       pyramid_formencode_classic.tests.core.TestParsing_FormA_HtmlErrorPlaceholder \
                       pyramid_formencode_classic.tests.core.TestParsing_FormA_NoErrorMain \
                       pyramid_formencode_classic.tests.core.TestParsingErrorFormatters_FormA_HtmlErrorPlaceholder \
                       pyramid_formencode_classic.tests.core.TestParsingErrorFormatters_FormA_HtmlErrorPlaceholder_Alt \
                       pyramid_formencode_classic.tests.core.TestParsingErrorFormatters_FormA_NoErrorMain
     """
 
-    error_main_key = None
-    template = None
-    _test_submit__data = None  # placeholder
-    _test_no_params__data = None  # placeholder
+    _test_submit__data: Dict  # placeholder
+    _test_no_params__data: Dict  # placeholder
+    error_main_key: Optional[str] = None
+    template: str
+    request: Request
 
     def test_no_params(self):
-
         tests_completed = []
         tests_fail = []
 
         for test_name, test_data in self._test_no_params__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid()
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
@@ -185,45 +190,44 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_submit(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_submit__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid()
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
@@ -1820,15 +1824,14 @@
     python -munittest pyramid_formencode_classic.tests.core.TestCustomError
     """
 
     error_main_key = None
     template = "fixtures/form_a-html_error_placeholder-default.mako"
 
     def test_submit(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         # custom formatter
         def main_error_formatter(error):
             TEMPLATE_FORMSTASH_ERRORS = """<div class="alert alert-error"><div class="control-group error"><span class="help-inline"><i class="fa fa-exclamation-triangle"></i> %(error)s</span></div></div>"""
             return (
@@ -1843,39 +1846,39 @@
             ) + "\n"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_submit__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {"error_formatters": {}}
+            _reprint_kwargs: Dict = {"error_formatters": {}}
             if "error_formatters_default" in test_data:
                 if test_data["error_formatters_default"] == "main_error_formatter":
                     _reprint_kwargs["error_formatters"][
                         "default"
                     ] = main_error_formatter
             if "error_formatters_alt" in test_data:
                 if test_data["error_formatters_alt"] == "alt_error_formatter":
                     _reprint_kwargs["error_formatters"]["alt"] = alt_error_formatter
 
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             html_error_placeholder_template = test_data.get(
                 "html_error_placeholder_template", None
             )
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if html_error_placeholder_template:
                     formStash.html_error_placeholder_template = (
                         html_error_placeholder_template
                     )
 
                 if not result:
@@ -1953,15 +1956,14 @@
 
     python -munittest pyramid_formencode_classic.tests.core.TestMultiForm
     """
 
     template = "fixtures/form_b-multi.mako"
 
     def test_render_simple(self):
-
         _template = self.template
         _response_text = self._test_data["response_text-test_render_simple"]
 
         def _print_form_simple():
             rendered = render_to_response(_template, {"request": self.request})
             return rendered
 
@@ -1974,32 +1976,31 @@
                 print(rendered.text)
                 print("------------")
             raise
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_parse(self):
-
         _template = self.template
-        _validate_kwargs = {}
-        _reprint_kwargs = {}
+        _validate_kwargs: Dict = {}
+        _reprint_kwargs: Dict = {}
         html_error_placeholder_template = None
 
         def _print_form_simple():
             rendered = render_to_response(_template, {"request": self.request})
             return rendered
 
         # render form A
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 form_stash="a",
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if html_error_placeholder_template:
                 formStash.html_error_placeholder_template = (
                     html_error_placeholder_template
                 )
 
             if not result:
@@ -2026,15 +2027,15 @@
         # render form B
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 form_stash="b",
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if html_error_placeholder_template:
                 formStash.html_error_placeholder_template = (
                     html_error_placeholder_template
                 )
 
             if not result:
@@ -2057,37 +2058,36 @@
                     print("%s.test_parse" % self.__class__)
                     print(rendered.text)
                 raise
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_parse_error(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
         self.request.POST["email"] = "failmail"
         self.request.POST["username"] = ""
 
         _template = self.template
-        _validate_kwargs = {}
-        _reprint_kwargs = {}
+        _validate_kwargs: Dict = {}
+        _reprint_kwargs: Dict = {}
         html_error_placeholder_template = None
 
         def _print_form_simple():
             rendered = render_to_response(_template, {"request": self.request})
             return rendered
 
         # render form A
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 form_stash="a",
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if html_error_placeholder_template:
                 formStash.html_error_placeholder_template = (
                     html_error_placeholder_template
                 )
 
             if not result:
@@ -2100,15 +2100,15 @@
         except pyramid_formencode_classic.FormInvalid as exc:
             formStash.register_error_main_exception(exc)
             rendered = pyramid_formencode_classic.form_reprint(
                 self.request,
                 _print_form_simple,
                 form_stash="a",
                 data_formencode_form="a",
-                **_reprint_kwargs
+                **_reprint_kwargs,
             )
             try:
                 assert (
                     rendered.text == self._test_data["response_text-test_parse_error-a"]
                 )
             except:
                 if DEBUG_PRINT:
@@ -2120,15 +2120,15 @@
         # render form B
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 form_stash="b",
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if html_error_placeholder_template:
                 formStash.html_error_placeholder_template = (
                     html_error_placeholder_template
                 )
 
             if not result:
@@ -2141,15 +2141,15 @@
         except pyramid_formencode_classic.FormInvalid as exc:
             formStash.register_error_main_exception(exc)
             rendered = pyramid_formencode_classic.form_reprint(
                 self.request,
                 _print_form_simple,
                 form_stash="b",
                 data_formencode_form="b",
-                **_reprint_kwargs
+                **_reprint_kwargs,
             )
             try:
                 assert (
                     rendered.text == self._test_data["response_text-test_parse_error-b"]
                 )
             except:
                 if DEBUG_PRINT:
@@ -2258,57 +2258,57 @@
 class _TestParsingApi040(object):
     """
 
     python -munittest pyramid_formencode_classic.tests.core.TestParsingApi040_FormA_HtmlErrorPlaceholder_Default
     """
 
     error_main_key = None
-    template = None
+    template: str
+    request: Request
 
-    _test_manual_error_append__data = None  # placeholder
-    _test_manual_error_prepend__data = None  # placeholder
-    _test_manual_error_default__data = None  # placeholder
-    _test_fatal_form__data = None  # placeholder
-    _test_fatal_field__data = None  # placeholder
-    _test_raise_form_aware__data = None  # placeholder
+    _test_manual_error_append__data: Dict  # placeholder
+    _test_manual_error_prepend__data: Dict  # placeholder
+    _test_manual_error_default__data: Dict  # placeholder
+    _test_fatal_form__data: Dict  # placeholder
+    _test_fatal_field__data: Dict  # placeholder
+    _test_raise_form_aware__data: Dict  # placeholder
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_manual_error_default(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_manual_error_default__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid("OVERRIDE MESSAGE.")
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
@@ -2334,45 +2334,44 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_manual_error_append(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_manual_error_append__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid("OVERRIDE MESSAGE.")
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
@@ -2400,45 +2399,44 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_manual_error_prepend(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_manual_error_prepend__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid("OVERRIDE MESSAGE.")
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
@@ -2466,45 +2464,44 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_fatal_form(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_fatal_form__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 formStash.fatal_form(message="FATAL FORM.")
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
 
@@ -2543,45 +2540,44 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_fatal_field(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_fatal_field__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 formStash.fatal_field(
                     field="email", message="THIS FIELD CAUSED A FATAL ERROR."
                 )
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
@@ -2622,56 +2618,55 @@
 
         if tests_fail:
             raise ValueError(tests_fail)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
     def test_raise_form_aware(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
         tests_completed = []
         tests_fail = []
         for test_name, test_data in self._test_raise_form_aware__data.items():
             _template = self.template
             _response_text = test_data["response_text"]
-            _reprint_kwargs = {}
+            _reprint_kwargs: Dict = {}
             if "auto_error_formatter" in test_data:
                 _reprint_kwargs["auto_error_formatter"] = test_data[
                     "auto_error_formatter"
                 ]
             if "error_formatters" in test_data:
                 if test_data["error_formatters"] is not None:
                     _reprint_kwargs["error_formatters"] = test_data["error_formatters"]
-            _validate_kwargs = {}
+            _validate_kwargs: Dict = {}
             if self.error_main_key is not None:
                 _validate_kwargs["error_main_key"] = self.error_main_key
 
             def _print_form_simple():
                 rendered = render_to_response(_template, {"request": self.request})
                 return rendered
 
             try:
                 (result, formStash) = pyramid_formencode_classic.form_validate(
                     self.request,
                     schema=Form_EmailUsername,
                     error_main_text="There was an error with your form.",
-                    **_validate_kwargs
+                    **_validate_kwargs,
                 )
                 if not result:
                     raise pyramid_formencode_classic.FormInvalid(
                         "OVERRIDE MESSAGE.", form=formStash
                     )
 
                 raise ValueError(
                     "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
                 )
 
-            except pyramid_formencode_classic.FormInvalid as exc:
+            except pyramid_formencode_classic.FormInvalid as exc:  # noqa: F841
                 rendered = pyramid_formencode_classic.form_reprint(
                     self.request, _print_form_simple, **_reprint_kwargs
                 )
                 try:
                     assert rendered.text == _response_text
                 except:
                     if DEBUG_PRINT:
@@ -3359,22 +3354,21 @@
 <span class="error-message">Missing value</span>
 <input type="text" name="username" value="" class="error" />
 </form>
 </div></body></html>
 """
 
     def test_submit(self):
-
         # set the submit
         self.request.POST["submit"] = "submit"
 
-        _template = self.template
+        # _template = self.template
         _rendered = self.rendered
-        _reprint_kwargs = {}
-        _validate_kwargs = {}
+        _reprint_kwargs: Dict = {}
+        _validate_kwargs: Dict = {}
 
         def _print_form__valid():
             rendered = render_to_response(self.template, {"request": self.request})
             return rendered
 
         def _print_form__fail():
             unrendered = {"request": self.request}
@@ -3382,15 +3376,15 @@
 
         # first print this RIGHT
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if not result:
                 raise pyramid_formencode_classic.FormInvalid()
 
             raise ValueError(
                 "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
             )
@@ -3404,15 +3398,15 @@
 
         # then print this WRONG
         try:
             (result, formStash) = pyramid_formencode_classic.form_validate(
                 self.request,
                 schema=Form_EmailUsername,
                 error_main_text="There was an error with your form.",
-                **_validate_kwargs
+                **_validate_kwargs,
             )
             if not result:
                 raise pyramid_formencode_classic.FormInvalid()
 
             raise ValueError(
                 "`form_validate` should have raised `pyramid_formencode_classic.FormInvalid`"
             )
```

