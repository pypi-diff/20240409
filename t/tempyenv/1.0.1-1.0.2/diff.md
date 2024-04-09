# Comparing `tmp/tempyenv-1.0.1.tar.gz` & `tmp/tempyenv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempyenv-1.0.1.tar", last modified: Sun Apr  7 16:21:12 2024, max compression
+gzip compressed data, was "tempyenv-1.0.2.tar", last modified: Tue Apr  9 00:12:42 2024, max compression
```

## Comparing `tempyenv-1.0.1.tar` & `tempyenv-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-07 16:21:12.633455 tempyenv-1.0.1/
--rw-r--r--   0 starboarder2001   (501) staff       (20)     1063 2024-04-07 13:44:24.000000 tempyenv-1.0.1/LICENSE
--rw-r--r--   0 starboarder2001   (501) staff       (20)     2808 2024-04-07 16:21:12.632966 tempyenv-1.0.1/PKG-INFO
--rw-r--r--   0 starboarder2001   (501) staff       (20)      953 2024-04-07 13:54:16.000000 tempyenv-1.0.1/README.md
--rw-r--r--   0 starboarder2001   (501) staff       (20)      828 2024-04-07 16:20:40.000000 tempyenv-1.0.1/pyproject.toml
--rw-r--r--   0 starboarder2001   (501) staff       (20)       79 2024-04-07 16:21:12.635124 tempyenv-1.0.1/setup.cfg
--rw-r--r--   0 starboarder2001   (501) staff       (20)     2116 2024-04-07 16:10:42.000000 tempyenv-1.0.1/setup.py
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-07 16:21:12.620361 tempyenv-1.0.1/src/
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-07 16:21:12.624579 tempyenv-1.0.1/src/tempyenv/
--rw-r--r--   0 starboarder2001   (501) staff       (20)       53 2024-04-07 13:48:47.000000 tempyenv-1.0.1/src/tempyenv/__init__.py
--rw-r--r--   0 starboarder2001   (501) staff       (20)     1673 2024-04-07 16:16:55.000000 tempyenv-1.0.1/src/tempyenv/cli.py
-drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-07 16:21:12.631853 tempyenv-1.0.1/src/tempyenv.egg-info/
--rw-r--r--   0 starboarder2001   (501) staff       (20)     2808 2024-04-07 16:21:12.000000 tempyenv-1.0.1/src/tempyenv.egg-info/PKG-INFO
--rw-r--r--   0 starboarder2001   (501) staff       (20)      279 2024-04-07 16:21:12.000000 tempyenv-1.0.1/src/tempyenv.egg-info/SOURCES.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)        1 2024-04-07 16:21:12.000000 tempyenv-1.0.1/src/tempyenv.egg-info/dependency_links.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)       47 2024-04-07 16:21:12.000000 tempyenv-1.0.1/src/tempyenv.egg-info/entry_points.txt
--rw-r--r--   0 starboarder2001   (501) staff       (20)        9 2024-04-07 16:21:12.000000 tempyenv-1.0.1/src/tempyenv.egg-info/top_level.txt
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.054628 tempyenv-1.0.2/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1063 2024-04-07 13:44:24.000000 tempyenv-1.0.2/LICENSE
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     3234 2024-04-09 00:12:42.053361 tempyenv-1.0.2/PKG-INFO
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1379 2024-04-07 21:56:28.000000 tempyenv-1.0.2/README.md
+-rw-r--r--   0 starboarder2001   (501) staff       (20)      859 2024-04-09 00:11:34.000000 tempyenv-1.0.2/pyproject.toml
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       79 2024-04-09 00:12:42.057416 tempyenv-1.0.2/setup.cfg
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     2158 2024-04-09 00:11:34.000000 tempyenv-1.0.2/setup.py
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.039352 tempyenv-1.0.2/src/
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.046301 tempyenv-1.0.2/src/tempyenv/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       53 2024-04-09 00:11:34.000000 tempyenv-1.0.2/src/tempyenv/__init__.py
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     1661 2024-04-09 00:11:34.000000 tempyenv-1.0.2/src/tempyenv/cli.py
+drwxr-xr-x   0 starboarder2001   (501) staff       (20)        0 2024-04-09 00:12:42.051573 tempyenv-1.0.2/src/tempyenv.egg-info/
+-rw-r--r--   0 starboarder2001   (501) staff       (20)     3234 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/PKG-INFO
+-rw-r--r--   0 starboarder2001   (501) staff       (20)      279 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/SOURCES.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)        1 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/dependency_links.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)       75 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/entry_points.txt
+-rw-r--r--   0 starboarder2001   (501) staff       (20)        9 2024-04-09 00:12:42.000000 tempyenv-1.0.2/src/tempyenv.egg-info/top_level.txt
```

### Comparing `tempyenv-1.0.1/LICENSE` & `tempyenv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tempyenv-1.0.1/PKG-INFO` & `tempyenv-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempyenv
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easiest and quickest way to setup a temporary python virtual environment
 Home-page: https://github.com/outbit/tempyenv
 Author: David Whiteside
 Author-email: David Whiteside <david@davidwhiteside.com>
 License: MIT License
         
         Copyright (c) 2024 Outbit
@@ -38,14 +38,16 @@
 
 tempyenv
 =====================
 
 Description
 ===========
 
+The easiest and quickest way to create a temp/tmp/temporary python virtual environment.
+
 tempyenv sets up a python environment in a temporary path.  Quick way to create a throw away python environment.
 
 [![Build Status](https://app.travis-ci.com/outbit/tempyenv.svg?branch=develop "ansible-docs latest build")](http://travis-ci.org/outbit/tempyenv)
 [![PIP Version](https://img.shields.io/pypi/v/tempyenv.svg "tempyenv PyPI version")](https://pypi.python.org/pypi/tempyenv)
 [![Coverage Status](https://coveralls.io/repos/outbit/tempyenv/badge.svg?branch=develop&service=github)](https://coveralls.io/github/outbit/tempyenv?branch=develop)
 [![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/outbit/tempyenv)
 
@@ -58,14 +60,18 @@
 ```
 
 Usage
 ===========
 
 ```shell
 $ tempyenv
+(tempyenv) is setting up your virtual environment...hold tight
+Virtual environment created at /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
+Virtual environment loading from /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
+(tempyenv)(venv) $ echo "now you can pip install in your virtual environment"
 ```
 
 License
 =======
 
 tempyenv is released under the [MIT License](LICENSE.md).
```

### Comparing `tempyenv-1.0.1/pyproject.toml` & `tempyenv-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tempyenv"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="David Whiteside", email="david@davidwhiteside.com" },
 ]
 description = "Easiest and quickest way to setup a temporary python virtual environment"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -20,13 +20,14 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 tempyenv = "tempyenv.cli:main"
+tmpyenv = "tempyenv.cli:main"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
```

### Comparing `tempyenv-1.0.1/setup.py` & `tempyenv-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,13 @@
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
     python_requires='>=3.7',
     entry_points={
         'console_scripts': [
-          'tempyenv = tempyenv.cli:main'
+          'tempyenv = tempyenv.cli:main',
+          'tmpyenv = tempyenv.cli:main',
         ]
     },
     data_files=[],
 )
```

### Comparing `tempyenv-1.0.1/src/tempyenv/cli.py` & `tempyenv-1.0.2/src/tempyenv/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class TemporaryVenvCreator:
     def __init__(self):
         self.temp_dir = None
         self.venv_path = None
 
     def create_temporary_directory(self):
-        self.temp_dir = tempfile.TemporaryDirectory(delete=False)
+        self.temp_dir = tempfile.TemporaryDirectory()
         self.venv_path = os.path.join(self.temp_dir.name, 'venv')
 
     def create_virtual_environment(self):
         try:
             subprocess.run(['python3', '-m', 'venv', self.venv_path], check=True)
             print(f"Virtual environment created at {self.venv_path}")
         except subprocess.CalledProcessError as e:
```

### Comparing `tempyenv-1.0.1/src/tempyenv.egg-info/PKG-INFO` & `tempyenv-1.0.2/src/tempyenv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempyenv
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easiest and quickest way to setup a temporary python virtual environment
 Home-page: https://github.com/outbit/tempyenv
 Author: David Whiteside
 Author-email: David Whiteside <david@davidwhiteside.com>
 License: MIT License
         
         Copyright (c) 2024 Outbit
@@ -38,14 +38,16 @@
 
 tempyenv
 =====================
 
 Description
 ===========
 
+The easiest and quickest way to create a temp/tmp/temporary python virtual environment.
+
 tempyenv sets up a python environment in a temporary path.  Quick way to create a throw away python environment.
 
 [![Build Status](https://app.travis-ci.com/outbit/tempyenv.svg?branch=develop "ansible-docs latest build")](http://travis-ci.org/outbit/tempyenv)
 [![PIP Version](https://img.shields.io/pypi/v/tempyenv.svg "tempyenv PyPI version")](https://pypi.python.org/pypi/tempyenv)
 [![Coverage Status](https://coveralls.io/repos/outbit/tempyenv/badge.svg?branch=develop&service=github)](https://coveralls.io/github/outbit/tempyenv?branch=develop)
 [![Gitter IM](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/outbit/tempyenv)
 
@@ -58,14 +60,18 @@
 ```
 
 Usage
 ===========
 
 ```shell
 $ tempyenv
+(tempyenv) is setting up your virtual environment...hold tight
+Virtual environment created at /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
+Virtual environment loading from /var/folders/4b/dnp21z017cg_rbgfdtzclqlm0000gn/T/tmpacwjkg5z/venv
+(tempyenv)(venv) $ echo "now you can pip install in your virtual environment"
 ```
 
 License
 =======
 
 tempyenv is released under the [MIT License](LICENSE.md).
```

