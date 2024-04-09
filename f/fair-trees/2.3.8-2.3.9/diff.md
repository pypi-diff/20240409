# Comparing `tmp/fair_trees-2.3.8.tar.gz` & `tmp/fair_trees-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.8.tar", last modified: Tue Apr  9 16:09:03 2024, max compression
+gzip compressed data, was "fair_trees-2.3.9.tar", last modified: Tue Apr  9 16:13:10 2024, max compression
```

## Comparing `fair_trees-2.3.8.tar` & `fair_trees-2.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.861152 fair_trees-2.3.8/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.8/LICENSE
--rw-rw-rw-   0        0        0     4912 2024-04-09 16:09:03.860152 fair_trees-2.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     4350 2024-04-09 16:07:42.000000 fair_trees-2.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.856072 fair_trees-2.3.8/fair_trees/
--rw-rw-rw-   0        0        0       91 2024-04-09 16:08:52.000000 fair_trees-2.3.8/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.8/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:09:03.860152 fair_trees-2.3.8/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4912 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 16:09:03.000000 fair_trees-2.3.8/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:09:03.861152 fair_trees-2.3.8/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-04-09 16:07:26.000000 fair_trees-2.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.986160 fair_trees-2.3.9/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0     4916 2024-04-09 16:13:10.985160 fair_trees-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4354 2024-04-09 16:10:08.000000 fair_trees-2.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.980151 fair_trees-2.3.9/fair_trees/
+-rw-rw-rw-   0        0        0       91 2024-04-09 16:10:52.000000 fair_trees-2.3.9/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.9/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.985160 fair_trees-2.3.9/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4916 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:13:10.986160 fair_trees-2.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-04-09 16:13:03.000000 fair_trees-2.3.9/setup.py
```

### Comparing `fair_trees-2.3.8/LICENSE` & `fair_trees-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.8/PKG-INFO` & `fair_trees-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.8
+Version: 2.3.9
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
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.8 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.9 Summary: This package
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
-git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
-r requirements.txt ## Usage ```python import joblib from fair_trees import
-FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
-datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
-["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
-## Example ```python import joblib import numpy as np import pandas as pd
-import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
-pyplot as plt from sklearn.metrics import roc_auc_score from
+git clone https://github.com/pereirabarataap/fair_tree_classifier
+pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
+("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
 FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
 ("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
```

### Comparing `fair_trees-2.3.8/README.md` & `fair_trees-2.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Installation
 A)<br>
 <code>pip install fair-trees</code>
 
 or
 
 B)<br>
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 # Fair tree classifier using strong demographic parity _[_>_>_] This package learns
 fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. When incorporating
 FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
 learn pipelines, use the fit_params={"z": z} parameter to pass the sensitive
 attribute(s) z ## Installation A)
 pip install fair-trees or B)
-git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
-r requirements.txt ## Usage ```python import joblib from fair_trees import
-FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
-datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
-["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
-## Example ```python import joblib import numpy as np import pandas as pd
-import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
-pyplot as plt from sklearn.metrics import roc_auc_score from
+git clone https://github.com/pereirabarataap/fair_tree_classifier
+pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
+("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
 FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
 ("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
```

### Comparing `fair_trees-2.3.8/fair_trees/fair_trees.py` & `fair_trees-2.3.9/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.8/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.3.9/fair_trees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.8
+Version: 2.3.9
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
-<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><code>pip install -r requirements.txt</code>
+<code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
 from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.8 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.9 Summary: This package
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
-git clone https://github.com/pereirabarataap/fair_tree_classifierpip install -
-r requirements.txt ## Usage ```python import joblib from fair_trees import
-FairRandomForestClassifier as FRFC datasets = joblib.load("datasets.pkl") X =
-datasets["adult"]["X"] y = datasets["adult"]["y"] z = datasets["adult"]["z"]
-["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ```
-## Example ```python import joblib import numpy as np import pandas as pd
-import seaborn as sb from tqdm.notebook import tqdm from matplotlib import
-pyplot as plt from sklearn.metrics import roc_auc_score from
+git clone https://github.com/pereirabarataap/fair_tree_classifier
+pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
+("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
 FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
 ("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
```

### Comparing `fair_trees-2.3.8/setup.py` & `fair_trees-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.3.8",
+    version="2.3.9",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

