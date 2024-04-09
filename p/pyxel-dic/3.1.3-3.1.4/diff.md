# Comparing `tmp/pyxel-dic-3.1.3.tar.gz` & `tmp/pyxel-dic-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel-dic-3.1.3.tar", last modified: Mon Apr  8 13:09:18 2024, max compression
+gzip compressed data, was "pyxel-dic-3.1.4.tar", last modified: Mon Apr  8 13:20:37 2024, max compression
```

## Comparing `pyxel-dic-3.1.3.tar` & `pyxel-dic-3.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.807938 pyxel-dic-3.1.3/
--rw-rw-rw-   0        0        0     3197 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/LICENSE
--rw-rw-rw-   0        0        0     8950 2024-04-08 13:09:18.799238 pyxel-dic-3.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4247 2023-12-14 07:13:45.000000 pyxel-dic-3.1.3/README.md
--rw-rw-rw-   0        0        0      833 2024-04-08 13:07:36.000000 pyxel-dic-3.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      898 2024-04-08 13:09:18.811027 pyxel-dic-3.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.540295 pyxel-dic-3.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.745679 pyxel-dic-3.1.3/src/pyxel/
--rw-rw-rw-   0        0        0      409 2023-09-26 15:49:25.000000 pyxel-dic-3.1.3/src/pyxel/__init__.py
--rw-rw-rw-   0        0        0    29337 2023-10-10 15:10:56.000000 pyxel-dic-3.1.3/src/pyxel/bspline_patch.py
--rw-rw-rw-   0        0        0    41545 2023-10-10 15:14:01.000000 pyxel-dic-3.1.3/src/pyxel/bspline_routines.py
--rw-rw-rw-   0        0        0    32075 2024-03-21 10:29:35.000000 pyxel-dic-3.1.3/src/pyxel/camera.py
--rw-rw-rw-   0        0        0    25572 2024-03-20 21:54:51.000000 pyxel-dic-3.1.3/src/pyxel/dic.py
--rw-rw-rw-   0        0        0     2317 2023-12-14 15:57:00.000000 pyxel-dic-3.1.3/src/pyxel/exportpixmap.py
--rw-rw-rw-   0        0        0    15430 2024-01-23 18:19:07.000000 pyxel-dic-3.1.3/src/pyxel/image.py
--rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/levelset.py
--rw-rw-rw-   0        0        0     5908 2024-03-06 07:09:44.000000 pyxel-dic-3.1.3/src/pyxel/material.py
--rw-rw-rw-   0        0        0   139712 2024-04-08 13:01:41.000000 pyxel-dic-3.1.3/src/pyxel/mesh.py
--rw-rw-rw-   0        0        0    24345 2024-02-09 21:11:50.000000 pyxel-dic-3.1.3/src/pyxel/mesher.py
--rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/meshparser.py
--rw-rw-rw-   0        0        0     3926 2024-01-23 18:23:13.000000 pyxel-dic-3.1.3/src/pyxel/utils.py
--rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.1.3/src/pyxel/vtktools.py
-drwxrwxrwx   0        0        0        0 2024-04-08 13:09:18.793199 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/
--rw-rw-rw-   0        0        0     8950 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-08 13:09:18.000000 pyxel-dic-3.1.3/src/pyxel_dic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 13:20:37.940134 pyxel-dic-3.1.4/
+-rw-rw-rw-   0        0        0     3197 2023-04-17 15:11:38.000000 pyxel-dic-3.1.4/LICENSE
+-rw-rw-rw-   0        0        0     8950 2024-04-08 13:20:37.932672 pyxel-dic-3.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4247 2023-12-14 07:13:45.000000 pyxel-dic-3.1.4/README.md
+-rw-rw-rw-   0        0        0      833 2024-04-08 13:20:19.000000 pyxel-dic-3.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      898 2024-04-08 13:20:37.944050 pyxel-dic-3.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 13:20:37.735401 pyxel-dic-3.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 13:20:37.885716 pyxel-dic-3.1.4/src/pyxel/
+-rw-rw-rw-   0        0        0      409 2023-09-26 15:49:25.000000 pyxel-dic-3.1.4/src/pyxel/__init__.py
+-rw-rw-rw-   0        0        0    29337 2023-10-10 15:10:56.000000 pyxel-dic-3.1.4/src/pyxel/bspline_patch.py
+-rw-rw-rw-   0        0        0    41545 2023-10-10 15:14:01.000000 pyxel-dic-3.1.4/src/pyxel/bspline_routines.py
+-rw-rw-rw-   0        0        0    32075 2024-03-21 10:29:35.000000 pyxel-dic-3.1.4/src/pyxel/camera.py
+-rw-rw-rw-   0        0        0    25572 2024-03-20 21:54:51.000000 pyxel-dic-3.1.4/src/pyxel/dic.py
+-rw-rw-rw-   0        0        0     2317 2023-12-14 15:57:00.000000 pyxel-dic-3.1.4/src/pyxel/exportpixmap.py
+-rw-rw-rw-   0        0        0    15430 2024-01-23 18:19:07.000000 pyxel-dic-3.1.4/src/pyxel/image.py
+-rw-rw-rw-   0        0        0     9658 2023-04-17 15:11:38.000000 pyxel-dic-3.1.4/src/pyxel/levelset.py
+-rw-rw-rw-   0        0        0     5908 2024-03-06 07:09:44.000000 pyxel-dic-3.1.4/src/pyxel/material.py
+-rw-rw-rw-   0        0        0   139704 2024-04-08 13:20:10.000000 pyxel-dic-3.1.4/src/pyxel/mesh.py
+-rw-rw-rw-   0        0        0    24345 2024-02-09 21:11:50.000000 pyxel-dic-3.1.4/src/pyxel/mesher.py
+-rw-rw-rw-   0        0        0     6859 2023-04-17 15:11:38.000000 pyxel-dic-3.1.4/src/pyxel/meshparser.py
+-rw-rw-rw-   0        0        0     3926 2024-01-23 18:23:13.000000 pyxel-dic-3.1.4/src/pyxel/utils.py
+-rw-rw-rw-   0        0        0    16353 2023-04-17 15:11:38.000000 pyxel-dic-3.1.4/src/pyxel/vtktools.py
+drwxrwxrwx   0        0        0        0 2024-04-08 13:20:37.926625 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/
+-rw-rw-rw-   0        0        0     8950 2024-04-08 13:20:37.000000 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-08 13:20:37.000000 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 13:20:37.000000 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-08 13:20:37.000000 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-08 13:20:37.000000 pyxel-dic-3.1.4/src/pyxel_dic.egg-info/top_level.txt
```

### Comparing `pyxel-dic-3.1.3/LICENSE` & `pyxel-dic-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/PKG-INFO` & `pyxel-dic-3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.1.3
+Version: 3.1.4
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
```

### Comparing `pyxel-dic-3.1.3/README.md` & `pyxel-dic-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/pyproject.toml` & `pyxel-dic-3.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools==68.2.2",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyxel-dic"
-version = "3.1.3"
+version = "3.1.4"
 authors = [
   { name="JC Passieux", email="jc.passieux@gmail.com" },
 ]
 description = "Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyxel-dic-3.1.3/setup.cfg` & `pyxel-dic-3.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/bspline_patch.py` & `pyxel-dic-3.1.4/src/pyxel/bspline_patch.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/bspline_routines.py` & `pyxel-dic-3.1.4/src/pyxel/bspline_routines.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/camera.py` & `pyxel-dic-3.1.4/src/pyxel/camera.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/dic.py` & `pyxel-dic-3.1.4/src/pyxel/dic.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/exportpixmap.py` & `pyxel-dic-3.1.4/src/pyxel/exportpixmap.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/image.py` & `pyxel-dic-3.1.4/src/pyxel/image.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/levelset.py` & `pyxel-dic-3.1.4/src/pyxel/levelset.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/material.py` & `pyxel-dic-3.1.4/src/pyxel/material.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/mesh.py` & `pyxel-dic-3.1.4/src/pyxel/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -3444,11 +3444,11 @@
                     rep = np.arange(nec[eti]) + ielem * nec[eti]
                     eg[eti][rep, :] = mc.e[eti] + ielem * nnc
                 ielem += 1
         mg = Mesh(eg, ng, self.dim)
         print('Removing Unused nodes...')
         mg.RemoveUnusedNodes()
         print('Removing Double nodes...')
-        mg.RemoveDoubleNodes(eps=3e-5)
+        mg.RemoveDoubleNodes()
         print('Removing Double Elements...')
         mg.RemoveDoubleElems()
         return mg
```

### Comparing `pyxel-dic-3.1.3/src/pyxel/mesher.py` & `pyxel-dic-3.1.4/src/pyxel/mesher.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/meshparser.py` & `pyxel-dic-3.1.4/src/pyxel/meshparser.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/utils.py` & `pyxel-dic-3.1.4/src/pyxel/utils.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel/vtktools.py` & `pyxel-dic-3.1.4/src/pyxel/vtktools.py`

 * *Files identical despite different names*

### Comparing `pyxel-dic-3.1.3/src/pyxel_dic.egg-info/PKG-INFO` & `pyxel-dic-3.1.4/src/pyxel_dic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-dic
-Version: 3.1.3
+Version: 3.1.4
 Summary: Finite Element (FE) Digital Image/Volume Correlation (DIC/DVC) library for experimental mechanics
 Home-page: https://github.com/jcpassieux/pyxel
 Author: Jean-Charles Passieux
 Author-email: JC Passieux <jc.passieux@gmail.com>
 License: 
           CeCILL FREE SOFTWARE LICENSE AGREEMENT
```

### Comparing `pyxel-dic-3.1.3/src/pyxel_dic.egg-info/SOURCES.txt` & `pyxel-dic-3.1.4/src/pyxel_dic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

