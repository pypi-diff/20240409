# Comparing `tmp/automotifs-1.0.3.tar.gz` & `tmp/automotifs-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.0.3.tar", last modified: Sat Mar 16 15:02:38 2024, max compression
+gzip compressed data, was "automotifs-1.1.tar", last modified: Tue Apr  9 12:25:42 2024, max compression
```

## Comparing `automotifs-1.0.3.tar` & `automotifs-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 15:02:38.541920 automotifs-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-16 15:02:18.000000 automotifs-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-16 15:02:38.541920 automotifs-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-16 15:02:18.000000 automotifs-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 15:02:38.541920 automotifs-1.0.3/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-16 15:02:18.000000 automotifs-1.0.3/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-03-16 15:02:18.000000 automotifs-1.0.3/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 15:02:38.541920 automotifs-1.0.3/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-16 15:02:38.000000 automotifs-1.0.3/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-16 15:02:38.000000 automotifs-1.0.3/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 15:02:38.000000 automotifs-1.0.3/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-16 15:02:38.000000 automotifs-1.0.3/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-16 15:02:38.000000 automotifs-1.0.3/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 15:02:38.541920 automotifs-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-16 15:02:18.000000 automotifs-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 15:02:38.541920 automotifs-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-03-16 15:02:18.000000 automotifs-1.0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:25:42.315771 automotifs-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 12:25:20.000000 automotifs-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-09 12:25:42.315771 automotifs-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-09 12:25:20.000000 automotifs-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:25:42.311771 automotifs-1.1/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 12:25:20.000000 automotifs-1.1/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-09 12:25:20.000000 automotifs-1.1/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:25:42.315771 automotifs-1.1/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-09 12:25:42.000000 automotifs-1.1/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 12:25:42.000000 automotifs-1.1/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:25:42.000000 automotifs-1.1/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 12:25:42.000000 automotifs-1.1/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 12:25:42.000000 automotifs-1.1/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:25:42.315771 automotifs-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 12:25:21.000000 automotifs-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:25:42.315771 automotifs-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-09 12:25:21.000000 automotifs-1.1/tests/test.py
```

### Comparing `automotifs-1.0.3/LICENSE` & `automotifs-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `automotifs-1.0.3/PKG-INFO` & `automotifs-1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.0.3
+Version: 1.1
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,40 +12,43 @@
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
-AutoMotif helps you find patterns, called motifs, in network graphs. It uses NetworkX for working with graphs, dotmotif for finding the patterns, and pandas for handling data. Whether your graphs are directed or not, AutoMotif can search for motifs based on the criteria you set, like motif size and whether to consider pattern repetitions (automorphisms).
+AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
 
 ```bash
 pip install automotifs
 ```
 ## Quick Start
 ```python
 from automotif import AutoMotif
+from dotmotif import executors
 import networkx as nx
 # Example: A random directed graph
 G = nx.gnp_random_graph(100, 0.5, directed=True)
 # Set up AutoMotif
-motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True)
+motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO = True)
 # Start finding motifs
 motifs = motif_finder.find_all_motifs()
+# Calculate the Z-Score for the motifs
+z_scores = motif_finder.calculate_zscore(num_random_graphs = 30, Executor = executors.NetworkXExecutor)
 ```
 ## Features
-- Automated Detection: Find motifs in your network without manually tweaking every parameter. AutoMotif takes care of the heavy lifting.
-- Flexibility: Whether your networks are directed or undirected, AutoMotif can handle them. Plus, you can decide if you want to look for automorphisms and set the size of motifs to search for.
-- Save for Later: Directly save your findings to CSV files, making it easier to analyze results or share them with others.
+- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing researchers to focus more on analysis and less on setup.
+- **Flexible and Powerful**: Capable of handling both directed and undirected graphs, AutoMotif provides flexibility in defining motifs, including size and whether to consider automorphisms, ensuring a broad applicability across different types of network analyses.
+- **Data Organization and Export**: Directly save your motifs to CSV files for easy access, further analysis, or sharing with your team or research community.
+- **Z-Score Calculation**: Assess the statistical significance of detected motifs by calculating their Z-scores, providing insights into the rarity or commonality of patterns within your network compared to random expectations.
 ## Contributions
-Contributions to AutoMotif are welcome! If you have suggestions for improvement or new features, feel free to open an issue or submit a pull request.
+We encourage contributions to AutoMotif! If you have ideas for improvements or new features, don't hesitate to open an issue or submit a pull request on our repository.
 ## License
 AutoMotif is made available under the MIT License. See the LICENSE file for more details.
 ***
 ## Who made this? 
-Giorgio Micaletto, under Professor Marta Zava's supervision at Bocconi University, put together AutoMotif. It was created to make network motif analysis less of a headache.
-
+AutoMotif was developed by Giorgio Micaletto under the guidance of Professor Marta Zava at Bocconi University. This tool is designed to simplify and facilitate the complex process of network motif analysis.
 Contacts:
 - giorgio.micaletto@studbocconi.it
-- linkedin.com/in/giorgio-micaletto/
+- [linkedin](linkedin.com/in/giorgio-micaletto/)
```

### Comparing `automotifs-1.0.3/automotif/automotif.py` & `automotifs-1.1/automotif/automotif.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,41 +18,44 @@
 import pandas as pd 
 import networkx as nx
 import os
 from dotmotif import Motif
 from itertools import product
 import dotmotif.executors as executors
 from typing import Union
+import numpy as np
 
 class AutoMotif:
     """
     Wrapper class for dotmotif to find all possible motifs in a graph automatically.
-    Parameters:
+    Inputs:
     - Graph (networkx.Graph): The graph to analyze.
     - size (int): Size of the motif to find.
     - directed (bool, optional): Whether the graph is directed. Defaults to False.
     - allow_automorphism (bool, optional): Whether to allow automorphisms. Defaults to False.
     - upto (bool, optional): Whether to generate motifs from a lower bound to the specified size. Defaults to False.
     - lower (int, optional): Lower bound for motif size. Defaults to 3.
     - save (bool, optional): Whether to save the motifs to a CSV file. Defaults to False.
     - path (str, optional): Directory to save the motifs. Defaults to None.
     - find (bool, optional): Whether to find all motifs directly. Defaults to False.
     - verbose (bool, optional): Whether to print progress. Defaults to False.
+    - use_GrandISO (bool, optional): Whether to use GrandISO for motif detection. Defaults to False.
     """
     def __init__(self, 
                  Graph: Union[nx.Graph, nx.DiGraph, nx.MultiGraph, nx.MultiDiGraph], 
                  size: int, 
                  directed: bool = False, 
                  allow_automorphism: bool = False, 
                  upto: bool = False,
                  lower: int = 3, 
                  save: bool = False, 
                  path: str = None,
                  find: bool = False, 
-                 verbose: bool = False):
+                 verbose: bool = False,
+                 use_GrandISO: bool = False):
         if not hasattr(Graph, "nodes") or not callable(getattr(Graph, "nodes")):
             raise ValueError("Graph should be a NetworkX graph")
         elif type(size) != int:
             raise ValueError("Size should be an integer")
         elif type(upto) != bool:
             raise ValueError("Upto should be a boolean")
         elif type(save) != bool:
@@ -70,28 +73,30 @@
         self.upto = upto
         self.save = save
         self.path = path
         self.verbose = verbose
         self.directed = directed
         self.allow_automorphism = allow_automorphism
         self.lower = lower
-        self.Ex = executors.NetworkXExecutor(graph = self.Graph)
+        if use_GrandISO == True:
+            self.Ex = executors.GrandIsoExecutor(graph = self.Graph)
+        else:
+            self.Ex = executors.NetworkXExecutor(graph = self.Graph)
         self.motifs = None
         self.generate_required_motifs()
+        self.motifs_found = None
         if find == True:
             self.find_all_motifs()    
     
-    def generate_graphs(self, n):
+    def generate_graphs(self, n: int) -> list:
         """
         Generate all possible directed graphs for n nodes, ignoring self-loops,
         and ensure no isolated nodes are present. Each graph is represented by its adjacency matrix.
-        Parameters:
+        Inputs:
         - n (int): Number of nodes.
-        Returns:
-        - list: List of adjacency matrices representing all possible graphs.
         """
         if self.verbose == True:
             print("Generating graphs for", n, "nodes")
         graphs = []
         for edges in product([0, 1], repeat=n*(n-1)):
             matrix = [[0 for _ in range(n)] for _ in range(n)]
             edge_index = 0
@@ -103,130 +108,206 @@
             has_isolated_node = False
             for i in range(n):
                 if all(matrix[i][j] == 0 for j in range(n)) or all(matrix[j][i] == 0 for j in range(n)):
                     has_isolated_node = True
                     break
             if not has_isolated_node:
                 graphs.append(matrix)
-        print("Generated", len(graphs), "graphs for", n, "nodes")
+        if self.verbose == True:
+            print("Generated", len(graphs), "graphs for", n, "nodes")
         return graphs
     
-    def matrix_to_motif(self, matrix, node_labels):
+    def matrix_to_motif(self, matrix: list, node_labels: list) -> Motif:
         """
         Convert an adjacency matrix to the specified motif format.
-        Parameters:
+        Inputs:
         - matrix (list): Adjacency matrix.
         - node_labels (list): List of node labels.
-        Returns:
-        - Motif: Motif object.
         """
         motif_str = ""
         for i, row in enumerate(matrix):
             for j, edge in enumerate(row):
                 if edge:
                     motif_str += f"{node_labels[i]} -> {node_labels[j]}\n"
         remove_automorphisms = not self.allow_automorphism
         ignore_direct = not self.directed
         motif_obj = Motif(input_motif=motif_str, enforce_inequality = True, exclude_automorphisms = remove_automorphisms, ignore_direction = ignore_direct)
         return motif_obj
     
-    def generate_motifs(self, n):
+    def generate_motifs(self, n: int) -> list:
         """
         Generate all unique motifs of n nodes and convert them to the desired format.
-        Parameters:
-        - n (int): Number of nodes.
-        Returns:
-        - list: List of motifs.
+        Inputs:
+        - n (int): Number of nodes in the motif.
         """
         if self.verbose == True:
             print("Generating motifs for", n, "nodes")
         motifs = []
         graphs = self.generate_graphs(n)
         node_labels = [chr(ord('A') + i) for i in range(n)]
         for graph in graphs:
             motif_str = self.matrix_to_motif(graph, node_labels)
             if motif_str not in motifs:
                 motifs.append(motif_str)
-        print("Generated", len(motifs), "motifs for", n, "nodes")
+
+        if self.verbose == True:
+            print("Generated", len(motifs), "motifs for", n, "nodes")
         return motifs
     
     def generate_required_motifs(self):
         """Generate the required motifs based on the class parameters."""
         if self.verbose == True:
             print("Generating motifs")
         motifs = {}
         if self.upto == True:
             for i in range(self.lower, self.size + 1):
                 motifs[i] = self.generate_motifs(i)
         else:
             motifs[self.size] = self.generate_motifs(self.size)
         self.motifs = motifs
 
-
-    def sanitize_filename(self, filename):
+    def sanitize_filename(self, filename: str) -> str:
         """
-        Sanitize the filename to remove invalid characters and limit length.
-        Parameters:
-        - filename (str): The filename to sanitize.
-        Returns:
-        - str: Sanitized filename.
+        Sanitize the filename by removing invalid characters and truncating it to 255 characters to prevent OS errors.
+        Inputs:
+        - filename (str): Filename to sanitize.
         """
         invalid_chars = '<>:"/\\|?*'
         for char in invalid_chars:
             filename = filename.replace(char, '')
         return filename[:255]  
     
-    def generate_unique_filename(self, edges):
+    def generate_unique_filename(self, edges: dict) -> str:
         """
-        Generate a unique filename representing the graph's edges.
-        Parameters:
-        - edges (list): List of edges in the graph.
-        - max_edges_in_name (int, optional): Maximum number of edges to include in the name. Defaults to 5.
-        Returns:
-        - str: Unique filename.
+        Generates an unique filename based on the edges of the motif.
+        Inputs:
+        - edges (list): List of edges in the motif.
         """
         simplified_edges = "_".join(f"{source}to{target}" for source, target in edges)
         filename = f"{simplified_edges}.csv"
         return self.sanitize_filename(filename)
 
-    def find_motifs(self, motif, size, save: bool = None):
+    def find_motifs(self, motif, size, save: bool = None, Executor: executors.Executor = None) -> pd.DataFrame:
         """
-        Find and optionally save motifs to a CSV file.
-        Parameters:
-        - motif (Motif): The motif to find.
+        Search for the specified motif in the graph and optionally save the results to a CSV file.
+        Inputs:
+        - motif (dotmotif.Motif): Motif to find.
         - size (int): Size of the motif.
-        - save (bool): Whether to save the motifs to a file.
+        - save (bool): Whether to save the motif to a CSV file. Defaults to None.
+        - Executor (dotmotif.executors.Executor): Executor to use for motif detection. Defaults to None.
         """
         if self.verbose == True:
-            print("Finding motifs for", size)
+            print("Finding motifs for size", size)
         if save is None: save = self.save
         if save == True:
             dir_to_save = self.path
             os.makedirs(os.path.join(dir_to_save, f"Size_{size}"), exist_ok = True)
             raw_name = [(source, target) for source, target, *_ in motif._g.edges]
             name = self.generate_unique_filename(raw_name)
-            result = self.Ex.find(motif)
+            if Executor is not None:
+                result = Executor.find(motif)
+            else:
+                result = self.Ex.find(motif)
             result_df = pd.DataFrame(result)
             result_df.to_csv(os.path.join(dir_to_save, f"Size_{size}", f"{name}"))
             if self.verbose == True:
                 print("Saved motif to", os.path.join(dir_to_save, f"Size_{size}", f"{name}"))
         else:
-            result = self.Ex.find(motif)
+            if Executor is not None:
+                result = Executor.find(motif)
+            else:
+                result = self.Ex.find(motif)
             result_df = pd.DataFrame(result)
             return result_df
     
-    def find_all_motifs(self):
+    def find_all_motifs(self) -> dict:
         """Find all motifs based on the class parameters and optionally save them to files."""
         if self.verbose == True:
             print("Finding all motifs")
         final_dict = {}
         for size, motifs in self.motifs.items():
             if self.verbose == True:
                 print("Finding motifs for size", size)
             for motif in motifs:
                 try:
                     ret_df = self.find_motifs(motif, size)
                     final_dict[motif] = ret_df
                 except ValueError as e:
                     print("Failed to generate motif", motif, "due to error:", e)
         if len(final_dict) != 0:
+            self.motifs_found = final_dict
             return final_dict
+        else:
+            raise ValueError("No motifs found")
+    
+    def generate_random_graphs(self, num_nodes: int, num_graphs: int, seed: int = None) -> list:
+        """
+        Generate random graphs for Z-Score calculation, with the probability of an edge being present
+        determined by a random value between 0 and 1.
+        Inputs:
+        - num_nodes (int): Number of nodes in the graph.
+        - num_graphs (int): Number of random graphs to generate.
+        - seed (int): Seed for random number generation for reproducibility. Defaults to None.
+        """
+        if self.verbose == True:
+            print("Generating random graphs")
+        graphs = []
+        if seed is not None:
+            np.random.seed(seed)
+        for i in range(num_graphs):
+            if i % (num_graphs // 10) == 0 and self.verbose == True:
+                print(f"Generated {i} random graphs out of {num_graphs}")
+            p = np.random.rand()
+            graph = nx.fast_gnp_random_graph(num_nodes, p, directed = self.directed, seed = seed)
+            graph.remove_edges_from(nx.selfloop_edges(graph))
+            graphs.append(graph)
+        return graphs
+
+    def calculate_zscore(self, num_random_graphs: int = 100, Executor: executors.Executor = executors.GrandIsoExecutor ,seed: int = None) -> dict:
+        """
+        Method to calculate the Z-Scores for each motif based on the number of motifs found in random graphs.
+        Inputs:
+        - num_random_graphs (int): Number of random graphs to generate. Defaults to 100.
+        - Executor (dotmotif.executors.Executor): Executor to use for motif detection. Defaults to GrandIsoExecutor.
+        - seed (int): Seed for random number generation. Defaults to None.
+        Returns:
+        - dict: Dictionary containing the Z-Scores for each motif.
+        - Saves the Z-Scores to a CSV file if save is set to True.
+        """
+        if self.verbose == True:
+            print("Calculating Z-Scores")
+        num_nodes = len(self.Graph.nodes)
+        graphs = self.generate_random_graphs(num_nodes, num_random_graphs, seed)
+        if self.verbose == True:
+            print("Generated random graphs")
+        actual_motifs = self.find_all_motifs() if self.motifs_found is None else self.motifs_found
+        actual_motif_counts = {motif: len(df) for motif, df in actual_motifs.items()}
+        random_motif_counts = {motif: [] for motif in actual_motifs.keys()}
+        if self.verbose == True:
+            print("Finding motifs in random graphs")
+        for graph in graphs:
+            for motif in actual_motifs.keys():
+                try:
+                    executor = Executor(graph = graph)
+                    result = self.find_motifs(motif, len(motif._g.nodes), save = False, Executor = executor)
+                    random_motif_counts[motif].append(len(result))
+                except ValueError as e:
+                    print("Failed to generate motif", motif, "due to error:", e)
+        if self.verbose == True:
+            print("Calculating Z-Scores")
+        motif_zscores = {}
+        for motif, counts in random_motif_counts.items():
+            actual_count = actual_motif_counts[motif]
+            mean = np.mean(counts)
+            std = np.std(counts)
+            zscore = (actual_count - mean) / std
+            motif_zscores[motif] = zscore
+        if self.verbose == True:
+            print("Z-Scores calculated")
+        if self.save:
+            if self.verbose == True:
+                print("Saving Z-Scores")
+            dir_to_save = self.path
+            os.makedirs(os.path.join(dir_to_save, "ZScores"), exist_ok = True)
+            zscore_df = pd.DataFrame(motif_zscores.items(), columns = ["Motif", "ZScore"])
+            zscore_df.to_csv(os.path.join(dir_to_save, "ZScores", "ZScores.csv"))
+        return motif_zscores
```

### Comparing `automotifs-1.0.3/automotifs.egg-info/PKG-INFO` & `automotifs-1.1/automotifs.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.0.3
+Version: 1.1
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,40 +12,43 @@
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
-AutoMotif helps you find patterns, called motifs, in network graphs. It uses NetworkX for working with graphs, dotmotif for finding the patterns, and pandas for handling data. Whether your graphs are directed or not, AutoMotif can search for motifs based on the criteria you set, like motif size and whether to consider pattern repetitions (automorphisms).
+AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 ## Installation
 
 ```bash
 pip install automotifs
 ```
 ## Quick Start
 ```python
 from automotif import AutoMotif
+from dotmotif import executors
 import networkx as nx
 # Example: A random directed graph
 G = nx.gnp_random_graph(100, 0.5, directed=True)
 # Set up AutoMotif
-motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True)
+motif_finder = AutoMotif(Graph=G, size=3, directed=True, verbose=True, use_GrandISO = True)
 # Start finding motifs
 motifs = motif_finder.find_all_motifs()
+# Calculate the Z-Score for the motifs
+z_scores = motif_finder.calculate_zscore(num_random_graphs = 30, Executor = executors.NetworkXExecutor)
 ```
 ## Features
-- Automated Detection: Find motifs in your network without manually tweaking every parameter. AutoMotif takes care of the heavy lifting.
-- Flexibility: Whether your networks are directed or undirected, AutoMotif can handle them. Plus, you can decide if you want to look for automorphisms and set the size of motifs to search for.
-- Save for Later: Directly save your findings to CSV files, making it easier to analyze results or share them with others.
+- **Automated Detection**: AutoMotif automates the detection of motifs, eliminating the need for manual parameter adjustments. It's designed to be efficient and user-friendly, allowing researchers to focus more on analysis and less on setup.
+- **Flexible and Powerful**: Capable of handling both directed and undirected graphs, AutoMotif provides flexibility in defining motifs, including size and whether to consider automorphisms, ensuring a broad applicability across different types of network analyses.
+- **Data Organization and Export**: Directly save your motifs to CSV files for easy access, further analysis, or sharing with your team or research community.
+- **Z-Score Calculation**: Assess the statistical significance of detected motifs by calculating their Z-scores, providing insights into the rarity or commonality of patterns within your network compared to random expectations.
 ## Contributions
-Contributions to AutoMotif are welcome! If you have suggestions for improvement or new features, feel free to open an issue or submit a pull request.
+We encourage contributions to AutoMotif! If you have ideas for improvements or new features, don't hesitate to open an issue or submit a pull request on our repository.
 ## License
 AutoMotif is made available under the MIT License. See the LICENSE file for more details.
 ***
 ## Who made this? 
-Giorgio Micaletto, under Professor Marta Zava's supervision at Bocconi University, put together AutoMotif. It was created to make network motif analysis less of a headache.
-
+AutoMotif was developed by Giorgio Micaletto under the guidance of Professor Marta Zava at Bocconi University. This tool is designed to simplify and facilitate the complex process of network motif analysis.
 Contacts:
 - giorgio.micaletto@studbocconi.it
-- linkedin.com/in/giorgio-micaletto/
+- [linkedin](linkedin.com/in/giorgio-micaletto/)
```

### Comparing `automotifs-1.0.3/setup.py` & `automotifs-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This module sets up the package for distribution."""
 from setuptools import setup, find_packages
 setup(
     name='automotifs',
-    version='1.0.3',
+    version='1.1',
     packages=find_packages(),
     description='A wrapper for automatic Motif Detection',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/auto_dotmotif/',
```

### Comparing `automotifs-1.0.3/tests/test.py` & `automotifs-1.1/tests/test.py`

 * *Files identical despite different names*

