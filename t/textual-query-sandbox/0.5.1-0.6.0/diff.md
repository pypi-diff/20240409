# Comparing `tmp/textual-query-sandbox-0.5.1.tar.gz` & `tmp/textual-query-sandbox-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-query-sandbox-0.5.1.tar", last modified: Tue Apr  9 08:02:33 2024, max compression
+gzip compressed data, was "textual-query-sandbox-0.6.0.tar", last modified: Tue Apr  9 08:08:00 2024, max compression
```

## Comparing `textual-query-sandbox-0.5.1.tar` & `textual-query-sandbox-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:02:33.958039 textual-query-sandbox-0.5.1/
--rw-r--r--   0 davep      (501) staff       (20)     1815 2024-04-09 08:02:33.957973 textual-query-sandbox-0.5.1/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      521 2023-08-31 21:16:50.000000 textual-query-sandbox-0.5.1/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-09-02 06:45:41.000000 textual-query-sandbox-0.5.1/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1469 2024-04-09 08:02:33.958327 textual-query-sandbox-0.5.1/setup.cfg
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:02:33.956751 textual-query-sandbox-0.5.1/textual_query_sandbox/
--rw-r--r--   0 davep      (501) staff       (20)      401 2023-09-20 20:06:42.000000 textual-query-sandbox-0.5.1/textual_query_sandbox/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      228 2023-09-03 08:17:12.000000 textual-query-sandbox-0.5.1/textual_query_sandbox/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)     7475 2023-09-10 07:54:32.000000 textual-query-sandbox-0.5.1/textual_query_sandbox/sandbox.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:02:33.957705 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     1815 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      407 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       59 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       16 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-09 08:02:33.000000 textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:08:00.663429 textual-query-sandbox-0.6.0/
+-rw-r--r--   0 davep      (501) staff       (20)     1815 2024-04-09 08:08:00.663376 textual-query-sandbox-0.6.0/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      521 2023-08-31 21:16:50.000000 textual-query-sandbox-0.6.0/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-09-02 06:45:41.000000 textual-query-sandbox-0.6.0/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1469 2024-04-09 08:08:00.663689 textual-query-sandbox-0.6.0/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:08:00.662256 textual-query-sandbox-0.6.0/textual_query_sandbox/
+-rw-r--r--   0 davep      (501) staff       (20)      406 2024-04-09 08:07:44.000000 textual-query-sandbox-0.6.0/textual_query_sandbox/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      228 2023-09-03 08:17:12.000000 textual-query-sandbox-0.6.0/textual_query_sandbox/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)     7475 2023-09-10 07:54:32.000000 textual-query-sandbox-0.6.0/textual_query_sandbox/sandbox.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-09 08:08:00.663174 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     1815 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      407 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       59 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       16 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       22 2024-04-09 08:08:00.000000 textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/top_level.txt
```

### Comparing `textual-query-sandbox-0.5.1/PKG-INFO` & `textual-query-sandbox-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-query-sandbox
-Version: 0.5.1
+Version: 0.6.0
 Summary: A sandbox for practicing Textual queries
 Home-page: https://github.com/davep/textual-query-sandbox
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `textual-query-sandbox-0.5.1/README.md` & `textual-query-sandbox-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `textual-query-sandbox-0.5.1/setup.cfg` & `textual-query-sandbox-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `textual-query-sandbox-0.5.1/textual_query_sandbox/sandbox.py` & `textual-query-sandbox-0.6.0/textual_query_sandbox/sandbox.py`

 * *Files identical despite different names*

### Comparing `textual-query-sandbox-0.5.1/textual_query_sandbox.egg-info/PKG-INFO` & `textual-query-sandbox-0.6.0/textual_query_sandbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-query-sandbox
-Version: 0.5.1
+Version: 0.6.0
 Summary: A sandbox for practicing Textual queries
 Home-page: https://github.com/davep/textual-query-sandbox
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

