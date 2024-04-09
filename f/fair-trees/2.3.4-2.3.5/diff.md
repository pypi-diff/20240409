# Comparing `tmp/fair_trees-2.3.4.tar.gz` & `tmp/fair_trees-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fair_trees-2.3.4.tar", last modified: Tue Apr  9 15:57:39 2024, max compression
+gzip compressed data, was "fair_trees-2.3.5.tar", last modified: Tue Apr  9 16:00:11 2024, max compression
```

## Comparing `fair_trees-2.3.4.tar` & `fair_trees-2.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.575883 fair_trees-2.3.4/
--rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.4/LICENSE
--rw-rw-rw-   0        0        0     4912 2024-04-09 15:57:39.574883 fair_trees-2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     4350 2024-04-09 15:56:29.000000 fair_trees-2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.569950 fair_trees-2.3.4/fair_trees/
--rw-rw-rw-   0        0        0      210 2024-04-09 15:44:19.000000 fair_trees-2.3.4/fair_trees/__init__.py
--rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.4/fair_trees/fair_trees.py
-drwxrwxrwx   0        0        0        0 2024-04-09 15:57:39.574883 fair_trees-2.3.4/fair_trees.egg-info/
--rw-rw-rw-   0        0        0     4912 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 15:57:39.000000 fair_trees-2.3.4/fair_trees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 15:57:39.575883 fair_trees-2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      781 2024-04-09 15:57:31.000000 fair_trees-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:11.371818 fair_trees-2.3.5/
+-rw-rw-rw-   0        0        0    35821 2024-04-09 15:36:15.000000 fair_trees-2.3.5/LICENSE
+-rw-rw-rw-   0        0        0     4912 2024-04-09 16:00:11.371818 fair_trees-2.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4350 2024-04-09 15:56:29.000000 fair_trees-2.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:11.365822 fair_trees-2.3.5/fair_trees/
+-rw-rw-rw-   0        0        0      210 2024-04-09 15:44:19.000000 fair_trees-2.3.5/fair_trees/__init__.py
+-rw-rw-rw-   0        0        0    26689 2024-04-09 13:34:38.000000 fair_trees-2.3.5/fair_trees/fair_trees.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:00:11.370847 fair_trees-2.3.5/fair_trees.egg-info/
+-rw-rw-rw-   0        0        0     4912 2024-04-09 16:00:11.000000 fair_trees-2.3.5/fair_trees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-04-09 16:00:11.000000 fair_trees-2.3.5/fair_trees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:00:11.000000 fair_trees-2.3.5/fair_trees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-09 16:00:11.000000 fair_trees-2.3.5/fair_trees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-09 16:00:11.000000 fair_trees-2.3.5/fair_trees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:00:11.371818 fair_trees-2.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-04-09 16:00:04.000000 fair_trees-2.3.5/setup.py
```

### Comparing `fair_trees-2.3.4/LICENSE` & `fair_trees-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.4/PKG-INFO` & `fair_trees-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.4
+Version: 2.3.5
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
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.4 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.5 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
```

### Comparing `fair_trees-2.3.4/README.md` & `fair_trees-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.4/fair_trees/fair_trees.py` & `fair_trees-2.3.5/fair_trees/fair_trees.py`

 * *Files identical despite different names*

### Comparing `fair_trees-2.3.4/fair_trees.egg-info/PKG-INFO` & `fair_trees-2.3.5/fair_trees.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fair_trees
-Version: 2.3.4
+Version: 2.3.5
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
-Metadata-Version: 2.1 Name: fair_trees Version: 2.3.4 Summary: This package
+Metadata-Version: 2.1 Name: fair_trees Version: 2.3.5 Summary: This package
 learns fair decision tree classifiers which can then be bagged into fair random
 forests, following the scikit-learn API standards. Home-page: https://
 github.com/pereirabarataap/fair_tree_classifier Author: Antonio Pereira Barata
 Author-email: apbarata@gmail.com Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: scipy Requires-Dist: numpy Requires-Dist:
 pandas Requires-Dist: joblib Requires-Dist: scikit-learn Requires-Dist:
 requests_mock # Fair tree classifier using strong demographic parity _[_>_>_] This
```

### Comparing `fair_trees-2.3.4/setup.py` & `fair_trees-2.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fair_trees",
-    version="2.3.4",
+    version="2.3.5",
     packages=find_packages(),
     description="This package learns fair decision tree classifiers which can then be bagged into fair random forests, following the scikit-learn API standards.",
     author="Antonio Pereira Barata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="apbarata@gmail.com",
     url="https://github.com/pereirabarataap/fair_tree_classifier",
```

