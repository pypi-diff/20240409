# Comparing `tmp/dynamic-yaml-1.3.5.tar.gz` & `tmp/dynamic-yaml-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-yaml-1.3.5.tar", last modified: Tue Oct 24 21:47:01 2023, max compression
+gzip compressed data, was "dynamic-yaml-2.0.0.tar", last modified: Tue Apr  9 20:52:37 2024, max compression
```

## Comparing `dynamic-yaml-1.3.5.tar` & `dynamic-yaml-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1071 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/LICENSE.txt
--rw-r--r--   0 liam      (1000) liam      (1000)     6461 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)     4699 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/dynamic_yaml/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1766 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/dynamic_yaml/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3242 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/dynamic_yaml/yaml_wrappers.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/
--rw-r--r--   0 liam      (1000) liam      (1000)     6461 2023-10-24 21:47:01.000000 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      327 2023-10-24 21:47:01.000000 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-10-24 21:47:01.000000 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       12 2023-10-24 21:47:01.000000 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       13 2023-10-24 21:47:01.000000 dynamic-yaml-1.3.5/dynamic_yaml.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      653 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/pyproject.toml
--rw-rw-r--   0 liam      (1000) liam      (1000)       38 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/setup.cfg
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-10-24 21:47:01.045581 dynamic-yaml-1.3.5/tests/
--rw-rw-r--   0 liam      (1000) liam      (1000)     8082 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/tests/test_dynamic_yaml.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1164 2023-10-24 21:45:42.000000 dynamic-yaml-1.3.5/tests/test_representations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:37.789964 dynamic-yaml-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-09 20:52:37.789964 dynamic-yaml-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:37.785964 dynamic-yaml-2.0.0/dynamic_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/dynamic_yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/dynamic_yaml/yaml_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:37.789964 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-09 20:52:37.000000 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 20:52:37.000000 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:52:37.000000 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 20:52:37.000000 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 20:52:37.000000 dynamic-yaml-2.0.0/dynamic_yaml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:52:37.789964 dynamic-yaml-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:52:37.789964 dynamic-yaml-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/tests/test_dynamic_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-09 20:52:32.000000 dynamic-yaml-2.0.0/tests/test_representations.py
```

### Comparing `dynamic-yaml-1.3.5/LICENSE.txt` & `dynamic-yaml-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.5/PKG-INFO` & `dynamic-yaml-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-yaml
-Version: 1.3.5
+Version: 2.0.0
 Summary: Enables self referential yaml entries
 Author-email: "Liam H. Childs" <liam.h.childs@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Liam H. Childs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dynamic-yaml-1.3.5/README.md` & `dynamic-yaml-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.5/dynamic_yaml/__init__.py` & `dynamic-yaml-2.0.0/dynamic_yaml/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 
 def load(stream, loader=DynamicYamlLoader, recursive=False):
     result = yaml.load(stream, Loader=loader)
     result._set_as_root(recursive=recursive)
     return result
 
 
-def dump(data, *args, **kwargs):
-    return yaml.dump(data, *args, **kwargs)
+def dump(data, sort_keys=False, *args, **kwargs):
+    return yaml.dump(data, sort_keys=sort_keys, *args, **kwargs)
 
 
 add_wrappers(DynamicYamlLoader)
```

### Comparing `dynamic-yaml-1.3.5/dynamic_yaml/yaml_wrappers.py` & `dynamic-yaml-2.0.0/dynamic_yaml/yaml_wrappers.py`

 * *Files identical despite different names*

### Comparing `dynamic-yaml-1.3.5/dynamic_yaml.egg-info/PKG-INFO` & `dynamic-yaml-2.0.0/dynamic_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-yaml
-Version: 1.3.5
+Version: 2.0.0
 Summary: Enables self referential yaml entries
 Author-email: "Liam H. Childs" <liam.h.childs@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Liam H. Childs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dynamic-yaml-1.3.5/pyproject.toml` & `dynamic-yaml-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dynamic-yaml"
-version = "1.3.5"
+version = "2.0.0"
 description = "Enables self referential yaml entries"
 readme = "README.md"
 authors = [{ name = "Liam H. Childs", email = "liam.h.childs@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `dynamic-yaml-1.3.5/tests/test_dynamic_yaml.py` & `dynamic-yaml-2.0.0/tests/test_dynamic_yaml.py`

 * *Files identical despite different names*

