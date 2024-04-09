# Comparing `tmp/unitlab-2.1.6.tar.gz` & `tmp/unitlab-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-2.1.6.tar", last modified: Mon Apr  8 13:29:09 2024, max compression
+gzip compressed data, was "unitlab-2.1.7.tar", last modified: Tue Apr  9 10:30:19 2024, max compression
```

## Comparing `unitlab-2.1.6.tar` & `unitlab-2.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/
--rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.6/LICENSE.md
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-08 13:29:09.347086 unitlab-2.1.6/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.6/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-08 13:29:09.347086 unitlab-2.1.6/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-08 13:28:42.000000 unitlab-2.1.6/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.6/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.6/src/unitlab/__main__.py
--rw-rw-r--   0 me        (1000) me        (1000)    12065 2024-04-08 12:17:22.000000 unitlab-2.1.6/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.6/src/unitlab/dataset.py
--rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.6/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     4553 2024-04-08 12:17:26.000000 unitlab-2.1.6/src/unitlab/main.py
--rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.6/src/unitlab/utils.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-08 13:29:09.347086 unitlab-2.1.6/src/unitlab.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-08 13:29:09.000000 unitlab-2.1.6/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 10:30:19.215947 unitlab-2.1.7/
+-rw-rw-r--   0 me        (1000) me        (1000)     1069 2024-02-13 07:39:37.000000 unitlab-2.1.7/LICENSE.md
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-09 10:30:19.215947 unitlab-2.1.7/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1434 2023-09-24 12:59:00.000000 unitlab-2.1.7/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2024-04-09 10:30:19.219947 unitlab-2.1.7/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1092 2024-04-09 10:29:37.000000 unitlab-2.1.7/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 10:30:19.215947 unitlab-2.1.7/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 10:30:19.215947 unitlab-2.1.7/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2024-04-05 11:53:23.000000 unitlab-2.1.7/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)       29 2024-03-06 15:43:31.000000 unitlab-2.1.7/src/unitlab/__main__.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12065 2024-04-09 10:29:15.000000 unitlab-2.1.7/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12386 2024-04-05 09:59:30.000000 unitlab-2.1.7/src/unitlab/dataset.py
+-rw-rw-r--   0 me        (1000) me        (1000)      950 2024-04-05 12:19:27.000000 unitlab-2.1.7/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     4560 2024-04-09 10:15:52.000000 unitlab-2.1.7/src/unitlab/main.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1852 2024-04-05 12:20:07.000000 unitlab-2.1.7/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2024-04-09 10:30:19.215947 unitlab-2.1.7/src/unitlab.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      793 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      411 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       45 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       48 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2024-04-09 10:30:19.000000 unitlab-2.1.7/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-2.1.6/LICENSE.md` & `unitlab-2.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/PKG-INFO` & `unitlab-2.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.6
+Version: 2.1.7
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-2.1.6/README.md` & `unitlab-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/setup.py` & `unitlab-2.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="2.1.6",
+    version="2.1.7",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-2.1.6/src/unitlab/client.py` & `unitlab-2.1.7/src/unitlab/client.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/src/unitlab/dataset.py` & `unitlab-2.1.7/src/unitlab/dataset.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/src/unitlab/exceptions.py` & `unitlab-2.1.7/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/src/unitlab/main.py` & `unitlab-2.1.7/src/unitlab/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,13 +140,13 @@
     ] = "COCO",
 ):
     if download_type == DownloadType.annotation:
         if not export_type:
             raise typer.BadParameter(
                 "Export type is required when download type is annotation"
             )
-        get_client(api_key).dataset_download(pk, export_type)
+        return get_client(api_key).dataset_download(pk, export_type)
     get_client(api_key).dataset_download_files(pk)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `unitlab-2.1.6/src/unitlab/utils.py` & `unitlab-2.1.7/src/unitlab/utils.py`

 * *Files identical despite different names*

### Comparing `unitlab-2.1.6/src/unitlab.egg-info/PKG-INFO` & `unitlab-2.1.7/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 2.1.6
+Version: 2.1.7
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

