# Comparing `tmp/multidefusion-0.0.3.tar.gz` & `tmp/multidefusion-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.3.tar", last modified: Tue Apr  9 14:58:56 2024, max compression
+gzip compressed data, was "multidefusion-0.0.4.tar", last modified: Tue Apr  9 15:05:07 2024, max compression
```

## Comparing `multidefusion-0.0.3.tar` & `multidefusion-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:58:56.525563 multidefusion-0.0.3/
--rw-rw-rw-   0        0        0      176 2024-04-08 16:20:52.000000 multidefusion-0.0.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     1095 2024-04-08 16:20:52.000000 multidefusion-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-08 16:20:52.000000 multidefusion-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1595 2024-04-09 14:58:56.525055 multidefusion-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-08 16:20:52.000000 multidefusion-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:58:56.511379 multidefusion-0.0.3/multidefusion/
--rw-rw-rw-   0        0        0      143 2024-04-08 16:20:52.000000 multidefusion-0.0.3/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    18556 2024-04-08 23:12:19.000000 multidefusion-0.0.3/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     1664 2024-04-09 14:22:12.000000 multidefusion-0.0.3/multidefusion/fushion.py
--rw-rw-rw-   0        0        0    26033 2024-04-09 14:51:22.000000 multidefusion-0.0.3/multidefusion/integration.py
--rw-rw-rw-   0        0        0       20 2024-04-08 16:20:52.000000 multidefusion-0.0.3/multidefusion/multidefusion.py
--rw-rw-rw-   0        0        0    44676 2024-04-08 23:12:19.000000 multidefusion-0.0.3/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:58:56.524052 multidefusion-0.0.3/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     1595 2024-04-09 14:58:56.000000 multidefusion-0.0.3/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-09 14:58:56.000000 multidefusion-0.0.3/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       70 2024-04-09 14:58:56.000000 multidefusion-0.0.3/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 14:45:03.000000 multidefusion-0.0.3/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-04-09 14:58:56.000000 multidefusion-0.0.3/multidefusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 14:58:56.000000 multidefusion-0.0.3/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       73 2024-04-09 14:37:16.000000 multidefusion-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-04-09 14:58:56.526571 multidefusion-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-04-09 14:57:35.000000 multidefusion-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:58:56.523046 multidefusion-0.0.3/tests/
--rw-rw-rw-   0        0        0      438 2024-04-08 16:20:52.000000 multidefusion-0.0.3/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:05:07.058366 multidefusion-0.0.4/
+-rw-rw-rw-   0        0        0      176 2024-04-08 16:20:52.000000 multidefusion-0.0.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1095 2024-04-08 16:20:52.000000 multidefusion-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-08 16:20:52.000000 multidefusion-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1595 2024-04-09 15:05:07.057365 multidefusion-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-08 16:20:52.000000 multidefusion-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:05:07.046964 multidefusion-0.0.4/multidefusion/
+-rw-rw-rw-   0        0        0      143 2024-04-08 16:20:52.000000 multidefusion-0.0.4/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0    18556 2024-04-08 23:12:19.000000 multidefusion-0.0.4/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     1664 2024-04-09 14:22:12.000000 multidefusion-0.0.4/multidefusion/fushion.py
+-rw-rw-rw-   0        0        0    26033 2024-04-09 14:51:22.000000 multidefusion-0.0.4/multidefusion/integration.py
+-rw-rw-rw-   0        0        0    44676 2024-04-08 23:12:19.000000 multidefusion-0.0.4/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:05:07.056358 multidefusion-0.0.4/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     1595 2024-04-09 15:05:06.000000 multidefusion-0.0.4/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-09 15:05:06.000000 multidefusion-0.0.4/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-09 15:05:06.000000 multidefusion-0.0.4/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 14:45:03.000000 multidefusion-0.0.4/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-09 15:05:06.000000 multidefusion-0.0.4/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 15:05:06.000000 multidefusion-0.0.4/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-09 14:37:16.000000 multidefusion-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-04-09 15:05:07.059365 multidefusion-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2024-04-09 15:04:34.000000 multidefusion-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:05:07.054964 multidefusion-0.0.4/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-08 16:20:52.000000 multidefusion-0.0.4/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.3/LICENSE` & `multidefusion-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/PKG-INFO` & `multidefusion-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.3
+Version: 0.0.4
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondaś
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.3/README.md` & `multidefusion-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/multidefusion/datainterface.py` & `multidefusion-0.0.4/multidefusion/datainterface.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/multidefusion/fushion.py` & `multidefusion-0.0.4/multidefusion/fushion.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/multidefusion/integration.py` & `multidefusion-0.0.4/multidefusion/integration.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/multidefusion/results.py` & `multidefusion-0.0.4/multidefusion/results.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.3/multidefusion.egg-info/PKG-INFO` & `multidefusion-0.0.4/multidefusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.3
+Version: 0.0.4
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondaś
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.3/setup.py` & `multidefusion-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='multidefusion',
     name='multidefusion',
     packages=find_packages(include=['multidefusion', 'multidefusion.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/damiantondas/multidefusion',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

