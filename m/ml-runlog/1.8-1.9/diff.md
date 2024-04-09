# Comparing `tmp/ml_runlog-1.8.tar.gz` & `tmp/ml_runlog-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_runlog-1.8.tar", last modified: Tue Apr  9 04:20:37 2024, max compression
+gzip compressed data, was "ml_runlog-1.9.tar", last modified: Tue Apr  9 06:00:46 2024, max compression
```

## Comparing `ml_runlog-1.8.tar` & `ml_runlog-1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/
--rw-rw-r--   0 anag      (1000) anag      (1000)      232 2024-04-09 04:20:37.668134 ml_runlog-1.8/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-1.8/README.md
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/ml_runlog/
--rw-rw-r--   0 anag      (1000) anag      (1000)     1941 2024-04-09 03:29:18.000000 ml_runlog-1.8/ml_runlog/__init__.py
--rw-rw-r--   0 anag      (1000) anag      (1000)      880 2024-04-09 03:18:50.000000 ml_runlog-1.8/ml_runlog/main.py
-drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 04:20:37.668134 ml_runlog-1.8/ml_runlog.egg-info/
--rw-rw-r--   0 anag      (1000) anag      (1000)      232 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/PKG-INFO
--rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/SOURCES.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/dependency_links.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 03:24:40.000000 ml_runlog-1.8/ml_runlog.egg-info/not-zip-safe
--rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/requires.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-09 04:20:37.000000 ml_runlog-1.8/ml_runlog.egg-info/top_level.txt
--rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-09 04:20:37.668134 ml_runlog-1.8/setup.cfg
--rw-rw-r--   0 anag      (1000) anag      (1000)      421 2024-04-09 04:14:28.000000 ml_runlog-1.8/setup.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/
+-rw-rw-r--   0 anag      (1000) anag      (1000)    35149 2024-04-09 05:52:10.000000 ml_runlog-1.9/LICENSE
+-rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 06:00:46.948664 ml_runlog-1.9/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)     1827 2024-04-09 03:18:50.000000 ml_runlog-1.9/README.md
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/ml_runlog/
+-rw-rw-r--   0 anag      (1000) anag      (1000)     2072 2024-04-09 05:50:10.000000 ml_runlog-1.9/ml_runlog/__init__.py
+-rw-rw-r--   0 anag      (1000) anag      (1000)      880 2024-04-09 03:18:50.000000 ml_runlog-1.9/ml_runlog/main.py
+drwxrwxr-x   0 anag      (1000) anag      (1000)        0 2024-04-09 06:00:46.948664 ml_runlog-1.9/ml_runlog.egg-info/
+-rw-rw-r--   0 anag      (1000) anag      (1000)      254 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/PKG-INFO
+-rw-rw-r--   0 anag      (1000) anag      (1000)      262 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)        1 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/not-zip-safe
+-rw-rw-r--   0 anag      (1000) anag      (1000)       17 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/requires.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       10 2024-04-09 06:00:46.000000 ml_runlog-1.9/ml_runlog.egg-info/top_level.txt
+-rw-rw-r--   0 anag      (1000) anag      (1000)       38 2024-04-09 06:00:46.948664 ml_runlog-1.9/setup.cfg
+-rw-rw-r--   0 anag      (1000) anag      (1000)      421 2024-04-09 05:55:02.000000 ml_runlog-1.9/setup.py
```

### Comparing `ml_runlog-1.8/README.md` & `ml_runlog-1.9/README.md`

 * *Files identical despite different names*

### Comparing `ml_runlog-1.8/ml_runlog/__init__.py` & `ml_runlog-1.9/ml_runlog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,19 @@
     global gc
     global sno
     global worksheet 
     global column_idx
 
     creds_path = creds_path_
     sheet_name = sheet_name_
-    worksheet_idx = worksheet_idx_
+    worksheet_idx = worksheet_idx_      
+
+    gc = pygsheets.authorize(service_file=creds_path) 
+    sheet = gc.open(sheet_name)
+    worksheet = sheet[worksheet_idx]
 
 def log_data(offset=0, increment_cols=True, verify_timeout=None, **kwargs):
     global sno 
     global column_idx
     global worksheet 
     global sno_logged
```

### Comparing `ml_runlog-1.8/ml_runlog/main.py` & `ml_runlog-1.9/ml_runlog/main.py`

 * *Files identical despite different names*

