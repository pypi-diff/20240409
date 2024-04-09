# Comparing `tmp/resamp-1.6.2.tar.gz` & `tmp/resamp-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resamp-1.6.2.tar", last modified: Sun Mar 10 04:17:18 2024, max compression
+gzip compressed data, was "resamp-1.6.3.tar", last modified: Tue Apr  9 20:04:19 2024, max compression
```

## Comparing `resamp-1.6.2.tar` & `resamp-1.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:17:18.704607 resamp-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-10 04:17:13.000000 resamp-1.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-03-10 04:17:18.704607 resamp-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-03-10 04:17:13.000000 resamp-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:17:18.704607 resamp-1.6.2/resamp/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-10 04:17:13.000000 resamp-1.6.2/resamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32392 2024-03-10 04:17:13.000000 resamp-1.6.2/resamp/resamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 04:17:18.704607 resamp-1.6.2/resamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-03-10 04:17:18.000000 resamp-1.6.2/resamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-10 04:17:18.000000 resamp-1.6.2/resamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 04:17:18.000000 resamp-1.6.2/resamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-10 04:17:18.000000 resamp-1.6.2/resamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-10 04:17:18.000000 resamp-1.6.2/resamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 04:17:18.704607 resamp-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-10 04:17:13.000000 resamp-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.530227 resamp-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 20:04:15.000000 resamp-1.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:04:19.530227 resamp-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18721 2024-04-09 20:04:15.000000 resamp-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.526227 resamp-1.6.3/resamp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-09 20:04:15.000000 resamp-1.6.3/resamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32392 2024-04-09 20:04:15.000000 resamp-1.6.3/resamp/resamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:04:19.530227 resamp-1.6.3/resamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:04:19.000000 resamp-1.6.3/resamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:04:19.530227 resamp-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 20:04:15.000000 resamp-1.6.3/setup.py
```

### Comparing `resamp-1.6.2/LICENSE` & `resamp-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resamp-1.6.2/resamp/__init__.py` & `resamp-1.6.3/resamp/__init__.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.2/resamp/resamp.py` & `resamp-1.6.3/resamp/resamp.py`

 * *Files identical despite different names*

### Comparing `resamp-1.6.2/setup.py` & `resamp-1.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='resamp',
-    version='1.6.2',
+    version='1.6.3',
     author='Vishanth Hari Raj Balasubramanian',
     author_email='rbvish1007@gmail.com',
     description='A custom statistics library/ resampling technqiues for chi-abs, boostrapting analysis and other statistical functions.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vishanth10/resamp.git',
     packages=find_packages(),
```

