# Comparing `tmp/dirhash-0.3.0a0.tar.gz` & `tmp/dirhash-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirhash-0.3.0a0.tar", last modified: Tue Apr  9 21:04:48 2024, max compression
+gzip compressed data, was "dirhash-0.3.0a1.tar", last modified: Tue Apr  9 21:33:24 2024, max compression
```

## Comparing `dirhash-0.3.0a0.tar` & `dirhash-0.3.0a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.764720 dirhash-0.3.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.764720 dirhash-0.3.0a0/src/dirhash/
--rw-r--r--   0 runner    (1001) docker     (127)    25634 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24505 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/src/dirhash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28212 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/tests/test_dirhash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.483601 dirhash-0.3.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash/
+-rw-r--r--   0 runner    (1001) docker     (127)    25634 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/src/dirhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/src/dirhash/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/src/dirhash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 21:33:24.000000 dirhash-0.3.0a1/src/dirhash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:33:24.487601 dirhash-0.3.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28212 2024-04-09 21:33:20.000000 dirhash-0.3.0a1/tests/test_dirhash.py
```

### Comparing `dirhash-0.3.0a0/LICENSE` & `dirhash-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a0/PKG-INFO` & `dirhash-0.3.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirhash
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Python module and CLI for hashing of file system directories.
 Home-page: https://github.com/andhus/dirhash-python
 Author: Anders Huss
 Author-email: andhus@kth.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dirhash-0.3.0a0/README.md` & `dirhash-0.3.0a1/README.md`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a0/setup.py` & `dirhash-0.3.0a1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         long_description = '\n' + f.read()
 except IOError:
     long_description = DESCRIPTION
 
 setup(
     name='dirhash',
     version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/andhus/dirhash-python',
     author="Anders Huss",
     author_email="andhus@kth.se",
     license='MIT',
```

### Comparing `dirhash-0.3.0a0/src/dirhash/__init__.py` & `dirhash-0.3.0a1/src/dirhash/__init__.py`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a0/src/dirhash/cli.py` & `dirhash-0.3.0a1/src/dirhash/cli.py`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a0/src/dirhash.egg-info/PKG-INFO` & `dirhash-0.3.0a1/src/dirhash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirhash
-Version: 0.3.0a0
+Version: 0.3.0a1
 Summary: Python module and CLI for hashing of file system directories.
 Home-page: https://github.com/andhus/dirhash-python
 Author: Anders Huss
 Author-email: andhus@kth.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dirhash-0.3.0a0/tests/test_cli.py` & `dirhash-0.3.0a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dirhash-0.3.0a0/tests/test_dirhash.py` & `dirhash-0.3.0a1/tests/test_dirhash.py`

 * *Files identical despite different names*

