# Comparing `tmp/prosperity2submit-0.2.2.tar.gz` & `tmp/prosperity2submit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.2.2.tar", last modified: Mon Apr  8 11:38:13 2024, max compression
+gzip compressed data, was "prosperity2submit-0.2.3.tar", last modified: Tue Apr  9 15:27:11 2024, max compression
```

## Comparing `prosperity2submit-0.2.2.tar` & `prosperity2submit-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:13.980605 prosperity2submit-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 11:38:10.000000 prosperity2submit-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-08 11:38:13.980605 prosperity2submit-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-08 11:38:10.000000 prosperity2submit-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:13.980605 prosperity2submit-0.2.2/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:10.000000 prosperity2submit-0.2.2/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-08 11:38:10.000000 prosperity2submit-0.2.2/prosperity2submit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-08 11:38:10.000000 prosperity2submit-0.2.2/prosperity2submit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:38:13.980605 prosperity2submit-0.2.2/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 11:38:13.000000 prosperity2submit-0.2.2/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 11:38:11.000000 prosperity2submit-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 11:38:13.980605 prosperity2submit-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-09 15:27:07.000000 prosperity2submit-0.2.3/prosperity2submit/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:27:11.000000 prosperity2submit-0.2.3/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-09 15:27:08.000000 prosperity2submit-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:27:11.171610 prosperity2submit-0.2.3/setup.cfg
```

### Comparing `prosperity2submit-0.2.2/LICENSE` & `prosperity2submit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.2/PKG-INFO` & `prosperity2submit-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.2/README.md` & `prosperity2submit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.2/prosperity2submit/core.py` & `prosperity2submit-0.2.3/prosperity2submit/core.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.2.2/prosperity2submit/main.py` & `prosperity2submit-0.2.3/prosperity2submit/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,7 +33,10 @@
     elif args.no_logs:
         output_file = None
     else:
         timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         output_file = Path.cwd() / "submissions" / f"{timestamp}.log"
 
     submit(algorithm_file, output_file, args.vis)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `prosperity2submit-0.2.2/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.2.3/prosperity2submit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2submit-0.2.2/pyproject.toml` & `prosperity2submit-0.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -21,15 +21,15 @@
 dependencies = [
     "keyring",
     "requests",
     "requests-toolbelt",
 ]
 
 [project.scripts]
-prosperity2submit = "prosperity2submit.main:main"
+prosperity2submit = "prosperity2submit.__main__:main"
 
 [project.urls]
 Repository = "https://github.com/jmerle/imc-prosperity-2-submitter"
 Issues = "https://github.com/jmerle/imc-prosperity-2-submitter/issues"
 Changelog = "https://github.com/jmerle/imc-prosperity-2-submitter/releases"
 
 [tool.setuptools.packages.find]
```

