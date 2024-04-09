# Comparing `tmp/ts-soup-0.1.0.tar.gz` & `tmp/ts-soup-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-gejmd28n\ts-soup-0.1.0.tar", last modified: Tue Apr  9 03:14:10 2024, max compression
+gzip compressed data, was "D:\PythonProjects\GDtrading\ts-soup\dist\.tmp-7t86jf1n\ts-soup-0.1.1.tar", last modified: Tue Apr  9 03:17:47 2024, max compression
```

## Comparing `ts-soup-0.1.0.tar` & `ts-soup-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.901619 ts-soup-0.1.0/
--rw-rw-rw-   0        0        0     1028 2024-04-09 03:14:10.900617 ts-soup-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 03:14:10.901619 ts-soup-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-09 03:12:51.000000 ts-soup-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.887588 ts-soup-0.1.0/ts_soup/
--rw-rw-rw-   0        0        0      411 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/app.py
--rw-rw-rw-   0        0        0    15530 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/common.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.896665 ts-soup-0.1.0/ts_soup/workers/
--rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/workers/__init__.py
--rw-rw-rw-   0        0        0     3689 2024-04-07 01:22:11.000000 ts-soup-0.1.0/ts_soup/workers/sources.py
--rw-rw-rw-   0        0        0     3955 2024-04-09 03:12:17.000000 ts-soup-0.1.0/ts_soup/workers/targets.py
-drwxrwxrwx   0        0        0        0 2024-04-09 03:14:10.899116 ts-soup-0.1.0/ts_soup.egg-info/
--rw-rw-rw-   0        0        0     1028 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 03:14:10.000000 ts-soup-0.1.0/ts_soup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:47.829576 ts-soup-0.1.1/
+-rw-rw-rw-   0        0        0     1028 2024-04-09 03:17:47.827575 ts-soup-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-04-07 01:22:11.000000 ts-soup-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 03:17:47.829576 ts-soup-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-09 03:17:31.000000 ts-soup-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:47.815590 ts-soup-0.1.1/ts_soup/
+-rw-rw-rw-   0        0        0      373 2024-04-09 03:17:12.000000 ts-soup-0.1.1/ts_soup/__init__.py
+-rw-rw-rw-   0        0        0     1418 2024-04-07 01:22:11.000000 ts-soup-0.1.1/ts_soup/app.py
+-rw-rw-rw-   0        0        0    15530 2024-04-09 03:12:17.000000 ts-soup-0.1.1/ts_soup/common.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:47.825574 ts-soup-0.1.1/ts_soup/workers/
+-rw-rw-rw-   0        0        0       78 2024-04-07 01:22:11.000000 ts-soup-0.1.1/ts_soup/workers/__init__.py
+-rw-rw-rw-   0        0        0     3689 2024-04-07 01:22:11.000000 ts-soup-0.1.1/ts_soup/workers/sources.py
+-rw-rw-rw-   0        0        0     3955 2024-04-09 03:12:17.000000 ts-soup-0.1.1/ts_soup/workers/targets.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:17:47.826575 ts-soup-0.1.1/ts_soup.egg-info/
+-rw-rw-rw-   0        0        0     1028 2024-04-09 03:17:47.000000 ts-soup-0.1.1/ts_soup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-09 03:17:47.000000 ts-soup-0.1.1/ts_soup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:17:47.000000 ts-soup-0.1.1/ts_soup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 03:17:47.000000 ts-soup-0.1.1/ts_soup.egg-info/top_level.txt
```

### Comparing `ts-soup-0.1.0/PKG-INFO` & `ts-soup-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.0
+Version: 0.1.1
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ts-soup-0.1.0/README.md` & `ts-soup-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.0/setup.py` & `ts-soup-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='utf8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="ts-soup",
-  version="0.1.0",
+  version="0.1.1",
   author="feihan ye",
   author_email="445280206@qq.com",
   description="date series data synchronization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   # url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `ts-soup-0.1.0/ts_soup/app.py` & `ts-soup-0.1.1/ts_soup/app.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.0/ts_soup/common.py` & `ts-soup-0.1.1/ts_soup/common.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.0/ts_soup/workers/sources.py` & `ts-soup-0.1.1/ts_soup/workers/sources.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.0/ts_soup/workers/targets.py` & `ts-soup-0.1.1/ts_soup/workers/targets.py`

 * *Files identical despite different names*

### Comparing `ts-soup-0.1.0/ts_soup.egg-info/PKG-INFO` & `ts-soup-0.1.1/ts_soup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-soup
-Version: 0.1.0
+Version: 0.1.1
 Summary: date series data synchronization
 Author: feihan ye
 Author-email: 445280206@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

