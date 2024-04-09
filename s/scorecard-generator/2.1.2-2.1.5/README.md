# Comparing `tmp/scorecard_generator-2.1.2.tar.gz` & `tmp/scorecard_generator-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_generator-2.1.2.tar", last modified: Tue Apr  9 16:59:46 2024, max compression
+gzip compressed data, was "scorecard_generator-2.1.5.tar", last modified: Tue Apr  9 17:07:52 2024, max compression
```

## Comparing `scorecard_generator-2.1.2.tar` & `scorecard_generator-2.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/
--rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    10351 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9212 2024-04-09 16:52:24.000000 scorecard_generator-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.886494 scorecard_generator-2.1.2/scorecard_generator/
--rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.2/scorecard_generator/__init__.py
--rw-rw-rw-   0        0        0    13222 2024-04-09 16:51:49.000000 scorecard_generator-2.1.2/scorecard_generator/scorecard.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/scorecard_generator.egg-info/
--rw-rw-rw-   0        0        0    10351 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-04-09 16:52:34.000000 scorecard_generator-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:07:52.077033 scorecard_generator-2.1.5/
+-rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    10351 2024-04-09 17:07:52.077033 scorecard_generator-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9212 2024-04-09 17:07:20.000000 scorecard_generator-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 17:07:52.026192 scorecard_generator-2.1.5/scorecard_generator/
+-rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.5/scorecard_generator/__init__.py
+-rw-rw-rw-   0        0        0    13222 2024-04-09 16:51:49.000000 scorecard_generator-2.1.5/scorecard_generator/scorecard.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:07:52.077033 scorecard_generator-2.1.5/scorecard_generator.egg-info/
+-rw-rw-rw-   0        0        0    10351 2024-04-09 17:07:51.000000 scorecard_generator-2.1.5/scorecard_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-09 17:07:51.000000 scorecard_generator-2.1.5/scorecard_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:07:51.000000 scorecard_generator-2.1.5/scorecard_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-09 17:07:51.000000 scorecard_generator-2.1.5/scorecard_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 17:07:51.000000 scorecard_generator-2.1.5/scorecard_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:07:52.077033 scorecard_generator-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-09 17:07:09.000000 scorecard_generator-2.1.5/setup.py
```

### Comparing `scorecard_generator-2.1.2/LICENSE.txt` & `scorecard_generator-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scorecard_generator-2.1.2/PKG-INFO` & `scorecard_generator-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.2
+Version: 2.1.5
 Summary: A Python Library for Creating Scorecards From Classification Models.
 Home-page: https://github.com/knowusuboaky/scorecard_generator
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: scorecard,classification,woe,linear,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.2
+pip install scorecard_generator==2.1.5
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.2/README.md` & `scorecard_generator-2.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.2
+pip install scorecard_generator==2.1.5
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.2/scorecard_generator/scorecard.py` & `scorecard_generator-2.1.5/scorecard_generator/scorecard.py`

 * *Files identical despite different names*

### Comparing `scorecard_generator-2.1.2/scorecard_generator.egg-info/PKG-INFO` & `scorecard_generator-2.1.5/scorecard_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.2
+Version: 2.1.5
 Summary: A Python Library for Creating Scorecards From Classification Models.
 Home-page: https://github.com/knowusuboaky/scorecard_generator
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: scorecard,classification,woe,linear,machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.2
+pip install scorecard_generator==2.1.5
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.2/setup.py` & `scorecard_generator-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scorecard_generator',
-    version='2.1.2',
+    version='2.1.5',
     packages=find_packages(),
     description='A Python Library for Creating Scorecards From Classification Models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kwadwo Daddy Nyame Owusu - Boakye',
     author_email='kwadwo.owusuboakye@outlook.com',
     url='https://github.com/knowusuboaky/scorecard_generator',
```

