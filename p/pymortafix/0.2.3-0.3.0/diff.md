# Comparing `tmp/pymortafix-0.2.3.tar.gz` & `tmp/pymortafix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymortafix-0.2.3.tar", last modified: Tue Dec  6 14:38:28 2022, max compression
+gzip compressed data, was "pymortafix-0.3.0.tar", last modified: Tue Apr  9 07:18:24 2024, max compression
```

## Comparing `pymortafix-0.2.3.tar` & `pymortafix-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 Moris      (501) staff       (20)        0 2022-12-06 14:38:28.729117 pymortafix-0.2.3/
--rwxrwxrwx   0 Moris      (501) staff       (20)     1068 2020-09-15 12:01:30.000000 pymortafix-0.2.3/LICENSE
--rw-r--r--   0 Moris      (501) staff       (20)     1047 2022-12-06 14:38:28.728944 pymortafix-0.2.3/PKG-INFO
--rwxr-xr-x   0 Moris      (501) staff       (20)      471 2021-03-02 13:14:50.000000 pymortafix-0.2.3/README.md
-drwxr-xr-x   0 Moris      (501) staff       (20)        0 2022-12-06 14:38:28.727634 pymortafix-0.2.3/pymortafix/
--rw-r--r--   0 Moris      (501) staff       (20)        0 2021-01-12 08:56:06.000000 pymortafix-0.2.3/pymortafix/__init__.py
--rwxr-xr-x   0 Moris      (501) staff       (20)      761 2022-12-06 14:12:30.000000 pymortafix-0.2.3/pymortafix/_getchar.py
--rwxr-xr-x   0 Moris      (501) staff       (20)     3285 2022-12-06 14:37:34.000000 pymortafix-0.2.3/pymortafix/telegram.py
--rwxr-xr-x   0 Moris      (501) staff       (20)     2025 2022-12-06 14:12:30.000000 pymortafix-0.2.3/pymortafix/utils.py
-drwxr-xr-x   0 Moris      (501) staff       (20)        0 2022-12-06 14:38:28.728708 pymortafix-0.2.3/pymortafix.egg-info/
--rw-r--r--   0 Moris      (501) staff       (20)     1047 2022-12-06 14:38:28.000000 pymortafix-0.2.3/pymortafix.egg-info/PKG-INFO
--rw-r--r--   0 Moris      (501) staff       (20)      284 2022-12-06 14:38:28.000000 pymortafix-0.2.3/pymortafix.egg-info/SOURCES.txt
--rw-r--r--   0 Moris      (501) staff       (20)        1 2022-12-06 14:38:28.000000 pymortafix-0.2.3/pymortafix.egg-info/dependency_links.txt
--rw-r--r--   0 Moris      (501) staff       (20)       16 2022-12-06 14:38:28.000000 pymortafix-0.2.3/pymortafix.egg-info/requires.txt
--rw-r--r--   0 Moris      (501) staff       (20)       11 2022-12-06 14:38:28.000000 pymortafix-0.2.3/pymortafix.egg-info/top_level.txt
--rw-r--r--   0 Moris      (501) staff       (20)       38 2022-12-06 14:38:28.729174 pymortafix-0.2.3/setup.cfg
--rwxr-xr-x   0 Moris      (501) staff       (20)      880 2022-12-06 14:22:04.000000 pymortafix-0.2.3/setup.py
+drwxr-xr-x   0 moris      (501) staff       (20)        0 2024-04-09 07:18:24.753883 pymortafix-0.3.0/
+-rwxrwxrwx   0 moris      (501) staff       (20)     1068 2021-01-13 07:32:06.000000 pymortafix-0.3.0/LICENSE
+-rw-r--r--   0 moris      (501) staff       (20)     1142 2024-04-09 07:18:24.753664 pymortafix-0.3.0/PKG-INFO
+-rwxrwxrwx   0 moris      (501) staff       (20)      471 2021-01-14 10:19:32.000000 pymortafix-0.3.0/README.md
+drwxr-xr-x   0 moris      (501) staff       (20)        0 2024-04-09 07:18:24.752105 pymortafix-0.3.0/pymortafix/
+-rwxrwxrwx   0 moris      (501) staff       (20)        0 2021-01-13 07:33:20.000000 pymortafix-0.3.0/pymortafix/__init__.py
+-rwxrwxrwx   0 moris      (501) staff       (20)      761 2021-03-05 08:04:00.000000 pymortafix-0.3.0/pymortafix/_getchar.py
+-rwxr-xr-x   0 moris      (501) staff       (20)     3346 2024-04-09 07:17:18.000000 pymortafix-0.3.0/pymortafix/telegram.py
+-rwxrwxrwx   0 moris      (501) staff       (20)     2025 2022-01-28 10:05:48.000000 pymortafix-0.3.0/pymortafix/utils.py
+drwxr-xr-x   0 moris      (501) staff       (20)        0 2024-04-09 07:18:24.753353 pymortafix-0.3.0/pymortafix.egg-info/
+-rw-r--r--   0 moris      (501) staff       (20)     1142 2024-04-09 07:18:24.000000 pymortafix-0.3.0/pymortafix.egg-info/PKG-INFO
+-rwxrwxrwx   0 moris      (501) staff       (20)      320 2024-04-09 07:18:24.000000 pymortafix-0.3.0/pymortafix.egg-info/SOURCES.txt
+-rwxrwxrwx   0 moris      (501) staff       (20)        1 2024-04-09 07:18:24.000000 pymortafix-0.3.0/pymortafix.egg-info/dependency_links.txt
+-rwxrwxrwx   0 moris      (501) staff       (20)       48 2024-04-09 07:18:24.000000 pymortafix-0.3.0/pymortafix.egg-info/requires.txt
+-rwxrwxrwx   0 moris      (501) staff       (20)       16 2024-04-09 07:18:24.000000 pymortafix-0.3.0/pymortafix.egg-info/top_level.txt
+-rw-r--r--   0 moris      (501) staff       (20)       38 2024-04-09 07:18:24.753930 pymortafix-0.3.0/setup.cfg
+-rwxr-xr-x   0 moris      (501) staff       (20)      948 2024-04-09 07:12:55.000000 pymortafix-0.3.0/setup.py
+drwxr-xr-x   0 moris      (501) staff       (20)        0 2024-04-09 07:18:24.753119 pymortafix-0.3.0/test/
+-rwxrwxrwx   0 moris      (501) staff       (20)        0 2021-03-05 09:30:28.000000 pymortafix-0.3.0/test/__init__.py
+-rwxrwxrwx   0 moris      (501) staff       (20)     2874 2021-07-12 08:19:16.000000 pymortafix-0.3.0/test/utils_test.py
```

### Comparing `pymortafix-0.2.3/LICENSE` & `pymortafix-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymortafix-0.2.3/PKG-INFO` & `pymortafix-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pymortafix
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python module to collect some usefull stuff
 Home-page: https://github.com/mortafix/PyMortafix
 Author: Moris Doratiotto
 Author-email: moris.doratiotto@gmail.com
 Keywords: telegram,bot,utils
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorifix==2.0.4
+Requires-Dist: emoji==2.11.0
+Requires-Dist: requests==2.31.0
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymortafix)
 [![PyPI](https://img.shields.io/pypi/v/pymortafix?color=red)](https://pypi.org/project/pymortafix/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub](https://img.shields.io/github/license/mortafix/PyMortafix)
 
 # Setup
```

### Comparing `pymortafix-0.2.3/pymortafix/_getchar.py` & `pymortafix-0.3.0/pymortafix/_getchar.py`

 * *Files identical despite different names*

### Comparing `pymortafix-0.2.3/pymortafix/utils.py` & `pymortafix-0.3.0/pymortafix/utils.py`

 * *Files identical despite different names*

### Comparing `pymortafix-0.2.3/pymortafix.egg-info/PKG-INFO` & `pymortafix-0.3.0/pymortafix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pymortafix
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python module to collect some usefull stuff
 Home-page: https://github.com/mortafix/PyMortafix
 Author: Moris Doratiotto
 Author-email: moris.doratiotto@gmail.com
 Keywords: telegram,bot,utils
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colorifix==2.0.4
+Requires-Dist: emoji==2.11.0
+Requires-Dist: requests==2.31.0
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pymortafix)
 [![PyPI](https://img.shields.io/pypi/v/pymortafix?color=red)](https://pypi.org/project/pymortafix/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub](https://img.shields.io/github/license/mortafix/PyMortafix)
 
 # Setup
```

### Comparing `pymortafix-0.2.3/setup.py` & `pymortafix-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymortafix",
-    version="0.2.3",
+    version="0.3.0",
     author="Moris Doratiotto",
     author_email="moris.doratiotto@gmail.com",
     description="A python module to collect some usefull stuff",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mortafix/PyMortafix",
     packages=setuptools.find_packages(),
-    install_requires=["colorifix", "emoji"],
+    install_requires=[
+        "colorifix==2.0.4",
+        "emoji==2.11.0",
+        "requests==2.31.0",
+    ],
     classifiers=[
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.10",
     keywords=[
         "telegram",
         "bot",
         "utils",
     ],
 )
```

