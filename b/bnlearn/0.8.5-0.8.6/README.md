# Comparing `tmp/bnlearn-0.8.5.tar.gz` & `tmp/bnlearn-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.8.5.tar", last modified: Sat Mar 16 14:41:59 2024, max compression
+gzip compressed data, was "bnlearn-0.8.6.tar", last modified: Tue Apr  9 19:51:11 2024, max compression
```

## Comparing `bnlearn-0.8.5.tar` & `bnlearn-0.8.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.873778 bnlearn-0.8.5/
--rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.5/LICENSE
--rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12800 2024-03-16 14:41:59.873778 bnlearn-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.836779 bnlearn-0.8.5/bnlearn/
--rw-rw-rw-   0        0        0     4643 2024-03-16 14:38:55.000000 bnlearn-0.8.5/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    72287 2023-11-10 21:59:03.000000 bnlearn-0.8.5/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.856973 bnlearn-0.8.5/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.873778 bnlearn-0.8.5/bnlearn/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/discretize/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.5/bnlearn/discretize/discretize.py
--rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.5/bnlearn/discretize/learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    47916 2024-03-16 14:32:22.000000 bnlearn-0.8.5/bnlearn/examples.py
--rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/examples_discretize.py
--rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/network.py
--rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.5/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.873778 bnlearn-0.8.5/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.873778 bnlearn-0.8.5/bnlearn/tests/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/tests/discretize/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/tests/discretize/test_discretize.py
--rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.5/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.5/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-03-16 14:41:59.856973 bnlearn-0.8.5/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    12800 2024-03-16 14:41:59.000000 bnlearn-0.8.5/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2024-03-16 14:41:59.000000 bnlearn-0.8.5/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 14:41:59.000000 bnlearn-0.8.5/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2024-03-16 14:41:59.000000 bnlearn-0.8.5/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-16 14:41:59.000000 bnlearn-0.8.5/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 14:41:59.873778 bnlearn-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     2131 2024-03-16 14:36:04.000000 bnlearn-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.528980 bnlearn-0.8.6/
+-rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12276 2024-04-09 19:51:11.528980 bnlearn-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.479159 bnlearn-0.8.6/bnlearn/
+-rw-rw-rw-   0        0        0     4729 2024-04-09 19:32:51.000000 bnlearn-0.8.6/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    72560 2024-04-09 19:32:38.000000 bnlearn-0.8.6/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.512926 bnlearn-0.8.6/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.512926 bnlearn-0.8.6/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.6/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.6/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    52338 2024-03-28 11:59:09.000000 bnlearn-0.8.6/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.6/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.522962 bnlearn-0.8.6/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.522962 bnlearn-0.8.6/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.6/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.6/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:51:11.510914 bnlearn-0.8.6/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12276 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      204 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 19:51:11.000000 bnlearn-0.8.6/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:51:11.528980 bnlearn-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     2088 2024-04-09 19:29:59.000000 bnlearn-0.8.6/setup.py
```

### Comparing `bnlearn-0.8.5/LICENSE` & `bnlearn-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/MANIFEST.in` & `bnlearn-0.8.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/PKG-INFO` & `bnlearn-0.8.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: bnlearn
-Version: 0.8.5
-Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
-Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.5.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pgmpy>=0.1.18
-Requires-Dist: networkx>=2.7.1
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas==1.5.3
-Requires-Dist: d3blocks>=1.4.9
-Requires-Dist: tqdm
-Requires-Dist: ismember
-Requires-Dist: scikit-learn
-Requires-Dist: funcsigs
-Requires-Dist: statsmodels
-Requires-Dist: python-louvain
-Requires-Dist: packaging
-Requires-Dist: df2onehot
-Requires-Dist: fsspec
-Requires-Dist: pypickle
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: datazets
-
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,38 +1,24 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.5 Summary: Python package for
-learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.5.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist:
-d3blocks>=1.4.9 Requires-Dist: tqdm Requires-Dist: ismember Requires-Dist:
-scikit-learn Requires-Dist: funcsigs Requires-Dist: statsmodels Requires-Dist:
-python-louvain Requires-Dist: packaging Requires-Dist: df2onehot Requires-Dist:
-fsspec Requires-Dist: pypickle Requires-Dist: tabulate Requires-Dist:
-ipywidgets Requires-Dist: datazets # bnlearn - Library for Bayesian network
-learning and inference [![Python](https://img.shields.io/pypi/pyversions/
-bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version]
-(https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) !
-[GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://
-img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/
-bnlearn/network) [![Open Issues](https://img.shields.io/github/issues/erdogant/
-bnlearn.svg)](https://github.com/erdogant/bnlearn/issues) [![Project Status]
-(http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/bnlearn/
-month)](https://pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/
-badge/bnlearn)](https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/
-badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs]
-(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-bnlearn/) [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
+# bnlearn - Library for Bayesian network learning and inference [![Python]
+(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
+pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
+(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
+231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
 erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) ![GitHub
 repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn) [![Donate]
 (https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
 html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
 Documentation.html#colab-notebook) ### ``bnlearn`` is Python package for
```

### Comparing `bnlearn-0.8.5/README.md` & `bnlearn-0.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: bnlearn
+Version: 0.8.6
+Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,9 +1,17 @@
-# bnlearn - Library for Bayesian network learning and inference [![Python]
-(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.6 Summary: Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
 (https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
 img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
 img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
 bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
 erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
 Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
```

### Comparing `bnlearn-0.8.5/bnlearn/__init__.py` & `bnlearn-0.8.6/bnlearn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,41 +34,42 @@
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.8.5'
+__version__ = '0.8.6'
 
 import pgmpy
 # Check version pgmpy
 if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
     raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
 import matplotlib
 if not version.parse(matplotlib.__version__) >= version.parse("3.3.4"):
     raise ImportError('[bnlearn] >Error: Matplotlib version should be >= v3.3.4\nTry to: pip install -U matplotlib')
 
 import networkx as nx
-if not version.parse(nx.__version__) >= version.parse("2.7.1"):
+if version.parse(nx.__version__) < version.parse("2.7.1"):
     raise ImportError('[bnlearn] >Error: networkx version should be > 2.7.1\nTry to: pip install -U networkx')
 
 import numpy as np
-if not version.parse(np.__version__) >= version.parse("1.24.1"):
+if version.parse(np.__version__) < version.parse("1.24.1"):
     raise ImportError('[bnlearn] >Error: numpy version should be > 1.24.1\nTry to: pip install -U numpy')
 
 import pandas as pd
-if not version.parse(pd.__version__) <= version.parse("1.5.3"):
+if version.parse(pd.__version__) > version.parse("1.5.3"):
     raise ImportError('[bnlearn] >Error: pands version should be <= 1.5.3')
 
-import d3blocks as d3
-if not version.parse(d3.__version__) <= version.parse("1.4.9"):
-    raise ImportError('[bnlearn] >Error: d3blocks version should be >= 1.4.9')
+# This one is moved towards the interactive plot function because it is not required in the setup.
+# import d3blocks as d3
+# if version.parse(d3.__version__) < version.parse("1.4.9"):
+#     raise ImportError('[bnlearn] >Error: d3blocks version should be >= 1.4.9')
 
 # module level doc-string
 __doc__ = """
 bnlearn - bnlearn is an Python package for learning the graphical structure of Bayesian networks, estimate their parameters, perform inference, sampling and comparing networks.
 ================================================================================================================================================================================
 
 Description
```

### Comparing `bnlearn-0.8.5/bnlearn/bnlearn.py` & `bnlearn-0.8.6/bnlearn/bnlearn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1169,19 +1169,24 @@
     # Return
     return fig
 
 
 # %% Plot interactive
 def _plot_interactive(params_interactive, nodelist, node_colors, node_sizes, edgelist, edge_colors, edge_weights, title, tooltip, verbose=3):
     # Try to import d3blocks
+    from packaging import version
     try:
         # Load library
         from d3blocks import D3Blocks
     except ModuleNotFoundError:
-        if verbose>=1: raise Exception('[bnlearn] >"d3blocks" library is not installed. Please pip install first: "pip install d3blocks"')
+        if verbose>=1: raise Exception('[bnlearn] >"d3blocks" library is not installed. Pip install first: "pip install d3blocks"')
+
+    import d3blocks as d3
+    if version.parse(d3.__version__) < version.parse("1.4.9"):
+        raise ImportError('[bnlearn] >Error: d3blocks version should be >= 1.4.9. Pip install to the latest version first: "pip install -U d3blocks"')
 
     if params_interactive['filepath'] is None: params_interactive['filepath'] = title.strip().replace(' ', '_') + '.html'
 
     # Initialize
     d3 = D3Blocks()
 
     # Set the min_weight
```

### Comparing `bnlearn-0.8.5/bnlearn/confmatrix.py` & `bnlearn-0.8.6/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/discretize/discretize.py` & `bnlearn-0.8.6/bnlearn/discretize/discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/discretize/learn_discrete_bayes_net.py` & `bnlearn-0.8.6/bnlearn/discretize/learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/examples.py` & `bnlearn-0.8.6/bnlearn/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,123 @@
+# %% compute causalities
+import bnlearn as bn
+# Load asia DAG
+df = bn.import_example('asia', verbose=0)
+# print(tabulate(df.head(), tablefmt="grid", headers="keys"))
+# print(df)
+
+# Structure learning
+model = bn.structure_learning.fit(df, verbose=0, scoretype='bic', methodtype='hc')
+model = bn.structure_learning.fit(df, verbose=0, scoretype='k2', methodtype='hc')
+
+# Plot the DAG
+bn.plot(model, verbose=0, interactive=True, node_color='#000000')
+
+# Test for independence
+model = bn.independence_test(model, df, prune=False)
+
+# Plot the DAG
+bn.plot(model, verbose=0, interactive=True, node_color='#000000')
+# Print the CPDs
+bn.print_CPD(model)
+# Comparison
+
+# Learn its parameters from data and perform the inference.
+model_with_CPD = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
+model = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
+# Print the CPDs
+bn.print_CPD(model_with_CPD)
+
+# Nothing is changed for the DAG. Only the CPDs are estimated now.
+bn.compare_networks(model_with_CPD, model, verbose=0)
+
+# Make inference
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1, 'bronc':1}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1, 'bronc':1, 'xray':1}, verbose=3)
+
+# q4 = bn.inference.fit(model_with_CPD, variables=['bronc', 'lung'], evidence={'smoke': 1, 'xray': 0}, verbose=3)
+# q4 = bn.inference.fit(DAG, variables=['bronc','lung','xray'], evidence={'smoke':1}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['xray'], evidence={'smoke':1})
+
+# pd.DataFrame(index=q4.variables, data=q4.values, columns=q4.variables)
+
+# edges = [('Cloudy', 'Sprinkler'),
+#          ('Cloudy', 'Rain'),
+#          ('Sprinkler', 'Wet_Grass'),
+#          ('Rain', 'Wet_Grass')]
+
+# # Make the actual Bayesian DAG
+# DAG = bn.make_DAG(edges)
+
+
+# %% Police shooting
+import bnlearn as bn
+from datazets import datazets
+df = datazets.get(url=r'https://raw.githubusercontent.com/washingtonpost/data-police-shootings/master/v2/fatal-police-shootings-data.csv', overwrite=True)
+del df['id']
+del df['name']
+del df['county']
+del df['state']
+del df['date']
+del df['agency_ids']
+del df['latitude']
+del df['longitude']
+del df['race_source']
+
+# dfhot, dfnum = bn.df2onehot(df, y_min=2)
+
+# Structure learning
+DAG = bn.structure_learning.fit(df, methodtype='hc', scoretype='bic') # hillclimbsearch
+
+# Constrained based
+# DAG = bn.structure_learning.fit(df, methodtype='cs')
+
+# Set class node (endpoint)
+df = df.dropna()
+DAG = bn.structure_learning.fit(df, methodtype='tan', class_node='threat_type')
+
+# Structure learning
+DAG = bn.independence_test(DAG, df, prune=True)
+# Plot
+G = bn.plot(DAG)
+G = bn.plot(DAG, interactive=True)
+# Parameter learning
+model = bn.parameter_learning.fit(DAG, df)
+# Make inference
+q1 = bn.inference.fit(model, variables=['threat_type'], evidence={'flee_status': 'foot'})
+q1 = bn.inference.fit(model, variables=['gender'], evidence={'threat_type': 'accident', 'armed_with': 'gun'})
+
+# No connection in the DAG, thus the evidence should not influence the outcome
+q1 = bn.inference.fit(model, variables=['body_camera'], evidence={'gender': 'male'})
+q1 = bn.inference.fit(model, variables=['body_camera'], evidence={'armed_with': 'gun'})
+
+print(q1)
+print(q1.df)
+# bn.print_CPD(model)
+
+# Create test dataset
+Xtest = bn.sampling(model, n=100)
+
+
+# %%
 import bnlearn as bn
 # Load asia DAG
 model = bn.import_DAG('asia')
 # plot ground truth
 G = bn.plot(model)
 
 Gi = bn.plot(model, interactive=True)
 
+bn.print_CPD(model)
+
+# Lets create an example dataset with 100 samples and make inferences on the entire dataset.
+df = bn.sampling(model, n=10000)
+
+
 # %% issue plot static vs dynamic is different
 import bnlearn as bn
 
 # Load example dataset
 df = bn.import_example('sprinkler')
 
 edges = [('Cloudy', 'Sprinkler'),
@@ -64,14 +172,15 @@
 Xy_train = Xy_train.dropna(axis=0)
 
 tarvar=['Survived']
 model = bn.structure_learning.fit(Xy_train, methodtype='tan', class_node = 'Survived')
 model = bn.parameter_learning.fit(model, Xy_train, methodtype='bayes', scoretype='bdeu')
 y_train_pred = bn.predict(model, Xy_train, variables = tarvar, verbose=4)
 
+
 # %% issue #84
 # Load library
 from pgmpy.factors.discrete import TabularCPD
 import bnlearn as bn
 
 # Create some edges, all starting from the same root node: A
 edges = [('A', 'B'), ('A', 'C'), ('A', 'D')]
@@ -90,15 +199,14 @@
 DAG = bn.make_DAG(DAG, CPD=[cpd_A, cpd_B, cpd_C, cpd_D], checkmodel=True)
 # Plot the CPDs as a sanity check
 bn.print_CPD(DAG, checkmodel=True)
 # Plot the DAG
 bn.plot(DAG)
 
 
-
 # %%
 import bnlearn as bn
 
 # Load example dataset
 df = bn.import_example('sprinkler')
 
 edges = [('Cloudy', 'Sprinkler'),
@@ -1164,33 +1272,46 @@
 # %% compute causalities
 # Load asia DAG
 df = bn.import_example('asia', verbose=0)
 # print(tabulate(df.head(), tablefmt="grid", headers="keys"))
 # print(df)
 
 # Structure learning
-model = bn.structure_learning.fit(df, verbose=0)
+model = bn.structure_learning.fit(df, verbose=0, scoretype='bic', methodtype='hc')
+model = bn.structure_learning.fit(df, verbose=0, scoretype='k2', methodtype='hc')
+
+# Plot the DAG
+bn.plot(model, verbose=0, interactive=True, node_color='#000000')
+
+# Test for independence
+model = bn.independence_test(model, df, prune=False)
+
 # Plot the DAG
 bn.plot(model, verbose=0, interactive=True, node_color='#000000')
 # Print the CPDs
 bn.print_CPD(model)
 # Comparison
 
 # Learn its parameters from data and perform the inference.
-DAG = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
+model_with_CPD = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
+model = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
 # Print the CPDs
-bn.print_CPD(DAG)
+bn.print_CPD(model_with_CPD)
 
 # Nothing is changed for the DAG. Only the CPDs are estimated now.
-bn.compare_networks(DAG, model, verbose=0)
+bn.compare_networks(model_with_CPD, model, verbose=0)
 
 # Make inference
-q4 = bn.inference.fit(DAG, variables=['bronc', 'lung'], evidence={'smoke': 1, 'xray': 0}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1, 'bronc':1}, verbose=3)
+q1 = bn.inference.fit(model_with_CPD, variables=['lung'], evidence={'smoke': 1, 'bronc':1, 'xray':1}, verbose=3)
+
+# q4 = bn.inference.fit(model_with_CPD, variables=['bronc', 'lung'], evidence={'smoke': 1, 'xray': 0}, verbose=3)
 # q4 = bn.inference.fit(DAG, variables=['bronc','lung','xray'], evidence={'smoke':1}, verbose=3)
-# q4 = bn.inference.fit(DAGnew, variables=['bronc','lung'], evidence={'smoke':0, 'xray':0})
+q1 = bn.inference.fit(model_with_CPD, variables=['xray'], evidence={'smoke':1})
 
 # pd.DataFrame(index=q4.variables, data=q4.values, columns=q4.variables)
 
 # %% Example compare networks
 # Load asia DAG
 DAG = bn.import_DAG('asia')
 # plot ground truth
@@ -1247,15 +1368,15 @@
 q2.values
 q2.variables
 q2.state_names
 q2.name_to_no
 q2.no_to_name,
 
 # %% LOAD BIF FILE
-DAG = bn.import_DAG('water', verbose=0)
+DAG = bn.import_DAG('asia', verbose=0)
 # Sampling
 df = bn.sampling(DAG, n=1000)
 # Parameter learning
 model = bn.parameter_learning.fit(DAG, df)
 G = bn.plot(model)
 
 # Test for independence
```

### Comparing `bnlearn-0.8.5/bnlearn/examples_discretize.py` & `bnlearn-0.8.6/bnlearn/examples_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/inference.py` & `bnlearn-0.8.6/bnlearn/inference.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/network.py` & `bnlearn-0.8.6/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/parameter_learning.py` & `bnlearn-0.8.6/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/structure_learning.py` & `bnlearn-0.8.6/bnlearn/structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/tests/discretize/test_discretize.py` & `bnlearn-0.8.6/bnlearn/tests/discretize/test_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py` & `bnlearn-0.8.6/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.6/bnlearn/tests/test_bnlearn.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.6/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.6/bnlearn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,21 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.5.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pgmpy>=0.1.18
-Requires-Dist: networkx>=2.7.1
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas==1.5.3
-Requires-Dist: d3blocks>=1.4.9
-Requires-Dist: tqdm
-Requires-Dist: ismember
-Requires-Dist: scikit-learn
-Requires-Dist: funcsigs
-Requires-Dist: statsmodels
-Requires-Dist: python-louvain
-Requires-Dist: packaging
-Requires-Dist: df2onehot
-Requires-Dist: fsspec
-Requires-Dist: pypickle
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: datazets
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,38 +1,32 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.5 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.6 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.5.tar.gz Author:
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.6.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist:
-d3blocks>=1.4.9 Requires-Dist: tqdm Requires-Dist: ismember Requires-Dist:
-scikit-learn Requires-Dist: funcsigs Requires-Dist: statsmodels Requires-Dist:
-python-louvain Requires-Dist: packaging Requires-Dist: df2onehot Requires-Dist:
-fsspec Requires-Dist: pypickle Requires-Dist: tabulate Requires-Dist:
-ipywidgets Requires-Dist: datazets # bnlearn - Library for Bayesian network
-learning and inference [![Python](https://img.shields.io/pypi/pyversions/
-bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version]
-(https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) !
-[GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://
-img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/
-bnlearn/network) [![Open Issues](https://img.shields.io/github/issues/erdogant/
-bnlearn.svg)](https://github.com/erdogant/bnlearn/issues) [![Project Status]
-(http://www.repostatus.org/badges/latest/active.svg)](http://
-www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/bnlearn/
-month)](https://pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/
-badge/bnlearn)](https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/
-badge/231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs]
-(https://img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-bnlearn/) [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
+www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
+#active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
+pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
+(https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
+231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
+img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
 erdogant.github.io/bnlearn/pages/html/Documentation.html#medium-blog) ![GitHub
 repo size](https://img.shields.io/github/repo-size/erdogant/bnlearn) [![Donate]
 (https://img.shields.io/badge/Support%20this%20project-
 grey.svg?logo=github%20sponsors)](https://erdogant.github.io/bnlearn/pages/
 html/Documentation.html#) [![Colab](https://colab.research.google.com/assets/
 colab-badge.svg)](https://erdogant.github.io/bnlearn/pages/html/
 Documentation.html#colab-notebook) ### ``bnlearn`` is Python package for
```

### Comparing `bnlearn-0.8.5/bnlearn.egg-info/SOURCES.txt` & `bnlearn-0.8.6/bnlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.5/setup.py` & `bnlearn-0.8.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     long_description = fh.read()
 setuptools.setup(
      install_requires=["pgmpy>=0.1.18",
                        "networkx>=2.7.1",
                        "matplotlib>=3.3.4",
                        "numpy>=1.24.1",
                        'pandas==1.5.3',
-                       'd3blocks>=1.4.9',
                        'tqdm',
                        'ismember',
                        'scikit-learn',
                        'funcsigs',
                        'statsmodels',
                        'python-louvain',
                        'packaging',
```

