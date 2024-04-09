# Comparing `tmp/scorecard_generator-2.1.7.tar.gz` & `tmp/scorecard_generator-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_generator-2.1.7.tar", last modified: Tue Apr  9 18:13:25 2024, max compression
+gzip compressed data, was "scorecard_generator-2.1.8.tar", last modified: Tue Apr  9 18:37:21 2024, max compression
```

## Comparing `scorecard_generator-2.1.7.tar` & `scorecard_generator-2.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:13:25.568020 scorecard_generator-2.1.7/
--rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0    10351 2024-04-09 18:13:25.568020 scorecard_generator-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     9212 2024-04-09 18:12:49.000000 scorecard_generator-2.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 18:13:25.523248 scorecard_generator-2.1.7/scorecard_generator/
--rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.7/scorecard_generator/__init__.py
--rw-rw-rw-   0        0        0    13738 2024-04-09 18:07:12.000000 scorecard_generator-2.1.7/scorecard_generator/scorecard.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:13:25.552392 scorecard_generator-2.1.7/scorecard_generator.egg-info/
--rw-rw-rw-   0        0        0    10351 2024-04-09 18:13:25.000000 scorecard_generator-2.1.7/scorecard_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-04-09 18:13:25.000000 scorecard_generator-2.1.7/scorecard_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:13:25.000000 scorecard_generator-2.1.7/scorecard_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-09 18:13:25.000000 scorecard_generator-2.1.7/scorecard_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 18:13:25.000000 scorecard_generator-2.1.7/scorecard_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 18:13:25.568020 scorecard_generator-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-04-09 18:12:38.000000 scorecard_generator-2.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.559526 scorecard_generator-2.1.8/
+-rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    10351 2024-04-09 18:37:21.555987 scorecard_generator-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9212 2024-04-09 18:37:03.000000 scorecard_generator-2.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.508652 scorecard_generator-2.1.8/scorecard_generator/
+-rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.8/scorecard_generator/__init__.py
+-rw-rw-rw-   0        0        0    13118 2024-04-09 18:31:25.000000 scorecard_generator-2.1.8/scorecard_generator/scorecard.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:37:21.539705 scorecard_generator-2.1.8/scorecard_generator.egg-info/
+-rw-rw-rw-   0        0        0    10351 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 18:37:21.000000 scorecard_generator-2.1.8/scorecard_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:37:21.559526 scorecard_generator-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-09 18:36:41.000000 scorecard_generator-2.1.8/setup.py
```

### Comparing `scorecard_generator-2.1.7/LICENSE.txt` & `scorecard_generator-2.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scorecard_generator-2.1.7/PKG-INFO` & `scorecard_generator-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.7
+Version: 2.1.8
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
 
-pip install scorecard_generator==2.1.7
+pip install scorecard_generator==2.1.8
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.7/README.md` & `scorecard_generator-2.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==2.1.7
+pip install scorecard_generator==2.1.8
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.7/scorecard_generator/scorecard.py` & `scorecard_generator-2.1.8/scorecard_generator/scorecard.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,28 +196,16 @@
             return None
     except AttributeError:
         return "This classification method does not support this operation."
 
     # Calculate min and max sum of coefficients excluding the intercept
     min_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].min()
     max_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].max()
-
-    # Check if min_coef is a singular value (e.g., int, float) or a collection (e.g., list, numpy array)
-    if isinstance(min_coef, (int, float)):  # Checks if it's a singular numerical value
-        # Code to execute if min_coef is a singular value
-        min_sum_coef = min_coef
-    else:
-        min_sum_coef = min_coef.sum()
-
-    # Check if max_coef is a singular value (e.g., int, float) or a collection (e.g., list, numpy array)
-    if isinstance(max_coef, (int, float)):  # Checks if it's a singular numerical value
-        # Code to execute if max_coef is a singular value
-        max_sum_coef = max_coef
-    else:
-        max_sum_coef = max_coef.sum()
+    min_sum_coef = min_coef
+    max_sum_coef = max_coef
 
     # Score calculation for all features
     coeff_df['Score - Calculation'] = (coeff_df['Coefficients'] * (max_score - min_score) / (max_sum_coef - min_sum_coef)).round().astype(int)
     
     # Find the position of the intercept
     n = coeff_df.index[coeff_df['Feature Name'] == 'Intercept'].tolist()[0]
```

### Comparing `scorecard_generator-2.1.7/scorecard_generator.egg-info/PKG-INFO` & `scorecard_generator-2.1.8/scorecard_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 2.1.7
+Version: 2.1.8
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
 
-pip install scorecard_generator==2.1.7
+pip install scorecard_generator==2.1.8
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-2.1.7/setup.py` & `scorecard_generator-2.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scorecard_generator',
-    version='2.1.7',
+    version='2.1.8',
     packages=find_packages(),
     description='A Python Library for Creating Scorecards From Classification Models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kwadwo Daddy Nyame Owusu - Boakye',
     author_email='kwadwo.owusuboakye@outlook.com',
     url='https://github.com/knowusuboaky/scorecard_generator',
```

