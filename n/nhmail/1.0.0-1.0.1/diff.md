# Comparing `tmp/nhmail-1.0.0.tar.gz` & `tmp/nhmail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhmail-1.0.0.tar", last modified: Mon Apr  8 07:48:38 2024, max compression
+gzip compressed data, was "nhmail-1.0.1.tar", last modified: Mon Apr  8 07:54:56 2024, max compression
```

## Comparing `nhmail-1.0.0.tar` & `nhmail-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-08 07:48:38.880495 nhmail-1.0.0/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.0/LICENSE
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-08 07:48:38.880282 nhmail-1.0.0/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1098 2024-04-08 07:35:36.000000 nhmail-1.0.0/README.md
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-08 07:48:38.880026 nhmail-1.0.0/nhmail.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-08 07:48:38.000000 nhmail-1.0.0/nhmail.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      175 2024-04-08 07:48:38.000000 nhmail-1.0.0/nhmail.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-08 07:48:38.000000 nhmail-1.0.0/nhmail.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-08 07:48:38.000000 nhmail-1.0.0/nhmail.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-08 07:48:38.000000 nhmail-1.0.0/nhmail.egg-info/top_level.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-08 07:48:38.880547 nhmail-1.0.0/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      797 2024-04-08 07:46:27.000000 nhmail-1.0.0/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-08 07:54:56.819276 nhmail-1.0.1/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1062 2024-04-08 06:19:52.000000 nhmail-1.0.1/LICENSE
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-08 07:54:56.819073 nhmail-1.0.1/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1098 2024-04-08 07:35:36.000000 nhmail-1.0.1/README.md
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-08 07:54:56.818865 nhmail-1.0.1/nhmail.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      523 2024-04-08 07:54:56.000000 nhmail-1.0.1/nhmail.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      175 2024-04-08 07:54:56.000000 nhmail-1.0.1/nhmail.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-08 07:54:56.000000 nhmail-1.0.1/nhmail.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-08 07:54:56.000000 nhmail-1.0.1/nhmail.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)        1 2024-04-08 07:54:56.000000 nhmail-1.0.1/nhmail.egg-info/top_level.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-08 07:54:56.819329 nhmail-1.0.1/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      797 2024-04-08 07:54:49.000000 nhmail-1.0.1/setup.py
```

### Comparing `nhmail-1.0.0/LICENSE` & `nhmail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.0/PKG-INFO` & `nhmail-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.0/README.md` & `nhmail-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nhmail-1.0.0/nhmail.egg-info/PKG-INFO` & `nhmail-1.0.1/nhmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: email of nandh SDK for Python
 Home-page: https://github.com/ITNHL/nh-mail-sdk
 Author: it@nandhlogistics.vn
 Author-email: it@nandhlogistics.vn
 License: Version 1.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `nhmail-1.0.0/setup.py` & `nhmail-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 PKG = "nhmail"
-version = "1.0.0"
+version = "1.0.1"
 long_desc = (
     """This SDK is a programatic inteface into the mail APIs of NandH Logistics."""
 )
 
 setup(
     name=PKG,
     version=version,
```

