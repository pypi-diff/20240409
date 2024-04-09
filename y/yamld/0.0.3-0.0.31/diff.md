# Comparing `tmp/yamld-0.0.3.tar.gz` & `tmp/yamld-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamld-0.0.3.tar", last modified: Mon Apr  8 16:53:23 2024, max compression
+gzip compressed data, was "yamld-0.0.31.tar", last modified: Tue Apr  9 05:31:22 2024, max compression
```

## Comparing `yamld-0.0.3.tar` & `yamld-0.0.31.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/
--rw-r--r--   0 hunter    (1000) hunter    (1000)      395 2024-04-08 16:53:23.101043 yamld-0.0.3/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2187 2024-04-08 16:48:54.000000 yamld-0.0.3/README.md
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/bin/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3233 2024-04-08 11:42:17.000000 yamld-0.0.3/bin/csv2yamld
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2202 2024-04-08 11:48:25.000000 yamld-0.0.3/bin/yamld
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1659 2024-04-08 11:08:12.000000 yamld-0.0.3/bin/yamld2csv
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2024-04-08 16:53:23.101043 yamld-0.0.3/setup.cfg
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      652 2024-04-08 16:51:00.000000 yamld-0.0.3/setup.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/tests/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1077 2024-04-06 15:40:32.000000 yamld-0.0.3/tests/test_basic_parse_test.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/yamld/
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      534 2024-04-06 19:00:33.000000 yamld-0.0.3/yamld/__init__.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      332 2024-04-08 11:36:44.000000 yamld-0.0.3/yamld/common.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     3394 2024-04-08 14:47:35.000000 yamld-0.0.3/yamld/parser.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1814 2024-04-08 14:49:37.000000 yamld-0.0.3/yamld/with_iofile.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     1433 2024-04-08 14:40:39.000000 yamld-0.0.3/yamld/with_pandas.py
--rw-rw-r--   0 hunter    (1000) hunter    (1000)     2660 2024-04-08 11:28:42.000000 yamld-0.0.3/yamld/writer.py
-drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-08 16:53:23.101043 yamld-0.0.3/yamld.egg-info/
--rw-r--r--   0 hunter    (1000) hunter    (1000)      395 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/PKG-INFO
--rw-rw-r--   0 hunter    (1000) hunter    (1000)      339 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/SOURCES.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/dependency_links.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)       14 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/requires.txt
--rw-rw-r--   0 hunter    (1000) hunter    (1000)        6 2024-04-08 16:53:23.000000 yamld-0.0.3/yamld.egg-info/top_level.txt
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-09 05:31:22.554049 yamld-0.0.31/
+-rw-r--r--   0 hunter    (1000) hunter    (1000)      396 2024-04-09 05:31:22.554049 yamld-0.0.31/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2187 2024-04-08 16:48:54.000000 yamld-0.0.31/README.md
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-09 05:31:22.554049 yamld-0.0.31/bin/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3233 2024-04-08 11:42:17.000000 yamld-0.0.31/bin/csv2yamld
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2202 2024-04-08 11:48:25.000000 yamld-0.0.31/bin/yamld
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1659 2024-04-08 11:08:12.000000 yamld-0.0.31/bin/yamld2csv
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       38 2024-04-09 05:31:22.554049 yamld-0.0.31/setup.cfg
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      653 2024-04-09 05:31:10.000000 yamld-0.0.31/setup.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-09 05:31:22.554049 yamld-0.0.31/tests/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1077 2024-04-06 15:40:32.000000 yamld-0.0.31/tests/test_basic_parse_test.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-09 05:31:22.554049 yamld-0.0.31/yamld/
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      534 2024-04-06 19:00:33.000000 yamld-0.0.31/yamld/__init__.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      332 2024-04-08 11:36:44.000000 yamld-0.0.31/yamld/common.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     3394 2024-04-08 14:47:35.000000 yamld-0.0.31/yamld/parser.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1814 2024-04-08 14:49:37.000000 yamld-0.0.31/yamld/with_iofile.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     1433 2024-04-08 14:40:39.000000 yamld-0.0.31/yamld/with_pandas.py
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)     2660 2024-04-08 11:28:42.000000 yamld-0.0.31/yamld/writer.py
+drwxrwxr-x   0 hunter    (1000) hunter    (1000)        0 2024-04-09 05:31:22.554049 yamld-0.0.31/yamld.egg-info/
+-rw-r--r--   0 hunter    (1000) hunter    (1000)      396 2024-04-09 05:31:22.000000 yamld-0.0.31/yamld.egg-info/PKG-INFO
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)      339 2024-04-09 05:31:22.000000 yamld-0.0.31/yamld.egg-info/SOURCES.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        1 2024-04-09 05:31:22.000000 yamld-0.0.31/yamld.egg-info/dependency_links.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)       14 2024-04-09 05:31:22.000000 yamld-0.0.31/yamld.egg-info/requires.txt
+-rw-rw-r--   0 hunter    (1000) hunter    (1000)        6 2024-04-09 05:31:22.000000 yamld-0.0.31/yamld.egg-info/top_level.txt
```

### Comparing `yamld-0.0.3/README.md` & `yamld-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/bin/csv2yamld` & `yamld-0.0.31/bin/csv2yamld`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/bin/yamld` & `yamld-0.0.31/bin/yamld`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/bin/yamld2csv` & `yamld-0.0.31/bin/yamld2csv`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/setup.py` & `yamld-0.0.31/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='yamld',
-    version='0.0.3',
+    version='0.0.31',
     author='Yahya Badran',
     author_email='techtweaking@gmail.com',
     description='parser of YAMLd, a tiny subset of YAML',
     url='https://github.com/badranx/yaml-datasets',
     install_requires=['pandas >= 1.0.0'],
     packages = [package for package in find_packages() if package.startswith("yamld")],
     scripts=['bin/csv2yamld', 'bin/yamld2csv', 'bin/yamld'],
```

### Comparing `yamld-0.0.3/tests/test_basic_parse_test.py` & `yamld-0.0.31/tests/test_basic_parse_test.py`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/yamld/__init__.py` & `yamld-0.0.31/yamld/__init__.py`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/yamld/parser.py` & `yamld-0.0.31/yamld/parser.py`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/yamld/with_iofile.py` & `yamld-0.0.31/yamld/with_iofile.py`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/yamld/with_pandas.py` & `yamld-0.0.31/yamld/with_pandas.py`

 * *Files identical despite different names*

### Comparing `yamld-0.0.3/yamld/writer.py` & `yamld-0.0.31/yamld/writer.py`

 * *Files identical despite different names*

