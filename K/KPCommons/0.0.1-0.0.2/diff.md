# Comparing `tmp/KPCommons-0.0.1.tar.gz` & `tmp/KPCommons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KPCommons-0.0.1.tar", last modified: Wed Mar 27 12:43:45 2024, max compression
+gzip compressed data, was "KPCommons-0.0.2.tar", last modified: Tue Apr  9 09:07:26 2024, max compression
```

## Comparing `KPCommons-0.0.1.tar` & `KPCommons-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 frede      (501) staff       (20)        0 2024-03-27 12:43:45.998654 KPCommons-0.0.1/
-drwxr-xr-x   0 frede      (501) staff       (20)        0 2024-03-27 12:43:45.998006 KPCommons-0.0.1/KPCommons.egg-info/
--rw-r--r--   0 frede      (501) staff       (20)    13453 2024-03-27 12:43:45.000000 KPCommons-0.0.1/KPCommons.egg-info/PKG-INFO
--rw-r--r--   0 frede      (501) staff       (20)      226 2024-03-27 12:43:45.000000 KPCommons-0.0.1/KPCommons.egg-info/SOURCES.txt
--rw-r--r--   0 frede      (501) staff       (20)        1 2024-03-27 12:43:45.000000 KPCommons-0.0.1/KPCommons.egg-info/dependency_links.txt
--rw-r--r--   0 frede      (501) staff       (20)       10 2024-03-27 12:43:45.000000 KPCommons-0.0.1/KPCommons.egg-info/top_level.txt
--rw-r--r--   0 frede      (501) staff       (20)    11347 2023-01-26 17:31:09.000000 KPCommons-0.0.1/LICENSE
--rw-r--r--   0 frede      (501) staff       (20)    13453 2024-03-27 12:43:45.998323 KPCommons-0.0.1/PKG-INFO
--rw-r--r--   0 frede      (501) staff       (20)        8 2024-03-27 10:23:57.000000 KPCommons-0.0.1/README.md
-drwxr-xr-x   0 frede      (501) staff       (20)        0 2024-03-27 12:43:45.997699 KPCommons-0.0.1/kpcommons/
--rw-r--r--   0 frede      (501) staff       (20)     2691 2024-03-27 12:43:28.000000 KPCommons-0.0.1/kpcommons/Footnote.py
--rw-r--r--   0 frede      (501) staff       (20)      507 2024-03-27 12:32:34.000000 KPCommons-0.0.1/kpcommons/Util.py
--rw-r--r--   0 frede      (501) staff       (20)        0 2024-03-27 12:18:34.000000 KPCommons-0.0.1/kpcommons/__init__.py
--rw-r--r--   0 frede      (501) staff       (20)      717 2024-03-27 12:26:40.000000 KPCommons-0.0.1/pyproject.toml
--rw-r--r--   0 frede      (501) staff       (20)       38 2024-03-27 12:43:45.998692 KPCommons-0.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/KPCommons.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14020 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-09 09:07:26.000000 KPCommons-0.0.2/KPCommons.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 06:42:51.000000 KPCommons-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14020 2024-04-09 09:07:26.008922 KPCommons-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-09 09:06:35.000000 KPCommons-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:07:26.008922 KPCommons-0.0.2/kpcommons/
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-04-09 06:42:51.000000 KPCommons-0.0.2/kpcommons/Footnote.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-04-09 09:06:35.000000 KPCommons-0.0.2/kpcommons/Util.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 09:07:11.000000 KPCommons-0.0.2/kpcommons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-04-09 09:06:35.000000 KPCommons-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:07:26.008922 KPCommons-0.0.2/setup.cfg
```

### Comparing `KPCommons-0.0.1/KPCommons.egg-info/PKG-INFO` & `KPCommons-0.0.2/KPCommons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KPCommons
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of reusable methods.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,7 +210,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Readme
+
+KPCommons is a collection of methods which are regularly needed.
+
+## Util
+
+Util.py contains a method to calculate the overlap between two ranges. For example,
+
+~~~
+Util.calculate_overlap(0, 10, 5, 10)
+~~~
+
+would return a result of 5. The first two arguments are the start and end position of the first range, and the last two
+arguments are the positions of the second range.
+
+**Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+
+## Footnote
+
+Footnote.py contains a collection of methods for working with footnotes.
```

### Comparing `KPCommons-0.0.1/LICENSE` & `KPCommons-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KPCommons-0.0.1/PKG-INFO` & `KPCommons-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KPCommons
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of reusable methods.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,7 +210,26 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Readme
+
+KPCommons is a collection of methods which are regularly needed.
+
+## Util
+
+Util.py contains a method to calculate the overlap between two ranges. For example,
+
+~~~
+Util.calculate_overlap(0, 10, 5, 10)
+~~~
+
+would return a result of 5. The first two arguments are the start and end position of the first range, and the last two
+arguments are the positions of the second range.
+
+**Note**: In case of no overlap, the distance between the two ranges is returned as a negative result.
+
+## Footnote
+
+Footnote.py contains a collection of methods for working with footnotes.
```

### Comparing `KPCommons-0.0.1/kpcommons/Footnote.py` & `KPCommons-0.0.2/kpcommons/Footnote.py`

 * *Files identical despite different names*

### Comparing `KPCommons-0.0.1/pyproject.toml` & `KPCommons-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "KPCommons"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Frederik Arnold", email = "frederik.arnold@hu-berlin.de"}
 ]
 description = "A collection of reusable methods."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

