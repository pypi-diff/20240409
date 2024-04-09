# Comparing `tmp/dfp-0.9.0.tar.gz` & `tmp/dfp-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfp-0.9.0.tar", last modified: Tue Mar 28 07:57:52 2023, max compression
+gzip compressed data, was "dfp-0.9.1.tar", last modified: Tue Apr  9 09:28:52 2024, max compression
```

## Comparing `dfp-0.9.0.tar` & `dfp-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2023-03-28 07:57:51.993304 dfp-0.9.0/
--rw-r--r--   0 jay       (1000) jay       (1000)    35149 2023-01-18 14:18:16.000000 dfp-0.9.0/LICENSE
--rw-r--r--   0 jay       (1000) jay       (1000)     1114 2023-03-28 07:57:51.997304 dfp-0.9.0/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)      847 2023-03-02 14:17:49.000000 dfp-0.9.0/README.md
--rw-r--r--   0 jay       (1000) jay       (1000)       87 2023-01-18 15:30:11.000000 dfp-0.9.0/pyproject.toml
--rw-r--r--   0 jay       (1000) jay       (1000)      465 2023-03-28 07:57:51.997304 dfp-0.9.0/setup.cfg
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2023-03-28 07:57:51.981304 dfp-0.9.0/src/
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2023-03-28 07:57:51.989304 dfp-0.9.0/src/dfp.egg-info/
--rw-r--r--   0 jay       (1000) jay       (1000)     1114 2023-03-28 07:57:51.000000 dfp-0.9.0/src/dfp.egg-info/PKG-INFO
--rw-r--r--   0 jay       (1000) jay       (1000)      225 2023-03-28 07:57:51.000000 dfp-0.9.0/src/dfp.egg-info/SOURCES.txt
--rw-r--r--   0 jay       (1000) jay       (1000)        1 2023-03-28 07:57:51.000000 dfp-0.9.0/src/dfp.egg-info/dependency_links.txt
--rw-r--r--   0 jay       (1000) jay       (1000)       23 2023-03-28 07:57:51.000000 dfp-0.9.0/src/dfp.egg-info/requires.txt
--rw-r--r--   0 jay       (1000) jay       (1000)        4 2023-03-28 07:57:51.000000 dfp-0.9.0/src/dfp.egg-info/top_level.txt
--rw-r--r--   0 jay       (1000) jay       (1000)    42375 2023-03-28 07:57:05.000000 dfp-0.9.0/src/dfp.py
-drwxr-xr-x   0 jay       (1000) jay       (1000)        0 2023-03-28 07:57:51.993304 dfp-0.9.0/tests/
--rw-r--r--   0 jay       (1000) jay       (1000)     7612 2023-03-28 07:56:31.000000 dfp-0.9.0/tests/test_dfp.py
+drwxr-xr-x   0 jaymorgan  (1001) jaymorgan  (1001)        0 2024-04-09 09:28:52.245476 dfp-0.9.1/
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)    35149 2024-04-09 09:21:45.000000 dfp-0.9.1/LICENSE
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)     1167 2024-04-09 09:28:52.245476 dfp-0.9.1/PKG-INFO
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)      847 2024-04-09 09:21:45.000000 dfp-0.9.1/README.md
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)       87 2024-04-09 09:21:45.000000 dfp-0.9.1/pyproject.toml
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)      465 2024-04-09 09:28:52.246476 dfp-0.9.1/setup.cfg
+drwxr-xr-x   0 jaymorgan  (1001) jaymorgan  (1001)        0 2024-04-09 09:28:52.244476 dfp-0.9.1/src/
+drwxr-xr-x   0 jaymorgan  (1001) jaymorgan  (1001)        0 2024-04-09 09:28:52.245476 dfp-0.9.1/src/dfp.egg-info/
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)     1167 2024-04-09 09:28:52.000000 dfp-0.9.1/src/dfp.egg-info/PKG-INFO
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)      225 2024-04-09 09:28:52.000000 dfp-0.9.1/src/dfp.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)        1 2024-04-09 09:28:52.000000 dfp-0.9.1/src/dfp.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)       23 2024-04-09 09:28:52.000000 dfp-0.9.1/src/dfp.egg-info/requires.txt
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)        4 2024-04-09 09:28:52.000000 dfp-0.9.1/src/dfp.egg-info/top_level.txt
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)    42490 2024-04-09 09:23:16.000000 dfp-0.9.1/src/dfp.py
+drwxr-xr-x   0 jaymorgan  (1001) jaymorgan  (1001)        0 2024-04-09 09:28:52.245476 dfp-0.9.1/tests/
+-rw-r--r--   0 jaymorgan  (1001) jaymorgan  (1001)     7843 2024-04-09 09:28:47.000000 dfp-0.9.1/tests/test_dfp.py
```

### Comparing `dfp-0.9.0/LICENSE` & `dfp-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dfp-0.9.0/PKG-INFO` & `dfp-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dfp
-Version: 0.9.0
+Version: 0.9.1
 Summary: A suite of functional tools for all your functional programming
 Home-page: https://github.com/jaypmorgan/dfp
 Author: Jay Morgan
 Author-email: jay@morganwastaken.com
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: tqdm>=4.62
+Requires-Dist: pandas==1.*
 
 # DFP: Dogmatic Functional Programming
 
 [![Documentation Status](https://readthedocs.org/projects/dogmatic-functional-programming/badge/?version=latest)](https://dogmatic-functional-programming.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/jaypmorgan/dfp/badge.svg?branch=main)](https://coveralls.io/github/jaypmorgan/dfp?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/dfp?label=dfp)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/dfp)
```

### Comparing `dfp-0.9.0/README.md` & `dfp-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dfp-0.9.0/src/dfp.egg-info/PKG-INFO` & `dfp-0.9.1/src/dfp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: dfp
-Version: 0.9.0
+Version: 0.9.1
 Summary: A suite of functional tools for all your functional programming
 Home-page: https://github.com/jaypmorgan/dfp
 Author: Jay Morgan
 Author-email: jay@morganwastaken.com
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: tqdm>=4.62
+Requires-Dist: pandas==1.*
 
 # DFP: Dogmatic Functional Programming
 
 [![Documentation Status](https://readthedocs.org/projects/dogmatic-functional-programming/badge/?version=latest)](https://dogmatic-functional-programming.readthedocs.io/en/latest/?badge=latest)
 [![Coverage Status](https://coveralls.io/repos/github/jaypmorgan/dfp/badge.svg?branch=main)](https://coveralls.io/github/jaypmorgan/dfp?branch=main)
 ![PyPI](https://img.shields.io/pypi/v/dfp?label=dfp)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/dfp)
```

### Comparing `dfp-0.9.0/src/dfp.py` & `dfp-0.9.1/src/dfp.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,14 +363,17 @@
 
         >>> from dfp import lmap
         >>> lmap(lambda x: x*2, range(5))
         [0, 2, 4, 6, 8]
 
     See `tmap` for more examples.
     """
+    if isinstance(lst, pd.Series):
+        # pandas series should be iterable over rows
+        lst = lst.tolist()
     return list(tmap(f, lst, parallel, p_workers, p_type, progress, progress_fn))
 
 
 @transducer
 def tmap(
         f: Callable,
         lst: Optional[Iterable] = None,
```

### Comparing `dfp-0.9.0/tests/test_dfp.py` & `dfp-0.9.1/tests/test_dfp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import unittest
 
+import pandas as pd
+
 from src import dfp
 
 
 class DFPTests(unittest.TestCase):
 
     def test_find(self):
         test_list = ['a', 'b', 'c', 'd']
@@ -52,14 +54,19 @@
         self.assertEqual(len(out), 10_000)
         self.assertEqual(out[-1], 9999**2)
         out = dfp.lmap(lambda x: x**2, map(lambda x: x, range(10_000)), parallel=False, progress=True)
         self.assertEqual(out[0], 0)
         self.assertEqual(len(out), 10_000)
         self.assertEqual(out[-1], 9999**2)
 
+        # check that lmap works as intended on Pandas Series
+        df = pd.DataFrame({'a': range(10), 'b': range(10)})
+        out = dfp.lmap(lambda x: x**2, df['b'])
+        self.assertEqual(out, [x**2 for x in range(10)])
+
     def test_lzip(self):
         out = dfp.lzip(dfp.tfilter(lambda i: i % 2 == 0, range(10)), dfp.tfilter(lambda i: i % 2 != 0, range(10)))
         self.assertEqual(out[0][0], 0)
         self.assertEqual(out[0][1], 1)
         self.assertEqual(out[1][0], 2)
         self.assertEqual(len(out), 5)
 
@@ -185,12 +192,11 @@
     def test_port_json(self):
         content = [["this is a test", "this is another line"]]
         filepath = dfp.port_json("/tmp/filename.json", content)
         self.assertEqual(filepath, "/tmp/filename.json")
         out_content = dfp.port_json(filepath)
         self.assertEqual(out_content[0][0], "this is a test")
         self.assertEqual(out_content[0][1], "this is another line")
-        
-        
+
 
 if __name__ == '__main__':
     unittest.main()
```

