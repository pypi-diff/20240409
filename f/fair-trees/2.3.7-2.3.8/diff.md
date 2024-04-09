# Comparing `tmp/fair_trees-2.3.7.tar.gz` & `tmp/fair_trees-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.7.tar", last modified: Tue Apr  9 16:06:40 2024, max compression
+gzip compressed data, was "fair_trees-2.3.8.tar", last modified: Tue Apr  9 16:09:03 2024, max compression
```

## Comparing `fair_trees-2.3.7.tar` & `fair_trees-2.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:06:40.078962 fair_trees-2.3.7/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.7/LICENSE
--rw-rw-rw-   0        0        0     4915 2024-04-09 16:06:40.077958 fair_trees-2.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     4353 2024-04-09 16:05:19.000000 fair_trees-2.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:06:40.072962 fair_trees-2.3.7/fair_trees/
--rw-rw-rw-   0        0        0       90 2024-04-09 16:03:46.000000 fair_trees-2.3.7/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.7/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:06:40.077958 fair_trees-2.3.7/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4915 2024-04-09 16:06:40.000000 fair_trees-2.3.7/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 16:06:40.000000 fair_trees-2.3.7/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:06:40.000000 fair_trees-2.3.7/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 16:06:40.000000 fair_trees-2.3.7/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 16:06:40.000000 fair_trees-2.3.7/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:06:40.078962 fair_trees-2.3.7/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-04-09 16:06:26.000000 fair_trees-2.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.861152 fair_trees-2.3.8/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.8/LICENSE
+-rw-rw-rw-   0        0        0     4912 2024-04-09 16:09:03.860152 fair_trees-2.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4350 2024-04-09 16:07:42.000000 fair_trees-2.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.856072 fair_trees-2.3.8/fair_trees/
+-rw-rw-rw-   0        0        0       91 2024-04-09 16:08:52.000000 fair_trees-2.3.8/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.8/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.860152 fair_trees-2.3.8/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4912 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:09:03.861152 fair_trees-2.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-04-09 16:07:26.000000 fair_trees-2.3.8/setup.py
```

### Comparing `fair_trees-2.3.7/LICENSE` & `fair_trees-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.7/PKG-INFO` & `fair_trees-2.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.7
+Version: 2.3.8
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -23,15 +23,15 @@
 ## Installation
 A)<br>
 <code>pip install fair-trees</code>
 
 or
 
 B)<br>
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.7 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.8 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
 package learns fair decision tree classifiers which can then be bagged into
 fair random forests, following the scikit-learn API standards. When
 incorporating FairDecisionTreeClassifier or FairRandomForestClassifier objects
 into scikit-learn pipelines, use the fit_params={"z": z} parameter to pass the
 sensitive attribute(s) z ## Installation A)
 pip install fair-trees or B)
-git clone https://github.com/pereirabarataap/fair_tree_classifier + pip install
--r requirements.txt ## Usage ```python import joblib from fair_trees import
+git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
+r requirements.txt ## Usage ```python import joblib from fair_trees import
 FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
 datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
 ["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
 ## Example ```python import joblib import numpy as np import pandas as pd
 import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
 pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
```

### Comparing `fair_trees-2.3.7/README.md` & `fair_trees-2.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Installation
 A)<br>
 <code>pip install fair-trees</code>
 
 or
 
 B)<br>
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 # Fair tree classifier using strong demographic parity _[_>_>_] This package learns
 fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. When incorporating
 FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
 learn pipelines, use the fit_params={"z": z} parameter to pass the sensitive
 attribute(s) z ## Installation A)
 pip install fair-trees or B)
-git clone https://github.com/pereirabarataap/fair_tree_classifier + pip install
--r requirements.txt ## Usage ```python import joblib from fair_trees import
+git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
+r requirements.txt ## Usage ```python import joblib from fair_trees import
 FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
 datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
 ["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
 ## Example ```python import joblib import numpy as np import pandas as pd
 import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
 pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
```

### Comparing `fair_trees-2.3.7/fair_trees/fair_trees.py` & `fair_trees-2.3.8/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.7/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.3.8/fair_trees.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.7
+Version: 2.3.8
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -23,15 +23,15 @@
 ## Installation
 A)<br>
 <code>pip install fair-trees</code>
 
 or
 
 B)<br>
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.7 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.8 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
 package learns fair decision tree classifiers which can then be bagged into
 fair random forests, following the scikit-learn API standards. When
 incorporating FairDecisionTreeClassifier or FairRandomForestClassifier objects
 into scikit-learn pipelines, use the fit_params={"z": z} parameter to pass the
 sensitive attribute(s) z ## Installation A)
 pip install fair-trees or B)
-git clone https://github.com/pereirabarataap/fair_tree_classifier + pip install
--r requirements.txt ## Usage ```python import joblib from fair_trees import
+git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
+r requirements.txt ## Usage ```python import joblib from fair_trees import
 FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
 datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
 ["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
 ## Example ```python import joblib import numpy as np import pandas as pd
 import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
 pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
```

### Comparing `fair_trees-2.3.7/setup.py` & `fair_trees-2.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.3.7",
+    version="2.3.8",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

