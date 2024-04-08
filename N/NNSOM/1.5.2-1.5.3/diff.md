# Comparing `tmp/nnsom-1.5.2.tar.gz` & `tmp/nnsom-1.5.3.tar.gz`

## Comparing `nnsom-1.5.2.tar` & `nnsom-1.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/som.py
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.5.2/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.2/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.2/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    77087 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    13419 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/som.py
+-rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.3/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.3/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.3/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.3/PKG-INFO
```

### Comparing `nnsom-1.5.2/src/NNSOM/plots.py` & `nnsom-1.5.3/src/NNSOM/plots.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.2/src/NNSOM/som.py` & `nnsom-1.5.3/src/NNSOM/som.py`

 * *Files 25% similar despite different names*

```diff
@@ -210,14 +210,96 @@
         self.outputs = self.sim_som(x)
         self.sim_flag = False
 
         print('Ending Training')
         current_time = now.strftime("%H:%M:%S")
         print("Current Time =", current_time)
 
+    def cluster_data(self, x):
+        """
+        Cluster the input data based on the trained SOM reference vectors.
+
+        Parameters
+        ----------
+        x : ndarray (normalized)
+            The input data to be clustered.
+
+        Returns
+        -------
+        clusters : list of lists
+            A list containing sub-lists, where each sublist represents a cluster.
+            The indices of the input data points belonging to the same cluster
+            are stored in the corresponding sublist, sorted by their proximity
+            to the cluster center.
+
+        cluster_distances : list of lists
+            A list containing sub-lists, where each sublist represents the distances
+            of the input data points to the corresponding cluster center, sorted in
+            the same order as the indices in the `clusters` list.
+
+        max_cluster_distances : ndarray
+            A list containing the maximum distance between each cluster center
+            and the data points belonging to that cluster.
+
+        cluster_sizes : ndarray
+            A list containing the number of data points in each cluster.
+
+        Raises
+        -------
+        ValueError
+            If the SOM has not been trained.
+
+        ValueError
+            If the number of features in the input data and the SOM weights do not match.
+        """
+
+        if self.sim_flag:
+            raise ValueError("SOM has not been trained.")
+
+        if x.shape[0] != self.w.shape[1]:
+            raise ValueError('The number of features in the input data and the SOM weights do not match.')
+
+        w = self.w
+        shapw = w.shape
+        S = shapw[0]
+
+        x_w_dist = cdist(w, np.transpose(x), 'euclidean')
+        ind1 = np.argmin(x_w_dist, axis=0)
+
+        clusters = []  # a cluster array of indices sorted by distances
+        cluster_distances = []  # a cluster array of distances sorted by distances
+        max_cluster_distances = np.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
+        cluster_sizes = []  # cluster array sizes
+
+        for i in range(S):
+            # Find which inputs are closest to each weight (in cluster i)
+            tempclust = np.where(ind1 == i)[0]
+
+            # Save distance of each input in the cluster to cluster center (weight)
+            tempdist = x_w_dist[i, tempclust]
+            indsort = np.argsort(tempdist)
+            tempclust = tempclust[indsort]  # Sort indices
+            tempdist = tempdist[indsort]
+
+            # Add to distance array sorted distances
+            cluster_distances.append(tempdist)
+
+            # Add to Cluster array sorted indices
+            clusters.append(tempclust)
+
+            # Cluster size
+            num = len(tempclust)
+            cluster_sizes.append(num)
+
+            # Save the maximum distance to any input in the cluster from cluster center
+            if num > 0:
+                max_cluster_distances[i] = tempdist[-1]
+
+        return clusters, cluster_distances, max_cluster_distances, cluster_sizes
+
     def quantization_error(self, dist):
         """
         Calculate quantization error
         """
         quant_err = np.array([0 if len(item) == 0 else np.mean(item) for item in dist]).mean()
 
         return quant_err
```

### Comparing `nnsom-1.5.2/src/NNSOM/utils.py` & `nnsom-1.5.3/src/NNSOM/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -129,82 +129,14 @@
     # Determine the shape of the elongated hexagon to represent edge between each cluster
     edgex = np.array([-1, 0, 1, 0]) * 0.5
     edgey = np.array([0, 1, 0, - 1]) * np.sqrt(0.75) / 3
 
     return edgex, edgey
 
 
-# Helper function to extract cluster details obtained from the SOM and input data
-def extract_cluster_details(som, data):
-    """
-    Returns Cluster Index Array, Cluster Distance Array,
-    Maximum Distance Array, and Cluster Size Array.
-
-    Parameters
-    ----------
-    som : SOM object
-        A SOM object trained on the input data.
-    data : numpy array
-        Input data to be clustered.
-
-    Returns
-    -------
-    clust : list
-        A cluster array of indices sorted by distances.
-    dist : list
-        A cluster array of distances sorted by distances.
-    mdist : numpy array
-        A list of maimum distance to any input in the cluster from cluster center.
-    clustSize : list
-        Cluster array sizes.
-    """
-
-    # Assertions (check if the input data and som weights have the same number of features)
-    if data.shape[0] != som.w.shape[1]:
-        raise ValueError('The number of features in the input data and the SOM weights do not match.')
-
-    w = som.w
-    shapw = w.shape
-    S = shapw[0]
-
-    x_w_dist = cdist(som.w, np.transpose(data), 'euclidean')
-    ind1 = np.argmin(x_w_dist, axis=0)
-
-    clust = []  # a cluster array of indices sorted by distances
-    dist = []  # a cluster array of distances sorted by distances
-    mdist = np.zeros(S)  # a list of maimum distance to any input in the cluster from cluster center
-    clustSize = []  # cluster array sizes
-
-    for i in range(S):
-        # Find which inputs are closest to each weight (in cluster i)
-        tempclust = np.where(ind1 == i)[0]
-
-        # Save distance of each input in the cluster to cluster center (weight)
-        tempdist = x_w_dist[i, tempclust]
-        indsort = np.argsort(tempdist)
-        tempclust = tempclust[indsort]  # Sort indices
-        tempdist = tempdist[indsort]
-
-        # Add to distance array sorted distances
-        dist.append(tempdist)
-
-        # Add to Cluster array sorted indices
-        clust.append(tempclust)
-
-        # Cluster size
-        num = len(tempclust)
-        clustSize.append(num)
-
-        # Save the maximum distance to any input in the cluster from cluster center
-        if num > 0:
-            mdist[i] = tempdist[-1]
-
-    return clust, dist, mdist, clustSize
-
-
 # Helper Functions to extract information from the input data for passing to the plot
 def get_cluster_data(data, clust):
     """
     For each cluster, extract the corresponding data points and return them in a list.
 
     Parameters
     ----------
@@ -397,44 +329,14 @@
             cluster_counts[i] = [np.sum(cat_feature[indices] == cls) for cls in unique_classes]
         else:
             cluster_counts[i] = np.zeros(num_classes, dtype=int)
 
     return cluster_counts
 
 
-def get_align_cluster(cat_feature, clust):
-    """
-    Create an array of alignments for each cluster based on class indices.
-
-    Parameters
-    ----------
-    cat_feature : array-like
-        Categorical feature array.
-    clust : list
-        A list of arrays, each containing the indices of elements in a cluster.
-
-    Returns
-    -------
-    alignment_cluster : numpy array
-        A 2D array with alignments for each cluster.
-    """
-    unique_classes = np.unique(cat_feature)
-    num_classes = len(unique_classes)
-
-    # Initialize the array to hold alignments for each cluster
-    alignment_cluster = np.zeros((len(clust), num_classes), dtype=int)
-
-    # Populate the alignment array
-    # Since the alignment seems to be the index of the class, we can directly use the unique_classes for alignment
-    for i in range(len(clust)):
-        alignment_cluster[i] = unique_classes
-
-    return alignment_cluster
-
-
 def cal_class_cluster_intersect(clust, *args):
     """
     Calculate the intersection sizes of each class with each neuron cluster.
 
     This function computes the size of the intersection between each given class
     (represented by arrays of indices) and each neuron cluster (represented by
     a list of lists of indices). The result is a 2D array where each row corresponds
```

### Comparing `nnsom-1.5.2/.gitignore` & `nnsom-1.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.2/pyproject.toml` & `nnsom-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.2"
+version = "1.5.3"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.2/PKG-INFO` & `nnsom-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.2
+Version: 1.5.3
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

