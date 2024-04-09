# Comparing `tmp/user_util-1.0.0.tar.gz` & `tmp/user_util-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_util-1.0.0.tar", last modified: Tue Jan 19 17:26:05 2021, max compression
+gzip compressed data, was "user_util-1.1.0.tar", last modified: Tue Apr  9 15:53:28 2024, max compression
```

## Comparing `user_util-1.0.0.tar` & `user_util-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2021-01-19 17:25:07.000000 user_util-1.0.0/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3564 2021-01-19 17:25:07.000000 user_util-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      724 2021-01-19 17:25:07.000000 user_util-1.0.0/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    35135 2021-01-19 17:25:07.000000 user_util-1.0.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2021-01-19 17:25:07.000000 user_util-1.0.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2021-01-19 17:26:05.777871 user_util-1.0.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1001 2021-01-19 17:25:07.000000 user_util-1.0.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4845 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1176 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      771 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2021-01-19 17:25:07.000000 user_util-1.0.0/docs/usage.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-01-19 17:25:07.000000 user_util-1.0.0/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      473 2021-01-19 17:26:05.777871 user_util-1.0.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2087 2021-01-19 17:25:07.000000 user_util-1.0.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11175 2021-01-19 17:25:07.000000 user_util-1.0.0/tests/test_user_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/user_util/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-01-19 17:25:07.000000 user_util-1.0.0/user_util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2021-01-19 17:25:07.000000 user_util-1.0.0/user_util/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6000 2021-01-19 17:25:07.000000 user_util-1.0.0/user_util/user_util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-19 17:26:05.777871 user_util-1.0.0/user_util.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2967 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-01-19 17:26:05.000000 user_util-1.0.0/user_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.587677 user_util-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-09 15:53:24.000000 user_util-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 15:53:24.000000 user_util-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35135 2024-04-09 15:53:24.000000 user_util-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 15:53:24.000000 user_util-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 15:53:28.587677 user_util-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-09 15:53:24.000000 user_util-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.583677 user_util-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 15:53:24.000000 user_util-1.1.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.583677 user_util-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 15:53:24.000000 user_util-1.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 15:53:28.587677 user_util-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-09 15:53:24.000000 user_util-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.583677 user_util-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-09 15:53:24.000000 user_util-1.1.0/tests/test_user_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.587677 user_util-1.1.0/user_util/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 15:53:24.000000 user_util-1.1.0/user_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-09 15:53:24.000000 user_util-1.1.0/user_util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-09 15:53:24.000000 user_util-1.1.0/user_util/user_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:53:28.587677 user_util-1.1.0/user_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:53:28.000000 user_util-1.1.0/user_util.egg-info/top_level.txt
```

### Comparing `user_util-1.0.0/LICENSE` & `user_util-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/README.rst` & `user_util-1.1.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Open edX User Utilities
 =======================
 
 
 .. image:: https://img.shields.io/pypi/v/user-util.svg
         :target: https://pypi.python.org/pypi/user-util
 
-.. image:: https://img.shields.io/travis/edx/user-util.svg
-        :target: https://travis-ci.com/edx/user-util
+.. image:: https://github.com/openedx/user-util/workflows/Python%20CI/badge.svg?branch=master
+        :target: https://github.com/openedx/user-util/actions?query=workflow%3A%22Python+CI%22
 
 .. image:: https://readthedocs.org/projects/user-util/badge/?version=latest
         :target: https://user-util.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
```

### Comparing `user_util-1.0.0/docs/Makefile` & `user_util-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/docs/conf.py` & `user_util-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/docs/installation.rst` & `user_util-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/docs/make.bat` & `user_util-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/setup.py` & `user_util-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
+import os
+import re
+
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
@@ -34,24 +37,43 @@
 def is_requirement(line):
     """
     Return True if the requirement line is a package requirement;
     that is, it is not blank, a comment, a URL, or an included file.
     """
     return line and not line.startswith(('-r', '#', '-e', 'git+', '-c'))
 
+
+def get_version(*file_paths):
+    """
+    Extract the version string from the file at the given relative path fragments.
+    """
+    filename = os.path.join(os.path.dirname(__file__), *file_paths)
+    with open(filename, encoding='utf-8') as opened_file:
+        version_file = opened_file.read()
+        version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
+                                  version_file, re.M)
+    if version_match:
+        return version_match.group(1)
+    raise RuntimeError('Unable to find version string.')
+
+
+VERSION = get_version("user_util", "__init__.py")
+
+
 setup(
     author="edX",
     author_email='oscm@edx.org',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
     ],
     description="User utilities for the Open edX platform",
     entry_points={
         'console_scripts': [
             'user_util=user_util.cli:retire_user',
         ],
     },
@@ -61,11 +83,11 @@
     include_package_data=True,
     keywords='user_util',
     name='user_util',
     packages=find_packages(include=['user_util']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/edx/user-util',
-    version='1.0.0',
+    url='https://github.com/openedx/user-util',
+    version=VERSION,
     zip_safe=False,
 )
```

### Comparing `user_util-1.0.0/tests/test_user_util.py` & `user_util-1.1.0/tests/test_user_util.py`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/user_util/cli.py` & `user_util-1.1.0/user_util/cli.py`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/user_util/user_util.py` & `user_util-1.1.0/user_util/user_util.py`

 * *Files identical despite different names*

### Comparing `user_util-1.0.0/user_util.egg-info/SOURCES.txt` & `user_util-1.1.0/user_util.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 AUTHORS.rst
-CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/Makefile
```

