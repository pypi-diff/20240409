# Comparing `tmp/pycutest-1.6.1.tar.gz` & `tmp/pycutest-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutest-1.6.1.tar", last modified: Fri Mar  8 09:27:34 2024, max compression
+gzip compressed data, was "pycutest-1.6.2.tar", last modified: Tue Apr  9 07:31:03 2024, max compression
```

## Comparing `pycutest-1.6.1.tar` & `pycutest-1.6.2.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:27:34.451775 pycutest-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-08 09:27:34.000000 pycutest-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-03-08 09:27:34.451775 pycutest-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-03-08 09:27:34.000000 pycutest-1.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:27:34.451775 pycutest-1.6.1/pycutest/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/build_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    75292 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/c_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/install_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    45385 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/problem_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/python_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/sifdecode_extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/system_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 09:27:34.451775 pycutest-1.6.1/pycutest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 09:27:34.000000 pycutest-1.6.1/pycutest.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 09:27:34.451775 pycutest-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-08 09:27:34.000000 pycutest-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-09 07:30:57.000000 pycutest-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-09 07:31:03.615249 pycutest-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-09 07:30:57.000000 pycutest-1.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/pycutest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/build_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75292 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/install_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45385 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/problem_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/python_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11613 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/sifdecode_extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-09 07:30:57.000000 pycutest-1.6.2/pycutest/system_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:31:03.615249 pycutest-1.6.2/pycutest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 07:31:03.000000 pycutest-1.6.2/pycutest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-09 07:30:57.000000 pycutest-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:31:03.615249 pycutest-1.6.2/setup.cfg
```

### Comparing `pycutest-1.6.1/LICENSE` & `pycutest-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/PKG-INFO` & `pycutest-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python wrapper to the CUTEst optimization test environment
-Home-page: https://github.com/jfowkes/pycutest/
-Author: Jaroslav Fowkes and Lindon Roberts
-Author-email: jaroslav.fowkes@maths.ox.ac.uk
-License: GNU GPL
-Download-URL: https://github.com/jfowkes/pycutest/releases/
+Author-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
+Maintainer-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/jfowkes/pycutest/
+Project-URL: Download, https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
 Project-URL: Documentation, https://jfowkes.github.io/pycutest/
 Project-URL: Source Code, https://github.com/jfowkes/pycutest/
-Keywords: mathematics optimization
-Platform: UNKNOWN
+Keywords: mathematics,optimization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 ====================================================================================================================================
 PyCUTEst: A Python interface to the CUTEst Optimization Test Environment |License| |Build Status| |PyPI Version| |Downloads| |Paper|
 ====================================================================================================================================
 
 PyCUTEst is a Python interface to `CUTEst <https://github.com/ralna/CUTEst>`_, a Fortran package for testing optimization software. It is based on the `interface originally developed for CUTEr <http://fides.fe.uni-lj.si/~arpadb/software-pycuter.html>`_ by `Prof. Arpad Buermen <http://www.fe.uni-lj.si/en/the_faculty/staff/alphabetically/55/>`_.
 
@@ -197,9 +205,7 @@
                   :alt: PyPI version
 .. |Downloads| image:: https://static.pepy.tech/personalized-badge/pycutest?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads
                :target: https://pepy.tech/project/pycutest
                :alt: Total downloads
 .. |Paper| image:: https://joss.theoj.org/papers/10.21105/joss.04377/status.svg
            :target: https://doi.org/10.21105/joss.04377
            :alt: JOSS Paper
-
-
```

### Comparing `pycutest-1.6.1/README.rst` & `pycutest-1.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/__init__.py` & `pycutest-1.6.2/pycutest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# Ensure compatibility with Python 2
-from __future__ import absolute_import, division, print_function, unicode_literals
+# Set PyCUTEst version number
+__version__ = '1.6.2'
 
+# Define submodules to expose on wildcard imports
 __all__ = []
 
-from .version import __version__
-__all__ += ['__version__']
-
 from .build_interface import import_problem, clear_cache, all_cached_problems
 __all__ += ['import_problem', 'clear_cache', 'all_cached_problems']
 
 from .sifdecode_extras import print_available_sif_params, problem_properties, find_problems
 __all__ += ['print_available_sif_params', 'problem_properties', 'find_problems']
 
 from .problem_class import CUTEstProblem
```

### Comparing `pycutest-1.6.1/pycutest/build_interface.py` & `pycutest-1.6.2/pycutest/build_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/c_interface.py` & `pycutest-1.6.2/pycutest/c_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/install_scripts.py` & `pycutest-1.6.2/pycutest/install_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Installation scripts for individual problems
 """
 
 import sys
 
 from .system_paths import get_cutest_path
-from .version import __version__
+from pycutest import __version__
 
 __all__ = ['get_setup_script']
 
 #
 # The setup.py script with a placeholder for platform-dependent part.
 #
 setupScript="""#!/usr/bin/env python
```

### Comparing `pycutest-1.6.1/pycutest/problem_class.py` & `pycutest-1.6.2/pycutest/problem_class.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/python_interface.py` & `pycutest-1.6.2/pycutest/python_interface.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/sifdecode_extras.py` & `pycutest-1.6.2/pycutest/sifdecode_extras.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest/system_paths.py` & `pycutest-1.6.2/pycutest/system_paths.py`

 * *Files identical despite different names*

### Comparing `pycutest-1.6.1/pycutest.egg-info/PKG-INFO` & `pycutest-1.6.2/pycutest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: pycutest
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python wrapper to the CUTEst optimization test environment
-Home-page: https://github.com/jfowkes/pycutest/
-Author: Jaroslav Fowkes and Lindon Roberts
-Author-email: jaroslav.fowkes@maths.ox.ac.uk
-License: GNU GPL
-Download-URL: https://github.com/jfowkes/pycutest/releases/
+Author-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
+Maintainer-email: Jaroslav Fowkes <jaroslav.fowkes@maths.ox.ac.uk>, Lindon Roberts <lindon.roberts@sydney.edu.au>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/jfowkes/pycutest/
+Project-URL: Download, https://github.com/jfowkes/pycutest/releases/
 Project-URL: Bug Tracker, https://github.com/jfowkes/pycutest/issues/
 Project-URL: Documentation, https://jfowkes.github.io/pycutest/
 Project-URL: Source Code, https://github.com/jfowkes/pycutest/
-Keywords: mathematics optimization
-Platform: UNKNOWN
+Keywords: mathematics,optimization
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 ====================================================================================================================================
 PyCUTEst: A Python interface to the CUTEst Optimization Test Environment |License| |Build Status| |PyPI Version| |Downloads| |Paper|
 ====================================================================================================================================
 
 PyCUTEst is a Python interface to `CUTEst <https://github.com/ralna/CUTEst>`_, a Fortran package for testing optimization software. It is based on the `interface originally developed for CUTEr <http://fides.fe.uni-lj.si/~arpadb/software-pycuter.html>`_ by `Prof. Arpad Buermen <http://www.fe.uni-lj.si/en/the_faculty/staff/alphabetically/55/>`_.
 
@@ -197,9 +205,7 @@
                   :alt: PyPI version
 .. |Downloads| image:: https://static.pepy.tech/personalized-badge/pycutest?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads
                :target: https://pepy.tech/project/pycutest
                :alt: Total downloads
 .. |Paper| image:: https://joss.theoj.org/papers/10.21105/joss.04377/status.svg
            :target: https://doi.org/10.21105/joss.04377
            :alt: JOSS Paper
-
-
```

