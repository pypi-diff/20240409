# Comparing `tmp/dirhash-0.2.1.tar.gz` & `tmp/dirhash-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dirhash-0.2.1.tar", last modified: Wed Aug 26 19:52:55 2020, max compression
+gzip compressed data, was "dirhash-0.3.0a0.tar", last modified: Tue Apr  9 21:04:48 2024, max compression
```

## Comparing `dirhash-0.2.1.tar` & `dirhash-0.3.0a0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 andershuss   (501) staff       (20)        0 2020-08-26 19:52:55.000000 dirhash-0.2.1/
--rw-r--r--   0 andershuss   (501) staff       (20)     1068 2020-04-21 11:43:39.000000 dirhash-0.2.1/LICENSE
--rw-r--r--   0 andershuss   (501) staff       (20)       26 2020-04-21 11:43:39.000000 dirhash-0.2.1/MANIFEST.in
--rw-r--r--   0 andershuss   (501) staff       (20)     5709 2020-08-26 19:52:55.000000 dirhash-0.2.1/PKG-INFO
--rw-r--r--   0 andershuss   (501) staff       (20)     4649 2020-04-26 11:43:36.000000 dirhash-0.2.1/README.md
--rw-r--r--   0 andershuss   (501) staff       (20)       38 2020-08-26 19:52:55.000000 dirhash-0.2.1/setup.cfg
--rw-r--r--   0 andershuss   (501) staff       (20)     1086 2020-08-26 19:48:39.000000 dirhash-0.2.1/setup.py
-drwxr-xr-x   0 andershuss   (501) staff       (20)        0 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/
-drwxr-xr-x   0 andershuss   (501) staff       (20)        0 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash/
--rw-r--r--   0 andershuss   (501) staff       (20)    25623 2020-08-26 19:48:39.000000 dirhash-0.2.1/src/dirhash/__init__.py
--rw-r--r--   0 andershuss   (501) staff       (20)     6413 2020-04-21 11:43:39.000000 dirhash-0.2.1/src/dirhash/cli.py
--rw-r--r--   0 andershuss   (501) staff       (20)       22 2020-08-26 19:48:39.000000 dirhash-0.2.1/src/dirhash/version.py
-drwxr-xr-x   0 andershuss   (501) staff       (20)        0 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/
--rw-r--r--   0 andershuss   (501) staff       (20)     5709 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/PKG-INFO
--rw-r--r--   0 andershuss   (501) staff       (20)      316 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/SOURCES.txt
--rw-r--r--   0 andershuss   (501) staff       (20)        1 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/dependency_links.txt
--rw-r--r--   0 andershuss   (501) staff       (20)       46 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/entry_points.txt
--rw-r--r--   0 andershuss   (501) staff       (20)       16 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/requires.txt
--rw-r--r--   0 andershuss   (501) staff       (20)        8 2020-08-26 19:52:55.000000 dirhash-0.2.1/src/dirhash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.764720 dirhash-0.3.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.764720 dirhash-0.3.0a0/src/dirhash/
+-rw-r--r--   0 runner    (1001) docker     (127)    25634 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24505 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/src/dirhash/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/src/dirhash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 21:04:48.000000 dirhash-0.3.0a0/src/dirhash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:04:48.768720 dirhash-0.3.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8290 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28212 2024-04-09 21:04:42.000000 dirhash-0.3.0a0/tests/test_dirhash.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dirhash-0.2.1/LICENSE` & `dirhash-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dirhash-0.2.1/PKG-INFO` & `dirhash-0.3.0a0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,107 @@
 Metadata-Version: 2.1
 Name: dirhash
-Version: 0.2.1
+Version: 0.3.0a0
 Summary: Python module and CLI for hashing of file system directories.
 Home-page: https://github.com/andhus/dirhash-python
 Author: Anders Huss
 Author-email: andhus@kth.se
 License: MIT
-Description: 
-        [![Build Status](https://travis-ci.com/andhus/dirhash-python.svg?branch=master)](https://travis-ci.com/andhus/dirhash-python)
-        [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
-        
-        # dirhash
-        A lightweight python module and CLI for computing the hash of any
-        directory based on its files' structure and content.
-        - Supports all hashing algorithms of Python's built-in `hashlib` module.
-        - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
-        - Multiprocessing for up to [6x speed-up](#performance)
-        
-        The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
-        
-        ## Installation
-        From PyPI:
-        ```commandline
-        pip install dirhash
-        ```
-        Or directly from source:
-        ```commandline
-        git clone git@github.com:andhus/dirhash-python.git
-        pip install dirhash/
-        ```
-        
-        ## Usage
-        Python module:
-        ```python
-        from dirhash import dirhash
-        
-        dirpath = "path/to/directory"
-        dir_md5 = dirhash(dirpath, "md5")
-        pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
-        no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
-        ```
-        CLI:
-        ```commandline
-        dirhash path/to/directory -a md5
-        dirhash path/to/directory -a md5 --match "*.py"
-        dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
-        ```
-        
-        ## Why?
-        If you (or your application) need to verify the integrity of a set of files as well
-        as their name and location, you might find this useful. Use-cases range from 
-        verification of your image classification dataset (before spending GPU-$$$ on 
-        training your fancy Deep Learning model) to validation of generated files in
-        regression-testing.
-        
-        There isn't really a standard way of doing this. There are plenty of recipes out 
-        there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-        and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
-        but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
-        and documented with a compelling user interface. `dirhash` was created with this as 
-        the goal.
-        
-        [checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
-        module/tool with similar intent (that inspired this project) but it lacks much of the
-        functionality offered here (most notably including file names/structure in the hash)
-        and lacks tests.
-        
-        ## Performance
-        The python `hashlib` implementation of common hashing algorithms are highly
-        optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
-        combines the output. Reasonable measures have been taken to minimize the overhead 
-        and for common use-cases, the majority of time is spent reading data from disk 
-        and executing `hashlib` code.
-        
-        The main effort to boost performance is support for multiprocessing, where the
-        reading and hashing is parallelized over individual files.
-        
-        As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
-        with the shell command:
-        
-        `find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
-        
-        which is the top answer for the SO-question: 
-        [Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-        Results for two test cases are shown below. Both have 1 GiB of random data: in 
-        "flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
-        "nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
-        in a binary tree of depth 8.
-        
-        Implementation      | Test Case       | Time (s) | Speed up
-        ------------------- | --------------- | -------: | -------:
-        shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
-        `dirhash`           | flat_1k_1MB     | 1.67     | 1.36
-        `dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
-        shell reference     | nested_32k_32kB | 6.82     | -> 1.0
-        `dirhash`           | nested_32k_32kB | 3.43     | 2.00
-        `dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
-        
-        The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
-        
-        ## Documentation
-        Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scantree>=0.0.2
+Requires-Dist: pathspec<0.10.0
+
+
+[![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
+
+# dirhash
+A lightweight python module and CLI for computing the hash of any
+directory based on its files' structure and content.
+- Supports all hashing algorithms of Python's built-in `hashlib` module.
+- Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
+- Multiprocessing for up to [6x speed-up](#performance)
+
+The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
+
+## Installation
+From PyPI:
+```commandline
+pip install dirhash
+```
+Or directly from source:
+```commandline
+git clone git@github.com:andhus/dirhash-python.git
+pip install dirhash/
+```
+
+## Usage
+Python module:
+```python
+from dirhash import dirhash
+
+dirpath = "path/to/directory"
+dir_md5 = dirhash(dirpath, "md5")
+pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
+no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
+```
+CLI:
+```commandline
+dirhash path/to/directory -a md5
+dirhash path/to/directory -a md5 --match "*.py"
+dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
+```
+
+## Why?
+If you (or your application) need to verify the integrity of a set of files as well
+as their name and location, you might find this useful. Use-cases range from 
+verification of your image classification dataset (before spending GPU-$$$ on 
+training your fancy Deep Learning model) to validation of generated files in
+regression-testing.
+
+There isn't really a standard way of doing this. There are plenty of recipes out 
+there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
+and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
+but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
+and documented with a compelling user interface. `dirhash` was created with this as 
+the goal.
+
+[checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
+module/tool with similar intent (that inspired this project) but it lacks much of the
+functionality offered here (most notably including file names/structure in the hash)
+and lacks tests.
+
+## Performance
+The python `hashlib` implementation of common hashing algorithms are highly
+optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
+combines the output. Reasonable measures have been taken to minimize the overhead 
+and for common use-cases, the majority of time is spent reading data from disk 
+and executing `hashlib` code.
+
+The main effort to boost performance is support for multiprocessing, where the
+reading and hashing is parallelized over individual files.
+
+As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
+with the shell command:
+
+`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
+
+which is the top answer for the SO-question: 
+[Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
+Results for two test cases are shown below. Both have 1 GiB of random data: in 
+"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
+"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
+in a binary tree of depth 8.
+
+Implementation      | Test Case       | Time (s) | Speed up
+------------------- | --------------- | -------: | -------:
+shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
+`dirhash`           | flat_1k_1MB     | 1.67     | 1.36
+`dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
+shell reference     | nested_32k_32kB | 6.82     | -> 1.0
+`dirhash`           | nested_32k_32kB | 3.43     | 2.00
+`dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
+
+The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
+
+## Documentation
+Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

### Comparing `dirhash-0.2.1/README.md` & `dirhash-0.3.0a0/src/dirhash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-[![Build Status](https://travis-ci.com/andhus/dirhash-python.svg?branch=master)](https://travis-ci.com/andhus/dirhash-python)
+Metadata-Version: 2.1
+Name: dirhash
+Version: 0.3.0a0
+Summary: Python module and CLI for hashing of file system directories.
+Home-page: https://github.com/andhus/dirhash-python
+Author: Anders Huss
+Author-email: andhus@kth.se
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scantree>=0.0.2
+Requires-Dist: pathspec<0.10.0
+
+
 [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
 
 # dirhash
 A lightweight python module and CLI for computing the hash of any
 directory based on its files' structure and content.
 - Supports all hashing algorithms of Python's built-in `hashlib` module.
 - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
@@ -87,8 +100,8 @@
 shell reference     | nested_32k_32kB | 6.82     | -> 1.0
 `dirhash`           | nested_32k_32kB | 3.43     | 2.00
 `dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
 
 The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
 
 ## Documentation
-Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
+Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

### Comparing `dirhash-0.2.1/setup.py` & `dirhash-0.3.0a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 import io
 import os
 from setuptools import setup, find_packages
 
-PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
+import versioneer
 
-version = {}
-with io.open(os.path.join(PROJECT_ROOT, "src", "dirhash", "version.py")) as fp:
-    exec(fp.read(), version)
+PROJECT_ROOT = os.path.abspath(os.path.dirname(__file__))
 
 DESCRIPTION = 'Python module and CLI for hashing of file system directories.'
 
 try:
     with io.open(os.path.join(PROJECT_ROOT, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except IOError:
     long_description = DESCRIPTION
 
 setup(
     name='dirhash',
-    version=version['__version__'],
+    version=versioneer.get_version(),
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/andhus/dirhash-python',
     author="Anders Huss",
     author_email="andhus@kth.se",
     license='MIT',
-    install_requires=['scantree>=0.0.1'],
+    install_requires=['scantree>=0.0.2', 'pathspec<0.10.0'],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     include_package_data=True,
     entry_points={
         'console_scripts': ['dirhash=dirhash.cli:main'],
     },
     tests_require=['pytest', 'pytest-cov']
```

### Comparing `dirhash-0.2.1/src/dirhash/__init__.py` & `dirhash-0.3.0a0/src/dirhash/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 """dirhash - a python library (and CLI) for hashing of file system directories.
 """
 from __future__ import print_function, division
 
 import os
 import hashlib
-import pkg_resources
 
 from functools import partial
 from multiprocessing import Pool
 
 from scantree import (
     scantree,
     RecursionFilter,
     CyclicLinkedDir,
 )
 
-from dirhash.version import __version__
+from . import _version
+__version__ = _version.get_versions()['version']
 
 __all__ = [
     '__version__',
     'algorithms_guaranteed',
     'algorithms_available',
     'dirhash',
     'dirhash_impl',
```

### Comparing `dirhash-0.2.1/src/dirhash/cli.py` & `dirhash-0.3.0a0/src/dirhash/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,26 +76,26 @@
     filter_options.add_argument(
         '-m', '--match',
         nargs='+',
         default=['*'],
         help=(
             'One or several patterns for paths to include. NOTE: patterns '
             'with an asterisk must be in quotes ("*") or the asterisk '
-            'preceded by an escape character (\*).'
+            'preceded by an escape character (`*).'
         ),
         metavar=''
     )
     filter_options.add_argument(
         '-i', '--ignore',
         nargs='+',
         default=None,
         help=(
             'One or several patterns for paths to exclude. NOTE: patterns '
             'with an asterisk must be in quotes ("*") or the asterisk '
-            'preceded by an escape character (\*).'
+            'preceded by an escape character (`*).'
         ),
         metavar=''
     )
     filter_options.add_argument(
         '--empty-dirs',
         action='store_true',
         default=False,
```

### Comparing `dirhash-0.2.1/src/dirhash.egg-info/PKG-INFO` & `dirhash-0.3.0a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,93 @@
-Metadata-Version: 2.1
-Name: dirhash
-Version: 0.2.1
-Summary: Python module and CLI for hashing of file system directories.
-Home-page: https://github.com/andhus/dirhash-python
-Author: Anders Huss
-Author-email: andhus@kth.se
-License: MIT
-Description: 
-        [![Build Status](https://travis-ci.com/andhus/dirhash-python.svg?branch=master)](https://travis-ci.com/andhus/dirhash-python)
-        [![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
-        
-        # dirhash
-        A lightweight python module and CLI for computing the hash of any
-        directory based on its files' structure and content.
-        - Supports all hashing algorithms of Python's built-in `hashlib` module.
-        - Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
-        - Multiprocessing for up to [6x speed-up](#performance)
-        
-        The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
-        
-        ## Installation
-        From PyPI:
-        ```commandline
-        pip install dirhash
-        ```
-        Or directly from source:
-        ```commandline
-        git clone git@github.com:andhus/dirhash-python.git
-        pip install dirhash/
-        ```
-        
-        ## Usage
-        Python module:
-        ```python
-        from dirhash import dirhash
-        
-        dirpath = "path/to/directory"
-        dir_md5 = dirhash(dirpath, "md5")
-        pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
-        no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
-        ```
-        CLI:
-        ```commandline
-        dirhash path/to/directory -a md5
-        dirhash path/to/directory -a md5 --match "*.py"
-        dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
-        ```
-        
-        ## Why?
-        If you (or your application) need to verify the integrity of a set of files as well
-        as their name and location, you might find this useful. Use-cases range from 
-        verification of your image classification dataset (before spending GPU-$$$ on 
-        training your fancy Deep Learning model) to validation of generated files in
-        regression-testing.
-        
-        There isn't really a standard way of doing this. There are plenty of recipes out 
-        there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-        and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
-        but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
-        and documented with a compelling user interface. `dirhash` was created with this as 
-        the goal.
-        
-        [checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
-        module/tool with similar intent (that inspired this project) but it lacks much of the
-        functionality offered here (most notably including file names/structure in the hash)
-        and lacks tests.
-        
-        ## Performance
-        The python `hashlib` implementation of common hashing algorithms are highly
-        optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
-        combines the output. Reasonable measures have been taken to minimize the overhead 
-        and for common use-cases, the majority of time is spent reading data from disk 
-        and executing `hashlib` code.
-        
-        The main effort to boost performance is support for multiprocessing, where the
-        reading and hashing is parallelized over individual files.
-        
-        As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
-        with the shell command:
-        
-        `find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
-        
-        which is the top answer for the SO-question: 
-        [Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
-        Results for two test cases are shown below. Both have 1 GiB of random data: in 
-        "flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
-        "nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
-        in a binary tree of depth 8.
-        
-        Implementation      | Test Case       | Time (s) | Speed up
-        ------------------- | --------------- | -------: | -------:
-        shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
-        `dirhash`           | flat_1k_1MB     | 1.67     | 1.36
-        `dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
-        shell reference     | nested_32k_32kB | 6.82     | -> 1.0
-        `dirhash`           | nested_32k_32kB | 3.43     | 2.00
-        `dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
-        
-        The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
-        
-        ## Documentation
-        Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+[![codecov](https://codecov.io/gh/andhus/dirhash-python/branch/master/graph/badge.svg)](https://codecov.io/gh/andhus/dirhash-python)
+
+# dirhash
+A lightweight python module and CLI for computing the hash of any
+directory based on its files' structure and content.
+- Supports all hashing algorithms of Python's built-in `hashlib` module.
+- Glob/wildcard (".gitignore style") path matching for expressive filtering of files to include/exclude.
+- Multiprocessing for up to [6x speed-up](#performance)
+
+The hash is computed according to the [Dirhash Standard](https://github.com/andhus/dirhash), which is designed to allow for consistent and collision resistant generation/verification of directory hashes across implementations.
+
+## Installation
+From PyPI:
+```commandline
+pip install dirhash
+```
+Or directly from source:
+```commandline
+git clone git@github.com:andhus/dirhash-python.git
+pip install dirhash/
+```
+
+## Usage
+Python module:
+```python
+from dirhash import dirhash
+
+dirpath = "path/to/directory"
+dir_md5 = dirhash(dirpath, "md5")
+pyfiles_md5 = dirhash(dirpath, "md5", match=["*.py"])
+no_hidden_sha1 = dirhash(dirpath, "sha1", ignore=[".*", ".*/"])
+```
+CLI:
+```commandline
+dirhash path/to/directory -a md5
+dirhash path/to/directory -a md5 --match "*.py"
+dirhash path/to/directory -a sha1 --ignore ".*"  ".*/"
+```
+
+## Why?
+If you (or your application) need to verify the integrity of a set of files as well
+as their name and location, you might find this useful. Use-cases range from 
+verification of your image classification dataset (before spending GPU-$$$ on 
+training your fancy Deep Learning model) to validation of generated files in
+regression-testing.
+
+There isn't really a standard way of doing this. There are plenty of recipes out 
+there (see e.g. these SO-questions for [linux](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
+and [python](https://stackoverflow.com/questions/24937495/how-can-i-calculate-a-hash-for-a-filesystem-directory-using-python))
+but I couldn't find one that is properly tested (there are some gotcha:s to cover!) 
+and documented with a compelling user interface. `dirhash` was created with this as 
+the goal.
+
+[checksumdir](https://github.com/cakepietoast/checksumdir) is another python 
+module/tool with similar intent (that inspired this project) but it lacks much of the
+functionality offered here (most notably including file names/structure in the hash)
+and lacks tests.
+
+## Performance
+The python `hashlib` implementation of common hashing algorithms are highly
+optimised. `dirhash` mainly parses the file tree, pipes data to `hashlib` and 
+combines the output. Reasonable measures have been taken to minimize the overhead 
+and for common use-cases, the majority of time is spent reading data from disk 
+and executing `hashlib` code.
+
+The main effort to boost performance is support for multiprocessing, where the
+reading and hashing is parallelized over individual files.
+
+As a reference, let's compare the performance of the `dirhash` [CLI](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/cli.py) 
+with the shell command:
+
+`find path/to/folder -type f -print0 | sort -z | xargs -0 md5 | md5` 
+
+which is the top answer for the SO-question: 
+[Linux: compute a single hash for a given folder & contents?](https://stackoverflow.com/questions/545387/linux-compute-a-single-hash-for-a-given-folder-contents)
+Results for two test cases are shown below. Both have 1 GiB of random data: in 
+"flat_1k_1MB", split into 1k files (1 MiB each) in a flat structure, and in 
+"nested_32k_32kB", into 32k files (32 KiB each) spread over the 256 leaf directories 
+in a binary tree of depth 8.
+
+Implementation      | Test Case       | Time (s) | Speed up
+------------------- | --------------- | -------: | -------:
+shell reference     | flat_1k_1MB     | 2.29     | -> 1.0
+`dirhash`           | flat_1k_1MB     | 1.67     | 1.36
+`dirhash`(8 workers)| flat_1k_1MB     | 0.48     | **4.73**
+shell reference     | nested_32k_32kB | 6.82     | -> 1.0
+`dirhash`           | nested_32k_32kB | 3.43     | 2.00
+`dirhash`(8 workers)| nested_32k_32kB | 1.14     | **6.00**
+
+The benchmark was run a MacBook Pro (2018), further details and source code [here](https://github.com/andhus/dirhash-python/tree/master/benchmark).
+
+## Documentation
+Please refer to `dirhash -h`, the python [source code](https://github.com/andhus/dirhash-python/blob/master/src/dirhash/__init__.py) and the [Dirhash Standard](https://github.com/andhus/dirhash).
```

