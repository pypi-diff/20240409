# Comparing `tmp/google_trendy-1.4.tar.gz` & `tmp/google_trendy-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_trendy-1.4.tar", last modified: Tue Apr  9 18:37:49 2024, max compression
+gzip compressed data, was "google_trendy-1.5.tar", last modified: Tue Apr  9 18:49:50 2024, max compression
```

## Comparing `google_trendy-1.4.tar` & `google_trendy-1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:37:49.017907 google_trendy-1.4/
--rw-r--r--   0 michaelmondoro   (501) staff       (20)     1072 2024-04-09 18:12:48.000000 google_trendy-1.4/LICENSE
--rw-r--r--   0 michaelmondoro   (501) staff       (20)     2557 2024-04-09 18:37:49.016660 google_trendy-1.4/PKG-INFO
--rw-r--r--   0 michaelmondoro   (501) staff       (20)     2038 2024-04-09 18:37:15.000000 google_trendy-1.4/README.md
-drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:37:49.010101 google_trendy-1.4/google_trendy/
--rw-r--r--   0 michaelmondoro   (501) staff       (20)      153 2024-04-09 18:12:48.000000 google_trendy-1.4/google_trendy/__init__.py
--rw-r--r--   0 michaelmondoro   (501) staff       (20)     5518 2024-04-09 18:12:48.000000 google_trendy-1.4/google_trendy/google_trendy.py
-drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:37:49.015456 google_trendy-1.4/google_trendy.egg-info/
--rw-r--r--   0 michaelmondoro   (501) staff       (20)     2557 2024-04-09 18:37:48.000000 google_trendy-1.4/google_trendy.egg-info/PKG-INFO
--rw-r--r--   0 michaelmondoro   (501) staff       (20)      281 2024-04-09 18:37:48.000000 google_trendy-1.4/google_trendy.egg-info/SOURCES.txt
--rw-r--r--   0 michaelmondoro   (501) staff       (20)        1 2024-04-09 18:37:48.000000 google_trendy-1.4/google_trendy.egg-info/dependency_links.txt
--rw-r--r--   0 michaelmondoro   (501) staff       (20)       13 2024-04-09 18:37:48.000000 google_trendy-1.4/google_trendy.egg-info/requires.txt
--rw-r--r--   0 michaelmondoro   (501) staff       (20)       14 2024-04-09 18:37:48.000000 google_trendy-1.4/google_trendy.egg-info/top_level.txt
--rw-r--r--   0 michaelmondoro   (501) staff       (20)       38 2024-04-09 18:37:49.018237 google_trendy-1.4/setup.cfg
--rw-r--r--   0 michaelmondoro   (501) staff       (20)      749 2024-04-09 18:37:06.000000 google_trendy-1.4/setup.py
-drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:37:49.013741 google_trendy-1.4/tests/
--rw-r--r--   0 michaelmondoro   (501) staff       (20)      288 2024-04-09 18:12:48.000000 google_trendy-1.4/tests/test.py
+drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:49:50.423816 google_trendy-1.5/
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)     1072 2024-04-09 18:12:48.000000 google_trendy-1.5/LICENSE
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)     2577 2024-04-09 18:49:50.422542 google_trendy-1.5/PKG-INFO
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)     2038 2024-04-09 18:49:14.000000 google_trendy-1.5/README.md
+drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:49:50.414517 google_trendy-1.5/google_trendy/
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)      153 2024-04-09 18:12:48.000000 google_trendy-1.5/google_trendy/__init__.py
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)     5518 2024-04-09 18:12:48.000000 google_trendy-1.5/google_trendy/google_trendy.py
+drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:49:50.421436 google_trendy-1.5/google_trendy.egg-info/
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)     2577 2024-04-09 18:49:50.000000 google_trendy-1.5/google_trendy.egg-info/PKG-INFO
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)      281 2024-04-09 18:49:50.000000 google_trendy-1.5/google_trendy.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)        1 2024-04-09 18:49:50.000000 google_trendy-1.5/google_trendy.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)       18 2024-04-09 18:49:50.000000 google_trendy-1.5/google_trendy.egg-info/requires.txt
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)       14 2024-04-09 18:49:50.000000 google_trendy-1.5/google_trendy.egg-info/top_level.txt
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)       38 2024-04-09 18:49:50.424045 google_trendy-1.5/setup.cfg
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)      757 2024-04-09 18:49:27.000000 google_trendy-1.5/setup.py
+drwxr-xr-x   0 michaelmondoro   (501) staff       (20)        0 2024-04-09 18:49:50.420019 google_trendy-1.5/tests/
+-rw-r--r--   0 michaelmondoro   (501) staff       (20)      288 2024-04-09 18:12:48.000000 google_trendy-1.5/tests/test.py
```

### Comparing `google_trendy-1.4/LICENSE` & `google_trendy-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `google_trendy-1.4/PKG-INFO` & `google_trendy-1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: google_trendy
-Version: 1.4
+Version: 1.5
 Summary: Package for getting and analyzing tending Google searches
 Home-page: https://github.com/michaelMondoro/google_trendy
 Author: Michael Mondoro
 Author-email: michaelmondoro@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: requests
+Requires-Dist: lxml
 
 [![Generic badge](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Maintained-yes-green.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Python-3.10-yellow.svg)](https://shields.io/)
-[![Generic badge](https://img.shields.io/badge/google_trendy-1.4-red.svg)](https://pypi.org/project/google-trendy/)
+[![Generic badge](https://img.shields.io/badge/google_trendy-1.5-red.svg)](https://pypi.org/project/google-trendy/)
 [![Build](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml/badge.svg)](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml)
 
 ## Package
 Package for getting and analyzing tending Google searches
 
 ## Usage
 ```python
```

### Comparing `google_trendy-1.4/README.md` & `google_trendy-1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Generic badge](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Maintained-yes-green.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Python-3.10-yellow.svg)](https://shields.io/)
-[![Generic badge](https://img.shields.io/badge/google_trendy-1.4-red.svg)](https://pypi.org/project/google-trendy/)
+[![Generic badge](https://img.shields.io/badge/google_trendy-1.5-red.svg)](https://pypi.org/project/google-trendy/)
 [![Build](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml/badge.svg)](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml)
 
 ## Package
 Package for getting and analyzing tending Google searches
 
 ## Usage
 ```python
```

### Comparing `google_trendy-1.4/google_trendy/google_trendy.py` & `google_trendy-1.5/google_trendy/google_trendy.py`

 * *Files identical despite different names*

### Comparing `google_trendy-1.4/google_trendy.egg-info/PKG-INFO` & `google_trendy-1.5/google_trendy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: google-trendy
-Version: 1.4
+Version: 1.5
 Summary: Package for getting and analyzing tending Google searches
 Home-page: https://github.com/michaelMondoro/google_trendy
 Author: Michael Mondoro
 Author-email: michaelmondoro@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: requests
+Requires-Dist: lxml
 
 [![Generic badge](https://img.shields.io/badge/Licence-MIT-blue.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Maintained-yes-green.svg)](https://shields.io/)
 [![Generic badge](https://img.shields.io/badge/Python-3.10-yellow.svg)](https://shields.io/)
-[![Generic badge](https://img.shields.io/badge/google_trendy-1.4-red.svg)](https://pypi.org/project/google-trendy/)
+[![Generic badge](https://img.shields.io/badge/google_trendy-1.5-red.svg)](https://pypi.org/project/google-trendy/)
 [![Build](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml/badge.svg)](https://github.com/michaelMondoro/google_trendy/actions/workflows/python-package.yml)
 
 ## Package
 Package for getting and analyzing tending Google searches
 
 ## Usage
 ```python
```

### Comparing `google_trendy-1.4/setup.py` & `google_trendy-1.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="google_trendy",
-    version="1.4",
+    version="1.5",
     author="Michael Mondoro",
     author_email="michaelmondoro@gmail.com",
     description="Package for getting and analyzing tending Google searches",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelMondoro/google_trendy",
     packages=setuptools.find_packages(exclude="tests"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['bs4', 'requests'],
+    install_requires=['bs4', 'requests', 'lxml'],
     python_requires='>=3.7',
 )
```

