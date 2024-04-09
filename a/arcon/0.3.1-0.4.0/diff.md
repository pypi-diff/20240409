# Comparing `tmp/arcon-0.3.1.tar.gz` & `tmp/arcon-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcon-0.3.1.tar", max compression
+gzip compressed data, was "arcon-0.4.0.tar", max compression
```

## Comparing `arcon-0.3.1.tar` & `arcon-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-08-12 07:56:57.178613 arcon-0.3.1/LICENSE
--rw-r--r--   0        0        0     3095 2023-09-17 08:18:42.974526 arcon-0.3.1/README.rst
--rw-r--r--   0        0        0     6504 2023-11-26 04:41:45.169843 arcon-0.3.1/arcon/__init__.py
--rw-r--r--   0        0        0      208 2023-11-26 04:41:45.365625 arcon-0.3.1/arcon/_version.py
--rw-r--r--   0        0        0        0 2023-08-12 07:56:58.076541 arcon-0.3.1/arcon/py.typed
--rw-r--r--   0        0        0     2038 2023-11-26 04:41:45.367017 arcon-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 arcon-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-09 03:28:50.083099 arcon-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3095 2024-04-09 03:10:31.099060 arcon-0.4.0/README.rst
+-rw-r--r--   0        0        0     6696 2024-04-09 03:28:54.689030 arcon-0.4.0/arcon/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-09 03:29:29.436859 arcon-0.4.0/arcon/_version.py
+-rw-r--r--   0        0        0        0 2023-08-12 07:56:58.076541 arcon-0.4.0/arcon/py.typed
+-rw-r--r--   0        0        0     2022 2024-04-09 03:29:29.437664 arcon-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 arcon-0.4.0/PKG-INFO
```

### Comparing `arcon-0.3.1/LICENSE` & `arcon-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Stephen Whitlock
+Copyright (c) 2024 Stephen Whitlock
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `arcon-0.3.1/README.rst` & `arcon-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `arcon-0.3.1/arcon/__init__.py` & `arcon-0.4.0/arcon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Persistent runtime config."""
+
 from __future__ import annotations
 
 import os as _os
 import re as _re
 import typing as _t
 from argparse import Action as _Action
 from argparse import ArgumentParser as _ArgumentParser
@@ -96,18 +97,21 @@
     :param conflict_handler: String indicating how to handle conflicts.
     :param add_help: Add a -h/-help option.
     :param allow_abbrev: Allow long options to be abbreviated
         unambiguously.
     :param config: A dict object containing default values for parser.
         If no dict object provided than a pyproject.toml file will be
         loaded.
+    :param version_short_form: Alternative short form for version.
     """
 
     # noinspection PyDefaultArgument
-    def __init__(  # pylint: disable=dangerous-default-value,too-many-arguments
+    # pylint: disable=dangerous-default-value,too-many-arguments
+    # pylint: disable=too-many-locals
+    def __init__(
         self,
         version: str,
         prog: str | None = None,
         usage: str | None = None,
         description: str | None = None,
         epilog: str | None = None,
         parents: _t.Sequence[ArgumentParser] = [],  # noqa
@@ -115,14 +119,15 @@
         prefix_chars: str = "-",
         fromfile_prefix_chars: str | None = None,
         argument_default: _t.Any = None,
         conflict_handler: str = "error",
         add_help: bool = True,
         allow_abbrev: bool = True,
         config: dict[str, _t.Any] | None = None,
+        version_short_form: str = "-v",
     ) -> None:
         super().__init__(
             prog,
             usage,
             description,
             epilog,
             parents,
@@ -130,29 +135,31 @@
             prefix_chars,
             fromfile_prefix_chars,
             argument_default,
             conflict_handler,
             add_help,
             allow_abbrev,
         )
-        self.add_argument("-v", "--version", action="version", version=version)
+        self.add_argument(
+            version_short_form, "--version", action="version", version=version
+        )
         self._config = {
             k.replace("-", "_"): v
             for k, v in _mergedeep.merge(
                 _get_config(ANSI_ESCAPE.sub("", self.prog)),
                 config or {},
                 strategy=_mergedeep.Strategy.ADDITIVE,
             ).items()
         }
 
     def parse_known_args(  # type: ignore
         self,
         args: _t.Sequence[str] | None = None,
         namespace: _Namespace | None = None,
-    ) -> tuple[_Namespace, list[str]]:
+    ) -> tuple[_Namespace | None, list[str]]:
         namespace, args = super().parse_known_args(args, namespace)
         namedict = namespace.__dict__
         for key, value in self._config.items():
             if key in namedict and namedict[key] in (None, False):
                 namedict[key] = value
 
         namespace.__dict__ = _mergedeep.merge(
```

### Comparing `arcon-0.3.1/pyproject.toml` & `arcon-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -63,41 +63,40 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "arcon"
 readme = "README.rst"
 repository = "https://github.com/jshwi/arcon"
-version = "0.3.1"
+version = "0.4.0"
 
 [tool.poetry.dependencies]
 mergedeep = "^1.3.4"
 python = "^3.8"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 deptry = "^0.12.0"
 ipython = "^8.12.2"
 pre-commit = "^3.4.0"
-pyaud = "^7.2.0"
-pylint = "2.17.7"
-pytest = "^7.4.3"
+pyaud = "^7.5.0"
 pytest-randomly = "^3.15.0"
-pytest-sugar = "^0.9.6"
+pytest-sugar = "^1.0.0"
 restview = "^3.0.0"
 sphinx-toolbox = "^3.5.0"
 templatest = "^0.10.1"
 tomli-w = "^1.0.0"
 
 [tool.pyaud]
 audit = [
   "about-tests",
   "commit-policy",
   "const",
+  "copyright-year",
   "docs",
   "files",
   "format",
   "format-docs",
   "format-str",
   "imports",
   "lint",
```

### Comparing `arcon-0.3.1/PKG-INFO` & `arcon-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcon
-Version: 0.3.1
+Version: 0.4.0
 Summary: Persistent runtime config
 Home-page: https://pypi.org/project/arcon/
 License: MIT
 Keywords: arguments,config,params,parser,runtime
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://arcon.readthedocs.io/en/latest
 Project-URL: Repository, https://github.com/jshwi/arcon
 Description-Content-Type: text/x-rst
 
 arcon
```

