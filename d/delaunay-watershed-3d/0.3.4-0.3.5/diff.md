# Comparing `tmp/delaunay_watershed_3d-0.3.4.tar.gz` & `tmp/delaunay_watershed_3d-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_watershed_3d-0.3.4.tar", last modified: Wed Apr  3 13:48:41 2024, max compression
+gzip compressed data, was "delaunay_watershed_3d-0.3.5.tar", last modified: Tue Apr  9 13:43:23 2024, max compression
```

## Comparing `delaunay_watershed_3d-0.3.4.tar` & `delaunay_watershed_3d-0.3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/
--rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/PKG-INFO
--rw-r--r--   0 perez     (1000) perez     (1000)     7069 2024-03-12 15:12:15.000000 delaunay_watershed_3d-0.3.4/README.md
--rw-r--r--   0 perez     (1000) perez     (1000)     1202 2024-02-13 09:09:41.000000 delaunay_watershed_3d-0.3.4/pyproject.toml
--rw-r--r--   0 perez     (1000) perez     (1000)     1072 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/setup.cfg
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.130415 delaunay_watershed_3d-0.3.4/src/
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 perez     (1000) perez     (1000)      673 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 perez     (1000) perez     (1000)        1 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 perez     (1000) perez     (1000)      163 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 perez     (1000) perez     (1000)        5 2024-04-03 13:48:41.000000 delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-03 13:48:41.133749 delaunay_watershed_3d-0.3.4/src/dw3d/
--rw-r--r--   0 perez     (1000) perez     (1000)     2513 2024-03-12 15:11:52.000000 delaunay_watershed_3d-0.3.4/src/dw3d/__init__.py
--rw-r--r--   0 perez     (1000) perez     (1000)     7400 2024-04-03 13:09:24.000000 delaunay_watershed_3d-0.3.4/src/dw3d/edt.py
--rw-r--r--   0 perez     (1000) perez     (1000)     8708 2024-03-12 15:19:46.000000 delaunay_watershed_3d-0.3.4/src/dw3d/io.py
--rw-r--r--   0 perez     (1000) perez     (1000)     4089 2024-03-11 16:02:21.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mask_reconstruction.py
--rw-r--r--   0 perez     (1000) perez     (1000)    12150 2024-03-27 14:21:14.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mesh_surgery.py
--rw-r--r--   0 perez     (1000) perez     (1000)     9302 2024-03-27 13:46:03.000000 delaunay_watershed_3d-0.3.4/src/dw3d/mesh_utilities.py
--rw-r--r--   0 perez     (1000) perez     (1000)     4958 2024-04-03 13:37:02.000000 delaunay_watershed_3d-0.3.4/src/dw3d/points_on_edt.py
--rw-r--r--   0 perez     (1000) perez     (1000)    11143 2024-04-03 13:00:16.000000 delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm.py
--rw-r--r--   0 perez     (1000) perez     (1000)     7981 2024-04-03 13:22:43.000000 delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm_factory.py
--rw-r--r--   0 perez     (1000) perez     (1000)     4161 2024-03-11 10:43:52.000000 delaunay_watershed_3d-0.3.4/src/dw3d/score_computation.py
--rw-r--r--   0 perez     (1000) perez     (1000)     1835 2024-03-08 08:45:06.000000 delaunay_watershed_3d-0.3.4/src/dw3d/segmentation.py
--rw-r--r--   0 perez     (1000) perez     (1000)      894 2024-03-11 14:41:02.000000 delaunay_watershed_3d-0.3.4/src/dw3d/tesselation.py
--rw-r--r--   0 perez     (1000) perez     (1000)     9637 2024-03-27 10:37:08.000000 delaunay_watershed_3d-0.3.4/src/dw3d/tesselation_graph.py
--rw-r--r--   0 perez     (1000) perez     (1000)     7919 2024-04-03 09:18:03.000000 delaunay_watershed_3d-0.3.4/src/dw3d/viewing.py
--rw-r--r--   0 perez     (1000) perez     (1000)     3797 2024-03-25 10:44:46.000000 delaunay_watershed_3d-0.3.4/src/dw3d/watershed.py
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-09 13:43:23.138725 delaunay_watershed_3d-0.3.5/
+-rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-09 13:43:23.138725 delaunay_watershed_3d-0.3.5/PKG-INFO
+-rw-r--r--   0 perez     (1000) perez     (1000)     7069 2024-03-12 15:12:15.000000 delaunay_watershed_3d-0.3.5/README.md
+-rw-r--r--   0 perez     (1000) perez     (1000)     1202 2024-02-13 09:09:41.000000 delaunay_watershed_3d-0.3.5/pyproject.toml
+-rw-r--r--   0 perez     (1000) perez     (1000)     1072 2024-04-09 13:43:23.138725 delaunay_watershed_3d-0.3.5/setup.cfg
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-09 13:43:23.135391 delaunay_watershed_3d-0.3.5/src/
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-09 13:43:23.135391 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 perez     (1000) perez     (1000)     8145 2024-04-09 13:43:23.000000 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 perez     (1000) perez     (1000)      673 2024-04-09 13:43:23.000000 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)        1 2024-04-09 13:43:23.000000 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)      162 2024-04-09 13:43:23.000000 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 perez     (1000) perez     (1000)        5 2024-04-09 13:43:23.000000 delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 perez     (1000) perez     (1000)        0 2024-04-09 13:43:23.135391 delaunay_watershed_3d-0.3.5/src/dw3d/
+-rw-r--r--   0 perez     (1000) perez     (1000)     2513 2024-03-12 15:11:52.000000 delaunay_watershed_3d-0.3.5/src/dw3d/__init__.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7400 2024-04-03 13:09:24.000000 delaunay_watershed_3d-0.3.5/src/dw3d/edt.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     8708 2024-03-12 15:19:46.000000 delaunay_watershed_3d-0.3.5/src/dw3d/io.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4089 2024-03-11 16:02:21.000000 delaunay_watershed_3d-0.3.5/src/dw3d/mask_reconstruction.py
+-rw-r--r--   0 perez     (1000) perez     (1000)    12150 2024-03-27 14:21:14.000000 delaunay_watershed_3d-0.3.5/src/dw3d/mesh_surgery.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     9302 2024-03-27 13:46:03.000000 delaunay_watershed_3d-0.3.5/src/dw3d/mesh_utilities.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4958 2024-04-03 13:37:02.000000 delaunay_watershed_3d-0.3.5/src/dw3d/points_on_edt.py
+-rw-r--r--   0 perez     (1000) perez     (1000)    11143 2024-04-03 13:00:16.000000 delaunay_watershed_3d-0.3.5/src/dw3d/reconstruction_algorithm.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7981 2024-04-03 13:22:43.000000 delaunay_watershed_3d-0.3.5/src/dw3d/reconstruction_algorithm_factory.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     4161 2024-03-11 10:43:52.000000 delaunay_watershed_3d-0.3.5/src/dw3d/score_computation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     1835 2024-03-08 08:45:06.000000 delaunay_watershed_3d-0.3.5/src/dw3d/segmentation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)      894 2024-03-11 14:41:02.000000 delaunay_watershed_3d-0.3.5/src/dw3d/tesselation.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     9637 2024-03-27 10:37:08.000000 delaunay_watershed_3d-0.3.5/src/dw3d/tesselation_graph.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     7919 2024-04-03 09:18:03.000000 delaunay_watershed_3d-0.3.5/src/dw3d/viewing.py
+-rw-r--r--   0 perez     (1000) perez     (1000)     3797 2024-03-25 10:44:46.000000 delaunay_watershed_3d-0.3.5/src/dw3d/watershed.py
```

### Comparing `delaunay_watershed_3d-0.3.4/PKG-INFO` & `delaunay_watershed_3d-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.3.4
+Version: 0.3.5
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Maintainer: Matthieu Perez
 Maintainer-email: matthieu.perez@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: edt>=2.2.0
+Requires-Dist: edt>=2.4.0
 Requires-Dist: meshio>=5.3.4
-Requires-Dist: networkx>=2.5.1
-Requires-Dist: numpy>=1.21.6
-Requires-Dist: scikit-image>=0.18.3
-Requires-Dist: scipy>=1.4.1
-Requires-Dist: trimesh>=3.8.12
+Requires-Dist: networkx>=2.8.0
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: scikit-image>=0.20.0
+Requires-Dist: scipy>=1.9.3
+Requires-Dist: trimesh>=4.0.0
 Provides-Extra: viewing
 Requires-Dist: napari[all]; extra == "viewing"
 Requires-Dist: polyscope>=1.2.0; extra == "viewing"
 Requires-Dist: matplotlib>=3.3.1; extra == "viewing"
 
 # Delaunay-Watershed 3D
```

### Comparing `delaunay_watershed_3d-0.3.4/README.md` & `delaunay_watershed_3d-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/pyproject.toml` & `delaunay_watershed_3d-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/setup.cfg` & `delaunay_watershed_3d-0.3.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.3.4
+version = 0.3.5
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 maintainer = Matthieu Perez
 maintainer_email = matthieu.perez@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -19,22 +19,22 @@
 license = CC BY-NC-SA 4.0
 
 [options]
 include_package_data = True
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
-install_requires = edt>=2.2.0
+python_requires = >=3.10
+install_requires = edt>=2.4.0
 	meshio>=5.3.4
-	networkx>=2.5.1
-	numpy>=1.21.6
-	scikit-image>=0.18.3
-	scipy>=1.4.1
-	trimesh>=3.8.12
+	networkx>=2.8.0
+	numpy>=1.24.0
+	scikit-image>=0.20.0
+	scipy>=1.9.3
+	trimesh>=4.0.0
 
 [options.extras_require]
 viewing = napari[all]
 	polyscope>=1.2.0
 	matplotlib>=3.3.1
 
 [options.packages.find]
```

### Comparing `delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: delaunay_watershed_3d
-Version: 0.3.4
+Version: 0.3.5
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Maintainer: Matthieu Perez
 Maintainer-email: matthieu.perez@college-de-france.fr
 License: CC BY-NC-SA 4.0
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: edt>=2.2.0
+Requires-Dist: edt>=2.4.0
 Requires-Dist: meshio>=5.3.4
-Requires-Dist: networkx>=2.5.1
-Requires-Dist: numpy>=1.21.6
-Requires-Dist: scikit-image>=0.18.3
-Requires-Dist: scipy>=1.4.1
-Requires-Dist: trimesh>=3.8.12
+Requires-Dist: networkx>=2.8.0
+Requires-Dist: numpy>=1.24.0
+Requires-Dist: scikit-image>=0.20.0
+Requires-Dist: scipy>=1.9.3
+Requires-Dist: trimesh>=4.0.0
 Provides-Extra: viewing
 Requires-Dist: napari[all]; extra == "viewing"
 Requires-Dist: polyscope>=1.2.0; extra == "viewing"
 Requires-Dist: matplotlib>=3.3.1; extra == "viewing"
 
 # Delaunay-Watershed 3D
```

### Comparing `delaunay_watershed_3d-0.3.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.3.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/__init__.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/__init__.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/edt.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/edt.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/io.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/io.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/mask_reconstruction.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/mesh_surgery.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/mesh_surgery.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/mesh_utilities.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/points_on_edt.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/points_on_edt.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/reconstruction_algorithm.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/reconstruction_algorithm_factory.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/reconstruction_algorithm_factory.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/score_computation.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/score_computation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/segmentation.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/segmentation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/tesselation.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/tesselation.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/tesselation_graph.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/tesselation_graph.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/viewing.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/viewing.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.3.4/src/dw3d/watershed.py` & `delaunay_watershed_3d-0.3.5/src/dw3d/watershed.py`

 * *Files identical despite different names*

