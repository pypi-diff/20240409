# Comparing `tmp/kmerdb-0.7.8.tar.gz` & `tmp/kmerdb-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerdb-0.7.8.tar", last modified: Thu Mar 28 19:31:30 2024, max compression
+gzip compressed data, was "kmerdb-0.7.9.tar", last modified: Tue Apr  9 19:42:40 2024, max compression
```

## Comparing `kmerdb-0.7.8.tar` & `kmerdb-0.7.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-28 19:31:30.627722 kmerdb-0.7.8/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.7.8/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.7.8/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)    25333 2024-03-28 19:31:30.631722 kmerdb-0.7.8/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    10629 2024-03-21 22:18:34.000000 kmerdb-0.7.8/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-28 19:31:30.627722 kmerdb-0.7.8/kmerdb/
--rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.7.8/kmerdb/CITATION.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)    97576 2024-03-28 19:10:10.000000 kmerdb-0.7.8/kmerdb/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.7.8/kmerdb/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    13901 2024-03-23 14:51:45.000000 kmerdb-0.7.8/kmerdb/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)  1164381 2024-03-28 19:10:22.000000 kmerdb-0.7.8/kmerdb/distance.c
--rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.7.8/kmerdb/distance.pyx
--rw-rw-r--   0 matt      (1000) matt      (1000)    42768 2024-03-25 19:01:09.000000 kmerdb-0.7.8/kmerdb/fileutil.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    51371 2024-03-28 17:29:15.000000 kmerdb-0.7.8/kmerdb/graph.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.7.8/kmerdb/index.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22573 2024-03-25 20:35:53.000000 kmerdb-0.7.8/kmerdb/kmer.py
--rw-r-----   0 matt      (1000) matt      (1000)    20826 2024-03-25 22:53:30.000000 kmerdb-0.7.8/kmerdb/parse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.7.8/kmerdb/probability.py
--rw-r-----   0 matt      (1000) matt      (1000)     5235 2022-05-01 17:20:48.000000 kmerdb-0.7.8/kmerdb/python_distances.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-03-21 01:07:55.000000 kmerdb-0.7.8/kmerdb/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-28 19:31:30.627722 kmerdb-0.7.8/kmerdb.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    25333 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      555 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-03-09 18:02:00.000000 kmerdb-0.7.8/kmerdb.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      390 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-03-28 19:31:30.000000 kmerdb-0.7.8/kmerdb.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     5415 2024-03-12 03:17:09.000000 kmerdb-0.7.8/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-03-28 19:31:30.631722 kmerdb-0.7.8/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     6355 2024-03-12 03:17:09.000000 kmerdb-0.7.8/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-03-28 19:31:30.627722 kmerdb-0.7.8/test/
--rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.7.8/test/test_kmer.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.7.9/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.7.9/MANIFEST.in
+-rw-r--r--   0 matt      (1000) matt      (1000)    26600 2024-04-09 19:42:40.389017 kmerdb-0.7.9/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    10606 2024-04-06 05:32:04.000000 kmerdb-0.7.9/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/kmerdb/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.7.9/kmerdb/CITATION.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)    95832 2024-04-09 19:12:35.000000 kmerdb-0.7.9/kmerdb/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.7.9/kmerdb/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    27137 2024-04-09 19:14:01.000000 kmerdb-0.7.9/kmerdb/appmap.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.7.9/kmerdb/banners.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    15992 2024-04-09 17:09:24.000000 kmerdb-0.7.9/kmerdb/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)  1166079 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb/distance.c
+-rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.7.9/kmerdb/distance.pyx
+-rw-rw-r--   0 matt      (1000) matt      (1000)    42776 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/fileutil.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    51253 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/graph.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.7.9/kmerdb/index.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22573 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/kmer.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.7.9/kmerdb/legacy.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    19206 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/parse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.7.9/kmerdb/probability.py
+-rw-r-----   0 matt      (1000) matt      (1000)     5235 2022-05-01 17:20:48.000000 kmerdb-0.7.9/kmerdb/python_distances.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.7.9/kmerdb/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/kmerdb.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    26600 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      607 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      287 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-04-09 19:42:40.000000 kmerdb-0.7.9/kmerdb.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4592 2024-04-09 19:42:27.000000 kmerdb-0.7.9/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-04-09 19:42:40.389017 kmerdb-0.7.9/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-04-09 17:08:02.000000 kmerdb-0.7.9/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-09 19:42:40.389017 kmerdb-0.7.9/test/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.7.9/test/test_kmer.py
```

### Comparing `kmerdb-0.7.8/LICENSE.txt` & `kmerdb-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/PKG-INFO` & `kmerdb-0.7.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.7.8
-Summary: Yet another kmer library for Python
+Version: 0.7.9
+Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.0.tar.gz
-Author: Matthew Ralston
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
+Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -207,38 +207,69 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://matthewralston.github.io/kmerdb
 Project-URL: QuickStart, https://matthewralston.github.io/kmerdb/quickstart.html
-Project-URL: Install, https://matthewralston.github.io/kmerdb/installation.html
-Project-URL: ForAcademics, https://matthewralston.github.io/kmerdb/academics.html
 Project-URL: Github, https://github.com/MatthewRalston/kmerdb
 Project-URL: Issues, https://github.com/MatthewRalston/kmerdb/issues
-Keywords: bioinformatics,fastq,fasta,k-mer,kmer,k-merdb,kmerdb,kdb
+Keywords: bioinformatics,fastq,fasta,k-mer,kmer
 Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 7 - Inactive
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: PalmOS
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8.0
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: Free For Educational Use
+Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Topic :: File Formats
+Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Topic :: Text Processing :: Indexing
+Classifier: Topic :: Text Processing
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.7.4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: psutil>=4.2.0
+Requires-Dist: Cython>=3.0.8
+Requires-Dist: biopython>=1.81
+Requires-Dist: scipy>=1.11.4
+Requires-Dist: scikit-learn==1.2.2
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: setuptools>=69.2.0
+Provides-Extra: dev
+Requires-Dist: auditwheel>=5.1.2; extra == "dev"
+Requires-Dist: build>=0.9.0; extra == "dev"
+Requires-Dist: coverage>=4.5.4; extra == "dev"
+Requires-Dist: expects>=0.9.0; extra == "dev"
+Requires-Dist: docutils>=0.17; extra == "dev"
+Requires-Dist: sphinx>=4.3.2; extra == "dev"
+Requires-Dist: pytest>=5.3.5; extra == "dev"
+Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
 > A Python CLI and module for k-mer profiles, similarities, and graph databases
 
 NOTE: This project is in beta stage. Development is ongoing. But feel free to clone the repository and play with the code for yourself.
 
 ## Development Status
@@ -283,24 +314,24 @@
 
 All other dependencies are managed directly by pip. 
 
 
 ### OSX and Linux release:
 
 ```sh
-pip install kmerdb
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
 
 ### Development installation:
 
 ```sh
 git clone https://github.com/MatthewRalston/kmerdb.git
-pip install -e .
+pip install .
 ```
 
 ## Usage Example
 
 NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
 
 <!-- ## NOTE: Temporary usage pattern:
@@ -382,15 +413,15 @@
 python setup.py test
 ```
 
 ## License
 
 Created by Matthew Ralston - [Scientist, Programmer, Musician](http://matthewralston.github.io) - [Email](mailto:mralston.development@gmail.com)
 
-Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, but we march into the information age with this ethos. I have the patent rights to this software. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
+Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, and im the author and maintainer. cheers, on me. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
 
 ```
    Copyright 2020 Matthew Ralston
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
```

### Comparing `kmerdb-0.7.8/README.md` & `kmerdb-0.7.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,24 @@
 
 All other dependencies are managed directly by pip. 
 
 
 ### OSX and Linux release:
 
 ```sh
-pip install kmerdb
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
 
 ### Development installation:
 
 ```sh
 git clone https://github.com/MatthewRalston/kmerdb.git
-pip install -e .
+pip install .
 ```
 
 ## Usage Example
 
 NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
 
 <!-- ## NOTE: Temporary usage pattern:
@@ -144,15 +144,15 @@
 python setup.py test
 ```
 
 ## License
 
 Created by Matthew Ralston - [Scientist, Programmer, Musician](http://matthewralston.github.io) - [Email](mailto:mralston.development@gmail.com)
 
-Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, but we march into the information age with this ethos. I have the patent rights to this software. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
+Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, and im the author and maintainer. cheers, on me. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
 
 ```
    Copyright 2020 Matthew Ralston
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
```

### Comparing `kmerdb-0.7.8/kmerdb/__init__.py` & `kmerdb-0.7.9/kmerdb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,25 +36,24 @@
 logger = None
 
 
 def print_argv():
     argv = sys.argv
     sys.stderr.write(" ".join(argv[0:4]) + " ...\n")
 
-def citation(arguments):
-    import pkg_resources
-    citation = None
-    if pkg_resources.resource_exists('kmerdb', 'CITATION.txt'):
-        citation_fname = pkg_resources.resource_filename('kmerdb', 'CITATION.txt')
-        with open(citation_fname, 'w') as citation_file:
-            citation_file.write("")
+def citation():
 
+    MODULE_ROOT = os.path.dirname(__file__)
+    citation_file = os.path.join(MODULE_ROOT,  'CITATION.txt')
+    if os.access(citation_file, os.R_OK):
+        with open(citation_file, 'w') as cit_file:
+            cit_file.write("")
 
     sys.stderr.write("On the real, we gotta eat.")
-    sys.stderr.write("Consider a +1 to keep it real...")
+    sys.stderr.write("Consider a +1 on Github to keep it real...")
 
 def index_file(arguments):
     from kmerdb import fileutil, index
     from kmerdb.config import DONE
     
     with fileutil.open(arguments.kdb, mode='r') as kdb:
         k = kdb.metadata['k']
@@ -82,67 +81,103 @@
                     x = 1
                     for i in shuffled:
                         kmer_id, count, kmer_metadata = index.read_line(kdb, kdbi, i)
                         kdb_out.write("{0}\t{1}\t{2}".format(x, count, kmer_metadata))
                         x += 1
     sys.stderr.write(DONE)
     
-def markov_probability(arguments):
-    """
-    A very old function that is probably broken in the indexing function.
-    
-    :param arguments: argparse Namespace
-    :type arguments:
-    """
-    import pandas as pd
-    import numpy as np
-    from kmerdb import fileutil, index, probability, parse
-    from kmerdb.config import DONE
+# def markov_probability(arguments):
+#     """
+#     A very old function that is probably broken in the indexing function.
+    
+#     :param arguments: argparse Namespace
+#     :type arguments:
+#     """
+#     import pandas as pd
+#     import numpy as np
+#     from kmerdb import fileutil, index, probability, parse
+#     from kmerdb.config import DONE
 
-    if os.path.splitext(arguments.kdb)[-1] != ".kdb":
-        raise IOError("Model .kdb filepath does not end in '.kdb'")
+#     if os.path.splitext(arguments.kdb)[-1] != ".kdb":
+#         raise IOError("Model .kdb filepath does not end in '.kdb'")
 
 
-    if index.has_index(arguments.kdb):
-        arguments.kdbi = arguments.kdb + "i"
-        #df = pd.DataFrame([], columns=["SequenceID", "Log_Odds_ratio", "p_of_seq"])
-        profiles = np.array([], dtype="int64")
-        with fileutil.open(arguments.kdb, 'r', slurp=True) as kdb:
-            k = kdb.metadata['k']
-            with index.open(arguments.kdbi, 'r') as kdbi:
-                with parse.SeqParser(arguments.seqfile, arguments.fastq_block_size, k) as seqprsr:
-                    recs = [r for r in seqprsr]
-                    if seqprsr.fastq:
-                        logger.debug("Read exactly b=={0}=={1} records from the {2} seqparser object".format(b, len(recs), s))
-                        assert len(recs) == b, "The seqparser should return exactly {0} records at a time".format(b)
-                    else:
-                        logger.debug("Read {0} sequences from the {1} seqparser object".format(len(recs), seqprsr))
-                        logger.debug("Skipping the block size assertion for fasta files")
+#     if index.has_index(arguments.kdb):
+#         arguments.kdbi = arguments.kdb + "i"
+#         #df = pd.DataFrame([], columns=["SequenceID", "Log_Odds_ratio", "p_of_seq"])
+#         profiles = np.array([], dtype="int64")
+#         with fileutil.open(arguments.kdb, 'r', slurp=True) as kdb:
+#             k = kdb.metadata['k']
+#             with index.open(arguments.kdbi, 'r') as kdbi:
+#                 with parse.SeqParser(arguments.seqfile, arguments.fastq_block_size, k) as seqprsr:
+#                     recs = [r for r in seqprsr]
+#                     if seqprsr.fastq:
+#                         logger.debug("Read exactly b=={0}=={1} records from the {2} seqparser object".format(b, len(recs), s))
+#                         assert len(recs) == b, "The seqparser should return exactly {0} records at a time".format(b)
+#                     else:
+#                         logger.debug("Read {0} sequences from the {1} seqparser object".format(len(recs), seqprsr))
+#                         logger.debug("Skipping the block size assertion for fasta files")
 
-                    while len(recs): # While the seqprsr continues to produce blocks of reads
-                        # Do something here
+#                     while len(recs): # While the seqprsr continues to produce blocks of reads
+#                         # Do something here
                     
-                        markov_probs = list(map(lambda p: [p["seq"].name, p["log_odds_ratio"], p["p_of_seq"]], [probability.markov_probability(seq, kdb, kdbi) for seq in recs]))
+#                         markov_probs = list(map(lambda p: [p["seq"].name, p["log_odds_ratio"], p["p_of_seq"]], [probability.markov_probability(seq, kdb, kdbi) for seq in recs]))
+
+#                         sys.stderr.write(json.dumps(markov_probs))
+#                         if profiles.shape == (0,):
+#                             profiles = np.array(markov_probs)
+#                         else:
+#                             np.append(profiles, markov_probs, axis=0)
+
+#                         recs = [r for r in seqprsr] # Essentially accomplishes an iteration in the file, wrapped by the parse.SeqParser class
+#         df = pd.DataFrame(profiles, columns=["SequenceID", "Log_Odds_ratio", "p_of_seq"])
+#         df.to_csv(sys.stdout, sep=arguments.delimiter, index=False)
+
+#     else:
+#         raise IndexError(".kdb file '{0}' has no corresponding index file. Please run 'kdb index -h' for details on index generation".format(arguments.kdb))
+
+    
+#     sys.stderr.write(DONE)
 
-                        sys.stderr.write(json.dumps(markov_probs))
-                        if profiles.shape == (0,):
-                            profiles = np.array(markov_probs)
-                        else:
-                            np.append(profiles, markov_probs, axis=0)
 
-                        recs = [r for r in seqprsr] # Essentially accomplishes an iteration in the file, wrapped by the parse.SeqParser class
-        df = pd.DataFrame(profiles, columns=["SequenceID", "Log_Odds_ratio", "p_of_seq"])
-        df.to_csv(sys.stdout, sep=arguments.delimiter, index=False)
 
-    else:
-        raise IndexError(".kdb file '{0}' has no corresponding index file. Please run 'kdb index -h' for details on index generation".format(arguments.kdb))
 
+
+
+def expanded_help(arguments):
+
+    import sys
     
-    sys.stderr.write(DONE)
-                    
+    argv = sys.argv
+    
+    from kmerdb import config, appmap
+
+    kmerdb_appmap = appmap.kmerdb_appmap( argv )
+
+    #kmerdb_appmap.print_program_header()
+    
+    if arguments.method not in config.subcommands:
+        raise ValueError("unsupported method")
+    elif arguments.method == "profile":
+        kmerdb_appmap.print_profile_header()
+    elif arguments.method == "graph":
+        kmerdb_appmap.print_graph_header()
+    elif arguments.method == "index":
+        #kmerdb_appmap.print_index_header()
+        raise ValueError("Unsupported method")
+    elif arguments.method == "shuf":
+        #kmerdb_appmap.print_shuf_header()
+        raise ValueError("Unsupported method")
+    elif arguments.method == "matrix":
+        kmerdb_appmap.print_matrix_header()
+    elif arguments.method == "distance":
+        kmerdb_appmap.print_distance_header()
+
+
+
 def distances(arguments):
     """
     An end-user function to provide CLI access to certain distances
     """
     from multiprocessing import Pool
     import multiprocessing as mp
 
@@ -294,19 +329,14 @@
                             p = mp.Process(target=pearson_correlation, args=(profiles[i], profiles[j], profiles[i].size, r))
                             p.start()
                             #data[i][j] = correlation(profiles[i], profiles[j], profiles[i].size)
                             p.join()
                             data[i][j] = r.value
                         else:
                             raise RuntimeError("Cannot calculate pearson correlation without NumPy and Cython")
-                    elif arguments.metric == "euclidean":
-                        logger.error("Custom Euclidean distance is DEPRECATED")
-                        raise RuntimeError("Genuine bug, please report the usage of deprecated custom distance functions")
-                        logger.info("Computing custom euclidean distance")
-                        data[i][j] = distance.euclidean(profiles[i], profiles[j])
                     elif arguments.metric == "spearman":
                         cor, pval = distance.spearman(profiles[i], profiles[j])
                         logger.info("Computing SciPy Spearman distance")
                         # FIXME! also print pval matrices
                         data[i][j] = cor
                     elif arguments.metric == "EMD":
                         logger.error("Custom EMD distance is deprecated")
@@ -545,17 +575,18 @@
         # logger.debug("final_df should be set as normalized")
         # sys.exit(1)
         final_df = normalized
     elif arguments.method == "pass":
         #df.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
         final_df = df
     elif arguments.method == "Frequency":
-        k = suggested_metadata['k']
-        total_kmers = suggested_metadata["total_kmers"]
-        final_df = df.div(total_kmers)
+        final_df = df # 4/5/24 - frequencies are given in the standard format
+        #k = suggested_metadata['k']
+        #total_kmers = suggested_metadata["total_kmers"]
+        #final_df = df.div(total_kmers)
     elif arguments.method == "PCA":
         # This method is actually dimensionality reduction via SVD, and this process is used during principal components analysis.
         # We generate the elbow graph in this step if the required dimensionality parameter '-n' is not supplied.
         # In this case we assume they have not provided the parameter because they'd like to use the so-called 'auto-detection'
         
         # I've specified a feature called 'auto-detect' such that the elbow graph is produced
         # they supply the number of dimensions they'd like after viewing the graph,
@@ -577,18 +608,21 @@
         plt.ylabel("Cumulative explained variance")
         plt.savefig(config.pca_variance_fig_filepath)
 
         if arguments.n is not None:
             logger.info("Using selected PCA dimensionality to reduce the transpose matrix/DataFrame again for use in 'kdb kmeans'")
             pca = PCA(n_components=arguments.n)
             pca.fit(np.transpose(df))
-            #logger.debug("Explained variances: {0}".format(pca.explained_variance_ratio_))
-            #logger.debug("Log-likelihoods: {0}".format(pca.score_samples(normalized)))
-            #logger.debug("Overall log-likelihood of all samples: {0}".format(pca.score(normalized)))
-            #logger.debug("MLE estimate of components for dimensionality reduction produced this shape: {0}".format(pca.components_.shape))
+            sys.stderr.write("\n\n\n")
+            sys.stderr.write("-"*30)
+            
+            sys.stderr.write("Explained variances: {0}\n".format(pca.explained_variance_ratio_))
+            sys.stderr.write("Log-likelihoods: {0}\n".format(pca.score_samples(normalized)))
+            sys.stderr.write("Log-likelihood of all samples: {0}\n".format(pca.score(normalized)))
+            sys.stderr.write("MLE estimate of components for dimensionality reduction produced this shape: {0}\n".format(pca.components_.shape))
 
             score_matrix = pca.transform(np.transpose(df))
             score_df = pd.DataFrame(np.transpose(score_matrix), columns=columns)
 
             #score_df.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
             final_df = score_df
         else:
@@ -1242,14 +1276,29 @@
     if arguments.parallel > 1:
         with Pool(processes=arguments.parallel) as pool:
             # data files_metadata
             data = pool.map(infile.parsefile, arguments.seqfile) # Returns a list of k-mer ids
     else:
             # data files_metadata
             data = list(map(infile.parsefile, arguments.seqfile))
+
+
+
+    """
+    ######################################
+    Step 1. Completed
+    ######################################
+    """
+
+
+
+
+
+
+            
     """
     Summary statistics and metadata structure
     """
 
     nullomer_ids = []
     counts = []
     for d in data:
@@ -1311,47 +1360,68 @@
 
 
 
     """
     ACCUMULATE ALL EDGE WEIGHTS ACROSS ALL FILES
     """
     """
-    Step 1: initialize the final edge datastructure, a hashmap, keyed on a pair of k-mer ids, and containing only an integer weight
+    task 1: initialize the final edge datastructure, a hashmap, keyed on a pair of k-mer ids, and containing only an integer weight
     """
     # Initialize empty data structures
     all_edges_in_kspace = {}
     n1 = []
     n2 = []
     weights = []
     # Loop over the input files and initialize the dictionary on the valid pairs, setting them to 0.
     for d in data:
         edges, h, counts, nullomers = d
         pair_ids = edges.keys()
         for p in pair_ids:
             all_edges_in_kspace[p] = 0
     """
-    Step 2: Accumulate all edge weights across all files
+    task 2: Accumulate all edge weights across all files
     """
     for d in data:
         edges, h, counts, nullomers = d
         pair_ids = edges.keys()
         
         for p in pair_ids:
             try:
                 all_edges_in_kspace[p] += edges[p]
             except KeyError as e:
                 logger.error("Unknown edge detected, evaded prepopulation. Internal error.")
                 raise e
     """
-    Step 3: Add edges (2 k-mer ids) and weight to lists for conversion to NumPy array.
+    task 3: Add edges (2 k-mer ids) and weight to lists for conversion to NumPy array.
     """
     for e in all_edges_in_kspace.keys():
         n1.append(e[0])
         n2.append(e[1])
         weights.append(all_edges_in_kspace[e])
+
+
+    """
+    #################################################
+    Step 2. Completed
+    #################################################
+    """
+
+
+
+
+
+
+
+
+
+
+
+
+
+        
     """
     N would be the number of edges, pairs of nodes, and weights.
     """
     N = len(n1)
     
     logger.debug("Initializing Numpy arrays of {0} uint for the edges and corresponding weight...".format(N))
     n1 = np.array(n1, dtype=metadata["n1_dtype"])
@@ -1493,26 +1563,22 @@
         data = list(map(infile.parsefile, arguments.seqfile))
 
     # 'data' is now a list of 4-tuples
     # Each 4-tuple represents a single file
     # (edges, header_dictionary<dict>, nullomers<list>, all_kmer_metadata<list>)
 
     # Construct a final_counts array for the composite profile across all inputs
-    logger.debug("Initializing large list for extended metadata")
-    all_kmer_metadata = list([] for x in range(total_kmers)) if arguments.all_metadata else None
-    logger.debug("Allocation completed")
+
+
     counts = np.zeros(N, dtype="uint64")
     # Complete collating of counts across files
     # This technically uses 1 more arrray than necessary 'final_counts' but its okay
     logger.info("Summing counts from individual fasta/fastq files into a composite profile...")
     for d in data:
         counts = counts + d[0]
-        if arguments.all_metadata:
-            logger.info("\n\nMerging metadata from all files...\n\n")
-            all_kmer_metadata = util.merge_metadata_lists(arguments.k, all_kmer_metadata, d[3])
 
     sys.stderr.write("\n\n\tCompleted summation and metadata aggregation across all inputs...\n\n")
     # unique_kmers = int(np.count_nonzero(counts))
     # #total_nullomers = total_kmers - unique_kmers
 
     # nullomer_ids = list(map(lambda n: n[2], data))
     # all_observed_kmers = int(np.sum(list(map(lambda h: h['total_kmers'], file_metadata))))
@@ -1566,15 +1632,15 @@
     metadata=OrderedDict({
         "version": VERSION,
         "metadata_blocks": 1,
         "k": arguments.k,
         "total_kmers": all_observed_kmers,
         "unique_kmers": unique_kmers,
         "unique_nullomers": unique_nullomers,
-        "metadata": arguments.all_metadata,
+        "metadata": False,
         "sorted": arguments.sorted,
         "kmer_ids_dtype": "uint64",
         "profile_dtype": "uint64",
         "count_dtype": "uint64",
         "frequencies_dtype": "float64",
         "tags": [],
         "files": file_metadata
@@ -1609,106 +1675,43 @@
 
 
         # Numpy indexing is trash
         #kmer_ids = np.zeros(total_kmers, dtype=metadata["kmer_ids_dtype"])
         #profile = np.zeros(total_kmers, dtype=metadata["profile_dtype"])
         #counts = np.zeros(total_kmers, dtype=metadata["count_dtype"])
         #frequencies = np.zeros(total_kmers, dtype=metadata["frequencies_dtype"])
-        all_metadata = []
-        if arguments.all_metadata:
-
-            if arguments.sorted is True:
-                j = 0
-                list_of_duples = list(zip(kmer_ids, counts))
-                logger.debug(list_of_duples[0:3])
-                kmer_ids_sorted_by_count = np.lexsort(list_of_duples)
-                reverse_kmer_ids_sorted_by_count = np.flipud(kmer_ids_sorted_by_count)
-                for i, idx in enumerate(reverse_kmer_ids_sorted_by_count):
-                    seq = kmer.id_to_kmer(idx, arguments.k)
-                    kmer_id = int(idx)
-
-                    
-                    kmer_metadata = kmer.neighbors(seq, kmer_id, arguments.k) # metadata is initialized by the neighbors
-                    reads = []
-                    starts = []
-                    reverses = []
-                    frequency = float(count)/N
-                    for read, start, reverse in all_kmer_metadata[idx]:
-                        reads.append(read)
-                        starts.append(start)
-                        reverses.append(reverse)
-                        kmer_metadata["reads"] = reads
-                        kmer_metadata["starts"] = starts
-                        kmer_metadata["reverses"] = reverses
-                    counts[idx] = counts[idx]
-                    frequencies[idx] = frequencies[idx]
-                    all_metadata.append(kmer_metadata)
-                    assert j <= i + 1, "profile | row index was not sequential. Possibly read improperly."
-                    assert idx == kmer_ids[i], "profile | row index did not match a kmer_id"
-                    logger.info("First is the implicit row index, next is a k-mer id, next is the corresponding k-mer id to the row-index (may not match from sorting), next is the count and frequencies")
-                    if arguments.quiet is not True:
-                        print("{0}\t{1}\t{2}\t{3}".format(i, kmer_ids[idx], counts[idx], frequencies[idx]))
-                    kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_ids[idx], counts[idx], frequencies[idx], json.dumps(kmer_metadata)))
-                    j += 1
-            else:
-                j = 0
-                for i, idx in enumerate(kmer_ids):
-                    seq = kmer.id_to_kmer(kmer_id, arguments.k)
-                    kmer_id = int(idx)
-
-                    kmer_metadata = kmer.neighbors(seq, kmer_id, arguments.k)
-                    #logger.info("{0}\t{1}\t{2}\t{3}\t{4}".format(i, idx, kmer_ids[i], counts[kmer_id], frequencies[kmer_id]))
-                    
+        if arguments.sorted:
 
-                    all_metadata.append(kmer_metadata)
-                    c = counts[idx]
-                    f = frequencies[idx]
-                    logger.info("First is the implicit row index, next is a k-mer id, next is the corresponding k-mer id to the row-index (may not match from sorting), next is the count and frequencies")
-                    if arguments.quiet is not True:
-                        print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
-                    kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_id, c, f, json.dumps(kmer_metadata)))
-                    j += 1
+            kmer_ids_sorted_by_count = np.lexsort(duple_of_arrays)
+            reverse_kmer_ids_sorted_by_count = list(kmer_ids_sorted_by_count)
+            reverse_kmer_ids_sorted_by_count.reverse()
+            logger.debug("K-mer id sort example: {0}".format(reverse_kmer_ids_sorted_by_count[:30]))
+            for i, idx in enumerate(reverse_kmer_ids_sorted_by_count):
+
+                kmer_id = int(kmer_ids[idx])
+                seq = kmer.id_to_kmer(kmer_id, arguments.k)
+                logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_ids[idx], counts[idx], frequencies[idx]))
+                c[idx] = counts[idx]
+                f[idx] = frequencies[idx]
+                if arguments.quiet is not True:
+                    print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
+                kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_id, c, f))
         else:
-            if arguments.sorted:
-
-                kmer_ids_sorted_by_count = np.lexsort(duple_of_arrays)
-                reverse_kmer_ids_sorted_by_count = list(kmer_ids_sorted_by_count)
-                logger.info("FIXME before reverse : ", reverse_kmer_ids_sorted_by_count)
-                reverse_kmer_ids_sorted_by_count.reverse()
-                logger.info("FIXME after reverse : ", reverse_kmer_ids_sorted_by_count)
-                logger.debug("K-mer id sort shape: {0}".format(len(kmer_ids_sorted_by_count)))
-                for i, idx in enumerate(reverse_kmer_ids_sorted_by_count):
-
-                    kmer_id = int(kmer_ids[idx])
-                    seq = kmer.id_to_kmer(kmer_id, arguments.k)
-                    kmer_metadata = kmer.neighbors(seq, kmer_id, arguments.k)
-
-                    logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_ids[idx], counts[idx], frequencies[idx]))
-                    all_metadata.append(kmer_metadata)
-                    c[idx] = counts[idx]
-                    f[idx] = frequencies[idx]
-                    if arguments.quiet is not True:
-                        print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
-                    kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_id, c, f, json.dumps(kmer_metadata)))
-            else:
-                for i, idx in enumerate(kmer_ids):
-
-
-                    kmer_id = int(kmer_ids[idx])
-                    seq = kmer.id_to_kmer(kmer_id, arguments.k)
-                    c = counts[idx]
-                    f = frequencies[idx]
+            for i, idx in enumerate(kmer_ids):
 
-                    kmer_metadata = kmer.neighbors(seq, kmer_id, arguments.k) # metadata is initialized by the neighbors
-                    logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
 
-                    all_metadata.append(kmer_metadata)
-                    if arguments.quiet is not True:
-                        print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
-                    kdb_out.write("{0}\t{1}\t{2}\t{3}\t{4}\n".format(i, kmer_id, c, f, json.dumps(kmer_metadata)))
+                kmer_id = int(kmer_ids[idx])
+                seq = kmer.id_to_kmer(kmer_id, arguments.k)
+                c = counts[idx]
+                f = frequencies[idx]
+
+                logger.info("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
+                if arguments.quiet is not True:
+                    print("{0}\t{1}\t{2}\t{3}".format(i, kmer_id, c, f))
+                kdb_out.write("{0}\t{1}\t{2}\t{3}\n".format(i, kmer_id, c, f))
         logger.info("Wrote 4^k = {0} k-mer counts + neighbors to the .kdb file.".format(total_kmers))
 
         logger.info("Done")
             
     finally:
         kdb_out._write_block(kdb_out._buffer)
         kdb_out._handle.flush()
@@ -1741,110 +1744,150 @@
         if ('boto' in name) or ('urllib3' in name) or ('s3' in name) or ('findfont' in name):
             logging.getLogger(name).setLevel(logging.WARNING)
 
     return root_logger
 
 
 def citation_info():
-    import pkg_resources
     citation = None
-    if pkg_resources.resource_exists('kmerdb', 'CITATION.txt'):
-        citation = pkg_resources.resource_string('kmerdb', 'CITATION.txt').decode('utf-8').rstrip()
+
+    MODULE_ROOT = os.path.dirname(__file__)
+    citation_file = os.path.join(MODULE_ROOT,  'CITATION.txt')
+    if os.access(citation_file, os.R_OK):
+        with open(citation_file, 'r') as citation_f:
+            citation = citation_f.read().rstrip()
+
         if citation == "":
             return
         else:
             sys.stderr.write("Printing citation notice to stderr. This will not interfere with the execution of the program in any way. Please see CITATION_FAQ.md for any questions.\n")
             sys.stderr.write(citation + "\n\n\n")
             sys.stderr.write("Run 'kmerdb citation' to silence.\n")
     else:
         raise IOError("Cannot locate the extra package data file 'kmerdb/CITATION', which should have been distributed with the program")
 
 
+def get_program_header(arguments):
+    import appmap.py
+    import sys
+
+
+    argv = sys.argv
+
+    kmerdb_appmap = appmap.kmerdb_appmap( argv )
+
+
+    kmerdb_appmap.print_program_header()
+
+
+    return kmerdb_appmap
+
 def cli():
+
+    import sys
+
+
+    
+    argv = sys.argv
+
+    
     sys.stderr.write("Running kdb script from '{0}'\n".format(__file__))
     sys.stderr.write("Checking installed environment...\n")
     primary_path = sys.path[0]
     ver_info = sys.version_info
     py_version = "python{0}.{1}".format(ver_info.major, ver_info.minor)
     #sys.path.append(os.path.join(primary_path, "../lib/{0}/site-packages".format(py_version)))
     #sys.path.append(os.path.join(os.path.dirname(__file__), "../lib"))
     #site_packages = [p for p in sys.path if "kdb" in p]
     
     #sys.stderr.write("PYTHONPATH={0}".format(sys.path))
     #sys.path.remove(os.path.dirname(os.path.abspath(__file__)))
     citation_info()
 
+
     
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(help="Use --help with sub-commands")
 
 
     profile_parser = subparsers.add_parser("profile", help="Parse data into the database from one or more sequence files")
     profile_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     profile_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)")
 
     profile_parser.add_argument("-p", "--parallel", type=int, default=1, help="Shred k-mers from reads in parallel")
 
-    profile_parser.add_argument("--batch-size", type=int, default=100000, help="Number of updates to issue per batch to PostgreSQL while counting")
-    profile_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
-    profile_parser.add_argument("-n", type=int, default=1000, help="Number of k-mer metadata records to keep in memory at once before transactions are submitted, this is a space limitation parameter after the initial block of reads is parsed. And during on-disk database generation")
-    #profile_parser.add_argument("--keep-S3-file", action="store_true", help="Download S3 file to the current working directory")
+    # profile_parser.add_argument("--batch-size", type=int, default=100000, help="Number of updates to issue per batch to PostgreSQL while counting")
+    # profile_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
+    #profile_parser.add_argument("-n", type=int, default=1000, help="Number of k-mer metadata records to keep in memory at once before transactions are submitted, this is a space limitation parameter after the initial block of reads is parsed. And during on-disk database generation")
+
     profile_parser.add_argument("--keep-db", action="store_true", help=argparse.SUPPRESS)
-    profile_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
-    profile_parser.add_argument("--all-metadata", action="store_true", default=False, help="Include read-level k-mer metadata in the .kdb")
+    #profile_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
+    
+    #profile_parser.add_argument("--all-metadata", action="store_true", default=False, help="Include read-level k-mer metadata in the .kdb")
     profile_parser.add_argument("--sorted", action="store_true", default=False, help="Sort the output kdb file by count")
     profile_parser.add_argument("--quiet", action="store_true", default=False, help="Do not log the entire .kdb file to stdout")
     #profile_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
 
     profile_parser.add_argument("seqfile", nargs="+", type=str, metavar="<.fasta|.fastq>", help="Fasta or fastq files")
     profile_parser.add_argument("kdb", type=str, help="Kdb file")
     profile_parser.set_defaults(func=profile)
 
-    header_parser = subparsers.add_parser("header", help="Print the YAML header of the .kdb file and exit")
-    header_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
-    header_parser.add_argument("-j", "--json", help="Print as JSON. DEFAULT: YAML")
-    header_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
-    header_parser.set_defaults(func=header)
-
     graph_parser = subparsers.add_parser("graph", help="Generate an adjacency list from .fa/.fq files")
     graph_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
-    graph_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)")
+    graph_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)", required=True)
 
-    graph_parser.add_argument("-p", "--parallel", type=int, default=1, help="Shred k-mers from reads in parallel")
+    graph_parser.add_argument("-p", "--parallel", type=int, default=1, help="Parallel file reading only.")
 
-    graph_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
-    graph_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
+    #graph_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
+    #graph_parser.add_argument("--both-strands", action="store_true", default=False, help="Retain k-mers from the forward strand of the fast(a|q) file only")
     graph_parser.add_argument("--quiet", action="store_true", default=False, help="Do not list all edges and neighboring relationships to stderr")
     graph_parser.add_argument("--sorted", action="store_true", default=False, help=argparse.SUPPRESS)
-    #profile_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
+    #graph_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
 
     graph_parser.add_argument("seqfile", nargs="+", type=str, metavar="<.fasta|.fastq>", help="Fasta or fastq files")
     graph_parser.add_argument("kdbg", type=str, help=".kdbg file")
     graph_parser.set_defaults(func=make_kdbg)
 
     # assembly_parser = subparsers.add_parser("assemble", help="Use NetworkX (and/or cugraph) to perform deBruijn graphs")
     # assembly_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     # assembly_parser.add_argument("-g", "--gpu", action="store_true", default=False, help="Utilize GPU resources (requires CUDA library cugraph)")
     # assembly_parser.add_argument("kdbg", type=str, help=".kdbg file")
     # assembly_parser.set_defaults(func=assembly)
 
+
+    usage_parser = subparsers.add_parser("usage", help="provide expanded usage information on parameters and functions provided")
+    usage_parser.add_argument("-m", "--method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), required=True, help="Print expanded usage statement")
+    usage_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    usage_parser.set_defaults(func=expanded_help)
+
+    help_parser = subparsers.add_parser("help", help="provide expanded help section on parameters and functions provided")
+    help_parser.add_argument("-m", "--method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), required=True, help="Print expanded usage statement")
+    help_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    help_parser.set_defaults(func=expanded_help)
+    
     
     view_parser = subparsers.add_parser("view", help="View the contents of the .kdb file")
     view_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     view_parser.add_argument("-H", "--header", action="store_true", help="Include header in the output")
     view_parser.add_argument("--re-sort", action="store_true", help="Sort the k-mer profile before displaying")
     view_parser.add_argument("--un-sort", action="store_true", help="Unsort the k-mer profile before displaying")
     view_parser.add_argument("--dtype", type=str, default="uint64", help="Read in the profiles as unsigned integer 64bit NumPy arrays")
     view_parser.add_argument("-d", "--decompress", action="store_true", help="Decompress input? DEFAULT: ")
     view_parser.add_argument("-c", "--compress", action="store_true", help="Print compressed output")
     view_parser.add_argument("kdb_in", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be read (Optional)")
     view_parser.add_argument("kdb_out", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be written to (Optional)")
     view_parser.set_defaults(func=view)
 
+    header_parser = subparsers.add_parser("header", help="Print the YAML header of the .kdb file and exit")
+    header_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    header_parser.add_argument("-j", "--json", help="Print as JSON. DEFAULT: YAML")
+    header_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
+    header_parser.set_defaults(func=header)
+
 
     matrix_parser = subparsers.add_parser("matrix", help="Generate a reduced-dimensionality matrix of the 4^k * n (k-mers x samples) data matrix.")
     matrix_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     matrix_parser.add_argument("-p", "--parallel", type=int, default=1, help="Read files in parallel")
     matrix_parser.add_argument("--with-index", default=False, action="store_true", help="Print the row indices as well")
     matrix_parser.add_argument("--column-names", default=None, type=str, help="A filepath to a plaintext flat file of column names.")
     matrix_parser.add_argument("--delimiter", default="\t", type=str, help="The choice of delimiter to parse the input .tsv with. DEFAULT: '\t'")
@@ -1933,34 +1976,48 @@
     shuf_parser = subparsers.add_parser("shuf", help="Create a shuffled .kdb file")
     shuf_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     shuf_parser.add_argument("kdb_in", type=str, help="An indexed k-mer database file (.kdb)")
     shuf_parser.add_argument("kdb_out", type=str, help="The output shuffled k-mer database file (.kdb)")
     shuf_parser.set_defaults(func=shuf)
 
     
-    markov_probability_parser = subparsers.add_parser("probability", help=u"""
-Calculate the log-odds ratio of the Markov probability of a given sequence from the product (pi) of the transition probabilities(aij) times the frequency of the first k-mer (P(X1)), given the entire k-mer profile of a species.
+    # markov_probability_parser = subparsers.add_parser("probability", help=u"""
+# Calculate the log-odds ratio of the Markov probability of a given sequence from the product (pi) of the transition probabilities(aij) times the frequency of the first k-mer (P(X1)), given the entire k-mer profile of a species.
 
-See https://matthewralston.github.io/quickstart#kmerdb-probability for more details.
+# See https://matthewralston.github.io/quickstart#kmerdb-probability for more details.
 
-1. Durbin, R., Eddy, S.R., Krogh, A. and Mitchison, G., 1998. Biological sequence analysis: probabilistic models of proteins and nucleic acids. Cambridge university press.
-""")
+# 1. Durbin, R., Eddy, S.R., Krogh, A. and Mitchison, G., 1998. Biological sequence analysis: probabilistic models of proteins and nucleic acids. Cambridge university press.
+# """)
 
-    markov_probability_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
-    markov_probability_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter to use when reading the csv.")
-    markov_probability_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
-    markov_probability_parser.add_argument("seqfile", type=str, metavar="<.fasta|.fastq>", default=None, help="Sequences to calculate standard Markov-chain probabilities from, either .fasta or .fastq")
-    markov_probability_parser.add_argument("kdb", type=str, help="An indexed k-mer database file (.kdb)")
-    markov_probability_parser.set_defaults(func=markov_probability)
+    # markov_probability_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
+    # markov_probability_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter to use when reading the csv.")
+    # markov_probability_parser.add_argument("-b", "--fastq-block-size", type=int, default=100000, help="Number of reads to load in memory at once for processing")
+    # markov_probability_parser.add_argument("seqfile", type=str, metavar="<.fasta|.fastq>", default=None, help="Sequences to calculate standard Markov-chain probabilities from, either .fasta or .fastq")
+    # markov_probability_parser.add_argument("kdb", type=str, help="An indexed k-mer database file (.kdb)")
+    # markov_probability_parser.set_defaults(func=markov_probability)
 
     citation_parser = subparsers.add_parser("citation", help="Silence the citation notice on further runs")
     citation_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     citation_parser.set_defaults(func=citation)
     
     args=parser.parse_args()
     global logger
     logger = get_root_logger(args.verbose)
 
     sys.stderr.write("Constructed a logger for the program...\n")
     #logger.debug(sys.path)
+
+    # Print program header
+
+
+
+
+    """
+    Print detailed debugging information prior to program log.
+    """
+    from kmerdb import appmap
+    kmerdb_appmap = appmap.kmerdb_appmap( argv )
+    kmerdb_appmap.print_program_header()
+
+    
     args.func(args)
```

### Comparing `kmerdb-0.7.8/kmerdb/__main__.py` & `kmerdb-0.7.9/kmerdb/__main__.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/distance.c` & `kmerdb-0.7.9/kmerdb/distance.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/_dev/hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/core/include"
+            "/home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "kmerdb.distance",
         "sources": [
             "kmerdb/distance.pyx"
         ]
     },
     "module_name": "kmerdb.distance"
@@ -48,18 +48,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -143,14 +143,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -204,14 +206,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -265,60 +269,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -401,14 +428,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -1644,177 +1674,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1847,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2665,30 +2695,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_9
-#define __PYX_HAVE_RT_ImportType_proto_3_0_9
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_9(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_9 {
-   __Pyx_ImportType_CheckSize_Error_3_0_9 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_9 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_9 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -18000,261 +18030,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18263,29 +18293,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18296,15 +18326,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18313,29 +18343,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18346,15 +18376,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18363,29 +18393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18396,15 +18426,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18413,29 +18443,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18446,15 +18476,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18463,29 +18493,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18496,217 +18526,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18722,15 +18752,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18738,68 +18768,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18807,15 +18837,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18830,15 +18860,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18854,15 +18884,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18870,68 +18900,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18939,15 +18969,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18962,15 +18992,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18986,15 +19016,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19002,68 +19032,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19071,15 +19101,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19094,170 +19124,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22047,26 +22077,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-wfm7_y81/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../home/matt/.local/share/virtualenvs/kdb-sj-FIAv9/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -22462,41 +22492,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_9(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_9); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_9(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_9(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_9); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -26550,18 +26580,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_9
-#define __PYX_HAVE_RT_ImportType_3_0_9
-static PyTypeObject *__Pyx_ImportType_3_0_9(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_9 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -26607,23 +26637,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_9 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_9 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `kmerdb-0.7.8/kmerdb/distance.pyx` & `kmerdb-0.7.9/kmerdb/distance.pyx`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/fileutil.py` & `kmerdb-0.7.9/kmerdb/fileutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
         else:
             raise RuntimeError("kmerdb.fileutil.KDBReader encountered an unexpected type for the header_dict read from the .kdb header blocks")
         logger.info("Reading additional blocks as YAML...")
         logger.debug("Reading additional blocks as YAML...")
         sys.stderr.write("\n")
         logger.info("Validating the header data against the schema...")
         try:
-            jsonschema.validate(instance=initial_header_data, schema=config.metadata_schema)
+            jsonschema.validate(instance=initial_header_data, schema=config.kdb_metadata_schema)
             self.metadata = dict(initial_header_data)
             
             self.k = self.metadata['k']
             self.kmer_ids_dtype = self.metadata["kmer_ids_dtype"]
             self.count_dtype = self.metadata["count_dtype"]
             self.frequencies_dtype = self.metadata["frequencies_dtype"]
             self.sorted = self.metadata["sorted"]
@@ -766,15 +766,15 @@
     
     def __init__(self, metadata:OrderedDict, filename=None, mode="w", fileobj=None, compresslevel=6):
         """Initilize the class."""
         if not isinstance(metadata, OrderedDict):
             raise TypeError("kmerdb.fileutil.KDBWriter expects a valid metadata object as its first positional argument")
         try:
             logger.debug("Validating metadata schema against the config.py header schema")
-            jsonschema.validate(instance=dict(metadata), schema=config.metadata_schema)
+            jsonschema.validate(instance=dict(metadata), schema=config.kdb_metadata_schema)
             self.metadata = metadata
             self.k = self.metadata['k']
         except jsonschema.ValidationError as e:
             logger.debug(e)
             logger.error("kmerdb.fileutil.KDBReader couldn't validate the header YAML")
             raise e
```

### Comparing `kmerdb-0.7.8/kmerdb/graph.py` & `kmerdb-0.7.9/kmerdb/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from builtins import open as _open
 
 import jsonschema
 from Bio import SeqIO, Seq, bgzf
 
 
 import numpy as np
-import networkx as nx
+#import networkx as nx
 
 from kmerdb import fileutil, parse, kmer, config, util
 
 # Logging configuration
 import logging
 logger = logging.getLogger(__file__)
 
@@ -270,15 +270,15 @@
     counts = np.zeros(N, dtype="uint64")
     
     logger.debug("Initializing edge list fileparser...")
     seqprsr = parse.SeqParser(filepath, b, k)
     fasta = not seqprsr.fastq # Look inside the seqprsr object for the type of file
     
     # Initialize the kmer class for sequence shredding activities
-    Kmer = kmer.Kmers(k, strand_specific=not both_strands, verbose=fasta, all_metadata=True) # A wrapper class to shred k-mers with
+    Kmer = kmer.Kmers(k) # A wrapper class to shred k-mers with
     
     # Actually load in records 'recs'
     recs = [r for r in seqprsr]
         
     logger.info("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
         
         
@@ -609,16 +609,16 @@
             current_kmer
             pair : the pair of adjacent k-mers with the k-1mer as identical sequence
             pair_ids  : ids
             k1 : k-1mer   current_kmer[1:] left-most char ommitted, (neighbors *will* get appended to right side)
             k2 : k-1mer   current_kmer[:-1] right-most char ommitted, neighbors prepended
 
             # e.g. ACTGACTG
-            # pair0 = CTGACTG (k-1 mer via first char removed. k-1 mer that receives appends.
-            # pair1 = ACTGACT (k-1 mer via last char removed. k-1 mer that gets at its prepend.
+            # pair0 = CTGACTG (k-1 mer via first char removed. k-1 mer that receives appends)
+            # pair1 = ACTGACT (k-1 mer via last char removed. k-1 mer that gets at its prepend.)
 
             DECLARATIONS FINISHED
             """
             # Commented 3/11/24 ish thanks nic
             # Working on some bills, then back to the drawing board.
             # I mean, aside from a lab job, if i could wfh or work localish then taking a month or so off to go to the mountains for soil sampling.
             # I'd really want to go with a guide or expert.
@@ -726,15 +726,15 @@
     """
     return all_edges_in_kspace
 
 
 
 def create_graph(nodes:list, edge_tuples:list, gpu:bool=False):
 
-
+    import networkx as nx
 
     if nodes is None or type(nodes) is not list or not all(type(n) is not int for n in nodes):
         raise TypeError("kmerdb.graph.create_graph expects the first argument to be a list of ints")
     elif edge_tuples is None or type(edge_tuples) is not list or not all(len(e) != 3 for e in edge_tuples) or not all((type(e[0]) is int and type(e[1]) is int) for e in edge_tuples):
         raise TypeError("kmerdb.graph.create_graph expects the second argument to be a list of tuples of length 2")
     elif gpu is None or type(gpu) is not bool:
         raise TypeError("kmerdb.graph.create_graph expects the keyword argument gpu to be a bool")
@@ -1308,11 +1308,11 @@
         
     def parsefile(self, filename):
         """Wrapper function for graph.parsefile to keep arguments succinct for deployment through multiprocessing.Pool
             
         :param filename: the filepath of the fasta(.gz)/fastq(.gz) to process with kmerdb.graph.parsefile
         :type filename: str
         """
-        return parsefile(filename, self.arguments.k, quiet=self.arguments.quiet, b=self.arguments.fastq_block_size, both_strands=self.arguments.both_strands)
+        return parsefile(filename, self.arguments.k, quiet=self.arguments.quiet)
```

### Comparing `kmerdb-0.7.8/kmerdb/index.py` & `kmerdb-0.7.9/kmerdb/index.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/kmer.py` & `kmerdb-0.7.9/kmerdb/kmer.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/parse.py` & `kmerdb-0.7.9/kmerdb/parse.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,33 +46,28 @@
 import logging
 logger = logging.getLogger(__file__)
 
 
 
 
 
-def parsefile(filepath:str, k:int, rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
+def parsefile(filepath:str, k:int, ): #rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
     """Parse a single sequence file in blocks/chunks with multiprocessing support
 
     :param filepath: Path to a fasta or fastq file
     :type filepath: str
     :param k: Choice of k to shred k-mers with
     :type k: int
     :param b: Number of reads (per block) to process in parallel
     :type b: int
     :param stranded: Strand specificity argument for k-mer shredding process
     :type stranded: bool
     :raise TypeError: filepath was invalid
     :raise OSError: filepath was invalid
     :raise TypeError: k was invalid
-    :raise TypeError: rows_per_batch was invalid
-    :raise TypeError: b was invalid
-    :raise TypeError: n was invalid
-    :raise TypeError: both_strands was invalid
-    :raise TypeError: all_metadata was invalid
     :raise TypeError: invalid dtype
     :raise ValueError: invalid (None) kmer id detected
     :raise ValueError: mismatched number of kmer_ids, associated sequence/read ids, starting locations, and reverse bools
     :raise AssertionError: Error in nullomer count estimation
     :returns: (counts, header_dictionary, nullomer_array, all_metadata) header_dictionary is the file's metadata for the header block
     :rtype: (numpy.ndarray, dict, list, list)
 
@@ -81,45 +76,45 @@
     from kmerdb import kmer
     if filepath is None or type(filepath) is not str:
         raise TypeError("kmerdb.parse.parsefile expects a str as its first positional argument")
     elif not os.path.exists(filepath):
         raise OSError("kmerdb.parse.parsefile could not find the file '{0}' on the filesystem".format(filepath))
     elif k is None or type(k) is not int:
         raise TypeError("kmerdb.parse.parsefile expects an int as its second positional argument")
-    elif rows_per_batch is None or type(rows_per_batch) is not int:
-        raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'rows_per_batch' to be an int")
-    elif b is None or type(b) is not int:
-        raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'b' to be an int")
-    elif n is None or type(n) is not int:
-        raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'n' to be an int")
-    elif both_strands is None or type(both_strands) is not bool:
-        raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'both_strands' to be a bool")
-    elif all_metadata is None or type(all_metadata) is not bool:
-        raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'all_metadata' to be a bool")
+    # elif rows_per_batch is None or type(rows_per_batch) is not int:
+    #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'rows_per_batch' to be an int")
+    # elif b is None or type(b) is not int:
+    #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'b' to be an int")
+    # elif n is None or type(n) is not int:
+    #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'n' to be an int")
+    # elif both_strands is None or type(both_strands) is not bool:
+    #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'both_strands' to be a bool")
+    # elif all_metadata is None or type(all_metadata) is not bool:
+    #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'all_metadata' to be a bool")
     data = {} # This is the dictionary of tuples, keyed on k-mer id, and containing 3-tuples ('kmer_id', 'read/start/reverse')
     keys = set()
     rows = []
     N = 4**k
     nullomers = set()
     # Build fasta/fastq parser object to stream reads into memory
     logger.debug("Initializing parser...")
-    seqprsr = SeqParser(filepath, b, k)
+    seqprsr = SeqParser(filepath, k)
     fasta = not seqprsr.fastq # Look inside the seqprsr object for the type of file
 
     # Initialize the kmer array
     try:
         counts = np.zeros(N, dtype="uint64")
     except TypeError as e:
         logger.error("Invalid dtype for numpy array instantiation")
         logger.error(e)
         raise e
 
     logger.info("Successfully allocated space for {0} unsigned integers: {1} bytes".format(N, counts.nbytes))
         # Instantiate the kmer class
-    Kmer = kmer.Kmers(k, strand_specific=not both_strands, verbose=fasta, all_metadata=all_metadata) # A wrapper class to shred k-mers with
+    Kmer = kmer.Kmers(k, verbose=fasta) # A wrapper class to shred k-mers with
 
     recs = [r for r in seqprsr] # A block of exactly 'b' reads-per-block to process in parallel
     if not fasta:
         logger.debug("Read exactly {0} records from the seqparser object".format(len(recs)))
         assert len(recs) <= b, "The seqparser should return exactly {0} records at a time".format(b)
     else:
         logger.debug("Skipping the block size assertion for fasta files")
@@ -165,70 +160,51 @@
         # The graph can be explicitly collapsed when you want to, by supplying reads or sequence information, that is contiguous "in your judgement".
         # By introducing these artificial gaps, we expose the errors or unspecified bases through data.
         #
         logger.info("Found {0} invalid or enumerable k-mers, sequences which have no defined index, i".format(num_sus))
         logger.debug("In other words, one or more characters in your .fasta or .fastq file were 'N' or otherwise contained IUPAC characters that need to be substituted.")
         logger.debug("We have chosen to omit k-mer with unspecified nucleotides 'N', and these make gaps in our database explicitly.")
         logger.info("These can be recovered from the reads if they are needed, and the read ids may be found with the experimental --all-metadata flag")
-        if all_metadata:
+        # if all_metadata:
+
+        #     logger.warning("\n\n\nGENERATING ALL METADATA\n\n\nThis is extremely expensive and experimental. You have been warned.\n\n\n")
+        #     reads = list(chain.from_iterable(map(lambda x: x['seqids'], list_of_dicts)))
+        #     starts = list(chain.from_iterable(map(lambda x: x['starts'], list_of_dicts)))
+        #     reverses = list(chain.from_iterable(map(lambda x: x['reverses'], list_of_dicts)))
+        #     logger.debug("Checking each k-mer for N-content and IUPAC substitution")
+        #     for i, x in enumerate(kmer_ids): # This removes N content
+        #         if i in sus: # This is where we actually delete the N content, in case that is eventually supported.
+        #             kmer_ids[i] = None
+        #             reads[i] = None
+        #             starts[i] = None
+        #             reverses[i] = None
+        #     kmer_ids = list(filter(lambda k: k is not None, kmer_ids)) 
+        #     reads = list(filter(lambda r: r is not None, reads))
+        #     starts = list(filter(lambda s: s is not None, starts))
+        #     reverses = list(filter(lambda r: r is not None, reverses))
+        # else:
+        logger.debug("Checking each k-mer for IUPAC substitution or N content.")
+        for i, x in enumerate(kmer_ids): # Here we remove the k-mer ids where N-content is detected, in case they are needed, you can use kmer_ids prior to this point to build functionality.
+            if i in sus:
+                kmer_ids[i] = None
+        logger.info("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions")
+        kmer_ids = list(filter(lambda k: k is not None, kmer_ids))
+        reads = [] # I'm keeping this in, just in case for some reason the variable names are needed in the 
+        starts = []
+        reverses = []
+        if None in kmer_ids:
+            # Actually they were just introduced to be filtered out, instead of deleted
+            # Because each deletion whould cange the array index
+            # So instead we set ghtme to None, and filter out
+            raise ValueError("kmerdb.parse.parsefile encountered an invalid kmer_id. Internal error.")
 
-            logger.warning("\n\n\nGENERATING ALL METADATA\n\n\nThis is extremely expensive and experimental. You have been warned.\n\n\n")
-            reads = list(chain.from_iterable(map(lambda x: x['seqids'], list_of_dicts)))
-            starts = list(chain.from_iterable(map(lambda x: x['starts'], list_of_dicts)))
-            reverses = list(chain.from_iterable(map(lambda x: x['reverses'], list_of_dicts)))
-            logger.debug("Checking each k-mer for N-content and IUPAC substitution")
-            for i, x in enumerate(kmer_ids): # This removes N content
-                if i in sus: # This is where we actually delete the N content, in case that is eventually supported.
-                    kmer_ids[i] = None
-                    reads[i] = None
-                    starts[i] = None
-                    reverses[i] = None
-            kmer_ids = list(filter(lambda k: k is not None, kmer_ids)) 
-            reads = list(filter(lambda r: r is not None, reads))
-            starts = list(filter(lambda s: s is not None, starts))
-            reverses = list(filter(lambda r: r is not None, reverses))
-        else:
-            logger.debug("Checking each k-mer for IUPAC substitution or N content.")
-            for i, x in enumerate(kmer_ids): # Here we remove the k-mer ids where N-content is detected, in case they are needed, you can use kmer_ids prior to this point to build functionality.
-                if i in sus:
-                    kmer_ids[i] = None
-            logger.info("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions")
-            kmer_ids = list(filter(lambda k: k is not None, kmer_ids))
-            reads = [] # I'm keeping this in, just in case for some reason the variable names are needed in the 
-            starts = []
-            reverses = []
-            if None in kmer_ids:
-                logger.debug("In the no-metadata field")
-                # Actually they were just introduced to be filtered out, instead of deleted
-                # Because each deletion whould cange the array index
-                # So instead we set ghtme to None, and filter out
-                raise ValueError("kmerdb.parse.parsefile encountered an invalid kmer_id. Internal error.")
 
-        #logger.debug(kmer_ids)
         logger.debug("{0} 'clean' kmers were identified successfully from {1} input sequences".format(len(kmer_ids), num_recs))
         logger.debug("Flatmapped {0} kmers for their metadata aggregation".format(len(kmer_ids), len(starts)))
         # Assert that all list lengths are equal before adding metadata to k-mers
-        if all_metadata is True and len(kmer_ids) == len(reads) and len(reads) == len(starts) and len(starts) == len(reverses):
-            N = len(starts)
-                
-            kmer_metadata = list(zip(kmer_ids, reads, starts, reverses))
-            # Everything is in the right order
-            logger.warning("Dumping all metadata into the .kdb file eventually. This could be expensive...")
-
-        elif not all_metadata and len(reads) == 0 and len(starts) == 0 and len(reverses) == 0:
-            logger.debug("Skipping metadata allocation")
-            pass # If we're not doing metadata, don't do it
-        else: # Raise an error if the numbers of items per list are not equal
-            logger.error("{0} kmer ids".format(len(kmer_ids)))
-            logger.error("{0} sequence/read associations".format(len(reads)))
-            logger.error("{0} start positions for the associations found".format(len(starts)))
-            logger.error("{0} reverse bools for each association".format(len(reverses)))
-                
-            raise ValueError("Unexpectedly, the number of ids did not match up with the number of other metadata elements per k-mer OR other unknown error. Internal error.")
-
         # else:
         #     raise RuntimeError("Still have no clue what's going on...")
         # On disk k-mer counting
         # Thank you, this was brilliant
         # https://stackoverflow.com/a/9294062/12855110
         # 01-01-2022 This has been removed in favor of in-memory counting
         num_kmers = len(kmer_ids)
@@ -236,17 +212,17 @@
         if num_kmers == 0:
             raise ValueError("No k-mers available to add. Please report to the issue tracker")
         else:
             sys.stderr.write("\nAccumulating all k-mers from this set of records...")
             for kmer in kmer_ids:
                 counts[kmer] += 1
         # all_kmer_metadata
-        if all_metadata:
-            for single_kmer_id, read, start, reverse in kmer_metadata:
-                all_kmer_metadata[single_kmer_id].append((read, start, reverse))
+        # if all_metadata:
+        #     for single_kmer_id, read, start, reverse in kmer_metadata:
+        #         all_kmer_metadata[single_kmer_id].append((read, start, reverse))
 
         recs = [r for r in seqprsr] # The next block of exactly 'b' reads
         logger.info("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"))
     # Get nullomers
     # only nullomer counts
     unique_kmers = int(np.count_nonzero(counts))
 
@@ -265,17 +241,17 @@
     seqprsr.total_kmers = int(np.sum(counts))
     seqprsr.unique_kmers = unique_kmers
     seqprsr.nullomers = num_nullomers
 
 
     
     seqprsr.nullomer_array = np.array(all_theoretical_kmer_ids, dtype="uint64")[is_nullomer]
-    sys.stderr.write("\n\n\nFinished counting k-mers{0} from '{1}'...\n\n\n".format(' and metadata' if all_metadata else '', filepath))
+    sys.stderr.write("\n\n\nFinished counting k-mers from '{0}'...\n\n\n".format(filepath))
 
-    return counts, seqprsr.header_dict(), seqprsr.nullomer_array, all_kmer_metadata
+    return counts, seqprsr.header_dict(), seqprsr.nullomer_array
 
 
 
 
 
 class SeqParser:
     """
@@ -284,21 +260,23 @@
     It allows you to read either fasta or fastq data in blocks, obviously useful for the latter.
 
 
     :ivar filepath: The .fastq, .fastq.gz, .fasta, .fasta.gz, .fna, .fna.gz, .fa, or .fa.gz file.
     :ivar num: The number of records to read in from a .fastq
     :ivar k: The choice of k to initialize the calculation of kmer/nullomer counts.
     """
-    def __init__(self, filepath, num, k):
+    def __init__(self, filepath:str, k:int, num:int=100000, ):
         """
         The SeqParser class wraps up some functionality  
         """
         
         if type(filepath) is not str:
             raise TypeError("kmerdb.parse.SeqParser expects a str as its first positional argument")
+        elif not os.access(filepath, os.R_OK):
+            raise TypeError("kmerdb.parse.SeqParser expects an existing path on the operating system as its first argument")
         elif type(num) is not int:
             raise TypeError("kmerdb.parse.SeqParser expects an int as its second positional argument")
         elif type(k) is not int:
             raise TypeError("kmerdb.parse.SeqParser expects an int as its third positional argument")
         
         self.k = k
         self.num = num
@@ -449,10 +427,10 @@
     def parsefile(self, filename):
         """Wrapper function for parse.parsefile to keep arguments succinct for deployment through multiprocessing.Pool
             
         :param filename: the filepath of the fasta(.gz)/fastq(.gz) to process with parsefile -> parse.SeqParser
         :type filename: str
         :returns: (db, m, n)
         """
-        return parsefile(filename, self.arguments.k, rows_per_batch=self.arguments.batch_size, b=self.arguments.fastq_block_size, n=self.arguments.n, both_strands=self.arguments.both_strands, all_metadata=self.arguments.all_metadata)
+        return parsefile(filename, self.arguments.k)
```

### Comparing `kmerdb-0.7.8/kmerdb/probability.py` & `kmerdb-0.7.9/kmerdb/probability.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/python_distances.py` & `kmerdb-0.7.9/kmerdb/python_distances.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb/util.py` & `kmerdb-0.7.9/kmerdb/util.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.7.8/kmerdb.egg-info/PKG-INFO` & `kmerdb-0.7.9/kmerdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.7.8
-Summary: Yet another kmer library for Python
+Version: 0.7.9
+Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.0.tar.gz
-Author: Matthew Ralston
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
+Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -207,38 +207,69 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://matthewralston.github.io/kmerdb
 Project-URL: QuickStart, https://matthewralston.github.io/kmerdb/quickstart.html
-Project-URL: Install, https://matthewralston.github.io/kmerdb/installation.html
-Project-URL: ForAcademics, https://matthewralston.github.io/kmerdb/academics.html
 Project-URL: Github, https://github.com/MatthewRalston/kmerdb
 Project-URL: Issues, https://github.com/MatthewRalston/kmerdb/issues
-Keywords: bioinformatics,fastq,fasta,k-mer,kmer,k-merdb,kmerdb,kdb
+Keywords: bioinformatics,fastq,fasta,k-mer,kmer
 Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 7 - Inactive
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: PalmOS
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8.0
+Classifier: Intended Audience :: Other Audience
+Classifier: License :: Free For Educational Use
+Classifier: License :: Free for non-commercial use
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Topic :: File Formats
+Classifier: Topic :: Games/Entertainment :: Puzzle Games
+Classifier: Topic :: Text Processing :: Indexing
+Classifier: Topic :: Text Processing
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.7.4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: numpy>=1.21.2
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: jsonschema>=4.17.3
+Requires-Dist: psutil>=4.2.0
+Requires-Dist: Cython>=3.0.8
+Requires-Dist: biopython>=1.81
+Requires-Dist: scipy>=1.11.4
+Requires-Dist: scikit-learn==1.2.2
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: setuptools>=69.2.0
+Provides-Extra: dev
+Requires-Dist: auditwheel>=5.1.2; extra == "dev"
+Requires-Dist: build>=0.9.0; extra == "dev"
+Requires-Dist: coverage>=4.5.4; extra == "dev"
+Requires-Dist: expects>=0.9.0; extra == "dev"
+Requires-Dist: docutils>=0.17; extra == "dev"
+Requires-Dist: sphinx>=4.3.2; extra == "dev"
+Requires-Dist: pytest>=5.3.5; extra == "dev"
+Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
 > A Python CLI and module for k-mer profiles, similarities, and graph databases
 
 NOTE: This project is in beta stage. Development is ongoing. But feel free to clone the repository and play with the code for yourself.
 
 ## Development Status
@@ -283,24 +314,24 @@
 
 All other dependencies are managed directly by pip. 
 
 
 ### OSX and Linux release:
 
 ```sh
-pip install kmerdb
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
 
 ### Development installation:
 
 ```sh
 git clone https://github.com/MatthewRalston/kmerdb.git
-pip install -e .
+pip install .
 ```
 
 ## Usage Example
 
 NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
 
 <!-- ## NOTE: Temporary usage pattern:
@@ -382,15 +413,15 @@
 python setup.py test
 ```
 
 ## License
 
 Created by Matthew Ralston - [Scientist, Programmer, Musician](http://matthewralston.github.io) - [Email](mailto:mralston.development@gmail.com)
 
-Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, but we march into the information age with this ethos. I have the patent rights to this software. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
+Distributed under the Apache license. See `LICENSE.txt` for the copy distributed with this project. Open source software is not for everyone, and im the author and maintainer. cheers, on me. You may use and distribute this software, gratis, so long as the original LICENSE.txt is distributed along with the software. This software is distributed AS IS and provides no warranties of any kind.
 
 ```
    Copyright 2020 Matthew Ralston
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
```

### Comparing `kmerdb-0.7.8/kmerdb.egg-info/SOURCES.txt` & `kmerdb-0.7.9/kmerdb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 kmerdb/CITATION.txt
 kmerdb/__init__.py
 kmerdb/__main__.py
+kmerdb/appmap.py
+kmerdb/banners.py
 kmerdb/config.py
 kmerdb/distance.c
 kmerdb/distance.pyx
 kmerdb/fileutil.py
 kmerdb/graph.py
 kmerdb/index.py
 kmerdb/kmer.py
+kmerdb/legacy.py
 kmerdb/parse.py
 kmerdb/probability.py
 kmerdb/python_distances.py
 kmerdb/util.py
 kmerdb.egg-info/PKG-INFO
 kmerdb.egg-info/SOURCES.txt
 kmerdb.egg-info/dependency_links.txt
```

### Comparing `kmerdb-0.7.8/setup.py` & `kmerdb-0.7.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,37 +105,53 @@
         return None
                 
 # Package meta-data.
 NAME = 'kmerdb'
 DESCRIPTION = 'Yet another kmer library for Python'
 long_description = 'See README.md for details'
 URL = 'https://github.com/MatthewRalston/kmerdb'
-CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.7.0.tar.gz"
-EMAIL = 'mrals89@gmail.com'
-AUTHOR = 'Matthew Ralston'
-REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "0.7.8"
-KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer", "k-merdb", "kmerdb", "kdb"],
+CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz"
+EMAIL = 'mralston.development@gmail.com'
+AUTHOR = 'fross'
+REQUIRES_PYTHON = ">=3.7.4"
+#REQUIRES_PYTHON = '>=3.12.2'
+VERSION = "0.7.9"
+KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer"]
 CLASSIFIERS = [
-    "Development Status :: 1 - Planning",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Bio-Informatics",
-    "Topic :: Software Development :: Libraries :: Python Modules",
+	    "Development Status :: 1 - Planning",
+	    "Development Status :: 2 - Pre-Alpha",
+	    "Development Status :: 7 - Inactive",
+	    "Environment :: Console",
+	    "Intended Audience :: Developers",
+	    "Intended Audience :: Science/Research",
+	    "License :: OSI Approved :: Apache Software License",
+	    "Operating System :: OS Independent",
+	    "Programming Language :: Python",
+	    "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3.12",
+	    "Programming Language :: Python :: 3 :: Only",
+	    "Operating System :: PalmOS",
+	    "Topic :: Scientific/Engineering",
+	    "Topic :: Scientific/Engineering :: Bio-Informatics",
+	    "Topic :: Software Development :: Libraries :: Python Modules",
+	    "Intended Audience :: Other Audience",
+	    "License :: Free For Educational Use",
+	    "License :: Free for non-commercial use",
+	    "License :: OSI Approved :: Academic Free License (AFL)",
+	    "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+	    "Topic :: File Formats",
+	    "Topic :: Games/Entertainment :: Puzzle Games",
+	    "Topic :: Text Processing :: Indexing",
+	    "Topic :: Text Processing",
+	    #"Topic :: Software Development :: Assemblers"
+	    "Operating System :: POSIX :: Linux",
 ]
+
+
 # What packages are required for this module to be executed?
 
 #REQUIRED = [l.rstrip() for l in open('./requirements.txt', 'r')]
 #REQUIRED.remove("-e git://github.com/MatthewRalston/ecopy.git#egg=ecopy")
 #REQUIRED.append("ecopy @ git+https://github.com/MatthewRalston/ecopy@master")
```

### Comparing `kmerdb-0.7.8/test/test_kmer.py` & `kmerdb-0.7.9/test/test_kmer.py`

 * *Files identical despite different names*

