# Comparing `tmp/feature_engineering-2.1.2.tar.gz` & `tmp/feature_engineering-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_engineering-2.1.2.tar", last modified: Thu Feb 29 20:42:32 2024, max compression
+gzip compressed data, was "feature_engineering-2.1.3.tar", last modified: Tue Apr  9 00:26:38 2024, max compression
```

## Comparing `feature_engineering-2.1.2.tar` & `feature_engineering-2.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 20:42:32.352023 feature_engineering-2.1.2/
--rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 feature_engineering-2.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    25806 2024-02-29 20:42:32.352023 feature_engineering-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    23978 2024-02-29 19:55:09.000000 feature_engineering-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 20:42:32.252382 feature_engineering-2.1.2/feature_engineering/
--rw-rw-rw-   0        0        0      307 2024-02-29 16:21:10.000000 feature_engineering-2.1.2/feature_engineering/__init__.py
--rw-rw-rw-   0        0        0    20417 2024-02-29 17:15:07.000000 feature_engineering-2.1.2/feature_engineering/feature_engineering.py
-drwxrwxrwx   0        0        0        0 2024-02-29 20:42:32.352023 feature_engineering-2.1.2/feature_engineering.egg-info/
--rw-rw-rw-   0        0        0    25806 2024-02-29 20:42:31.000000 feature_engineering-2.1.2/feature_engineering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-02-29 20:42:32.000000 feature_engineering-2.1.2/feature_engineering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 20:42:31.000000 feature_engineering-2.1.2/feature_engineering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-02-29 20:42:31.000000 feature_engineering-2.1.2/feature_engineering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-02-29 20:42:31.000000 feature_engineering-2.1.2/feature_engineering.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 20:42:32.352023 feature_engineering-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2028 2024-02-29 07:51:30.000000 feature_engineering-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:26:38.688496 feature_engineering-2.1.3/
+-rw-rw-rw-   0        0        0     1088 2024-01-22 03:40:39.000000 feature_engineering-2.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    25806 2024-04-09 00:26:38.688496 feature_engineering-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    23978 2024-04-09 00:12:57.000000 feature_engineering-2.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 00:26:38.579465 feature_engineering-2.1.3/feature_engineering/
+-rw-rw-rw-   0        0        0      307 2024-02-29 16:21:10.000000 feature_engineering-2.1.3/feature_engineering/__init__.py
+-rw-rw-rw-   0        0        0    20690 2024-04-09 00:12:21.000000 feature_engineering-2.1.3/feature_engineering/feature_engineering.py
+drwxrwxrwx   0        0        0        0 2024-04-09 00:26:38.677488 feature_engineering-2.1.3/feature_engineering.egg-info/
+-rw-rw-rw-   0        0        0    25806 2024-04-09 00:26:38.000000 feature_engineering-2.1.3/feature_engineering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-09 00:26:38.000000 feature_engineering-2.1.3/feature_engineering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 00:26:38.000000 feature_engineering-2.1.3/feature_engineering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-04-09 00:26:38.000000 feature_engineering-2.1.3/feature_engineering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-09 00:26:38.000000 feature_engineering-2.1.3/feature_engineering.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 00:26:38.688496 feature_engineering-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2028 2024-04-09 00:14:08.000000 feature_engineering-2.1.3/setup.py
```

### Comparing `feature_engineering-2.1.2/LICENSE.txt` & `feature_engineering-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `feature_engineering-2.1.2/PKG-INFO` & `feature_engineering-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_engineering
-Version: 2.1.2
+Version: 2.1.3
 Summary: Unleash the Power of Your Data with Feature Engineering: The Ultimate Python Library for Machine Learning Preprocessing and Enhancement
 Home-page: https://github.com/knowusuboaky/feature_engineering
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: machine learning,data preprocessing,feature engineering,data transformation,data cleaning,outlier handling,imputation,scaling,one-hot encoding,feature selection,variance threshold,correlation filtering,embedded methods,wrapper methods,class imbalance,sampling techniques,hyperparameter tuning,model optimization,categorical data processing,numeric data processing,date feature extraction,custom transformers,Python,data science,predictive modeling,classification,regression,ML workflows,data analysis,data enrichment,model performance improvement
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install feature_engineering==2.1.2
+pip install feature_engineering==2.1.3
 ```
 
 ## Load Package
 ``` bash
 
 from feature_engineering import FeatureEngineering
 ```
```

### Comparing `feature_engineering-2.1.2/README.md` & `feature_engineering-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install feature_engineering==2.1.2
+pip install feature_engineering==2.1.3
 ```
 
 ## Load Package
 ``` bash
 
 from feature_engineering import FeatureEngineering
 ```
```

### Comparing `feature_engineering-2.1.2/feature_engineering/feature_engineering.py` & `feature_engineering-2.1.3/feature_engineering/feature_engineering.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,29 +402,34 @@
             # Now, apply hyperparameter tuning if specified
             tuned_model = self.perform_hyperparameter_tuning(model, self.X_preprocessed, self.y)
 
             if score > best_score:
                 best_score, best_model = score, tuned_model
         return best_model    
     
-
+        
     def run(self):
         """Executes the entire feature engineering process and ensures unique names for columns and features."""
 
         # Step 1: Preprocess data
         self.preprocess_data()
 
         # Step 2: Apply sampling techniques if specified
         if self.sampling_strategies:
             self.apply_sampling_techniques()
+            # Use the potentially modified 'y' after sampling
+            target_variable_final = self.y
+        else:
+            # If no sampling strategies were applied, use the original target column
+            target_variable_final = self.df[self.target]
 
         # Step 3: Perform feature selection
         self.select_features()
 
         # Concatenate preprocessed features with the target variable for the final DataFrame
-        df_final = pd.concat([self.X_preprocessed, self.df[[self.target]]], axis=1)
+        df_final = pd.concat([self.X_preprocessed, target_variable_final], axis=1)
 
         self.progress.description = 'Feature engineering process completed successfully. Data is now ready for model training.'
         self.progress.value = 100
 
         # Return the preprocessed data and unique selected features
         return df_final, self.selected_features
```

### Comparing `feature_engineering-2.1.2/feature_engineering.egg-info/PKG-INFO` & `feature_engineering-2.1.3/feature_engineering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_engineering
-Version: 2.1.2
+Version: 2.1.3
 Summary: Unleash the Power of Your Data with Feature Engineering: The Ultimate Python Library for Machine Learning Preprocessing and Enhancement
 Home-page: https://github.com/knowusuboaky/feature_engineering
 Author: Kwadwo Daddy Nyame Owusu - Boakye
 Author-email: kwadwo.owusuboakye@outlook.com
 Keywords: machine learning,data preprocessing,feature engineering,data transformation,data cleaning,outlier handling,imputation,scaling,one-hot encoding,feature selection,variance threshold,correlation filtering,embedded methods,wrapper methods,class imbalance,sampling techniques,hyperparameter tuning,model optimization,categorical data processing,numeric data processing,date feature extraction,custom transformers,Python,data science,predictive modeling,classification,regression,ML workflows,data analysis,data enrichment,model performance improvement
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -51,15 +51,15 @@
 
 ## Installation
 
 You can install the Scorecard Generator via pip:
 
 ``` bash
 
-pip install feature_engineering==2.1.2
+pip install feature_engineering==2.1.3
 ```
 
 ## Load Package
 ``` bash
 
 from feature_engineering import FeatureEngineering
 ```
```

### Comparing `feature_engineering-2.1.2/setup.py` & `feature_engineering-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='feature_engineering',
-    version='2.1.2',
+    version='2.1.3',
     packages=find_packages(),
     description='Unleash the Power of Your Data with Feature Engineering: The Ultimate Python Library for Machine Learning Preprocessing and Enhancement',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kwadwo Daddy Nyame Owusu - Boakye',
     author_email='kwadwo.owusuboakye@outlook.com',
     url='https://github.com/knowusuboaky/feature_engineering',
```

