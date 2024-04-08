# Comparing `tmp/uf-toolkit-0.2.2.tar.gz` & `tmp/uf-toolkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uf-toolkit-0.2.2.tar", last modified: Mon Apr  8 21:44:54 2024, max compression
+gzip compressed data, was "uf-toolkit-0.2.3.tar", last modified: Mon Apr  8 22:30:53 2024, max compression
```

## Comparing `uf-toolkit-0.2.2.tar` & `uf-toolkit-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 chashuggins   (501) staff       (20)        0 2024-04-08 21:44:54.029908 uf-toolkit-0.2.2/
--rw-r--r--   0 chashuggins   (501) staff       (20)     1071 2024-03-27 23:06:15.000000 uf-toolkit-0.2.2/LICENSE
--rw-r--r--   0 chashuggins   (501) staff       (20)     2861 2024-04-08 21:44:54.029667 uf-toolkit-0.2.2/PKG-INFO
--rw-r--r--   0 chashuggins   (501) staff       (20)     2275 2024-04-04 21:39:35.000000 uf-toolkit-0.2.2/README.md
--rw-r--r--   0 chashuggins   (501) staff       (20)      605 2024-04-08 21:44:42.000000 uf-toolkit-0.2.2/pyproject.toml
--rw-r--r--   0 chashuggins   (501) staff       (20)       38 2024-04-08 21:44:54.029961 uf-toolkit-0.2.2/setup.cfg
--rw-r--r--   0 chashuggins   (501) staff       (20)      734 2024-04-08 21:44:03.000000 uf-toolkit-0.2.2/setup.py
-drwxr-xr-x   0 chashuggins   (501) staff       (20)        0 2024-04-08 21:44:54.029421 uf-toolkit-0.2.2/uf_toolkit.egg-info/
--rw-r--r--   0 chashuggins   (501) staff       (20)     2861 2024-04-08 21:44:54.000000 uf-toolkit-0.2.2/uf_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 chashuggins   (501) staff       (20)      177 2024-04-08 21:44:54.000000 uf-toolkit-0.2.2/uf_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 chashuggins   (501) staff       (20)        1 2024-04-08 21:44:54.000000 uf-toolkit-0.2.2/uf_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 chashuggins   (501) staff       (20)        1 2024-04-08 21:44:54.000000 uf-toolkit-0.2.2/uf_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 chashuggins   (501) staff       (20)        0 2024-04-08 22:30:53.150184 uf-toolkit-0.2.3/
+-rw-r--r--   0 chashuggins   (501) staff       (20)     1071 2024-03-27 23:06:15.000000 uf-toolkit-0.2.3/LICENSE
+-rw-r--r--   0 chashuggins   (501) staff       (20)     2861 2024-04-08 22:30:53.149944 uf-toolkit-0.2.3/PKG-INFO
+-rw-r--r--   0 chashuggins   (501) staff       (20)     2275 2024-04-04 21:39:35.000000 uf-toolkit-0.2.3/README.md
+-rw-r--r--   0 chashuggins   (501) staff       (20)      681 2024-04-08 22:28:45.000000 uf-toolkit-0.2.3/pyproject.toml
+-rw-r--r--   0 chashuggins   (501) staff       (20)       38 2024-04-08 22:30:53.150241 uf-toolkit-0.2.3/setup.cfg
+-rw-r--r--   0 chashuggins   (501) staff       (20)      722 2024-04-08 22:28:14.000000 uf-toolkit-0.2.3/setup.py
+drwxr-xr-x   0 chashuggins   (501) staff       (20)        0 2024-04-08 22:30:53.148961 uf-toolkit-0.2.3/uf-toolkit/
+-rw-r--r--   0 chashuggins   (501) staff       (20)       34 2024-03-27 22:47:02.000000 uf-toolkit-0.2.3/uf-toolkit/__init__.py
+-rw-r--r--   0 chashuggins   (501) staff       (20)     1039 2024-03-27 22:47:02.000000 uf-toolkit-0.2.3/uf-toolkit/union_find.py
+drwxr-xr-x   0 chashuggins   (501) staff       (20)        0 2024-04-08 22:30:53.149713 uf-toolkit-0.2.3/uf_toolkit.egg-info/
+-rw-r--r--   0 chashuggins   (501) staff       (20)     2861 2024-04-08 22:30:53.000000 uf-toolkit-0.2.3/uf_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 chashuggins   (501) staff       (20)      225 2024-04-08 22:30:53.000000 uf-toolkit-0.2.3/uf_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 chashuggins   (501) staff       (20)        1 2024-04-08 22:30:53.000000 uf-toolkit-0.2.3/uf_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 chashuggins   (501) staff       (20)       11 2024-04-08 22:30:53.000000 uf-toolkit-0.2.3/uf_toolkit.egg-info/top_level.txt
```

### Comparing `uf-toolkit-0.2.2/LICENSE` & `uf-toolkit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uf-toolkit-0.2.2/PKG-INFO` & `uf-toolkit-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: uf-toolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple Union Find Class for Python.
 Home-page: https://github.com/hugginsc10/uf-toolkit
 Author: Chas Huggins
 Author-email: Chas Huggins <Hugginsc10@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Name: UF-Toolkit
 
 ## Description
```

### Comparing `uf-toolkit-0.2.2/README.md` & `uf-toolkit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `uf-toolkit-0.2.2/pyproject.toml` & `uf-toolkit-0.2.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
-requires = ["setuptools>=61.0", "wheel"]
+requires = ["setuptools>=61.0.8", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uf-toolkit"
-version = "0.2.2"
+version = "0.2.3"
 description = "A simple Union Find Class for Python."
 readme = "README.md"
 authors = [
     { name = "Chas Huggins", email = "Hugginsc10@gmail.com" },
 ]
 license = { text = "MIT" }
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
-]
+]
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.txt"] }
```

### Comparing `uf-toolkit-0.2.2/setup.py` & `uf-toolkit-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name="uf-toolkit",
-    version="0.2.2",
-    packages=find_packages('uf-toolkit'),
+    version="0.2.3",
+    packages=find_packages(),
     description="A simple Union Find Class for Python.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Chas Huggins",
     author_email="hugginsc10@gmail.com",
     url="https://github.com/hugginsc10/uf-toolkit",
     classifiers=[
```

### Comparing `uf-toolkit-0.2.2/uf_toolkit.egg-info/PKG-INFO` & `uf-toolkit-0.2.3/uf_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: uf-toolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple Union Find Class for Python.
 Home-page: https://github.com/hugginsc10/uf-toolkit
 Author: Chas Huggins
 Author-email: Chas Huggins <Hugginsc10@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Project Name: UF-Toolkit
 
 ## Description
```

