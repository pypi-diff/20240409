# Comparing `tmp/dynamics_utils-0.0.tar.gz` & `tmp/dynamics_utils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamics_utils-0.0.tar", last modified: Thu Feb  8 16:44:44 2024, max compression
+gzip compressed data, was "dynamics_utils-0.0.1.tar", last modified: Tue Apr  9 12:41:41 2024, max compression
```

## Comparing `dynamics_utils-0.0.tar` & `dynamics_utils-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.604643 dynamics_utils-0.0/
--rw-r--r--   0 chris-mbp   (501) staff       (20)      241 2024-02-08 16:44:44.604482 dynamics_utils-0.0/PKG-INFO
--rw-r--r--   0 chris-mbp   (501) staff       (20)     2058 2023-12-11 17:34:03.000000 dynamics_utils-0.0/README.md
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.601807 dynamics_utils-0.0/dynamics_utils/
--rw-r--r--   0 chris-mbp   (501) staff       (20)        0 2023-08-29 13:01:39.000000 dynamics_utils-0.0/dynamics_utils/__init__.py
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.602991 dynamics_utils-0.0/dynamics_utils/file_handling/
--rw-r--r--   0 chris-mbp   (501) staff       (20)        0 2023-08-31 08:49:13.000000 dynamics_utils-0.0/dynamics_utils/file_handling/__init__.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     1555 2024-02-08 16:44:31.000000 dynamics_utils-0.0/dynamics_utils/file_handling/load_files.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     4853 2023-09-14 15:09:14.000000 dynamics_utils-0.0/dynamics_utils/math.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)    19637 2024-02-07 15:36:51.000000 dynamics_utils-0.0/dynamics_utils/msm.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     3847 2023-08-29 16:13:06.000000 dynamics_utils-0.0/dynamics_utils/nmr.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     1263 2024-02-06 10:49:52.000000 dynamics_utils-0.0/dynamics_utils/potential.py
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.603813 dynamics_utils-0.0/dynamics_utils/utils/
--rw-r--r--   0 chris-mbp   (501) staff       (20)        1 2023-08-29 16:06:08.000000 dynamics_utils-0.0/dynamics_utils/utils/__init__.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     1264 2024-02-06 14:21:21.000000 dynamics_utils-0.0/dynamics_utils/utils/decorators.py
--rw-r--r--   0 chris-mbp   (501) staff       (20)     2541 2023-08-30 12:00:51.000000 dynamics_utils-0.0/dynamics_utils/utils/torch_utils.py
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.602723 dynamics_utils-0.0/dynamics_utils.egg-info/
--rw-r--r--   0 chris-mbp   (501) staff       (20)      241 2024-02-08 16:44:44.000000 dynamics_utils-0.0/dynamics_utils.egg-info/PKG-INFO
--rw-r--r--   0 chris-mbp   (501) staff       (20)      531 2024-02-08 16:44:44.000000 dynamics_utils-0.0/dynamics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 chris-mbp   (501) staff       (20)        1 2024-02-08 16:44:44.000000 dynamics_utils-0.0/dynamics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 chris-mbp   (501) staff       (20)       26 2024-02-08 16:44:44.000000 dynamics_utils-0.0/dynamics_utils.egg-info/requires.txt
--rw-r--r--   0 chris-mbp   (501) staff       (20)       15 2024-02-08 16:44:44.000000 dynamics_utils-0.0/dynamics_utils.egg-info/top_level.txt
--rw-r--r--   0 chris-mbp   (501) staff       (20)       38 2024-02-08 16:44:44.604691 dynamics_utils-0.0/setup.cfg
--rw-r--r--   0 chris-mbp   (501) staff       (20)      446 2024-02-06 10:29:48.000000 dynamics_utils-0.0/setup.py
-drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-02-08 16:44:44.604135 dynamics_utils-0.0/tests/
--rw-r--r--   0 chris-mbp   (501) staff       (20)      288 2023-08-30 11:17:46.000000 dynamics_utils-0.0/tests/test.py
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.806071 dynamics_utils-0.0.1/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)      243 2024-04-09 12:41:41.805925 dynamics_utils-0.0.1/PKG-INFO
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     2058 2023-12-11 17:34:03.000000 dynamics_utils-0.0.1/README.md
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.803529 dynamics_utils-0.0.1/dynamics_utils/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)        0 2023-08-29 13:01:39.000000 dynamics_utils-0.0.1/dynamics_utils/__init__.py
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.804634 dynamics_utils-0.0.1/dynamics_utils/file_handling/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)        0 2023-08-31 08:49:13.000000 dynamics_utils-0.0.1/dynamics_utils/file_handling/__init__.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     1555 2024-02-08 16:44:31.000000 dynamics_utils-0.0.1/dynamics_utils/file_handling/load_files.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     4853 2023-09-14 15:09:14.000000 dynamics_utils-0.0.1/dynamics_utils/math.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)    19637 2024-02-07 15:36:51.000000 dynamics_utils-0.0.1/dynamics_utils/msm.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     3847 2023-08-29 16:13:06.000000 dynamics_utils-0.0.1/dynamics_utils/nmr.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     1263 2024-02-06 10:49:52.000000 dynamics_utils-0.0.1/dynamics_utils/potential.py
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.805383 dynamics_utils-0.0.1/dynamics_utils/utils/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)        1 2023-08-29 16:06:08.000000 dynamics_utils-0.0.1/dynamics_utils/utils/__init__.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     1264 2024-02-06 14:21:21.000000 dynamics_utils-0.0.1/dynamics_utils/utils/decorators.py
+-rw-r--r--   0 chris-mbp   (501) staff       (20)     2541 2024-04-09 12:34:44.000000 dynamics_utils-0.0.1/dynamics_utils/utils/torch_utils.py
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.804399 dynamics_utils-0.0.1/dynamics_utils.egg-info/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)      243 2024-04-09 12:41:41.000000 dynamics_utils-0.0.1/dynamics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 chris-mbp   (501) staff       (20)      531 2024-04-09 12:41:41.000000 dynamics_utils-0.0.1/dynamics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 chris-mbp   (501) staff       (20)        1 2024-04-09 12:41:41.000000 dynamics_utils-0.0.1/dynamics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 chris-mbp   (501) staff       (20)       26 2024-04-09 12:41:41.000000 dynamics_utils-0.0.1/dynamics_utils.egg-info/requires.txt
+-rw-r--r--   0 chris-mbp   (501) staff       (20)       15 2024-04-09 12:41:41.000000 dynamics_utils-0.0.1/dynamics_utils.egg-info/top_level.txt
+-rw-r--r--   0 chris-mbp   (501) staff       (20)       38 2024-04-09 12:41:41.806119 dynamics_utils-0.0.1/setup.cfg
+-rw-r--r--   0 chris-mbp   (501) staff       (20)      448 2024-04-09 12:41:22.000000 dynamics_utils-0.0.1/setup.py
+drwxr-xr-x   0 chris-mbp   (501) staff       (20)        0 2024-04-09 12:41:41.805631 dynamics_utils-0.0.1/tests/
+-rw-r--r--   0 chris-mbp   (501) staff       (20)      288 2023-08-30 11:17:46.000000 dynamics_utils-0.0.1/tests/test.py
```

### Comparing `dynamics_utils-0.0/README.md` & `dynamics_utils-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/file_handling/load_files.py` & `dynamics_utils-0.0.1/dynamics_utils/file_handling/load_files.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/math.py` & `dynamics_utils-0.0.1/dynamics_utils/math.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/msm.py` & `dynamics_utils-0.0.1/dynamics_utils/msm.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/nmr.py` & `dynamics_utils-0.0.1/dynamics_utils/nmr.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/potential.py` & `dynamics_utils-0.0.1/dynamics_utils/potential.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/utils/decorators.py` & `dynamics_utils-0.0.1/dynamics_utils/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils/utils/torch_utils.py` & `dynamics_utils-0.0.1/dynamics_utils/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `dynamics_utils-0.0/dynamics_utils.egg-info/SOURCES.txt` & `dynamics_utils-0.0.1/dynamics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

