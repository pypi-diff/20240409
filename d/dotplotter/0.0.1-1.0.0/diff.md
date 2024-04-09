# Comparing `tmp/dotplotter-0.0.1.tar.gz` & `tmp/dotplotter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotplotter-0.0.1.tar", last modified: Tue Apr  9 12:40:11 2024, max compression
+gzip compressed data, was "dotplotter-1.0.0.tar", last modified: Tue Apr  9 12:43:37 2024, max compression
```

## Comparing `dotplotter-0.0.1.tar` & `dotplotter-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:40:11.459318 dotplotter-0.0.1/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)    35149 2024-04-03 15:32:47.000000 dotplotter-0.0.1/LICENSE
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2724 2024-04-09 12:40:11.459318 dotplotter-0.0.1/PKG-INFO
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2348 2024-04-09 12:29:57.000000 dotplotter-0.0.1/README.md
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:40:11.459318 dotplotter-0.0.1/dotplotter/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)        0 2024-03-27 13:24:00.000000 dotplotter-0.0.1/dotplotter/__init__.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2121 2024-04-09 11:25:15.000000 dotplotter-0.0.1/dotplotter/check_input.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3765 2024-04-09 11:28:25.000000 dotplotter-0.0.1/dotplotter/chunks.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3645 2024-04-09 11:27:35.000000 dotplotter-0.0.1/dotplotter/main.py
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2765 2024-04-09 11:34:02.000000 dotplotter-0.0.1/dotplotter/parser.py
-drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:40:11.459318 dotplotter-0.0.1/dotplotter.egg-info/
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2724 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/PKG-INFO
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      342 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/SOURCES.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)        1 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/dependency_links.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       53 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/entry_points.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       11 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/requires.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       11 2024-04-09 12:40:11.000000 dotplotter-0.0.1/dotplotter.egg-info/top_level.txt
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)       38 2024-04-09 12:40:11.459318 dotplotter-0.0.1/setup.cfg
--rw-r--r--   0 thoboo    (1000) thoboo    (1000)      661 2024-04-09 09:27:42.000000 dotplotter-0.0.1/setup.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:43:37.832695 dotplotter-1.0.0/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)    35149 2024-04-03 15:32:47.000000 dotplotter-1.0.0/LICENSE
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2730 2024-04-09 12:43:37.832695 dotplotter-1.0.0/PKG-INFO
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2348 2024-04-09 12:29:57.000000 dotplotter-1.0.0/README.md
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:43:37.832695 dotplotter-1.0.0/dotplotter/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)        0 2024-03-27 13:24:00.000000 dotplotter-1.0.0/dotplotter/__init__.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2121 2024-04-09 11:25:15.000000 dotplotter-1.0.0/dotplotter/check_input.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3765 2024-04-09 11:28:25.000000 dotplotter-1.0.0/dotplotter/chunks.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     3645 2024-04-09 11:27:35.000000 dotplotter-1.0.0/dotplotter/main.py
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2765 2024-04-09 11:34:02.000000 dotplotter-1.0.0/dotplotter/parser.py
+drwxr-xr-x   0 thoboo    (1000) thoboo    (1000)        0 2024-04-09 12:43:37.832695 dotplotter-1.0.0/dotplotter.egg-info/
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)     2730 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/PKG-INFO
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      342 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)        1 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       52 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/entry_points.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       11 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/requires.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       11 2024-04-09 12:43:37.000000 dotplotter-1.0.0/dotplotter.egg-info/top_level.txt
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)       38 2024-04-09 12:43:37.832695 dotplotter-1.0.0/setup.cfg
+-rw-r--r--   0 thoboo    (1000) thoboo    (1000)      661 2024-04-09 12:40:27.000000 dotplotter-1.0.0/setup.py
```

### Comparing `dotplotter-0.0.1/LICENSE` & `dotplotter-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/PKG-INFO` & `dotplotter-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dotplotter
-Version: 0.0.1
+Version: 1.0.0
 Summary: A python for plotting dot plots from blast results.
 Home-page: https://github.com/DrBoothTJ/dotplotter
 Author: Thomas J. Booth
 Author-email: thoboo@biosustain.dtu.dk
 License: GNU General Public License v3.0
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
 
 # dotplotter
 build dotplots from blastn results
 
 ## Description
 `dotplotter` can take blast results, either as standard input or from a .tsv file and plots a standard dot plot. It can also highlight regions based on provided arguments (single region) or from a file (single or multiple regions) see below. Dot plots are a classic way to visualise DNA similarity and can be used for whole chromosomes or small regions.
 
@@ -70,9 +70,7 @@
 ## Citation
 Coming soon...
 
 ## Patch Notes
 ### Verion 1
 - 1.0.0
   - initial release
-
-
```

### Comparing `dotplotter-0.0.1/README.md` & `dotplotter-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/dotplotter/check_input.py` & `dotplotter-1.0.0/dotplotter/check_input.py`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/dotplotter/chunks.py` & `dotplotter-1.0.0/dotplotter/chunks.py`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/dotplotter/main.py` & `dotplotter-1.0.0/dotplotter/main.py`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/dotplotter/parser.py` & `dotplotter-1.0.0/dotplotter/parser.py`

 * *Files identical despite different names*

### Comparing `dotplotter-0.0.1/dotplotter.egg-info/PKG-INFO` & `dotplotter-1.0.0/dotplotter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dotplotter
-Version: 0.0.1
+Version: 1.0.0
 Summary: A python for plotting dot plots from blast results.
 Home-page: https://github.com/DrBoothTJ/dotplotter
 Author: Thomas J. Booth
 Author-email: thoboo@biosustain.dtu.dk
 License: GNU General Public License v3.0
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
 
 # dotplotter
 build dotplots from blastn results
 
 ## Description
 `dotplotter` can take blast results, either as standard input or from a .tsv file and plots a standard dot plot. It can also highlight regions based on provided arguments (single region) or from a file (single or multiple regions) see below. Dot plots are a classic way to visualise DNA similarity and can be used for whole chromosomes or small regions.
 
@@ -70,9 +70,7 @@
 ## Citation
 Coming soon...
 
 ## Patch Notes
 ### Verion 1
 - 1.0.0
   - initial release
-
-
```

### Comparing `dotplotter-0.0.1/setup.py` & `dotplotter-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="dotplotter",
-    version="0.0.1",
+    version="1.0.0",
     author="Thomas J. Booth",
     author_email="thoboo@biosustain.dtu.dk",
     packages=find_packages(),
     description="A python for plotting dot plots from blast results.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/DrBoothTJ/dotplotter",
```

