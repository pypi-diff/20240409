# Comparing `tmp/alfred-workflow-packager-3.1.0b1.tar.gz` & `tmp/alfred-workflow-packager-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred-workflow-packager-3.1.0b1.tar", last modified: Sat Mar 30 19:51:00 2024, max compression
+gzip compressed data, was "alfred-workflow-packager-3.1.1.tar", last modified: Tue Apr  9 16:06:45 2024, max compression
```

## Comparing `alfred-workflow-packager-3.1.0b1.tar` & `alfred-workflow-packager-3.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-30 19:51:00.000000 alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/awp/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/argparse_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/awp/data/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/data/config-schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9843 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/packager.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/awp/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-30 19:50:50.000000 alfred-workflow-packager-3.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 19:51:00.429229 alfred-workflow-packager-3.1.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 16:06:45.000000 alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/awp/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/argparse_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/awp/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/data/config-schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9872 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/packager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/awp/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-09 16:06:33.000000 alfred-workflow-packager-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:06:45.934551 alfred-workflow-packager-3.1.1/setup.cfg
```

### Comparing `alfred-workflow-packager-3.1.0b1/LICENSE.txt` & `alfred-workflow-packager-3.1.1/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016-2023 Caleb Evans
+Copyright (c) 2016-2024 Caleb Evans
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `alfred-workflow-packager-3.1.0b1/PKG-INFO` & `alfred-workflow-packager-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: alfred-workflow-packager
-Version: 3.1.0b1
+Version: 3.1.1
 Summary: A CLI utility for packaging and exporting Alfred workflows
 Author-email: Caleb Evans <caleb@calebevans.me>
 Maintainer-email: Caleb Evans <caleb@calebevans.me>
 License: The MIT License (MIT)
         
-        Copyright (c) 2016-2023 Caleb Evans
+        Copyright (c) 2016-2024 Caleb Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -34,15 +34,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: jsonschema<5,>=4
 
 # Alfred Workflow Packager
 
-*Copyright 2016-2023 Caleb Evans*  
+*Copyright 2016-2024 Caleb Evans*  
 *Released under the MIT license*
 
 Alfred Workflow Packager is a command-line utility which makes the process of
 packaging and exporting an [Alfred](https://www.alfredapp.com/) workflow
 incredibly quick and easy. The utility supports Alfred 3 and up, on projects running Python 3 (Python 2 is no longer supported).
 
 ## Setup
```

### Comparing `alfred-workflow-packager-3.1.0b1/README.md` & `alfred-workflow-packager-3.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Alfred Workflow Packager
 
-*Copyright 2016-2023 Caleb Evans*  
+*Copyright 2016-2024 Caleb Evans*  
 *Released under the MIT license*
 
 Alfred Workflow Packager is a command-line utility which makes the process of
 packaging and exporting an [Alfred](https://www.alfredapp.com/) workflow
 incredibly quick and easy. The utility supports Alfred 3 and up, on projects running Python 3 (Python 2 is no longer supported).
 
 ## Setup
```

### Comparing `alfred-workflow-packager-3.1.0b1/alfred_workflow_packager.egg-info/PKG-INFO` & `alfred-workflow-packager-3.1.1/alfred_workflow_packager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: alfred-workflow-packager
-Version: 3.1.0b1
+Version: 3.1.1
 Summary: A CLI utility for packaging and exporting Alfred workflows
 Author-email: Caleb Evans <caleb@calebevans.me>
 Maintainer-email: Caleb Evans <caleb@calebevans.me>
 License: The MIT License (MIT)
         
-        Copyright (c) 2016-2023 Caleb Evans
+        Copyright (c) 2016-2024 Caleb Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -34,15 +34,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: jsonschema<5,>=4
 
 # Alfred Workflow Packager
 
-*Copyright 2016-2023 Caleb Evans*  
+*Copyright 2016-2024 Caleb Evans*  
 *Released under the MIT license*
 
 Alfred Workflow Packager is a command-line utility which makes the process of
 packaging and exporting an [Alfred](https://www.alfredapp.com/) workflow
 incredibly quick and easy. The utility supports Alfred 3 and up, on projects running Python 3 (Python 2 is no longer supported).
 
 ## Setup
```

### Comparing `alfred-workflow-packager-3.1.0b1/awp/argparse_extras.py` & `alfred-workflow-packager-3.1.1/awp/argparse_extras.py`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.1.0b1/awp/data/config-schema.json` & `alfred-workflow-packager-3.1.1/awp/data/config-schema.json`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.1.0b1/awp/main.py` & `alfred-workflow-packager-3.1.1/awp/main.py`

 * *Files identical despite different names*

### Comparing `alfred-workflow-packager-3.1.0b1/awp/packager.py` & `alfred-workflow-packager-3.1.1/awp/packager.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import contextlib
 import filecmp
 import glob
 import os
 import os.path
 import plistlib
+import re
 import shutil
 import xml
 from zipfile import ZIP_DEFLATED, ZipFile
 
 
 # Create parent directories for the given path if they don't exist
 def create_parent_dirs(path):
@@ -204,16 +205,16 @@
         info["readme"] = new_readme
         print("Updated workflow README")
 
 
 # Set the workflow version to a new version number if one is given
 def update_workflow_version(info, new_version_num):
     if new_version_num:
-        info["version"] = new_version_num
-        print("Set version to v{version}".format(version=new_version_num))
+        info["version"] = re.sub(r"^v", "", new_version_num)
+        print("Set version to v{version}".format(version=info["version"]))
 
 
 # Write installed workflow subdirectory files to the given zip file
 def zip_workflow_dir_files(workflow_path, zip_file, root, relative_root, files):
     for file_name in files:
         file_path = os.path.join(root, file_name)
         # Get path to current file relative to workflow directory
```

### Comparing `alfred-workflow-packager-3.1.0b1/pyproject.toml` & `alfred-workflow-packager-3.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "alfred-workflow-packager"
-version = "3.1.0-beta.1"
+version = "3.1.1"
 description = "A CLI utility for packaging and exporting Alfred workflows"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
     {name = "Caleb Evans", email = "caleb@calebevans.me"}
 ]
 maintainers = [
```

