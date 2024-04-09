# Comparing `tmp/mutwo.core-1.4.0.tar.gz` & `tmp/mutwo.core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.core-1.4.0.tar", last modified: Wed Nov  1 09:18:20 2023, max compression
+gzip compressed data, was "mutwo.core-2.0.0.tar", last modified: Tue Apr  9 17:08:58 2024, max compression
```

## Comparing `mutwo.core-1.4.0.tar` & `mutwo.core-2.0.0.tar`

### file list

```diff
@@ -1,50 +1,47 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.871060 mutwo.core-1.4.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo/core_configurations/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_configurations/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo/core_constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1207 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_constants/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo/core_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9365 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_converters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9604 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_converters/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13949 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_converters/tempos.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo/core_events/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    50936 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    50392 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5664 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    37270 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/envelopes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_events/tempos.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo/core_generators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_generators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2320 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_generators/generic.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/mutwo/core_parameters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12931 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/abc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      771 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      915 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/durations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2777 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_parameters/tempos.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/mutwo/core_utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/decorators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7168 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/tests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19427 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_utilities/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/mutwo/core_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/mutwo/core_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-01 09:18:20.875060 mutwo.core-1.4.0/mutwo.core.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2023-11-01 09:18:20.000000 mutwo.core-1.4.0/mutwo.core.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1131 2023-11-01 09:18:20.000000 mutwo.core-1.4.0/mutwo.core.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-11-01 09:18:20.000000 mutwo.core-1.4.0/mutwo.core.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-11-01 09:18:20.000000 mutwo.core-1.4.0/mutwo.core.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-11-01 09:18:20.000000 mutwo.core-1.4.0/mutwo.core.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-11-01 09:18:20.879060 mutwo.core-1.4.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2001 2023-11-01 09:18:09.000000 mutwo.core-1.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2267 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      899 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.967424 mutwo.core-2.0.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.971424 mutwo.core-2.0.0/mutwo/core_configurations/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1400 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_configurations/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.971424 mutwo.core-2.0.0/mutwo/core_constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1622 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_constants/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.971424 mutwo.core-2.0.0/mutwo/core_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1034 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8459 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_converters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1109 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7783 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_converters/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9977 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_converters/tempos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.971424 mutwo.core-2.0.0/mutwo/core_events/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2544 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    46313 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    44983 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1265 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28888 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/envelopes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4053 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_events/patchparameters.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.971424 mutwo.core-2.0.0/mutwo/core_parameters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1173 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_parameters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13522 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_parameters/abc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2037 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_parameters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3039 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_parameters/durations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4434 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_parameters/tempos.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/mutwo/core_utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1077 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      956 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4243 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7454 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2437 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/mutwo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1952 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/tests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21649 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_utilities/tools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/mutwo/core_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      868 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/mutwo/core_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/mutwo.core.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2267 2024-04-09 17:08:58.000000 mutwo.core-2.0.0/mutwo.core.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2024-04-09 17:08:58.000000 mutwo.core-2.0.0/mutwo.core.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-09 17:08:58.000000 mutwo.core-2.0.0/mutwo.core.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-09 17:08:58.000000 mutwo.core-2.0.0/mutwo.core.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-09 17:08:58.000000 mutwo.core-2.0.0/mutwo.core.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-09 17:08:58.975424 mutwo.core-2.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2643 2024-04-09 17:08:46.000000 mutwo.core-2.0.0/setup.py
```

### Comparing `mutwo.core-1.4.0/LICENSE` & `mutwo.core-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.4.0/PKG-INFO` & `mutwo.core-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mutwo.core
-Version: 1.4.0
+Version: 2.0.0
 Summary: core library for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo.core
-Author: Tim Pauli, Levin Eric Zimmermann
-Author-email: tim.pauli@folkwang-uni.de, levin.eric.zimmermann@posteo.eu
+Author: Levin Eric Zimmermann, Tim Pauli
+Author-email: levin.eric.zimmermann@posteo.eu, tim.pauli@folkwang-uni.de
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -22,18 +22,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<2.00,>=1.18
-Requires-Dist: scipy<2.0.0,>=1.4.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
-Requires-Dist: quicktions<2.0,>=1.10
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.core
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.core.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.core)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.core-1.4.0/README.md` & `mutwo.core-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.core-1.4.0/mutwo/core_converters/abc.py` & `mutwo.core-2.0.0/mutwo/core_converters/abc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,37 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Defining the public API for any converter class."""
 
 import abc
 import typing
 
 from mutwo import core_events
 from mutwo import core_parameters
+from mutwo import core_utilities
 
 __all__ = ("Converter", "EventConverter", "SymmetricalEventConverter")
 
 
-class Converter(abc.ABC):
+class Converter(core_utilities.MutwoObject, abc.ABC):
     """Abstract base class for all Converter classes.
 
     Converter classes are defined as classes that convert data between
     two different encodings. Their only public method (besides initialisation)
     should be a `convert` method. The first argument of the convert method
     should be the data to convert.
     """
@@ -32,203 +50,168 @@
     """Abstract base class for Converter which handle mutwo events.
 
     This class helps building new classes which convert mutwo events
     with few general private methods (and without adding any new public
     method). Converting mutwo event often involves the same pattern:
     due to the nested structure of an Event, the converter has
     to iterate through the different layers until it reaches leaves
-    (any class that inherits from :class:`mutwo.core_events.SimpleEvent`).
+    (any class that inherits from :class:`mutwo.core_events.Chronon`).
     This common iteration process and the different time treatment
-    between :class:`mutwo.core_events.SequentialEvent` and
-    :class:`mutwo.core_events.SimultaneousEvent` are implemented in
+    between :class:`mutwo.core_events.Consecution` and
+    :class:`mutwo.core_events.Concurrence` are implemented in
     :class:`EventConverter`.  For writing a new EventConverter class,
-    one only has to override the abstract method :func:`_convert_simple_event`
+    one only has to override the abstract method :func:`_convert_chronon`
     and the abstract method :func:`convert` (where one will perhaps call
     :func:`_convert_event`.).
 
     **Example:**
 
     The following example defines a dummy class for demonstrating how
     to use EventConverter.
 
     >>> from mutwo import core_converters
     >>> class DurationPrintConverter(core_converters.abc.EventConverter):
-    ...     def _convert_simple_event(self, event_to_convert, absolute_entry_delay):
-    ...         return "{}: {}".format(absolute_entry_delay, event_to_convert.duration),
+    ...     def _convert_chronon(self, event_to_convert, absolute_time):
+    ...         return "{}: {}".format(absolute_time, event_to_convert.duration),
     ...     def convert(self, event_to_convert):
     ...         data_per_event = self._convert_event(event_to_convert, 0)
     ...         [print(data) for data in data_per_event]
     >>> # now test with random event
     >>> import random
     >>> from mutwo import core_events
     >>> random.seed(100)
-    >>> random_event = core_events.SimultaneousEvent(
+    >>> random_event = core_events.Concurrence(
     ...     [
-    ...        core_events.SequentialEvent(
+    ...        core_events.Consecution(
     ...             [
-    ...                core_events.SimpleEvent(random.uniform(0.5, 2))
+    ...                core_events.Chronon(random.uniform(0.5, 2))
     ...                 for _ in range(random.randint(2, 5))
     ...             ]
     ...         )
     ...         for _ in range(random.randint(1, 3))
     ...     ]
     ... )
     >>> DurationPrintConverter().convert(random_event)
-    DirectDuration(duration = 0): DirectDuration(duration = 332813340356277/281474976710656)
-    DirectDuration(duration = 332813340356277/281474976710656): DirectDuration(duration = 3729376151804513/2251799813685248)
-    DirectDuration(duration = 6391882874654729/2251799813685248): DirectDuration(duration = 7017823472572815/4503599627370496)
-    DirectDuration(duration = 19801589221882273/4503599627370496): DirectDuration(duration = 449779690686865/281474976710656)
-    DirectDuration(duration = 26998064272872113/4503599627370496): DirectDuration(duration = 5180362984867255/4503599627370496)
+    D(0.0): D(1.1823905068)
+    D(1.1823905068): D(1.6561757085)
+    D(2.8385662153): D(1.5582698404)
+    D(4.3968360557): D(1.5979384595)
+    D(5.9947745152): D(1.1502716523)
     """
 
     @abc.abstractmethod
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        event_to_convert: core_events.SimpleEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        event_to_convert: core_events.Chronon,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
     ) -> typing.Sequence[typing.Any]:
-        """Convert instance of :class:`mutwo.core_events.SimpleEvent`."""
+        """Convert instance of :class:`mutwo.core_events.Chronon`."""
 
-    def _convert_simultaneous_event(
+    def _convert_concurrence(
         self,
-        simultaneous_event: core_events.SimultaneousEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        concurrence: core_events.Concurrence,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
     ) -> typing.Sequence[typing.Any]:
-        """Convert instance of :class:`mutwo.core_events.SimultaneousEvent`."""
-
-        data_per_simple_event_list: list[tuple[typing.Any]] = []
-
-        for event in simultaneous_event:
-            data_per_simple_event_list.extend(
-                self._convert_event(event, absolute_entry_delay, depth + 1)
-            )
-        return tuple(data_per_simple_event_list)
+        """Convert instance of :class:`mutwo.core_events.Concurrence`."""
+        d: list[tuple[typing.Any]] = []
+        for e in concurrence:
+            d.extend(self._convert_event(e, absolute_time, depth + 1))
+        return tuple(d)
 
-    def _convert_sequential_event(
+    def _convert_consecution(
         self,
-        sequential_event: core_events.SequentialEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        consecution: core_events.Consecution,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
     ) -> typing.Sequence[typing.Any]:
-        """Convert instance of :class:`mutwo.core_events.SequentialEvent`."""
-
-        data_per_simple_event_list: list[tuple[typing.Any]] = []
-        for event_start, event in zip(
-            sequential_event.absolute_time_tuple, sequential_event
-        ):
-            data_per_simple_event_list.extend(
-                self._convert_event(
-                    event, event_start + absolute_entry_delay, depth + 1
-                )
-            )
-        return tuple(data_per_simple_event_list)
+        """Convert instance of :class:`mutwo.core_events.Consecution`."""
+        d: list[tuple[typing.Any]] = []
+        for t, e in zip(consecution.absolute_time_tuple, consecution):
+            d.extend(self._convert_event(e, t + absolute_time, depth + 1))
+        return tuple(d)
 
     def _convert_event(
         self,
         event_to_convert: core_events.abc.Event,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
     ) -> typing.Any:
         """Convert :class:`mutwo.core_events.abc.Event` of unknown type.
 
         The method calls different subroutines depending on whether
         the passed event either are instances from:
 
-            1. :class:`mutwo.core_events.SimpleEvent` or
-            2. :class:`mutwo.core_events.SequentialEvent` or
-            3. :class:`mutwo.core_events.SimultaneousEvent`.
+            1. :class:`mutwo.core_events.Chronon` or
+            2. :class:`mutwo.core_events.Consecution` or
+            3. :class:`mutwo.core_events.Concurrence`.
         """
-
-        absolute_entry_delay = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_entry_delay
-        )
-
-        if isinstance(event_to_convert, core_events.SequentialEvent):
-            conversion_method = self._convert_sequential_event
-        elif isinstance(
-            event_to_convert,
-            core_events.SimultaneousEvent,
-        ):
-            conversion_method = self._convert_simultaneous_event
-        elif isinstance(
-            event_to_convert,
-            core_events.SimpleEvent,
-        ):
-            conversion_method = self._convert_simple_event
-        else:
-            raise TypeError(
-                f"Can't convert object '{event_to_convert}' of type "
-                f"'{type(event_to_convert)}' with EventConverter."
-                " Supported types only include all inherited classes "
-                f"from '{core_events.abc.Event}'."
-            )
-
+        e = event_to_convert
+        t = core_parameters.abc.Duration.from_any(absolute_time)
+        match e:
+            case core_events.Consecution():
+                f = self._convert_consecution
+            case core_events.Concurrence():
+                f = self._convert_concurrence
+            case core_events.Chronon():
+                f = self._convert_chronon
+            case _:
+                raise TypeError(
+                    f"Can't convert object '{event_to_convert}' of type "
+                    f"'{type(event_to_convert)}' with EventConverter."
+                    " Supported types only include all inherited classes "
+                    f"from '{core_events.abc.Event}'."
+                )
         try:
-            return conversion_method(event_to_convert, absolute_entry_delay, depth)
+            return f(event_to_convert, t, depth)
         except TypeError:
-            return conversion_method(event_to_convert, absolute_entry_delay)
+            return f(event_to_convert, t)
 
 
 class SymmetricalEventConverter(EventConverter):
     """Abstract base class for Converter which handle mutwo core_events.
 
     This converter is a more specified version of the :class:`EventConverter`.
     It helps for building converters which aim to return mutwo core_events.
     """
 
     @abc.abstractmethod
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        event_to_convert: core_events.SimpleEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        event_to_convert: core_events.Chronon,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
-    ) -> core_events.SimpleEvent:
-        """Convert instance of :class:`mutwo.core_events.SimpleEvent`."""
+    ) -> core_events.Chronon:
+        """Convert instance of :class:`mutwo.core_events.Chronon`."""
 
-    def _convert_simultaneous_event(
+    def _convert_concurrence(
         self,
-        simultaneous_event: core_events.SimultaneousEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        concurrence: core_events.Concurrence,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
-    ) -> core_events.SimultaneousEvent:
-        """Convert instance of :class:`mutwo.core_events.SimultaneousEvent`."""
-
-        converted_simultaneous_event: core_events.SimultaneousEvent = (
-            simultaneous_event.empty_copy()
-        )
+    ) -> core_events.Concurrence:
+        """Convert instance of :class:`mutwo.core_events.Concurrence`."""
+        sim: core_events.Concurrence = concurrence.empty_copy()
+        for e in concurrence:
+            sim.append(self._convert_event(e, absolute_time, depth + 1))
+        return sim
 
-        for event in simultaneous_event:
-            converted_simultaneous_event.append(
-                self._convert_event(event, absolute_entry_delay, depth + 1)
-            )
-        return converted_simultaneous_event
-
-    def _convert_sequential_event(
+    def _convert_consecution(
         self,
-        sequential_event: core_events.SequentialEvent,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        consecution: core_events.Consecution,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
-    ) -> core_events.SequentialEvent:
-        """Convert instance of :class:`mutwo.core_events.SequentialEvent`."""
-
-        converted_sequential_event: core_events.SequentialEvent = (
-            sequential_event.empty_copy()
-        )
-        for event_start, event in zip(
-            sequential_event.absolute_time_tuple, sequential_event
-        ):
-            converted_sequential_event.append(
-                self._convert_event(
-                    event, event_start + absolute_entry_delay, depth + 1
-                )
-            )
-        return converted_sequential_event
+    ) -> core_events.Consecution:
+        """Convert instance of :class:`mutwo.core_events.Consecution`."""
+        cons: core_events.Consecution = consecution.empty_copy()
+        for t, e in zip(consecution.absolute_time_tuple, consecution):
+            cons.append(self._convert_event(e, t + absolute_time, depth + 1))
+        return cons
 
     def _convert_event(
         self,
         event_to_convert: core_events.abc.Event,
-        absolute_entry_delay: core_parameters.abc.Duration | float | int,
+        absolute_time: core_parameters.abc.Duration | float | int,
         depth: int = 0,
-    ) -> core_events.abc.ComplexEvent[core_events.abc.Event]:
-        return super()._convert_event(event_to_convert, absolute_entry_delay, depth)
+    ) -> core_events.abc.Compound[core_events.abc.Event]:
+        return super()._convert_event(event_to_convert, absolute_time, depth)
```

### Comparing `mutwo.core-1.4.0/mutwo/core_converters/parsers.py` & `mutwo.core-2.0.0/mutwo/core_converters/parsers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,96 @@
-"""Standardization for transformations between parameters and simple events
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2023
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""Standardization for transformations between parameters and chronons
 
 Adds classes to allow transformations in two directions:
 
-1. Extract data (e.g. mutwo parameters) from simple events
-2. Convert data (e.g. mutwo parameters) to simple events
+1. Extract data (e.g. mutwo parameters) from chronons
+2. Convert data (e.g. mutwo parameters) to chronons
 """
 
 import typing
 
-from mutwo import core_constants
 from mutwo import core_converters
 from mutwo import core_events
 from mutwo import core_utilities
 
 
 __all__ = (
-    "SimpleEventToAttribute",
+    "ChrononToAttribute",
     "MutwoParameterDict",
     "MutwoParameterDictToKeywordArgument",
     "MutwoParameterDictToDuration",
-    "MutwoParameterDictToSimpleEvent",
-    "UnknownObjectToObject",
+    "MutwoParameterDictToChronon",
 )
 
 
-class SimpleEventToAttribute(core_converters.abc.Converter):
-    """Extract from a simple event an attribute.
+class ChrononToAttribute(core_converters.abc.Converter):
+    """Extract from a chronon an attribute.
 
     :param attribute_name: The name of the attribute which is fetched
-        from a :class:`mutwo.core_events.SimpleEvent`.
+        from a :class:`mutwo.core_events.Chronon`.
     :param exception_value: This value is returned in case an `AttributeError`
         raises .
     """
 
     def __init__(self, attribute_name: str, exception_value: typing.Any):
         self._attribute_name = attribute_name
         self._exception_value = exception_value
 
-    def convert(self, simple_event_to_convert: core_events.SimpleEvent) -> typing.Any:
-        """Extract from a :class:`mutwo.core_events.SimpleEvent` an attribute.
+    def convert(self, chronon_to_convert: core_events.Chronon) -> typing.Any:
+        """Extract from a :class:`mutwo.core_events.Chronon` an attribute.
 
-        :param simple_event_to_convert: The :class:`mutwo.core_events.SimpleEvent`
+        :param chronon_to_convert: The :class:`mutwo.core_events.Chronon`
             from which an attribute shall be extracted.
-        :type simple_event_to_convert: mutwo.core_events.SimpleEvent
+        :type chronon_to_convert: mutwo.core_events.Chronon
 
         **Example:**
 
         >>> from mutwo import core_converters
         >>> from mutwo import core_events
-        >>> simple_event = core_events.SimpleEvent(duration=10)
-        >>> simple_event_to_duration = core_converters.SimpleEventToAttribute(
+        >>> chronon = core_events.Chronon(duration=10.0)
+        >>> chronon_to_duration = core_converters.ChrononToAttribute(
         ...     'duration', 0
         ... )
-        >>> simple_event_to_duration.convert(simple_event)
-        DirectDuration(10)
-        >>> simple_event_to_pasta = core_converters.SimpleEventToAttribute(
+        >>> chronon_to_duration.convert(chronon)
+        DirectDuration(10.0)
+        >>> chronon_to_pasta = core_converters.ChrononToAttribute(
         ...     'pasta', 'spaghetti'
         ... )
-        >>> simple_event_to_pasta.convert(simple_event)
+        >>> chronon_to_pasta.convert(chronon)
         'spaghetti'
-        >>> simple_event.pasta = 'tagliatelle'
-        >>> simple_event_to_pasta.convert(simple_event)
+        >>> chronon.pasta = 'tagliatelle'
+        >>> chronon_to_pasta.convert(chronon)
         'tagliatelle'
         """
 
         return core_utilities.call_function_except_attribute_error(
-            lambda simple_event: getattr(simple_event, self._attribute_name),
-            simple_event_to_convert,
+            lambda chronon: getattr(chronon, self._attribute_name),
+            chronon_to_convert,
             self._exception_value,
         )
 
 
-MutwoParameterDict = dict[str, core_constants.ParameterType]
+MutwoParameterDict: typing.TypeAlias = dict[str, typing.Any]
 
 
 class MutwoParameterDictToKeywordArgument(core_converters.abc.Converter):
     """Extract from a dict of mutwo parameters specific objects.
 
     :param mutwo_parameter_to_search_name: The parameter name which
         should be fetched from the MutwoParameterDict (if it exists).
@@ -86,30 +101,28 @@
 
     **Example:**
 
     >>> from mutwo import core_converters
     >>> from mutwo import core_parameters
     >>> mutwo_parameter_dict_to_keyword_argument = core_converters.MutwoParameterDictToKeywordArgument('duration')
     >>> mutwo_parameter_dict_to_keyword_argument.convert(
-    ...     {'duration': core_parameters.DirectDuration(1)}
+    ...     {'duration': core_parameters.DirectDuration(1.0)}
     ... )
-    ('duration', DirectDuration(1))
+    ('duration', DirectDuration(1.0))
     """
 
     def __init__(
         self, mutwo_parameter_to_search_name: str, keyword: typing.Optional[str] = None
     ):
-        if keyword is None:
-            keyword = str(mutwo_parameter_to_search_name)
         self._mutwo_parameter_to_search_name = mutwo_parameter_to_search_name
-        self._keyword = keyword
+        self._keyword = keyword or str(mutwo_parameter_to_search_name)
 
     def convert(
         self, mutwo_parameter_dict_to_convert: MutwoParameterDict
-    ) -> typing.Optional[tuple[str, core_constants.ParameterType]]:
+    ) -> typing.Optional[tuple[str, typing.Any]]:
         try:
             return (
                 self._keyword,
                 mutwo_parameter_dict_to_convert[self._mutwo_parameter_to_search_name],
             )
         except KeyError:
             return None
@@ -133,117 +146,57 @@
     """
 
     def __init__(
         self,
         duration_to_search_name: typing.Optional[str] = None,
         duration_keyword_name: typing.Optional[str] = None,
     ):
-        if duration_to_search_name is None:
-            duration_to_search_name = (
-                core_converters.configurations.DEFAULT_DURATION_TO_SEARCH_NAME
-            )
-        if duration_keyword_name is None:
-            duration_keyword_name = (
-                core_converters.configurations.DEFAULT_DURATION_KEYWORD_NAME
-            )
-        assert isinstance(duration_to_search_name, str)
-        assert isinstance(duration_keyword_name, str)
-        super().__init__(duration_to_search_name, duration_keyword_name)
+        super().__init__(
+            duration_to_search_name
+            or core_converters.configurations.DEFAULT_DURATION_TO_SEARCH_NAME,
+            duration_keyword_name
+            or core_converters.configurations.DEFAULT_DURATION_KEYWORD_NAME,
+        )
 
 
-class MutwoParameterDictToSimpleEvent(core_converters.abc.Converter):
-    """Convert a dict of mutwo parameters to a :class:`mutwo.core_events.SimpleEvent`
+class MutwoParameterDictToChronon(core_converters.abc.Converter):
+    """Convert a dict of mutwo parameters to a :class:`mutwo.core_events.Chronon`
 
     :param mutwo_parameter_dict_to_keyword_argument_sequence: A sequence of
         :class:`MutwoParameterDictToKeywordArgument`. If set to `None`
         a sequence with :class:`MutwoParameterDictToDuration` will be created.
         Default to `None`.
     :type mutwo_parameter_dict_to_keyword_argument_sequence: typing.Optional[typing.Sequence[MutwoParameterDictToKeywordArgument]]
-    :param simple_event_class: Default to :class:`mutwo.core_events.SimpleEvent`.
-    :type simple_event_class: typing.Type[core_events.SimpleEvent]
+    :param chronon_class: Default to :class:`mutwo.core_events.Chronon`.
+    :type chronon_class: typing.Type[core_events.Chronon]
     """
 
     def __init__(
         self,
         mutwo_parameter_dict_to_keyword_argument_sequence: typing.Optional[
             typing.Sequence[MutwoParameterDictToKeywordArgument]
         ] = None,
-        simple_event_class: typing.Type[
-            core_events.SimpleEvent
-        ] = core_events.SimpleEvent,
+        chronon_class: typing.Type[core_events.Chronon] = core_events.Chronon,
     ):
-        if mutwo_parameter_dict_to_keyword_argument_sequence is None:
-            mutwo_parameter_dict_to_keyword_argument_sequence = (
-                MutwoParameterDictToDuration(),
-            )
         self._mutwo_parameter_dict_to_keyword_argument_sequence = (
             mutwo_parameter_dict_to_keyword_argument_sequence
+            or (MutwoParameterDictToDuration(),)
         )
-        self._simple_event_class = simple_event_class
+        self._chronon_class = chronon_class
 
     def convert(
         self, mutwo_parameter_dict_to_convert: MutwoParameterDict
-    ) -> core_events.SimpleEvent:
+    ) -> core_events.Chronon:
         keyword_argument_dict = {}
         for (
             mutwo_parameter_dict_to_keyword_argument
         ) in self._mutwo_parameter_dict_to_keyword_argument_sequence:
             keyword_argument_or_none = mutwo_parameter_dict_to_keyword_argument.convert(
                 mutwo_parameter_dict_to_convert
             )
             if keyword_argument_or_none:
                 keyword, argument = keyword_argument_or_none
                 keyword_argument_dict.update({keyword: argument})
-        return self._simple_event_class(**keyword_argument_dict)
+        return self._chronon_class(**keyword_argument_dict)
 
 
 T = typing.TypeVar("T")
-
-
-class UnknownObjectToObject(core_converters.abc.Converter, typing.Generic[T]):
-    """Helper to simplify standardisation of syntactic sugar.
-
-    :param type_tuple_to_callable_dict: Define which types are converted by
-        which methods.
-
-    **Example:**
-
-    >>> from mutwo import core_converters
-    >>> anything_to_string = core_converters.UnknownObjectToObject[str](
-    ...     (
-    ...         ((float, int, list), str),
-    ...         ((tuple,), lambda t: str(len(t))),
-    ...         ([], lambda _: "..."),
-    ...     )
-    ... )
-    >>> anything_to_string.convert(100)
-    '100'
-    >>> anything_to_string.convert(7.32)
-    '7.32'
-    >>> anything_to_string.convert((1, 2, 3))
-    '3'
-    >>> anything_to_string.convert(b'')
-    '...'
-    """
-
-    def __init__(
-        self,
-        type_tuple_and_callable_tuple: tuple[tuple[typing.Type, ...], typing.Callable],
-    ):
-        self._type_tuple_and_callable_tuple = type_tuple_and_callable_tuple
-
-    def convert(self, unknown_object_to_convert: typing.Any) -> T:
-        # XXX: This may break in the future, because it is an implementation
-        # detail.
-        if isinstance(unknown_object_to_convert, typing.get_args(self.__orig_class__)):
-            return unknown_object_to_convert
-        for type_tuple, callable_object in self._type_tuple_and_callable_tuple:
-            if type_tuple:
-                if isinstance(unknown_object_to_convert, type_tuple):
-                    return callable_object(unknown_object_to_convert)
-            else:
-                return callable_object(unknown_object_to_convert)
-
-        raise NotImplementedError(
-            f"No conversion routine defined for object '{unknown_object_to_convert}'"
-            f" of type '{type(unknown_object_to_convert)}'."
-        )
```

### Comparing `mutwo.core-1.4.0/mutwo/core_events/abc.py` & `mutwo.core-2.0.0/mutwo/core_events/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,81 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Abstract base classes for events (definition of public API)."""
 
 from __future__ import annotations
 
 import abc
-import copy
 import functools
 import typing
 
 from mutwo import core_constants
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 
-__all__ = ("Event", "ComplexEvent")
+__all__ = ("Event", "Compound")
 
 
-class Event(abc.ABC):
+class Event(core_utilities.MutwoObject, abc.ABC):
     """Abstract Event-Object
 
-    :param tempo_envelope: An envelope which describes the dynamic tempo of an event.
+    :param tempo: An envelope which describes the dynamic tempo of an event.
+    :param tag: The name of the event. This can be used to find the event
+        inside a :class:`Compound`.
     """
 
-    # It looks tempting to drop the 'tempo_envelope' attribute of events.
+    # It looks tempting to drop the 'tempo' attribute of events.
     # It may look simpler (and therefore more elegant) if events are only
     # defined by one attribute: their duration. Let's remember why the
-    # 'tempo_envelope' attribute was initially introduced [1]:
+    # 'tempo' attribute was initially introduced [1]:
     #
     # - With [1] it was decided that durations are represented in the unit
-    #   'beats'.
+    #   'beat_count'.
     #
     # - An event should have an unambiguous duration, so that converters
     #   (and all other 'mutwo' parts) can treat an event consistently.
     #
-    # - The unit of 'beats' doesn't say anything about the real duration: only
-    #   in cooperation with a specified tempo it can be clearly stated how long
-    #   an event is.
+    # - The unit of 'beat_count' doesn't say anything about the real duration:
+    #   only in cooperation with a specified tempo it can be clearly stated how
+    #   long an event is.
     #
     # - Therefore the combination of (a) having duration specified in the unit
-    #   'beats' and (b) wanting to have events with unambiguous duration leads
-    #   to the necessity to attach tempo envelopes to events.
+    #   'beat_count' and (b) wanting to have events with unambiguous duration
+    #   leads to the necessity to attach tempos to events.
     #
     # In the early days of mutwo (b) wasn't considered to be an objective:
     # it was the opposite, an implicit ambiguity was considered to be a good
     # idea [2]. But in the practical usage of the library it turned out that
     # this approach rather increased complexity, as other code bits are unable
     # to treat an event consistently and a user constantly has to keep in mind
     # the specific way how each converter interprets a duration. To fix this
-    # complexity, the 'beat' unit was specified and a 'tempo_envelope'
-    # attribute has been added. Now converters could be reliable to produce
+    # complexity, the 'beat' unit was specified and a 'tempo'
+    # attribute has been added. Now converters could reliably produce
     # results which match the duration of an event.
     #
-    # Now we could change durations to be no longer in the unit 'beats', but in
-    # the unit 'seconds'. Then the duration of an event would still be
-    # unambiguous without the need of a tempo envelope attribute.  We could
+    # Now we could change durations to be no longer in the unit 'beat_count',
+    # but in the unit 'seconds'. Then the duration of an event would still be
+    # unambiguous without the need of a tempo attribute.  We could
     # furthermore implement duration representations with beat & tempo as a
     # subclass of a more general 'duration=seconds' approach. This has two
     # problems:
     #
     # (1) It may be more computation intensive to ask for the
     #     'absolute_time_tuple' of a event with beat-based durations as their
     #     'seconds' attribute would need to be calculated from their beat+tempo
@@ -66,33 +84,40 @@
     # (2) It would be very impractical to use all event methods with absolute
     #     times as arguments (e. g. 'slide_in', 'split_at', ...) in a beat
     #     approached subclass, as we wouldn't squash in our event at the given
     #     'beat', but a given duration in seconds, which would depend on the
     #     tempo - and wouldn't resonate with how we usually think about music.
     #
     # (3) If we think of tempo, it's rather a global trajectory independent
-    #     from single notes. Therefore a 'TempoEnvelope' object seems to be
-    #     more consistent with how we usually approach tempo in music than a
-    #     specific tempo for each note. To still be able to have this global
-    #     trajectory, a 'duration=seconds' approach would need additional
-    #     helper functions, to apply a tempo envelope on an event with beat
-    #     based durations.
+    #     from single notes. So we usually think of a tempo trajectory as
+    #     something that belongs to a nested event (e.g. a 'Consecution' or
+    #     a 'Concurrence'). But with the duration=seconds approach such a
+    #     tempo trajectory couldn't be persistently mapped to a nested event,
+    #     because the duration of a Compound isn't a statically mapped and
+    #     available entity, but ephemerally and dynamically calculated when
+    #     needed. When the duration of a Compound is set, it becomes
+    #     propagated to the duration of its children until it finds a leaf that
+    #     statically declares its duration and then it's lost. So in order to
+    #     have a persistently available tempo trajectory on a Compound
+    #     that can be read and modified-in-place, we need an extra tempo
+    #     attribute. Otherwise we would break the rule that the duration of
+    #     a Compound is only a sum or max of its children duration.
     #
     # Due to these reasons, that describe new complexities by switching to a
-    # 'duration=seconds' model, we should stick to the beats/tempo_envelope
+    # 'duration=seconds' model, we should stick to the beats/tempo
     # approach until we can find a better solution.
     #
     # Now we could also ask the other way around, because if durations are in
     # 'beats', are musical applications too dominant in 'mutwo' and is the
     # 'mutwo' model not general enough? Interestingly duration as beats+tempo
     # isn't only a subset of a 'duration=seconds' model, but this is also
     # true vice versa: if the default tempo of an event (which is 60 BPM)
     # isn't changed, the beats of a duration does in fact equal seconds.
     # So for users who don't care about splitting duration into beats+tempo,
-    # they can simply avoid any 'tempo_envelope' attribute and directly write
+    # they can simply avoid any 'tempo' attribute and directly write
     # their duration in seconds.
     #
     # ---
     #
     # [1] https://github.com/mutwo-org/mutwo.core/commit/c2c7f3ba
     # [2] In fact this ambiguity was always only true for durations: pitches
     #     or volumes for instance were always unambiguous. Nowadays we can
@@ -100,17 +125,19 @@
     #     represent a clear idea of *something*. Converters, on the other
     #     hand, interpret this event as it is in the converters idiosyncratic
     #     understanding of it, but by trying to be as true as possible to
     #     the original idea.
 
     def __init__(
         self,
-        tempo_envelope: typing.Optional[core_events.TempoEnvelope] = None,
+        tempo: typing.Optional[core_parameters.abc.Tempo] = None,
+        tag: typing.Optional[str] = None,
     ):
-        self.tempo_envelope = tempo_envelope
+        self.tempo = tempo
+        self.tag = tag
 
     # ###################################################################### #
     #                        abstract properties                             #
     # ###################################################################### #
 
     @property
     @abc.abstractmethod
@@ -122,387 +149,345 @@
 
     # ###################################################################### #
     #                           private methods                              #
     # ###################################################################### #
 
     @staticmethod
     def _assert_correct_start_and_end_values(
-        start: core_parameters.abc.Duration,
-        end: core_parameters.abc.Duration,
+        start: core_parameters.abc.Duration | core_constants.Real,
+        end: core_parameters.abc.Duration | core_constants.Real,
         condition: typing.Callable[
             [core_parameters.abc.Duration, core_parameters.abc.Duration], bool
         ] = lambda start, end: end
         >= start,
     ):
         """Helper method to make sure that start < end.
 
         Can be used within the different cut_out methods.
         """
         if not condition(start, end):
             raise core_utilities.InvalidStartAndEndValueError(start, end)
 
     @staticmethod
-    def _assert_valid_absolute_time(t: core_parameters.abc.Duration):
+    def _assert_valid_absolute_time(
+        t: core_parameters.abc.Duration | core_constants.Real,
+    ):
         if t < 0:
             raise core_utilities.InvalidAbsoluteTime(t)
 
     @functools.cached_property
     def _event_to_metrized_event(self):
         # Import in method to avoid circular import error
         return __import__(
             "mutwo.core_converters"
         ).core_converters.EventToMetrizedEvent()
 
     @abc.abstractmethod
     def _set_parameter(
         self,
         parameter_name: str,
-        object_or_function: typing.Callable[
-            [core_constants.ParameterType], core_constants.ParameterType
-        ]
-        | core_constants.ParameterType,
+        object_or_function: typing.Callable[[typing.Any], typing.Any] | typing.Any,
         set_unassigned_parameter: bool,
         id_set: set[int],
     ) -> Event:
         ...
 
     @abc.abstractmethod
     def _mutate_parameter(
         self,
         parameter_name: str,
-        function: typing.Callable[[core_constants.ParameterType], None] | typing.Any,
+        function: typing.Callable[[typing.Any], None] | typing.Any,
         id_set: set[int],
     ) -> Event:
         ...
 
     # ###################################################################### #
     #                           public properties                            #
     # ###################################################################### #
 
     @property
-    def tempo_envelope(self) -> core_events.TempoEnvelope:
-        """The dynamic tempo of an event; specified as an envelope.
-
-        Tempo envelopes are represented as :class:`core_events.TempoEnvelope`
-        objects. Tempo envelopes are valid for its respective event and all its
-        children events.
-        """
-        if self._tempo_envelope is None:
-            self.reset_tempo_envelope()
-        return self._tempo_envelope
-
-    @tempo_envelope.setter
-    def tempo_envelope(
-        self, tempo_envelope: typing.Optional[core_events.TempoEnvelope]
-    ):
-        self._tempo_envelope = tempo_envelope
+    def tempo(self) -> core_parameters.abc.Tempo:
+        """The tempo of an event."""
+        if self._tempo is None:
+            self.reset_tempo()
+        return self._tempo
+
+    @tempo.setter
+    def tempo(self, tempo: typing.Optional[core_parameters.abc.Tempo]):
+        self._tempo = core_parameters.abc.Tempo.from_any(tempo) if tempo else None
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
-    def copy(self) -> Event:
-        """Return a deep copy of the given Event."""
-        return copy.deepcopy(self)
-
     @abc.abstractmethod
     def destructive_copy(self) -> Event:
         """Adapted deep copy method that returns a new object for every leaf.
 
         It's called 'destructive', because it forgets potential repetitions of
         the same object in compound objects. Instead of reproducing the original
         structure of the compound object that shall be copied, every repetition
-        of the same reference will return a new unique independent object.
+        of the same reference returns a new unique independent object.
 
         The following example shall illustrate the difference between copy.deepcopy
         and destructive_copy:
 
         >>> import copy
         >>> from mutwo import core_events
-        >>> my_simple_event_0 = core_events.SimpleEvent(2)
-        >>> my_simple_event_1 = core_events.SimpleEvent(3)
-        >>> my_sequential_event = core_events.SequentialEvent(
-        ...     [my_simple_event_0, my_simple_event_1, my_simple_event_0]
-        ... )
-        >>> deepcopied_event = copy.deepcopy(my_sequential_event)
-        >>> destructivecopied_event = my_sequential_event.destructive_copy()
-        >>> deepcopied_event[0].duration = 10  # setting the duration of the first event
-        >>> destructivecopied_event[0].duration = 10
+        >>> chn0 = core_events.Chronon(2)
+        >>> chn1 = core_events.Chronon(3)
+        >>> cns = core_events.Consecution([chn0, chn1, chn0])
+        >>> cns_copy = copy.deepcopy(cns)
+        >>> cns_destr_copy = cns.destructive_copy()
+        >>> cns_copy[0].duration = 10  # setting the duration of the first event
+        >>> cns_destr_copy[0].duration = 10
         >>> # return True because the first and the third objects share the same
-        >>> # reference (both are the same copy of 'my_simple_event_0')
-        >>> deepcopied_event[0].duration == deepcopied_event[2].duration
+        >>> # reference (both are the same copy of 'my_chronon_0')
+        >>> cns_copy[0].duration == cns_copy[2].duration
         True
         >>> # return False because destructive_copy forgets the shared reference
-        >>> destructivecopied_event[0].duration == destructivecopied_event[2].duration
+        >>> cns_destr_copy[0].duration == cns_destr_copy[2].duration
         False
         """
 
-    @core_utilities.add_copy_option
     def set(self, attribute_name: str, value: typing.Any) -> Event:
         """Set an attribute of the object to a specific value
 
         :param attribute_name: The name of the attribute which value shall be set.
         :param value: The value which shall be assigned to the given
             :attr:`attribute_name`
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
         :return: The event.
 
         This function is merely a convenience wrapper for...
 
         ``event.attribute_name = value``
 
         Because the function return the event itself it can be used
         in function composition.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(2)])
-        >>> sequential_event.set('duration', 10).set('my_new_attribute', 'hello-world!')
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 10))])
+        >>> cns = core_events.Consecution([core_events.Chronon(2)])
+        >>> cns.set('duration', 10).set('my_new_attribute', 'hello-world!')
+        Consecution([Chronon(duration=DirectDuration(10.0))])
         """
         setattr(self, attribute_name, value)
         return self
 
     @abc.abstractmethod
     def get_parameter(
         self, parameter_name: str, flat: bool = False, filter_undefined: bool = False
-    ) -> tuple[core_constants.ParameterType, ...] | core_constants.ParameterType:
+    ) -> tuple[typing.Any, ...] | typing.Any:
         """Return event attribute with the entered name.
 
         :param parameter_name: The name of the attribute that shall be returned.
         :type parameter_name: str
         :param flat: ``True`` for flat sequence of parameter values, ``False`` if the
             resulting ``tuple`` shall repeat the nested structure of the event.
         :type flat: bool
         :param filter_undefined: If set to ``True`` all ``None`` values will be filtered
             from the returned tuple. Default to ``False``. This flag has no effect on
-            :func:`get_parameter` of :class:`mutwo.core_events.SimpleEvent`.
+            :func:`get_parameter` of :class:`mutwo.core_events.Chronon`.
         :type flat: bool
         :return: Return tuple containing the assigned values for each contained
             event. If an event doesn't posses the asked parameter, mutwo will simply
             add None to the tuple for the respective event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SimpleEvent(2), core_events.SimpleEvent(3)]
+        >>> cns = core_events.Consecution(
+        ...     [core_events.Chronon(2), core_events.Chronon(3)]
         ... )
-        >>> sequential_event.get_parameter('duration')
-        (DirectDuration(2), DirectDuration(3))
-        >>> simple_event = core_events.SimpleEvent(10)
-        >>> simple_event.get_parameter('duration')
-        DirectDuration(10)
-        >>> simple_event.get_parameter('undefined_parameter')
+        >>> cns.get_parameter('duration')
+        (DirectDuration(2.0), DirectDuration(3.0))
+        >>> chn = core_events.Chronon(10)
+        >>> chn.get_parameter('duration')
+        DirectDuration(10.0)
+        >>> chn.get_parameter('undefined_parameter')
         """
 
     def set_parameter(
         self,
         parameter_name: str,
-        object_or_function: typing.Callable[
-            [core_constants.ParameterType], core_constants.ParameterType
-        ]
-        | core_constants.ParameterType,
+        object_or_function: typing.Callable[[typing.Any], typing.Any] | typing.Any,
         set_unassigned_parameter: bool = True,
-        mutate: bool = True,
     ) -> typing.Optional[Event]:
         """Sets parameter to new value for all children events.
 
         :param parameter_name: The name of the parameter which values shall be changed.
         :type parameter_name: str
         :param object_or_function: For setting the parameter either a new value can be
             passed directly or a function can be passed. The function gets as an
             argument the previous value that has had been assigned to the respective
             object and has to return a new value that will be assigned to the object.
         :param set_unassigned_parameter: If set to False a new parameter will only be
             assigned to an Event if the Event already has a attribute with the
             respective `parameter_name`. If the Event doesn't know the attribute yet
             and `set_unassigned_parameter` is False, the method call will simply be
             ignored.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
         :return: The event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SimpleEvent(2), core_events.SimpleEvent(3)]
+        >>> cns = core_events.Consecution(
+        ...     [core_events.Chronon(2), core_events.Chronon(3)]
         ... )
-        >>> sequential_event.set_parameter('duration', lambda duration: duration * 2)
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 4)), SimpleEvent(duration = DirectDuration(duration = 6))])
-        >>> sequential_event.get_parameter('duration')
-        (DirectDuration(4), DirectDuration(6))
+        >>> cns.set_parameter('duration', lambda duration: duration * 2)
+        Consecution([Chronon(duration=DirectDuration(4.0)), Chronon(duration=DirectDuration(6.0))])
+        >>> cns.get_parameter('duration')
+        (DirectDuration(4.0), DirectDuration(6.0))
 
         **Warning:**
 
         If there are multiple references of the same Event inside a
-        :class:`~mutwo.core_events.SequentialEvent` or a
-        :class:`~mutwo.core_events.SimultaneousEvent`, ``set_parameter``
+        :class:`~mutwo.core_events.Consecution` or a
+        :class:`~mutwo.core_events.Concurrence`, ``set_parameter``
         is only called once for each Event. So multiple references
         of the same event will be ignored. This behaviour ensures,
         that on a big scale level each item inside the
-        :class:`mutwo.core_events.abc.ComplexEvent` is treated equally
+        :class:`mutwo.core_events.abc.Compound` is treated equally
         (so for instance the duration of each item is doubled, and
         nor for some doubled and for those with references which
         appear twice quadrupled).
         """
         return self._set_parameter(
             parameter_name,
             object_or_function,
             set_unassigned_parameter=set_unassigned_parameter,
-            mutate=mutate,
             id_set=set([]),
         )
 
     def mutate_parameter(
         self,
         parameter_name: str,
-        function: typing.Callable[[core_constants.ParameterType], None] | typing.Any,
-        mutate: bool = True,
+        function: typing.Callable[[typing.Any], None] | typing.Any,
     ) -> typing.Optional[Event]:
         """Mutate parameter with a function.
 
         :param parameter_name: The name of the parameter which shall be mutated.
         :param function: The function which mutates the parameter. The function gets
             as an input the assigned value for the passed parameter_name of the
             respective object. The function shouldn't return anything, but simply
             calls a method of the parameter value.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
         This method is useful when a particular parameter has been assigned to objects
         that know methods which mutate themselves. Then 'mutate_parameter' is a
         convenient wrapper to call the methods of those parameters for all children
         events.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SimpleEvent(1)]
-        ... )
-        >>> sequential_event.mutate_parameter(
+        >>> cons= core_events.Consecution([core_events.Chronon(1)])
+        >>> cons.mutate_parameter(
         ...     'duration', lambda duration: duration.add(1)
         ... )
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))])
+        Consecution([Chronon(duration=DirectDuration(2.0))])
         >>> # now duration should be + 1
-        >>> sequential_event.get_parameter('duration')
-        (DirectDuration(2),)
+        >>> cons.get_parameter('duration')
+        (DirectDuration(2.0),)
 
         **Warning:**
 
         If there are multiple references of the same Event inside a
-        :class:`~mutwo.core_events.SequentialEvent` or a
-        ~mutwo.core_events.SimultaneousEvent`, ``mutate_parameter`` will
+        :class:`~mutwo.core_events.Consecution` or a
+        ~mutwo.core_events.Concurrence`, ``mutate_parameter`` will
         only be called once for each Event. So multiple references
         of the same event will be ignored. This behaviour ensures,
         that on a big scale level each item inside the
-        :class:`mutwo.core_events.abc.ComplexEvent` is treated equally
+        :class:`mutwo.core_events.abc.Compound` is treated equally
         (so for instance the duration of each item is doubled, and
         nor for some doubled and for those with references which
         appear twice quadrupled).
         """
         return self._mutate_parameter(
             parameter_name,
             function,
-            mutate=mutate,
             id_set=set([]),
         )
 
-    @core_utilities.add_copy_option
-    def reset_tempo_envelope(self) -> Event:
-        """Set events tempo envelope so that one beat equals one second (tempo 60).
-
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
+    def reset_tempo(self) -> Event:
+        """Set events tempo so that one beat equals one second (tempo 60).
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> simple_event = core_events.SimpleEvent(duration = 1)
-        >>> simple_event.tempo_envelope[0].value = 100
-        >>> simple_event.tempo_envelope
-        TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1), value = 100), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))])
-        >>> simple_event.reset_tempo_envelope()
-        SimpleEvent(duration = DirectDuration(duration = 1))
-        >>> simple_event.tempo_envelope
-        TempoEnvelope([TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 1), tempo_point = DirectTempoPoint(BPM = 60, reference = 1)), TempoEvent(curve_shape = 0, duration = DirectDuration(duration = 0), tempo_point = DirectTempoPoint(BPM = 60, reference = 1))])
+        >>> chn = core_events.Chronon(duration = 1)
+        >>> chn.tempo.bpm = 100
+        >>> print(chn.tempo)
+        D(100.0)
+        >>> chn.reset_tempo()
+        Chronon(duration=DirectDuration(1.0))
+        >>> print(chn.tempo)
+        D(60.0)
         """
-
-        self.tempo_envelope = core_events.TempoEnvelope([[0, 60], [1, 60]])
+        self.tempo = core_parameters.DirectTempo(60)
+        return self
 
     @abc.abstractmethod
     def metrize(self) -> typing.Optional[Event]:
-        """Apply tempo envelope of event on itself
+        """Apply tempo of event on itself
 
         Metrize is only syntactic sugar for a call of
         :class:`EventToMetrizedEvent`:
 
         >>> from mutwo import core_converters
         >>> from mutwo import core_events
-        >>> my_event = core_events.SimpleEvent(1)
-        >>> my_event.tempo_envelope = core_events.TempoEnvelope([[0, 100], [1, 40]])
-        >>> core_converters.EventToMetrizedEvent().convert(
-        ...     my_event
-        ... ) == my_event.metrize()
+        >>> chn = core_events.Chronon(1)
+        >>> chn.tempo = core_parameters.FlexTempo([[0, 100], [1, 40]])
+        >>> core_converters.EventToMetrizedEvent().convert(chn) == chn.metrize()
         True
         """
 
     @abc.abstractmethod
     def cut_out(
         self,
-        start: core_parameters.abc.Duration,
-        end: core_parameters.abc.Duration,
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
     ) -> typing.Optional[Event]:
         """Time-based slicing of the respective event.
 
         :param start: Duration when the cut out shall start.
         :param end: Duration when the cut up shall end.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SimpleEvent(3), core_events.SimpleEvent(2)]
-        ... )
-        >>> sequential_event.cut_out(1, 4)
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2)), SimpleEvent(duration = DirectDuration(duration = 1))])
+        >>> chn0, chn1 = (core_events.Chronon(3), core_events.Chronon(2))
+        >>> cns = core_events.Consecution([chn0, chn1])
+        >>> cns.cut_out(1, 4)
+        Consecution([Chronon(duration=DirectDuration(2.0)), Chronon(duration=DirectDuration(1.0))])
         """
 
     @abc.abstractmethod
     def cut_off(
         self,
-        start: core_parameters.abc.Duration,
-        end: core_parameters.abc.Duration,
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
     ) -> typing.Optional[Event]:
         """Time-based deletion / shortening of the respective event.
 
         :param start: Duration when the cut off shall start.
         :param end: Duration when the cut off shall end.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SimpleEvent(3), core_events.SimpleEvent(2)]
-        ... )
-        >>> sequential_event.cut_off(1, 3)
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 2))])
+        >>> chn0, chn1 = (core_events.Chronon(3), core_events.Chronon(2))
+        >>> cns = core_events.Consecution([chn0, chn1])
+        >>> cns.cut_off(1, 3)
+        Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(2.0))])
         """
 
     def split_at(
         self,
-        *absolute_time: core_parameters.abc.Duration,
+        *absolute_time: core_parameters.abc.Duration.Type,
         ignore_invalid_split_point: bool = False,
     ) -> tuple[Event, ...]:
         """Split event into *n* events at :attr:`absolute_time`.
 
         :param *absolute_time: where event shall be split
         :param ignore_invalid_split_point: If set to `True` `split_at` won't raise
             :class:`mutwo.core_utilities.SplitError` in case a split time isn't
@@ -515,43 +500,45 @@
             `ignore_invalid_split_point` is not set.
         :return:  Tuple of events that result from splitting the present event.
 
         **Hint:**
 
         Calling ``split_at`` once with multiple split time arguments is much more efficient
         than calling ``split_at`` multiple times with only one split time for
-        :class:`mutwo.core_events.SequentialEvent`.
+        :class:`mutwo.core_events.Consecution`.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(3)])
-        >>> sequential_event.split_at(1)
-        (SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))]))
-        >>> sequential_event[0].split_at(1)
-        (SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 2)))
+        >>> cns = core_events.Consecution([core_events.Chronon(3)])
+        >>> cns.split_at(1)
+        (Consecution([Chronon(duration=DirectDuration(1.0))]), Consecution([Chronon(duration=DirectDuration(2.0))]))
+        >>> cns[0].split_at(1)
+        (Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(2.0)))
         """
         if not absolute_time:
             raise core_utilities.NoSplitTimeError()
 
-        absolute_time_list = list(sorted(absolute_time))
+        abst_list = list(
+            sorted([core_parameters.abc.Duration.from_any(t) for t in absolute_time])
+        )
         # Already sorted => check if smallest t < 0
-        self._assert_valid_absolute_time(absolute_time_list[0])
-        if 0 not in absolute_time_list:
-            absolute_time_list.insert(0, core_parameters.DirectDuration(0))
-
-        if (duration := self.duration) > absolute_time_list[-1]:
-            absolute_time_list.append(duration)
-        elif duration < absolute_time_list[-1] and not ignore_invalid_split_point:
-            raise core_utilities.SplitError(absolute_time_list[-1])
+        self._assert_valid_absolute_time(abst_list[0])
+        if 0 not in abst_list:
+            abst_list.insert(0, core_parameters.DirectDuration(0))
+
+        if (dur := self.duration) > abst_list[-1]:
+            abst_list.append(dur)
+        elif dur < abst_list[-1] and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(abst_list[-1])
 
         split_event_list = []
-        for t0, t1 in zip(absolute_time_list, absolute_time_list[1:]):
+        for t0, t1 in zip(abst_list, abst_list[1:]):
             try:
-                split_event_list.append(self.cut_out(t0, t1, mutate=False))
+                split_event_list.append(self.copy().cut_out(t0, t1))
             except (
                 core_utilities.InvalidStartAndEndValueError,
                 core_utilities.InvalidCutOutStartAndEndValuesError,
             ):
                 if not ignore_invalid_split_point:
                     raise core_utilities.SplitError(t0)
 
@@ -560,87 +547,84 @@
 
 T = typing.TypeVar("T", bound=Event)
 
 
 # FIXME(This Event can be initialised (no abstract error).
 # Please see the following issue for comparison:
 #   https://bugs.python.org/issue35815
-class ComplexEvent(Event, abc.ABC, list[T], typing.Generic[T]):
+class Compound(Event, abc.ABC, list[T], typing.Generic[T]):
     """Abstract Event-Object, which contains other Event-Objects."""
 
+    _short_name_length = 4
+
     def __init__(
         self,
         iterable: typing.Iterable[T] = [],
-        tempo_envelope: typing.Optional[core_events.TempoEnvelope] = None,
+        *,
+        tempo: typing.Optional[core_parameters.abc.Tempo] = None,
+        tag: typing.Optional[str] = None,
     ):
-        Event.__init__(self, tempo_envelope)
+        Event.__init__(self, tempo, tag)
         list.__init__(self, iterable)
-        self._logger = core_utilities.get_cls_logger(type(self))
 
     def __init_subclass__(
         cls, class_specific_side_attribute_tuple: tuple[str, ...] = tuple([])
     ):
         # It's better to prove `class_specific_side_attribute_tuple`
         # as a class initialisation attribute instead of a simple class attribute,
         # because with a simple class attribute we have no guarantee that the
         # content of the parent class is available and we always have to explicitly
         # make it available with something like:
         #
-        #   class MyComplexEvent(ComplexEvent):
+        #   class MyCompound(Compound):
         #        _class_specific_side_attribute_tuple = (("new_attribute",) +
-        #          ComplexEvent._class_specific_side_attribute_tuple)
+        #          Compound._class_specific_side_attribute_tuple)
         #
         # With __init_subclass__ we can simply write:
         #
-        #   class MyComplexEvent(
-        #     ComplexEvent,
+        #   class MyCompound(
+        #     Compound,
         #    class_specific_side_attribute_tuple = ("new_attribute",)
         #   ): pass
         #
-        super_class_class_specific_side_attribute_tuple = getattr(
-            cls, "_class_specific_side_attribute_tuple", ("tempo_envelope",)
-        )
-        class_specific_side_attribute_tuple = (
-            super_class_class_specific_side_attribute_tuple
-            + class_specific_side_attribute_tuple
+        super_class_attr_tuple = getattr(
+            cls, "_class_specific_side_attribute_tuple", ("tempo", "tag")
         )
-        cls._class_specific_side_attribute_tuple = class_specific_side_attribute_tuple
+        class_attr_tuple = super_class_attr_tuple + class_specific_side_attribute_tuple
+        cls._class_specific_side_attribute_tuple = class_attr_tuple
 
     # ###################################################################### #
     #                           magic methods                                #
     # ###################################################################### #
 
-    def __repr__(self) -> str:
-        return "{}({})".format(type(self).__name__, super().__repr__())
-
-    def __add__(self, event: list[T]) -> ComplexEvent[T]:
-        empty_copy = self.empty_copy()
-        empty_copy.extend(super().__add__(event))
-        return empty_copy
-
-    def __mul__(self, factor: int) -> ComplexEvent[T]:
-        empty_copy = self.empty_copy()
-        empty_copy.extend(super().__mul__(factor))
-        return empty_copy
+    def __add__(self, event: list[T]) -> Compound[T]:
+        e = self.empty_copy()
+        e.extend(super().__add__(event))
+        return e
+
+    def __mul__(self, factor: int) -> Compound[T]:
+        e = self.empty_copy()
+        e.extend(super().__mul__(factor))
+        return e
 
     @typing.overload
     def __getitem__(self, index_or_slice_or_tag: int) -> T:
         ...
 
     @typing.overload
-    def __getitem__(self, index_or_slice_or_tag: slice) -> ComplexEvent[T]:
+    def __getitem__(self, index_or_slice_or_tag: slice) -> Compound[T]:
         ...
 
     @typing.overload
     def __getitem__(self, index_or_slice_or_tag: str) -> T:
         ...
 
     def __getitem__(
         self, index_or_slice_or_tag: int | slice | str
-    ) -> T | ComplexEvent[T]:
+    ) -> T | Compound[T]:
         try:
             event = super().__getitem__(index_or_slice_or_tag)
         except TypeError as error:
             if isinstance(index_or_slice_or_tag, str):
                 return self.__getitem__(self._tag_to_index(index_or_slice_or_tag))
             # It can't be a tag, therefore simply raise
             # original exception.
@@ -701,325 +685,313 @@
             # original exception.
             raise error
 
     def __eq__(self, other: typing.Any) -> bool:
         """Test for checking if two objects are equal."""
         try:
             parameter_to_compare_set = set([])
-            for object_ in (self, other):
-                for (
-                    parameter_to_compare
-                ) in object_._class_specific_side_attribute_tuple:
-                    parameter_to_compare_set.add(parameter_to_compare)
+            for obj in (self, other):
+                for param in obj._class_specific_side_attribute_tuple:
+                    parameter_to_compare_set.add(param)
         except AttributeError:
             return False
         return core_utilities.test_if_objects_are_equal_by_parameter_tuple(
             self, other, tuple(parameter_to_compare_set)
         ) and super().__eq__(other)
 
     def __ne__(self, other: typing.Any):
         return not self.__eq__(other)
 
+    def __repr_content__(self):
+        return list.__repr__(self)
+
+    def __str_content__(self):
+        return ", ".join([str(e) for e in self])
+
     # ###################################################################### #
     #                           properties                                   #
     # ###################################################################### #
 
     @Event.duration.setter  # type: ignore
-    def duration(self, duration: core_parameters.abc.Duration):
+    def duration(self, duration: core_parameters.abc.Duration.Type):
         if not self:  # If empty and duration == 0, we'd run into ZeroDivision
-            raise core_utilities.CannotSetDurationOfEmptyComplexEvent()
+            raise core_utilities.CannotSetDurationOfEmptyCompound()
 
-        duration = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
-        if (old_duration := self.duration) != 0:
+        durf = core_parameters.abc.Duration.from_any(duration).beat_count
+        if (old_durf := self.duration.beat_count) != 0:
 
             def f(event_duration: core_parameters.abc.Duration):
                 return core_utilities.scale(
-                    event_duration, 0, old_duration, 0, duration
+                    event_duration.beat_count, 0, old_durf, 0, durf
                 )
 
         else:
             f = duration / len(self)
 
         self.set_parameter("duration", f)
 
     # ###################################################################### #
     #                           private methods                              #
     # ###################################################################### #
 
     # Keep private because:
     #   (1) Then we can later change the internal implementation of
-    #       ComplexEvent (for instance: no longer inheriting from list).
+    #       Compound (for instance: no longer inheriting from list).
     #   (2) It's not sure if tag_to_index is valuable for end users of
-    #       ComplexEvent
+    #       Compound
     def _tag_to_index(self, tag: str) -> int:
         # Find index of an event by its tag.
         # param tag: The `tag` of the event which shall be found.
         # type tag: str
-
-        for event_index, event in enumerate(self):
-            try:
-                event_tag = event.tag
-            except AttributeError:
-                continue
-            if tag == event_tag:
-                return event_index
+        for i, e in enumerate(self):
+            if tag == e.tag:
+                return i
         raise KeyError(f"No event found with tag = '{tag}'.")
 
-    def _assert_start_in_range(self, start: core_parameters.abc.Duration):
+    def _assert_start_in_range(
+        self, start: core_parameters.abc.Duration | core_constants.Real
+    ):
         """Helper method to make sure that start < event.duration.
 
         Can be used within the different squash_in methods.
         """
         if self.duration < start:
             raise core_utilities.InvalidStartValueError(start, self.duration)
 
     def _apply_once_per_event(
         self, method_name: str, *args, id_set: set[int], **kwargs
-    ):
-        for event in self:
-            if (event_id := id(event)) not in id_set:
-                id_set.add(event_id)
-                getattr(event, method_name)(*args, id_set=id_set, **kwargs)
+    ) -> Compound[T]:
+        for e in self:
+            if (e_id := id(e)) not in id_set:
+                id_set.add(e_id)
+                getattr(e, method_name)(*args, id_set=id_set, **kwargs)
+        return self
 
-    @core_utilities.add_copy_option
     def _set_parameter(  # type: ignore
         self,
         parameter_name: str,
-        object_or_function: typing.Callable[
-            [core_constants.ParameterType], core_constants.ParameterType
-        ]
-        | core_constants.ParameterType,
+        object_or_function: typing.Callable[[typing.Any], typing.Any] | typing.Any,
         set_unassigned_parameter: bool,
         id_set: set[int],
-    ) -> ComplexEvent[T]:
-        self._apply_once_per_event(
+    ) -> Compound[T]:
+        return self._apply_once_per_event(
             "_set_parameter",
             parameter_name,
             object_or_function,
             id_set=id_set,
             set_unassigned_parameter=set_unassigned_parameter,
         )
 
-    @core_utilities.add_copy_option
     def _mutate_parameter(  # type: ignore
         self,
         parameter_name: str,
-        function: typing.Callable[[core_constants.ParameterType], None] | typing.Any,
+        function: typing.Callable[[typing.Any], None] | typing.Any,
         id_set: set[int],
-    ) -> ComplexEvent[T]:
-        self._apply_once_per_event(
+    ) -> Compound[T]:
+        return self._apply_once_per_event(
             "_mutate_parameter",
             parameter_name,
             function,
             id_set=id_set,
         )
 
-    def _concatenate_tempo_envelope(self, other: ComplexEvent):
+    def _concatenate_tempo(self, other: Compound):
         """Concatenate the tempo of event with tempo of other event.
 
         If we concatenate events on the time axis, we also want to
         ensure that the tempo information is not lost.
-        This includes the `+` magic method of ``SequentialEvent``,
-        but also the `concatenate_by...` methods of ``SimultaneousEvent``.
+        This includes the `+` magic method of ``Consecution``,
+        but also the `concatenate_by...` methods of ``Concurrence``.
 
         It's important to first call this method before appending the
         child events of the other container, because we still need
         to know the original duration of the target event. Due to this
         difficulty this method is private.
         """
-        # We need to ensure the tempo envelope of the event
-        # is as long as it's duration, otherwise the others tempo
-        # envelope may be postponed (if our envelope is longer
-        # than the event) or may be too early (if our envelope
-        # is shorted than the event).
-        # We don't care here if the others event envelope is too
+        # Trivial case: if tempo doesn't change and isn't flex, we
+        # don't need to do anything to preserve the tempo of the other event.
+        is_not_flex = map(
+            lambda t: not isinstance(t, core_parameters.FlexTempo),
+            (self.tempo, other.tempo),
+        )
+        if all(is_not_flex) and self.tempo == other.tempo:
+            return
+
+        # Convert to flex tempo, to easily handle tempos.
+        for o in (self, other):
+            o.tempo = core_parameters.FlexTempo.from_parameter(o.tempo)
+
+        # We need to ensure the tempo of the event is as long as
+        # it's duration, otherwise the others tempo may be
+        # postponed (if our envelope is longer than the event)
+        # or may be too early (if our tempo is shorted than the event).
+        # We don't care here if the others event tempo is too
         # short or too long, because the relationships are still
         # the same.
-        if (d := self.duration) < (d_env := self.tempo_envelope.duration):
+        if (d := self.duration) < (d_env := self.tempo.duration):
             self._logger.warning(
                 f"Tempo envelope of '{str(self)[:35]}...' needed "
                 "to be truncated because the envelope was "
                 "longer than the actual event."
             )
-            self.tempo_envelope.cut_out(0, d)
+            self.tempo.cut_out(0, d)
         elif d > d_env:
-            self.tempo_envelope.extend_until(d)
-        self.tempo_envelope.extend(other.tempo_envelope.copy())
+            self.tempo.extend_until(d)
+        self.tempo.extend(other.tempo.copy())
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
-    def destructive_copy(self) -> ComplexEvent[T]:
+    def destructive_copy(self) -> Compound[T]:
         empty_copy = self.empty_copy()
         empty_copy.extend([event.destructive_copy() for event in self])
         return empty_copy
 
-    def empty_copy(self) -> ComplexEvent[T]:
-        """Make a copy of the `ComplexEvent` without any child events.
+    def empty_copy(self) -> Compound[T]:
+        """Make a copy of the `Compound` without any child events.
 
-        This method is useful if one wants to copy an instance of :class:`ComplexEvent`
+        This method is useful if one wants to copy an instance of :class:`Compound`
         and make sure that all side attributes (e.g. any assigned properties specific
         to the respective subclass) get saved.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> piano_voice_0 = core_events.TaggedSequentialEvent([core_events.SimpleEvent(2)], tag="piano")
+        >>> piano_voice_0 = core_events.Consecution([core_events.Chronon(2)], tag="piano")
         >>> piano_voice_1 = piano_voice_0.empty_copy()
         >>> piano_voice_1.tag
         'piano'
         >>> piano_voice_1
-        TaggedSequentialEvent([])
+        Consecution([])
         """
         return type(self)(
             [],
-            **{
-                attribute_name: getattr(self, attribute_name)
-                for attribute_name in self._class_specific_side_attribute_tuple
-            },
+            **{a: getattr(self, a) for a in self._class_specific_side_attribute_tuple},
         )
 
     def get_event_from_index_sequence(
         self, index_sequence: typing.Sequence[int]
     ) -> Event:
         """Get nested :class:`Event` from a sequence of indices.
 
         :param index_sequence: The indices of the nested :class:`Event`.
         :type index_sequence: typing.Sequence[int]
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> nested_sequential_event = core_events.SequentialEvent(
-        ...     [core_events.SequentialEvent([core_events.SimpleEvent(2)])]
+        >>> nested_consecution = core_events.Consecution(
+        ...     [core_events.Consecution([core_events.Chronon(2)])]
         ... )
-        >>> nested_sequential_event.get_event_from_index_sequence((0, 0))
-        SimpleEvent(duration = DirectDuration(duration = 2))
+        >>> nested_consecution.get_event_from_index_sequence((0, 0))
+        Chronon(duration=DirectDuration(2.0))
         >>> # this is equal to:
-        >>> nested_sequential_event[0][0]
-        SimpleEvent(duration = DirectDuration(duration = 2))
+        >>> nested_consecution[0][0]
+        Chronon(duration=DirectDuration(2.0))
         """
 
         return core_utilities.get_nested_item_from_index_sequence(index_sequence, self)
 
     def get_parameter(
         self, parameter_name: str, flat: bool = False, filter_undefined: bool = False
-    ) -> tuple[core_constants.ParameterType, ...]:
-        parameter_value_list: list[core_constants.ParameterType] = []
-        for event in self:
-            parameter_value_or_parameter_value_tuple = event.get_parameter(
-                parameter_name, flat=flat
-            )
-
-            if is_simple_event := isinstance(event, core_events.SimpleEvent):
-                parameter_value_tuple = (parameter_value_or_parameter_value_tuple,)
+    ) -> tuple[typing.Any, ...]:
+        plist: list[typing.Any] = []
+        for e in self:
+            param_or_param_tuple = e.get_parameter(parameter_name, flat=flat)
+            if is_chronon := isinstance(e, core_events.Chronon):
+                param_tuple = (param_or_param_tuple,)
             else:
-                parameter_value_tuple = parameter_value_or_parameter_value_tuple
+                param_tuple = param_or_param_tuple
             if filter_undefined:
-                parameter_value_tuple = tuple(
-                    filter(
-                        lambda parameter_value: parameter_value is not None,
-                        parameter_value_tuple,
-                    )
-                )
+                param_tuple = tuple(filter(lambda v: v is not None, param_tuple))
             if flat:
-                parameter_value_list.extend(parameter_value_tuple)
+                plist.extend(param_tuple)
             else:
                 # Simple events should be added without tuple, they only
                 # provide one parameter.
-                if is_simple_event:
-                    if parameter_value_tuple:
-                        parameter_value_list.append(parameter_value_tuple[0])
+                if is_chronon:
+                    if param_tuple:
+                        plist.append(param_tuple[0])
                 else:
-                    parameter_value_list.append(parameter_value_tuple)
-        return tuple(parameter_value_list)
+                    plist.append(param_tuple)
+        return tuple(plist)
 
-    @core_utilities.add_copy_option
     def remove_by(  # type: ignore
         self, condition: typing.Callable[[Event], bool]
-    ) -> ComplexEvent[T]:
+    ) -> Compound[T]:
         """Condition-based deletion of child events.
 
         :param condition: Function which takes a :class:`Event` and returns ``True``
             or ``False``. If the return value of the function is ``False`` the
             respective `Event` will be deleted.
         :type condition: typing.Callable[[Event], bool]
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> simultaneous_event = core_events.SimultaneousEvent(
-        ...     [core_events.SimpleEvent(1), core_events.SimpleEvent(3), core_events.SimpleEvent(2)]
+        >>> concurrence = core_events.Concurrence(
+        ...     [core_events.Chronon(1), core_events.Chronon(3), core_events.Chronon(2)]
         ... )
-        >>> simultaneous_event.remove_by(lambda event: event.duration > 2)
-        SimultaneousEvent([SimpleEvent(duration = DirectDuration(duration = 3))])
+        >>> concurrence.remove_by(lambda event: event.duration > 2)
+        Concurrence([Chronon(duration=DirectDuration(3.0))])
         """
+        for i, e in zip(reversed(range(len(self))), reversed(self)):
+            if not condition(e):
+                del self[i]
+        return self
 
-        for item_index, item in zip(reversed(range(len(self))), reversed(self)):
-            shall_survive = condition(item)
-            if not shall_survive:
-                del self[item_index]
-
-    @core_utilities.add_copy_option
     def tie_by(  # type: ignore
         self,
         condition: typing.Callable[[Event, Event], bool],
         process_surviving_event: typing.Callable[
             [Event, Event], None
         ] = lambda event_to_survive, event_to_delete: event_to_survive.__setattr__(
             "duration", event_to_delete.duration + event_to_survive.duration
         ),
         event_type_to_examine: typing.Type[Event] = Event,
         event_to_remove: bool = True,
-    ) -> ComplexEvent[T]:
+    ) -> Compound[T]:
         """Condition-based deletion of neighboring child events.
 
         :param condition: Function which compares two neighboring
             events and decides whether one of those events shall be
             removed. The function should return `True` for deletion and
             `False` for keeping both events.
         :param process_surviving_event: Function which gets two arguments: first
             the surviving event and second the event which shall be removed.
             The function should process the surviving event depending on
             the removed event. By default, mutwo will simply add the
             :attr:`duration` of the removed event to the duration of the surviving
             event.
         :param event_type_to_examine: Defines which events shall be compared.
             If one only wants to process the leaves, this should perhaps be
-            :class:`mutwo.core_events.SimpleEvent`.
+            :class:`mutwo.core_events.Chronon`.
         :param event_to_remove: `True` if the second (left) event shall be removed
             and `False` if the first (right) event shall be removed.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
         """
 
         # Nothing to tie if no child events exist
         if not self:
             return self
 
-        def tie_by_if_available(event_to_tie: Event):
-            if hasattr(event_to_tie, "tie_by"):
-                event_to_tie.tie_by(
+        def tie_by_if_available(e: Event):
+            if hasattr(e, "tie_by"):
+                e.tie_by(
                     condition,
                     process_surviving_event,
                     event_type_to_examine,
                     event_to_remove,
                 )
 
         pointer = 0
         while pointer + 1 < len(self):
             event_tuple = self[pointer], self[pointer + 1]
-            if all(isinstance(event, event_type_to_examine) for event in event_tuple):
-                shall_delete = condition(*event_tuple)
-                if shall_delete:
+            if all(isinstance(e, event_type_to_examine) for e in event_tuple):
+                if condition(*event_tuple):  # shall_delete
                     if event_to_remove:
                         process_surviving_event(*event_tuple)
                         del self[pointer + 1]
                     else:
                         process_surviving_event(*reversed(event_tuple))
                         del self[pointer]
                 else:
@@ -1032,132 +1004,118 @@
                 pointer += 1
 
         # Previously only the first event of the examined pairs has been tied,
         # therefore the very last event could have been forgotten.
         if not isinstance(self[-1], event_type_to_examine):
             tie_by_if_available(self[-1])
 
+        return self
+
+    def metrize(self) -> Compound:
+        metrized_event = self._event_to_metrized_event(self)
+        self.tempo = metrized_event.tempo
+        self[:] = metrized_event[:]
+        return self
+
     # ###################################################################### #
     #                           abstract methods                             #
     # ###################################################################### #
 
-    def metrize(self, mutate: bool = True) -> ComplexEvent:
-        metrized_event = self._event_to_metrized_event(self)
-        if mutate:
-            self.tempo_envelope = metrized_event.tempo_envelope
-            self[:] = metrized_event[:]
-            return self
-        else:
-            return metrized_event
-
     @abc.abstractmethod
     def squash_in(
-        self, start: core_parameters.abc.Duration, event_to_squash_in: Event
-    ) -> typing.Optional[ComplexEvent[T]]:
+        self, start: core_parameters.abc.Duration.Type, event_to_squash_in: Event
+    ) -> typing.Optional[Compound[T]]:
         """Time-based insert of a new event with overriding given event.
 
         :param start: Absolute time where the event shall be inserted.
         :param event_to_squash_in: the event that shall be squashed into
             the present event.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
-        Unlike `ComplexEvent.slide_in` the events duration won't change.
+        Unlike `Compound.slide_in` the events duration won't change.
         If there is already an event at `start` this event will be shortened
         or removed.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(3)])
-        >>> sequential_event.squash_in(1, core_events.SimpleEvent(1.5))
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 3/2)), SimpleEvent(duration = DirectDuration(duration = 1/2))])
+        >>> consecution = core_events.Consecution([core_events.Chronon(3)])
+        >>> consecution.squash_in(1, core_events.Chronon(1.5))
+        Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(1.5)), Chronon(duration=DirectDuration(0.5))])
         """
 
     @abc.abstractmethod
     def slide_in(
-        self, start: core_parameters.abc.Duration, event_to_slide_in: Event
-    ) -> ComplexEvent[T]:
+        self, start: core_parameters.abc.Duration.Type, event_to_slide_in: Event
+    ) -> Compound[T]:
         """Time-based insert of a new event into the present event.
 
         :param start: Absolute time where the event shall be inserted.
         :param event_to_slide_in: the event that shall be slide into
             the present event.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
-        Unlike `ComplexEvent.squash_in` the events duration will be prolonged
+        Unlike `Compound.squash_in` the events duration will be prolonged
         by the event which is added. If there is an event at `start` the
         event will be split into two parts, but it won't be shortened or
         processed in any other way.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(3)])
-        >>> sequential_event.slide_in(1, core_events.SimpleEvent(1.5))
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 3/2)), SimpleEvent(duration = DirectDuration(duration = 2))])
+        >>> consecution = core_events.Consecution([core_events.Chronon(3)])
+        >>> consecution.slide_in(1, core_events.Chronon(1.5))
+        Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(1.5)), Chronon(duration=DirectDuration(2.0))])
         """
 
     @abc.abstractmethod
     def split_child_at(
-        self, absolute_time: core_parameters.abc.Duration
-    ) -> typing.Optional[ComplexEvent[T]]:
+        self, absolute_time: core_parameters.abc.Duration.Type
+    ) -> typing.Optional[Compound[T]]:
         """Split child event in two events at :attr:`absolute_time`.
 
         :param absolute_time: where child event shall be split
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(3)])
-        >>> sequential_event.split_child_at(1)
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 2))])
+        >>> consecution = core_events.Consecution([core_events.Chronon(3)])
+        >>> consecution.split_child_at(1)
+        Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(2.0))])
         """
 
     @abc.abstractmethod
     def extend_until(
         self,
-        duration: core_parameters.abc.Duration,
+        duration: core_parameters.abc.Duration.Type,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], Event]
         ] = None,
-        prolong_simple_event: bool = True,
-    ) -> ComplexEvent:
+        prolong_chronon: bool = True,
+    ) -> Compound:
         """Prolong event until at least `duration` by appending an empty event.
 
         :param duration: Until which duration the event shall be extended.
             If event is already longer than or equal to given `duration`,
-            nothing will be changed. For :class:`~mutwo.core_events.SimultaneousEvent`
+            nothing will be changed. For :class:`~mutwo.core_events.Concurrence`
             the default value is `None` which is equal to the duration of
-            the `SimultaneousEvent`.
-        :type duration: core_parameters.abc.Duration
+            the `Concurrence`.
+        :type duration: core_parameters.abc.Duration.Type
         :param duration_to_white_space: A function which creates the 'rest' or
             'white space' event from :class:`~mutwo.core_parameters.abc.Duration`.
             If this is ``None`` `mutwo` will fall back to use the default function
             which is `mutwo.core_events.configurations.DEFAULT_DURATION_TO_WHITE_SPACE`.
             Default to `None`.
         :type duration_to_white_space: typing.Optional[typing.Callable[[core_parameters.abc.Duration], Event]]
-        :param prolong_simple_event: If set to ``True`` `mutwo` will prolong a single
-            :class:`~mutwo.core_events.SimpleEvent` inside a :class:`~mutwo.core_events.SimultaneousEvent`.
+        :param prolong_chronon: If set to ``True`` `mutwo` will prolong a single
+            :class:`~mutwo.core_events.Chronon` inside a :class:`~mutwo.core_events.Concurrence`.
             If set to ``False`` `mutwo` will raise an :class:`~mutwo.core_utilities.ImpossibleToExtendUntilError`
-            in case it finds a single `SimpleEvent` inside a `SimultaneousEvent`.
-            This doesn't effect `SimpleEvent` inside a `SequentialEvent`, here we can
+            in case it finds a single `Chronon` inside a `Concurrence`.
+            This doesn't effect `Chronon` inside a `Consecution`, here we can
             simply append a new white space event.
-        :type prolong_simple_event: bool
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
-        :type mutate: bool
+        :type prolong_chronon: bool
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> s = core_events.SequentialEvent([core_events.SimpleEvent(1)])
-        >>> s.extend_until(10)
-        SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 9))])
+        >>> cns = core_events.Consecution([core_events.Chronon(1)])
+        >>> cns.extend_until(10)
+        Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(9.0))])
         """
```

### Comparing `mutwo.core-1.4.0/mutwo/core_events/basic.py` & `mutwo.core-2.0.0/mutwo/core_events/basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,72 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Generic event classes which can be used in multiple contexts.
 
 The different events differ in their timing structure and whether they
 are nested or not:
 """
 
 from __future__ import annotations
 
 import bisect
-import copy
 import functools
 import operator
 import types
 import typing
 
 import ranges
 
-from mutwo import core_constants
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 
-__all__ = (
-    "SimpleEvent",
-    "SequentialEvent",
-    "SimultaneousEvent",
-    "TaggedSimpleEvent",
-    "TaggedSequentialEvent",
-    "TaggedSimultaneousEvent",
-)
+__all__ = ("Chronon", "Consecution", "Concurrence")
 
 
-class SimpleEvent(core_events.abc.Event):
-    """A :class:`SimpleEvent` is an event without any children (a leaf).
+class Chronon(core_events.abc.Event):
+    """A :class:`Chronon` is an event that cannot be further subdivided (a leaf of a tree).
 
-    :param duration: The duration of the ``SimpleEvent``. Mutwo will convert
+    :param duration: The duration of the ``Chronon``. Mutwo converts
         the incoming object to a :class:`mutwo.core_parameters.abc.Duration` object
-        with the global `core_events.configurations.UNKNOWN_OBJECT_TO_DURATION`
+        with the global `core_parameters.abc.Duration.from_any`
         callable.
+    :param *args: Arguments parsed to :class:`mutwo.core_events.abc.Event`.
+    :param **kwargs: Keyword arguments parsed to :class:`mutwo.core_events.abc.Event`.
 
     **Example:**
 
     >>> from mutwo import core_events
-    >>> simple_event = core_events.SimpleEvent(2)
-    >>> print(simple_event)
-    SimpleEvent(duration = DirectDuration(duration = 2))
+    >>> chronon = core_events.Chronon(2)
+    >>> chronon
+    Chronon(duration=DirectDuration(2.0))
+    >>> print(chronon)  # pretty print for debugging
+    C(dur=D(2.0))
     """
 
-    parameter_to_exclude_from_representation_tuple = ("tempo_envelope",)
+    parameter_to_exclude_from_representation_tuple = ("tempo", "tag")
 
-    def __init__(
-        self,
-        duration: core_parameters.abc.Duration,
-        tempo_envelope: typing.Optional[core_events.TempoEnvelope] = None,
-    ):
-        super().__init__(tempo_envelope)
+    def __init__(self, duration: core_parameters.abc.Duration.Type, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.duration = duration
 
     # ###################################################################### #
     #                           magic methods                                #
     # ###################################################################### #
 
     def __eq__(self, other: typing.Any) -> bool:
@@ -70,78 +78,78 @@
                     parameter_to_compare_set.add(parameter_to_compare)
         except AttributeError:
             return False
         return core_utilities.test_if_objects_are_equal_by_parameter_tuple(
             self, other, tuple(parameter_to_compare_set)
         )
 
-    def __repr__(self) -> str:
-        attribute_iterator = (
-            "{} = {}".format(attribute, getattr(self, attribute))
-            for attribute in self._parameter_to_print_tuple
+    def __repr_content__(self) -> str:
+        return ", ".join([f"{attr}={repr(v)}" for attr, v in self._print_data.items()])
+
+    def __str_content__(self) -> str:
+        return ", ".join(
+            [f"{attr[:3]}={str(v)}" for attr, v in self._print_data.items()]
         )
-        return "{}({})".format(type(self).__name__, ", ".join(attribute_iterator))
 
     # ###################################################################### #
     #                           private methods                              #
     # ###################################################################### #
 
-    @core_utilities.add_copy_option
     def _set_parameter(
         self,
         parameter_name: str,
-        object_or_function: typing.Callable[
-            [core_constants.ParameterType], core_constants.ParameterType
-        ]
-        | core_constants.ParameterType,
+        object_or_function: typing.Callable[[typing.Any], typing.Any] | typing.Any,
         set_unassigned_parameter: bool,
         id_set: set[int],
-    ) -> SimpleEvent:
+    ) -> Chronon:
         old_parameter = self.get_parameter(parameter_name)
         if set_unassigned_parameter or old_parameter is not None:
             if hasattr(object_or_function, "__call__"):
                 new_parameter = object_or_function(old_parameter)
             else:
                 new_parameter = object_or_function
             setattr(self, parameter_name, new_parameter)
+        return self
 
-    @core_utilities.add_copy_option
     def _mutate_parameter(
         self,
         parameter_name: str,
-        function: typing.Callable[[core_constants.ParameterType], None] | typing.Any,
+        function: typing.Callable[[typing.Any], None] | typing.Any,
         id_set: set[int],
-    ) -> SimpleEvent:
-        parameter = self.get_parameter(parameter_name)
-        if parameter is not None:
-            function(parameter)
+    ) -> Chronon:
+        if (p := self.get_parameter(parameter_name)) is not None:
+            function(p)
+        return self
 
     # ###################################################################### #
     #                           properties                                   #
     # ###################################################################### #
 
     @property
     def _parameter_to_print_tuple(self) -> tuple[str, ...]:
         """Return tuple of attribute names which shall be printed for repr."""
-        # Fix infinite circular loop (due to 'tempo_envelope')
-        # and avoid printing too verbose parameters.
+        # Avoid printing too verbose parameters.
         return tuple(
             filter(
                 lambda attribute: attribute
                 not in self.parameter_to_exclude_from_representation_tuple,
                 self._parameter_to_compare_tuple,
             )
         )
 
     @property
+    def _print_data(self) -> dict[str, typing.Any]:
+        return {attr: getattr(self, attr) for attr in self._parameter_to_print_tuple}
+
+    @property
     def _parameter_to_compare_tuple(self) -> tuple[str, ...]:
-        """Return tuple of attribute names which values define the :class:`SimpleEvent`.
+        """Return tuple of attribute names which values define the :class:`Chronon`.
 
         The returned attribute names are used for equality check between two
-        :class:`SimpleEvent` objects.
+        :class:`Chronon` objects.
         """
         return tuple(
             attribute
             for attribute in dir(self)
             # We have to use 'and' (lazy evaluation) instead of
             #      'all', to avoid redundant checks!
             #
@@ -154,261 +162,228 @@
         )
 
     @property
     def duration(self) -> core_parameters.abc.Duration:
         return self._duration
 
     @duration.setter
-    def duration(self, duration: core_parameters.abc.Duration):
-        self._duration = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
+    def duration(self, duration: core_parameters.abc.Duration.Type):
+        self._duration = core_parameters.abc.Duration.from_any(duration)
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
-    def destructive_copy(self) -> SimpleEvent:
-        return copy.deepcopy(self)
+    def destructive_copy(self) -> Chronon:
+        return self.copy()
 
     def get_parameter(
         self, parameter_name: str, flat: bool = False, filter_undefined: bool = False
-    ) -> core_constants.ParameterType:
+    ) -> typing.Any:
         return getattr(self, parameter_name, None)
 
     # Update docstring
     def set_parameter(  # type: ignore
         self,
         *args,
         **kwargs,
-    ) -> SimpleEvent:
+    ) -> Chronon:
         """Sets event parameter to new value.
 
         :param parameter_name: The name of the parameter which values shall be changed.
         :param object_or_function: For setting the parameter either a new value can be
             passed directly or a function can be passed. The function gets as an
             argument the previous value that has had been assigned to the respective
-            object and has to return a new value that will be assigned to the object.
-        :param set_unassigned_parameter: If set to ``False`` a new parameter will only
-            be assigned to an Event if the Event already has a attribute with the
+            object and has to return a new value that is assigned to the object.
+        :param set_unassigned_parameter: If set to ``False`` a new parameter is only
+            assigned to an Event if the Event already has a attribute with the
             respective `parameter_name`. If the Event doesn't know the attribute yet
-            and `set_unassigned_parameter` is False, the method call will simply be
+            and `set_unassigned_parameter` is False, the method call is simply
             ignored.
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> simple_event = core_events.SimpleEvent(2)
-        >>> simple_event.set_parameter(
+        >>> chronon = core_events.Chronon(2)
+        >>> chronon.set_parameter(
         ...     'duration', lambda old_duration: old_duration * 2
         ... )
-        SimpleEvent(duration = DirectDuration(duration = 4))
-        >>> simple_event.duration
-        DirectDuration(4)
-        >>> simple_event.set_parameter('duration', 3)
-        SimpleEvent(duration = DirectDuration(duration = 3))
-        >>> simple_event.duration
-        DirectDuration(3)
-        >>> simple_event.set_parameter(
+        Chronon(duration=DirectDuration(4.0))
+        >>> chronon.duration
+        DirectDuration(4.0)
+        >>> chronon.set_parameter('duration', 3)
+        Chronon(duration=DirectDuration(3.0))
+        >>> chronon.duration
+        DirectDuration(3.0)
+        >>> chronon.set_parameter(
         ...     'unknown_parameter', 10, set_unassigned_parameter=False
         ... )  # this will be ignored
-        SimpleEvent(duration = DirectDuration(duration = 3))
-        >>> simple_event.unknown_parameter
+        Chronon(duration=DirectDuration(3.0))
+        >>> chronon.unknown_parameter
         Traceback (most recent call last):
           File "<stdin>", line 1, in <module>
-        AttributeError: 'SimpleEvent' object has no attribute 'unknown_parameter'
-        >>> simple_event.set_parameter(
+        AttributeError: 'Chronon' object has no attribute 'unknown_parameter'
+        >>> chronon.set_parameter(
         ...     'unknown_parameter', 10, set_unassigned_parameter=True
         ... )  # this will be written
-        SimpleEvent(duration = DirectDuration(duration = 3), unknown_parameter = 10)
-        >>> simple_event.unknown_parameter
+        Chronon(duration=DirectDuration(3.0), unknown_parameter=10)
+        >>> chronon.unknown_parameter
         10
         """
-
         return super().set_parameter(*args, **kwargs)
 
-    def metrize(self, mutate: bool = True) -> SimpleEvent:
+    def metrize(self) -> Chronon:
         metrized_event = self._event_to_metrized_event(self)
-        if mutate:
-            self.duration = metrized_event.duration
-            self.tempo_envelope = metrized_event.tempo_envelope
-            return self
-        else:
-            return metrized_event
+        self.duration = metrized_event.duration
+        self.tempo = metrized_event.tempo
+        return self
 
-    @core_utilities.add_copy_option
     def cut_out(  # type: ignore
         self,
-        start: core_parameters.abc.Duration,
-        end: core_parameters.abc.Duration,
-    ) -> SimpleEvent:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Chronon:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(
             start, end, condition=lambda start, end: start < end
         )
 
-        duration = self.duration
-
-        difference_to_duration: core_parameters.DirectDuration = (
-            core_parameters.DirectDuration(0)
-        )
+        dur = self.duration
+        diff: core_parameters.DirectDuration = core_parameters.DirectDuration(0)
 
         if start > 0:
-            difference_to_duration += start
-        if end < duration:
-            difference_to_duration += duration - end
-
-        if difference_to_duration >= duration:
+            diff += start
+        if end < dur:
+            diff += dur - end
+        if diff >= dur:
             raise core_utilities.InvalidCutOutStartAndEndValuesError(
-                start, end, self, duration
+                start, end, self, dur
             )
 
-        self.duration -= difference_to_duration
+        self.duration -= diff
+        return self
 
-    @core_utilities.add_copy_option
     def cut_off(  # type: ignore
         self,
-        start: core_parameters.abc.Duration,
-        end: core_parameters.abc.Duration,
-    ) -> SimpleEvent:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Chronon:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
 
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
 
         duration = self.duration
         if start < duration:
             if end > duration:
                 end = duration
-
             self.duration -= end - start
+        return self
 
 
 T = typing.TypeVar("T", bound=core_events.abc.Event)
 
 
-class SequentialEvent(core_events.abc.ComplexEvent, typing.Generic[T]):
-    """A :class:`SequentialEvent` is a sequence of events."""
+class Consecution(core_events.abc.Compound, typing.Generic[T]):
+    """A :class:`Consecution`hosts events that take place one after the other."""
 
     # ###################################################################### #
     #                           magic methods                                #
     # ###################################################################### #
 
-    def __add__(self, event: list[T]) -> SequentialEvent[T]:
+    def __add__(self, event: list[T]) -> Consecution[T]:
         e = self.copy()
-        e._concatenate_tempo_envelope(event)
+        e._concatenate_tempo(event)
         e.extend(event)
         return e
 
     # ###################################################################### #
     #                    private static methods                              #
     # ###################################################################### #
 
     @staticmethod
     def _get_index_at_from_absolute_time_tuple(
-        absolute_time: float,
-        absolute_time_tuple: float,
+        abst: float,
+        abst_tuple: float,
         duration: float,
     ) -> typing.Optional[int]:
-        if absolute_time < duration and absolute_time >= 0:
-            return bisect.bisect_right(absolute_time_tuple, absolute_time) - 1
+        if abst < duration and abst >= 0:
+            return bisect.bisect_right(abst_tuple, abst) - 1
         else:
             return None
 
     # ###################################################################### #
     #                        private  methods                                #
     # ###################################################################### #
 
     # We need to have a private "_cut_off" method to simplify
     # overriding the public "cut_off" method in children classes
-    # of SequentialEvent. This is necessary, because the implementation
+    # of Consecution. This is necessary, because the implementation
     # of "squash_in" makes use of "_cut_off". In this way it is possible
     # to adjust the meaning of the public "cut_off" method, without
     # having to change the meaning of "squash_in" (this happens for instance
     # in the mutwo.core_events.Envelope class).
     def _cut_off(
         self,
         start: core_parameters.abc.Duration,
         end: core_parameters.abc.Duration,
         cut_off_duration: typing.Optional[core_parameters.abc.Duration] = None,
-    ) -> SequentialEvent[T]:
+    ) -> Consecution[T]:
         if cut_off_duration is None:
             cut_off_duration = end - start
-
-        # Collect core_events which are only active within the
-        # cut_off - range
+        # Collect events which are only active within the cut_off - range
         event_to_delete_list = []
-        absolute_time_tuple = self.absolute_time_tuple
-        for event_index, event_start, event_end, event in zip(
-            range(len(self)),
-            absolute_time_tuple,
-            absolute_time_tuple[1:] + (None,),
-            self,
+        abst_tuple = self.absolute_time_tuple
+        for i, t0, t1, e in zip(
+            range(len(self)), abst_tuple, abst_tuple[1:] + (None,), self
         ):
-            if event_end is None:
-                event_end = event_start + event.duration
-
-            if event_start >= start and event_end <= end:
-                event_to_delete_list.append(event_index)
-
+            if t1 is None:
+                t1 = t0 + e.duration
+            if t0 >= start and t1 <= end:
+                event_to_delete_list.append(i)
             # Shorten event which are partly active within the
             # cut_off - range
-            elif event_start <= start and event_end >= start:
-                difference_to_event_start = start - event_start
-                event.cut_off(
-                    difference_to_event_start,
-                    difference_to_event_start + cut_off_duration,
-                )
-
-            elif event_start < end and event_end > end:
-                difference_to_event_start = event_start - start
-                event.cut_off(0, cut_off_duration - difference_to_event_start)
-
-        for index in reversed(event_to_delete_list):
-            del self[index]
-
+            elif t0 <= start and t1 >= start:
+                diff = start - t0
+                e.cut_off(diff, diff + cut_off_duration)
+            elif t0 < end and t1 > end:
+                diff = t0 - start
+                e.cut_off(0, cut_off_duration - diff)
+        for i in reversed(event_to_delete_list):
+            del self[i]
         return self
 
     def _split_child_at(
         self,
-        absolute_time: core_parameters.abc.Duration | typing.Any,
-        absolute_time_in_floats_tuple: tuple[float, ...],
-        duration_in_floats: float,
+        absolute_time: core_parameters.abc.Duration.Type,
+        abstf_tuple: tuple[float, ...],
+        durf: float,
     ) -> int:
-        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        )
+        absolute_time = core_parameters.abc.Duration.from_any(absolute_time)
         self._assert_valid_absolute_time(absolute_time)
-        absolute_time_in_floats = absolute_time.duration_in_floats
+        abstf = absolute_time.beat_count
 
-        event_index = SequentialEvent._get_index_at_from_absolute_time_tuple(
-            absolute_time_in_floats, absolute_time_in_floats_tuple, duration_in_floats
+        event_index = Consecution._get_index_at_from_absolute_time_tuple(
+            abstf, abstf_tuple, durf
         )
 
         # If there is no event at the requested time, raise error
         if event_index is None:
             raise core_utilities.SplitUnavailableChildError(absolute_time)
 
         # Only try to split child event at the requested time if there isn't
         # a segregation already anyway
-        elif absolute_time_in_floats != absolute_time_in_floats_tuple[event_index]:
+        elif abstf != abstf_tuple[event_index]:
             try:
-                end = absolute_time_in_floats_tuple[event_index + 1]
+                end = abstf_tuple[event_index + 1]
             except IndexError:
-                end = duration_in_floats
+                end = durf
 
-            difference = end - absolute_time_in_floats
+            difference = end - abstf
             split_event = self[event_index].split_at(difference)
             split_event_count = len(split_event)
             match split_event_count:
                 case 1:
                     pass
                 case 2:
                     self[event_index] = split_event[0]
@@ -420,450 +395,399 @@
         return event_index
 
     # ###################################################################### #
     #                        private   properties                            #
     # ###################################################################### #
 
     @property
-    def _absolute_time_tuple_and_duration(
+    def _abst_tuple_and_dur(
         self,
     ) -> [tuple[core_parameters.abc.Duration, ...], core_parameters.abc.Duration]:
         """Return start time for each event and the end time of the last event.
 
         This property helps to improve performance of various functions
         which uses duration and absolute_time_tuple attribute.
         """
-
-        duration_iterator = (event.duration for event in self)
-        absolute_time_tuple = tuple(
-            core_utilities.accumulate_from_n(
-                duration_iterator, core_parameters.DirectDuration(0)
-            )
+        d_iter = (e.duration for e in self)
+        abst_tuple = tuple(
+            core_utilities.accumulate_from_n(d_iter, core_parameters.DirectDuration(0))
         )
-        return absolute_time_tuple[:-1], absolute_time_tuple[-1]
+        return abst_tuple[:-1], abst_tuple[-1]
 
     @property
-    def _absolute_time_in_floats_tuple_and_duration(
+    def _abstf_tuple_and_dur(
         self,
     ) -> tuple[tuple[float, ...], float]:
         """Return start time for each event and the end time of the last event.
 
         This property helps to improve performance of various functions
         which uses duration and absolute_time_tuple attribute.
         """
-
-        duration_iterator = (event.duration.duration_in_floats for event in self)
-        absolute_time_tuple = tuple(
+        d_iter = (e.duration.beat_count for e in self)
+        abstf_tuple = tuple(
             # We need to round each duration again after accumulation,
             # because floats were summed which could lead to
             # potential floating point errors again, which will
             # lead to bad errors later (for instance in
             # core_utilities.scale).
             map(
                 lambda d: core_utilities.round_floats(
                     d,
                     core_parameters.configurations.ROUND_DURATION_TO_N_DIGITS,
                 ),
-                core_utilities.accumulate_from_n(duration_iterator, 0),
+                core_utilities.accumulate_from_n(d_iter, 0),
             )
         )
-        return absolute_time_tuple[:-1], absolute_time_tuple[-1]
+        return abstf_tuple[:-1], abstf_tuple[-1]
 
     # ###################################################################### #
     #                           properties                                   #
     # ###################################################################### #
 
-    @core_events.abc.ComplexEvent.duration.getter
+    @core_events.abc.Compound.duration.getter
     def duration(self) -> core_parameters.abc.Duration:
         try:
-            return functools.reduce(operator.add, (event.duration for event in self))
-        # If SequentialEvent is empty
+            return functools.reduce(operator.add, (e.duration for e in self))
+        # If Consecution is empty
         except TypeError:
             return core_parameters.DirectDuration(0)
 
     @property
     def absolute_time_tuple(self) -> tuple[core_parameters.abc.Duration, ...]:
         """Return start time as :class:`core_parameters.abc.Duration` for each event."""
-        return self._absolute_time_tuple_and_duration[0]
+        return self._abst_tuple_and_dur[0]
 
     @property
     def absolute_time_in_floats_tuple(self) -> tuple[float, ...]:
         """Return start time as `float` for each event."""
-        return self._absolute_time_in_floats_tuple_and_duration[0]
+        return self._abstf_tuple_and_dur[0]
 
     @property
     def start_and_end_time_per_event(
         self,
     ) -> tuple[ranges.Range, ...]:
         """Return start and end time for each event."""
-
-        duration_iterator = (event.duration for event in self)
-        absolute_time_tuple = tuple(
-            core_utilities.accumulate_from_n(
-                duration_iterator, core_parameters.DirectDuration(0)
-            )
-        )
-        return tuple(
-            ranges.Range(*start_and_end_time)
-            for start_and_end_time in zip(absolute_time_tuple, absolute_time_tuple[1:])
+        d_iter = (e.duration for e in self)
+        abst_tuple = tuple(
+            core_utilities.accumulate_from_n(d_iter, core_parameters.DirectDuration(0))
         )
+        return tuple(ranges.Range(*t) for t in zip(abst_tuple, abst_tuple[1:]))
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
     def get_event_index_at(
-        self, absolute_time: core_parameters.abc.Duration | typing.Any
+        self, absolute_time: core_parameters.abc.Duration.Type
     ) -> typing.Optional[int]:
         """Get index of event which is active at the passed absolute_time.
 
         :param absolute_time: The absolute time where the method shall search
             for the active event.
-        :type absolute_time: core_parameters.abc.Duration | typing.Any
+        :type absolute_time: core_parameters.abc.Duration.Type
         :return: Index of event if there is any event at the requested absolute time
             and ``None`` if there isn't any event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(2), core_events.SimpleEvent(3)])
-        >>> sequential_event.get_event_index_at(1)
+        >>> consecution = core_events.Consecution([core_events.Chronon(2), core_events.Chronon(3)])
+        >>> consecution.get_event_index_at(1)
         0
-        >>> sequential_event.get_event_index_at(3)
+        >>> consecution.get_event_index_at(3)
         1
-        >>> sequential_event.get_event_index_at(100)
+        >>> consecution.get_event_index_at(100)
 
         **Warning:**
 
         This method ignores events with duration == 0.
         """
-
-        absolute_time_in_floats = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        ).duration_in_floats
-        (
-            absolute_time_in_floats_tuple,
-            duration_in_floats,
-        ) = self._absolute_time_in_floats_tuple_and_duration
-        return SequentialEvent._get_index_at_from_absolute_time_tuple(
-            absolute_time_in_floats, absolute_time_in_floats_tuple, duration_in_floats
+        abstf = core_parameters.abc.Duration.from_any(absolute_time).beat_count
+        abstf_tuple, durf = self._abstf_tuple_and_dur
+        return Consecution._get_index_at_from_absolute_time_tuple(
+            abstf, abstf_tuple, durf
         )
 
     def get_event_at(
-        self, absolute_time: core_parameters.abc.Duration | typing.Any
+        self, absolute_time: core_parameters.abc.Duration.Type
     ) -> typing.Optional[T]:
         """Get event which is active at the passed absolute_time.
 
         :param absolute_time: The absolute time where the method shall search
             for the active event.
-        :type absolute_time: core_parameters.abc.Duration | typing.Any
+        :type absolute_time: core_parameters.abc.Duration.Type
         :return: Event if there is any event at the requested absolute time
             and ``None`` if there isn't any event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> sequential_event = core_events.SequentialEvent([core_events.SimpleEvent(2), core_events.SimpleEvent(3)])
-        >>> sequential_event.get_event_at(1)
-        SimpleEvent(duration = DirectDuration(duration = 2))
-        >>> sequential_event.get_event_at(3)
-        SimpleEvent(duration = DirectDuration(duration = 3))
-        >>> sequential_event.get_event_at(100)
+        >>> consecution = core_events.Consecution([core_events.Chronon(2), core_events.Chronon(3)])
+        >>> consecution.get_event_at(1)
+        Chronon(duration=DirectDuration(2.0))
+        >>> consecution.get_event_at(3)
+        Chronon(duration=DirectDuration(3.0))
+        >>> consecution.get_event_at(100)
 
         **Warning:**
 
         This method ignores events with duration == 0.
         """
-
         event_index = self.get_event_index_at(absolute_time)
         if event_index is None:
             return None
-        else:
-            return self[event_index]  # type: ignore
+        return self[event_index]  # type: ignore
 
-    @core_utilities.add_copy_option
     def cut_out(  # type: ignore
         self,
-        start: core_constants.DurationType,
-        end: core_constants.DurationType,
-    ) -> SequentialEvent[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Consecution[T]:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
 
         event_to_remove_index_list = []
-        for event_index, event_start, event in zip(
-            range(len(self)), self.absolute_time_tuple, self
-        ):
-            event_duration = event.duration
-            event_end = event_start + event_duration
-
+        for i, t0, e in zip(range(len(self)), self.absolute_time_tuple, self):
+            event_duration = e.duration
+            t1 = t0 + event_duration
             cut_out_start: core_parameters.DirectDuration = (
                 core_parameters.DirectDuration(0)
             )
             cut_out_end = event_duration
-
-            if event_start < start:
-                cut_out_start += start - event_start
-
-            if event_end > end:
-                cut_out_end -= event_end - end
-
+            if t0 < start:
+                cut_out_start += start - t0
+            if t1 > end:
+                cut_out_end -= t1 - end
             if cut_out_start < cut_out_end:
-                event.cut_out(cut_out_start, cut_out_end)
+                e.cut_out(cut_out_start, cut_out_end)
             elif not (
                 # Support special case of events with duration = 0.
-                event.duration == 0
-                and event_start >= start
-                and event_start <= end
+                e.duration == 0
+                and t0 >= start
+                and t0 <= end
             ):
-                event_to_remove_index_list.append(event_index)
+                event_to_remove_index_list.append(i)
 
         for event_to_remove_index in reversed(event_to_remove_index_list):
             del self[event_to_remove_index]
+        return self
 
-    @core_utilities.add_copy_option
     def cut_off(  # type: ignore
         self,
-        start: core_constants.DurationType,
-        end: core_constants.DurationType,
-    ) -> SequentialEvent[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Consecution[T]:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
-
         cut_off_duration = end - start
-
         # Avoid unnecessary iterations
         if cut_off_duration > 0:
             return self._cut_off(start, end, cut_off_duration)
+        return self
 
-    @core_utilities.add_copy_option
     def squash_in(  # type: ignore
         self,
-        start: core_parameters.abc.Duration | typing.Any,
+        start: core_parameters.abc.Duration.Type,
         event_to_squash_in: core_events.abc.Event,
-    ) -> SequentialEvent[T]:
-        start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+    ) -> Consecution[T]:
+        start = core_parameters.abc.Duration.from_any(start)
         self._assert_valid_absolute_time(start)
-        start_in_floats = start.duration_in_floats
+        start_in_floats = start.beat_count
         self._assert_start_in_range(start_in_floats)
 
         # Only run cut_off if necessary -> Improve performance
         if (event_to_squash_in_duration := event_to_squash_in.duration) > 0:
             cut_off_end = start + event_to_squash_in_duration
             self._cut_off(start, cut_off_end, event_to_squash_in_duration)
 
         # We already know that the given start is within the
         # range of the event. This means that if the start
         # is bigger than the duration, it is only due to a
         # floating point rounding error. To avoid odd bugs
         # we therefore have to define the bigger-equal
         # relationship.
-        (
-            absolute_time_in_floats_tuple,
-            duration_in_floats,
-        ) = self._absolute_time_in_floats_tuple_and_duration
-        if start_in_floats >= duration_in_floats:
+        abstf_tuple, durf = self._abstf_tuple_and_dur
+        if start_in_floats >= durf:
             self.append(event_to_squash_in)
         else:
             try:
-                insert_index = absolute_time_in_floats_tuple.index(start)
+                insert_index = abstf_tuple.index(start)
             # There is an event on the given point which need to be
             # split.
             except ValueError:
-                active_event_index = (
-                    SequentialEvent._get_index_at_from_absolute_time_tuple(
-                        start_in_floats,
-                        absolute_time_in_floats_tuple,
-                        duration_in_floats,
-                    )
-                )
-                split_position = (
-                    start_in_floats - absolute_time_in_floats_tuple[active_event_index]
+                active_event_index = Consecution._get_index_at_from_absolute_time_tuple(
+                    start_in_floats,
+                    abstf_tuple,
+                    durf,
                 )
+                split_position = start_in_floats - abstf_tuple[active_event_index]
                 if (
                     split_position > 0
                     and split_position < self[active_event_index].duration
                 ):
                     split_active_event = self[active_event_index].split_at(
                         split_position
                     )
                     self[active_event_index] = split_active_event[1]
                     self.insert(active_event_index, split_active_event[0])
                     active_event_index += 1
 
                 insert_index = active_event_index
 
             self.insert(insert_index, event_to_squash_in)
+        return self
 
-    @core_utilities.add_copy_option
     def slide_in(
         self,
-        start: core_parameters.abc.Duration,
+        start: core_parameters.abc.Duration.Type,
         event_to_slide_in: core_events.abc.Event,
-    ) -> SequentialEvent[T]:
-        start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+    ) -> Consecution[T]:
+        start = core_parameters.abc.Duration.from_any(start)
         self._assert_valid_absolute_time(start)
-        start_in_floats = start.duration_in_floats
+        start_in_floats = start.beat_count
         if start_in_floats == 0:
             self.insert(0, event_to_slide_in)
             return self
         self._assert_start_in_range(start_in_floats)
         try:
             self[:], b = self.split_at(start)
         except ValueError:  # Only one event => start == duration.
             self.append(event_to_slide_in)
         else:
             self.extend([event_to_slide_in] + b)
         return self
 
-    @core_utilities.add_copy_option
     def split_child_at(
-        self, absolute_time: core_parameters.abc.Duration | typing.Any
-    ) -> SequentialEvent[T]:
-        (
-            absolute_time_in_floats_tuple,
-            duration_in_floats,
-        ) = self._absolute_time_in_floats_tuple_and_duration
-
-        return self._split_child_at(
-            absolute_time, absolute_time_in_floats_tuple, duration_in_floats
-        )
+        self, absolute_time: core_parameters.abc.Duration.Type
+    ) -> Consecution[T]:
+        abstf_tuple, durf = self._abstf_tuple_and_dur
+        self._split_child_at(absolute_time, abstf_tuple, durf)
+        return self
 
     def split_at(
         self,
-        *absolute_time: core_parameters.abc.Duration,
+        *absolute_time: core_parameters.abc.Duration.Type,
         ignore_invalid_split_point: bool = False,
-    ) -> tuple[SequentialEvent, ...]:
+    ) -> tuple[Consecution, ...]:
         if not absolute_time:
             raise core_utilities.NoSplitTimeError()
 
-        (
-            absolute_time_in_floats_tuple,
-            duration_in_floats,
-        ) = self._absolute_time_in_floats_tuple_and_duration
-
-        absolute_time_list = list(absolute_time_in_floats_tuple)
-
-        # NOTE: maybe we can add a 'mutate=False' keyword in case
-        # someone doesn't care about keeping the old event and wants
-        # to save some seconds of expensive copy-operation?
+        split_abstf_list = [
+            core_parameters.abc.Duration.from_any(t).beat_count for t in absolute_time
+        ]
+
+        abstf_tuple, durf = self._abstf_tuple_and_dur
+        abstf_list = list(abstf_tuple)
         c = self.copy()
 
         index_list = []
         is_first = True
-        for t in sorted(absolute_time):
+        for t in sorted(split_abstf_list):
             if is_first:  # First is smallest, check if t < 0
                 self._assert_valid_absolute_time(t)
                 is_first = False
             # Improve performance: don't try to split if we know it is
             # already split here. We also need to be sure to not
             # add any duplicates to 'absolute_time_list', so we need
             # to check anyway.
-            if t in absolute_time_list:
-                index_list.append(absolute_time_list.index(t))
+            if t in abstf_list:
+                index_list.append(abstf_list.index(t))
                 continue
             # It's okay to ignore, this is still within the given event
             # (if we don't continue 'split_child_at' raises an error).
-            if t == duration_in_floats:
+            if t == durf:
                 continue
             try:
-                i = c._split_child_at(t, tuple(absolute_time_list), duration_in_floats)
+                i = c._split_child_at(t, tuple(abstf_list), durf)
             except core_utilities.SplitUnavailableChildError:
                 if not ignore_invalid_split_point:
                     raise core_utilities.SplitError(t)
                 # We can stop, because if there isn't any child at this time
                 # there won't be any child at a later time (remember: our
                 # absolute times are sorted).
                 break
             index_list.append(i)
-            absolute_time_list.append(t)
-            absolute_time_list.sort()
+            abstf_list.append(t)
+            abstf_list.sort()
 
         # Add frame indices (if not already present)
         if 0 not in index_list:
             index_list.insert(0, 0)
 
         if (event_count := len(c)) not in index_list:
             index_list.append(event_count)
 
         return tuple(c[i0:i1] for i0, i1 in zip(index_list, index_list[1:]))
 
-    @core_utilities.add_copy_option
     def extend_until(
         self,
-        duration: core_parameters.abc.Duration,
+        duration: core_parameters.abc.Duration.Type,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
         ] = None,
-        prolong_simple_event: bool = True,
-    ) -> SequentialEvent[T]:
-        duration = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
+        prolong_chronon: bool = True,
+    ) -> Consecution[T]:
+        duration = core_parameters.abc.Duration.from_any(duration)
         duration_to_white_space = (
             duration_to_white_space
             or core_events.configurations.DEFAULT_DURATION_TO_WHITE_SPACE
         )
         if (difference := duration - self.duration) > 0:
             self.append(duration_to_white_space(difference))
+        return self
 
 
-class SimultaneousEvent(core_events.abc.ComplexEvent, typing.Generic[T]):
-    """A :class:`SimultaneousEvent` is a simultaneity of events."""
+class Concurrence(core_events.abc.Compound, typing.Generic[T]):
+    """A :class:`Concurrence` hosts events that take place at the same time."""
 
     # ###################################################################### #
     #                       private static methods                           #
     # ###################################################################### #
 
     @staticmethod
     def _extend_ancestor(ancestor: core_events.abc.Event, event: core_events.abc.Event):
         try:
-            ancestor._concatenate_tempo_envelope(event)
-        # We can't concatenate to a simple event.
+            ancestor._concatenate_tempo(event)
+        # We can't concatenate to a chronon.
         # We also can't concatenate to anything else.
         except AttributeError:
             raise core_utilities.ConcatenationError(ancestor, event)
         match ancestor:
-            case core_events.SequentialEvent():
+            case core_events.Consecution():
                 ancestor.extend(event)
-            case core_events.SimultaneousEvent():
+            case core_events.Concurrence():
                 try:
                     ancestor.concatenate_by_tag(event)
                 except core_utilities.NoTagError:
                     ancestor.concatenate_by_index(event)
             # This should already fail above, but if this strange object
-            # somehow owned '_concatenate_tempo_envelope', it should
+            # somehow owned '_concatenate_tempo', it should
             # fail here.
             case _:
                 raise core_utilities.ConcatenationError(ancestor, event)
 
     # ###################################################################### #
     #                           private methods                              #
     # ###################################################################### #
 
     def _make_event_slice_tuple(
         self,
         absolute_time_list: list[core_parameters.abc.Duration],
         slice_tuple_to_event: typing.Callable[
-            [tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event
+            [tuple[core_events.abc.Event, ...]], core_events.abc.Event
         ],
     ) -> tuple[core_events.abc.Event, ...]:
         """Split at given times and cast split events into new events."""
+        abst_list = absolute_time_list
 
         # Slice all child events
         slices = []
         for e in self:
-            slices.append(
-                list(e.split_at(*absolute_time_list, ignore_invalid_split_point=True))
-            )
+            slices.append(list(e.split_at(*abst_list, ignore_invalid_split_point=True)))
 
         # Ensure all slices have the same amount of entries,
         # because we use 'zip' later and if one of them is
         # shorter we loose some parts of our event.
         if slices:
             slices_count_tuple = tuple(len(s) for s in slices)
             max_slice_count = max(slices_count_tuple)
@@ -880,350 +804,316 @@
 
         return tuple(event_list)
 
     # ###################################################################### #
     #                           properties                                   #
     # ###################################################################### #
 
-    @core_events.abc.ComplexEvent.duration.getter
-    def duration(self) -> core_constants.DurationType:
+    @core_events.abc.Compound.duration.getter
+    def duration(self) -> core_parameters.abc.Duration:
         try:
-            return max(event.duration for event in self)
-        # If SimultaneousEvent is empty
+            return max(e.duration for e in self)
+        # If Concurrence is empty
         except ValueError:
             return core_parameters.DirectDuration(0)
 
     # ###################################################################### #
     #                           public methods                               #
     # ###################################################################### #
 
-    @core_utilities.add_copy_option
     def cut_out(  # type: ignore
         self,
-        start: core_parameters.abc.Duration | typing.Any,
-        end: core_parameters.abc.Duration | typing.Any,
-    ) -> SimultaneousEvent[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Concurrence[T]:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
-        [event.cut_out(start, end) for event in self]
+        [e.cut_out(start, end) for e in self]
+        return self
 
-    @core_utilities.add_copy_option
     def cut_off(  # type: ignore
         self,
-        start: core_constants.DurationType,
-        end: core_constants.DurationType,
-    ) -> SimultaneousEvent[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start: core_parameters.abc.Duration.Type,
+        end: core_parameters.abc.Duration.Type,
+    ) -> Concurrence[T]:
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(start, end)
-        [event.cut_off(start, end) for event in self]
+        [e.cut_off(start, end) for e in self]
+        return self
 
-    @core_utilities.add_copy_option
     def squash_in(  # type: ignore
         self,
-        start: core_parameters.abc.Duration | typing.Any,
+        start: core_parameters.abc.Duration.Type,
         event_to_squash_in: core_events.abc.Event,
-    ) -> SimultaneousEvent[T]:
-        start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+    ) -> Concurrence[T]:
+        start = core_parameters.abc.Duration.from_any(start)
         self._assert_valid_absolute_time(start)
         self._assert_start_in_range(start)
 
-        for event in self:
+        for e in self:
             try:
-                event.squash_in(start, event_to_squash_in)  # type: ignore
+                e.squash_in(start, event_to_squash_in)  # type: ignore
             # Simple events don't have a 'squash_in' method.
             except AttributeError:
                 raise core_utilities.ImpossibleToSquashInError(self, event_to_squash_in)
+        return self
 
-    @core_utilities.add_copy_option
     def slide_in(
         self,
-        start: core_parameters.abc.Duration,
+        start: core_parameters.abc.Duration.Type,
         event_to_slide_in: core_events.abc.Event,
-    ) -> SimultaneousEvent[T]:
-        start = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(start)
+    ) -> Concurrence[T]:
+        start = core_parameters.abc.Duration.from_any(start)
         self._assert_valid_absolute_time(start)
         self._assert_start_in_range(start)
-        for event in self:
+        for e in self:
             try:
-                event.slide_in(start, event_to_slide_in)  # type: ignore
+                e.slide_in(start, event_to_slide_in)  # type: ignore
             # Simple events don't have a 'slide_in' method.
             except AttributeError:
                 raise core_utilities.ImpossibleToSlideInError(self, event_to_slide_in)
+        return self
 
-    @core_utilities.add_copy_option
     def split_child_at(
-        self, absolute_time: core_constants.DurationType
-    ) -> SimultaneousEvent[T]:
-        for event_index, event in enumerate(self):
+        self, absolute_time: core_parameters.abc.Duration.Type
+    ) -> Concurrence[T]:
+        abst = core_parameters.abc.Duration.from_any(absolute_time)
+        for i, e in enumerate(self):
             try:
-                event.split_child_at(absolute_time)
-            # simple events don't have a 'split_child_at' method
+                e.split_child_at(abst)
+            # chronons don't have a 'split_child_at' method
             except AttributeError:
-                split_event = event.split_at(absolute_time)
-                self[event_index] = SequentialEvent(split_event)
+                split_event = e.split_at(abst)
+                self[i] = Consecution(split_event)
+        return self
 
-    @core_utilities.add_copy_option
     def extend_until(
         self,
-        duration: typing.Optional[core_parameters.abc.Duration] = None,
+        duration: typing.Optional[core_parameters.abc.Duration.Type] = None,
         duration_to_white_space: typing.Optional[
             typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
         ] = None,
-        prolong_simple_event: bool = True,
-    ) -> SimultaneousEvent[T]:
+        prolong_chronon: bool = True,
+    ) -> Concurrence[T]:
         duration = (
             self.duration
             if duration is None
-            else core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
+            else core_parameters.abc.Duration.from_any(duration)
         )
         duration_to_white_space = (
             duration_to_white_space
             or core_events.configurations.DEFAULT_DURATION_TO_WHITE_SPACE
         )
-        # We only append simple events to sequential events, because there
-        # are many problems with the SimultaneousEvent[SimpleEvent] construct
+        # We only append chronons to consecutions, because there
+        # are many problems with the Concurrence[Chronon] construct
         # ('extend_until' and 'squash_in' will fail on such a container).
-        # Therefore calling 'extend_until' on an empty SimultaneousEvent is
-        # in fact ineffective: The user would get a SimultaneousEvent which
+        # Therefore calling 'extend_until' on an empty Concurrence is
+        # in fact ineffective: The user would get a Concurrence which
         # still has duration = 0, which is absolutely unexpected. Therefore
         # we raise an error, to avoid confusion by the user.
         if not self:
             raise core_utilities.IneffectiveExtendUntilError(self)
-        for event in self:
+        for e in self:
             try:
-                event.extend_until(
-                    duration, duration_to_white_space, prolong_simple_event
-                )
-            # SimpleEvent
+                e.extend_until(duration, duration_to_white_space, prolong_chronon)
+            # Chronon
             except AttributeError:
-                if prolong_simple_event:
-                    if (difference := duration - event.duration) > 0:
-                        event.duration += difference
+                if prolong_chronon:
+                    if (difference := duration - e.duration) > 0:
+                        e.duration += difference
                 else:
-                    raise core_utilities.ImpossibleToExtendUntilError(event)
+                    raise core_utilities.ImpossibleToExtendUntilError(e)
+        return self
+
+    def concatenate_by_index(self, other: Concurrence) -> Concurrence:
+        """Concatenate with other :class:`~mutwo.core_events.Concurrence` along their indices.
 
-    @core_utilities.add_copy_option
-    def concatenate_by_index(self, other: SimultaneousEvent) -> SimultaneousEvent:
-        """Concatenate with other :class:`~mutwo.core_events.SimultaneousEvent` along their indices.
-
-        :param other: The other `SimultaneousEvent` with which to concatenate.
-            The other `SimultaneousEvent` can contain more or less events.
-        :type other: SimultaneousEvent
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
-        :type mutate: bool
-        :raises core_utilities.ConcatenationError: If there are any :class:`SimpleEvent`
-            inside a :class:`SimultaneousEvent`.
+        :param other: The other `Concurrence` with which to concatenate.
+            The other `Concurrence` can contain more or less events.
+        :type other: Concurrence
+        :raises core_utilities.ConcatenationError: If there are any :class:`Chronon`
+            inside a :class:`Concurrence`.
 
         **Hint:**
 
         Similarly to Pythons ``list.extend`` the concatenation simply appends
         the children of the other event to the sequence without copying them.
         This means when changing the children in the new event, it also changes
         the child event in the original sequence. If you want to avoid this,
         call ``event.copy()`` before concatenating it to the host event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> s = core_events.SimultaneousEvent(
-        ...     [core_events.SequentialEvent([core_events.SimpleEvent(1)])]
+        >>> cnc = core_events.Concurrence(
+        ...     [core_events.Consecution([core_events.Chronon(1)])]
         ... )
-        >>> s.concatenate_by_index(s)
-        SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 1))])])
+        >>> cnc.concatenate_by_index(cnc)
+        Concurrence([Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(1.0))])])
         """
-        if (self_duration := self.duration) > 0:
-            self.extend_until(self_duration)
-        for index, event in enumerate(other):
+        if (dur := self.duration) > 0:
+            self.extend_until(dur)
+        for i, e in enumerate(other):
             try:
-                ancestor = self[index]
+                ancestor = self[i]
             except IndexError:
-                if self_duration > 0:
+                if dur > 0:
                     # Shallow copy before 'slide_in': We use the same
                     # events, but we don't want to change the other sequence.
-                    event_new = event.empty_copy()
-                    event_new.extend(event[:])
-                    event = event_new.slide_in(0, core_events.SimpleEvent(self_duration))
-                self.append(event)
+                    e_new = e.empty_copy()
+                    e_new.extend(e[:])
+                    e = e_new.slide_in(0, core_events.Chronon(dur))
+                self.append(e)
             else:
-                self._extend_ancestor(ancestor, event)
+                self._extend_ancestor(ancestor, e)
+        return self
+
+    def concatenate_by_tag(self, other: Concurrence) -> Concurrence:
+        """Concatenate with other :class:`~mutwo.core_events.Concurrence` along their tags.
 
-    @core_utilities.add_copy_option
-    def concatenate_by_tag(self, other: SimultaneousEvent) -> SimultaneousEvent:
-        """Concatenate with other :class:`~mutwo.core_events.SimultaneousEvent` along their tags.
-
-        :param other: The other `SimultaneousEvent` with which to concatenate.
-            The other `SimultaneousEvent` can contain more or less events.
-        :type other: SimultaneousEvent
-        :param mutate: If ``False`` the function will return a copy of the given object.
-            If set to ``True`` the object itself will be changed and the function will
-            return the changed object. Default to ``True``.
-        :type mutate: bool
+        :param other: The other `Concurrence` with which to concatenate.
+            The other `Concurrence` can contain more or less events.
+        :type other: Concurrence
         :return: Concatenated event.
         :raises core_utilities.NoTagError: If any child event doesn't have a 'tag'
             attribute.
-        :raises core_utilities.ConcatenationError: If there are any :class:`SimpleEvent`
-            inside a :class:`SimultaneousEvent`.
+        :raises core_utilities.ConcatenationError: If there are any :class:`Chronon`
+            inside a :class:`Concurrence`.
 
         **Hint:**
 
         Similarly to Pythons ``list.extend`` the concatenation simply appends
         the children of the other event to the sequence without copying them.
         This means when changing the children in the new event, it also changes
         the child event in the original sequence. If you want to avoid this,
         call ``event.copy()`` before concatenating it to the host event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> s = core_events.SimultaneousEvent(
-        ...      [core_events.TaggedSequentialEvent([core_events.SimpleEvent(1)], tag="test")]
+        >>> cnc = core_events.Concurrence(
+        ...      [core_events.Consecution([core_events.Chronon(1)], tag="test")]
         ...  )
-        >>> s.concatenate_by_tag(s)
-        SimultaneousEvent([TaggedSequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1)), SimpleEvent(duration = DirectDuration(duration = 1))])])
+        >>> cnc.concatenate_by_tag(cnc)
+        Concurrence([Consecution([Chronon(duration=DirectDuration(1.0)), Chronon(duration=DirectDuration(1.0))])])
         """
-        if (self_duration := self.duration) > 0:
-            self.extend_until(self_duration)
-        for tagged_event in other:
-            if not hasattr(tagged_event, "tag"):
-                raise core_utilities.NoTagError(tagged_event)
-            tag = tagged_event.tag
+        if (dur := self.duration) > 0:
+            self.extend_until(dur)
+        for e in other:
+            if not (tag := e.tag):
+                raise core_utilities.NoTagError(e)
             try:
                 ancestor = self[tag]
             except KeyError:
-                if self_duration > 0:
+                if dur > 0:
                     # Shallow copy before 'slide_in': We use the same
                     # events, but we don't want to change the other sequence.
-                    event_new = tagged_event.empty_copy()
-                    event_new.extend(tagged_event[:])
-                    tagged_event = event_new.slide_in(0, core_events.SimpleEvent(self_duration))
-                self.append(tagged_event)
+                    e_new = e.empty_copy()
+                    e_new.extend(e[:])
+                    e = e_new.slide_in(0, core_events.Chronon(dur))
+                self.append(e)
             else:
-                self._extend_ancestor(ancestor, tagged_event)
+                self._extend_ancestor(ancestor, e)
+        return self
 
-    # NOTE: 'sequentalize' is very generic, it works for all type of child
+    # NOTE: 'sequentialize' is very generic, it works for all type of child
     # event structure. This is good, but in it's current form it's mostly
     # only useful with rather long and complex user defined 'slice_tuple_to_event'
     # definitions. For instance when sequentializing
-    # SimultaneousEvent[SequentialEvent[SimpleEvent]] the returned event will be
-    # SequentialEvent[SimultaneousEvent[SequentialEvent[SimpleEvent]]]. Here the
-    # inner sequential events are always pointless, since they will always only
-    # contain one simple event.
+    # Concurrence[Consecution[Chronon]] the returned event will be
+    # Consecution[Concurrence[Consecution[Chronon]]]. Here the
+    # inner consecutions are always pointless, since they will always only
+    # contain one chronon.
     def sequentialize(
         self,
         slice_tuple_to_event: typing.Optional[
-            typing.Callable[
-                [tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event
-            ]
+            typing.Callable[[tuple[core_events.abc.Event, ...]], core_events.abc.Event]
         ] = None,
-    ) -> core_events.SequentialEvent:
-        """Convert parallel structure to a sequential structure.
+    ) -> core_events.Consecution:
+        """Convert parallel structure to a consuential structure.
 
         :param slice_tuple_to_event: In order to sequentialize the event
             `mutwo` splits each child event into small 'event slices'. These
             'event slices' are simply events created by the `split_at` method.
             Each of those parallel slice groups need to be bound together to
-            one new event. These new events are sequentially ordered to result
-            in a new sequential structure. The simplest and default way to
+            one new event. These new events are consuentially ordered to result
+            in a new consuential structure. The simplest and default way to
             archive this is by simply putting all event parts into a new
-            :class:`SimultaneousEvent`, so the resulting :class:`SequentialEvent`
-            will be a sequence of `SimultaneousEvent`. This parameter is
+            :class:`Concurrence`, so the resulting :class:`Consecution`
+            is a sequence of `Concurrence`. This parameter is
             available so that users can convert her/his parallel structure in
             meaningful ways (for instance to imitate the ``.chordify``
             `method from music21 <https://web.mit.edu/music21/doc/usersGuide/usersGuide_09_chordify.html>`
             which transforms polyphonic music to a chord structure).
             If ``None`` `slice_tuple_to_event` is set to
-            :class:`SimultaneousEvent`. Default to ``None``.
-        :type slice_tuple_to_event: typing.Optional[typing.Callable[[tuple[core_parameters.abc.Event, ...]], core_parameters.abc.Event]]
+            :class:`Concurrence`. Default to ``None``.
+        :type slice_tuple_to_event: typing.Optional[typing.Callable[[tuple[core_events.abc.Event, ...]], core_events.abc.Event]]
+
+        **Warning:**
+
+        Because the returned event is a :class:`Consecution` class specific
+        side attributes of the :class:`Concurrence` aren't persistent in
+        the returned event.
 
         **Example:**
 
         >>> from mutwo import core_events
-        >>> e = core_events.SimultaneousEvent(
+        >>> e = core_events.Concurrence(
         ...     [
-        ...         core_events.SequentialEvent(
-        ...             [core_events.SimpleEvent(2), core_events.SimpleEvent(1)]
+        ...         core_events.Consecution(
+        ...             [core_events.Chronon(2), core_events.Chronon(1)]
         ...         ),
-        ...         core_events.SequentialEvent(
-        ...             [core_events.SimpleEvent(3)]
+        ...         core_events.Consecution(
+        ...             [core_events.Chronon(3)]
         ...         ),
         ...     ]
         ... )
-        >>> e.sequentialize()
-        SequentialEvent([SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 2))])]), SimultaneousEvent([SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))]), SequentialEvent([SimpleEvent(duration = DirectDuration(duration = 1))])])])
+        >>> cns = e.sequentialize()
+        >>> print(cns)
+        Cons(Conc(Cons(C(dur=D(2.0))), Cons(C(dur=D(2.0)))), Conc(Cons(C(dur=D(1.0))), Cons(C(dur=D(1.0)))))
         """
         if slice_tuple_to_event is None:
-            slice_tuple_to_event = SimultaneousEvent
+            slice_tuple_to_event = Concurrence
 
         # Find all start/end times
-        absolute_time_set = set([])
+        abst_set = set([])
         for e in self:
-            try:  # SequentialEvent
-                (
-                    absolute_time_tuple,
-                    duration,
-                ) = e._absolute_time_in_floats_tuple_and_duration
-            except AttributeError:  # SimpleEvent or SimultaneousEvent
-                absolute_time_tuple, duration = (0,), e.duration.duration_in_floats
-            for t in absolute_time_tuple + (duration,):
-                absolute_time_set.add(t)
+            try:  # Consecution
+                abst_tuple, dur = e._abstf_tuple_and_dur
+            except AttributeError:  # Chronon or Concurrence
+                abst_tuple, dur = (0,), e.duration.beat_count
+            for t in abst_tuple + (dur,):
+                abst_set.add(t)
 
         # Sort, but also remove the last entry: we don't need
         # to split at complete duration, because after duration
         # there isn't any event left in any child.
-        absolute_time_list = sorted(absolute_time_set)[:-1]
+        abst_list = sorted(abst_set)[:-1]
 
-        return core_events.SequentialEvent(
-            self._make_event_slice_tuple(absolute_time_list, slice_tuple_to_event)
+        return core_events.Consecution(
+            self._make_event_slice_tuple(abst_list, slice_tuple_to_event),
+            tag=self.tag,
         )
 
     def split_at(
         self,
-        *absolute_time: core_parameters.abc.Duration,
+        *absolute_time: core_parameters.abc.Duration.Type,
         ignore_invalid_split_point: bool = False,
-    ) -> tuple[SimultaneousEvent, ...]:
+    ) -> tuple[Concurrence, ...]:
         if not absolute_time:
             raise core_utilities.NoSplitTimeError()
 
-        absolute_time = sorted(absolute_time)
-        self._assert_valid_absolute_time(absolute_time[0])
-        if absolute_time[-1] > self.duration and not ignore_invalid_split_point:
-            raise core_utilities.SplitError(absolute_time[-1])
+        abst_list = sorted(
+            [core_parameters.abc.Duration.from_any(t) for t in absolute_time]
+        )
+        self._assert_valid_absolute_time(abst_list[0])
+        if abst_list[-1] > self.duration and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(abst_list[-1])
 
         def slice_tuple_to_event(slice_tuple):
             e = self.empty_copy()
             e[:] = slice_tuple
             return e
 
-        return self._make_event_slice_tuple(absolute_time, slice_tuple_to_event)
-
-
-@core_utilities.add_tag_to_class
-class TaggedSimpleEvent(SimpleEvent):
-    """:class:`SimpleEvent` with tag."""
-
-
-@core_utilities.add_tag_to_class
-class TaggedSequentialEvent(
-    SequentialEvent, typing.Generic[T], class_specific_side_attribute_tuple=("tag",)
-):
-    """:class:`SequentialEvent` with tag."""
-
-
-@core_utilities.add_tag_to_class
-class TaggedSimultaneousEvent(
-    SimultaneousEvent, typing.Generic[T], class_specific_side_attribute_tuple=("tag",)
-):
-    """:class:`SimultaneousEvent` with tag."""
-
-    def sequentialize(self, *args, **kwargs):
-        sequential_event = super().sequentialize(*args, **kwargs)
-        return TaggedSequentialEvent(sequential_event, tag=self.tag)
+        return self._make_event_slice_tuple(abst_list, slice_tuple_to_event)
```

### Comparing `mutwo.core-1.4.0/mutwo/core_events/envelopes.py` & `mutwo.core-2.0.0/mutwo/core_events/envelopes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,196 +1,102 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Envelope events"""
 
 from __future__ import annotations
 
 import bisect
+import functools
+import math
 import typing
 
-from scipy import integrate
+import ranges
 
 from mutwo import core_constants
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 
-__all__ = ("Envelope", "RelativeEnvelope", "TempoEnvelope")
+__all__ = ("Envelope",)
 
 T = typing.TypeVar("T", bound=core_events.abc.Event)
 
 
-class Envelope(
-    core_events.SequentialEvent,
-    typing.Generic[T],
-    class_specific_side_attribute_tuple=(
-        "event_to_parameter",
-        "event_to_curve_shape",
-        "value_to_parameter",
-        "parameter_to_value",
-        "apply_parameter_on_event",
-        "apply_curve_shape_on_event",
-        "default_event_class",
-        "initialise_default_event_class",
-    ),
-):
+class Envelope(core_events.Consecution, typing.Generic[T]):
     """Model continuous changing values (e.g. glissandi, crescendo).
 
     :param event_iterable_or_point_sequence: An iterable filled with events
         or with points. If the sequence is filled with points, the points
-        will be converted to events. Each event represents a point in a
+        are converted to events. Each event represents a point in a
         two dimensional graph where the x-axis presents time and the y-axis
         a changing value. Any event class can be used. It is
         more important that the used event classes fit with the functions
         passed in the following parameters.
     :type event_iterable_or_point_sequence: typing.Iterable[T]
-    :param event_to_parameter: A function which receives an event and has to
-        return a parameter object (any object). By default the function will
-        ask the event for its `value` property. If the property can't be found
-        it will return 0.
-    :type event_to_parameter: typing.Callable[[core_events.abc.Event], core_constants.ParameterType]
-    :param event_to_curve_shape: A function which receives an event and has
-        to return a curve_shape. A curve_shape is either a float, an integer
-        or a fraction. For a curve_shape = 0 a linear transition between two
-        points is created. For a curve_shape > 0 the envelope changes slower
-        at the beginning and faster at the end, for a curve_shape < 0 it is
-        the inverse behaviour. The default function will ask the event for its
-        `curve_shape` property. If the property can't be found
-        it will return 0.
-    :type event_to_curve_shape: typing.Callable[[core_events.abc.Event], CurveShape]
-    :param parameter_to_value: Convert a parameter to a value. A value is any
-        object which supports mathematical operations.
-    :type parameter_to_value: typing.Callable[[Value], core_constants.ParameterType]
-    :param value_to_parameter: A callable object which converts a value to a parameter.
-    :type value_to_parameter: typing.Callable[[Value], core_constants.ParameterType]
-    :param apply_parameter_on_event: A callable object which applies a parameter on an event.
-    :type apply_parameter_on_event: typing.Callable[[core_events.abc.Event, core_constants.ParameterType], None]
-    :param apply_curve_shape_on_event: A callable object which applies a curve shape on an event.
-    :type apply_curve_shape_on_event: typing.Callable[[core_events.abc.Event, CurveShape], None]
-    :param default_event_class: The default event class which describes a point.
-    :type default_event_class: type[core_events.abc.Event]
-    :param initialise_default_event_class:
-    :type initialise_default_event_class: typing.Callable[[type[core_events.abc.Event], core_constants.DurationType], core_events.abc.Event]
 
     This class is inspired by Marc Evansteins `Envelope` class in his
     `expenvelope <https://git.sr.ht/~marcevanstein/expenvelope>`_
     python package and is made to fit better into the `mutwo` ecosystem.
 
     **Hint:**
 
-    When comparing two envelopes (e.g. `env0 == env1`) `mutwo` will only return
-    `True` in case all control points (= simple events inside the envelope) are
+    When comparing two envelopes (e.g. `env0 == env1`) `mutwo` only returns
+    `True` in case all control points (= events inside the envelope) are
     equal between both envelopes. So `mutwo` won't make the much more
     complicated test to check if two envelopes have the same shape (= the same
     value at each `env0.value_at(x) == env1.value_at(x)` for each possible
     `x`). Such a test is not implemented yet.
 
     **Example:**
 
     >>> from mutwo import core_events
     >>> core_events.Envelope([[0, 0, 1], [0.5, 1]])
-    Envelope([SimpleEvent(curve_shape = 1, duration = DirectDuration(duration = 1/2), value = 0), SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 0), value = 1)])
+    Envelope([Chronon(curve_shape=1, duration=DirectDuration(0.5), value=0), Chronon(curve_shape=0, duration=DirectDuration(0.0), value=1)])
     """
 
     # Type definitions
-    Value = core_constants.Real
-    CurveShape = core_constants.Real
-    IncompletePoint = tuple[core_constants.DurationType, core_constants.ParameterType]
-    CompletePoint = tuple[
-        core_constants.DurationType, core_constants.ParameterType, CurveShape  # type: ignore
+    Value: typing.TypeAlias = core_constants.Real
+    Parameter: typing.TypeAlias = typing.Any
+    CurveShape: typing.TypeAlias = core_constants.Real
+    IncompletePoint: typing.TypeAlias = tuple["core_parameters.abc.Duration", Parameter]
+    CompletePoint: typing.TypeAlias = tuple[
+        "core_parameters.abc.Duration", Parameter, CurveShape  # type: ignore
     ]
-    Point = CompletePoint | IncompletePoint
+    Point: typing.TypeAlias = CompletePoint | IncompletePoint
+
+    default_event_class = core_events.Chronon
+
+    _short_name_length = 3
 
     def __init__(
         self,
         event_iterable_or_point_sequence: typing.Iterable[T] | typing.Sequence[Point],
-        tempo_envelope: typing.Optional[core_events.TempoEnvelope] = None,
-        event_to_parameter: typing.Callable[
-            [core_events.abc.Event], core_constants.ParameterType
-        ] = lambda event: getattr(
-            event, core_events.configurations.DEFAULT_PARAMETER_ATTRIBUTE_NAME
-        )
-        if hasattr(event, core_events.configurations.DEFAULT_PARAMETER_ATTRIBUTE_NAME)
-        else 0,
-        event_to_curve_shape: typing.Callable[
-            [core_events.abc.Event], CurveShape
-        ] = lambda event: getattr(
-            event, core_events.configurations.DEFAULT_CURVE_SHAPE_ATTRIBUTE_NAME
-        )
-        if hasattr(event, core_events.configurations.DEFAULT_CURVE_SHAPE_ATTRIBUTE_NAME)
-        else 0,
-        parameter_to_value: typing.Callable[
-            [Value], core_constants.ParameterType
-        ] = lambda parameter: parameter,
-        value_to_parameter: typing.Callable[
-            [Value], core_constants.ParameterType
-        ] = lambda value: value,
-        apply_parameter_on_event: typing.Callable[
-            [core_events.abc.Event, core_constants.ParameterType], None
-        ] = lambda event, parameter: setattr(
-            event,
-            core_events.configurations.DEFAULT_PARAMETER_ATTRIBUTE_NAME,
-            parameter,
-        ),
-        apply_curve_shape_on_event: typing.Callable[
-            [core_events.abc.Event, CurveShape], None
-        ] = lambda event, curve_shape: setattr(
-            event,
-            core_events.configurations.DEFAULT_CURVE_SHAPE_ATTRIBUTE_NAME,
-            curve_shape,
-        ),
-        default_event_class: type[core_events.abc.Event] = core_events.SimpleEvent,
-        initialise_default_event_class: typing.Callable[
-            [type[core_events.abc.Event], core_constants.DurationType],
-            core_events.abc.Event,
-        ] = lambda simple_event_class, duration: simple_event_class(
-            duration
-        ),  # type: ignore
+        *args,
+        **kwargs,
     ):
-        self.event_to_parameter = event_to_parameter
-        self.event_to_curve_shape = event_to_curve_shape
-        self.value_to_parameter = value_to_parameter
-        self.parameter_to_value = parameter_to_value
-        self.apply_parameter_on_event = apply_parameter_on_event
-        self.apply_curve_shape_on_event = apply_curve_shape_on_event
-        self.default_event_class = default_event_class
-        self.initialise_default_event_class = initialise_default_event_class
-
         event_iterable = self._event_iterable_or_point_sequence_to_event_iterable(
             event_iterable_or_point_sequence
         )
-        super().__init__(event_iterable, tempo_envelope)
-
-    # ###################################################################### #
-    #                      public class methods                              #
-    # ###################################################################### #
-
-    @classmethod
-    def from_points(
-        cls,
-        *point: Point,
-        **kwargs,
-    ) -> Envelope:
-        """Create new :class:`Envelope` from points.
-
-        This is merely a convenience wrapper to write
-
-            >>> Envelope.from_points([0, 1], [1, 100])
-            Envelope([SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 1), value = 1), SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 0), value = 100)])
-
-        instead of
-
-            >>> Envelope([[0, 1], [1, 100]])
-            Envelope([SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 1), value = 1), SimpleEvent(curve_shape = 0, duration = DirectDuration(duration = 0), value = 100)])
-
-        to mimic the default initialization behaviour of
-        `expenvelope.Envelope`. It's recommended to initialise
-        an Envelope without this method. This method will be
-        removed sooner or later.
-        """
-        return cls(point, **kwargs)
+        super().__init__(event_iterable, *args, **kwargs)
 
     # ###################################################################### #
     #                           magic methods                                #
     # ###################################################################### #
 
     @typing.overload  # type: ignore
     def __setitem__(self, index_or_slice: int, event_or_sequence: T):
@@ -221,54 +127,53 @@
     #                    private static methods                              #
     # ###################################################################### #
 
     @staticmethod
     def _point_sequence_to_corrected_point_list(
         point_or_invalid_type_sequence: typing.Sequence[Point | typing.Any],
     ) -> list[Envelope.CompletePoint | None]:
-        corrected_point_list: list[Envelope.CompletePoint | None] = []
-        for point in point_or_invalid_type_sequence:
-            point_count = len(point)
-            if point_count == 2:
-                point += (0,)  # type: ignore
-            elif point_count != 3:
-                raise core_utilities.InvalidPointError(point, point_count)
-            corrected_point_list.append(point)  # type: ignore
-        return corrected_point_list
+        pnorm_list: list[Envelope.CompletePoint | None] = []
+        for p in point_or_invalid_type_sequence:
+            if (point_size := len(p)) == 2:
+                p += (0,)  # type: ignore
+            elif point_size != 3:
+                raise core_utilities.InvalidPointError(p, point_size)
+            pnorm_list.append(p)  # type: ignore
+        return pnorm_list
 
     # ###################################################################### #
     #                         private methods                                #
     # ###################################################################### #
 
     def _make_event(self, duration, parameter, curve_shape):
-        event = self.initialise_default_event_class(self.default_event_class, duration)
+        event = self.initialise_default_event_class(duration)
         self.apply_parameter_on_event(event, parameter)
         self.apply_curve_shape_on_event(event, curve_shape)
         return event
 
     def _point_sequence_to_event_list(
         self,
         point_or_invalid_type_sequence: typing.Sequence[Point | typing.Any],
     ) -> list[core_events.abc.Event]:
-        corrected_point_list = Envelope._point_sequence_to_corrected_point_list(
+        pnorm_list = Envelope._point_sequence_to_corrected_point_list(
             point_or_invalid_type_sequence
         )
-        corrected_point_list.append(None)
+        pnorm_list.append(None)
         event_list = []
-        for point0, point1 in zip(corrected_point_list, corrected_point_list[1:]):
-            if point0 is not None:
-                absolute_time0, value_or_parameter, curve_shape = point0
+        for p0, p1 in zip(pnorm_list, pnorm_list[1:]):
+            if p0 is not None:
+                abst0, value_or_parameter, curve_shape = p0
             else:
                 raise TypeError("Found unexpected position of None in provided points.")
-            if point1:
-                absolute_time1 = point1[0]
-                assert absolute_time1 >= absolute_time0
+            if p1:
+                abst1 = p1[0]
+                assert abst1 >= abst0
             else:
-                absolute_time1 = absolute_time0
-            duration = absolute_time1 - absolute_time0
+                abst1 = abst0
+            duration = abst1 - abst0
             event = self._make_event(duration, value_or_parameter, curve_shape)
             event_list.append(event)
         return event_list
 
     def _event_iterable_or_point_sequence_to_event_iterable(
         self,
         event_iterable_or_point_sequence: typing.Iterable[T] | typing.Sequence[Point],
@@ -292,20 +197,118 @@
                 event_iterable_or_point_sequence  # type: ignore
             )
         return event_iterable  # type: ignore
 
     def _event_to_value(self, event: core_events.abc.Event) -> Value:
         return self.parameter_to_value(self.event_to_parameter(event))
 
+    # Keep this part private so that functions can cache
+    # absolute_time_tuple if it helps their performance.
+    def _curve_shape_at(
+        self,
+        abst: "core_parameters.abc.Duration",
+        abst_tuple: tuple["core_parameters.abc.Duration", ...],
+        dur: "core_parameters.abc.Duration",
+    ):
+        if not self:
+            raise core_utilities.EmptyEnvelopeError(self, "curve_shape_at")
+        e_idx = core_events.Consecution._get_index_at_from_absolute_time_tuple(
+            abst, abst_tuple, dur
+        )
+        if e_idx is not None:
+            e = self[e_idx]
+            cs = self.event_to_curve_shape(e)
+            csx = ((abst - abst_tuple[e_idx]) / e.duration).beat_count * cs
+            cs_at_abst = cs - csx
+            self.apply_curve_shape_on_event(e, csx)
+        else:
+            cs_at_abst = 0
+        return cs_at_abst
+
+    def _value_at(
+        self,
+        abst: "core_parameters.abc.Duration",
+        abst_tuple: tuple["core_parameters.abc.Duration", ...],
+        dur: "core_parameters.abc.Duration",
+    ):
+        abstf = abst.beat_count
+        abstf_tuple = tuple(map(float, abst_tuple))
+        durf = float(dur)
+
+        try:
+            use_only_first_event = abstf <= abstf_tuple[0]
+        except IndexError:
+            raise core_utilities.EmptyEnvelopeError(self, "value_at")
+
+        use_only_last_event = abstf >= (
+            # If the duration of the last event == 0 there is the danger
+            # of floating point errors (the value in absolute_time_tuple could
+            # be slightly higher than the duration of the Envelope. If this
+            # happens the function raises an AssertionError, because
+            # "_get_index_at_from_absolute_time_tuple" returns
+            # "None"). With explicitly testing if the last duration
+            # equals 0 we can avoid this danger.
+            abstf_tuple[-1]
+            if self[-1].duration > 0
+            else durf
+        )
+        if use_only_first_event or use_only_last_event:
+            index = 0 if use_only_first_event else -1
+            return self._event_to_value(self[index])
+
+        event_0_index = self._get_index_at_from_absolute_time_tuple(
+            abstf, abstf_tuple, durf
+        )
+        assert event_0_index is not None
+
+        v0, v1 = (self._event_to_value(self[event_0_index + n]) for n in range(2))
+        cs = self.event_to_curve_shape(self[event_0_index])
+
+        return core_utilities.scale(
+            abstf,
+            abstf_tuple[event_0_index],
+            abstf_tuple[event_0_index + 1],
+            v0,
+            v1,
+            cs,
+        )
+
+    def _parameter_at(
+        self,
+        abst: "core_parameters.abc.Duration",
+        abst_tuple: tuple["core_parameters.abc.Duration", ...],
+        dur: "core_parameters.abc.Duration",
+    ):
+        return self.value_to_parameter(self._value_at(abst, abst_tuple, dur))
+
+    def _point_at(
+        self,
+        abst: "core_parameters.abc.Duration",
+        abst_tuple: tuple["core_parameters.abc.Duration", ...],
+        dur: "core_parameters.abc.Duration",
+    ):
+        if not self:
+            raise core_utilities.EmptyEnvelopeError(self, "point_at")
+        if abst not in abst_tuple:
+            point = (
+                abst,
+                self._value_at(abst, abst_tuple, dur),
+                self._curve_shape_at(abst, abst_tuple, dur),
+            )
+        else:
+            e = self[abst_tuple.index(abst)]
+            point = (abst, self._event_to_value(e), self.event_to_curve_shape(e))
+        return point
+
     # ###################################################################### #
     #                         public properties                              #
     # ###################################################################### #
 
     @property
-    def parameter_tuple(self) -> tuple[core_constants.ParameterType, ...]:
+    def parameter_tuple(self) -> tuple[typing.Any, ...]:
         """Get `parameter` for each event inside :class:`Envelope`."""
         return tuple(map(self.event_to_parameter, self))
 
     @property
     def value_tuple(self) -> tuple[Value, ...]:
         """Get `value` for each event inside :class:`Envelope`."""
         return tuple(map(self.parameter_to_value, self.parameter_tuple))
@@ -320,22 +323,54 @@
         """Return `True` if :class:`Envelope` only has one static value."""
         return len(set(self.value_tuple)) <= 1
 
     # ###################################################################### #
     #                          public methods                                #
     # ###################################################################### #
 
-    def value_at(
-        self, absolute_time: core_parameters.abc.Duration | typing.Any
-    ) -> Value:
+    def event_to_parameter(self, event: core_events.abc.Event) -> typing.Any:
+        """Fetch 'parameter' from event."""
+        return event.value
+
+    def event_to_curve_shape(self, event: core_events.abc.Event) -> core_constants.Real:
+        """Fetch 'curve_shape' from event."""
+        return event.curve_shape
+
+    def parameter_to_value(self, parameter: typing.Any) -> core_constants.Real:
+        """Convert from 'parameter' to 'value'."""
+        return parameter
+
+    def value_to_parameter(self, value: core_constants.Real) -> typing.Any:
+        """Convert from 'value' to 'parameter'."""
+        return value
+
+    def apply_parameter_on_event(
+        self, event: core_events.abc.Event, parameter: typing.Any
+    ):
+        """Apply 'parameter' on given event"""
+        event.value = parameter
+
+    def apply_curve_shape_on_event(
+        self, event: core_events.abc.Event, curve_shape: core_constants.Real
+    ):
+        """Apply 'curve_shape' on given event"""
+        event.curve_shape = curve_shape
+
+    def initialise_default_event_class(
+        self, duration: core_parameters.abc.Duration
+    ) -> core_events.abc.Event:
+        """Create new event object from event type."""
+        return self.default_event_class(duration=duration)
+
+    def value_at(self, absolute_time: "core_parameters.abc.Duration.Type") -> Value:
         """Get `value` at `absolute_time`.
 
         :param absolute_time: Absolute position in time at which value shall be found.
             This is 'x' in the function notation 'f(x)'.
-        :type absolute_time: core_parameters.abc.Duration | typing.Any
+        :type absolute_time: core_parameters.abc.Duration.Type
 
         This function interpolates between the control points according to
         their `curve_shape` property.
 
         **Example:**
 
         >>> from mutwo import core_events
@@ -343,193 +378,208 @@
         >>> e.value_at(0)
         0
         >>> e.value_at(1)
         2
         >>> e.value_at(0.5)
         1.0
         """
-        absolute_time = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(
-            absolute_time
-        )
-        absolute_time_in_floats = absolute_time.duration_in_floats
-
-        (
-            absolute_time_in_floats_tuple,
-            duration_in_floats,
-        ) = self._absolute_time_in_floats_tuple_and_duration
-
-        try:
-            use_only_first_event = (
-                absolute_time_in_floats <= absolute_time_in_floats_tuple[0]
-            )
-        except IndexError:
-            raise core_utilities.EmptyEnvelopeError(self, "value_at")
-
-        use_only_last_event = absolute_time_in_floats >= (
-            # If the duration of the last event == 0 there is the danger
-            # of floating point errors (the value in absolute_time_tuple could
-            # be slightly higher than the duration of the Envelope. If this
-            # happens the function will raise an AssertionError, because
-            # "_get_index_at_from_absolute_time_tuple" will return
-            # "None"). With explicitly testing if the last duration
-            # equals 0 we can avoid this danger.
-            absolute_time_in_floats_tuple[-1]
-            if self[-1].duration > 0
-            else duration_in_floats
-        )
-        if use_only_first_event or use_only_last_event:
-            index = 0 if use_only_first_event else -1
-            return self._event_to_value(self[index])
-
-        event_0_index = self._get_index_at_from_absolute_time_tuple(
-            absolute_time, absolute_time_in_floats_tuple, duration_in_floats
-        )
-        assert event_0_index is not None
-
-        value0, value1 = (
-            self._event_to_value(self[event_0_index + n]) for n in range(2)
-        )
-        curve_shape = self.event_to_curve_shape(self[event_0_index])
-
-        return core_utilities.scale(
-            absolute_time_in_floats,
-            absolute_time_in_floats_tuple[event_0_index],
-            absolute_time_in_floats_tuple[event_0_index + 1],
-            value0,
-            value1,
-            curve_shape,
-        )
+        abst = core_parameters.abc.Duration.from_any(absolute_time)
+        return self._value_at(abst, *self._abst_tuple_and_dur)
 
     def parameter_at(
-        self, absolute_time: core_parameters.abc.Duration | typing.Any
-    ) -> core_constants.ParameterType:
+        self, absolute_time: "core_parameters.abc.Duration.Type"
+    ) -> typing.Any:
         """Get `parameter` at `absolute_time`.
 
         :param absolute_time: Absolute position in time at which parameter shall
             be found. This is 'x' in the function notation 'f(x)'.
-        :type absolute_time: core_parameters.abc.Duration | typing.Any
+        :type absolute_time: core_parameters.abc.Duration.Type
         """
         return self.value_to_parameter(self.value_at(absolute_time))
 
-    @core_utilities.add_copy_option
+    def curve_shape_at(
+        self, absolute_time: "core_parameters.abc.Duration.Type"
+    ) -> float:
+        """Get `curve_shape` at `absolute_time`.
+
+        :param absolute_time: Absolute position in time at which curve shape shall
+            be found. This is 'x' in the function notation 'f(x)'.
+        :type absolute_time: core_parameters.abc.Duration.Type
+        """
+        abst = core_parameters.abc.Duration.from_any(absolute_time)
+        return self._curve_shape_at(abst, *self._abst_tuple_and_dur)
+
+    def point_at(
+        self,
+        absolute_time: "core_parameters.abc.Duration.Type",
+    ):
+        """Get `point` at `absolute_time`.
+
+        :param absolute_time: Absolute position in time at which point shall
+            be found. This is 'x' in the function notation 'f(x)'.
+        :type absolute_time: core_parameters.abc.Duration.Type
+
+        A point is a tuple with (absolute_time, value, curve_shape).
+        """
+        abst = core_parameters.abc.Duration.from_any(absolute_time)
+        return self._point_at(abst, *self._abst_tuple_and_dur)
+
     def sample_at(
         self,
-        absolute_time: core_parameters.abc.Duration | typing.Any,
-        append_duration: core_parameters.abc.Duration | typing.Any = 0,
+        absolute_time: "core_parameters.abc.Duration.Type",
+        append_duration: "core_parameters.abc.Duration.Type" = 0,
     ) -> Envelope:
         """Discretize envelope at given time
 
         :param absolute_time: Position in time where the envelope should
             define a new event.
-        :type absolute_time: core_parameters.abc.Duration | typing.Any
+        :type absolute_time: core_parameters.abc.Duration.Type
         :param append_duration: In case we add a new control point after any
             already defined point, the duration of this control point will be
             equal to "append_duration". Default to core_parameters.DirectDuration(0)
         """
 
-        def find_duration(
-            absolute_time: core_parameters.abc.Duration,
-            absolute_time_tuple: tuple[core_parameters.abc.Duration, ...],
+        def find_dur(
+            abst: "core_parameters.abc.Duration",
+            abst_tuple: tuple["core_parameters.abc.Duration", ...],
         ):
             """Find duration of new control point"""
-            next_event_start_index = bisect.bisect_right(
-                absolute_time_tuple, absolute_time
-            )
+            next_event_start_index = bisect.bisect_right(abst_tuple, abst)
             try:
-                next_event_start = absolute_time_tuple[next_event_start_index]
+                next_event_start = abst_tuple[next_event_start_index]
             # In case we call "sample_at" at a position after any already
             # specified point.
             except IndexError:
-                duration_new_event = append_duration
+                return append_duration
             else:
-                duration_new_event = next_event_start - absolute_time
-
-            return duration_new_event
-
-        def find_curve_shape(
-            absolute_time: core_parameters.abc.Duration,
-            absolute_time_tuple: tuple[core_parameters.abc.Duration, ...],
-            envelope_duration: core_parameters.abc.Duration,
-        ):
-            """Find curve shape of new control point"""
-            old_event_index = (
-                core_events.SequentialEvent._get_index_at_from_absolute_time_tuple(
-                    absolute_time, absolute_time_tuple, envelope_duration
-                )
-            )
-            if old_event_index is not None:
-                old_event = self[old_event_index]
-                curve_shape = self.event_to_curve_shape(old_event)
-                curve_shape_old_event = (
-                    (absolute_time - absolute_time_tuple[old_event_index])
-                    / old_event.duration
-                ).duration_in_floats * curve_shape
-                curve_shape_new_event = curve_shape - curve_shape_old_event
-                self.apply_curve_shape_on_event(old_event, curve_shape_old_event)
-            else:
-                curve_shape_new_event = 0
-
-            return curve_shape_new_event
+                return next_event_start - abst
 
         if not self:
             raise core_utilities.EmptyEnvelopeError(self, "sample_at")
 
-        absolute_time, append_duration = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (absolute_time, append_duration)
+        abst, append_duration = (
+            core_parameters.abc.Duration.from_any(o)
+            for o in (absolute_time, append_duration)
         )
 
-        self._assert_valid_absolute_time(absolute_time)
+        self._assert_valid_absolute_time(abst)
+        abst_tuple, dur = self._abst_tuple_and_dur
 
         # We only add a new event in case there isn't any event yet at
         # given point in time.
-        if absolute_time not in (absolute_time_tuple := self.absolute_time_tuple):
-            envelope_duration = absolute_time_tuple[-1] + self[-1].duration
-            event = self._make_event(
-                find_duration(absolute_time, absolute_time_tuple),
-                self.parameter_at(absolute_time),
-                find_curve_shape(absolute_time, absolute_time_tuple, envelope_duration),
+        if abst not in abst_tuple:
+            p = self._point_at(abst, abst_tuple, dur)
+            e = self._make_event(
+                find_dur(abst, abst_tuple), self.value_to_parameter(p[1]), p[2]
             )
 
             try:
-                self.squash_in(absolute_time, event)
+                self.squash_in(abst, e)
             # This means we want to squash in at a position much
             # later than any already defined event.
             except core_utilities.InvalidStartValueError:
-                difference = absolute_time - envelope_duration
+                difference = abst - dur
                 self[-1].duration += difference
-                self.append(event)
+                self.append(e)
 
         return self
 
+    def time_range_to_point_tuple(
+        self, time_range: ranges.Range
+    ) -> tuple[CompletePoint, ...]:
+        """Return all control points in given time range.
+
+        :param time_range: Start and end time encapsulated in a
+            :class:`ranges.Range` object.
+        :type time_range: ranges.Range
+
+        If at start and end time aren't any control points, the functions
+        creates them ad-hoc via ``point_at``.
+        """
+        start, end = (
+            core_parameters.abc.Duration.from_any(o)
+            for o in (time_range.start, time_range.end)
+        )
+        abst_tuple, dur = self._abst_tuple_and_dur
+        p = functools.partial(  # point_at
+            self._point_at, abst_tuple=abst_tuple, dur=dur
+        )
+
+        plist = []
+        if start not in abst_tuple:
+            plist.append(p(start))
+            i0 = bisect.bisect_left(abst_tuple, start)
+        else:
+            i0 = abst_tuple.index(start)
+        if end not in abst_tuple:
+            i1 = bisect.bisect_left(abst_tuple, end)
+            last_point = p(end)
+        else:
+            i1 = abst_tuple.index(end) + 1
+            last_point = None
+        for t, ev in zip(abst_tuple[i0:i1], self[i0:i1]):
+            plist.append((t, self._event_to_value(ev), self.event_to_curve_shape(ev)))
+        if last_point is not None:
+            plist.append(last_point)
+        return tuple(plist)
+
     def integrate_interval(
-        self, start: core_constants.DurationType, end: core_constants.DurationType
+        self,
+        start: "core_parameters.abc.Duration.Type",
+        end: "core_parameters.abc.Duration.Type",
     ) -> float:
         """Integrate envelope above given interval.
 
         :param start: Beginning of integration interval.
-        :type start: core_parameters.abc.Duration
+        :type start: core_parameters.abc.Duration.Type
         :param end: End of integration interval.
-        :type end: core_parameters.abc.Duration
+        :type end: core_parameters.abc.Duration.Type
         """
-        return integrate.quad(lambda x: self.value_at(x), start, end)[0]
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
+        if start == end:
+            return 0
+
+        point_tuple = self.time_range_to_point_tuple(ranges.Range(start, end))
+        integral = 0
+        for p0, p1 in zip(point_tuple, point_tuple[1:]):
+            t0, v0, cchr0 = p0  # (absolute_time, value, curve_shape)
+            t1, v1, _ = p1
+            if (d0 := float(t1 - t0)) > 0:
+                if cchr0 != 0:
+                    # See https://git.sr.ht/~marcevanstein/expenvelope/tree/cd4a3710/item/expenvelope/envelope_segment.py#L102-103
+                    A = v0 - (v1 - v0) / (math.exp(cchr0) - 1)
+                    B = (v1 - v0) / (cchr0 * (math.exp(cchr0) - 1))
+
+                    def antiderivative(tn):
+                        # See https://git.sr.ht/~marcevanstein/expenvelope/tree/cd4a3710/item/expenvelope/envelope_segment.py#L239
+                        return A * tn + B * math.exp(cchr0 * tn)
+
+                    a0, a1 = (antiderivative(i) for i in (0, 1))
+                    integral += d0 * (a1 - a0)
+                else:  # linear interpolation
+                    diff = v1 - v0 if v1 > v0 else v0 - v1
+                    square = d0 * min((v0, v1))
+                    triangle = 0.5 * d0 * diff
+                    integral += square + triangle
+
+        return float(integral)
 
     def get_average_value(
         self,
-        start: typing.Optional[core_parameters.abc.Duration | typing.Any] = None,
-        end: typing.Optional[core_parameters.abc.Duration | typing.Any] = None,
+        start: typing.Optional["core_parameters.abc.Duration.Type"] = None,
+        end: typing.Optional["core_parameters.abc.Duration.Type"] = None,
     ) -> Value:
         """Find average `value` in given interval.
 
         :param start: The beginning of the interval. If set to `None` this
-            will be 0. Default to `None`.
-        :type start: typing.Optional[core_parameters.abc.Duration | typing.Any]
+            is set to0. Default to `None`.
+        :type start: typing.Optional[core_parameters.abc.Duration.Type]
         :param end: The end of the interval. If set to `None` this
-            will be the duration of the :class:`Envelope`.. Default to `None`.
-        :type end: typing.Optional[core_parameters.abc.Duration | typing.Any]
+            is set to the duration of the :class:`Envelope`.. Default to `None`.
+        :type end: typing.Optional[core_parameters.abc.Duration.Type]
 
         **Example:**
 
         >>> from mutwo import core_events
         >>> e = core_events.Envelope([[0, 1], [2, 0]])
         >>> e.get_average_value()
         0.5
@@ -539,62 +589,55 @@
         0.625
         """
         if start is None:
             start = core_parameters.DirectDuration(0)
         if end is None:
             end = self.duration
 
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
 
         duration = end - start
         if duration == 0:
             self._logger.warning(core_utilities.InvalidAverageValueStartAndEndWarning())
             return self.value_at(start)
-        return self.integrate_interval(start, end) / duration.duration
+        return self.integrate_interval(start, end) / duration.beat_count
 
     def get_average_parameter(
         self,
-        start: typing.Optional[core_constants.DurationType] = None,
-        end: typing.Optional[core_constants.DurationType] = None,
-    ) -> core_constants.ParameterType:
+        start: typing.Optional["core_parameters.abc.Duration.Type"] = None,
+        end: typing.Optional["core_parameters.abc.Duration.Type"] = None,
+    ) -> typing.Any:
         """Find average `parameter` in given interval.
 
         :param start: The beginning of the interval. If set to `None` this
-            will be 0. Default to `None`.
-        :type start: typing.Optional[core_parameters.abc.Duration | typing.Any]
+            is set be 0. Default to `None`.
+        :type start: typing.Optional[core_parameters.abc.Duration.Type]
         :param end: The end of the interval. If set to `None` this
-            will be the duration of the :class:`Envelope`.. Default to `None`.
-        :type end: typing.Optional[core_parameters.abc.Duration | typing.Any]
+            is set to the duration of the :class:`Envelope`.. Default to `None`.
+        :type end: typing.Optional[core_parameters.abc.Duration.Type]
 
         **Example:**
 
         >>> from mutwo import core_events
         >>> e = core_events.Envelope([[0, 1], [2, 0]])
         >>> e.get_average_parameter()
         0.5
         >>> e.get_average_parameter(0.5)
         0.375
         >>> e.get_average_parameter(0.5, 1)
         0.625
         """
         return self.value_to_parameter(self.get_average_value(start, end))
 
-    @core_utilities.add_copy_option
     def cut_out(
         self,
-        start: core_parameters.abc.Duration | typing.Any,
-        end: core_parameters.abc.Duration | typing.Any,
+        start: "core_parameters.abc.Duration.Type",
+        end: "core_parameters.abc.Duration.Type",
     ) -> Envelope[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         # _assert_correct_start_and_end_values and _assert_valid_absolute_time
         # is called when super().cut_out is called later.
 
         self.sample_at(start, append_duration=end - start)
         self.sample_at(end)
 
         last_point = self.get_event_at(end)
@@ -610,24 +653,20 @@
         assert last_point
 
         cut_out_envelope = super().cut_out(start, end)
         cut_out_envelope.append(last_point.set("duration", 0))
 
         return cut_out_envelope
 
-    @core_utilities.add_copy_option
     def cut_off(
         self,
-        start: core_parameters.abc.Duration | typing.Any,
-        end: core_parameters.abc.Duration | typing.Any,
+        start: "core_parameters.abc.Duration.Type",
+        end: "core_parameters.abc.Duration.Type",
     ) -> Envelope[T]:
-        start, end = (
-            core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(unknown_object)
-            for unknown_object in (start, end)
-        )
+        start, end = (core_parameters.abc.Duration.from_any(o) for o in (start, end))
         self._assert_valid_absolute_time(start)
         self._assert_correct_start_and_end_values(
             start, end, condition=lambda start, end: start < end
         )
 
         if (cut_off_duration := end - start) > 0:
             # It is sufficient to find the first control point
@@ -643,50 +682,51 @@
             self.sample_at(end)
 
             self._cut_off(start, end, cut_off_duration)
             self.squash_in(start, event_0)
 
         return self
 
-    @core_utilities.add_copy_option
     def extend_until(
         self,
-        duration: core_parameters.abc.Duration,
+        duration: "core_parameters.abc.Duration.Type",
         duration_to_white_space: typing.Optional[
-            typing.Callable[[core_parameters.abc.Duration], core_events.abc.Event]
+            typing.Callable[["core_parameters.abc.Duration"], core_events.abc.Event]
         ] = None,
-        prolong_simple_event: bool = True,
+        prolong_chronon: bool = True,
     ) -> Envelope[T]:
         if not self:
             raise core_utilities.EmptyEnvelopeError(self, "extend_until")
-        self.sample_at(duration)
+        return self.sample_at(duration)
 
     def split_at(
         self,
-        *absolute_time: core_parameters.abc.Duration,
+        *absolute_time: "core_parameters.abc.Duration.Type",
         ignore_invalid_split_point: bool = False,
     ) -> tuple[Envelope, ...]:
         if not absolute_time:
             raise core_utilities.NoSplitTimeError()
 
-        absolute_time = sorted(absolute_time)
-        if absolute_time[-1] > self.duration and not ignore_invalid_split_point:
-            raise core_utilities.SplitError(absolute_time[-1])
+        abst_list = sorted(
+            [core_parameters.abc.Duration.from_any(t) for t in absolute_time]
+        )
+        if abst_list[-1] > self.duration and not ignore_invalid_split_point:
+            raise core_utilities.SplitError(abst_list[-1])
 
         # We copy, because the 'sample_at' calls would change our envelope.
         self = self.copy()
 
-        for t in absolute_time:
+        for t in abst_list:
             self.sample_at(t)
 
         def add(s, value):
             s.append(s._make_event(0, s.value_to_parameter(value), 0))
 
         segment_tuple = super().split_at(
-            *absolute_time, ignore_invalid_split_point=ignore_invalid_split_point
+            *abst_list, ignore_invalid_split_point=ignore_invalid_split_point
         )
 
         # We already added the interpolation points with 'self.sample_at(*t)',
         # but they are always only available in the segments after the split
         # point (because for each segment the start is included, but the end
         # duration isn't included anymore). So we need to add them to the
         # segments before the split points, otherwise 'value_at' returns wrong
@@ -701,189 +741,7 @@
             # yet anyway (minimal changes).
             # This condition is 'true' if we only split at
             # start time ('env.split_at(0)').
             if s.value_at(s.duration) != v:
                 add(s, v)
 
         return segment_tuple
-
-
-class RelativeEnvelope(Envelope, typing.Generic[T]):
-    __parent_doc_string = Envelope.__doc__.split("\n")[2:]  # type: ignore
-    __after_parameter_text_index = __parent_doc_string.index("")
-    __doc__ = "\n".join(
-        ["Envelope with relative durations and values / parameters.\n"]
-        + __parent_doc_string[:__after_parameter_text_index]
-        + [
-            "    :param base_parameter_and_relative_parameter_to_absolute_parameter: A function",
-            "        which runs when the :func:`resolve` is called. It expects the base parameter",
-            "        and the relative parameter (which is extracted from the envelope events)",
-            "        and should return an absolute parameter.",
-        ]
-        + __parent_doc_string[__after_parameter_text_index:]
-        + [
-            "    The :class:`RelativeEnvelope` adds the :func:`resolve` method",
-            "    to the base class :class:`Envelope`.",
-        ]
-    )
-
-    def __init__(
-        self,
-        *args,
-        base_parameter_and_relative_parameter_to_absolute_parameter: typing.Callable[
-            [core_constants.ParameterType, core_constants.ParameterType],
-            core_constants.ParameterType,
-        ],
-        **kwargs,
-    ):
-        self.base_parameter_and_relative_parameter_to_absolute_parameter = (
-            base_parameter_and_relative_parameter_to_absolute_parameter
-        )
-        super().__init__(*args, **kwargs)
-
-    def resolve(
-        self,
-        duration: core_parameters.abc.Duration | typing.Any,
-        base_parameter: core_constants.ParameterType,
-        resolve_envelope_class: type[Envelope] = Envelope,
-    ) -> Envelope:
-        duration = core_events.configurations.UNKNOWN_OBJECT_TO_DURATION(duration)
-        point_list = []
-        try:
-            duration_factor = duration / self.duration
-        except ZeroDivisionError:
-            duration_factor = core_parameters.DirectDuration(0)
-        for absolute_time, event in zip(self.absolute_time_tuple, self):
-            relative_parameter = self.event_to_parameter(event)
-            new_parameter = (
-                self.base_parameter_and_relative_parameter_to_absolute_parameter(
-                    base_parameter, relative_parameter
-                )
-            )
-            point = (
-                absolute_time * duration_factor,
-                new_parameter,
-                self.event_to_curve_shape(event),
-            )
-            point_list.append(point)
-        return resolve_envelope_class(point_list)
-
-
-TempoPoint: typing.TypeAlias = "core_parameters.abc.TempoPoint | core_constants.Real"
-
-
-class TempoEnvelope(Envelope):
-    """Define dynamic or static tempo trajectories.
-
-    You can either define a new `TempoEnvelope` with instances
-    of classes which inherit from :class:`mutwo.core_parameters.abc.TempoPoint`
-    (for instance :class:`mutwo.core_parameters.DirectTempoPoint`) or with
-    `float` or `int` objects which represent beats per minute.
-
-    Please see the :class:`mutwo.core_events.Envelope` for full documentation
-    for initialization attributes.
-
-    The default parameters of the `TempoEnvelope` class expects
-    :class:`mutwo.core_events.SimpleEvent` to which a tempo point
-    was assigned by the name "tempo_point". This is specified in the global
-    `mutwo.core_events.configurations.DEFAULT_TEMPO_ENVELOPE_PARAMETER_NAME`
-    and can be adjusted.
-
-    **Example:**
-
-    >>> from mutwo import core_events
-    >>> from mutwo import core_parameters
-    >>> # (1) define with floats
-    >>> #     So we have an envelope which moves from tempo 60 to 30
-    >>> #     and back to 60.
-    >>> tempo_envelope_with_float = core_events.TempoEnvelope(
-    ...     [[0, 60], [1, 30], [2, 60]]
-    ... )
-    >>> # (2) define with tempo points
-    >>> tempo_envelope_with_tempo_points = core_events.TempoEnvelope(
-    ...     [
-    ...         [0, core_parameters.DirectTempoPoint(60)],
-    ...         [1, core_parameters.DirectTempoPoint(30)],
-    ...         [2, core_parameters.DirectTempoPoint(30, reference=2)],
-    ...     ]
-    ... )
-    """
-
-    def __init__(
-        self,
-        *args,
-        event_to_parameter: typing.Optional[
-            typing.Callable[[core_events.abc.Event], core_constants.ParameterType]
-        ] = None,
-        value_to_parameter: typing.Optional[
-            typing.Callable[[core_events.Envelope.Value], core_constants.ParameterType]
-        ] = None,
-        parameter_to_value: typing.Optional[
-            typing.Callable[[core_constants.ParameterType], core_events.Envelope.Value]
-        ] = None,
-        apply_parameter_on_event: typing.Optional[
-            typing.Callable[[core_events.abc.Event, core_constants.ParameterType], None]
-        ] = None,
-        default_event_class: type[core_events.abc.Event] = core_events.TempoEvent,
-        initialise_default_event_class: typing.Callable[
-            [type[core_events.abc.Event], core_constants.DurationType],
-            core_events.abc.Event,
-        ] = lambda simple_event_class, duration: simple_event_class(
-            tempo_point=1, duration=duration
-        ),
-        **kwargs,
-    ):
-        def default_event_to_parameter(event: core_events.abc.Event) -> TempoPoint:
-            return getattr(
-                event,
-                core_events.configurations.DEFAULT_TEMPO_ENVELOPE_PARAMETER_NAME,
-            )
-
-        def default_value_to_parameter(value: float) -> TempoPoint:
-            return core_parameters.DirectTempoPoint(value)
-
-        def default_parameter_to_value(parameter: TempoPoint) -> float:
-            # Here we specify, that we allow either core_parameters.abc.TempoPoint
-            # or float/number objects.
-            # So in case we have a core_parameters.abc.TempoPoint 'getattr' is
-            # successful, if not it will return 'parameter', because it
-            # will assume that we have a number based tempo point.
-            return float(
-                getattr(parameter, "absolute_tempo_in_beats_per_minute", parameter)
-            )
-
-        def default_apply_parameter_on_event(
-            event: core_events.abc.Event, parameter: TempoPoint
-        ):
-            setattr(
-                event,
-                core_events.configurations.DEFAULT_TEMPO_ENVELOPE_PARAMETER_NAME,
-                parameter,
-            )
-
-        super().__init__(
-            *args,
-            event_to_parameter=event_to_parameter or default_event_to_parameter,
-            value_to_parameter=value_to_parameter or default_value_to_parameter,
-            parameter_to_value=parameter_to_value or default_parameter_to_value,
-            apply_parameter_on_event=apply_parameter_on_event
-            or default_apply_parameter_on_event,
-            default_event_class=default_event_class,
-            initialise_default_event_class=initialise_default_event_class,
-            **kwargs,
-        )
-
-    def __eq__(self, other: typing.Any):
-        # TempoEnvelope can't use the default '__eq__' method inherited
-        # from list, because this would create endless recursion
-        # (because every event has a TempoEnvelope, so Python would forever
-        #  compare the TempoEnvelopes of TempoEnvelopes).
-        try:
-            return (
-                # Prefer lazy evaluation for better performance
-                # (use 'and' instead of 'all').
-                self.absolute_time_tuple == other.absolute_time_tuple
-                and self.curve_shape_tuple == other.curve_shape_tuple
-                and self.value_tuple == other.value_tuple
-            )
-        except AttributeError:
-            return False
```

### Comparing `mutwo.core-1.4.0/mutwo/core_parameters/abc.py` & `mutwo.core-2.0.0/mutwo/core_parameters/abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,90 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Abstract base classes for different parameters.
 
 This module defines the public API of parameters.
 Most other mutwo classes rely on this API. This means
 when someone creates a new class inheriting from any of the
 abstract parameter classes which are defined in this module,
 she or he can make use of all other mutwo modules with this
 newly created parameter class.
 """
 
 from __future__ import annotations
 
 import abc
+import ast
 import functools
 import operator
 import typing
 
 try:
     import quicktions as fractions
 except ImportError:
     import fractions
+
     _fractions = None
 else:
     import fractions as _fractions
 
-import ranges
-
 from mutwo import core_constants
-from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import core_utilities
 
 __all__ = (
+    "Parameter",
     "SingleValueParameter",
     "SingleNumberParameter",
-    "ParameterWithEnvelope",
     "Duration",
-    "TempoPoint",
+    "Tempo",
 )
 
+T = typing.TypeVar("T", bound="Parameter")
 
-class ParameterWithEnvelope(abc.ABC):
-    """Abstract base class for all parameters with an envelope."""
 
-    def __init__(self, envelope: core_events.RelativeEnvelope):
-        self.envelope = envelope
+class Parameter(core_utilities.MutwoObject, abc.ABC):
+    """A Parameter is the base class for all mutwo parameters
 
-    @property
-    def envelope(self) -> core_events.RelativeEnvelope:
-        return self._envelope
+    It can be useful as a type hint for any code where a parameter
+    object is expected. This isn't necessarily at many places,
+    as mostly any object can be assigned as a parameter to an event.
+    """
 
-    @envelope.setter
-    def envelope(self, new_envelope: typing.Any):
-        if not isinstance(new_envelope, core_events.RelativeEnvelope):
-            raise TypeError(
-                f"Found illegal object '{new_envelope}' of not "
-                f"supported type '{type(new_envelope)}'. "
-                f"Only instances of '{core_events.RelativeEnvelope}'"
-                " are allowed!"
-            )
-        self._envelope = new_envelope
+    @classmethod
+    def from_any(cls: typing.Type[T], object) -> T:
+        """Parse any object to Parameter.
+
+        :param object: Object that is parsed to the parameter.
+        :raises: core_utilities.CannotParseError in case the object
+          can't be parsed to the parameter type.
 
-    def resolve_envelope(
-        self,
-        duration: core_constants.DurationType,
-        # XXX: We can't directly set the default attribute value,
-        # but we have to do it with `None` and resolve it later,
-        # because otherwise we will get a circular import
-        # (core_parameters need to be imported before core_events,
-        #  because we need core_parameters.Duration in core_events).
-        resolve_envelope_class: typing.Optional[type[core_events.Envelope]] = None,
-    ) -> core_events.Envelope:
-        resolve_envelope_class = resolve_envelope_class or core_events.Envelope
-        return self.envelope.resolve(duration, self, resolve_envelope_class)
+        This method is useful for allowing syntactic sugar.
+        """
+        if not isinstance(object, cls):
+            raise core_utilities.CannotParseError(object, cls)
+        return object
 
 
-class SingleValueParameter(abc.ABC):
+class SingleValueParameter(Parameter):
     """Abstract base class for all parameters which are defined by one value.
 
     Classes which inherit from this base class have
     to provide an additional keyword argument `value_name`.
     Furthermore they can provide the optional keyword argument
     `value_return_type`.
 
@@ -139,21 +145,21 @@
                     raise NotImplementedError
 
                 setattr(cls, value_name, property(abstract_method))
 
             if hasattr(cls, "value_name"):
                 raise core_utilities.AlreadyDefinedValueNameError(cls)
 
-            setattr(cls, "value_name", property(lambda _: value_name))
+            setattr(cls, "value_name", classmethod(property(lambda _: value_name)))
 
-    def __str__(self) -> str:
-        return (
-            f"{type(self).__name__}"
-            f"({self.value_name} = {getattr(self, self.value_name)})"  # type: ignore
-        )
+    def __repr_content__(self) -> str:
+        return f"{getattr(self, self.value_name)}"  # type: ignore
+
+    def __str_content__(self) -> str:
+        return f"{getattr(self, self.value_name)}"  # type: ignore
 
     def __eq__(self, other: typing.Any) -> bool:
         try:
             return getattr(self, self.value_name) == getattr(other, self.value_name)  # type: ignore
         except AttributeError:
             return False
 
@@ -227,16 +233,15 @@
             if raise_exception:
                 raise TypeError(
                     f"Can't compare object '{self}' of type '{type(self)}' with"
                     f" object '{other}' of type '{type(other)}'!"
                 )
             return False
 
-        value0, value1 = self._prepare_value_pair_for_comparison(value_pair)
-        return compare(value0, value1)
+        return compare(*self._prepare_value_pair_for_comparison(value_pair))
 
     def __float__(self) -> float:
         return float(getattr(self, self.value_name))  # type: ignore
 
     def __int__(self) -> int:
         return int(float(self))
 
@@ -244,142 +249,138 @@
         return self._compare(other, lambda value0, value1: value0 == value1, False)
 
     def __lt__(self, other: typing.Any) -> bool:
         return self._compare(other, lambda value0, value1: value0 < value1, True)
 
 
 class Duration(
-    SingleNumberParameter, value_name="duration", value_return_type="fractions.Fraction"
+    SingleNumberParameter, value_name="beat_count", value_return_type="float"
 ):
     """Abstract base class for any duration.
 
     If the user wants to define a Duration class, the abstract
-    property :attr:`duration` has to be overridden.
+    property :attr:`beat_count` has to be overridden.
 
-    The attribute :attr:`duration` is stored in unit `beats`.
-
-    The ``duration`` of :mod:`mutwo` events are therefore not
+    The ``duration`` of :mod:`mutwo` events are not
     related to a clear physical unit as for instance seconds.
     The reason for this decision is to simplify musical usage.
     """
 
     direct_comparison_type_tuple = (float, int, fractions.Fraction)
     if _fractions:
         direct_comparison_type_tuple += (_fractions.Fraction,)
 
+    Type: typing.TypeAlias = typing.Union[core_constants.Real, str, "Duration"]
+    """Duration.Type hosts all types that are supported by the duration parser
+    :func:`Duration.from_any`."""
+
     def _math_operation(
-        self, other: DurationOrReal, operation: typing.Callable[[float, float], float]
+        self,
+        other: Duration | core_constants.Real,
+        operation: typing.Callable[[float, float], float],
     ) -> Duration:
-        self.duration = fractions.Fraction(
-            operation(self.duration, getattr(other, "duration", other))
+        self.beat_count = float(
+            operation(self.beat_count, getattr(other, "beat_count", other))
         )
         return self
 
-    @core_utilities.add_copy_option
-    def add(self, other: DurationOrReal) -> Duration:
+    def add(self, other: Duration | core_constants.Real) -> Duration:
         return self._math_operation(other, operator.add)
 
-    @core_utilities.add_copy_option
-    def subtract(self, other: DurationOrReal) -> Duration:
+    def subtract(self, other: Duration | core_constants.Real) -> Duration:
         return self._math_operation(other, operator.sub)
 
-    @core_utilities.add_copy_option
-    def multiply(self, other: DurationOrReal) -> Duration:
+    def multiply(self, other: Duration | core_constants.Real) -> Duration:
         return self._math_operation(other, operator.mul)
 
-    @core_utilities.add_copy_option
-    def divide(self, other: DurationOrReal) -> Duration:
+    def divide(self, other: Duration | core_constants.Real) -> Duration:
         return self._math_operation(other, operator.truediv)
 
-    def __add__(self, other: DurationOrReal) -> Duration:
-        return self.add(other, mutate=False)
+    def __add__(self, other: Duration | core_constants.Real) -> Duration:
+        return self.copy().add(other)
 
-    def __sub__(self, other: DurationOrReal) -> Duration:
-        return self.subtract(other, mutate=False)
+    def __sub__(self, other: Duration | core_constants.Real) -> Duration:
+        return self.copy().subtract(other)
 
-    def __mul__(self, other: DurationOrReal) -> Duration:
-        return self.multiply(other, mutate=False)
+    def __mul__(self, other: Duration | core_constants.Real) -> Duration:
+        return self.copy().multiply(other)
 
-    def __truediv__(self, other: DurationOrReal) -> Duration:
-        return self.divide(other, mutate=False)
+    def __truediv__(self, other: Duration | core_constants.Real) -> Duration:
+        return self.copy().divide(other)
 
     def __float__(self) -> float:
-        return core_utilities.round_floats(
-            float(self.duration),
-            core_parameters.configurations.ROUND_DURATION_TO_N_DIGITS,
-        )
-
-    @property
-    def duration_in_floats(self) -> float:
-        return float(self)
+        return self.beat_count
 
     @property
-    def duration(self) -> fractions.Fraction:
+    @abc.abstractmethod
+    def beat_count(self) -> float:
         ...
 
-    @duration.setter
+    @beat_count.setter
     @abc.abstractmethod
-    def duration(self, duration: fractions.Fraction):
+    def beat_count(self, beat_count: core_constants.Real):
         ...
 
+    @classmethod
+    def from_any(cls: typing.Type[T], object: Duration.Type) -> T:
+        builtin_fraction = _fractions.Fraction if _fractions else fractions.Fraction
+        match object:
+            case Duration():
+                return object
+            case float() | int():
+                return core_parameters.DirectDuration(object)
+            case fractions.Fraction() | builtin_fraction():
+                return core_parameters.RatioDuration(object)
+            case str():
+                f = core_utilities.str_to_number_parser(object)
+                try:
+                    v = f(object)
+                except ValueError:
+                    pass
+                else:
+                    return Duration.from_any(v)
+            case _:
+                pass
 
-DurationOrReal = Duration | core_constants.Real
+        raise core_utilities.CannotParseError(object, cls)
 
 
-class TempoPoint(abc.ABC):
+class Tempo(SingleNumberParameter, value_name="bpm", value_return_type="float"):
     """Represent the active tempo at a specific moment in time.
 
-    If the user wants to define a `TempoPoint` class, the abstract
-    properties :attr:`tempo_or_tempo_range_in_beats_per_minute`
-    and `reference` have to be overridden.
+    If the user wants to define a `Tempo` class, the abstract
+    property :attr:`bpm` needs to be overridden. ``BPM`` is an abbreviation
+    for 'beats per minute' and the unit of the parameter tempo, see more
+    information at this `wikipedia article <https://en.wikipedia.org/wiki/Tempo#Measurement>`_.
     """
 
-    def __repr__(self) -> str:
-        return "{}(BPM = {}, reference = {})".format(
-            type(self).__name__, self.tempo_in_beats_per_minute, self.reference
-        )
-
-    def __eq__(self, other: object) -> bool:
-        attribute_to_compare_tuple = (
-            "tempo_in_beats_per_minute",
-            "reference",
-        )
-        return core_utilities.test_if_objects_are_equal_by_parameter_tuple(
-            self, other, attribute_to_compare_tuple
-        )
-
-    @property
-    @abc.abstractmethod
-    def tempo_or_tempo_range_in_beats_per_minute(
-        self,
-    ) -> core_parameters.constants.TempoOrTempoRangeInBeatsPerMinute:
-        ...
-
-    @property
-    @abc.abstractmethod
-    def reference(self) -> core_constants.Real:
-        ...
+    Type: typing.TypeAlias = typing.Union["Tempo", core_constants.Real]
+    """Tempo.Type hosts all types that are supported by the tempo
+    parser :func:`Tempo.from_any`."""
 
     @property
-    def tempo_in_beats_per_minute(
-        self,
-    ) -> core_parameters.constants.TempoInBeatsPerMinute:
-        """Get tempo in `beats per minute <https://en.wikipedia.org/wiki/Tempo#Measurement>`_
-
-        If :attr:`tempo_or_tempo_range_in_beats_per_minute` is a range
-        mutwo will return the minimal tempo.
-        """
-
-        if isinstance(self.tempo_or_tempo_range_in_beats_per_minute, ranges.Range):
-            return self.tempo_or_tempo_range_in_beats_per_minute.start
-        else:
-            return self.tempo_or_tempo_range_in_beats_per_minute
-
-    @property
-    def absolute_tempo_in_beats_per_minute(self) -> float:
-        """Get absolute tempo in `beats per minute <https://en.wikipedia.org/wiki/Tempo#Measurement>`_
-
-        The absolute tempo takes the :attr:`reference` of the :class:`TempoPoint`
-        into account.
-        """
-
-        return self.tempo_in_beats_per_minute * self.reference
+    def seconds(self) -> float:
+        """How many seconds one beat lasts with current BPM."""
+        return float(60 / self.bpm)
+
+    @classmethod
+    def from_any(cls: typing.Type[T], object: Tempo.Type) -> T:
+        builtin_fraction = _fractions.Fraction if _fractions else fractions.Fraction
+        match object:
+            case Tempo():
+                return object
+            case float() | int() | fractions.Fraction() | builtin_fraction():
+                return core_parameters.DirectTempo(object)
+            case list() | tuple():
+                return core_parameters.FlexTempo(object)
+            case str():
+                f, v = core_utilities.str_to_number_parser(object), None
+                try:
+                    v = f(object)
+                except ValueError:
+                    try:
+                        v = ast.literal_eval(object)
+                    except Exception:
+                        raise core_utilities.CannotParseError(object, cls)
+                return Tempo.from_any(v)
+            case _:
+                raise core_utilities.CannotParseError(object, cls)
```

### Comparing `mutwo.core-1.4.0/mutwo/core_utilities/decorators.py` & `mutwo.core-2.0.0/mutwo/core_utilities/decorators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,40 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2023
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Generic decorators that are used within :mod:`mutwo`."""
 
-import copy
 import functools
 import os
 import types
 import typing
 
-__all__ = ("add_copy_option", "add_tag_to_class", "compute_lazy")
+__all__ = ("compute_lazy",)
 
 from mutwo import core_utilities
 
 
 F = typing.TypeVar("F", bound=typing.Callable[..., typing.Any])
-
-
-def add_copy_option(function: F) -> F:
-    """This decorator adds a copy option for object mutating methods.
-
-    :arg function: The method which shall be adjusted.
-
-    The 'add_copy_option' decorator adds the 'mutate' keyword argument
-    to the decorated method. If 'mutate' is set to ``False``, the decorator deep
-    copies the respective object, then applies the called method on the new
-    copied object and finally returns the copied object. This can be useful
-    for methods that by default mutate its object. When adding this method,
-    it is up to the user whether the original object shall be changed
-    and returned (for mutate=True) or if a copied version of the object with
-    the respective mutation shall be returned (for mutate=False).
-    """
-
-    @functools.wraps(function)
-    def wrapper(self, *args, mutate: bool = True, **kwargs) -> typing.Any:
-        if mutate is True:
-            function(self, *args, **kwargs)
-            return self
-        else:
-            deep_copied_object = copy.deepcopy(self)
-            function(deep_copied_object, *args, **kwargs)
-            return deep_copied_object
-
-    wrapped_function = typing.cast(F, wrapper)
-    wrapped_function.__annotations__.update({"mutate": bool})
-
-    return wrapped_function
-
-
 G = typing.TypeVar("G")
 
 
-def add_tag_to_class(class_to_decorate: G) -> G:
-    """This decorator adds a 'tag' argument to the init method of a class.
-
-    :arg class_to_decorate: The class which shall be decorated.
-    """
-
-    init = class_to_decorate.__init__
-
-    def init_with_tag(self, *args, tag: typing.Optional[str] = None, **kwargs):
-        init(self, *args, **kwargs)
-        self.tag = tag
-
-    class_to_decorate.__init__ = init_with_tag
-    return class_to_decorate
-
-
 def compute_lazy(
     path: str,
     force_to_compute: bool = False,
     pickle_module: typing.Optional[types.ModuleType] = None,
 ):
     """Cache function output to disk via pickle.
```

### Comparing `mutwo.core-1.4.0/mutwo/core_utilities/exceptions.py` & `mutwo.core-2.0.0/mutwo/core_utilities/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,58 @@
-"""Module for mutwo specific exceptions."""
-
-import typing
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from mutwo import core_constants
+"""Module for mutwo specific exceptions."""
 
 __all__ = (
-    "CannotSetDurationOfEmptyComplexEvent",
+    "CannotSetDurationOfEmptyCompound",
     "AlreadyDefinedValueNameError",
     "InvalidAverageValueStartAndEndWarning",
     "InvalidStartValueError",
     "InvalidPointError",
     "ImpossibleToPutInError",
     "ImpossibleToSquashInError",
     "ImpossibleToSlideInError",
     "ImpossibleToExtendUntilError",
     "IneffectiveExtendUntilError",
     "InvalidStartAndEndValueError",
     "InvalidCutOutStartAndEndValuesError",
     "SplitUnavailableChildError",
-    "NoSolutionFoundError",
     "EmptyEnvelopeError",
-    "UndefinedReferenceWarning",
     "ConcatenationError",
     "NoTagError",
     "SplitError",
     "InvalidAbsoluteTime",
     "NoSplitTimeError",
+    "CannotParseError",
 )
 
 
-class CannotSetDurationOfEmptyComplexEvent(Exception):
+class CannotSetDurationOfEmptyCompound(Exception):
     def __init__(self):
         super().__init__(
-            "You tried to set the duration of a complex "
-            "event (e.g. 'SequentialEvent' or 'SimultaneousEvent') "
+            "You tried to set the duration of a Compound "
+            "(e.g. 'Consecution' or 'Concurrence') "
             "which doesn't have any child events. This"
-            " is impossible, because the duration of a 'ComplexEvent'"
-            " is simply the sum of its sequentially ordered child events."
+            " is impossible, because the duration of a 'Compound'"
+            " is simply the sum of its consuentially ordered child events."
         )
 
 
 class AlreadyDefinedValueNameError(Exception):
     def __init__(self, cls):
         super().__init__(
             f"Confusing setup in class '{cls}' which inherits from "
@@ -80,18 +92,18 @@
 
 
 class ImpossibleToPutInError(TypeError):
     def __init__(self, event_to_be_put_into, event_to_put_in, method_name):
         m = method_name
         super().__init__(
             f"Can't {m} '{event_to_put_in}' in '{event_to_be_put_into}'. "
-            "Does the SimultaneousEvent contain SimpleEvents or events that inherit"
-            f" from SimpleEvent? For being able to {m} in, the"
-            " SimultaneousEvent needs to only contain SequentialEvents or"
-            " SimultaneousEvents."
+            "Does the Concurrence contain Chronons or events that inherit"
+            f" from Chronon? For being able to {m} in, the"
+            " Concurrence needs to only contain Consecutions or"
+            " Concurrences."
         )
 
 
 class ImpossibleToSquashInError(ImpossibleToPutInError):
     def __init__(self, event_to_be_squashed_into, event_to_squash_in):
         super().__init__(event_to_be_squashed_into, event_to_squash_in, "squash")
 
@@ -102,99 +114,85 @@
 
 
 class ImpossibleToExtendUntilError(TypeError):
     def __init__(self, event_to_extend_until):
         super().__init__(
             f"Can't extend '{event_to_extend_until}' of type"
             f"'{type(event_to_extend_until)}' which resides inside a "
-            "SimultaneousEvent. Set 'prolong_simple_event' to 'True' in"
-            "case you want simple events to be prolonged."
+            "Concurrence. Set 'prolong_chronon' to 'True' in"
+            "case you want chronons to be prolonged."
         )
 
 
 class IneffectiveExtendUntilError(ValueError):
     def __init__(self, event_to_extend_until):
         super().__init__(
             f"Can't extend empty event '{event_to_extend_until}' of type"
             f"'{type(event_to_extend_until)}'. If you want to extend "
-            "a SimultaneousEvent you should first append an empty "
-            "SequentialEvent to your SimultaneousEvent."
+            "a Concurrence you should first append an empty "
+            "Consecution to your Concurrence."
         )
 
 
 class InvalidStartAndEndValueError(Exception):
     def __init__(self, start, end):
         super().__init__(
             f"Invalid values for start and end property (start = '{start}' "
             f"and end = '{end}')!"
             " Value for 'end' has to be bigger than value for 'start'."
         )
 
 
 class InvalidCutOutStartAndEndValuesError(Exception):
-    def __init__(self, start, end, simple_event, duration):
+    def __init__(self, start, end, chronon, duration):
         super().__init__(
-            f"Can't cut out SimpleEvent '{simple_event}' with "
+            f"Can't cut out Chronon '{chronon}' with "
             f"duration '{duration}' from"
             f" (start = {start} to end = {end})."
         )
 
 
 class SplitError(Exception):
-    def __init__(self, absolute_time: core_constants.DurationType):
+    def __init__(self, absolute_time: "core_parameters.abc.Duration"):
         super().__init__(f"Can't split event at absolute time '{absolute_time}'.")
 
 
 class SplitUnavailableChildError(Exception):
-    def __init__(self, absolute_time: core_constants.DurationType):
+    def __init__(self, absolute_time: "core_parameters.abc.Duration"):
         super().__init__(
             f"Can't split child at absolute time '{absolute_time}'. There is no child"
             " event available at the requested time."
         )
 
 
-class NoSolutionFoundError(Exception):
-    def __init__(self, message: str):
-        super().__init__(message)
-
-
 class EmptyEnvelopeError(Exception):
     def __init__(self, envelope, method):
         super().__init__(f"Can't call '{method}' on empty envelope '{envelope}'!")
 
 
-class UndefinedReferenceWarning(RuntimeWarning):
-    def __init__(self, tempo_point: typing.Any):
-        super().__init__(
-            f"Tempo point '{tempo_point}' of type '{type(tempo_point)}' "
-            "doesn't know attribute 'reference'."
-            " Therefore reference has been set to 1."
-        )
-
-
 class ConcatenationError(TypeError):
     def __init__(self, ancestor, event):
         super().__init__(
             f"Can't concatenate event '{event}' to event '{ancestor}' "
             f"of type '{type(ancestor)}'. It is only possible to"
             " concatenate a new event to events which are instances of "
-            "SequentialEvent or SimultaneousEvent. To fix this bug you can"
-            f" put your event '{ancestor}' inside a SequentialEvent or"
-            " a SimultaneousEvent."
+            "Consecution or Concurrence. To fix this bug you can"
+            f" put your event '{ancestor}' inside a Consecution or"
+            " a Concurrence."
         )
 
 
 class NoTagError(Exception):
     def __init__(self, event_without_tag):
         super().__init__(
             "It's not possible to concatenate an event "
             "with the 'concatenate_by_tag' method if not "
-            "all child events have tags. Here 'mutwo' detected the "
+            "all child events have tags != None. Here 'mutwo' detected the "
             f"child event '{str(event_without_tag)[:50]}...' "
-            "which doesn't have any 'tag' attribute."
+            "which has a tag attribute that is set to 'None'."
         )
 
 
 class InvalidAbsoluteTime(Exception):
     def __init__(self, t):
         super().__init__(
             f"Duration '{t}' is smaller than 0 and can therefore not "
@@ -202,7 +200,12 @@
             "from 0 until +inf and therefore the smallest absolute time is 0."
         )
 
 
 class NoSplitTimeError(Exception):
     def __init__(self):
         super().__init__("Nothing to split (no split time given)!")
+
+
+class CannotParseError(NotImplementedError):
+    def __init__(self, o, parse_type):
+        super().__init__(f"Can't parse '{o}' of type '{type(o)}' to '{parse_type}'!")
```

### Comparing `mutwo.core-1.4.0/mutwo/core_utilities/tools.py` & `mutwo.core-2.0.0/mutwo/core_utilities/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,42 @@
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2024
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
 """Generic utility functions."""
 
 import bisect
 import copy
 import functools
 import itertools
 import logging
 import math
 import operator
 import types
 import typing
+import warnings
+
+try:
+    import quicktions as fractions
+except ImportError:
+    import fractions
+
 
 from mutwo import core_configurations
 from mutwo import core_constants
 
 
 __all__ = (
     "scale",
@@ -30,14 +54,16 @@
     "find_numbers_which_sums_up_to",
     "call_function_except_attribute_error",
     "round_floats",
     "camel_case_to_snake_case",
     "test_if_objects_are_equal_by_parameter_tuple",
     "get_all",
     "get_cls_logger",
+    "str_to_number_parser",
+    "deprecated",
 )
 
 
 def scale(
     value: core_constants.Real,
     old_min: core_constants.Real,
     old_max: core_constants.Real,
@@ -54,15 +80,15 @@
     :param new_max: The maxima of the new range.
     :param translation_shape: 0 for a linear translation,
         values > 0 for a slower change at the beginning,
         values < 0 for a faster change at the beginning.
 
     The algorithmic to change the translation with the
     `translation_shape` has been copied from
-    `expenvelope <https://git.sr.ht/~marcevanstein/expenvelope/tree/master/item/expenvelope/envelope_segment.py#L206>`_
+    `expenvelope <https://git.sr.ht/~marcevanstein/expenvelope/tree/cd4a3710/item/expenvelope/envelope_segment.py#L234>`_
     by M. Evanstein.
 
     **Example:**
 
     >>> from mutwo import core_utilities
     >>> core_utilities.scale(1, 0, 1, 0, 100)
     100.0
@@ -254,16 +280,18 @@
     ('hi', 100)
     """
     return sequence[find_closest_index(item, sequence, key=key)]
 
 
 def uniqify_sequence(
     sequence: typing.Sequence,
-    sort_key: typing.Callable[[typing.Any], core_constants.Real] = None,
-    group_by_key: typing.Callable[[typing.Any], typing.Any] = None,
+    sort_key: typing.Optional[
+        typing.Callable[[typing.Any], core_constants.Real]
+    ] = None,
+    group_by_key: typing.Optional[typing.Callable[[typing.Any], typing.Any]] = None,
 ) -> typing.Iterable:
     """Not-Order preserving function to uniqify any iterable with non-hashable objects.
 
     :param sequence: The iterable which items shall be uniqified.
     :return: Return uniqified version of the entered iterable.
         The function will try to return the same type of the passed
         iterable. If Python raises an error during initialisation of
@@ -338,20 +366,20 @@
 
         character_list.append(character)
 
     return "".join(character_list)
 
 
 def get_nested_item_from_index_sequence(
-    index_sequence: typing.Sequence[int], sequence: typing.Sequence
+    index_sequence: typing.Sequence, sequence: typing.Sequence
 ) -> typing.Any:
     """Get item in nested Sequence.
 
     :param index_sequence: The indices of the nested item.
-    :type index_sequence: typing.Sequence[int]
+    :type index_sequence: typing.Sequence
     :param sequence: A nested sequence.
     :type sequence: typing.Sequence[typing.Any]
 
 
     **Example:**
 
     >>> from mutwo import core_utilities
@@ -364,69 +392,61 @@
 
     for index in index_sequence:
         sequence = sequence[index]
     return sequence
 
 
 def set_nested_item_from_index_sequence(
-    index_sequence: typing.Sequence[int],
+    index_sequence: typing.Sequence,
     sequence: typing.MutableSequence,
     item: typing.Any,
 ) -> None:
     """Set item in nested Sequence.
 
     :param index_sequence: The indices of the nested item which shall be set.
-    :type index_sequence: typing.Sequence[int]
+    :type index_sequence: typing.Sequence
     :param sequence: A nested sequence.
     :type sequence: typing.MutableSequence[typing.Any]
     :param item: The new item value.
     :type item: typing.Any
 
     **Example:**
 
     >>> from mutwo import core_utilities
     >>> nested_sequence = [1, 2, [4, [5, 1], [9, [3]]]]
     >>> core_utilities.set_nested_item_from_index_sequence((2, 2, 0), nested_sequence, 100)
     >>> nested_sequence[2][2][0] = 100  # is equal
     """
-
-    index_count = len(index_sequence)
-    for index_index, index in enumerate(index_sequence):
-        if index_count == index_index + 1:
-            sequence.__setitem__(index, item)
-        else:
-            sequence = sequence[index]
+    for index in index_sequence[:-1]:
+        sequence = sequence[index]
+    sequence.__setitem__(index_sequence[-1], item)
 
 
 def del_nested_item_from_index_sequence(
-    index_sequence: typing.Sequence[int],
+    index_sequence: typing.Sequence,
     sequence: typing.MutableSequence,
 ) -> None:
     """Delete item in nested Sequence.
 
     :param index_sequence: The indices of the nested item which shall be deleted.
-    :type index_sequence: typing.Sequence[int]
+    :type index_sequence: typing.Sequence
     :param sequence: A nested sequence.
     :type sequence: typing.MutableSequence[typing.Any]
 
     **Example:**
 
     >>> from mutwo import core_utilities
     >>> nested_sequence = [1, 2, [4, [5, 1], [9, [3]]]]
     >>> core_utilities.del_nested_item_from_index_sequence((2, 2, 0), nested_sequence)
     >>> nested_sequence
     [1, 2, [4, [5, 1], [[3]]]]
     """
-
-    index_count = len(index_sequence)
-    for index_index, index in enumerate(index_sequence):
-        if index_count == index_index + 1:
-            sequence.__delitem__(index)
-        else:
-            sequence = sequence[index]
+    for index in index_sequence[:-1]:
+        sequence = sequence[index]
+    sequence.__delitem__(index_sequence[-1])
 
 
 def round_floats(
     number_to_round: core_constants.Real, n_digits: int
 ) -> core_constants.Real:
     """Round number if it is an instance of float, otherwise unaltered number.
 
@@ -595,7 +615,59 @@
     :return: A :class:`logging.Logger`.
     """
     if level is None:
         level = core_configurations.LOGGING_LEVEL
     logger = logging.getLogger(f"{cls.__module__}.{cls.__name__}")
     logger.setLevel(level)
     return logger
+
+
+def str_to_number_parser(string: str) -> typing.Callable:
+    """Find function that, if called with string, may return a number.
+
+    :param string: The string for which a suitable function is searched for.
+    :type string: str
+    :return: The function that if called with the string as an input may
+        return a number object (int, float, fraction, ...). It could be
+        that no suitable function could found and calling the function
+        with the string returns an error or unexpected results.
+
+    **Example:**
+
+    >>> from mutwo import core_utilities
+    >>> # floats are detected
+    >>> core_utilities.str_to_number_parser('3.21')('3.21')
+    3.21
+    >>> # int are detected
+    >>> core_utilities.str_to_number_parser('7')('7')
+    7
+    >>> # fractions are detected
+    >>> core_utilities.str_to_number_parser('7/4')('7/4')
+    Fraction(7, 4)
+    """
+    if "." in string:
+        return float
+    elif "/" in string:
+        return fractions.Fraction
+    else:
+        return int
+
+
+def deprecated(info: typing.Optional[str] = None) -> typing.Callable:
+    """Mark a callable as deprecated.
+
+    :param info: Deprecation info printed to the user.
+    :type info: str
+    """
+
+    def _(f: typing.Callable):
+        def wrapper(*args, **kwargs):
+            o = f(*args, **kwargs)
+            try:
+                o._logger.warning(f"DeprecationWarning: {info or 'Deprecation'}")
+            except AttributeError:
+                warnings.warn(Warning(info or "Deprecation"))
+            return o
+
+        return wrapper
+
+    return _
```

### Comparing `mutwo.core-1.4.0/mutwo.core.egg-info/PKG-INFO` & `mutwo.core-2.0.0/mutwo.core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mutwo.core
-Version: 1.4.0
+Version: 2.0.0
 Summary: core library for event based framework mutwo
 Home-page: https://github.com/mutwo-org/mutwo.core
-Author: Tim Pauli, Levin Eric Zimmermann
-Author-email: tim.pauli@folkwang-uni.de, levin.eric.zimmermann@posteo.eu
+Author: Levin Eric Zimmermann, Tim Pauli
+Author-email: levin.eric.zimmermann@posteo.eu, tim.pauli@folkwang-uni.de
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -22,18 +22,15 @@
 Classifier: Topic :: Multimedia :: Sound/Audio :: MIDI
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<2.00,>=1.18
-Requires-Dist: scipy<2.0.0,>=1.4.1
 Requires-Dist: python-ranges<2.0.0,>=1.2.0
-Requires-Dist: quicktions<2.0,>=1.10
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.core
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.core.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.core)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.core-1.4.0/mutwo.core.egg-info/SOURCES.txt` & `mutwo.core-2.0.0/mutwo.core.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,21 @@
 mutwo/core_converters/parsers.py
 mutwo/core_converters/tempos.py
 mutwo/core_events/__init__.py
 mutwo/core_events/abc.py
 mutwo/core_events/basic.py
 mutwo/core_events/configurations.py
 mutwo/core_events/envelopes.py
-mutwo/core_events/tempos.py
-mutwo/core_generators/__init__.py
-mutwo/core_generators/generic.py
+mutwo/core_events/patchparameters.py
 mutwo/core_parameters/__init__.py
 mutwo/core_parameters/abc.py
 mutwo/core_parameters/configurations.py
-mutwo/core_parameters/constants.py
 mutwo/core_parameters/durations.py
 mutwo/core_parameters/tempos.py
 mutwo/core_utilities/__init__.py
 mutwo/core_utilities/configurations.py
 mutwo/core_utilities/decorators.py
 mutwo/core_utilities/exceptions.py
+mutwo/core_utilities/mutwo.py
 mutwo/core_utilities/tests.py
 mutwo/core_utilities/tools.py
 mutwo/core_version/__init__.py
```

### Comparing `mutwo.core-1.4.0/setup.py` & `mutwo.core-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,25 @@
-import setuptools  # type: ignore
+# This file is part of mutwo, ecosystem for time-based arts.
+#
+# Copyright (C) 2020-2023
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import setuptools  # type: ignore
 
 version = {}
 with open("mutwo/core_version/__init__.py") as fp:
     exec(fp.read(), version)
 
 VERSION = version["VERSION"]
 
@@ -15,33 +31,30 @@
 setuptools.setup(
     name="mutwo.core",
     version=VERSION,
     license="GPL",
     description="core library for event based framework mutwo",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author="Tim Pauli, Levin Eric Zimmermann",
-    author_email="tim.pauli@folkwang-uni.de, levin.eric.zimmermann@posteo.eu",
+    author="Levin Eric Zimmermann, Tim Pauli",
+    author_email="levin.eric.zimmermann@posteo.eu, tim.pauli@folkwang-uni.de",
     url="https://github.com/mutwo-org/mutwo.core",
     project_urls={"Documentation": "https://mutwo-org.github.io"},
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "numpy>=1.18, <2.00",
-        "scipy>=1.4.1, <2.0.0",
         "python-ranges>=1.2.0, <2.0.0",
-        "quicktions>=1.10, <2.0",
     ],
     extras_require=extras_require,
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Education",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: Unix",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.10",
```

