# Comparing `tmp/advcalc-0.1.7.tar.gz` & `tmp/advcalc-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advcalc-0.1.7.tar", last modified: Mon Apr  8 03:13:54 2024, max compression
+gzip compressed data, was "advcalc-0.1.8.tar", last modified: Tue Apr  9 04:26:52 2024, max compression
```

## Comparing `advcalc-0.1.7.tar` & `advcalc-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 03:13:54.325625 advcalc-0.1.7/
-drwxrwxrwx   0        0        0        0 2024-04-08 03:13:54.266817 advcalc-0.1.7/ADVCALC/
--rw-rw-rw-   0        0        0     2122 2024-04-07 23:46:12.000000 advcalc-0.1.7/ADVCALC/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      799 2024-04-08 03:13:54.322223 advcalc-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 03:13:54.319594 advcalc-0.1.7/advcalc.egg-info/
--rw-rw-rw-   0        0        0      799 2024-04-08 03:13:54.000000 advcalc-0.1.7/advcalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-04-08 03:13:54.000000 advcalc-0.1.7/advcalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 03:13:54.000000 advcalc-0.1.7/advcalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-08 03:13:54.000000 advcalc-0.1.7/advcalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-08 03:13:54.000000 advcalc-0.1.7/advcalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 03:13:54.325625 advcalc-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-04-08 03:13:51.000000 advcalc-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 04:26:52.425344 advcalc-0.1.8/
+drwxrwxrwx   0        0        0        0 2024-04-09 04:26:52.398656 advcalc-0.1.8/ADVCALC/
+-rw-rw-rw-   0        0        0     2703 2024-04-09 04:23:23.000000 advcalc-0.1.8/ADVCALC/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-05 02:48:20.000000 advcalc-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      799 2024-04-09 04:26:52.423312 advcalc-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-07 23:50:10.000000 advcalc-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 04:26:52.421298 advcalc-0.1.8/advcalc.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 04:26:52.000000 advcalc-0.1.8/advcalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 04:26:52.425344 advcalc-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      743 2024-04-09 04:26:48.000000 advcalc-0.1.8/setup.py
```

### Comparing `advcalc-0.1.7/LICENSE` & `advcalc-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.7/PKG-INFO` & `advcalc-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

### Comparing `advcalc-0.1.7/README.md` & `advcalc-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `advcalc-0.1.7/advcalc.egg-info/PKG-INFO` & `advcalc-0.1.8/advcalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: advcalc
-Version: 0.1.7
+Version: 0.1.8
 Summary: Advanced Python Calculator With an API
 Author: Zack
 License: MIT
 Keywords: python,calculator
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
```

### Comparing `advcalc-0.1.7/setup.py` & `advcalc-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
-VERSION = '0.1.7' 
+VERSION = '0.1.8' 
 DESCRIPTION = 'Advanced Python Calculator With an API'
 
 setup(
     name="advcalc", 
     version=VERSION,
     author="Zack",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # Make sure this correctly locates all your packages
     keywords=['python', 'calculator'],
     license="MIT",  # Verify that this license matches your project
-    install_requires=["setuptools>=61.0"]
+    install_requires=["setuptools>=61.0"],
+    entry_points={
+        "console_scripts": [
+            "advcalc = advcalc.init:main"
+        ]
+    }
 )
```

