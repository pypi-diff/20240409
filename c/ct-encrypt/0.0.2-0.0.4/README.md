# Comparing `tmp/ct_encrypt-0.0.2.tar.gz` & `tmp/ct_encrypt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ct_encrypt-0.0.2.tar", last modified: Mon Apr  8 23:52:34 2024, max compression
+gzip compressed data, was "ct_encrypt-0.0.4.tar", last modified: Tue Apr  9 19:21:15 2024, max compression
```

## Comparing `ct_encrypt-0.0.2.tar` & `ct_encrypt-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 oladeji   (1000) oladeji   (1000)        0 2024-04-08 23:52:34.620654 ct_encrypt-0.0.2/
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)      587 2024-04-08 23:52:34.620654 ct_encrypt-0.0.2/PKG-INFO
-drwxr-xr-x   0 oladeji   (1000) oladeji   (1000)        0 2024-04-08 23:52:34.620654 ct_encrypt-0.0.2/ct_encrypt.egg-info/
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)      587 2024-04-08 23:52:34.000000 ct_encrypt-0.0.2/ct_encrypt.egg-info/PKG-INFO
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)      144 2024-04-08 23:52:34.000000 ct_encrypt-0.0.2/ct_encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)        1 2024-04-08 23:52:34.000000 ct_encrypt-0.0.2/ct_encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)        1 2024-04-08 23:52:34.000000 ct_encrypt-0.0.2/ct_encrypt.egg-info/top_level.txt
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)       38 2024-04-08 23:52:34.620654 ct_encrypt-0.0.2/setup.cfg
--rw-r--r--   0 oladeji   (1000) oladeji   (1000)      858 2024-04-08 23:51:10.000000 ct_encrypt-0.0.2/setup.py
+drwxr-xr-x   0 oladeji   (1000) oladeji   (1000)        0 2024-04-09 19:21:15.608657 ct_encrypt-0.0.4/
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)      587 2024-04-09 19:21:15.588652 ct_encrypt-0.0.4/PKG-INFO
+drwxr-xr-x   0 oladeji   (1000) oladeji   (1000)        0 2024-04-09 19:21:15.588652 ct_encrypt-0.0.4/ct_encrypt.egg-info/
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)      587 2024-04-09 19:21:15.000000 ct_encrypt-0.0.4/ct_encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)      144 2024-04-09 19:21:15.000000 ct_encrypt-0.0.4/ct_encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)        1 2024-04-09 19:21:15.000000 ct_encrypt-0.0.4/ct_encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)        1 2024-04-09 19:21:15.000000 ct_encrypt-0.0.4/ct_encrypt.egg-info/top_level.txt
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)       38 2024-04-09 19:21:15.608657 ct_encrypt-0.0.4/setup.cfg
+-rw-r--r--   0 oladeji   (1000) oladeji   (1000)      858 2024-04-09 19:20:57.000000 ct_encrypt-0.0.4/setup.py
```

### Comparing `ct_encrypt-0.0.2/PKG-INFO` & `ct_encrypt-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ct_encrypt
-Version: 0.0.2
+Version: 0.0.4
 Summary: A custom cryptography script
 Home-page: https://github.com/Boluex/custom-cryptography-python-script.git
 Author: Oladeji Olaoluwa
 Author-email: oladejiolaoluwa46@gmail.com
 Keywords: custom crytography script
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ct_encrypt-0.0.2/ct_encrypt.egg-info/PKG-INFO` & `ct_encrypt-0.0.4/ct_encrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ct_encrypt
-Version: 0.0.2
+Version: 0.0.4
 Summary: A custom cryptography script
 Home-page: https://github.com/Boluex/custom-cryptography-python-script.git
 Author: Oladeji Olaoluwa
 Author-email: oladejiolaoluwa46@gmail.com
 Keywords: custom crytography script
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ct_encrypt-0.0.2/setup.py` & `ct_encrypt-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 base_dir = os.path.abspath(os.path.dirname('encrypt_dir'))
 
 
 setup(
     name='ct_encrypt',
-    version='0.0.2',
+    version='0.0.4',
     description='A custom cryptography script',
     packages=find_packages(where='encrypt_dir'),
     long_description='A custom cryptography script',
     long_description_content_type='text/markdown',
     url='https://github.com/Boluex/custom-cryptography-python-script.git',
     author='Oladeji Olaoluwa',
     author_email='oladejiolaoluwa46@gmail.com',
```

