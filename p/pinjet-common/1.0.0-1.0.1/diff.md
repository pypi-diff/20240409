# Comparing `tmp/pinjet-common-1.0.0.tar.gz` & `tmp/pinjet-common-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinjet-common-1.0.0.tar", last modified: Sun Apr  7 12:00:25 2024, max compression
+gzip compressed data, was "dist/pinjet-common-1.0.1.tar", last modified: Tue Apr  9 09:09:37 2024, max compression
```

## Comparing `pinjet-common-1.0.0.tar` & `pinjet-common-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/
--rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-1.0.0/LICENSE
--rw-r--r--   0 abetrack3   (501) staff       (20)      222 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-1.0.0/README.md
--rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/setup.cfg
--rw-r--r--   0 abetrack3   (501) staff       (20)      474 2024-04-07 11:58:53.000000 pinjet-common-1.0.0/setup.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-1.0.0/src/pinjet/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet/common/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-1.0.0/src/pinjet/common/__init__.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet/common/constants/
--rw-r--r--   0 abetrack3   (501) staff       (20)       46 2024-04-07 10:23:16.000000 pinjet-common-1.0.0/src/pinjet/common/constants/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-1.0.0/src/pinjet/common/constants/constants.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet/common/constants/io/
--rw-r--r--   0 abetrack3   (501) staff       (20)       86 2024-04-07 10:23:16.000000 pinjet-common-1.0.0/src/pinjet/common/constants/io/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)      279 2024-04-01 16:55:14.000000 pinjet-common-1.0.0/src/pinjet/common/constants/io/io.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet/common/decorators/
--rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-07 10:48:27.000000 pinjet-common-1.0.0/src/pinjet/common/decorators/__init__.py
--rw-r--r--   0 abetrack3   (501) staff       (20)     1186 2024-04-07 10:52:43.000000 pinjet-common-1.0.0/src/pinjet/common/decorators/function_timer.py
--rw-r--r--   0 abetrack3   (501) staff       (20)     1198 2024-04-07 11:38:08.000000 pinjet-common-1.0.0/src/pinjet/common/decorators/retry_on_exception.py
-drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/
--rw-r--r--   0 abetrack3   (501) staff       (20)      222 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/PKG-INFO
--rw-r--r--   0 abetrack3   (501) staff       (20)      583 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/SOURCES.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/dependency_links.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        8 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/requires.txt
--rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-07 12:00:25.000000 pinjet-common-1.0.0/src/pinjet_common.egg-info/top_level.txt
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/
+-rw-r--r--   0 abetrack3   (501) staff       (20)     1077 2024-04-01 16:41:11.000000 pinjet-common-1.0.1/LICENSE
+-rw-r--r--   0 abetrack3   (501) staff       (20)      222 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)       15 2024-04-01 16:41:11.000000 pinjet-common-1.0.1/README.md
+-rw-r--r--   0 abetrack3   (501) staff       (20)       38 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/setup.cfg
+-rw-r--r--   0 abetrack3   (501) staff       (20)      474 2024-04-09 09:09:36.000000 pinjet-common-1.0.1/setup.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-1.0.1/src/pinjet/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet/common/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-01 18:28:37.000000 pinjet-common-1.0.1/src/pinjet/common/__init__.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet/common/constants/
+-rw-r--r--   0 abetrack3   (501) staff       (20)       46 2024-04-07 10:23:16.000000 pinjet-common-1.0.1/src/pinjet/common/constants/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      425 2024-04-01 16:50:16.000000 pinjet-common-1.0.1/src/pinjet/common/constants/constants.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet/common/constants/io/
+-rw-r--r--   0 abetrack3   (501) staff       (20)       86 2024-04-07 10:23:16.000000 pinjet-common-1.0.1/src/pinjet/common/constants/io/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)      579 2024-04-09 09:08:44.000000 pinjet-common-1.0.1/src/pinjet/common/constants/io/io.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet/common/decorators/
+-rw-r--r--   0 abetrack3   (501) staff       (20)        0 2024-04-07 10:48:27.000000 pinjet-common-1.0.1/src/pinjet/common/decorators/__init__.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)     1186 2024-04-07 10:52:43.000000 pinjet-common-1.0.1/src/pinjet/common/decorators/function_timer.py
+-rw-r--r--   0 abetrack3   (501) staff       (20)     1198 2024-04-07 11:38:08.000000 pinjet-common-1.0.1/src/pinjet/common/decorators/retry_on_exception.py
+drwxr-xr-x   0 abetrack3   (501) staff       (20)        0 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/
+-rw-r--r--   0 abetrack3   (501) staff       (20)      222 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/PKG-INFO
+-rw-r--r--   0 abetrack3   (501) staff       (20)      583 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/SOURCES.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        1 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/dependency_links.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        8 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/requires.txt
+-rw-r--r--   0 abetrack3   (501) staff       (20)        7 2024-04-09 09:09:37.000000 pinjet-common-1.0.1/src/pinjet_common.egg-info/top_level.txt
```

### Comparing `pinjet-common-1.0.0/LICENSE` & `pinjet-common-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjet-common-1.0.0/src/pinjet/common/decorators/function_timer.py` & `pinjet-common-1.0.1/src/pinjet/common/decorators/function_timer.py`

 * *Files identical despite different names*

### Comparing `pinjet-common-1.0.0/src/pinjet/common/decorators/retry_on_exception.py` & `pinjet-common-1.0.1/src/pinjet/common/decorators/retry_on_exception.py`

 * *Files identical despite different names*

### Comparing `pinjet-common-1.0.0/src/pinjet_common.egg-info/SOURCES.txt` & `pinjet-common-1.0.1/src/pinjet_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

