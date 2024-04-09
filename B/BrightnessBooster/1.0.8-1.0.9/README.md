# Comparing `tmp/BrightnessBooster-1.0.8.tar.gz` & `tmp/BrightnessBooster-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrightnessBooster-1.0.8.tar", last modified: Tue Apr  9 19:05:13 2024, max compression
+gzip compressed data, was "BrightnessBooster-1.0.9.tar", last modified: Tue Apr  9 19:23:45 2024, max compression
```

## Comparing `BrightnessBooster-1.0.8.tar` & `BrightnessBooster-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:05:13.502453 BrightnessBooster-1.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:05:13.452448 BrightnessBooster-1.0.8/BrightnessBooster/
--rw-rw-rw-   0        0        0      304 2024-04-09 18:12:38.000000 BrightnessBooster-1.0.8/BrightnessBooster/__init__.py
--rw-rw-rw-   0        0        0     9109 2024-04-09 18:21:29.000000 BrightnessBooster-1.0.8/BrightnessBooster/brightnessbooster.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:05:13.500452 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/
--rw-rw-rw-   0        0        0     3072 2024-04-09 19:05:13.000000 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-09 19:05:13.000000 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:05:13.000000 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-09 19:05:13.000000 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 19:05:13.000000 BrightnessBooster-1.0.8/BrightnessBooster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3072 2024-04-09 19:05:13.503452 BrightnessBooster-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2696 2024-04-09 19:03:55.000000 BrightnessBooster-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 19:05:13.512452 BrightnessBooster-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      566 2024-04-09 19:03:18.000000 BrightnessBooster-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.095174 BrightnessBooster-1.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.065478 BrightnessBooster-1.0.9/BrightnessBooster/
+-rw-rw-rw-   0        0        0      304 2024-04-09 18:12:38.000000 BrightnessBooster-1.0.9/BrightnessBooster/__init__.py
+-rw-rw-rw-   0        0        0     9132 2024-04-09 19:23:06.000000 BrightnessBooster-1.0.9/BrightnessBooster/brightnessbooster.py
+drwxrwxrwx   0        0        0        0 2024-04-09 19:23:45.093245 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/
+-rw-rw-rw-   0        0        0     3072 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-09 19:23:44.000000 BrightnessBooster-1.0.9/BrightnessBooster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3072 2024-04-09 19:23:45.095174 BrightnessBooster-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2696 2024-04-09 19:03:55.000000 BrightnessBooster-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 19:23:45.097175 BrightnessBooster-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      566 2024-04-09 19:23:28.000000 BrightnessBooster-1.0.9/setup.py
```

### Comparing `BrightnessBooster-1.0.8/BrightnessBooster/brightnessbooster.py` & `BrightnessBooster-1.0.9/BrightnessBooster/brightnessbooster.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,16 @@
 
 
 def approximate_beta_distribution(data):
 
     sorted_indixes = np.argsort(data)
     sorted_values = data[sorted_indixes]
 
-    norm_sorted_values = sorted_values / 255
+    max = np.max(data)
+    norm_sorted_values = sorted_values / max
 
 
     mean = np.mean(norm_sorted_values)
     variance = np.var(norm_sorted_values)
     variance = variance * variance
 
     a, b = calculate_beta_parameters(mean, variance)
```

### Comparing `BrightnessBooster-1.0.8/BrightnessBooster.egg-info/PKG-INFO` & `BrightnessBooster-1.0.9/BrightnessBooster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrightnessBooster
-Version: 1.0.8
+Version: 1.0.9
 Summary: The code enhances an image's brightness and contrast
 Home-page: UNKNOWN
 Author: necros2604
 Author-email: bair1hasykov@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BrightnessBooster-1.0.8/PKG-INFO` & `BrightnessBooster-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrightnessBooster
-Version: 1.0.8
+Version: 1.0.9
 Summary: The code enhances an image's brightness and contrast
 Home-page: UNKNOWN
 Author: necros2604
 Author-email: bair1hasykov@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BrightnessBooster-1.0.8/README.md` & `BrightnessBooster-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `BrightnessBooster-1.0.8/setup.py` & `BrightnessBooster-1.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import open
 from setuptools import setup
 
-version = '1.0.8'
+version = '1.0.9'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BrightnessBooster',
     version=version,
```

