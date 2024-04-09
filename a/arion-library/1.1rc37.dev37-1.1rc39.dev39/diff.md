# Comparing `tmp/arion_library-1.1rc37.dev37.tar.gz` & `tmp/arion_library-1.1rc39.dev39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc37.dev37.tar", last modified: Mon Apr  8 14:15:29 2024, max compression
+gzip compressed data, was "arion_library-1.1rc39.dev39.tar", last modified: Mon Apr  8 14:42:09 2024, max compression
```

## Comparing `arion_library-1.1rc37.dev37.tar` & `arion_library-1.1rc39.dev39.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.497987 arion_library-1.1rc37.dev37/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 14:15:29.000000 arion_library-1.1rc37.dev37/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 14:15:29.000000 arion_library-1.1rc37.dev37/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:15:29.000000 arion_library-1.1rc37.dev37/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 14:15:29.000000 arion_library-1.1rc37.dev37/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 14:15:29.000000 arion_library-1.1rc37.dev37/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/SFTP/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/SFTP/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/SFTP/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/SFTP/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/SFTP/lib/sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/SFTP/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/SFTP/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/SFTP/tests/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/TableStorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/TableStorage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/TableStorage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/TableStorage/lib/TableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/TableStorage/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/TableStorage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/TableStorage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/TableStorage/tests/test_table_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/azure_blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/azureBlobStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:15:29.501987 arion_library-1.1rc37.dev37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-08 14:15:09.000000 arion_library-1.1rc37.dev37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-08 14:42:09.000000 arion_library-1.1rc39.dev39/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-08 14:42:09.000000 arion_library-1.1rc39.dev39/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 14:42:09.000000 arion_library-1.1rc39.dev39/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 14:42:09.000000 arion_library-1.1rc39.dev39/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 14:42:09.000000 arion_library-1.1rc39.dev39/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/SFTP/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/SFTP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/SFTP/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/SFTP/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/SFTP/lib/sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/SFTP/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/SFTP/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/SFTP/tests/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/TableStorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/TableStorage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/TableStorage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/TableStorage/lib/TableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/TableStorage/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/TableStorage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/TableStorage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/TableStorage/tests/test_table_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/azure_blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.900654 arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/azureBlobStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 14:41:37.000000 arion_library-1.1rc39.dev39/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 14:42:09.904654 arion_library-1.1rc39.dev39/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-08 14:42:06.000000 arion_library-1.1rc39.dev39/setup.py
```

### Comparing `arion_library-1.1rc37.dev37/arion_library.egg-info/SOURCES.txt` & `arion_library-1.1rc39.dev39/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/SFTP/lib/sftp.py` & `arion_library-1.1rc39.dev39/processors/SFTP/lib/sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/SFTP/tests/test_sftp.py` & `arion_library-1.1rc39.dev39/processors/SFTP/tests/test_sftp.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/TableStorage/lib/TableStorage.py` & `arion_library-1.1rc39.dev39/processors/TableStorage/lib/TableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/TableStorage/tests/test_table_storage.py` & `arion_library-1.1rc39.dev39/processors/TableStorage/tests/test_table_storage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/azureBlobStorage.py` & `arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/azure_blob_storage/lib/config.py` & `arion_library-1.1rc39.dev39/processors/azure_blob_storage/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/test_blob.py` & `arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/azure_blob_storage/tests/test_env.py` & `arion_library-1.1rc39.dev39/processors/azure_blob_storage/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/msserversql/lib/MsServerSQL.py` & `arion_library-1.1rc39.dev39/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/processors/msserversql/tests/test_methods.py` & `arion_library-1.1rc39.dev39/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc37.dev37/setup.py` & `arion_library-1.1rc39.dev39/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 
 from setuptools import setup, find_packages
 import os
 
-# Read the version from the environment variable
-version = os.getenv('1.1rc37.dev37')
-
-
 # Get the absolute path of the directory containing setup.py
 base_dir = os.path.abspath(os.path.dirname(__file__))
 required_txt_path = os.path.join(base_dir, "required.txt")
 if os.path.exists(required_txt_path):
     with open(required_txt_path) as f:
         required = f.read().splitlines()
 else:
     required = []
 
-# with open('required.txt') as f:
-#     required = list(set(f.read().splitlines()))
-
-
 setup(
     name='arion_library',  # Replace with your package name
-    version='1.1rc37.dev37',  # Replace with your package version
+    version='1.1rc39.dev39',  # Replace with your package version
     author='Heni Nechi',  # Replace with your name
     author_email='h.nechi@arion-tech.com',  # Replace with your email
     url='https://github.com/Ariontech/ArionLibrary.git',  # Replace with your repository URL
     packages=find_packages(),  # Automatically find all packages
     python_requires='>=3.8',  # Specify Python version requirements
     install_requires=required,
 )
```

