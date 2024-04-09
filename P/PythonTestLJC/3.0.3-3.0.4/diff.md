# Comparing `tmp/PythonTestLJC-3.0.3.tar.gz` & `tmp/PythonTestLJC-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonTestLJC-3.0.3.tar", last modified: Mon Mar 11 17:05:04 2024, max compression
+gzip compressed data, was "PythonTestLJC-3.0.4.tar", last modified: Tue Apr  9 13:54:17 2024, max compression
```

## Comparing `PythonTestLJC-3.0.3.tar` & `PythonTestLJC-3.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 17:05:04.927370 PythonTestLJC-3.0.3/
--rw-rw-rw-   0        0        0     1100 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4980 2024-03-11 17:05:04.923403 PythonTestLJC-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.3/README.md
--rw-rw-rw-   0        0        0     7147 2024-03-11 17:04:55.000000 PythonTestLJC-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-11 17:05:04.927370 PythonTestLJC-3.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 17:05:04.897781 PythonTestLJC-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 17:05:04.923403 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/
--rw-rw-rw-   0        0        0     4980 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      232 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-11 17:05:04.000000 PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 17:05:04.923403 PythonTestLJC-3.0.3/src/sample/
--rw-rw-rw-   0        0        0      114 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.3/src/sample/__init__.py
--rw-rw-rw-   0        0        0        9 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.3/src/sample/package_data.dat
--rw-rw-rw-   0        0        0      383 2024-03-11 16:51:55.000000 PythonTestLJC-3.0.3/src/sample/simple.py
-drwxrwxrwx   0        0        0        0 2024-03-11 17:05:04.923403 PythonTestLJC-3.0.3/tests/
--rw-rw-rw-   0        0        0      434 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.3/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:54:17.233275 PythonTestLJC-3.0.4/
+-rw-rw-rw-   0        0        0     1100 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5005 2024-04-09 13:54:17.231267 PythonTestLJC-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.4/README.md
+-rw-rw-rw-   0        0        0     7158 2024-04-09 13:52:46.000000 PythonTestLJC-3.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 13:54:17.233275 PythonTestLJC-3.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 13:54:17.199306 PythonTestLJC-3.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 13:54:17.230267 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/
+-rw-rw-rw-   0        0        0     5005 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      241 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 13:54:17.000000 PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 13:54:17.222268 PythonTestLJC-3.0.4/src/sample/
+-rw-rw-rw-   0        0        0      114 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.4/src/sample/__init__.py
+-rw-rw-rw-   0        0        0        9 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.4/src/sample/package_data.dat
+-rw-rw-rw-   0        0        0      398 2024-04-09 13:51:45.000000 PythonTestLJC-3.0.4/src/sample/simple.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:54:17.224273 PythonTestLJC-3.0.4/tests/
+-rw-rw-rw-   0        0        0      434 2024-03-11 15:27:17.000000 PythonTestLJC-3.0.4/tests/test_simple.py
```

### Comparing `PythonTestLJC-3.0.3/LICENSE.txt` & `PythonTestLJC-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonTestLJC-3.0.3/PKG-INFO` & `PythonTestLJC-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonTestLJC
-Version: 3.0.3
+Version: 3.0.4
 Summary: A sample Python project
 Author-email: LJC <632688200@gmail.com>
 Maintainer-email: LJC <632688200@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -60,14 +60,15 @@
 Requires-Dist: pip
 Requires-Dist: pkginfo
 Requires-Dist: plumber
 Requires-Dist: pygments
 Requires-Dist: requests_toolbelt
 Requires-Dist: readme_renderer
 Requires-Dist: requests
+Requires-Dist: pypandoc
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # A sample Python project
```

### Comparing `PythonTestLJC-3.0.3/README.md` & `PythonTestLJC-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PythonTestLJC-3.0.3/pyproject.toml` & `PythonTestLJC-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "PythonTestLJC"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "3.0.3"  # REQUIRED, although can be dynamic
+version = "3.0.4"  # REQUIRED, although can be dynamic
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A sample Python project"
 
 # This is an optional longer description of your project that represents
@@ -134,15 +134,15 @@
 	"odict",
 	"pip",
 	"pkginfo",
 	"plumber",
 	"pygments",
 	"requests_toolbelt",
 	"readme_renderer",
-	"requests"
+	"requests","pypandoc"
 ]
 
 # List additional groups of dependencies here (e.g. development
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
```

### Comparing `PythonTestLJC-3.0.3/src/PythonTestLJC.egg-info/PKG-INFO` & `PythonTestLJC-3.0.4/src/PythonTestLJC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonTestLJC
-Version: 3.0.3
+Version: 3.0.4
 Summary: A sample Python project
 Author-email: LJC <632688200@gmail.com>
 Maintainer-email: LJC <632688200@gmail.com>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -60,14 +60,15 @@
 Requires-Dist: pip
 Requires-Dist: pkginfo
 Requires-Dist: plumber
 Requires-Dist: pygments
 Requires-Dist: requests_toolbelt
 Requires-Dist: readme_renderer
 Requires-Dist: requests
+Requires-Dist: pypandoc
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 # A sample Python project
```

