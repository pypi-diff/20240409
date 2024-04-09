# Comparing `tmp/fair_trees-2.3.2.tar.gz` & `tmp/fair_trees-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.2.tar", last modified: Tue Apr  9 15:38:24 2024, max compression
+gzip compressed data, was "fair_trees-2.3.3.tar", last modified: Tue Apr  9 15:45:05 2024, max compression
```

## Comparing `fair_trees-2.3.2.tar` & `fair_trees-2.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.361981 fair_trees-2.3.2/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.2/LICENSE
--rw-rw-rw-   0        0        0     4902 2024-04-09 15:38:24.360982 fair_trees-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2024-04-09 15:35:47.000000 fair_trees-2.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.355983 fair_trees-2.3.2/fair_trees/
--rw-rw-rw-   0        0        0       91 2024-04-09 15:36:28.000000 fair_trees-2.3.2/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.2/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:38:24.359981 fair_trees-2.3.2/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4902 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 15:38:24.000000 fair_trees-2.3.2/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 15:38:24.361981 fair_trees-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-04-09 15:37:49.000000 fair_trees-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.577436 fair_trees-2.3.3/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4902 2024-04-09 15:45:05.577436 fair_trees-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2024-04-09 15:35:47.000000 fair_trees-2.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.573335 fair_trees-2.3.3/fair_trees/
+-rw-rw-rw-   0        0        0      210 2024-04-09 15:44:19.000000 fair_trees-2.3.3/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.3/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 15:45:05.576432 fair_trees-2.3.3/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4902 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 15:45:05.000000 fair_trees-2.3.3/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 15:45:05.577436 fair_trees-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-04-09 15:45:00.000000 fair_trees-2.3.3/setup.py
```

### Comparing `fair_trees-2.3.2/LICENSE` & `fair_trees-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.2/PKG-INFO` & `fair_trees-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.2
+Version: 2.3.3
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.2 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.3 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
```

### Comparing `fair_trees-2.3.2/README.md` & `fair_trees-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.2/fair_trees/fair_trees.py` & `fair_trees-2.3.3/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.2/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.3.3/fair_trees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.2
+Version: 2.3.3
 Summary: This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.
 Home-page: https://github.com/pereirabarataap/fair_tree_classifier
 Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.2 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.3 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
```

### Comparing `fair_trees-2.3.2/setup.py` & `fair_trees-2.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-
 setup(
     name="fair_trees",
-    version="2.3.2",
+    version="2.3.3",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

