# Comparing `tmp/shdo-0.1.0.tar.gz` & `tmp/shdo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.1.0.tar", last modified: Mon Apr  8 23:07:58 2024, max compression
+gzip compressed data, was "shdo-0.1.1.tar", last modified: Mon Apr  8 23:15:25 2024, max compression
```

## Comparing `shdo-0.1.0.tar` & `shdo-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 23:07:58.690843 shdo-0.1.0/
--rw-rw-rw-   0        0        0      350 2024-04-08 23:07:58.689808 shdo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 23:07:58.691836 shdo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-04-08 23:07:56.000000 shdo-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 23:07:58.687811 shdo-0.1.0/shdo.egg-info/
--rw-rw-rw-   0        0        0      350 2024-04-08 23:07:58.000000 shdo-0.1.0/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-04-08 23:07:58.000000 shdo-0.1.0/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 23:07:58.000000 shdo-0.1.0/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 23:07:58.000000 shdo-0.1.0/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-08 23:07:58.000000 shdo-0.1.0/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    18429 2024-04-08 23:07:14.000000 shdo-0.1.0/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:15:25.894862 shdo-0.1.1/
+-rw-rw-rw-   0        0        0      350 2024-04-08 23:15:25.892394 shdo-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2036 2024-04-08 14:07:04.000000 shdo-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 23:15:25.894862 shdo-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-04-08 23:15:22.000000 shdo-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:15:25.890590 shdo-0.1.1/shdo.egg-info/
+-rw-rw-rw-   0        0        0      350 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-08 23:15:25.000000 shdo-0.1.1/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    18488 2024-04-08 23:15:09.000000 shdo-0.1.1/shdo.py
```

### Comparing `shdo-0.1.0/README.md` & `shdo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shdo-0.1.0/setup.py` & `shdo-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.1.0',
+    version='0.1.1',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main',
             'shdo-pair = shdo:main',
```

### Comparing `shdo-0.1.0/shdo.py` & `shdo-0.1.1/shdo.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,16 @@
             if verbose == True:
                 print("done.")
             
             # change the command by its new path
             command = debug_path
 
     # build the full command
-    full_command = f"'{command}' {parameters}" if command is not None else None
+    full_command = f"'{command}'" if command is not None else None
+    full_command += f" {parameters}" if parameters is not None else ""
         
     # run the elevated command
     return _adb.execute(full_command, verbose=verbose)
 
 
 # handle everything about android debug bridge
 class _adb:
```

