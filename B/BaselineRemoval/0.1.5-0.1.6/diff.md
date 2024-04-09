# Comparing `tmp/BaselineRemoval-0.1.5.tar.gz` & `tmp/BaselineRemoval-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaselineRemoval-0.1.5.tar", last modified: Sun Aug  6 13:35:06 2023, max compression
+gzip compressed data, was "dist/BaselineRemoval-0.1.6.tar", last modified: Tue Apr  9 10:45:07 2024, max compression
```

## Comparing `BaselineRemoval-0.1.5.tar` & `BaselineRemoval-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/
--rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 BaselineRemoval-0.1.5/LICENSE
--rw-rw-r--   0 azim      (1000) azim      (1000)     5556 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)     4322 2023-08-06 13:34:46.000000 BaselineRemoval-0.1.5/README.rst
--rw-r--r--   0 azim      (1000) azim      (1000)       79 2023-08-06 13:35:06.796745 BaselineRemoval-0.1.5/setup.cfg
--rw-r--r--   0 azim      (1000) azim      (1000)      874 2023-08-06 12:09:18.000000 BaselineRemoval-0.1.5/setup.py
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.792745 BaselineRemoval-0.1.5/src/
-drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2023-08-06 13:35:06.792745 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/
--rw-r--r--   0 azim      (1000) azim      (1000)     5556 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/PKG-INFO
--rw-r--r--   0 azim      (1000) azim      (1000)      274 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/SOURCES.txt
--rw-r--r--   0 azim      (1000) azim      (1000)        1 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/dependency_links.txt
--rw-r--r--   0 azim      (1000) azim      (1000)       25 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/requires.txt
--rw-r--r--   0 azim      (1000) azim      (1000)       16 2023-08-06 13:35:06.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/top_level.txt
--rw-r--r--   0 azim      (1000) azim      (1000)     7204 2023-02-17 14:06:32.000000 BaselineRemoval-0.1.5/src/BaselineRemoval.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2024-04-09 10:45:07.913939 BaselineRemoval-0.1.6/
+-rw-r--r--   0 azim      (1000) azim      (1000)     1068 2020-05-26 15:31:42.000000 BaselineRemoval-0.1.6/LICENSE
+-rw-rw-r--   0 azim      (1000) azim      (1000)     5556 2024-04-09 10:45:07.913939 BaselineRemoval-0.1.6/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)     4322 2023-08-06 13:34:46.000000 BaselineRemoval-0.1.6/README.rst
+-rw-r--r--   0 azim      (1000) azim      (1000)       79 2024-04-09 10:45:07.913939 BaselineRemoval-0.1.6/setup.cfg
+-rw-r--r--   0 azim      (1000) azim      (1000)      874 2024-04-09 10:42:47.000000 BaselineRemoval-0.1.6/setup.py
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2024-04-09 10:45:07.909939 BaselineRemoval-0.1.6/src/
+drwxrwxr-x   0 azim      (1000) azim      (1000)        0 2024-04-09 10:45:07.913939 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/
+-rw-r--r--   0 azim      (1000) azim      (1000)     5556 2024-04-09 10:45:07.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/PKG-INFO
+-rw-r--r--   0 azim      (1000) azim      (1000)      274 2024-04-09 10:45:07.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/SOURCES.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)        1 2024-04-09 10:45:07.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/dependency_links.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       25 2024-04-09 10:45:07.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/requires.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)       16 2024-04-09 10:45:07.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/top_level.txt
+-rw-r--r--   0 azim      (1000) azim      (1000)     7204 2024-04-09 10:44:22.000000 BaselineRemoval-0.1.6/src/BaselineRemoval.py
```

### Comparing `BaselineRemoval-0.1.5/LICENSE` & `BaselineRemoval-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `BaselineRemoval-0.1.5/PKG-INFO` & `BaselineRemoval-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BaselineRemoval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum
 Home-page: https://github.com/StatguyUser/BaselineRemoval
 Author: StatguyUser
 License: UNKNOWN
 Download-URL: https://github.com/StatguyUser/BaselineRemoval.git
 Description: What is it?
         ===========
```

### Comparing `BaselineRemoval-0.1.5/README.rst` & `BaselineRemoval-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `BaselineRemoval-0.1.5/setup.py` & `BaselineRemoval-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     with open('README.rst', encoding='utf-8') as f:
         long_description = f.read()
 
 
 setup(
     name='BaselineRemoval',
-    version='0.1.5',
+    version='0.1.6',
     description='Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='StatguyUser',
     url='https://github.com/StatguyUser/BaselineRemoval',
     install_requires=['numpy','scikit-learn','scipy'],
     download_url='https://github.com/StatguyUser/BaselineRemoval.git',
```

### Comparing `BaselineRemoval-0.1.5/src/BaselineRemoval.egg-info/PKG-INFO` & `BaselineRemoval-0.1.6/src/BaselineRemoval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BaselineRemoval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Perform baseline removal, baseline correction and baseline substraction for raman spectra using Modpoly, ImodPoly and Zhang fit. Returns baseline-subtracted spectrum
 Home-page: https://github.com/StatguyUser/BaselineRemoval
 Author: StatguyUser
 License: UNKNOWN
 Download-URL: https://github.com/StatguyUser/BaselineRemoval.git
 Description: What is it?
         ===========
```

### Comparing `BaselineRemoval-0.1.5/src/BaselineRemoval.py` & `BaselineRemoval-0.1.6/src/BaselineRemoval.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         - in the next step, discard the first column from above matrix.
 
         - for each value in the range of polynomial, starting from index 0 of pollynomial range, (for k in range(p+1))
             create an array in such a way that elements of array are (original_individual_value)^polynomial_index (x**k)
         - concatenate all of these arrays created through loop, as a master array. This is done through (np.vstack)
         - transpose the master array, so that its more like a tabular form(np.transpose)'''
         input_array_for_poly = np.array(input_array_for_poly,dtype='object')
-        X = np.transpose(np.vstack((input_array_for_poly**k for k in range(degree_for_poly+1))))
+        X = np.transpose(np.vstack([input_array_for_poly**k for k in range(degree_for_poly+1)]))
         return np.linalg.qr(X)[0][:,1:]
     def ModPoly(self,degree=2,repitition=100,gradient=0.001):
         '''Implementation of Modified polyfit method from paper: Automated Method for Subtraction of Fluorescence from Biological Raman Spectra, by Lieber & Mahadevan-Jansen (2003)
         
         degree: Polynomial degree, default is 2
 
         repitition: How many iterations to run. Default is 100
```

