# Comparing `tmp/GeoHD-0.1.9.tar.gz` & `tmp/GeoHD-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.9.tar", last modified: Mon Apr  8 19:46:31 2024, max compression
+gzip compressed data, was "GeoHD-0.2.1.tar", last modified: Tue Apr  9 17:33:06 2024, max compression
```

## Comparing `GeoHD-0.1.9.tar` & `GeoHD-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.537550 GeoHD-0.1.9/
-drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.523882 GeoHD-0.1.9/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.9/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.9/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.9/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.9/GeoHD/process.py
--rw-rw-rw-   0        0        0    23677 2024-04-08 19:45:44.000000 GeoHD-0.1.9/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.9/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.9/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.535545 GeoHD-0.1.9/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5266 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     5266 2024-04-08 19:46:31.536550 GeoHD-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 19:46:31.537550 GeoHD-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-08 19:46:21.000000 GeoHD-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.534912 GeoHD-0.1.9/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.9/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:33:06.659880 GeoHD-0.2.1/
+drwxrwxrwx   0        0        0        0 2024-04-09 17:33:06.656293 GeoHD-0.2.1/GeoHD/
+-rw-rw-rw-   0        0        0     8641 2024-04-09 17:31:08.000000 GeoHD-0.2.1/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.2.1/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.2.1/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.2.1/GeoHD/process.py
+-rw-rw-rw-   0        0        0    32021 2024-04-09 17:31:08.000000 GeoHD-0.2.1/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.2.1/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9597 2024-04-09 17:31:08.000000 GeoHD-0.2.1/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:33:06.659880 GeoHD-0.2.1/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5268 2024-04-09 17:33:06.000000 GeoHD-0.2.1/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-09 17:33:06.000000 GeoHD-0.2.1/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:33:06.000000 GeoHD-0.2.1/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-09 17:33:06.000000 GeoHD-0.2.1/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 17:33:06.000000 GeoHD-0.2.1/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5268 2024-04-09 17:33:06.659880 GeoHD-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4772 2024-04-09 17:31:08.000000 GeoHD-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:33:06.659880 GeoHD-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-09 17:32:11.000000 GeoHD-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:33:06.659880 GeoHD-0.2.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.2.1/test/__init__.py
```

### Comparing `GeoHD-0.1.9/GeoHD/AKDE.py` & `GeoHD-0.2.1/GeoHD/AKDE.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,16 @@
     plt.colorbar(label='Density')
     plt.xlabel('X')
     plt.ylabel('Y')
     plt.title('Adaptive KDE Density Estimation')
     plt.legend()
     plt.show()
 
+
+
 # Example usage:
 if __name__ == "__main__":
     import os
     # Define the name of the folder to be created
     folder_name = 'output'
     # Check if the folder exists, if not, create it
     if not os.path.exists(folder_name):
```

### Comparing `GeoHD-0.1.9/GeoHD/analyze.py` & `GeoHD-0.2.1/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.9/GeoHD/process.py` & `GeoHD-0.2.1/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.9/GeoHD/utils.py` & `GeoHD-0.2.1/GeoHD/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -449,14 +449,123 @@
     plt.title('Community Detection using Louvain Algorithm')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.show()
 
     return community_labels
 
+def op_euclidean_distance(p1, p2):
+    """
+    Calculate the Euclidean distance between two points.
+
+    Args:
+    p1 (tuple): Coordinates of the first point.
+    p2 (tuple): Coordinates of the second point.
+
+    Returns:
+    float: Euclidean distance between the two points.
+    """
+    return np.sqrt((p1[0] - p2[0])**2 + (p1[1] - p2[1])**2)
+
+def op_optics_cluster(points_gdf, epsilon, min_pts):
+    """
+    Perform clustering on a set of points using the OPTICS algorithm.
+
+    Args:
+    points_gdf (geopandas.GeoDataFrame): GeoDataFrame containing point data.
+    epsilon (float): Maximum distance to consider points as neighbors.
+    min_pts (int): Minimum number of points required to form a cluster.
+
+    Returns:
+    list: Cluster labels for each point.
+    """
+    num_points = len(points_gdf)
+    # Extract coordinates from GeoDataFrame
+    coordinates = np.array(points_gdf.geometry.apply(lambda point: (point.x, point.y)))
+    # Initialize reachability distances and cluster labels
+    reachability_distances = np.full(num_points, np.inf)
+    cluster_labels = np.full(num_points, -1)
+    # Iterate over each point
+    for i in range(num_points):
+        # Calculate distances to all other points
+        distances = [op_euclidean_distance(coordinates[i], coordinates[j]) for j in range(num_points)]
+        # Find neighbors within epsilon distance
+        neighbors = [j for j in range(num_points) if distances[j] <= epsilon and j != i]
+        if len(neighbors) >= min_pts:
+            # If core point, update reachability distances of neighbors
+            for neighbor in neighbors:
+                core_dist = max(distances[j] for j in neighbors if j != neighbor)
+                reachability_distances[neighbor] = min(core_dist, distances[neighbor])
+        # Assign point to a cluster if not already assigned
+        if cluster_labels[i] == -1:
+            if len(neighbors) >= min_pts:
+                # If core point, expand cluster
+                cluster_id = i
+                while True:
+                    cluster_labels[cluster_id] = cluster_id
+                    neighbors = [j for j in range(num_points) if distances[j] <= epsilon and j != cluster_id]
+                    if len(neighbors) == 0:
+                        break
+                    # Find next core point with minimum reachability distance
+                    next_core = min(neighbors, key=lambda x: reachability_distances[x])
+                    core_dist = max(distances[j] for j in neighbors if j != next_core)
+                    if reachability_distances[next_core] > core_dist:
+                        # If next core point is not directly reachable, mark it as outlier
+                        cluster_labels[next_core] = -1
+                    else:
+                        # If next core point is directly reachable, expand cluster
+                        cluster_id += 1
+                        cluster_labels[next_core] = cluster_id
+                        cluster_id = next_core
+            else:
+                # If outlier point, mark as noise
+                cluster_labels[i] = -1
+    return cluster_labels
+
+def op_plot_clusters(points_gdf, cluster_labels):
+    """
+    Plot clusters on a map.
+
+    Args:
+    points_gdf (geopandas.GeoDataFrame): GeoDataFrame containing point data.
+    cluster_labels (list): Cluster labels for each point.
+    """
+    fig, ax = plt.subplots(figsize=(10, 10))
+    colors = ['r', 'g', 'b', 'c', 'm', 'y', 'k']  # Color palette for clusters
+    for cluster_id in np.unique(cluster_labels):
+        if cluster_id == -1:
+            # Plot outliers as black
+            outlier_points = points_gdf.geometry[cluster_labels == -1]
+            ax.scatter([point.x for point in outlier_points], [point.y for point in outlier_points], c='k', label='Outliers')
+        else:
+            # Plot cluster points with different colors
+            cluster_points = points_gdf.geometry[cluster_labels == cluster_id]
+            ax.scatter([point.x for point in cluster_points], [point.y for point in cluster_points], c=colors[cluster_id % len(colors)], label=f'Cluster {cluster_id}')
+    ax.legend()
+    plt.title('Clustering using OPTICS Algorithm')
+    plt.xlabel('Longitude')
+    plt.ylabel('Latitude')
+    plt.show()
+
+def op_optics_clustering(points_shapefile, epsilon, min_pts):
+    """
+    Perform clustering on a set of points from a shapefile using the OPTICS algorithm and plot the clusters.
+
+    Args:
+    points_shapefile (str): Path to the shapefile containing point data.
+    epsilon (float): Maximum distance to consider points as neighbors.
+    min_pts (int): Minimum number of points required to form a cluster.
+    """
+    # Load shapefile point data
+    points_gdf = gpd.read_file(points_shapefile)
+    # Perform OPTICS clustering
+    cluster_labels = op_optics_cluster(points_gdf, epsilon, min_pts)
+    # Plot clusters
+    op_plot_clusters(points_gdf, cluster_labels)
+
 def GMM_gaussian(x, mean, cov):
     """
     Calculate the value of the Gaussian distribution at point x.
 
     Args:
     x (np.array): The point at which to evaluate the Gaussian.
     mean (np.array): The mean of the Gaussian distribution.
@@ -610,14 +719,86 @@
     plt.title('GMM Clustering')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.show()
 
     return cluster_labels
 
+def hdbscan_clustering(points_shapefile, min_samples, min_cluster_size):
+    """
+    Perform clustering on a set of points from a shapefile using the HDBSCAN algorithm and plot the clusters.
+
+    Args:
+    points_shapefile (str): Path to the shapefile containing point data.
+    min_samples (int): The number of samples in a neighborhood for a point to be considered a core point.
+    min_cluster_size (int): The minimum number of points required to form a cluster.
+    """
+    # Define a function to calculate Euclidean distance between two points
+    def euclidean_distance(p1, p2):
+        return np.sqrt((p1[0] - p2[0])**2 + (p1[1] - p2[1])**2)
+
+    # Define a function to expand a cluster starting from a core point
+    def expand_cluster(i, distances, cluster_labels, cluster_id, min_cluster_size):
+        cluster_labels[i] = cluster_id
+        seeds = [j for j in range(len(cluster_labels)) if distances[i, j] < min_samples]
+        while seeds:
+            j = seeds.pop(0)
+            if cluster_labels[j] == -1:
+                cluster_labels[j] = cluster_id
+                if np.sum(distances[j] < min_samples) >= min_samples:
+                    seeds.extend([k for k in range(len(cluster_labels)) if distances[j, k] < min_samples])
+            elif cluster_labels[j] == 0:
+                cluster_labels[j] = cluster_id
+
+    # Define a function to plot clusters on a map
+    def plot_clusters(points_gdf, cluster_labels):
+        fig, ax = plt.subplots(figsize=(10, 10))
+        colors = ['r', 'g', 'b', 'c', 'm', 'y', 'k']
+        for cluster_id in np.unique(cluster_labels):
+            if cluster_id == -1:
+                outlier_points = points_gdf.geometry[cluster_labels == -1]
+                ax.scatter([point.x for point in outlier_points], [point.y for point in outlier_points], c='k', label='Outliers')
+            else:
+                cluster_points = points_gdf.geometry[cluster_labels == cluster_id]
+                ax.scatter([point.x for point in cluster_points], [point.y for point in cluster_points], c=colors[cluster_id % len(colors)], label=f'Cluster {cluster_id}')
+        ax.legend()
+        plt.title('Clustering using HDBSCAN Algorithm')
+        plt.xlabel('Longitude')
+        plt.ylabel('Latitude')
+        plt.show()
+
+    # Load shapefile point data
+    points_gdf = gpd.read_file(points_shapefile)
+    num_points = len(points_gdf)
+    coordinates = np.array(points_gdf.geometry.apply(lambda point: (point.x, point.y)))
+
+    # Compute pairwise distances
+    distances = np.zeros((num_points, num_points))
+    for i in range(num_points):
+        for j in range(i+1, num_points):
+            distances[i, j] = euclidean_distance(coordinates[i], coordinates[j])
+            distances[j, i] = distances[i, j]
+
+    # Compute core points
+    core_points = np.sum(distances < min_samples, axis=1) >= min_samples
+
+    # Initialize cluster labels
+    cluster_labels = np.full(num_points, -1)
+    cluster_id = 0
+
+    # Iterate over each point
+    for i in range(num_points):
+        if cluster_labels[i] == -1 and core_points[i]:
+            cluster_id += 1
+            expand_cluster(i, distances, cluster_labels, cluster_id, min_cluster_size)
+
+    # Plot clusters
+    plot_clusters(points_gdf, cluster_labels)
+
+
 
 
 # Example usage:
 if __name__ == "__main__":
     density_data_path = './output/AKDE_density_grid.npy'
     hotspots = extract_hotspots(density_data_path)
     visualize_hotspots(np.load(density_data_path), hotspots)
```

### Comparing `GeoHD-0.1.9/GeoHD/visualize.py` & `GeoHD-0.2.1/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.9/GeoHD/zone.py` & `GeoHD-0.2.1/GeoHD/zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,20 +228,18 @@
     plt.title('Heatmap of Hexagonal Grids based on Crash Point Count')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.show()
 
 
 
-
-
 # Example usage
 # create_cell_zones('./data/area.shp', './data/crash.shp')
 
 # Example usage
 # create_hex_grid_zones('./data/area.shp', './data/crash.shp')
 
 # Example usage
 # create_cell_heatmap('./data/area.shp', './data/crash.shp')
 
 # Example usage
-# create_hexagonal_heatmap('./data/area.shp', './data/crash.shp')
+# create_hexagonal_heatmap('./data/area.shp', './data/crash.shp')
```

### Comparing `GeoHD-0.1.9/GeoHD.egg-info/PKG-INFO` & `GeoHD-0.2.1/GeoHD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.9
+Version: 0.2.1
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.1.5-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.1.5-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.1.9-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.1.9-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -134,10 +134,11 @@
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
 
+
 ## Authors
 
 * Yuchen Yan
```

### Comparing `GeoHD-0.1.9/LICENSE` & `GeoHD-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.9/PKG-INFO` & `GeoHD-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.9
+Version: 0.2.1
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.1.5-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.1.5-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.1.9-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.1.9-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -134,10 +134,11 @@
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
 
+
 ## Authors
 
 * Yuchen Yan
```

### Comparing `GeoHD-0.1.9/README.md` & `GeoHD-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.1.5-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.1.5-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.1.9-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.1.9-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -117,10 +117,11 @@
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
 
+
 ## Authors
 
-* Yuchen Yan
+* Yuchen Yan
```

### Comparing `GeoHD-0.1.9/setup.py` & `GeoHD-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.1.9',
+    version='0.2.1',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

