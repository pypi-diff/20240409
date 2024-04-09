# Comparing `tmp/invenio-subjects-lcsh-2023.11.2.tar.gz` & `tmp/invenio-subjects-lcsh-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-subjects-lcsh-2023.11.2.tar", last modified: Thu Mar 21 20:10:55 2024, max compression
+gzip compressed data, was "invenio-subjects-lcsh-2024.1.0.tar", last modified: Tue Apr  9 18:06:08 2024, max compression
```

## Comparing `invenio-subjects-lcsh-2023.11.2.tar` & `invenio-subjects-lcsh-2024.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.526426 invenio-subjects-lcsh-2023.11.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.530426 invenio-subjects-lcsh-2023.11.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.530426 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127) 62781366 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/vocabularies/subjects_lcsh.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh/vocabularies/vocabularies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 20:10:55.000000 invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 20:10:55.606425 invenio-subjects-lcsh-2023.11.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-21 20:03:51.000000 invenio-subjects-lcsh-2023.11.2/tests/test_invenio_subjects_lcsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.564359 invenio-subjects-lcsh-2024.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.568359 invenio-subjects-lcsh-2024.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.568359 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127) 40020881 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/vocabularies/subjects_lcsh.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh/vocabularies/vocabularies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 18:06:08.000000 invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 18:06:08.616359 invenio-subjects-lcsh-2024.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-09 18:04:23.000000 invenio-subjects-lcsh-2024.1.0/tests/test_invenio_subjects_lcsh.py
```

### Comparing `invenio-subjects-lcsh-2023.11.2/.editorconfig` & `invenio-subjects-lcsh-2024.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-subjects-lcsh-2023.11.2/.github/workflows/publish-to-pypi.yml` & `invenio-subjects-lcsh-2024.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `invenio-subjects-lcsh-2023.11.2/.github/workflows/run-tests.yml` & `invenio-subjects-lcsh-2024.1.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-subjects-lcsh-2023.11.2/LICENSE` & `invenio-subjects-lcsh-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-subjects-lcsh-2023.11.2/MANIFEST.in` & `invenio-subjects-lcsh-2024.1.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 #  check-manifest -u
 
 include .editorconfig
 recursive-include .github/workflows *.yml
 
 # added by check-manifest
 include *.md
-recursive-include invenio_subjects_lcsh *.jsonl
+recursive-include invenio_subjects_lcsh *.csv
 recursive-include invenio_subjects_lcsh *.yaml *.yml
 recursive-include tests *.py
```

### Comparing `invenio-subjects-lcsh-2023.11.2/invenio_subjects_lcsh.egg-info/SOURCES.txt` & `invenio-subjects-lcsh-2024.1.0/invenio_subjects_lcsh.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 invenio_subjects_lcsh.egg-info/PKG-INFO
 invenio_subjects_lcsh.egg-info/SOURCES.txt
 invenio_subjects_lcsh.egg-info/dependency_links.txt
 invenio_subjects_lcsh.egg-info/entry_points.txt
 invenio_subjects_lcsh.egg-info/requires.txt
 invenio_subjects_lcsh.egg-info/top_level.txt
 invenio_subjects_lcsh/vocabularies/__init__.py
-invenio_subjects_lcsh/vocabularies/subjects_lcsh.jsonl
+invenio_subjects_lcsh/vocabularies/subjects_lcsh.csv
 invenio_subjects_lcsh/vocabularies/vocabularies.yaml
 tests/test_invenio_subjects_lcsh.py
```

### Comparing `invenio-subjects-lcsh-2023.11.2/pyproject.toml` & `invenio-subjects-lcsh-2024.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,49 +13,42 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.10"
+]
+dependencies = [
+    "galter-subjects-utils>=0.4.1,<2.0",
 ]
-dependencies = []
 description = "LCSH subject terms for InvenioRDM"
-dynamic = ["version"]
 keywords = ["invenio", "inveniordm", "subjects", "LCSH"]
 license = {file = "LICENSE"}
 name = "invenio-subjects-lcsh"
 readme = "README.md"
 requires-python = ">=3.8"
 urls = {Repository = "https://github.com/galterlibrary/invenio-subjects-lcsh"}
+version = "2024.1.0"
 
 [project.optional-dependencies]
 dev = [
     "check-manifest>=0.49",
     "invoke>=2.2,<3.0",
-    "galter-subjects-utils>=0.2.0,<2.0",
     "pyyaml>=5.4.1",
-    "pytest>=7.2.0",
-    "pytest-cov>=3.0.0",
-    "pytest-isort>=3.0.0",
-    "pytest-pycodestyle>=2.2.0",
-    "pytest-pydocstyle>=2.2.3"
+    "pytest-invenio>=2.1.1,<3.0.0",
 ]
 
 [project.entry-points."invenio_rdm_records.fixtures"]
 invenio_subjects_lcsh = "invenio_subjects_lcsh.vocabularies"
 
 [tool.setuptools]
 packages = ["invenio_subjects_lcsh", "invenio_subjects_lcsh.vocabularies"]
 
-[tool.setuptools.dynamic]
-version = {attr = "invenio_subjects_lcsh.__version__"}
-
 [tool.check-manifest]
 ignore = [
     ".*-requirements.txt",
     "*.bin",
     "*.gitkeep",
     ".venv/",
     ".editorconfig",
```

### Comparing `invenio-subjects-lcsh-2023.11.2/tests/test_invenio_subjects_lcsh.py` & `invenio-subjects-lcsh-2024.1.0/tests/test_invenio_subjects_lcsh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Northwestern University.
+# Copyright (C) 2021-2024 Northwestern University.
 #
 # invenio-subjects-lcsh is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Test subjects extension conforms to subjects extension interface."""
 
 from pathlib import Path
 
 import pkg_resources
 import yaml
 
-from invenio_subjects_lcsh import __version__
-
-
-def test_version():
-    """Test version import."""
-    assert __version__
-
 
 def test_vocabularies_yaml():
     """Test vocabularies.yaml structure."""
     extensions = [
         ep.load() for ep in
         pkg_resources.iter_entry_points('invenio_rdm_records.fixtures')
     ]
```

