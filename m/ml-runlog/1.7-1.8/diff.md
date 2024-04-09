# Comparing `tmp/ml_runlog-1.7.tar.gz` & `tmp/ml_runlog-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_runlog-1.7.tar", last modified: Fri Jan  7 06:15:25 2022, max compression
+gzip compressed data, was "ml_runlog-1.8.tar", last modified: Tue Apr  9 04:20:37 2024, max compression
```

## Comparing `ml_runlog-1.7.tar` & `ml_runlog-1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 anag      (1009) anag      (1009)        0 2022-01-07 06:15:25.607879 ml_runlog-1.7/
--rw-r--r--   0 anag      (1009) anag      (1009)      260 2022-01-07 06:15:25.607879 ml_runlog-1.7/PKG-INFO
-drwxr-xr-x   0 anag      (1009) anag      (1009)        0 2022-01-07 06:15:25.607879 ml_runlog-1.7/ml_runlog/
--rw-r--r--   0 anag      (1009) anag      (1009)     1315 2022-01-07 06:14:46.000000 ml_runlog-1.7/ml_runlog/__init__.py
--rw-r--r--   0 anag      (1009) anag      (1009)      880 2022-01-05 18:10:07.000000 ml_runlog-1.7/ml_runlog/main.py
-drwxr-xr-x   0 anag      (1009) anag      (1009)        0 2022-01-07 06:15:25.607879 ml_runlog-1.7/ml_runlog.egg-info/
--rw-r--r--   0 anag      (1009) anag      (1009)      260 2022-01-07 06:15:25.000000 ml_runlog-1.7/ml_runlog.egg-info/PKG-INFO
--rw-r--r--   0 anag      (1009) anag      (1009)      244 2022-01-07 06:15:25.000000 ml_runlog-1.7/ml_runlog.egg-info/SOURCES.txt
--rw-r--r--   0 anag      (1009) anag      (1009)        1 2022-01-07 06:15:25.000000 ml_runlog-1.7/ml_runlog.egg-info/dependency_links.txt
--rw-r--r--   0 anag      (1009) anag      (1009)        1 2021-11-08 23:59:45.000000 ml_runlog-1.7/ml_runlog.egg-info/not-zip-safe
--rw-r--r--   0 anag      (1009) anag      (1009)       17 2022-01-07 06:15:25.000000 ml_runlog-1.7/ml_runlog.egg-info/requires.txt
--rw-r--r--   0 anag      (1009) anag      (1009)       10 2022-01-07 06:15:25.000000 ml_runlog-1.7/ml_runlog.egg-info/top_level.txt
--rw-r--r--   0 anag      (1009) anag      (1009)       38 2022-01-07 06:15:25.607879 ml_runlog-1.7/setup.cfg
--rw-r--r--   0 anag      (1009) anag      (1009)      421 2022-01-07 06:15:00.000000 ml_runlog-1.7/setup.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/
+-rw-rw-r--   0 anag      (1000) anag      (1000)      232 2024-04-09 04:20:37.668134 ml_runlog-1.8/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-1.8/README.md
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/ml_runlog/
+-rw-rw-r--   0 anag      (1000) anag      (1000)     1941 2024-04-09 03:29:18.000000 ml_runlog-1.8/ml_runlog/__init__.py
+-rw-rw-r--   0 anag      (1000) anag      (1000)      880 2024-04-09 03:18:50.000000 ml_runlog-1.8/ml_runlog/main.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/ml_runlog.egg-info/
+-rw-rw-r--   0 anag      (1000) anag      (1000)      232 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 03:24:40.000000 ml_runlog-1.8/ml_runlog.egg-info/not-zip-safe
+-rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/requires.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/top_level.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-09 04:20:37.668134 ml_runlog-1.8/setup.cfg
+-rw-rw-r--   0 anag      (1000) anag      (1000)      421 2024-04-09 04:14:28.000000 ml_runlog-1.8/setup.py
```

### Comparing `ml_runlog-1.7/ml_runlog/main.py` & `ml_runlog-1.8/ml_runlog/main.py`

 * *Files identical despite different names*

