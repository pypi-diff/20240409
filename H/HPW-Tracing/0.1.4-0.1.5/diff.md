# Comparing `tmp/HPW_Tracing-0.1.4.tar.gz` & `tmp/HPW_Tracing-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HPW_Tracing-0.1.4.tar", last modified: Fri Apr  5 19:29:19 2024, max compression
+gzip compressed data, was "HPW_Tracing-0.1.5.tar", last modified: Tue Apr  9 15:35:10 2024, max compression
```

## Comparing `HPW_Tracing-0.1.4.tar` & `HPW_Tracing-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.395591 HPW_Tracing-0.1.4/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.353813 HPW_Tracing-0.1.4/HPW_Tracing/
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.365016 HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/
--rw-rw-rw-   0        0        0       48 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/__init__.py
--rw-rw-rw-   0        0        0     2679 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/make_graph.py
--rw-rw-rw-   0        0        0    13216 2024-04-04 19:25:14.000000 HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/network_correction.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.369831 HPW_Tracing-0.1.4/HPW_Tracing/Load_data/
--rw-rw-rw-   0        0        0       32 2024-04-04 14:56:41.000000 HPW_Tracing-0.1.4/HPW_Tracing/Load_data/__init__.py
--rw-rw-rw-   0        0        0     2486 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.4/HPW_Tracing/Load_data/load_data.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.375935 HPW_Tracing-0.1.4/HPW_Tracing/Tracing/
--rw-rw-rw-   0        0        0     7356 2024-04-04 20:36:27.000000 HPW_Tracing-0.1.4/HPW_Tracing/Tracing/Tracing_with_distance.py
--rw-rw-rw-   0        0        0      176 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.4/HPW_Tracing/Tracing/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-04 20:11:50.000000 HPW_Tracing-0.1.4/HPW_Tracing/Tracing/mh_name_ufid_lookup.py
--rw-rw-rw-   0        0        0        8 2024-04-04 18:50:07.000000 HPW_Tracing-0.1.4/HPW_Tracing/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.360953 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/
--rw-rw-rw-   0        0        0      362 2024-04-05 19:29:19.000000 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-04-05 19:29:19.000000 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 19:29:19.000000 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2024-04-05 19:29:19.000000 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 19:29:19.000000 HPW_Tracing-0.1.4/HPW_Tracing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      362 2024-04-05 19:29:19.393555 HPW_Tracing-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-05 19:29:19.395591 HPW_Tracing-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      574 2024-04-05 19:29:05.000000 HPW_Tracing-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 19:29:19.390829 HPW_Tracing-0.1.4/test/
--rw-rw-rw-   0        0        0      671 2024-04-04 20:21:14.000000 HPW_Tracing-0.1.4/test/test.py
--rw-rw-rw-   0        0        0      586 2024-03-27 19:25:12.000000 HPW_Tracing-0.1.4/test/test_1_tracing_with_nodes.py
--rw-rw-rw-   0        0        0      303 2024-03-27 19:28:52.000000 HPW_Tracing-0.1.4/test/test_2_tracing_with_links.py
--rw-rw-rw-   0        0        0      294 2024-03-27 19:33:05.000000 HPW_Tracing-0.1.4/test/test_3_tracing_between_nodes.py
--rw-rw-rw-   0        0        0      190 2024-03-27 19:40:19.000000 HPW_Tracing-0.1.4/test/test_4_tracing_between_links.py
--rw-rw-rw-   0        0        0     1810 2024-04-04 13:52:51.000000 HPW_Tracing-0.1.4/test/test_load_gis_data_from_warehouse.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.227252 HPW_Tracing-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.129299 HPW_Tracing-0.1.5/HPW_Tracing/
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.142300 HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/
+-rw-rw-rw-   0        0        0       48 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/__init__.py
+-rw-rw-rw-   0        0        0     2679 2024-04-04 21:09:08.000000 HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/make_graph.py
+-rw-rw-rw-   0        0        0    13216 2024-04-04 19:25:14.000000 HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/network_correction.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.161302 HPW_Tracing-0.1.5/HPW_Tracing/Load_data/
+-rw-rw-rw-   0        0        0       32 2024-04-04 14:56:41.000000 HPW_Tracing-0.1.5/HPW_Tracing/Load_data/__init__.py
+-rw-rw-rw-   0        0        0     2486 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.5/HPW_Tracing/Load_data/load_data.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.168300 HPW_Tracing-0.1.5/HPW_Tracing/Tracing/
+-rw-rw-rw-   0        0        0     7359 2024-04-09 15:33:37.000000 HPW_Tracing-0.1.5/HPW_Tracing/Tracing/Tracing_with_distance.py
+-rw-rw-rw-   0        0        0      176 2024-04-04 19:19:16.000000 HPW_Tracing-0.1.5/HPW_Tracing/Tracing/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-04 20:11:50.000000 HPW_Tracing-0.1.5/HPW_Tracing/Tracing/mh_name_ufid_lookup.py
+-rw-rw-rw-   0        0        0        8 2024-04-04 18:50:07.000000 HPW_Tracing-0.1.5/HPW_Tracing/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.137303 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/
+-rw-rw-rw-   0        0        0      362 2024-04-09 15:35:09.000000 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-04-09 15:35:10.000000 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:35:09.000000 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-04-09 15:35:09.000000 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 15:35:09.000000 HPW_Tracing-0.1.5/HPW_Tracing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      362 2024-04-09 15:35:10.223129 HPW_Tracing-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:35:10.227252 HPW_Tracing-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      574 2024-04-09 15:34:12.000000 HPW_Tracing-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:35:10.221130 HPW_Tracing-0.1.5/test/
+-rw-rw-rw-   0        0        0      671 2024-04-04 20:21:14.000000 HPW_Tracing-0.1.5/test/test.py
+-rw-rw-rw-   0        0        0      586 2024-03-27 19:25:12.000000 HPW_Tracing-0.1.5/test/test_1_tracing_with_nodes.py
+-rw-rw-rw-   0        0        0      303 2024-03-27 19:28:52.000000 HPW_Tracing-0.1.5/test/test_2_tracing_with_links.py
+-rw-rw-rw-   0        0        0      294 2024-03-27 19:33:05.000000 HPW_Tracing-0.1.5/test/test_3_tracing_between_nodes.py
+-rw-rw-rw-   0        0        0      190 2024-03-27 19:40:19.000000 HPW_Tracing-0.1.5/test/test_4_tracing_between_links.py
+-rw-rw-rw-   0        0        0     1810 2024-04-04 13:52:51.000000 HPW_Tracing-0.1.5/test/test_load_gis_data_from_warehouse.py
```

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/make_graph.py` & `HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/make_graph.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing/Build_graphs/network_correction.py` & `HPW_Tracing-0.1.5/HPW_Tracing/Build_graphs/network_correction.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing/Load_data/load_data.py` & `HPW_Tracing-0.1.5/HPW_Tracing/Load_data/load_data.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing/Tracing/Tracing_with_distance.py` & `HPW_Tracing-0.1.5/HPW_Tracing/Tracing/Tracing_with_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,17 @@
             return tracing_with_node_short_distance(graph, start_node, direction, distance)
 
     # Reverse the graph if tracing upstream
     if direction == 'upstream':
         graph = graph.reverse()
 
     # Perform BFS in the specified direction
-    bfs_edges = list(nx.bfs_edges(graph, start_node))
+    bfs_edges = list(nx.edge_bfs(graph, start_node))
+
+
     node_distances = nx.single_source_dijkstra_path_length(graph, start_node, weight='length')
 
     # Filter edges based on distance condition
     if distance is not None:
         bfs_edges = [edge for edge in bfs_edges if node_distances[edge[1]] <= distance]
         node_distances = {node: distance_node for node, distance_node in node_distances.items() if distance_node <= distance}
```

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing/Tracing/mh_name_ufid_lookup.py` & `HPW_Tracing-0.1.5/HPW_Tracing/Tracing/mh_name_ufid_lookup.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/HPW_Tracing.egg-info/SOURCES.txt` & `HPW_Tracing-0.1.5/HPW_Tracing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/setup.py` & `HPW_Tracing-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 
 
 setup(
     name='HPW_Tracing',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.9',
```

### Comparing `HPW_Tracing-0.1.4/test/test.py` & `HPW_Tracing-0.1.5/test/test.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/test/test_1_tracing_with_nodes.py` & `HPW_Tracing-0.1.5/test/test_1_tracing_with_nodes.py`

 * *Files identical despite different names*

### Comparing `HPW_Tracing-0.1.4/test/test_load_gis_data_from_warehouse.py` & `HPW_Tracing-0.1.5/test/test_load_gis_data_from_warehouse.py`

 * *Files identical despite different names*

