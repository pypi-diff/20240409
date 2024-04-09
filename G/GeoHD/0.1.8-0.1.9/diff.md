# Comparing `tmp/GeoHD-0.1.8.tar.gz` & `tmp/GeoHD-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.8.tar", last modified: Mon Apr  8 19:37:50 2024, max compression
+gzip compressed data, was "GeoHD-0.1.9.tar", last modified: Mon Apr  8 19:46:31 2024, max compression
```

## Comparing `GeoHD-0.1.8.tar` & `GeoHD-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/
-drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.930373 GeoHD-0.1.8/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.8/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.8/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.8/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.8/GeoHD/process.py
--rw-rw-rw-   0        0        0    19103 2024-04-08 19:37:31.000000 GeoHD-0.1.8/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.8/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.8/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5266 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-08 19:37:50.000000 GeoHD-0.1.8/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     5266 2024-04-08 19:37:50.935317 GeoHD-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 19:37:50.935317 GeoHD-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-08 19:37:40.000000 GeoHD-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 19:37:50.935317 GeoHD-0.1.8/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.8/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.537550 GeoHD-0.1.9/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.523882 GeoHD-0.1.9/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.9/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.1.9/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.9/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4358 2024-04-05 18:26:40.000000 GeoHD-0.1.9/GeoHD/process.py
+-rw-rw-rw-   0        0        0    23677 2024-04-08 19:45:44.000000 GeoHD-0.1.9/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.1.9/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0     9599 2024-04-05 18:21:57.000000 GeoHD-0.1.9/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.535545 GeoHD-0.1.9/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5266 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-08 19:46:31.000000 GeoHD-0.1.9/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     5266 2024-04-08 19:46:31.536550 GeoHD-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4768 2024-04-05 18:54:02.000000 GeoHD-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 19:46:31.537550 GeoHD-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-08 19:46:21.000000 GeoHD-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:46:31.534912 GeoHD-0.1.9/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.9/test/__init__.py
```

### Comparing `GeoHD-0.1.8/GeoHD/AKDE.py` & `GeoHD-0.1.9/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/GeoHD/analyze.py` & `GeoHD-0.1.9/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/GeoHD/process.py` & `GeoHD-0.1.9/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/GeoHD/utils.py` & `GeoHD-0.1.9/GeoHD/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -337,15 +337,125 @@
     plt.title('Hierarchical Clustering')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.show()
 
     return cluster_labels
 
+def louvain_euclidean_distance(p1, p2):
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
+def louvain_community_detection(points_shapefile, max_iterations=100, tolerance=1e-6):
+    """
+    Perform community detection on a set of points from a shapefile using the Louvain algorithm.
+
+    Args:
+    points_shapefile (str): Path to the shapefile containing point data.
+    max_iterations (int): Maximum number of iterations for the Louvain algorithm.
+    tolerance (float): Convergence threshold for the Louvain algorithm.
+
+    Returns:
+    list: Community labels for each point.
+    """
+    # Load shapefile point data
+    points_gdf = gpd.read_file(points_shapefile)
+    num_points = len(points_gdf)
+
+    # Extract coordinates from GeoDataFrame
+    coordinates = np.array(points_gdf.geometry.apply(lambda point: (point.x, point.y)))
+
+    # Create adjacency matrix
+    adjacency_matrix = np.zeros((num_points, num_points))
+    for i in range(num_points):
+        for j in range(i+1, num_points):
+            # Calculate Euclidean distance as edge weight
+            dist = louvain_euclidean_distance(coordinates[i], coordinates[j])
+            # Assign weight to adjacency matrix
+            adjacency_matrix[i, j] = dist
+            adjacency_matrix[j, i] = dist
+
+    # Initialize community labels for each point
+    community_labels = list(range(num_points))
+
+    # Louvain algorithm
+    prev_modularity = -1
+    for _ in range(max_iterations):
+        # Initialize change flag and modularity
+        change = False
+        modularity = 0
+
+        # Iterate over each point
+        for i in range(num_points):
+            # Calculate the modularity change by moving the point to its neighboring communities
+            current_community = community_labels[i]
+            best_community = current_community
+            max_modularity_change = 0
+            
+            # Find neighboring communities
+            neighbors = np.unique([community_labels[j] for j in np.nonzero(adjacency_matrix[i])[0]])
+            
+            # Calculate modularity change for each neighboring community
+            for neighbor in neighbors:
+                if neighbor != current_community:
+                    # Calculate modularity change
+                    modularity_change = 0
+                    for j in range(num_points):
+                        if community_labels[j] == current_community:
+                            modularity_change -= adjacency_matrix[i, j]
+                        elif community_labels[j] == neighbor:
+                            modularity_change += adjacency_matrix[i, j]
+                    
+                    # Update best community if modularity change is positive
+                    if modularity_change > max_modularity_change:
+                        max_modularity_change = modularity_change
+                        best_community = neighbor
+            
+            # Move the point to the community with the maximum modularity change
+            if best_community != current_community:
+                community_labels[i] = best_community
+                change = True
+        
+        # Calculate modularity
+        for i in range(num_points):
+            for j in range(num_points):
+                if community_labels[i] == community_labels[j]:
+                    modularity += adjacency_matrix[i, j]
+
+        # Check for convergence
+        if abs(modularity - prev_modularity) < tolerance:
+            break
+        prev_modularity = modularity
+
+        # If no change occurred, stop iterating
+        if not change:
+            break
+
+    # Plot communities
+    fig, ax = plt.subplots(figsize=(10, 10))
+    colors = ['r', 'g', 'b', 'c', 'm', 'y', 'k']  # Color palette for communities
+    for i, community in enumerate(np.unique(community_labels)):
+        community_points = points_gdf.geometry[np.array(community_labels) == community]
+        ax.scatter([point.x for point in community_points], [point.y for point in community_points], c=colors[i % len(colors)], label=f'Community {i+1}')
+    ax.legend()
+    plt.title('Community Detection using Louvain Algorithm')
+    plt.xlabel('Longitude')
+    plt.ylabel('Latitude')
+    plt.show()
 
+    return community_labels
 
 def GMM_gaussian(x, mean, cov):
     """
     Calculate the value of the Gaussian distribution at point x.
 
     Args:
     x (np.array): The point at which to evaluate the Gaussian.
```

### Comparing `GeoHD-0.1.8/GeoHD/visualize.py` & `GeoHD-0.1.9/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/GeoHD/zone.py` & `GeoHD-0.1.9/GeoHD/zone.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/GeoHD.egg-info/PKG-INFO` & `GeoHD-0.1.9/GeoHD.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `GeoHD-0.1.8/LICENSE` & `GeoHD-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/PKG-INFO` & `GeoHD-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `GeoHD-0.1.8/README.md` & `GeoHD-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.8/setup.py` & `GeoHD-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.1.8',
+    version='0.1.9',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

