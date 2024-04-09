# Comparing `tmp/scorecard_generator-0.1.0.tar.gz` & `tmp/scorecard_generator-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_generator-0.1.0.tar", last modified: Thu Feb 22 05:04:31 2024, max compression
+gzip compressed data, was "scorecard_generator-2.1.2.tar", last modified: Tue Apr  9 16:59:46 2024, max compression
```

## Comparing `scorecard_generator-0.1.0.tar` & `scorecard_generator-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 05:04:31.984378 scorecard_generator-0.1.0/
--rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0    10351 2024-02-22 05:04:31.968621 scorecard_generator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9212 2024-02-22 05:03:00.000000 scorecard_generator-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 05:04:31.906584 scorecard_generator-0.1.0/scorecard_generator/
--rw-rw-rw-   0        0        0      197 2024-02-22 03:20:42.000000 scorecard_generator-0.1.0/scorecard_generator/__init__.py
--rw-rw-rw-   0        0        0    13084 2024-02-22 03:42:10.000000 scorecard_generator-0.1.0/scorecard_generator/scorecard.py
-drwxrwxrwx   0        0        0        0 2024-02-22 05:04:31.968621 scorecard_generator-0.1.0/scorecard_generator.egg-info/
--rw-rw-rw-   0        0        0    10351 2024-02-22 05:04:31.000000 scorecard_generator-0.1.0/scorecard_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-02-22 05:04:31.000000 scorecard_generator-0.1.0/scorecard_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 05:04:31.000000 scorecard_generator-0.1.0/scorecard_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-02-22 05:04:31.000000 scorecard_generator-0.1.0/scorecard_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-22 05:04:31.000000 scorecard_generator-0.1.0/scorecard_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 05:04:31.985030 scorecard_generator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1328 2024-02-22 03:59:24.000000 scorecard_generator-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 scorecard_generator-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    10351 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9212 2024-04-09 16:52:24.000000 scorecard_generator-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.886494 scorecard_generator-2.1.2/scorecard_generator/
+-rw-rw-rw-   0        0        0      201 2024-03-18 05:47:42.000000 scorecard_generator-2.1.2/scorecard_generator/__init__.py
+-rw-rw-rw-   0        0        0    13222 2024-04-09 16:51:49.000000 scorecard_generator-2.1.2/scorecard_generator/scorecard.py
+drwxrwxrwx   0        0        0        0 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/scorecard_generator.egg-info/
+-rw-rw-rw-   0        0        0    10351 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 16:59:46.000000 scorecard_generator-2.1.2/scorecard_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 16:59:46.951058 scorecard_generator-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-04-09 16:52:34.000000 scorecard_generator-2.1.2/setup.py
```

### Comparing `scorecard_generator-0.1.0/LICENSE.txt` & `scorecard_generator-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scorecard_generator-0.1.0/PKG-INFO` & `scorecard_generator-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 0.1.0
+Version: 2.1.2
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
 
-pip install scorecard_generator==0.1.0
+pip install scorecard_generator==2.1.2
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-0.1.0/README.md` & `scorecard_generator-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install scorecard_generator==0.1.0
+pip install scorecard_generator==2.1.2
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-0.1.0/scorecard_generator/scorecard.py` & `scorecard_generator-2.1.2/scorecard_generator/scorecard.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,19 @@
         else:
             print("Model does not provide coefficients or feature importances.")
             return None
     except AttributeError:
         return "This classification method does not support this operation."
 
     # Calculate min and max sum of coefficients excluding the intercept
-    min_sum_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].min().sum()
-    max_sum_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].max().sum()
+    # Corrected calculation of min and max sum of coefficients excluding the intercept
+    min_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].min()
+    max_coef = coeff_df[coeff_df['Feature Name'] != 'Intercept']['Coefficients'].max()
+    min_sum_coef = min_coef.sum()
+    max_sum_coef = max_coef.sum()
     
     # Score calculation for all features
     coeff_df['Score - Calculation'] = (coeff_df['Coefficients'] * (max_score - min_score) / (max_sum_coef - min_sum_coef)).round().astype(int)
     
     # Find the position of the intercept
     n = coeff_df.index[coeff_df['Feature Name'] == 'Intercept'].tolist()[0]
```

### Comparing `scorecard_generator-0.1.0/scorecard_generator.egg-info/PKG-INFO` & `scorecard_generator-2.1.2/scorecard_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scorecard_generator
-Version: 0.1.0
+Version: 2.1.2
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
 
-pip install scorecard_generator==0.1.0
+pip install scorecard_generator==2.1.2
 ```
 
 ## Load Package
 ``` bash
 
 from scorecard_generator import scorecard
 ```
```

### Comparing `scorecard_generator-0.1.0/setup.py` & `scorecard_generator-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scorecard_generator',
-    version='0.1.0',
+    version='2.1.2',
     packages=find_packages(),
     description='A Python Library for Creating Scorecards From Classification Models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kwadwo Daddy Nyame Owusu - Boakye',
     author_email='kwadwo.owusuboakye@outlook.com',
     url='https://github.com/knowusuboaky/scorecard_generator',
```

