# Comparing `tmp/molecularnetwork-0.3.7.tar.gz` & `tmp/molecularnetwork-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.3.7.tar", last modified: Sun Apr  7 17:20:35 2024, max compression
+gzip compressed data, was "molecularnetwork-0.3.8.tar", last modified: Tue Apr  9 09:17:09 2024, max compression
```

## Comparing `molecularnetwork-0.3.7.tar` & `molecularnetwork-0.3.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 17:20:35.658483 molecularnetwork-0.3.7/
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.7/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.7/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     2623 2024-04-07 17:20:35.658292 molecularnetwork-0.3.7/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     2200 2024-04-07 17:16:46.000000 molecularnetwork-0.3.7/README.md
--rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.7/banner.png
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 17:20:35.655376 molecularnetwork-0.3.7/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2783 2024-04-07 17:14:31.000000 molecularnetwork-0.3.7/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 17:20:35.658074 molecularnetwork-0.3.7/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     2623 2024-04-07 17:20:35.000000 molecularnetwork-0.3.7/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      452 2024-04-07 17:20:35.000000 molecularnetwork-0.3.7/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-07 17:20:35.000000 molecularnetwork-0.3.7/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-07 17:20:35.000000 molecularnetwork-0.3.7/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-07 17:20:35.000000 molecularnetwork-0.3.7/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.7/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-07 17:20:35.658529 molecularnetwork-0.3.7/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-07 17:17:28.000000 molecularnetwork-0.3.7/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 17:20:35.657819 molecularnetwork-0.3.7/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.7/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.7/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806924 molecularnetwork-0.3.8/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.8/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.8/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4756 2024-04-09 09:17:09.806699 molecularnetwork-0.3.8/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4333 2024-04-09 09:16:01.000000 molecularnetwork-0.3.8/README.md
+-rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.8/banner.png
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.802566 molecularnetwork-0.3.8/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2306 2024-04-09 09:16:19.000000 molecularnetwork-0.3.8/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806402 molecularnetwork-0.3.8/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     4756 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      460 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-09 09:17:09.000000 molecularnetwork-0.3.8/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)    94575 2024-04-09 08:17:30.000000 molecularnetwork-0.3.8/net.png
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.8/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-09 09:17:09.806975 molecularnetwork-0.3.8/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-09 09:16:33.000000 molecularnetwork-0.3.8/setup.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-09 09:17:09.806109 molecularnetwork-0.3.8/test/
+-rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.8/test/test.csv
+-rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/test/test.gpickle
+-rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.8/test/test.py
```

### Comparing `molecularnetwork-0.3.7/.gitignore` & `molecularnetwork-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/LICENSE` & `molecularnetwork-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/banner.png` & `molecularnetwork-0.3.8/banner.png`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/molecularnetwork/featurizer.py` & `molecularnetwork-0.3.8/molecularnetwork/featurizer.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/molecularnetwork/graph.py` & `molecularnetwork-0.3.8/molecularnetwork/graph.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,46 +13,37 @@
         self.fingerprint_calculator = FingerprintCalculator(descriptor)
         self.similarity_calculator = SimilarityCalculator(sim_metric)
         self.graph = networkx.Graph()
 
     def _create_graph(self, smiles_list, classes):
         if classes is None:
             classes = np.full(len(smiles_list), 0)
-        unique_classes, categorical_labels = self._convert_classes(classes)
         fps = self._calculate_fingerprints(smiles_list)
-        self._add_nodes(smiles_list, fps, unique_classes, categorical_labels)
+        self._add_nodes(smiles_list, fps, classes)
         self._add_edges(fps)
 
     def _calculate_fingerprints(self, smiles_list):
         return [
             self.fingerprint_calculator.calculate_fingerprint(smi)
             for smi in smiles_list
         ]
 
-    def _convert_classes(self, classes):
-        unique_classes = np.unique(classes)
-        categorical_labels = np.arange(len(unique_classes))
-        class_labels = np.array(
-            [categorical_labels[np.where(unique_classes == c)[0][0]] for c in classes]
-        )
-        return unique_classes, class_labels
-
-    def _add_nodes(self, smiles_list, fps, unique_classes, categorical_labels):
+    def _add_nodes(self, smiles_list, fps, classes):
         num_nodes = len(smiles_list)
         nodes = range(num_nodes)
         weighted_nodes = [
             (
                 node,
                 {
                     "smiles": smiles_list[node],
-                    "categorical_label": str(unique_classes[value]),
+                    "categorical_label": str(value),
                     "fp": np.array(fps[node])
                 },
             )
-            for node, value in zip(nodes, categorical_labels)
+            for node, value in zip(nodes, classes)
         ]
         self.graph.add_nodes_from(weighted_nodes)
 
     def _add_edges(self, fps):
         num_nodes = len(fps)
         for i in range(num_nodes):
             for j in range(i + 1, num_nodes):
```

### Comparing `molecularnetwork-0.3.7/molecularnetwork/similarity.py` & `molecularnetwork-0.3.8/molecularnetwork/similarity.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/setup.py` & `molecularnetwork-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.3.7",
+    version="0.3.8",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

### Comparing `molecularnetwork-0.3.7/test/test.csv` & `molecularnetwork-0.3.8/test/test.csv`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.7/test/test.gpickle` & `molecularnetwork-0.3.8/test/test.gpickle`

 * *Files identical despite different names*

