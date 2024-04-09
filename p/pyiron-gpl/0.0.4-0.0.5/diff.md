# Comparing `tmp/pyiron-gpl-0.0.4.tar.gz` & `tmp/pyiron-gpl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-gpl-0.0.4.tar", last modified: Sat Nov 18 10:54:03 2023, max compression
+gzip compressed data, was "pyiron-gpl-0.0.5.tar", last modified: Tue Apr  9 13:17:21 2024, max compression
```

## Comparing `pyiron-gpl-0.0.4.tar` & `pyiron-gpl-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/elastic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21979 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/elastic/elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28879 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/gaussian/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/nma/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/nma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/nma/nma.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/quickff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/quickff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/quickff/quickff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl/yaff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/yaff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36534 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/pyiron_gpl/yaff/yaff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/pyiron_gpl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-18 10:54:03.589932 pyiron-gpl-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-18 10:54:03.000000 pyiron-gpl-0.0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2023-11-18 10:53:57.000000 pyiron-gpl-0.0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/pyiron_gpl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/elastic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/elastic/elastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28879 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/gaussian/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/nma/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/nma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/nma/nma.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/quickff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/quickff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/quickff/quickff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.333114 pyiron-gpl-0.0.5/pyiron_gpl/yaff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/yaff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36534 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/pyiron_gpl/yaff/yaff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/pyiron_gpl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 13:17:21.000000 pyiron-gpl-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:17:21.337115 pyiron-gpl-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/tests/test_quickff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18204 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/tests/test_yaff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-09 13:17:19.000000 pyiron-gpl-0.0.5/versioneer.py
```

### Comparing `pyiron-gpl-0.0.4/LICENSE` & `pyiron-gpl-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-gpl-0.0.4/PKG-INFO` & `pyiron-gpl-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: pyiron-gpl
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_gpl
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: GPLv3
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: molmod>=1.4.8
-Requires-Dist: numpy>=1.26.0
-Requires-Dist: pyiron_atomistics>=0.3.6
-Requires-Dist: spglib>=2.1.0
-Requires-Dist: scipy>=1.11.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: atomistics>=0.1.24
+Requires-Dist: pyiron_atomistics>=0.5.0
+Requires-Dist: spglib>=2.3.1
+Requires-Dist: scipy>=1.12.0
 Requires-Dist: quickff>=2.2.4
 Requires-Dist: tamkin>=1.2.6
 Requires-Dist: yaff>=1.6.0
 
 http://pyiron.org
```

### Comparing `pyiron-gpl-0.0.4/pyiron_gpl/gaussian/gaussian.py` & `pyiron-gpl-0.0.5/pyiron_gpl/gaussian/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyiron-gpl-0.0.4/pyiron_gpl/nma/nma.py` & `pyiron-gpl-0.0.5/pyiron_gpl/nma/nma.py`

 * *Files identical despite different names*

### Comparing `pyiron-gpl-0.0.4/pyiron_gpl/quickff/quickff.py` & `pyiron-gpl-0.0.5/pyiron_gpl/quickff/quickff.py`

 * *Files identical despite different names*

### Comparing `pyiron-gpl-0.0.4/pyiron_gpl/yaff/yaff.py` & `pyiron-gpl-0.0.5/pyiron_gpl/yaff/yaff.py`

 * *Files identical despite different names*

### Comparing `pyiron-gpl-0.0.4/pyiron_gpl.egg-info/PKG-INFO` & `pyiron-gpl-0.0.5/pyiron_gpl.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: pyiron-gpl
-Version: 0.0.4
+Version: 0.0.5
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_gpl
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: GPLv3
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 Requires-Dist: molmod>=1.4.8
-Requires-Dist: numpy>=1.26.0
-Requires-Dist: pyiron_atomistics>=0.3.6
-Requires-Dist: spglib>=2.1.0
-Requires-Dist: scipy>=1.11.3
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: atomistics>=0.1.24
+Requires-Dist: pyiron_atomistics>=0.5.0
+Requires-Dist: spglib>=2.3.1
+Requires-Dist: scipy>=1.12.0
 Requires-Dist: quickff>=2.2.4
 Requires-Dist: tamkin>=1.2.6
 Requires-Dist: yaff>=1.6.0
 
 http://pyiron.org
```

### Comparing `pyiron-gpl-0.0.4/setup.py` & `pyiron-gpl-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,28 @@
     license='GPLv3',
 
     classifiers=['Development Status :: 5 - Production/Stable',
                  'Topic :: Scientific/Engineering :: Physics',
                  'License :: OSI Approved :: BSD License',
                  'Intended Audience :: Science/Research',
                  'Operating System :: OS Independent',
-                 'Programming Language :: Python :: 3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9'],
+                 'Programming Language :: Python :: 3.9',
+                 'Programming Language :: Python :: 3.10',
+                 'Programming Language :: Python :: 3.11',
+    ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'molmod>=1.4.8',
-        'numpy>=1.26.0',
-        'pyiron_atomistics>=0.3.6',
-        'spglib>=2.1.0',
-        'scipy>=1.11.3',
+        'numpy>=1.26.4',
+        'atomistics>=0.1.24',
+        'pyiron_atomistics>=0.5.0',
+        'spglib>=2.3.1',
+        'scipy>=1.12.0',
         'quickff>=2.2.4',
         'tamkin>=1.2.6',
         'yaff>=1.6.0'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron-gpl-0.0.4/versioneer.py` & `pyiron-gpl-0.0.5/versioneer.py`

 * *Files identical despite different names*

