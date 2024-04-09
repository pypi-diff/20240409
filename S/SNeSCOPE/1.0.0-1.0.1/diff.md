# Comparing `tmp/SNeSCOPE-1.0.0.tar.gz` & `tmp/SNeSCOPE-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SNeSCOPE-1.0.0.tar", last modified: Sun Apr  7 14:27:10 2024, max compression
+gzip compressed data, was "dist\SNeSCOPE-1.0.1.tar", last modified: Tue Apr  9 12:19:55 2024, max compression
```

## Comparing `SNeSCOPE-1.0.0.tar` & `SNeSCOPE-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/
--rw-rw-rw-   0        0        0    11544 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      321 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1683 2024-04-02 22:21:58.000000 SNeSCOPE-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-04-07 14:04:34.000000 SNeSCOPE-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE/
--rw-rw-rw-   0        0        0   100299 2024-04-07 12:54:24.000000 SNeSCOPE-1.0.0/SNeSCOPE/blackbody_tools.py
--rw-rw-rw-   0        0        0    28973 2024-04-01 10:29:56.000000 SNeSCOPE-1.0.0/SNeSCOPE/PhotoUtils.py
--rw-rw-rw-   0        0        0        0 2024-03-28 15:42:27.000000 SNeSCOPE-1.0.0/SNeSCOPE/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      321 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/requires.txt
--rw-rw-rw-   0        0        0      272 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 14:27:10.000000 SNeSCOPE-1.0.0/SNeSCOPE.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 12:19:55.000000 SNeSCOPE-1.0.1/
+-rw-rw-rw-   0        0        0    11544 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      321 2024-04-09 12:19:55.000000 SNeSCOPE-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-04-01 10:32:33.000000 SNeSCOPE-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1683 2024-04-02 22:21:58.000000 SNeSCOPE-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 12:19:55.000000 SNeSCOPE-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-09 12:19:40.000000 SNeSCOPE-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE/
+-rw-rw-rw-   0        0        0   100299 2024-04-09 12:06:26.000000 SNeSCOPE-1.0.1/SNeSCOPE/blackbody_tools.py
+-rw-rw-rw-   0        0        0    28973 2024-04-01 10:29:56.000000 SNeSCOPE-1.0.1/SNeSCOPE/PhotoUtils.py
+-rw-rw-rw-   0        0        0        0 2024-03-28 15:42:27.000000 SNeSCOPE-1.0.1/SNeSCOPE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 12:19:55.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      321 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      272 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2024-04-09 12:19:54.000000 SNeSCOPE-1.0.1/SNeSCOPE.egg-info/top_level.txt
```

### Comparing `SNeSCOPE-1.0.0/LICENSE` & `SNeSCOPE-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.0/pyproject.toml` & `SNeSCOPE-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.0/README.md` & `SNeSCOPE-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.0/setup.py` & `SNeSCOPE-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 description='SNeSCOPE is a python package for modeling supernova light curves using the analytic models of Morag et al 2023 and Morag et al 2024.',
 long_description=open('README.md').read(),
 long_description_content_type='text/markdown',
 
 setup(
     name='SNeSCOPE',
-    version='1.0.0',
+    version='1.0.1',
     description='Published version (April 2024)',  
     author='Ido Irani',
     author_email='idoirani@gmail.com', 
     url = 'https://github.com/idoirani/shock_cooling',
     keywords='astronomy',  
     packages=["SNeSCOPE"],
     #packages=find_packages(),
-    install_requires=['numpy','matplotlib','dynesty','scipy','numba','astropy','pandas'],  
+    install_requires=['numpy','matplotlib','dynesty','scipy','numba','astropy','pandas','tqdm','ipdb','extinction','os','sys'],  
     python_requires='>=3.6',
 )
```

### Comparing `SNeSCOPE-1.0.0/SNeSCOPE/blackbody_tools.py` & `SNeSCOPE-1.0.1/SNeSCOPE/blackbody_tools.py`

 * *Files identical despite different names*

### Comparing `SNeSCOPE-1.0.0/SNeSCOPE/PhotoUtils.py` & `SNeSCOPE-1.0.1/SNeSCOPE/PhotoUtils.py`

 * *Files identical despite different names*

