# Comparing `tmp/edman_web-2024.3.5.tar.gz` & `tmp/edman_web-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_web-2024.3.5.tar", last modified: Tue Mar  5 01:29:59 2024, max compression
+gzip compressed data, was "edman_web-2024.4.9.tar", last modified: Tue Apr  9 02:01:41 2024, max compression
```

## Comparing `edman_web-2024.3.5.tar` & `edman_web-2024.4.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.991058 edman_web-2024.3.5/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2024.3.5/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2512 2024-03-05 01:29:58.991058 edman_web-2024.3.5/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      693 2023-07-19 02:31:04.000000 edman_web-2024.3.5/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.981058 edman_web-2024.3.5/edman_web/
--rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2024.3.5/edman_web/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     9483 2024-02-05 21:30:17.000000 edman_web-2024.3.5/edman_web/file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2024.3.5/edman_web/py.typed
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1743 2023-12-06 06:02:11.000000 edman_web-2024.3.5/edman_web/search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.991058 edman_web-2024.3.5/edman_web.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2512 2024-03-05 01:29:58.000000 edman_web-2024.3.5/edman_web.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      636 2024-03-05 01:29:58.000000 edman_web-2024.3.5/edman_web.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-03-05 01:29:58.000000 edman_web-2024.3.5/edman_web.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       62 2024-03-05 01:29:58.000000 edman_web-2024.3.5/edman_web.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2024-03-05 01:29:58.000000 edman_web-2024.3.5/edman_web.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1005 2024-03-05 01:28:38.000000 edman_web-2024.3.5/pyproject.toml
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-03-05 01:29:58.991058 edman_web-2024.3.5/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.981058 edman_web-2024.3.5/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    18418 2024-02-05 15:37:54.000000 edman_web-2024.3.5/tests/test_file_manager.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5897 2023-12-06 06:02:12.000000 edman_web-2024.3.5/tests/test_search_manager.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.981058 edman_web-2024.3.5/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:29:58.991058 edman_web-2024.3.5/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2024.3.5/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 00:15:38.000000 edman_web-2024.3.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.380567 edman_web-2024.4.9/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1115 2023-03-29 09:20:48.000000 edman_web-2024.4.9/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2512 2024-04-09 02:01:41.370567 edman_web-2024.4.9/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      693 2023-07-19 02:31:04.000000 edman_web-2024.4.9/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.370567 edman_web-2024.4.9/edman_web/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       82 2023-05-24 06:10:37.000000 edman_web-2024.4.9/edman_web/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     9483 2024-02-05 21:30:17.000000 edman_web-2024.4.9/edman_web/file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-23 00:36:23.000000 edman_web-2024.4.9/edman_web/py.typed
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1743 2023-12-06 06:02:11.000000 edman_web-2024.4.9/edman_web/search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.370567 edman_web-2024.4.9/edman_web.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2512 2024-04-09 02:01:41.000000 edman_web-2024.4.9/edman_web.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      636 2024-04-09 02:01:41.000000 edman_web-2024.4.9/edman_web.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 02:01:41.000000 edman_web-2024.4.9/edman_web.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       62 2024-04-09 02:01:41.000000 edman_web-2024.4.9/edman_web.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       32 2024-04-09 02:01:41.000000 edman_web-2024.4.9/edman_web.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1005 2024-04-09 01:59:51.000000 edman_web-2024.4.9/pyproject.toml
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 02:01:41.380567 edman_web-2024.4.9/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.370567 edman_web-2024.4.9/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    18418 2024-02-05 15:37:54.000000 edman_web-2024.4.9/tests/test_file_manager.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5897 2023-12-06 06:02:12.000000 edman_web-2024.4.9/tests/test_search_manager.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.370567 edman_web-2024.4.9/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 02:01:41.370567 edman_web-2024.4.9/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:43:44.000000 edman_web-2024.4.9/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 00:15:38.000000 edman_web-2024.4.9/venv/bin/rstpep2html.py
```

### Comparing `edman_web-2024.3.5/LICENSE.txt` & `edman_web-2024.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/PKG-INFO` & `edman_web-2024.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pymongo~=4.6.2
-Requires-Dist: edman~=2024.3.5
-Requires-Dist: Werkzeug~=3.0.1
-Requires-Dist: Pillow~=10.2.0
+Requires-Dist: edman~=2024.4.9
+Requires-Dist: Werkzeug~=3.0.2
+Requires-Dist: Pillow~=10.3.0
 
 edman_web
 =========
 
 |py_version|
 
 |  KEK IMSS SBRC/PF Experimental Data Management System.
```

### Comparing `edman_web-2024.3.5/README.rst` & `edman_web-2024.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/edman_web/file_manager.py` & `edman_web-2024.4.9/edman_web/file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/edman_web/search_manager.py` & `edman_web-2024.4.9/edman_web/search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/edman_web.egg-info/PKG-INFO` & `edman_web-2024.4.9/edman_web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_web
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: Sub-package of edman for web applications.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno, Yusuke Yamada
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,17 +19,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pymongo~=4.6.2
-Requires-Dist: edman~=2024.3.5
-Requires-Dist: Werkzeug~=3.0.1
-Requires-Dist: Pillow~=10.2.0
+Requires-Dist: edman~=2024.4.9
+Requires-Dist: Werkzeug~=3.0.2
+Requires-Dist: Pillow~=10.3.0
 
 edman_web
 =========
 
 |py_version|
 
 |  KEK IMSS SBRC/PF Experimental Data Management System.
```

### Comparing `edman_web-2024.3.5/edman_web.egg-info/SOURCES.txt` & `edman_web-2024.4.9/edman_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/pyproject.toml` & `edman_web-2024.4.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
     "pymongo~=4.6.2",
-    "edman~=2024.3.5",
-    "Werkzeug~=3.0.1",
-    "Pillow~=10.2.0"
+    "edman~=2024.4.9",
+    "Werkzeug~=3.0.2",
+    "Pillow~=10.3.0"
 ]
-version = "2024.3.5"
+version = "2024.4.9"
 
 [project.urls]
 "documentation" = "https://ryde.github.io/edman_web/"
 "repository" = "https://github.com/ryde/edman_web"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_web-2024.3.5/tests/test_file_manager.py` & `edman_web-2024.4.9/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/tests/test_search_manager.py` & `edman_web-2024.4.9/tests/test_search_manager.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/jp.py` & `edman_web-2024.4.9/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2html.py` & `edman_web-2024.4.9/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2html4.py` & `edman_web-2024.4.9/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2html5.py` & `edman_web-2024.4.9/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2latex.py` & `edman_web-2024.4.9/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2man.py` & `edman_web-2024.4.9/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2odt.py` & `edman_web-2024.4.9/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2odt_prepstyles.py` & `edman_web-2024.4.9/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2pseudoxml.py` & `edman_web-2024.4.9/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2s5.py` & `edman_web-2024.4.9/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2xetex.py` & `edman_web-2024.4.9/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rst2xml.py` & `edman_web-2024.4.9/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman_web-2024.3.5/venv/bin/rstpep2html.py` & `edman_web-2024.4.9/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

