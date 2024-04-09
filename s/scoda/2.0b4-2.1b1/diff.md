# Comparing `tmp/scoda-2.0b4.tar.gz` & `tmp/scoda-2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-2.0b4.tar", last modified: Tue Mar 26 15:53:24 2024, max compression
+gzip compressed data, was "scoda-2.1b1.tar", last modified: Tue Apr  9 11:36:46 2024, max compression
```

## Comparing `scoda-2.0b4.tar` & `scoda-2.1b1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.398388 scoda-2.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-26 15:53:13.000000 scoda-2.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-26 15:53:24.394388 scoda-2.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-03-26 15:53:13.000000 scoda-2.0b4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 15:53:13.000000 scoda-2.0b4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.390388 scoda-2.0b4/scoda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.390388 scoda-2.0b4/scoda/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/config/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.390388 scoda-2.0b4/scoda/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/elements/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/elements/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/elements/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/elements/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.390388 scoda-2.0b4/scoda/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/exceptions/bar_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/exceptions/sequence_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/exceptions/tokenisation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/exceptions/track_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda/midi/
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/midi/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/midi/midi_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/sequences/absolute_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/sequences/abstract_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    35044 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/sequences/relative_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    23639 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/sequences/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda/tokenisation/
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/tokenisation/base_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/tokenisation/gridlike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/tokenisation/midilike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25630 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/tokenisation/notelike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/tokenisation/transposed_notelike_tokenisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/utils/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/utils/music_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/utils/scoda_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-03-26 15:53:13.000000 scoda-2.0b4/scoda/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 15:53:24.394388 scoda-2.0b4/scoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-26 15:53:24.000000 scoda-2.0b4/scoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-26 15:53:24.000000 scoda-2.0b4/scoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 15:53:24.000000 scoda-2.0b4/scoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-26 15:53:24.000000 scoda-2.0b4/scoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-26 15:53:24.000000 scoda-2.0b4/scoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 15:53:24.398388 scoda-2.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 11:36:42.000000 scoda-2.1b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-09 11:36:46.694118 scoda-2.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-09 11:36:42.000000 scoda-2.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 11:36:42.000000 scoda-2.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.686118 scoda-2.1b1/scoda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/config/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/elements/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/bar_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/sequence_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/tokenisation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/exceptions/track_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/midi/midi_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.690118 scoda-2.1b1/scoda/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/music_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/scoda_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/misc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)    21873 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/absolute_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/abstract_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/relative_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23636 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda/tokenisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/base_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/gridlike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/midilike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25748 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/notelike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2024-04-09 11:36:42.000000 scoda-2.1b1/scoda/tokenisation/transposed_notelike_tokenisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:36:46.694118 scoda-2.1b1/scoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 11:36:46.000000 scoda-2.1b1/scoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:36:46.694118 scoda-2.1b1/setup.cfg
```

### Comparing `scoda-2.0b4/LICENSE.md` & `scoda-2.1b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/PKG-INFO` & `scoda-2.1b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.0b4
+Version: 2.1b1
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,35 +24,35 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/FelixSchoen/S-Coda
 Project-URL: Bugtracker, https://github.com/FelixSchoen/S-Coda/issues
 Keywords: midi,music
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: numpy>=1.26
-Requires-Dist: mido>=1.3
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: mido
 Provides-Extra: test
-Requires-Dist: pytest>=7.4; extra == "test"
-Requires-Dist: pytest-xdist>=3.5; extra == "test"
-Requires-Dist: pytest-cov>=4.1; extra == "test"
-Requires-Dist: coverage>=7.3; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: coverage; extra == "test"
 Provides-Extra: deploy
-Requires-Dist: build>=1.0; extra == "deploy"
-Requires-Dist: twine>=4.0; extra == "deploy"
-Requires-Dist: pdoc3>=0.10; extra == "deploy"
+Requires-Dist: build; extra == "deploy"
+Requires-Dist: twine; extra == "deploy"
+Requires-Dist: pdoc3; extra == "deploy"
 
 # S-Coda
 
 [![GitHub Release](https://img.shields.io/github/v/release/FelixSchoen/S-Coda?include_prereleases&label=Latest%20Release)](https://github.com/FelixSchoen/S-Coda/releases)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/FelixSchoen/S-Coda/scoda_test.yml?label=Build)](https://github.com/FelixSchoen/S-Coda/actions/workflows/scoda_test.yml)
-[![Python Version](https://img.shields.io/badge/Python%20Version-3.10-blue)](https://www.python.org/downloads/release/python-31013)
+[![Python Version](https://img.shields.io/badge/Python%20Version-3.11-blue)](https://www.python.org/downloads/release/python-3119)
 
 [![DOI](https://img.shields.io/badge/DOI-10.34726%2Fhss.2023.103585-blue)](https://doi.org/10.34726/hss.2023.103585)
 [![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--47546--7_19-blue)](https://doi.org/10.1007/978-3-031-47546-7_19)
 
 ## Overview
 
 S-Coda is a Python library for handling MIDI files.
@@ -66,21 +66,21 @@
 - judging the difficulty of pieces
 
 S-Coda was used in our project [PAUL-2](https://github.com/FelixSchoen/PAUL-2) to process MIDI files.
 For information about how to use S-Coda we refer to chapter 5 of the [thesis](https://doi.org/10.34726/hss.2023.103585) in which S-Coda was introduced.
 
 ## Installation
 
-We recommend installing S-Coda from PyPI using pip:
+We recommend installing S-Coda from [PyPI](https://pypi.org/project/scoda/) using pip:
 
 ```pip install scoda```
 
 ## Changelog
 
-See `CHANGELOG.md` for a detailed changelog.
+See [`CHANGELOG.md`](https://github.com/FelixSchoen/S-Coda/blob/main/CHANGELOG.md) for a detailed changelog.
 
 ## Usage
 
 We refer to the aforementioned thesis for a more in-depth guide on how to use S-Coda.
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
```

### Comparing `scoda-2.0b4/README.md` & `scoda-2.1b1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # S-Coda
 
 [![GitHub Release](https://img.shields.io/github/v/release/FelixSchoen/S-Coda?include_prereleases&label=Latest%20Release)](https://github.com/FelixSchoen/S-Coda/releases)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/FelixSchoen/S-Coda/scoda_test.yml?label=Build)](https://github.com/FelixSchoen/S-Coda/actions/workflows/scoda_test.yml)
-[![Python Version](https://img.shields.io/badge/Python%20Version-3.10-blue)](https://www.python.org/downloads/release/python-31013)
+[![Python Version](https://img.shields.io/badge/Python%20Version-3.11-blue)](https://www.python.org/downloads/release/python-3119)
 
 [![DOI](https://img.shields.io/badge/DOI-10.34726%2Fhss.2023.103585-blue)](https://doi.org/10.34726/hss.2023.103585)
 [![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--47546--7_19-blue)](https://doi.org/10.1007/978-3-031-47546-7_19)
 
 ## Overview
 
 S-Coda is a Python library for handling MIDI files.
@@ -20,21 +20,21 @@
 - judging the difficulty of pieces
 
 S-Coda was used in our project [PAUL-2](https://github.com/FelixSchoen/PAUL-2) to process MIDI files.
 For information about how to use S-Coda we refer to chapter 5 of the [thesis](https://doi.org/10.34726/hss.2023.103585) in which S-Coda was introduced.
 
 ## Installation
 
-We recommend installing S-Coda from PyPI using pip:
+We recommend installing S-Coda from [PyPI](https://pypi.org/project/scoda/) using pip:
 
 ```pip install scoda```
 
 ## Changelog
 
-See `CHANGELOG.md` for a detailed changelog.
+See [`CHANGELOG.md`](https://github.com/FelixSchoen/S-Coda/blob/main/CHANGELOG.md) for a detailed changelog.
 
 ## Usage
 
 We refer to the aforementioned thesis for a more in-depth guide on how to use S-Coda.
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
```

### Comparing `scoda-2.0b4/pyproject.toml` & `scoda-2.1b1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "scoda"
-version = "2.0-beta.4"
+version = "2.1-beta.1"
 authors = [{ name = "Felix Schön", email = "schoen@kr.tuwien.ac.at" }]
 description = "A MIDI and music data manipulation library"
 readme = "README.md"
-requires-python = ">= 3.10"
+requires-python = ">= 3.11"
 keywords = ["midi", "music"]
 license = { file = "LICENSE.md" }
 dependencies = [
-    "matplotlib >= 3.8",
-    "numpy >= 1.26",
-    "mido >= 1.3"
+    "matplotlib",
+    "numpy",
+    "mido"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FelixSchoen/S-Coda"
 "Bugtracker" = "https://github.com/FelixSchoen/S-Coda/issues"
 
 [project.optional-dependencies]
 test = [
-    "pytest >= 7.4",
-    "pytest-xdist >= 3.5",
-    "pytest-cov >= 4.1",
-    "coverage >= 7.3"
+    "pytest",
+    "pytest-xdist",
+    "pytest-cov",
+    "coverage"
 ]
 deploy = [
-    "build >= 1.0",
-    "twine >= 4.0",
-    "pdoc3 >= 0.10"
+    "build",
+    "twine",
+    "pdoc3"
 ]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
```

### Comparing `scoda-2.0b4/scoda/config/settings.json` & `scoda-2.1b1/scoda/config/settings.json`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/elements/bar.py` & `scoda-2.1b1/scoda/elements/bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import copy
 
 from scoda.elements.message import Message
 from scoda.exceptions.bar_exception import BarException
+from scoda.misc.enumerations import MessageType
+from scoda.misc.music_theory import Key
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
-from scoda.utils.enumerations import MessageType
-from scoda.utils.music_theory import Key
 
 
 class Bar:
     """Class representing a single bar, its length defined by a time signature.
     """
 
     def __init__(self, sequence: Sequence, numerator: int, denominator: int, key=None) -> None:
```

### Comparing `scoda-2.0b4/scoda/elements/composition.py` & `scoda-2.1b1/scoda/elements/composition.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/elements/message.py` & `scoda-2.1b1/scoda/elements/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from scoda.utils.enumerations import MessageType
-from scoda.utils.music_theory import Key
+from scoda.misc.enumerations import MessageType
+from scoda.misc.music_theory import Key
 
 
 class Message:
     """Class representing a musical message.
     """
 
     def __init__(self, message_type: MessageType = None, note: int = None, velocity: int = None, control: int = None,
```

### Comparing `scoda-2.0b4/scoda/elements/track.py` & `scoda-2.1b1/scoda/elements/track.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import copy
 
 from scoda.elements.bar import Bar
 from scoda.exceptions.track_exception import TrackException
+from scoda.misc.enumerations import MessageType
 from scoda.sequences.sequence import Sequence
-from scoda.utils.enumerations import MessageType
 
 
 class Track:
     """Class representing a track, which is made of (multiple) bars.
     """
 
     def __init__(self, bars: [Bar], name: str = None) -> None:
```

### Comparing `scoda-2.0b4/scoda/midi/midi_file.py` & `scoda-2.1b1/scoda/midi/midi_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import copy
 from typing import TYPE_CHECKING
 
 import mido
 
 from scoda.elements.message import Message
 from scoda.midi.midi_track import MidiTrack
+from scoda.misc.enumerations import MessageType
+from scoda.misc.scoda_logging import get_logger
 from scoda.settings.settings import PPQN
-from scoda.utils.enumerations import MessageType
-from scoda.utils.scoda_logging import get_logger
 
 if TYPE_CHECKING:
     from scoda.sequences.sequence import Sequence
 
 
 class MidiFile:
     LOGGER = get_logger(__name__)
```

### Comparing `scoda-2.0b4/scoda/midi/midi_message.py` & `scoda-2.1b1/scoda/midi/midi_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from scoda.elements.message import Message
-from scoda.utils.enumerations import MessageType
-from scoda.utils.music_theory import MusicMapping
+from scoda.misc.enumerations import MessageType
+from scoda.misc.music_theory import MusicMapping
 
 
 class MidiMessage:
 
     def __init__(self, message_type=None, control=None, denominator=None, numerator=None, key=None, note=None,
                  time=None, velocity=None, program=None) -> None:
         super().__init__()
```

### Comparing `scoda-2.0b4/scoda/midi/midi_track.py` & `scoda-2.1b1/scoda/midi/midi_track.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import mido
 
 from scoda.midi.midi_message import MidiMessage
-from scoda.utils.enumerations import MessageType
+from scoda.misc.enumerations import MessageType
 
 
 class MidiTrack:
 
     def __init__(self) -> None:
         super().__init__()
         self.name = ""
```

### Comparing `scoda-2.0b4/scoda/sequences/absolute_sequence.py` & `scoda-2.1b1/scoda/sequences/absolute_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import copy
 from statistics import geometric_mean
 from typing import TYPE_CHECKING
 
 from scoda.elements.message import Message
 from scoda.exceptions.sequence_exception import SequenceException
+from scoda.misc.enumerations import MessageType
+from scoda.misc.scoda_logging import get_logger
+from scoda.misc.util import binary_insort, find_minimal_distance, regress, minmax, simple_regression, \
+    get_note_durations, \
+    get_tuplet_durations, get_dotted_note_durations
 from scoda.sequences.abstract_sequence import AbstractSequence
 from scoda.settings.settings import PPQN, DIFF_DUAL_NOTE_VALUES_UPPER_BOUND, \
     DIFF_DUAL_NOTE_VALUES_LOWER_BOUND, NOTE_VALUE_UPPER_BOUND, NOTE_VALUE_LOWER_BOUND, VALID_TUPLETS, DOTTED_ITERATIONS, \
     SCALE_LOGLIKE
-from scoda.utils.enumerations import MessageType
-from scoda.utils.scoda_logging import get_logger
-from scoda.utils.util import binary_insort, find_minimal_distance, regress, minmax, simple_regression, \
-    get_note_durations, \
-    get_tuplet_durations, get_dotted_note_durations
 
 if TYPE_CHECKING:
     from scoda.sequences.relative_sequence import RelativeSequence
 
 
 class AbsoluteSequence(AbstractSequence):
     """Class representing a sequence with absolute message timings.
```

### Comparing `scoda-2.0b4/scoda/sequences/abstract_sequence.py` & `scoda-2.1b1/scoda/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/sequences/relative_sequence.py` & `scoda-2.1b1/scoda/sequences/relative_sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from statistics import mean
 from typing import TYPE_CHECKING
 
 from scoda.elements.message import Message
 from scoda.exceptions.sequence_exception import SequenceException
 from scoda.midi.midi_message import MidiMessage
 from scoda.midi.midi_track import MidiTrack
+from scoda.misc.enumerations import MessageType
+from scoda.misc.music_theory import Note, Key, MusicMapping
+from scoda.misc.scoda_logging import get_logger
+from scoda.misc.util import minmax, simple_regression
 from scoda.sequences.abstract_sequence import AbstractSequence
 from scoda.settings.settings import NOTE_LOWER_BOUND, NOTE_UPPER_BOUND, PPQN, DIFF_DUAL_DISTANCES_UPPER_BOUND, \
     DIFF_DUAL_DISTANCES_LOWER_BOUND, DIFF_DUAL_PATTERN_COVERAGE_UPPER_BOUND, DIFF_DUAL_PATTERN_COVERAGE_LOWER_BOUND, \
     PATTERN_LENGTH_MIN, REGEX_PATTERN, REGEX_SUBPATTERN, DIFF_DUAL_NOTE_CLASSES_UPPER_BOUND, \
     DIFF_DUAL_NOTE_CLASSES_LOWER_BOUND, \
     DIFF_DUAL_NOTE_AMOUNT_UPPER_BOUND, DIFF_DUAL_NOTE_AMOUNT_LOWER_BOUND, PATTERN_SECONDS_SEARCH_DURATION, \
     DIFF_DUAL_NOTE_CONCURRENT_UPPER_BOUND, DIFF_DUAL_NOTE_CONCURRENT_LOWER_BOUND, DIFF_DUAL_ACCIDENTALS_UPPER_BOUND, \
     DIFF_DUAL_ACCIDENTALS_LOWER_BOUND
-from scoda.utils.enumerations import MessageType
-from scoda.utils.music_theory import Note, Key, MusicMapping
-from scoda.utils.scoda_logging import get_logger
-from scoda.utils.util import minmax, simple_regression
 
 if TYPE_CHECKING:
     from scoda.sequences.absolute_sequence import AbsoluteSequence
 
 
 class RelativeSequence(AbstractSequence):
     """Class representing a sequence with relative message timings.
```

### Comparing `scoda-2.0b4/scoda/sequences/sequence.py` & `scoda-2.1b1/scoda/sequences/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import numpy as np
 from matplotlib import pyplot as plt, pyplot
 from matplotlib.patches import Rectangle
 
 from scoda.elements.message import Message
 from scoda.midi.midi_file import MidiFile
 from scoda.midi.midi_track import MidiTrack
+from scoda.misc.enumerations import MessageType
+from scoda.misc.music_theory import Key
+from scoda.misc.util import minmax, simple_regression
 from scoda.sequences.absolute_sequence import AbsoluteSequence
 from scoda.sequences.relative_sequence import RelativeSequence
 from scoda.settings.settings import PPQN, NOTE_LOWER_BOUND, NOTE_UPPER_BOUND, VELOCITY_MAX
-from scoda.utils.enumerations import MessageType
-from scoda.utils.music_theory import Key
-from scoda.utils.util import minmax, simple_regression
 
 if TYPE_CHECKING:
     from scoda.elements.bar import Bar
 
 
 class Sequence:
     """Wrapper for `scoda.sequence.absolute_sequence.AbsoluteSequence` and
```

### Comparing `scoda-2.0b4/scoda/settings/settings.py` & `scoda-2.1b1/scoda/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/tokenisation/base_tokenisation.py` & `scoda-2.1b1/scoda/tokenisation/base_tokenisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 
 from scoda.exceptions.tokenisation_exception import TokenisationException
+from scoda.misc.enumerations import Flags
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
-from scoda.utils.enumerations import Flags
 
 
 class BaseTokeniser(ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__()
```

### Comparing `scoda-2.0b4/scoda/tokenisation/gridlike_tokenisation.py` & `scoda-2.1b1/scoda/tokenisation/gridlike_tokenisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from abc import ABC
 
 from scoda.elements.message import Message
 from scoda.exceptions.tokenisation_exception import TokenisationException
+from scoda.misc.enumerations import MessageType, Flags
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
-from scoda.utils.enumerations import MessageType, Flags
 
 
 class BaseGridlikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
```

### Comparing `scoda-2.0b4/scoda/tokenisation/midilike_tokenisation.py` & `scoda-2.1b1/scoda/tokenisation/midilike_tokenisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 
 from scoda.elements.message import Message
 from scoda.exceptions.tokenisation_exception import TokenisationException
+from scoda.misc.enumerations import Flags, MessageType
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
-from scoda.utils.enumerations import Flags, MessageType
 
 
 class BaseMidilikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
```

### Comparing `scoda-2.0b4/scoda/tokenisation/notelike_tokenisation.py` & `scoda-2.1b1/scoda/tokenisation/notelike_tokenisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import math
 from abc import ABC
 
 from scoda.elements.message import Message
 from scoda.exceptions.tokenisation_exception import TokenisationException
+from scoda.misc.enumerations import Flags, MessageType
+from scoda.misc.music_theory import CircleOfFifths
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
-from scoda.utils.enumerations import Flags, MessageType
-from scoda.utils.music_theory import CircleOfFifths
 
 
 class BaseNotelikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
 
@@ -34,15 +34,15 @@
 
     def __init__(self, running_value: bool, running_pitch: bool, running_time_sig: bool) -> None:
         super().__init__(running_value, running_time_sig)
 
         self.flags[Flags.RUNNING_PITCH] = running_pitch
 
     def tokenise(self, sequence: Sequence, apply_buffer: bool = True, reset_time: bool = True,
-                 insert_border_tokens: bool = False) -> list[int]:
+                 insert_trailing_separator_token: bool = True, insert_border_tokens: bool = False) -> list[int]:
         tokens = []
         event_pairings = sequence.abs.get_message_time_pairings(
             [MessageType.NOTE_ON, MessageType.NOTE_OFF, MessageType.TIME_SIGNATURE, MessageType.INTERNAL])
 
         for event_pairing in event_pairings:
             msg_type = event_pairing[0].message_type
             msg_time = event_pairing[0].time
@@ -96,14 +96,17 @@
         if apply_buffer:
             tokens.extend(
                 self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=3, value_shift=4))
 
         if reset_time:
             self.reset_time()
 
+        if insert_trailing_separator_token:
+            tokens.append(4)
+
         if insert_border_tokens:
             tokens.insert(0, 1)
             tokens.append(2)
 
         return tokens
 
     @staticmethod
```

### Comparing `scoda-2.0b4/scoda/tokenisation/transposed_notelike_tokenisation.py` & `scoda-2.1b1/scoda/tokenisation/transposed_notelike_tokenisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import math
 from abc import ABC
 
 from scoda.elements.message import Message
 from scoda.exceptions.tokenisation_exception import TokenisationException
+from scoda.misc.enumerations import Flags, MessageType
 from scoda.sequences.sequence import Sequence
 from scoda.settings.settings import PPQN
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
-from scoda.utils.enumerations import Flags, MessageType
 
 
 class BaseTransposedNotelikeTokeniser(BaseTokeniser, ABC):
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
```

### Comparing `scoda-2.0b4/scoda/utils/enumerations.py` & `scoda-2.1b1/scoda/misc/enumerations.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/utils/music_theory.py` & `scoda-2.1b1/scoda/misc/music_theory.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/utils/scoda_logging.py` & `scoda-2.1b1/scoda/misc/scoda_logging.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda/utils/util.py` & `scoda-2.1b1/scoda/misc/util.py`

 * *Files identical despite different names*

### Comparing `scoda-2.0b4/scoda.egg-info/PKG-INFO` & `scoda-2.1b1/scoda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.0b4
+Version: 2.1b1
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,35 +24,35 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/FelixSchoen/S-Coda
 Project-URL: Bugtracker, https://github.com/FelixSchoen/S-Coda/issues
 Keywords: midi,music
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: numpy>=1.26
-Requires-Dist: mido>=1.3
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: mido
 Provides-Extra: test
-Requires-Dist: pytest>=7.4; extra == "test"
-Requires-Dist: pytest-xdist>=3.5; extra == "test"
-Requires-Dist: pytest-cov>=4.1; extra == "test"
-Requires-Dist: coverage>=7.3; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-xdist; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: coverage; extra == "test"
 Provides-Extra: deploy
-Requires-Dist: build>=1.0; extra == "deploy"
-Requires-Dist: twine>=4.0; extra == "deploy"
-Requires-Dist: pdoc3>=0.10; extra == "deploy"
+Requires-Dist: build; extra == "deploy"
+Requires-Dist: twine; extra == "deploy"
+Requires-Dist: pdoc3; extra == "deploy"
 
 # S-Coda
 
 [![GitHub Release](https://img.shields.io/github/v/release/FelixSchoen/S-Coda?include_prereleases&label=Latest%20Release)](https://github.com/FelixSchoen/S-Coda/releases)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/FelixSchoen/S-Coda/scoda_test.yml?label=Build)](https://github.com/FelixSchoen/S-Coda/actions/workflows/scoda_test.yml)
-[![Python Version](https://img.shields.io/badge/Python%20Version-3.10-blue)](https://www.python.org/downloads/release/python-31013)
+[![Python Version](https://img.shields.io/badge/Python%20Version-3.11-blue)](https://www.python.org/downloads/release/python-3119)
 
 [![DOI](https://img.shields.io/badge/DOI-10.34726%2Fhss.2023.103585-blue)](https://doi.org/10.34726/hss.2023.103585)
 [![DOI](https://img.shields.io/badge/DOI-10.1007%2F978--3--031--47546--7_19-blue)](https://doi.org/10.1007/978-3-031-47546-7_19)
 
 ## Overview
 
 S-Coda is a Python library for handling MIDI files.
@@ -66,21 +66,21 @@
 - judging the difficulty of pieces
 
 S-Coda was used in our project [PAUL-2](https://github.com/FelixSchoen/PAUL-2) to process MIDI files.
 For information about how to use S-Coda we refer to chapter 5 of the [thesis](https://doi.org/10.34726/hss.2023.103585) in which S-Coda was introduced.
 
 ## Installation
 
-We recommend installing S-Coda from PyPI using pip:
+We recommend installing S-Coda from [PyPI](https://pypi.org/project/scoda/) using pip:
 
 ```pip install scoda```
 
 ## Changelog
 
-See `CHANGELOG.md` for a detailed changelog.
+See [`CHANGELOG.md`](https://github.com/FelixSchoen/S-Coda/blob/main/CHANGELOG.md) for a detailed changelog.
 
 ## Usage
 
 We refer to the aforementioned thesis for a more in-depth guide on how to use S-Coda.
 We provide a short listing on how to use basic S-Coda functions:
 
 ```python
```

### Comparing `scoda-2.0b4/scoda.egg-info/SOURCES.txt` & `scoda-2.1b1/scoda.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 scoda/exceptions/bar_exception.py
 scoda/exceptions/sequence_exception.py
 scoda/exceptions/tokenisation_exception.py
 scoda/exceptions/track_exception.py
 scoda/midi/midi_file.py
 scoda/midi/midi_message.py
 scoda/midi/midi_track.py
+scoda/misc/decorators.py
+scoda/misc/enumerations.py
+scoda/misc/music_theory.py
+scoda/misc/scoda_logging.py
+scoda/misc/util.py
 scoda/sequences/absolute_sequence.py
 scoda/sequences/abstract_sequence.py
 scoda/sequences/relative_sequence.py
 scoda/sequences/sequence.py
 scoda/settings/settings.py
 scoda/tokenisation/base_tokenisation.py
 scoda/tokenisation/gridlike_tokenisation.py
 scoda/tokenisation/midilike_tokenisation.py
 scoda/tokenisation/notelike_tokenisation.py
-scoda/tokenisation/transposed_notelike_tokenisation.py
-scoda/utils/decorators.py
-scoda/utils/enumerations.py
-scoda/utils/music_theory.py
-scoda/utils/scoda_logging.py
-scoda/utils/util.py
+scoda/tokenisation/transposed_notelike_tokenisation.py
```

