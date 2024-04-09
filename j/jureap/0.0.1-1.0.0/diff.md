# Comparing `tmp/jureap-0.0.1.tar.gz` & `tmp/jureap-1.0.0.tar.gz`

## Comparing `jureap-0.0.1.tar` & `jureap-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jureap-0.0.1/.gitignore.local
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 jureap-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 jureap-0.0.1/.nvimrc
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jureap-0.0.1/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 jureap-0.0.1/src/jureap/__init__.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 jureap-0.0.1/src/jureap/metadata.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 jureap-0.0.1/test/bin/test_smoke.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jureap-0.0.1/test/share/env/env.json
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 jureap-0.0.1/test/share/result/baseline/data/01.csv
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 jureap-0.0.1/test/share/result/comparison/data/01.csv
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 jureap-0.0.1/test/share/result/strong/data/01.csv
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jureap-0.0.1/test/share/result/weak/data/01.csv
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 jureap-0.0.1/.gitignore
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 jureap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jureap-0.0.1/readme.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 jureap-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jureap-1.0.0/.git
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 jureap-1.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jureap-1.0.0/.reuse/dep5
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 jureap-1.0.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/benchmark.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/metadata.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/cli/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/cli/parser.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 jureap-1.0.0/src/jureap/log/__init__.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 jureap-1.0.0/test/bin/test_log.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 jureap-1.0.0/test/bin/test_smoke.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 jureap-1.0.0/test/share/log/00.input.csv
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jureap-1.0.0/test/share/log/00.output.json
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 jureap-1.0.0/test/share/log/01.input.csv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jureap-1.0.0/test/share/log/01.output.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 jureap-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 jureap-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jureap-1.0.0/readme.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jureap-1.0.0/PKG-INFO
```

### Comparing `jureap-0.0.1/.gitlab-ci.yml` & `jureap-1.0.0/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,31 +11,31 @@
   before_script:
     - python -m venv /root/venv
     - source /root/venv/bin/activate
     - pip install --upgrade pip
     - pip install hatch
     - pip install mypy
     - pip install types-PyYAML
-    - hatch env create
+    - hatch env create types
   script:
-    - hatch env run mypy .
+    - hatch env run --env types mypy .
 
 ####################################################################################################
 # Compatibility Checking
 ####################################################################################################
 compat.latest:
   image: python:latest
   before_script:
     - python -m venv /root/venv
     - source /root/venv/bin/activate
     - pip install --upgrade pip
     - pip install hatch pytest
-    - hatch env create
+    - hatch env create test
   script:
-    - hatch env run pytest
+    - hatch env run --env test --  pytest
 
 ####################################################################################################
 # License Check
 ####################################################################################################
 license.check:
   stage: .post
   tags: ["docker"]
```

### Comparing `jureap-0.0.1/LICENSES/Apache-2.0.txt` & `jureap-1.0.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `jureap-0.0.1/PKG-INFO` & `jureap-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: jureap
-Version: 0.0.1
+Version: 1.0.0
 Summary: A helper script for the jureap project
 Project-URL: Documentation, https://gitlab.jsc.fz-juelich.de/exacb/jureap
 Project-URL: Issues, https://gitlab.jsc.fz-juelich.de/exacb/jureap
 Project-URL: Source, https://gitlab.jsc.fz-juelich.de/exacb/jureap
 Author-email: Jayesh Badwaik <j.badwaik@fz-juelich.de>
 License-Expression: Apache-2.0
 Requires-Dist: semver
 Description-Content-Type: text/markdown
 
 <!--
 - SPDX-License-Identifier: Apache-2.0
 - Copyright (C) 2024 Jayesh Badwaik <j.badwaik@fz-juelich.de>
 -->
 
-# exacb
+# jureap
 
-Helper scripts for the [exacb](https://go.fzj.de/exacb) project.
+Report and log generator for jureap
```

