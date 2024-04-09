# Comparing `tmp/fair_trees-2.3.3.tar.gz` & `tmp/fair_trees-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.3.tar", last modified: Tue Apr  9 15:45:05 2024, max compression
+gzip compressed data, was "fair_trees-2.3.4.tar", last modified: Tue Apr  9 15:57:39 2024, max compression
```

## Comparing `fair_trees-2.3.3.tar` & `fair_trees-2.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.577436 fair_trees-2.3.3/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.3/LICENSE
--rw-rw-rw-   0        0        0     4902 2024-04-09 15:45:05.577436 fair_trees-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2024-04-09 15:35:47.000000 fair_trees-2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.573335 fair_trees-2.3.3/fair_trees/
--rw-rw-rw-   0        0        0      210 2024-04-09 15:44:19.000000 fair_trees-2.3.3/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.3/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.576432 fair_trees-2.3.3/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4902 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 15:45:05.577436 fair_trees-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-04-09 15:45:00.000000 fair_trees-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.575883 fair_trees-2.3.4/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4912 2024-04-09 15:57:39.574883 fair_trees-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4350 2024-04-09 15:56:29.000000 fair_trees-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.569950 fair_trees-2.3.4/fair_trees/
+-rw-rw-rw-   0        0        0      210 2024-04-09 15:44:19.000000 fair_trees-2.3.4/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.4/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.574883 fair_trees-2.3.4/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4912 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:57:39.575883 fair_trees-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-04-09 15:57:31.000000 fair_trees-2.3.4/setup.py
```

### Comparing `fair_trees-2.3.3/LICENSE` & `fair_trees-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.3/PKG-INFO` & `fair_trees-2.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.3
+Version: 2.3.4
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -17,31 +17,31 @@
 # Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines,<br>use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
-A) <code>pip install fair-trees==2.0</code>
+A) <code>pip install fair-trees</code>
 
 or
 
-B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br> + <code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import *
+from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
-clf = FairRandomForestClassifier(theta=0.5).fit(X,y,z)
+clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
 ## Example
 ```python
 import joblib
 import numpy as np
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.3 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.4 Summary: This package
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
 into scikit-learn pipelines,
 use the fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
-Installation A) pip install fair-trees==2.0 or B) git clone https://github.com/
-pereirabarataap/fair_tree_classifier + pip install -r requirements.txt ## Usage
-```python import joblib from fair_trees import * datasets = joblib.load
+Installation A) pip install fair-trees or B) git clone https://github.com/
+pereirabarataap/fair_tree_classifier
++ pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
 ("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FairRandomForestClassifier
-(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ``` ## Example ```python
-import joblib import numpy as np import pandas as pd import seaborn as sb from
-tqdm.notebook import tqdm from matplotlib import pyplot as plt from
-sklearn.metrics import roc_auc_score from sklearn.model_selection import
-StratifiedKFold as SKF from fair_trees import FairRandomForestClassifier as
-FRFC, sdp_score datasets = joblib.load("datasets.pkl") results_data = [] for
-dataset in tqdm(datasets): X = datasets[dataset]["X"] y = datasets[dataset]
-["y"] z = datasets[dataset]["z"] fold = 0 skf = SKF(n_splits=5,
-random_state=42, shuffle=True) # ensuring stratified kfold w.r.t. y and z
-splitter_y = pd.concat([y, z], axis=1).astype(str).apply( lambda row: row
-[y.name] + "".join([row[col] for col in z.columns]), axis=1 ).values desc_i =
-f"dataset={dataset} | processing folds" for train_idx, test_idx in tqdm
-(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train, X_test = X.loc
-[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx], y.loc
-[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j = f"fold=
-{fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
+sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
+FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
+("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
+skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
+kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
+( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
+).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
+test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
+X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
+y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
+f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
 desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
 max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
 min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
```

### Comparing `fair_trees-2.3.3/README.md` & `fair_trees-2.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines,<br>use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
-A) <code>pip install fair-trees==2.0</code>
+A) <code>pip install fair-trees</code>
 
 or
 
-B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br> + <code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import *
+from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
-clf = FairRandomForestClassifier(theta=0.5).fit(X,y,z)
+clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
 ## Example
 ```python
 import joblib
 import numpy as np
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
 # Fair tree classifier using strong demographic parity _[_>_>_] This package learns
 fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. When incorporating
 FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
 learn pipelines,
 use the fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
-Installation A) pip install fair-trees==2.0 or B) git clone https://github.com/
-pereirabarataap/fair_tree_classifier + pip install -r requirements.txt ## Usage
-```python import joblib from fair_trees import * datasets = joblib.load
+Installation A) pip install fair-trees or B) git clone https://github.com/
+pereirabarataap/fair_tree_classifier
++ pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
 ("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FairRandomForestClassifier
-(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ``` ## Example ```python
-import joblib import numpy as np import pandas as pd import seaborn as sb from
-tqdm.notebook import tqdm from matplotlib import pyplot as plt from
-sklearn.metrics import roc_auc_score from sklearn.model_selection import
-StratifiedKFold as SKF from fair_trees import FairRandomForestClassifier as
-FRFC, sdp_score datasets = joblib.load("datasets.pkl") results_data = [] for
-dataset in tqdm(datasets): X = datasets[dataset]["X"] y = datasets[dataset]
-["y"] z = datasets[dataset]["z"] fold = 0 skf = SKF(n_splits=5,
-random_state=42, shuffle=True) # ensuring stratified kfold w.r.t. y and z
-splitter_y = pd.concat([y, z], axis=1).astype(str).apply( lambda row: row
-[y.name] + "".join([row[col] for col in z.columns]), axis=1 ).values desc_i =
-f"dataset={dataset} | processing folds" for train_idx, test_idx in tqdm
-(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train, X_test = X.loc
-[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx], y.loc
-[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j = f"fold=
-{fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
+sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
+FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
+("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
+skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
+kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
+( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
+).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
+test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
+X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
+y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
+f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
 desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
 max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
 min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
```

### Comparing `fair_trees-2.3.3/fair_trees/fair_trees.py` & `fair_trees-2.3.4/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.3/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.3.4/fair_trees.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.3
+Version: 2.3.4
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -17,31 +17,31 @@
 # Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines,<br>use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
 ## Installation
-A) <code>pip install fair-trees==2.0</code>
+A) <code>pip install fair-trees</code>
 
 or
 
-B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code> + <code>pip install -r requirements.txt</code>
+B) <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br> + <code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import *
+from fair_trees import FairRandomForestClassifier as FRFC
 
 datasets = joblib.load("datasets.pkl")
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
-clf = FairRandomForestClassifier(theta=0.5).fit(X,y,z)
+clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
 ## Example
 ```python
 import joblib
 import numpy as np
 import pandas as pd
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.3 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.4 Summary: This package
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
 into scikit-learn pipelines,
 use the fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
-Installation A) pip install fair-trees==2.0 or B) git clone https://github.com/
-pereirabarataap/fair_tree_classifier + pip install -r requirements.txt ## Usage
-```python import joblib from fair_trees import * datasets = joblib.load
+Installation A) pip install fair-trees or B) git clone https://github.com/
+pereirabarataap/fair_tree_classifier
++ pip install -r requirements.txt ## Usage ```python import joblib from
+fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
 ("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FairRandomForestClassifier
-(theta=0.5).fit(X,y,z) y_proba = clf.predict_proba(X) ``` ## Example ```python
-import joblib import numpy as np import pandas as pd import seaborn as sb from
-tqdm.notebook import tqdm from matplotlib import pyplot as plt from
-sklearn.metrics import roc_auc_score from sklearn.model_selection import
-StratifiedKFold as SKF from fair_trees import FairRandomForestClassifier as
-FRFC, sdp_score datasets = joblib.load("datasets.pkl") results_data = [] for
-dataset in tqdm(datasets): X = datasets[dataset]["X"] y = datasets[dataset]
-["y"] z = datasets[dataset]["z"] fold = 0 skf = SKF(n_splits=5,
-random_state=42, shuffle=True) # ensuring stratified kfold w.r.t. y and z
-splitter_y = pd.concat([y, z], axis=1).astype(str).apply( lambda row: row
-[y.name] + "".join([row[col] for col in z.columns]), axis=1 ).values desc_i =
-f"dataset={dataset} | processing folds" for train_idx, test_idx in tqdm
-(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train, X_test = X.loc
-[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx], y.loc
-[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j = f"fold=
-{fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
+clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
+import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
+matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
+sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
+FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
+("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
+skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
+kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
+( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
+).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
+test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
+X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
+y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
+f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
 desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
 max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
 min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
```

### Comparing `fair_trees-2.3.3/setup.py` & `fair_trees-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.3.3",
+    version="2.3.4",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

