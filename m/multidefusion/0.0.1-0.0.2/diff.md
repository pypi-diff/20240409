# Comparing `tmp/multidefusion-0.0.1.tar.gz` & `tmp/multidefusion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.1.tar", last modified: Tue Apr  9 14:45:04 2024, max compression
+gzip compressed data, was "multidefusion-0.0.2.tar", last modified: Tue Apr  9 14:55:20 2024, max compression
```

## Comparing `multidefusion-0.0.1.tar` & `multidefusion-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 14:45:04.075111 multidefusion-0.0.1/
--rw-rw-rw-   0        0        0      176 2024-04-08 16:20:52.000000 multidefusion-0.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1095 2024-04-08 16:20:52.000000 multidefusion-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-08 16:20:52.000000 multidefusion-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1595 2024-04-09 14:45:04.075111 multidefusion-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-08 16:20:52.000000 multidefusion-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 14:45:04.059076 multidefusion-0.0.1/multidefusion/
--rw-rw-rw-   0        0        0      143 2024-04-08 16:20:52.000000 multidefusion-0.0.1/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    18556 2024-04-08 23:12:19.000000 multidefusion-0.0.1/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     1664 2024-04-09 14:22:12.000000 multidefusion-0.0.1/multidefusion/fushion.py
--rw-rw-rw-   0        0        0    26033 2024-04-09 14:22:23.000000 multidefusion-0.0.1/multidefusion/integration.py
--rw-rw-rw-   0        0        0       20 2024-04-08 16:20:52.000000 multidefusion-0.0.1/multidefusion/multidefusion.py
--rw-rw-rw-   0        0        0    44676 2024-04-08 23:12:19.000000 multidefusion-0.0.1/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:45:04.074598 multidefusion-0.0.1/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     1595 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       70 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 14:45:03.000000 multidefusion-0.0.1/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       73 2024-04-09 14:37:16.000000 multidefusion-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-04-09 14:45:04.077120 multidefusion-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1831 2024-04-08 16:20:52.000000 multidefusion-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 14:45:04.071600 multidefusion-0.0.1/tests/
--rw-rw-rw-   0        0        0      438 2024-04-08 16:20:52.000000 multidefusion-0.0.1/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:20.108794 multidefusion-0.0.2/
+-rw-rw-rw-   0        0        0      176 2024-04-08 16:20:52.000000 multidefusion-0.0.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1095 2024-04-08 16:20:52.000000 multidefusion-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-08 16:20:52.000000 multidefusion-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1595 2024-04-09 14:55:20.108794 multidefusion-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-08 16:20:52.000000 multidefusion-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:20.096605 multidefusion-0.0.2/multidefusion/
+-rw-rw-rw-   0        0        0      143 2024-04-08 16:20:52.000000 multidefusion-0.0.2/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0    18556 2024-04-08 23:12:19.000000 multidefusion-0.0.2/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     1664 2024-04-09 14:22:12.000000 multidefusion-0.0.2/multidefusion/fushion.py
+-rw-rw-rw-   0        0        0    26033 2024-04-09 14:51:22.000000 multidefusion-0.0.2/multidefusion/integration.py
+-rw-rw-rw-   0        0        0       20 2024-04-08 16:20:52.000000 multidefusion-0.0.2/multidefusion/multidefusion.py
+-rw-rw-rw-   0        0        0    44676 2024-04-08 23:12:19.000000 multidefusion-0.0.2/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:20.107792 multidefusion-0.0.2/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     1595 2024-04-09 14:55:19.000000 multidefusion-0.0.2/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2024-04-09 14:55:20.000000 multidefusion-0.0.2/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-09 14:55:19.000000 multidefusion-0.0.2/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-09 14:45:03.000000 multidefusion-0.0.2/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-09 14:55:19.000000 multidefusion-0.0.2/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 14:55:19.000000 multidefusion-0.0.2/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-09 14:37:16.000000 multidefusion-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-04-09 14:55:20.109794 multidefusion-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2024-04-09 14:54:18.000000 multidefusion-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 14:55:20.106780 multidefusion-0.0.2/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-08 16:20:52.000000 multidefusion-0.0.2/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.1/LICENSE` & `multidefusion-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/PKG-INFO` & `multidefusion-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondaś
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.1/README.md` & `multidefusion-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/multidefusion/datainterface.py` & `multidefusion-0.0.2/multidefusion/datainterface.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/multidefusion/fushion.py` & `multidefusion-0.0.2/multidefusion/fushion.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/multidefusion/integration.py` & `multidefusion-0.0.2/multidefusion/integration.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/multidefusion/results.py` & `multidefusion-0.0.2/multidefusion/results.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.1/multidefusion.egg-info/PKG-INFO` & `multidefusion-0.0.2/multidefusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.1
+Version: 0.0.2
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondaś
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.1/setup.py` & `multidefusion-0.0.2/setup.py`

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
-    version='0.0.1',
+    version='0.0.2',
     zip_safe=False,
 )
```

