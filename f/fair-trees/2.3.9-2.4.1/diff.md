# Comparing `tmp/fair_trees-2.3.9.tar.gz` & `tmp/fair_trees-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.9.tar", last modified: Tue Apr  9 16:13:10 2024, max compression
+gzip compressed data, was "fair_trees-2.4.1.tar", last modified: Tue Apr  9 16:58:01 2024, max compression
```

## Comparing `fair_trees-2.3.9.tar` & `fair_trees-2.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.986160 fair_trees-2.3.9/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.9/LICENSE
--rw-rw-rw-   0        0        0     4916 2024-04-09 16:13:10.985160 fair_trees-2.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     4354 2024-04-09 16:10:08.000000 fair_trees-2.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.980151 fair_trees-2.3.9/fair_trees/
--rw-rw-rw-   0        0        0       91 2024-04-09 16:10:52.000000 fair_trees-2.3.9/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.9/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:13:10.985160 fair_trees-2.3.9/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4916 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 16:13:10.000000 fair_trees-2.3.9/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:13:10.986160 fair_trees-2.3.9/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-04-09 16:13:03.000000 fair_trees-2.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.650777 fair_trees-2.4.1/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     4892 2024-04-09 16:58:01.649725 fair_trees-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4360 2024-04-09 16:57:32.000000 fair_trees-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.644990 fair_trees-2.4.1/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.1/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.1/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.649725 fair_trees-2.4.1/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4892 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:58:01.650777 fair_trees-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-09 16:57:52.000000 fair_trees-2.4.1/setup.py
```

### Comparing `fair_trees-2.3.9/LICENSE` & `fair_trees-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.9/PKG-INFO` & `fair_trees-2.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.9
+Version: 2.4.1
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
-Requires-Dist: requests_mock
 
 # Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines, use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
@@ -28,17 +27,17 @@
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import FairRandomForestClassifier as FRFC
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
@@ -48,17 +47,17 @@
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
-from fair_trees import FairRandomForestClassifier as FRFC, sdp_score
+from fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 
 results_data = []
 for dataset in tqdm(datasets):
     X = datasets[dataset]["X"]
     y = datasets[dataset]["y"]
     z = datasets[dataset]["z"]
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.9 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.1 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
-requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
-package learns fair decision tree classifiers which can then be bagged into
-fair random forests, following the scikit-learn API standards. When
-incorporating FairDecisionTreeClassifier or FairRandomForestClassifier objects
-into scikit-learn pipelines, use the fit_params={"z": z} parameter to pass the
-sensitive attribute(s) z ## Installation A)
+pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
+using strong demographic parity _[_>_>_] This package learns fair decision tree
+classifiers which can then be bagged into fair random forests, following the
+scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
+FairRandomForestClassifier objects into scikit-learn pipelines, use the
+fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
+Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
-("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
 clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
 import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
 matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
-("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
+load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
 ).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
 test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
 X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
```

### Comparing `fair_trees-2.3.9/README.md` & `fair_trees-2.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import FairRandomForestClassifier as FRFC
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
@@ -32,17 +32,17 @@
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
-from fair_trees import FairRandomForestClassifier as FRFC, sdp_score
+from fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 
 results_data = []
 for dataset in tqdm(datasets):
     X = datasets[dataset]["X"]
     y = datasets[dataset]["y"]
     z = datasets[dataset]["z"]
```

#### html2text {}

```diff
@@ -3,23 +3,23 @@
 forests, following the scikit-learn API standards. When incorporating
 FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
 learn pipelines, use the fit_params={"z": z} parameter to pass the sensitive
 attribute(s) z ## Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
-("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
 clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
 import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
 matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
-("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
+load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
 ).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
 test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
 X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
```

### Comparing `fair_trees-2.3.9/fair_trees/fair_trees.py` & `fair_trees-2.4.1/fair_trees/fair_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from sklearn.metrics import roc_auc_score, f1_score
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.preprocessing import OneHotEncoder as OHE, KBinsDiscretizer as KBD
 
 pd.set_option("future.no_silent_downcasting", True)
 warnings.filterwarnings("ignore", category=UserWarning)
 
+def load_datasets():
+    return joblib.load("datasets.pkl")
+
 def sdp_score(z_true, y_prob):
     """
     Strong Demographic Parity Score
     Same API as roc_auc_score from sklean.metric
     Returns a value between 0 and 1 in which:
         0 indicates complete algorithmic bias,
         1 indicates complete algorithmic fairness
@@ -103,23 +106,25 @@
         max_depth=None,
         bootstrap=False,
         random_state=42,
         max_features=None, 
         min_samples_leaf=1, 
         min_samples_split=2, 
         requires_data_processing=True,
+        generate_prediction_threshold=True,
     ):
         self.theta = theta
         self.n_bins=n_bins
         self.bootstrap = bootstrap
         self.max_features = max_features
         self.random_state = random_state
         self.min_samples_leaf = min_samples_leaf
         self.min_samples_split = min_samples_split
         self.requires_data_processing = requires_data_processing
+        self.generate_prediction_threshold = generate_prediction_threshold
         if isinstance(max_depth, type(None)):
             self.max_depth = np.inf
         else:
             self.max_depth = max_depth
             
         np.random.seed(self.random_state)
         self.parent_scaff = (1-self.theta)*0.5 - self.theta*0.5
@@ -368,21 +373,22 @@
         
         if self.bootstrap:
             resample_idx = np.random.choice(len(y), len(y), replace=True)
             X, y, z = X[resample_idx], y[resample_idx], z[resample_idx]
         
         self.tree_ = self._grow_tree(X, y, z)
         
-        if self.requires_data_processing:
-            # was already processed
-            self.requires_data_processing = False
-            self.prediction_threshold = self._prediction_threshold(X, y)
-            self.requires_data_processing = True
-        else:
-            self.prediction_threshold = self._prediction_threshold(X, y)
+        if self.generate_prediction_threshold:
+            if self.requires_data_processing:
+                # was already processed
+                self.requires_data_processing = False
+                self.prediction_threshold = self._prediction_threshold(X, y)
+                self.requires_data_processing = True
+            else:
+                self.prediction_threshold = self._prediction_threshold(X, y)
             
         return self
         
     def _predict_proba(self, node, X):
         num_samples = len(X)
         probabilities = np.empty((num_samples, self.n_classes_))
         stack = [(node, np.arange(num_samples))]  # Convert slice to list of indices
@@ -459,27 +465,29 @@
         bootstrap=True,
         random_state=42,
         n_estimators=500,
         min_samples_leaf=1, 
         min_samples_split=2,
         max_features="sqrt",
         requires_data_processing=True,
+        generate_prediction_threshold=True
     ):
         # forest-specific
         self.n_jobs = n_jobs
         self.n_estimators = n_estimators
         # tree-specific
         self.theta = theta
         self.n_bins=n_bins
         self.bootstrap = bootstrap
         self.max_features = max_features
         self.random_state = random_state
         self.min_samples_leaf = min_samples_leaf
         self.min_samples_split = min_samples_split
         self.requires_data_processing = requires_data_processing
+        self.generate_prediction_threshold=generate_prediction_threshold
         if isinstance(max_depth, type(None)):
             self.max_depth = np.inf
         else:
             self.max_depth = max_depth
             
         np.random.seed(self.random_state)
         
@@ -488,14 +496,15 @@
             theta=self.theta,
             n_bins=self.n_bins,
             random_state=base_rs+i,
             max_depth=self.max_depth,
             bootstrap=self.bootstrap,
             max_features=self.max_features,
             requires_data_processing=False,
+            generate_prediction_threshold=False,
             min_samples_leaf=self.min_samples_leaf,
             min_samples_split=self.min_samples_split,
         ) for i in range(n_estimators)]
     
     def _fit_trees_batch(self, tree_indices, X, y, z):
         fitted_trees_batch = []
         for i in tree_indices:
@@ -600,21 +609,22 @@
         # Fit trees in batches in parallel
         trees_batches = Parallel(n_jobs=n_jobs)(
             delayed(self._fit_trees_batch)(batch, X, y, z) for batch in batches)
         
         # Flatten the list of trees
         self.fitted_trees = [tree for batch in trees_batches for tree in batch]
         
-        if self.requires_data_processing:
-            # was already processed
-            self.requires_data_processing = False
-            self.prediction_threshold = self._prediction_threshold(X, y)
-            self.requires_data_processing = True
-        else:
-            self.prediction_threshold = self._prediction_threshold(X, y)
+        if self.generate_prediction_threshold:
+            if self.requires_data_processing:
+                # was already processed
+                self.requires_data_processing = False
+                self.prediction_threshold = self._prediction_threshold(X, y)
+                self.requires_data_processing = True
+            else:
+                self.prediction_threshold = self._prediction_threshold(X, y)
             
         return self
     
     def predict(self, X):
         y_proba = self.predict_proba(X)
         predictions = (y_proba[:,1] >= self.prediction_threshold).astype(int)
         return predictions
```

### Comparing `fair_trees-2.3.9/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.1/fair_trees.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.9
+Version: 2.4.1
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: joblib
 Requires-Dist: scikit-learn
-Requires-Dist: requests_mock
 
 # Fair tree classifier using strong demographic parity <a href="https://link.springer.com/article/10.1007/s10994-023-06376-z" target="blank">[>>]</a>
 
 This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 
 When incorporating <code>FairDecisionTreeClassifier</code> or <code>FairRandomForestClassifier</code> objects into scikit-learn pipelines, use the <code>fit_params={"z": z}</code> parameter to pass the sensitive attribute(s) <code>z</code>
 
@@ -28,17 +27,17 @@
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
 import joblib
-from fair_trees import FairRandomForestClassifier as FRFC
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
 y_proba = clf.predict_proba(X)
 ```
@@ -48,17 +47,17 @@
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
-from fair_trees import FairRandomForestClassifier as FRFC, sdp_score
+from fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
 
-datasets = joblib.load("datasets.pkl")
+datasets = load_datasets()
 
 results_data = []
 for dataset in tqdm(datasets):
     X = datasets[dataset]["X"]
     y = datasets[dataset]["y"]
     z = datasets[dataset]["z"]
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.9 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.1 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
-pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
-requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
-package learns fair decision tree classifiers which can then be bagged into
-fair random forests, following the scikit-learn API standards. When
-incorporating FairDecisionTreeClassifier or FairRandomForestClassifier objects
-into scikit-learn pipelines, use the fit_params={"z": z} parameter to pass the
-sensitive attribute(s) z ## Installation A)
+pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
+using strong demographic parity _[_>_>_] This package learns fair decision tree
+classifiers which can then be bagged into fair random forests, following the
+scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
+FairRandomForestClassifier objects into scikit-learn pipelines, use the
+fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
+Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
 pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC datasets = joblib.load
-("datasets.pkl") X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
+fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
 datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
 clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
 import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
 matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
 sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score datasets = joblib.load
-("datasets.pkl") results_data = [] for dataset in tqdm(datasets): X = datasets
+FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
+load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
 [dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
 kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
 ( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
 ).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
 test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
 X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
```

### Comparing `fair_trees-2.3.9/setup.py` & `fair_trees-2.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.3.9",
+    version="2.4.1",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
     install_requires=[
         "scipy",
         "numpy",
         "pandas",
         "joblib",
-        "scikit-learn",
-        "requests_mock"
+        "scikit-learn"
     ],
 )
```

