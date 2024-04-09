# Comparing `tmp/fair_trees-2.4.1.tar.gz` & `tmp/fair_trees-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.4.1.tar", last modified: Tue Apr  9 16:58:01 2024, max compression
+gzip compressed data, was "fair_trees-2.4.2.tar", last modified: Tue Apr  9 17:26:55 2024, max compression
```

## Comparing `fair_trees-2.4.1.tar` & `fair_trees-2.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.650777 fair_trees-2.4.1/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.1/LICENSE
--rw-rw-rw-   0        0        0     4892 2024-04-09 16:58:01.649725 fair_trees-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4360 2024-04-09 16:57:32.000000 fair_trees-2.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.644990 fair_trees-2.4.1/fair_trees/
--rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.1/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.1/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:01.649725 fair_trees-2.4.1/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4892 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 16:58:01.000000 fair_trees-2.4.1/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:58:01.650777 fair_trees-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-04-09 16:57:52.000000 fair_trees-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.776878 fair_trees-2.4.2/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.4.2/LICENSE
+-rw-rw-rw-   0        0        0     4900 2024-04-09 17:26:55.775827 fair_trees-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4368 2024-04-09 17:26:21.000000 fair_trees-2.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.769837 fair_trees-2.4.2/fair_trees/
+-rw-rw-rw-   0        0        0      106 2024-04-09 16:17:37.000000 fair_trees-2.4.2/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    27184 2024-04-09 16:55:06.000000 fair_trees-2.4.2/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:26:55.775827 fair_trees-2.4.2/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4900 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 17:26:55.000000 fair_trees-2.4.2/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:26:55.776878 fair_trees-2.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-04-09 17:26:48.000000 fair_trees-2.4.2/setup.py
```

### Comparing `fair_trees-2.4.1/LICENSE` & `fair_trees-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.1/PKG-INFO` & `fair_trees-2.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.1
+Version: 2.4.2
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -26,28 +26,27 @@
 or
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
-import joblib
-from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets, sdp_score
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_proba = clf.predict_proba(X)
+y_prob = clf.predict_proba(X)
+print(sdp_sore(z, y_prob))
 ```
 ## Example
 ```python
-import joblib
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.1 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.2 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
-pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+pip install -r requirements.txt ## Usage ```python from fair_trees import
+FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
-clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
-import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
-matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
-sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
-load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
-[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
-skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
-kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
-( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
-).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
-test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
-X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
-y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
-f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
-desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
-max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
-min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
+clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
+numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
+tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
+fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
+datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
+datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
+fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
+stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
+(str).apply( lambda row: row[y.name] + "".join([row[col] for col in
+z.columns]), axis=1 ).values desc_i = f"dataset={dataset} | processing folds"
+for train_idx, test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i,
+leave=False): X_train, X_test = X.loc[train_idx], X.loc[test_idx] y_train,
+y_test = y.loc[train_idx], y.loc[test_idx] z_train, z_test = z.loc[train_idx],
+z.loc[test_idx] desc_j = f"fold={fold} | fitting thetas" for theta in tqdm
+(np.linspace(0,1,11).round(1), desc=desc_j, leave=False): clf = FRFC( n_jobs=-
+1, n_bins=256, theta=theta, max_depth=None, bootstrap=True, random_state=42,
+n_estimators=500, min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp else: for
 sens_val in np.unique(z_test[sens_att]): z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp data_row =
```

### Comparing `fair_trees-2.4.1/README.md` & `fair_trees-2.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,27 @@
 or
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
-import joblib
-from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets, sdp_score
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_proba = clf.predict_proba(X)
+y_prob = clf.predict_proba(X)
+print(sdp_sore(z, y_prob))
 ```
 ## Example
 ```python
-import joblib
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
```

#### html2text {}

```diff
@@ -2,36 +2,36 @@
 fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. When incorporating
 FairDecisionTreeClassifier or FairRandomForestClassifier objects into scikit-
 learn pipelines, use the fit_params={"z": z} parameter to pass the sensitive
 attribute(s) z ## Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
-pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+pip install -r requirements.txt ## Usage ```python from fair_trees import
+FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
-clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
-import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
-matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
-sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
-load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
-[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
-skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
-kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
-( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
-).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
-test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
-X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
-y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
-f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
-desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
-max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
-min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
+clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
+numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
+tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
+fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
+datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
+datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
+fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
+stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
+(str).apply( lambda row: row[y.name] + "".join([row[col] for col in
+z.columns]), axis=1 ).values desc_i = f"dataset={dataset} | processing folds"
+for train_idx, test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i,
+leave=False): X_train, X_test = X.loc[train_idx], X.loc[test_idx] y_train,
+y_test = y.loc[train_idx], y.loc[test_idx] z_train, z_test = z.loc[train_idx],
+z.loc[test_idx] desc_j = f"fold={fold} | fitting thetas" for theta in tqdm
+(np.linspace(0,1,11).round(1), desc=desc_j, leave=False): clf = FRFC( n_jobs=-
+1, n_bins=256, theta=theta, max_depth=None, bootstrap=True, random_state=42,
+n_estimators=500, min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp else: for
 sens_val in np.unique(z_test[sens_att]): z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp data_row =
```

### Comparing `fair_trees-2.4.1/fair_trees/fair_trees.py` & `fair_trees-2.4.2/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.4.1/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.4.2/fair_trees.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.4.1
+Version: 2.4.2
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
@@ -26,28 +26,27 @@
 or
 
 B)<br>
 <code>git clone https://github.com/pereirabarataap/fair_tree_classifier</code><br><code>pip install -r requirements.txt</code>
 
 ## Usage
 ```python
-import joblib
-from fair_trees import FairRandomForestClassifier as FRFC, load_datasets
+from fair_trees import FairRandomForestClassifier as FRFC, load_datasets, sdp_score
 
 datasets = load_datasets()
 X = datasets["adult"]["X"]
 y = datasets["adult"]["y"]
 z = datasets["adult"]["z"]["gender"]
 
 clf = FRFC(theta=0.5).fit(X,y,z)
-y_proba = clf.predict_proba(X)
+y_prob = clf.predict_proba(X)
+print(sdp_sore(z, y_prob))
 ```
 ## Example
 ```python
-import joblib
 import numpy as np
 import pandas as pd
 import seaborn as sb
 from tqdm.notebook import tqdm
 from matplotlib import pyplot as plt
 from sklearn.metrics import roc_auc_score
 from sklearn.model_selection import StratifiedKFold as SKF
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.4.1 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.4.2 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn # Fair tree classifier
 using strong demographic parity _[_>_>_] This package learns fair decision tree
 classifiers which can then be bagged into fair random forests, following the
 scikit-learn API standards. When incorporating FairDecisionTreeClassifier or
 FairRandomForestClassifier objects into scikit-learn pipelines, use the
 fit_params={"z": z} parameter to pass the sensitive attribute(s) z ##
 Installation A)
 pip install fair-trees or B)
 git clone https://github.com/pereirabarataap/fair_tree_classifier
-pip install -r requirements.txt ## Usage ```python import joblib from
-fair_trees import FairRandomForestClassifier as FRFC, load_datasets datasets =
+pip install -r requirements.txt ## Usage ```python from fair_trees import
+FairRandomForestClassifier as FRFC, load_datasets, sdp_score datasets =
 load_datasets() X = datasets["adult"]["X"] y = datasets["adult"]["y"] z =
-datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_proba =
-clf.predict_proba(X) ``` ## Example ```python import joblib import numpy as np
-import pandas as pd import seaborn as sb from tqdm.notebook import tqdm from
-matplotlib import pyplot as plt from sklearn.metrics import roc_auc_score from
-sklearn.model_selection import StratifiedKFold as SKF from fair_trees import
-FairRandomForestClassifier as FRFC, sdp_score, load_datasets datasets =
-load_datasets() results_data = [] for dataset in tqdm(datasets): X = datasets
-[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"] fold = 0
-skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring stratified
-kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype(str).apply
-( lambda row: row[y.name] + "".join([row[col] for col in z.columns]), axis=1
-).values desc_i = f"dataset={dataset} | processing folds" for train_idx,
-test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i, leave=False): X_train,
-X_test = X.loc[train_idx], X.loc[test_idx] y_train, y_test = y.loc[train_idx],
-y.loc[test_idx] z_train, z_test = z.loc[train_idx], z.loc[test_idx] desc_j =
-f"fold={fold} | fitting thetas" for theta in tqdm(np.linspace(0,1,11).round(1),
-desc=desc_j, leave=False): clf = FRFC( n_jobs=-1, n_bins=256, theta=theta,
-max_depth=None, bootstrap=True, random_state=42, n_estimators=500,
-min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
+datasets["adult"]["z"]["gender"] clf = FRFC(theta=0.5).fit(X,y,z) y_prob =
+clf.predict_proba(X) print(sdp_sore(z, y_prob)) ``` ## Example ```python import
+numpy as np import pandas as pd import seaborn as sb from tqdm.notebook import
+tqdm from matplotlib import pyplot as plt from sklearn.metrics import
+roc_auc_score from sklearn.model_selection import StratifiedKFold as SKF from
+fair_trees import FairRandomForestClassifier as FRFC, sdp_score, load_datasets
+datasets = load_datasets() results_data = [] for dataset in tqdm(datasets): X =
+datasets[dataset]["X"] y = datasets[dataset]["y"] z = datasets[dataset]["z"]
+fold = 0 skf = SKF(n_splits=5, random_state=42, shuffle=True) # ensuring
+stratified kfold w.r.t. y and z splitter_y = pd.concat([y, z], axis=1).astype
+(str).apply( lambda row: row[y.name] + "".join([row[col] for col in
+z.columns]), axis=1 ).values desc_i = f"dataset={dataset} | processing folds"
+for train_idx, test_idx in tqdm(skf.split(X,splitter_y), desc=desc_i,
+leave=False): X_train, X_test = X.loc[train_idx], X.loc[test_idx] y_train,
+y_test = y.loc[train_idx], y.loc[test_idx] z_train, z_test = z.loc[train_idx],
+z.loc[test_idx] desc_j = f"fold={fold} | fitting thetas" for theta in tqdm
+(np.linspace(0,1,11).round(1), desc=desc_j, leave=False): clf = FRFC( n_jobs=-
+1, n_bins=256, theta=theta, max_depth=None, bootstrap=True, random_state=42,
+n_estimators=500, min_samples_leaf=1, min_samples_split=2, max_features="sqrt",
 requires_data_processing=True ).fit(X_train, y_train, z_train) y_prob =
 clf.predict_proba(X_test)[:,1] auc = roc_auc_score(y_test, y_prob) sdp_min =
 np.inf for sens_att in z.columns: if len(np.unique(z_test[sens_att]))==2:
 sens_val = np.unique(z_test[sens_att])[0] z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp else: for
 sens_val in np.unique(z_test[sens_att]): z_true = z_test[sens_att]==sens_val
 sdp = sdp_score(z_true, y_prob) if sdp < sdp_min: sdp_min = sdp data_row =
```

### Comparing `fair_trees-2.4.1/setup.py` & `fair_trees-2.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.4.1",
+    version="2.4.2",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

