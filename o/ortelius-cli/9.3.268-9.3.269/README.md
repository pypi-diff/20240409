# Comparing `tmp/ortelius-cli-9.3.268.tar.gz` & `tmp/ortelius-cli-9.3.269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.268.tar", last modified: Thu Apr  4 17:11:50 2024, max compression
+gzip compressed data, was "ortelius-cli-9.3.269.tar", last modified: Tue Apr  9 21:22:28 2024, max compression
```

## Comparing `ortelius-cli-9.3.268.tar` & `ortelius-cli-9.3.269.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 17:11:50.393519 ortelius-cli-9.3.268/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.268/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.268/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-04 17:11:50.391509 ortelius-cli-9.3.268/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.268/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 17:11:50.366458 ortelius-cli-9.3.268/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    70828 2024-04-04 17:11:28.000000 ortelius-cli-9.3.268/bin/dh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 17:11:50.369383 ortelius-cli-9.3.268/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-04 17:11:28.000000 ortelius-cli-9.3.268/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    71098 2024-03-21 23:53:08.000000 ortelius-cli-9.3.268/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 17:11:50.372345 ortelius-cli-9.3.268/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.268/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.268/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 17:11:50.386859 ortelius-cli-9.3.268/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-04 17:11:50.000000 ortelius-cli-9.3.268/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-04 17:11:50.000000 ortelius-cli-9.3.268/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-04 17:11:50.000000 ortelius-cli-9.3.268/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-04 17:11:50.000000 ortelius-cli-9.3.268/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-04 17:11:50.000000 ortelius-cli-9.3.268/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-04 17:11:50.393843 ortelius-cli-9.3.268/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-04 17:11:28.000000 ortelius-cli-9.3.268/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:22:28.548410 ortelius-cli-9.3.269/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.269/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.269/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 21:22:28.547346 ortelius-cli-9.3.269/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.269/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:22:28.535142 ortelius-cli-9.3.269/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70828 2024-04-09 21:22:13.000000 ortelius-cli-9.3.269/bin/dh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:22:28.537014 ortelius-cli-9.3.269/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-09 21:22:13.000000 ortelius-cli-9.3.269/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    71171 2024-04-09 21:19:40.000000 ortelius-cli-9.3.269/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:22:28.541870 ortelius-cli-9.3.269/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.269/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.269/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-09 21:22:28.546424 ortelius-cli-9.3.269/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-09 21:22:28.000000 ortelius-cli-9.3.269/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-09 21:22:28.000000 ortelius-cli-9.3.269/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-09 21:22:28.000000 ortelius-cli-9.3.269/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-09 21:22:28.000000 ortelius-cli-9.3.269/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-09 21:22:28.000000 ortelius-cli-9.3.269/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-09 21:22:28.548602 ortelius-cli-9.3.269/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-09 21:22:13.000000 ortelius-cli-9.3.269/setup.py
```

### Comparing `ortelius-cli-9.3.268/LICENSE` & `ortelius-cli-9.3.269/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.268/PKG-INFO` & `ortelius-cli-9.3.269/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.268
+Version: 9.3.269
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.268/README.md` & `ortelius-cli-9.3.269/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.268/bin/dh` & `ortelius-cli-9.3.269/bin/dh`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.268"
+__version__ = "9.3.269"
 
 import json
 import os
 import re
 import stat
 import sys
 from datetime import datetime
```

### Comparing `ortelius-cli-9.3.268/deployhub/dhapi.py` & `ortelius-cli-9.3.269/deployhub/dhapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,18 @@
             res = requests.post(url, data=payload, cookies=cookies, headers={"Content-Type": "application/json", "host": "console.deployhub.com"}, timeout=300)
 
         if res is None:
             return None
 
         if res.status_code < 200 and res.status_code > 299:
             return None
+        
+        if len(res.text) == 0:
+            return None
+        
         return res.json()
     except requests.exceptions.ConnectionError as conn_error:
         print(str(conn_error))
     return None
 
 
 def post_json_with_header(url, token):
```

### Comparing `ortelius-cli-9.3.268/doc/deployhub.md` & `ortelius-cli-9.3.269/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.268/doc/dh.md` & `ortelius-cli-9.3.269/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.268/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.269/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.268
+Version: 9.3.269
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.268/setup.py` & `ortelius-cli-9.3.269/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.268",
+    version="9.3.269",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

