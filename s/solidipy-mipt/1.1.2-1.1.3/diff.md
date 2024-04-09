# Comparing `tmp/solidipy_mipt-1.1.2.tar.gz` & `tmp/solidipy_mipt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipy_mipt-1.1.2.tar", last modified: Sun Apr  7 16:19:40 2024, max compression
+gzip compressed data, was "solidipy_mipt-1.1.3.tar", last modified: Tue Apr  9 13:45:58 2024, max compression
```

## Comparing `solidipy_mipt-1.1.2.tar` & `solidipy_mipt-1.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.905176 solidipy_mipt-1.1.2/
--rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5921 2024-04-07 16:19:40.902652 solidipy_mipt-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4812 2024-04-07 16:19:13.000000 solidipy_mipt-1.1.2/README.md
--rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 16:19:40.905176 solidipy_mipt-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-04-07 16:19:23.000000 solidipy_mipt-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.815200 solidipy_mipt-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.839906 solidipy_mipt-1.1.2/src/solidipy_mipt/
--rw-rw-rw-   0        0        0      266 2024-04-06 05:51:26.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/__init__.py
--rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/_metrics.py
--rw-rw-rw-   0        0        0     4584 2024-04-07 15:46:23.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.885713 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/
--rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/__init__.py
--rw-rw-rw-   0        0        0     4450 2024-04-07 15:39:21.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_np_regressor.py
--rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_predictor_abc.py
--rw-rw-rw-   0        0        0     6195 2024-04-07 15:48:48.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_wknn.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.889405 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/utils/
--rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/utils/__init__.py
--rw-rw-rw-   0        0        0     1638 2024-04-07 05:01:27.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/utils/distance.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.897398 solidipy_mipt-1.1.2/src/solidipy_mipt/utils/
--rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/utils/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/utils/errors.py
--rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.1.2/src/solidipy_mipt/utils/validate.py
-drwxrwxrwx   0        0        0        0 2024-04-07 16:19:40.901316 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/
--rw-rw-rw-   0        0        0     5921 2024-04-07 16:19:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-04-07 16:19:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 16:19:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 16:19:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 16:19:40.000000 solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:58.000837 solidipy_mipt-1.1.3/
+-rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5921 2024-04-09 13:45:57.998843 solidipy_mipt-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4812 2024-04-07 16:19:13.000000 solidipy_mipt-1.1.3/README.md
+-rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 13:45:58.000837 solidipy_mipt-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-04-09 13:45:44.000000 solidipy_mipt-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.947562 solidipy_mipt-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.962024 solidipy_mipt-1.1.3/src/solidipy_mipt/
+-rw-rw-rw-   0        0        0      266 2024-04-06 05:51:26.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/__init__.py
+-rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/_metrics.py
+-rw-rw-rw-   0        0        0     4584 2024-04-07 15:46:23.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.988837 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/
+-rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4471 2024-04-09 13:40:23.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_np_regressor.py
+-rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_predictor_abc.py
+-rw-rw-rw-   0        0        0     6216 2024-04-09 13:37:59.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_wknn.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.991845 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/
+-rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/__init__.py
+-rw-rw-rw-   0        0        0     1638 2024-04-07 05:01:27.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/distance.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.995839 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/
+-rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/errors.py
+-rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.1.3/src/solidipy_mipt/utils/validate.py
+drwxrwxrwx   0        0        0        0 2024-04-09 13:45:57.997839 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/
+-rw-rw-rw-   0        0        0     5921 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 13:45:57.000000 solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/top_level.txt
```

### Comparing `solidipy_mipt-1.1.2/LICENSE.txt` & `solidipy_mipt-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/PKG-INFO` & `solidipy_mipt-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.2 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.3 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.1.2/README.md` & `solidipy_mipt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/setup.py` & `solidipy_mipt-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="solidipy_mipt",
-    version="1.1.2",
+    version="1.1.3",
     description="Make your ML solid!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework",
     author="Matvei Gorskii",
     author_email="matveygor41@gmail.com",
     classifiers=[
```

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/_metrics.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/_metrics.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/_selection.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/_selection.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_np_regressor.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_np_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     Raises:
         ValueError: If `k_neighbor` is not more than 0 or not int.
     """
 
     _k_neighbour: int
     _X_train: np.ndarray | None
     _y_train: np.ndarray | None
+    _metric: Metric
 
     def __init__(
         self,
         k_neighbor: int = 1,
         metric: Metric = Metric.EUCLIDEAN
     ) -> None:
         k_neighbor = int(k_neighbor)
@@ -91,15 +92,15 @@
         check_size(X_train, y_train)
 
         self._X_train = X_train.copy()
         self._y_train = y_train.copy()
 
     def predict(
         self,
-        points: np.ndarray
+        X_test: np.ndarray
     ) -> np.ndarray:
         """
         Predict targets for test data using the trained NPRegressor.
 
         Args:
             X_test: The test sample.
 
@@ -116,17 +117,17 @@
             self._y_train is not None
         ]):
             raise UntrainedModelError(
                 "",
                 self.__class__.__name__
             )
 
-        check_size(points, self._X_train, axis=(-1, ))
+        check_size(X_test, self._X_train, axis=(-1, ))
 
-        distances = get_distances(points, self._X_train, self._metric)
+        distances = get_distances(X_test, self._X_train, self._metric)
         weights = self._get_weights(distances)
 
         y = self._y_train.reshape((1, self._y_train.shape[0]))
         coefficients = np.sum(y * weights, axis=-1) / np.sum(weights, axis=-1)
 
         return coefficients
```

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_predictor_abc.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_predictor_abc.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/_wknn.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/_wknn.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     Raises:
         ValueError: If `k_neighbors` is not more than 0 or not int.
     """
 
     _k_neighbors: int
     _X_train: np.ndarray | None
     _y_train: np.ndarray | None
+    _metric: Metric
 
     def __init__(
         self,
         k_neighbors: int = 5,
         metric: Metric = Metric.EUCLIDEAN
     ) -> None:
         k_neighbors = int(k_neighbors)
```

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/algorithms/utils/distance.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/algorithms/utils/distance.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/utils/errors.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/utils/errors.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt/utils/validate.py` & `solidipy_mipt-1.1.3/src/solidipy_mipt/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/PKG-INFO` & `solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.2 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.3 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
```

### Comparing `solidipy_mipt-1.1.2/src/solidipy_mipt.egg-info/SOURCES.txt` & `solidipy_mipt-1.1.3/src/solidipy_mipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

