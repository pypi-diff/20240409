# Comparing `tmp/maitai_sdk_python-0.374.tar.gz` & `tmp/maitai_sdk_python-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai_sdk_python-0.374.tar", last modified: Tue Apr  9 05:16:09 2024, max compression
+gzip compressed data, was "maitai_sdk_python-0.4.tar", last modified: Tue Apr  9 05:23:28 2024, max compression
```

## Comparing `maitai_sdk_python-0.374.tar` & `maitai_sdk_python-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.439869 maitai_sdk_python-0.374/
--rw-rw-rw-   0        0        0      356 2024-04-09 05:16:09.438869 maitai_sdk_python-0.374/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai_sdk_python-0.374/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.411136 maitai_sdk_python-0.374/maitai/
--rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai_sdk_python-0.374/maitai/__init__.py
--rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai_sdk_python-0.374/maitai/_config.py
--rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai_sdk_python-0.374/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     7111 2024-04-09 05:13:46.000000 maitai_sdk_python-0.374/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai_sdk_python-0.374/maitai/_loadable.py
--rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai_sdk_python-0.374/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:16:09.436869 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      356 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-09 05:16:09.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 05:16:08.000000 maitai_sdk_python-0.374/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 05:16:09.440505 maitai_sdk_python-0.374/setup.cfg
--rw-rw-rw-   0        0        0      554 2024-04-09 05:14:38.000000 maitai_sdk_python-0.374/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:23:28.525563 maitai_sdk_python-0.4/
+-rw-rw-rw-   0        0        0      354 2024-04-09 05:23:28.523569 maitai_sdk_python-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai_sdk_python-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:23:28.502698 maitai_sdk_python-0.4/maitai/
+-rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai_sdk_python-0.4/maitai/__init__.py
+-rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai_sdk_python-0.4/maitai/_config.py
+-rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai_sdk_python-0.4/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0     7111 2024-04-09 05:13:46.000000 maitai_sdk_python-0.4/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai_sdk_python-0.4/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai_sdk_python-0.4/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:23:28.522568 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      354 2024-04-09 05:23:28.000000 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-09 05:23:28.000000 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:23:28.000000 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 05:23:28.000000 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 05:23:28.000000 maitai_sdk_python-0.4/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:23:28.525563 maitai_sdk_python-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      552 2024-04-09 05:23:15.000000 maitai_sdk_python-0.4/setup.py
```

### Comparing `maitai_sdk_python-0.374/README.md` & `maitai_sdk_python-0.4/README.md`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.374/maitai/_config.py` & `maitai_sdk_python-0.4/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.374/maitai/_eval_request.py` & `maitai_sdk_python-0.4/maitai/_eval_request.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.374/maitai/_evaluator.py` & `maitai_sdk_python-0.4/maitai/_evaluator.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.374/maitai/_loadable.py` & `maitai_sdk_python-0.4/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai_sdk_python-0.374/setup.py` & `maitai_sdk_python-0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai_sdk_python',
-    version='0.374',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     # Optional metadata
     author='Christian DalSanto',
     author_email='christian@yewpay.com',
```

