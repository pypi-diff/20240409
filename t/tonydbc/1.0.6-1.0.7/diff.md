# Comparing `tmp/tonydbc-1.0.6.tar.gz` & `tmp/tonydbc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonydbc-1.0.6.tar", last modified: Sat Feb 10 11:39:12 2024, max compression
+gzip compressed data, was "tonydbc-1.0.7.tar", last modified: Tue Apr  9 06:14:00 2024, max compression
```

## Comparing `tonydbc-1.0.6.tar` & `tonydbc-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-02-10 11:39:12.965463 tonydbc-1.0.6/
--rw-rw-rw-   0        0        0     1083 2024-01-08 09:25:07.000000 tonydbc-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       43 2024-01-08 09:25:07.000000 tonydbc-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4227 2024-02-10 11:39:12.964463 tonydbc-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1907 2024-02-10 11:38:50.000000 tonydbc-1.0.6/README.md
--rw-rw-rw-   0        0        0     1503 2024-02-10 11:38:50.000000 tonydbc-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-10 11:39:12.965463 tonydbc-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-10 11:39:12.894112 tonydbc-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-02-10 11:39:12.938461 tonydbc-1.0.6/src/tonydbc/
--rw-rw-rw-   0        0        0     1243 2024-02-10 11:38:50.000000 tonydbc-1.0.6/src/tonydbc/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-08 09:25:07.000000 tonydbc-1.0.6/src/tonydbc/config.toml
--rw-rw-rw-   0        0        0     6000 2024-01-20 15:36:46.000000 tonydbc-1.0.6/src/tonydbc/create_test_database.py
--rw-rw-rw-   0        0        0    11534 2024-02-10 11:38:27.000000 tonydbc-1.0.6/src/tonydbc/dataframe_fast.py
--rw-rw-rw-   0        0        0     6766 2024-01-20 15:22:24.000000 tonydbc-1.0.6/src/tonydbc/env_utils.py
--rw-rw-rw-   0        0        0     3860 2024-01-08 09:25:07.000000 tonydbc-1.0.6/src/tonydbc/mqtt_client.py
--rw-rw-rw-   0        0        0     7372 2024-01-20 13:50:57.000000 tonydbc-1.0.6/src/tonydbc/tony_utils.py
--rw-rw-rw-   0        0        0    44595 2024-02-10 10:49:32.000000 tonydbc-1.0.6/src/tonydbc/tonydbc.py
-drwxrwxrwx   0        0        0        0 2024-02-10 11:39:12.962713 tonydbc-1.0.6/src/tonydbc.egg-info/
--rw-rw-rw-   0        0        0     4227 2024-02-10 11:39:12.000000 tonydbc-1.0.6/src/tonydbc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-02-10 11:39:12.000000 tonydbc-1.0.6/src/tonydbc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-10 11:39:12.000000 tonydbc-1.0.6/src/tonydbc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2024-02-10 11:39:12.000000 tonydbc-1.0.6/src/tonydbc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-10 11:39:12.000000 tonydbc-1.0.6/src/tonydbc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 06:14:00.065865 tonydbc-1.0.7/
+-rw-rw-rw-   0        0        0     1083 2024-01-08 09:25:07.000000 tonydbc-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-01-08 09:25:07.000000 tonydbc-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4227 2024-04-09 06:14:00.062864 tonydbc-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1907 2024-04-09 06:13:24.000000 tonydbc-1.0.7/README.md
+-rw-rw-rw-   0        0        0     1503 2024-04-09 06:13:24.000000 tonydbc-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 06:14:00.065865 tonydbc-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 06:13:59.988865 tonydbc-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 06:14:00.005864 tonydbc-1.0.7/src/tonydbc/
+-rw-rw-rw-   0        0        0     1243 2024-04-09 06:13:24.000000 tonydbc-1.0.7/src/tonydbc/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-08 09:25:07.000000 tonydbc-1.0.7/src/tonydbc/config.toml
+-rw-rw-rw-   0        0        0     6000 2024-01-20 15:36:46.000000 tonydbc-1.0.7/src/tonydbc/create_test_database.py
+-rw-rw-rw-   0        0        0    11534 2024-02-10 11:38:27.000000 tonydbc-1.0.7/src/tonydbc/dataframe_fast.py
+-rw-rw-rw-   0        0        0     8763 2024-04-09 06:12:19.000000 tonydbc-1.0.7/src/tonydbc/env_utils.py
+-rw-rw-rw-   0        0        0     3860 2024-01-08 09:25:07.000000 tonydbc-1.0.7/src/tonydbc/mqtt_client.py
+-rw-rw-rw-   0        0        0     7372 2024-01-20 13:50:57.000000 tonydbc-1.0.7/src/tonydbc/tony_utils.py
+-rw-rw-rw-   0        0        0    44595 2024-02-10 10:49:32.000000 tonydbc-1.0.7/src/tonydbc/tonydbc.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:14:00.059864 tonydbc-1.0.7/src/tonydbc.egg-info/
+-rw-rw-rw-   0        0        0     4227 2024-04-09 06:13:59.000000 tonydbc-1.0.7/src/tonydbc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-04-09 06:13:59.000000 tonydbc-1.0.7/src/tonydbc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 06:13:59.000000 tonydbc-1.0.7/src/tonydbc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2024-04-09 06:13:59.000000 tonydbc-1.0.7/src/tonydbc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 06:13:59.000000 tonydbc-1.0.7/src/tonydbc.egg-info/top_level.txt
```

### Comparing `tonydbc-1.0.6/LICENSE` & `tonydbc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/PKG-INFO` & `tonydbc-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonydbc
-Version: 1.0.6
+Version: 1.0.7
 Summary: A high-level database connector for MariaDB
 Author-email: Michael Currie <mcurrie@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Fling
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # TonyDBC
 
-Latest version: 1.0.6
+Latest version: 1.0.7
 
 Available on PyPI: https://pypi.org/project/tonydbc/
 
 2024-01-07: [Release announcement on Medium](https://mcurrie-59915.medium.com/introducing-tonydbc-a-high-level-database-connector-for-mariadb-python-and-pandas-8600676fbf88)
 
 Supports high-level database operations within Python.  TonyDBC is short for Tony’s Database Connector, named for Maria’s lover in West Side Story.
```

### Comparing `tonydbc-1.0.6/README.md` & `tonydbc-1.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # TonyDBC
 
-Latest version: 1.0.6
+Latest version: 1.0.7
 
 Available on PyPI: https://pypi.org/project/tonydbc/
 
 2024-01-07: [Release announcement on Medium](https://mcurrie-59915.medium.com/introducing-tonydbc-a-high-level-database-connector-for-mariadb-python-and-pandas-8600676fbf88)
 
 Supports high-level database operations within Python.  TonyDBC is short for Tony’s Database Connector, named for Maria’s lover in West Side Story.
```

### Comparing `tonydbc-1.0.6/pyproject.toml` & `tonydbc-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tonydbc"
-version = "1.0.6"
+version = "1.0.7"
 description = "A high-level database connector for MariaDB"
 readme = "README.md"
 authors = [{ name = "Michael Currie", email = "mcurrie@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -37,15 +37,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/Fling-Asia/tonydbc"
 
 [tool.bumpver]
-current_version = "1.0.6"
+current_version = "1.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `tonydbc-1.0.6/src/tonydbc/__init__.py` & `tonydbc-1.0.7/src/tonydbc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     MEDIA_BASE_PATH_PRODUCTION  = C:\\
 
 e.g. 
     import tonydbc
     tonydbc.load_dotenvs()
 
 """
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 
 from .env_utils import get_env_bool, get_env_list, load_dotenv, load_dotenvs
 from .tony_utils import (
     set_MYSQL_DATABASE,
     get_current_time,
     get_current_time_string,
     deserialize_table,
```

### Comparing `tonydbc-1.0.6/src/tonydbc/create_test_database.py` & `tonydbc-1.0.7/src/tonydbc/create_test_database.py`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/src/tonydbc/dataframe_fast.py` & `tonydbc-1.0.7/src/tonydbc/dataframe_fast.py`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/src/tonydbc/env_utils.py` & `tonydbc-1.0.7/src/tonydbc/env_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,21 +15,32 @@
 
 load_dotenvs() is all you need in most cases
 """
 
 import code
 import os
 import sys
+import logging
 import dotenv
 from dotenv import load_dotenv
 import json
 import pathlib
 from collections import Counter
 
 
+# We need this to capture the logging warning "Python-dotenv could not parse statement starting at line 1"
+class CaptureLogsHandler(logging.Handler):
+    def __init__(self):
+        super().__init__()
+        self.messages = []
+
+    def emit(self, record):
+        self.messages.append(record.getMessage())
+
+
 def check_duplicate_keys(dotenv_path):
     # Load key-value pairs from the .env file
     env_dict = dotenv.dotenv_values(dotenv_path)
 
     # Read the file again as a plain text file
     with open(dotenv_path, "r") as f:
         lines = f.readlines()
@@ -67,34 +78,73 @@
 
     if not os.path.isfile(example_env_filepath):
         raise AssertionError(
             "Your repo is missing a `.env.example` file in "
             f"{pathlib.Path(env_filepath).parent}\n"
         )
 
+    # We need this to capture the logging warning
+    # "Python-dotenv could not parse statement starting at line 1"
+    # Create the custom logging handler
+    dotenv_handler = CaptureLogsHandler()
+
+    # Get the logger for 'dotenv' and attach the handler
+    dotenv_logger = logging.getLogger("dotenv")
+    dotenv_logger.addHandler(dotenv_handler)
+    dotenv_logger.setLevel(logging.WARNING)
+
+    # LOAD the files to check for parsing errors
+    for fp in [env_filepath, example_env_filepath]:
+        dotenv.dotenv_values(fp)
+        parsed_errors = [
+            msg
+            for msg in dotenv_handler.messages
+            if "could not parse statement starting" in msg
+        ]
+        if len(parsed_errors) > 0:
+            raise AssertionError(f"{fp} contains errors {parsed_errors}")
+
     # Check for duplicate keys
     check_duplicate_keys(env_filepath)
     check_duplicate_keys(example_env_filepath)
 
-    # Check for missing keys in either file
+    # Check for DIFFERENCES in keys between the two files
     current_env = dotenv.dotenv_values(env_filepath)
     example_env = dotenv.dotenv_values(example_env_filepath)
-
     current_keys = set(current_env.keys())
     example_keys = set(example_env.keys())
 
+    # Check for missing keys in either file
     # Check the symmetric difference; if it's nonempty, a key is missing in
     # one or the other of the files
     if len(current_keys ^ example_keys) > 0:
         raise AssertionError(
+            f"For .env {env_filepath}:\n"
             "Your .env file and .env.example files have different variables defined.  Please fix this; \n "
             f"in .env but not in .env.example we have: {sorted(current_keys.difference(example_keys))}\n"
             f"in .env.example but not in .env we have: {sorted(example_keys.difference(current_keys))}\n"
         )
 
+    # Check that all variables ending in _PATH or _DIRECTORY are valid paths
+    path_keys = [
+        k
+        for k in current_keys
+        if any(k.endswith(j) for j in ["_PATH", "_DIRECTORY", "_FILEPATH"])
+    ]
+    for current_key in path_keys:
+        k_prefix = f".env {env_filepath} has variable {current_key}"
+        current_path = current_env[current_key]
+        if current_path == "":
+            print(f"WARNING: {k_prefix} which is blank.")
+            continue
+        if not (os.path.isdir(current_path) or os.path.isfile(current_path)):
+            raise AssertionError(
+                f"For {k_prefix} with path {current_path} which is not a valid path on your machine."
+            )
+
 
 def get_env_bool(key):
     """Handles the case of a boolean environment variable"""
     if not key in os.environ:
         raise KeyError(f"No environment variable {key}")
 
     if not os.environ[key] in ("True", "False"):
@@ -203,7 +253,9 @@
             print(f"WARNING: env path {p} does not exist")
             continue
         dotenv.load_dotenv(p)
         if do_check:
             print(f"Checking environment integrity on {p}")
             # Check environment variables are consistent between .env and .env.example
             check_environment_variable_integrity(p)
+    return paths
+
```

### Comparing `tonydbc-1.0.6/src/tonydbc/mqtt_client.py` & `tonydbc-1.0.7/src/tonydbc/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/src/tonydbc/tony_utils.py` & `tonydbc-1.0.7/src/tonydbc/tony_utils.py`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/src/tonydbc/tonydbc.py` & `tonydbc-1.0.7/src/tonydbc/tonydbc.py`

 * *Files identical despite different names*

### Comparing `tonydbc-1.0.6/src/tonydbc.egg-info/PKG-INFO` & `tonydbc-1.0.7/src/tonydbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonydbc
-Version: 1.0.6
+Version: 1.0.7
 Summary: A high-level database connector for MariaDB
 Author-email: Michael Currie <mcurrie@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Fling
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,15 +50,15 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # TonyDBC
 
-Latest version: 1.0.6
+Latest version: 1.0.7
 
 Available on PyPI: https://pypi.org/project/tonydbc/
 
 2024-01-07: [Release announcement on Medium](https://mcurrie-59915.medium.com/introducing-tonydbc-a-high-level-database-connector-for-mariadb-python-and-pandas-8600676fbf88)
 
 Supports high-level database operations within Python.  TonyDBC is short for Tony’s Database Connector, named for Maria’s lover in West Side Story.
```

