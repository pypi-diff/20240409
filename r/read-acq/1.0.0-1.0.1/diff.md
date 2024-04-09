# Comparing `tmp/read_acq-1.0.0.tar.gz` & `tmp/read_acq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_acq-1.0.0.tar", last modified: Mon Feb 12 18:05:57 2024, max compression
+gzip compressed data, was "read_acq-1.0.1.tar", last modified: Tue Apr  9 14:22:48 2024, max compression
```

## Comparing `read_acq-1.0.0.tar` & `read_acq-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.029199 read_acq-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-02-12 18:05:46.000000 read_acq-1.0.0/.coverage
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-12 18:05:46.000000 read_acq-1.0.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.021200 read_acq-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.025200 read_acq-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/auto-merge-deps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/release-draft.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-02-12 18:05:46.000000 read_acq-1.0.0/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-12 18:05:46.000000 read_acq-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-12 18:05:46.000000 read_acq-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-12 18:05:46.000000 read_acq-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-12 18:05:46.000000 read_acq-1.0.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-12 18:05:57.029199 read_acq-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-12 18:05:46.000000 read_acq-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-12 18:05:46.000000 read_acq-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-12 18:05:57.029199 read_acq-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-12 18:05:46.000000 read_acq-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.021200 read_acq-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.025200 read_acq-1.0.0/src/read_acq/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/decode.c
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/gsdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-02-12 18:05:46.000000 read_acq-1.0.0/src/read_acq/read_acq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.029199 read_acq-1.0.0/src/read_acq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-12 18:05:57.000000 read_acq-1.0.0/src/read_acq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 18:05:56.000000 read_acq-1.0.0/src/read_acq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.025200 read_acq-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:05:57.029199 read_acq-1.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   393687 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/data/pxspec.acq
--rw-r--r--   0 runner    (1001) docker     (127)   656907 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/data/sample.acq
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-12 18:05:46.000000 read_acq-1.0.0/tests/test_gsh5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.848219 read_acq-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    77824 2024-04-09 14:22:43.000000 read_acq-1.0.1/.coverage
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-09 14:22:43.000000 read_acq-1.0.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.840220 read_acq-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.844220 read_acq-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/auto-merge-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/check-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/release-draft.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-09 14:22:43.000000 read_acq-1.0.1/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-09 14:22:43.000000 read_acq-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 14:22:43.000000 read_acq-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-09 14:22:43.000000 read_acq-1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-09 14:22:43.000000 read_acq-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-09 14:22:48.848219 read_acq-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-09 14:22:43.000000 read_acq-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-09 14:22:43.000000 read_acq-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:22:48.848219 read_acq-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 14:22:43.000000 read_acq-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.840220 read_acq-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.844220 read_acq-1.0.1/src/read_acq/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/decode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/gsdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14772 2024-04-09 14:22:43.000000 read_acq-1.0.1/src/read_acq/read_acq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.848219 read_acq-1.0.1/src/read_acq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 14:22:48.000000 read_acq-1.0.1/src/read_acq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.844220 read_acq-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:22:48.844220 read_acq-1.0.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   393687 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/data/pxspec.acq
+-rw-r--r--   0 runner    (1001) docker     (127)   656907 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/data/sample.acq
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 14:22:43.000000 read_acq-1.0.1/tests/test_gsh5.py
```

### Comparing `read_acq-1.0.0/.coveragerc` & `read_acq-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/.github/labels.yml` & `read_acq-1.0.1/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/.github/workflows/check-build.yml` & `read_acq-1.0.1/.github/workflows/check-build.yml`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/.github/workflows/deploy.yaml` & `read_acq-1.0.1/.github/workflows/deploy.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         run: pip install build
 
       - name: Build a binary wheel
         run: |
           python -m build -s .
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.12
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `read_acq-1.0.0/.github/workflows/test_suite.yaml` & `read_acq-1.0.1/.github/workflows/test_suite.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -119,7 +119,8 @@
           coverage xml
 
       - uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
           verbose: true
           file: ./coverage.xml
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `read_acq-1.0.0/CHANGELOG.md` & `read_acq-1.0.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/LICENSE.rst` & `read_acq-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/PKG-INFO` & `read_acq-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,87 @@
 Metadata-Version: 2.1
 Name: read_acq
-Version: 1.0.0
+Version: 1.0.1
 Summary: Read/Write ACQ Spectrum Files
-Home-page: https://github.com/edges-collab/read_acq
-Author: EDGES Team
-Author-email: steven.g.murray@asu.edu
+Author-email: Steven Murray <steven.murray@sns.it>
 License: MIT
-Platform: any
+Project-URL: Documentation, https://read-acq.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/edges-collab/edges-cal
+Project-URL: Issues, https://github.com/edges-collab/edges-cal/issues
+Project-URL: Changelog, https://github.com/edges-collab/edges-cal/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE.rst
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pygsdata
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: dev
-Requires-Dist: edges-io; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest>=5; extra == "dev"
-Provides-Extra: h5
-Requires-Dist: edges-io; extra == "h5"
-
-========
-read_acq
-========
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+
+# read-acq
+
 **Read EDGES ACQ spectrum files.**
 
-.. image:: https://travis-ci.org/edges-collab/read_acq.svg?branch=master
-    :target: https://travis-ci.org/edges-collab/read_acq
-.. image:: https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg
-    :target: https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
+[![image](https://travis-ci.org/edges-collab/read_acq.svg?branch=master)](https://travis-ci.org/edges-collab/read_acq)
+
+[![image](https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg)](https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq)
+
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Installation
-============
+## Installation
 
-In a new/existing python environment, run
-``pip install git+https://github.com/edges-collab/read_acq``.
+In a new/existing python environment, run `pip install
+git+https://github.com/edges-collab/read_acq`.
 
-If you wish to develop ``read_acq``, do the following::
+If you wish to develop `read_acq`, do the following:
 
     git clone https://github.com/edges-collab/read_acq
     cd read_acq
     pip install -e .
 
-Usage
-=====
+## Usage
 
-``read_acq`` can be used in a Python interpreter or directly via the command line.
+`read_acq` can be used in a Python interpreter or directly via the
+command line.
 
-CLI
----
+### CLI
 
 To use the CLI, a single command is provided:
 
-    acq convert <data.acq> [<data2.acq> ...] [-f format1 [-f format2]]
+> acq convert \<data.acq\> \[\<data2.acq\> ...\] \[-f format1 \[-f
+> format2\]\]
 
-This will convert the file(s) provided to all formats provided, and place any resulting
-files in the same location as the original datafile(s) (but with different extension).
-The default format is 'mat'.
-The command can be run from anywhere on the system, and the file given can be a
-relative or absolute path.
+This will convert the file(s) provided to all formats provided, and
+place any resulting files in the same location as the original
+datafile(s) (but with different extension). The default format is 'mat'.
+The command can be run from anywhere on the system, and the file given
+can be a relative or absolute path.
 
-Multiple data files can be given, and each will be converted. Wildcards may also be
-used in any of the filenames, eg.::
+Multiple data files can be given, and each will be converted. Wildcards
+may also be used in any of the filenames, eg.:
 
     acq convert data/*.acq
 
-Library
--------
+### Library
 
-The main point of entry for the Python interface is ``decode_file``::
+The main point of entry for the Python interface is `decode_file`:
 
     >>> from read_acq import decode_file
     >>> data = decode_file("my_data.acq", write_formats=[])
 
-By default, this function will also write the file in ``.mat`` format, but you can turn
-that off by providing ``write_formats=[]``. The output is a ``numpy`` array of the data.
-Several more options are provided, use ``help(decode_file)`` in an interpreter to see
-all the options.
+By default, this function will also write the file in `.mat` format, but
+you can turn that off by providing `write_formats=[]`. The output is a
+`numpy` array of the data. Several more options are provided, use
+`help(decode_file)` in an interpreter to see all the options.
```

### Comparing `read_acq-1.0.0/README.rst` & `read_acq-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,55 @@
-========
-read_acq
-========
+# read-acq
+
 **Read EDGES ACQ spectrum files.**
 
-.. image:: https://travis-ci.org/edges-collab/read_acq.svg?branch=master
-    :target: https://travis-ci.org/edges-collab/read_acq
-.. image:: https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg
-    :target: https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
+[![image](https://travis-ci.org/edges-collab/read_acq.svg?branch=master)](https://travis-ci.org/edges-collab/read_acq)
+
+[![image](https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg)](https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq)
+
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Installation
-============
+## Installation
 
-In a new/existing python environment, run
-``pip install git+https://github.com/edges-collab/read_acq``.
+In a new/existing python environment, run `pip install
+git+https://github.com/edges-collab/read_acq`.
 
-If you wish to develop ``read_acq``, do the following::
+If you wish to develop `read_acq`, do the following:
 
     git clone https://github.com/edges-collab/read_acq
     cd read_acq
     pip install -e .
 
-Usage
-=====
+## Usage
 
-``read_acq`` can be used in a Python interpreter or directly via the command line.
+`read_acq` can be used in a Python interpreter or directly via the
+command line.
 
-CLI
----
+### CLI
 
 To use the CLI, a single command is provided:
 
-    acq convert <data.acq> [<data2.acq> ...] [-f format1 [-f format2]]
+> acq convert \<data.acq\> \[\<data2.acq\> ...\] \[-f format1 \[-f
+> format2\]\]
 
-This will convert the file(s) provided to all formats provided, and place any resulting
-files in the same location as the original datafile(s) (but with different extension).
-The default format is 'mat'.
-The command can be run from anywhere on the system, and the file given can be a
-relative or absolute path.
+This will convert the file(s) provided to all formats provided, and
+place any resulting files in the same location as the original
+datafile(s) (but with different extension). The default format is 'mat'.
+The command can be run from anywhere on the system, and the file given
+can be a relative or absolute path.
 
-Multiple data files can be given, and each will be converted. Wildcards may also be
-used in any of the filenames, eg.::
+Multiple data files can be given, and each will be converted. Wildcards
+may also be used in any of the filenames, eg.:
 
     acq convert data/*.acq
 
-Library
--------
+### Library
 
-The main point of entry for the Python interface is ``decode_file``::
+The main point of entry for the Python interface is `decode_file`:
 
     >>> from read_acq import decode_file
     >>> data = decode_file("my_data.acq", write_formats=[])
 
-By default, this function will also write the file in ``.mat`` format, but you can turn
-that off by providing ``write_formats=[]``. The output is a ``numpy`` array of the data.
-Several more options are provided, use ``help(decode_file)`` in an interpreter to see
-all the options.
+By default, this function will also write the file in `.mat` format, but
+you can turn that off by providing `write_formats=[]`. The output is a
+`numpy` array of the data. Several more options are provided, use
+`help(decode_file)` in an interpreter to see all the options.
```

### Comparing `read_acq-1.0.0/src/read_acq/cli.py` & `read_acq-1.0.1/src/read_acq/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #! /usr/bin/env python
 """Command-Line Interface for read_acq."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 import click
 
 from .gsdata import read_acq_to_gsdata
@@ -24,17 +25,17 @@
 )
 @click.option(
     "-d",
     "--direc",
     default=".",
     type=click.Path(exists=True, file_okay=False),
 )
-@click.option("--site", "--loc", default="edges", type=str)
+@click.option("--telescope", "--loc", default="edges-low", type=str)
 @click.option("-n", "--name", default="{year}_{day}", type=str)
-def convert(infile, outfile: str | None, direc: str, site: str, name: str):
+def convert(infile, outfile: str | None, direc: str, telescope: str, name: str):
     """Convert an ACQ file to a .gsh5 format file.
 
     Multiple input files can be provided, and they will be joined together in a single
     output file. Furthermore, the input files can have glob-style patterns in them so
     that they expand to a list of files, e.g.:
 
         $ acq convert 2023_070*.acq
@@ -44,12 +45,12 @@
     """
     infiles = [Path(fl) for fl in infile]
 
     fls = []
     for fl in infiles:
         fls += sorted(fl.parent.glob(fl.name))
 
-    gsd = read_acq_to_gsdata(fls, telescope_location=site, name=name)
+    gsd = read_acq_to_gsdata(fls, telescope=telescope, name=name)
     if outfile is None:
         outfile = f"{gsd.name}.gsh5"
 
     gsd.write_gsh5(Path(direc) / outfile)
```

### Comparing `read_acq-1.0.0/src/read_acq/codec.py` & `read_acq-1.0.1/src/read_acq/codec.py`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/src/read_acq/decode.c` & `read_acq-1.0.1/src/read_acq/decode.c`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/src/read_acq/gsdata.py` & `read_acq-1.0.1/src/read_acq/gsdata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Read an ACQ file into a GSData object."""
+
 from __future__ import annotations
 
 from collections.abc import Sequence
 from pathlib import Path
 
 import numpy as np
 from astropy import units as un
-from astropy.coordinates import EarthLocation, UnknownSiteException
 from astropy.time import Time
-from pygsdata import GSData
-from pygsdata.constants import KNOWN_LOCATIONS
+from pygsdata import KNOWN_TELESCOPES, GSData, Telescope
+from pygsdata.readers import gsdata_reader
+from pygsdata.utils import time_concat
 
 from .read_acq import ACQError, decode_file, encode
 
 
+@gsdata_reader(select_on_read=False, formats=["acq"])
 def read_acq_to_gsdata(
     path: str | Path | Sequence[str | Path],
-    telescope_location: str | EarthLocation,
+    telescope: Telescope = KNOWN_TELESCOPES["edges-low"],
     name: str = "{year}-{day}:{hour}:{minute}",
     **kwargs,
 ) -> GSData:
     """Read an ACQ file into a GSData object.
 
     Parameters
     ----------
@@ -36,55 +38,52 @@
         Additional keyword arguments to pass to the GSData constructor.
     """
     path = [Path(path)] if isinstance(path, (str, Path)) else [Path(p) for p in path]
 
     if not all(p.exists() for p in path):
         raise FileNotFoundError(f"File {path} does not exist")
 
-    if isinstance(telescope_location, str):
+    if isinstance(telescope, str):
         try:
-            telescope_location = EarthLocation.of_site(telescope_location)
-        except UnknownSiteException as e:
-            try:
-                telescope_location = KNOWN_LOCATIONS[telescope_location]
-            except KeyError:
-                raise ValueError(
-                    "telescope_location must be an EarthLocation or a known site, "
-                    f"got {telescope_location}. Known sites are {KNOWN_LOCATIONS}."
-                ) from e
+            telescope = KNOWN_TELESCOPES[telescope]
+        except KeyError as e:
+            raise ValueError(
+                "telescope must be a Telescope or name of a KNOWN_TELESCOPE, "
+                f"got {telescope}. Known 'scopes are {KNOWN_TELESCOPES.keys()}."
+            ) from e
 
     # Read the _first_ file to get the metadata
     _, (pant, pload, plns), anc = decode_file(path[0], meta=True)
     times = Time(anc.data.pop("times"), format="yday", scale="utc")
 
     # Concatenate all the files
     for p in path[1:]:
         _, (pant_, pload_, plns_), anc_ = decode_file(p, meta=True)
         times_ = Time(anc_.data.pop("times"), format="yday", scale="utc")
 
         pant = np.concatenate((pant, pant_), axis=1)
         pload = np.concatenate((pload, pload_), axis=1)
         plns = np.concatenate((plns, plns_), axis=1)
-        times = np.concatenate((times, times_))
+        times = time_concat((times, times_))
         anc.data = {k: np.concatenate((v, anc_.data[k])) for k, v in anc.data.items()}
 
     if pant.size == 0:
         raise ACQError(f"No data in any files: {path}")
 
     year, day, hour, minute = times[0, 0].to_value("yday", "date_hm").split(":")
     name = name.format(year=year, day=day, hour=hour, minute=minute, stem=path[0].stem)
     return GSData(
         data=np.array([pant.T, pload.T, plns.T])[:, np.newaxis],
-        time_array=times,
-        freq_array=anc.frequencies * un.MHz,
+        times=times,
+        freqs=anc.frequencies * un.MHz,
         data_unit="power",
         loads=("ant", "internal_load", "internal_load_plus_noise_source"),
         auxiliary_measurements={name: anc.data[name] for name in anc.data},
         filename=path[0] if len(path) == 1 else None,
-        telescope_location=telescope_location,
+        telescope=telescope,
         name=name,
         **kwargs,
     )
 
 
 def write_gsdata_to_acq(
     gsdata: GSData,
@@ -105,22 +104,22 @@
     nblk : int
         The number of blocks in the data.
     """
     if gsdata.nloads != 3:
         raise ValueError("Can only encode 3-load data to ACQ file.")
 
     ancillary = {
-        "times": gsdata.time_array.strftime("%Y:%j:%H:%M:%S"),
+        "times": gsdata.times.strftime("%Y:%j:%H:%M:%S"),
         "adcmax": gsdata.auxiliary_measurements["adcmax"],
         "adcmin": gsdata.auxiliary_measurements["adcmin"],
     }
 
     meta = {
         "temperature": temperature,
         "nblk": nblk,
-        "nfreq": len(gsdata.freq_array),
-        "freq_min": gsdata.freq_array.min().to_value("MHz"),
-        "freq_max": gsdata.freq_array.max().to_value("MHz"),
-        "freq_res": (gsdata.freq_array[1] - gsdata.freq_array[0]).to_value("MHz"),
+        "nfreq": gsdata.nfreqs,
+        "freq_min": gsdata.freqs.min().to_value("MHz"),
+        "freq_max": gsdata.freqs.max().to_value("MHz"),
+        "freq_res": (gsdata.freqs[1] - gsdata.freqs[0]).to_value("MHz"),
     }
 
     encode(outfile, p=gsdata.data[:, 0], meta=meta, ancillary=ancillary)
```

### Comparing `read_acq-1.0.0/src/read_acq/read_acq.py` & `read_acq-1.0.1/src/read_acq/read_acq.py`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/src/read_acq.egg-info/PKG-INFO` & `read_acq-1.0.1/src/read_acq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,87 @@
 Metadata-Version: 2.1
 Name: read_acq
-Version: 1.0.0
+Version: 1.0.1
 Summary: Read/Write ACQ Spectrum Files
-Home-page: https://github.com/edges-collab/read_acq
-Author: EDGES Team
-Author-email: steven.g.murray@asu.edu
+Author-email: Steven Murray <steven.murray@sns.it>
 License: MIT
-Platform: any
+Project-URL: Documentation, https://read-acq.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/edges-collab/edges-cal
+Project-URL: Issues, https://github.com/edges-collab/edges-cal/issues
+Project-URL: Changelog, https://github.com/edges-collab/edges-cal/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE.rst
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pygsdata
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: dev
-Requires-Dist: edges-io; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest>=5; extra == "dev"
-Provides-Extra: h5
-Requires-Dist: edges-io; extra == "h5"
-
-========
-read_acq
-========
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+
+# read-acq
+
 **Read EDGES ACQ spectrum files.**
 
-.. image:: https://travis-ci.org/edges-collab/read_acq.svg?branch=master
-    :target: https://travis-ci.org/edges-collab/read_acq
-.. image:: https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg
-    :target: https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
+[![image](https://travis-ci.org/edges-collab/read_acq.svg?branch=master)](https://travis-ci.org/edges-collab/read_acq)
+
+[![image](https://codecov.io/gh/edges-collab/read_acq/branch/master/graph/badge.svg)](https://travis-ci.org/edges-collabcodecov.io/gh/edges-collab/read_acq)
+
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-Installation
-============
+## Installation
 
-In a new/existing python environment, run
-``pip install git+https://github.com/edges-collab/read_acq``.
+In a new/existing python environment, run `pip install
+git+https://github.com/edges-collab/read_acq`.
 
-If you wish to develop ``read_acq``, do the following::
+If you wish to develop `read_acq`, do the following:
 
     git clone https://github.com/edges-collab/read_acq
     cd read_acq
     pip install -e .
 
-Usage
-=====
+## Usage
 
-``read_acq`` can be used in a Python interpreter or directly via the command line.
+`read_acq` can be used in a Python interpreter or directly via the
+command line.
 
-CLI
----
+### CLI
 
 To use the CLI, a single command is provided:
 
-    acq convert <data.acq> [<data2.acq> ...] [-f format1 [-f format2]]
+> acq convert \<data.acq\> \[\<data2.acq\> ...\] \[-f format1 \[-f
+> format2\]\]
 
-This will convert the file(s) provided to all formats provided, and place any resulting
-files in the same location as the original datafile(s) (but with different extension).
-The default format is 'mat'.
-The command can be run from anywhere on the system, and the file given can be a
-relative or absolute path.
+This will convert the file(s) provided to all formats provided, and
+place any resulting files in the same location as the original
+datafile(s) (but with different extension). The default format is 'mat'.
+The command can be run from anywhere on the system, and the file given
+can be a relative or absolute path.
 
-Multiple data files can be given, and each will be converted. Wildcards may also be
-used in any of the filenames, eg.::
+Multiple data files can be given, and each will be converted. Wildcards
+may also be used in any of the filenames, eg.:
 
     acq convert data/*.acq
 
-Library
--------
+### Library
 
-The main point of entry for the Python interface is ``decode_file``::
+The main point of entry for the Python interface is `decode_file`:
 
     >>> from read_acq import decode_file
     >>> data = decode_file("my_data.acq", write_formats=[])
 
-By default, this function will also write the file in ``.mat`` format, but you can turn
-that off by providing ``write_formats=[]``. The output is a ``numpy`` array of the data.
-Several more options are provided, use ``help(decode_file)`` in an interpreter to see
-all the options.
+By default, this function will also write the file in `.mat` format, but
+you can turn that off by providing `write_formats=[]`. The output is a
+`numpy` array of the data. Several more options are provided, use
+`help(decode_file)` in an interpreter to see all the options.
```

### Comparing `read_acq-1.0.0/src/read_acq.egg-info/SOURCES.txt` & `read_acq-1.0.1/src/read_acq.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 .coverage
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
-LICENSE.rst
-README.rst
+LICENSE.txt
+README.md
 pyproject.toml
-setup.cfg
 setup.py
 .github/dependabot.yml
 .github/labels.yml
 .github/release-drafter.yml
 .github/workflows/auto-merge-deps.yml
 .github/workflows/check-build.yml
 .github/workflows/deploy.yaml
@@ -23,15 +22,14 @@
 src/read_acq/decode.c
 src/read_acq/gsdata.py
 src/read_acq/read_acq.py
 src/read_acq.egg-info/PKG-INFO
 src/read_acq.egg-info/SOURCES.txt
 src/read_acq.egg-info/dependency_links.txt
 src/read_acq.egg-info/entry_points.txt
-src/read_acq.egg-info/not-zip-safe
 src/read_acq.egg-info/requires.txt
 src/read_acq.egg-info/top_level.txt
 tests/conftest.py
 tests/test_cli.py
 tests/test_encoding.py
 tests/test_gsh5.py
 tests/data/pxspec.acq
```

### Comparing `read_acq-1.0.0/tests/data/pxspec.acq` & `read_acq-1.0.1/tests/data/pxspec.acq`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/tests/data/sample.acq` & `read_acq-1.0.1/tests/data/sample.acq`

 * *Files identical despite different names*

### Comparing `read_acq-1.0.0/tests/test_cli.py` & `read_acq-1.0.1/tests/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of the CLI."""
+
 from pathlib import Path
 
 import numpy as np
 from click.testing import CliRunner
 from pygsdata import GSData
 from read_acq import decode_file
 from read_acq.cli import convert
```

### Comparing `read_acq-1.0.0/tests/test_encoding.py` & `read_acq-1.0.1/tests/test_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests of writing ACQ files."""
+
 from pathlib import Path
 
 import numpy as np
 import pytest
 from read_acq import decode_file, encode
 from read_acq.codec import _decode_line, _encode, _encode_line
 from read_acq.read_acq import (
```

