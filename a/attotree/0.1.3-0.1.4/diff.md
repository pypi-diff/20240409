# Comparing `tmp/attotree-0.1.3.tar.gz` & `tmp/attotree-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attotree-0.1.3.tar", last modified: Mon Apr  8 18:11:08 2024, max compression
+gzip compressed data, was "attotree-0.1.4.tar", last modified: Tue Apr  9 00:23:49 2024, max compression
```

## Comparing `attotree-0.1.3.tar` & `attotree-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.562548 attotree-0.1.3/
--rw-r--r--   0 karel      (503) staff       (20)     1071 2024-01-15 14:46:06.000000 attotree-0.1.3/LICENSE.txt
--rw-r--r--   0 karel      (503) staff       (20)     2650 2024-04-08 18:11:08.561979 attotree-0.1.3/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)     2072 2024-04-08 18:04:36.000000 attotree-0.1.3/README.rst
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.476066 attotree-0.1.3/attotree/
--rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 attotree-0.1.3/attotree/__init__.py
--rwxr-xr-x   0 karel      (503) staff       (20)    12878 2024-04-08 18:04:36.000000 attotree-0.1.3/attotree/attotree.py
--rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 attotree-0.1.3/attotree/increment_version.py
--rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-08 18:04:36.000000 attotree-0.1.3/attotree/version.py
-drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-08 18:11:08.561365 attotree-0.1.3/attotree.egg-info/
--rw-r--r--   0 karel      (503) staff       (20)     2650 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/PKG-INFO
--rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/SOURCES.txt
--rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/dependency_links.txt
--rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/entry_points.txt
--rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/requires.txt
--rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-08 18:11:08.000000 attotree-0.1.3/attotree.egg-info/top_level.txt
--rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-08 18:11:08.562623 attotree-0.1.3/setup.cfg
--rw-r--r--   0 karel      (503) staff       (20)     1351 2024-01-11 15:00:05.000000 attotree-0.1.3/setup.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-09 00:23:49.207808 attotree-0.1.4/
+-rw-r--r--   0 karel      (503) staff       (20)     1071 2024-01-15 14:46:06.000000 attotree-0.1.4/LICENSE.txt
+-rw-r--r--   0 karel      (503) staff       (20)     3432 2024-04-09 00:23:49.207043 attotree-0.1.4/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)     2854 2024-04-09 00:23:38.000000 attotree-0.1.4/README.rst
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-09 00:23:49.157568 attotree-0.1.4/attotree/
+-rw-r--r--   0 karel      (503) staff       (20)        0 2024-01-11 14:46:57.000000 attotree-0.1.4/attotree/__init__.py
+-rwxr-xr-x   0 karel      (503) staff       (20)    12873 2024-04-09 00:23:38.000000 attotree-0.1.4/attotree/attotree.py
+-rwxr-xr-x   0 karel      (503) staff       (20)      435 2024-01-11 14:46:57.000000 attotree-0.1.4/attotree/increment_version.py
+-rw-r--r--   0 karel      (503) staff       (20)       78 2024-04-09 00:23:38.000000 attotree-0.1.4/attotree/version.py
+drwxr-xr-x   0 karel      (503) staff       (20)        0 2024-04-09 00:23:49.205890 attotree-0.1.4/attotree.egg-info/
+-rw-r--r--   0 karel      (503) staff       (20)     3432 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/PKG-INFO
+-rw-r--r--   0 karel      (503) staff       (20)      317 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/SOURCES.txt
+-rw-r--r--   0 karel      (503) staff       (20)        1 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/dependency_links.txt
+-rw-r--r--   0 karel      (503) staff       (20)       52 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/entry_points.txt
+-rw-r--r--   0 karel      (503) staff       (20)        6 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/requires.txt
+-rw-r--r--   0 karel      (503) staff       (20)        9 2024-04-09 00:23:49.000000 attotree-0.1.4/attotree.egg-info/top_level.txt
+-rw-r--r--   0 karel      (503) staff       (20)       38 2024-04-09 00:23:49.207897 attotree-0.1.4/setup.cfg
+-rw-r--r--   0 karel      (503) staff       (20)     1351 2024-01-11 15:00:05.000000 attotree-0.1.4/setup.py
```

### Comparing `attotree-0.1.3/LICENSE.txt` & `attotree-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `attotree-0.1.3/PKG-INFO` & `attotree-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attotree
-Version: 0.1.3
+Version: 0.1.4
 Summary: description
 Home-page: https://github.com/karel-brinda/attotree
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,14 +15,27 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 Requires-Dist: wheel
 
 Attotree
 ========
 
+.. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
+    :target: https://github.com/karel-brinda/attotree
+.. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/attotree.svg
+    :target: https://github.com/karel-brinda/attotree/releases/
+.. |pypi-badge| image:: https://img.shields.io/pypi/v/attotree.svg
+    :target: https://pypi.org/project/attotree/
+.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
+    :target: https://doi.org/10.5281/zenodo.10945896
+.. |ci-tests-badge| image:: https://github.com/karel-brinda/attotree/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/karel-brinda/attotree/actions/
+
+|info-badge| |github-release-badge| |pypi-badge| |doi-badge| |ci-tests-badge|
+
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
 its output is identical to Mashtree,
@@ -68,17 +81,17 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
- 
+
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.3
+    Version: 0.1.4
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
     usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
```

### Comparing `attotree-0.1.3/README.rst` & `attotree-0.1.4/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Attotree
 ========
 
+.. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
+    :target: https://github.com/karel-brinda/attotree
+.. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/attotree.svg
+    :target: https://github.com/karel-brinda/attotree/releases/
+.. |pypi-badge| image:: https://img.shields.io/pypi/v/attotree.svg
+    :target: https://pypi.org/project/attotree/
+.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
+    :target: https://doi.org/10.5281/zenodo.10945896
+.. |ci-tests-badge| image:: https://github.com/karel-brinda/attotree/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/karel-brinda/attotree/actions/
+
+|info-badge| |github-release-badge| |pypi-badge| |doi-badge| |ci-tests-badge|
+
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
 its output is identical to Mashtree,
@@ -50,17 +63,17 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
- 
+
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.3
+    Version: 0.1.4
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
     usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
```

### Comparing `attotree-0.1.3/attotree/attotree.py` & `attotree-0.1.4/attotree/attotree.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 License: MIT
 """
 
 import argparse
 import datetime
 import os
 import re
+import shutil
 import subprocess
 import sys
 import tempfile
 import time
 
 sys.path.append(os.path.dirname(__file__))
 import version
@@ -226,15 +227,15 @@
         phylip_fn (str): The filename of the input phylip file.
         newick_fn (str): The filename of the output newick file.
         algorithm (str): The algorithm to use for tree construction. Valid options are "upgma" or "nj".
 
     Returns:
         None
     """
-    message("Running quicktree")
+    message("Running Quicktree")
 
     cmd = "quicktree -in m".split()
     if algorithm == "upgma":
         cmd += ["-upgma"]
     cmd += [phylip_fn]
     run_safe(cmd, output_fn=newick_fn, verbose=verbose)
 
@@ -291,36 +292,40 @@
     if debug:
         features.append("debuging")
     if len(features) > 0:
         fmsg = f" ({', '.join(features)})"
     else:
         fmsg = ""
     message(f"Attotree starting{fmsg}")
-    with tempfile.TemporaryDirectory(delete=not debug) as d:
-        message('Created a temporary directory', d)
-        phylip1_fn = os.path.join(d, "distances.phylip0")
-        phylip2_fn = os.path.join(d, "distances.phylip")
-        newick1_fn = os.path.join(d, "tree.nw")
-        newick2_fo = newick_fo
-        if fof:
-            #This is to make the list of file pass to Mash even with
-            #process substitutions
-            old_fof_fn = fns[0]
-            new_fof_fn = os.path.join(d, "fof.txt")
-            with open(old_fof_fn) as f, open(new_fof_fn, 'w') as g:
-                g.write(f.read())
-            fns = [new_fof_fn]
-        mash_triangle(fns, phylip1_fn, k=k, s=s, t=t, fof=fof, verbose=verbose)
-        postprocess_mash_phylip(phylip1_fn, phylip2_fn, verbose=verbose)
-        quicktree(phylip2_fn, newick1_fn, algorithm=phylogeny_algorithm, verbose=verbose)
-        postprocess_quicktree_nw(newick1_fn, newick2_fo, verbose=verbose)
+
+    d = tempfile.mkdtemp()
+
+    message('Creating a temporary directory', d)
+    phylip1_fn = os.path.join(d, "distances.phylip0")
+    phylip2_fn = os.path.join(d, "distances.phylip")
+    newick1_fn = os.path.join(d, "tree.nw")
+    newick2_fo = newick_fo
+    if fof:
+        #This is to make the list of file pass to Mash even with
+        #process substitutions
+        old_fof_fn = fns[0]
+        new_fof_fn = os.path.join(d, "fof.txt")
+        with open(old_fof_fn) as f, open(new_fof_fn, 'w') as g:
+            g.write(f.read())
+        fns = [new_fof_fn]
+    mash_triangle(fns, phylip1_fn, k=k, s=s, t=t, fof=fof, verbose=verbose)
+    postprocess_mash_phylip(phylip1_fn, phylip2_fn, verbose=verbose)
+    quicktree(phylip2_fn, newick1_fn, algorithm=phylogeny_algorithm, verbose=verbose)
+    postprocess_quicktree_nw(newick1_fn, newick2_fo, verbose=verbose)
 
     if debug:
         emsg = f" (auxiliary files retained in '{d}')"
     else:
+        shutil.rmtree(d)
+        message('Deleting the temporary directory', d)
         emsg = ""
     message(f"Attotree finished{emsg}")
 
 
 def main():
     """
     The main function that is executed when the script is run.
```

### Comparing `attotree-0.1.3/attotree.egg-info/PKG-INFO` & `attotree-0.1.4/attotree.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attotree
-Version: 0.1.3
+Version: 0.1.4
 Summary: description
 Home-page: https://github.com/karel-brinda/attotree
 Author: Karel Brinda
 Author-email: karel.brinda@inria.fr
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,14 +15,27 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 Requires-Dist: wheel
 
 Attotree
 ========
 
+.. |info-badge| image:: https://img.shields.io/badge/Project-Info-blue
+    :target: https://github.com/karel-brinda/attotree
+.. |github-release-badge| image:: https://img.shields.io/github/release/karel-brinda/attotree.svg
+    :target: https://github.com/karel-brinda/attotree/releases/
+.. |pypi-badge| image:: https://img.shields.io/pypi/v/attotree.svg
+    :target: https://pypi.org/project/attotree/
+.. |doi-badge| image:: https://zenodo.org/badge/DOI/110.5281/zenodo.10945896.svg
+    :target: https://doi.org/10.5281/zenodo.10945896
+.. |ci-tests-badge| image:: https://github.com/karel-brinda/attotree/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/karel-brinda/attotree/actions/
+
+|info-badge| |github-release-badge| |pypi-badge| |doi-badge| |ci-tests-badge|
+
 
 Introduction
 ------------
 
 Rapid estimation of phylogenetic trees directly from FASTA files in the style of
 `Mashtree <https://github.com/lskatz/mashtree>`_. With the default options,
 its output is identical to Mashtree,
@@ -68,17 +81,17 @@
 Command-line parameters
 -----------------------
 
 
 .. code-block::
 
     $ attotree -h
- 
+
     Program: attotree (rapid estimation of phylogenetic trees using sketching)
-    Version: 0.1.3
+    Version: 0.1.4
     Author:  Karel Brinda <karel.brinda@inria.fr>
 
     usage: attotree [-k INT] [-s INT] [-t INT] [-o FILE] [-f STR] [-L] [-D] [-V] genomes [genomes ...]
 
     positional arguments:
       genomes     input genome file (fasta / gzipped fasta / list of files when "-L")
```

### Comparing `attotree-0.1.3/setup.py` & `attotree-0.1.4/setup.py`

 * *Files identical despite different names*

