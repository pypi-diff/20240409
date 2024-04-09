# Comparing `tmp/arvados-cwl-runner-2.7.1.tar.gz` & `tmp/arvados-cwl-runner-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.7.1.tar", last modified: Tue Dec 12 20:51:57 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.7.2.tar", last modified: Tue Apr  9 20:11:28 2024, max compression
```

## Comparing `arvados-cwl-runner-2.7.1.tar` & `arvados-cwl-runner-2.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21372 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-12-12 20:51:56.000000 arvados-cwl-runner-2.7.1/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13323 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35717 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5794 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34462 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2260 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3935 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    45214 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18053 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    40584 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      213 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2140 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:57.000000 arvados-cwl-runner-2.7.1/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73538 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87248 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-12-12 20:51:23.000000 arvados-cwl-runner-2.7.1/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21372 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14533 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13027 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13514 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35935 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5794 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34462 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2260 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3935 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    45214 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18053 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    40584 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      213 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2140 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:28.000000 arvados-cwl-runner-2.7.2/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73538 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87248 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2024-04-09 20:11:07.000000 arvados-cwl-runner-2.7.2/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.7.1/LICENSE-2.0.txt` & `arvados-cwl-runner-2.7.2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/PKG-INFO` & `arvados-cwl-runner-2.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files 2% similar despite different names*

```diff
@@ -474,12 +474,17 @@
     - name: memoryErrorRegex
       type: string?
       doc: |
         A regular expression that will be used on the text of stdout
         and stderr produced by the tool to determine if a failed job
         should be retried with more RAM.  By default, searches for the
         substrings 'bad_alloc' and 'OutOfMemory'.
-    - name: memoryRetryMultipler
-      type: float
+    - name: memoryRetryMultiplier
+      type: float?
       doc: |
         If the container failed on its first run, re-submit the
         container with the RAM request multiplied by this factor.
+    - name: memoryRetryMultipler
+      type: float?
+      doc: |
+        Deprecated misspelling of "memoryRetryMultiplier".  Kept only
+        for backwards compatability, don't use this.
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files 3% similar despite different names*

```diff
@@ -417,12 +417,17 @@
     - name: memoryErrorRegex
       type: string?
       doc: |
         A regular expression that will be used on the text of stdout
         and stderr produced by the tool to determine if a failed job
         should be retried with more RAM.  By default, searches for the
         substrings 'bad_alloc' and 'OutOfMemory'.
-    - name: memoryRetryMultipler
-      type: float
+    - name: memoryRetryMultiplier
+      type: float?
       doc: |
         If the container failed on its first run, re-submit the
         container with the RAM request multiplied by this factor.
+    - name: memoryRetryMultipler
+      type: float?
+      doc: |
+        Deprecated misspelling of "memoryRetryMultiplier".  Kept only
+        for backwards compatability, don't use this.
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.7.2/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files 2% similar despite different names*

```diff
@@ -420,19 +420,25 @@
     - name: memoryErrorRegex
       type: string?
       doc: |
         A regular expression that will be used on the text of stdout
         and stderr produced by the tool to determine if a failed job
         should be retried with more RAM.  By default, searches for the
         substrings 'bad_alloc' and 'OutOfMemory'.
-    - name: memoryRetryMultipler
-      type: float
+    - name: memoryRetryMultiplier
+      type: float?
       doc: |
         If the container failed on its first run, re-submit the
         container with the RAM request multiplied by this factor.
+    - name: memoryRetryMultipler
+      type: float?
+      doc: |
+        Deprecated misspelling of "memoryRetryMultiplier".  Kept only
+        for backwards compatability, don't use this.
+
 
 - name: SeparateRunner
   type: record
   extends: cwl:ProcessRequirement
   inVocab: false
   doc: |
     Indicates that a subworkflow should run in a separate
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/arvcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,16 +366,21 @@
             else:
                 logger.warning("%s API revision is %s, revision %s is required to support setting properties on output collections.",
                                self.arvrunner.label(self), self.arvrunner.api._rootDesc["revision"], "20220510")
 
         ram_multiplier = [1]
 
         oom_retry_req, _ = self.get_requirement("http://arvados.org/cwl#OutOfMemoryRetry")
-        if oom_retry_req and oom_retry_req.get('memoryRetryMultipler'):
-            ram_multiplier.append(oom_retry_req.get('memoryRetryMultipler'))
+        if oom_retry_req:
+            if oom_retry_req.get('memoryRetryMultiplier'):
+                ram_multiplier.append(oom_retry_req.get('memoryRetryMultiplier'))
+            elif oom_retry_req.get('memoryRetryMultipler'):
+                ram_multiplier.append(oom_retry_req.get('memoryRetryMultipler'))
+            else:
+                ram_multiplier.append(2)
 
         if runtimeContext.runnerjob.startswith("arvwf:"):
             wfuuid = runtimeContext.runnerjob[6:runtimeContext.runnerjob.index("#")]
             wfrecord = self.arvrunner.api.workflows().get(uuid=wfuuid).execute(num_retries=self.arvrunner.num_retries)
             if container_request["name"] == "main":
                 container_request["name"] = wfrecord["name"]
             container_request["properties"]["template_uuid"] = wfuuid
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/context.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/done.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/done.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/executor.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/executor.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/perf.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/runner.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/runner.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl/util.py` & `arvados-cwl-runner-2.7.2/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.7.1/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.7.2/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/arvados_version.py` & `arvados-cwl-runner-2.7.2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/setup.py` & `arvados-cwl-runner-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/matcher.py` & `arvados-cwl-runner-2.7.2/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_container.py` & `arvados-cwl-runner-2.7.2/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_copy_deps.py` & `arvados-cwl-runner-2.7.2/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_fsaccess.py` & `arvados-cwl-runner-2.7.2/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_make_output.py` & `arvados-cwl-runner-2.7.2/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_pathmapper.py` & `arvados-cwl-runner-2.7.2/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.7.2/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_submit.py` & `arvados-cwl-runner-2.7.2/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_tq.py` & `arvados-cwl-runner-2.7.2/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_urljoin.py` & `arvados-cwl-runner-2.7.2/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.7.1/tests/test_util.py` & `arvados-cwl-runner-2.7.2/tests/test_util.py`

 * *Files identical despite different names*

