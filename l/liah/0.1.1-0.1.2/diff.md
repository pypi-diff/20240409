# Comparing `tmp/liah-0.1.1.tar.gz` & `tmp/liah-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liah-0.1.1.tar", last modified: Tue Apr  9 12:15:06 2024, max compression
+gzip compressed data, was "liah-0.1.2.tar", last modified: Tue Apr  9 12:28:22 2024, max compression
```

## Comparing `liah-0.1.1.tar` & `liah-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.724910 liah-0.1.1/
--rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.1/LICENSE
--rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.1/MANIFEST.in
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:15:06.724678 liah-0.1.1/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.1/README.md
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.720341 liah-0.1.1/liah/
--rw-r--r--   0 melvin     (501) staff       (20)     5124 2024-04-09 12:14:00.000000 liah-0.1.1/liah/Liah.py
--rw-r--r--   0 melvin     (501) staff       (20)        0 2024-04-06 16:08:56.000000 liah-0.1.1/liah/__init__.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.723769 liah-0.1.1/liah/dataset/
--rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.1/liah/dataset/README.md
--rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset/daughter_of_the_dawn.txt
--rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset/when_everybody_knew.txt
--rw-r--r--   0 melvin     (501) staff       (20)     8668 2024-04-06 16:08:56.000000 liah-0.1.1/liah/dataset_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-09 12:14:23.000000 liah-0.1.1/liah/evaluator.py
--rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.1/liah/plot_utils.py
--rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 16:08:56.000000 liah-0.1.1/liah/utils.py
-drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:15:06.724400 liah-0.1.1/liah.egg-info/
--rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/PKG-INFO
--rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/SOURCES.txt
--rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/dependency_links.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/requires.txt
--rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 12:15:06.000000 liah-0.1.1/liah.egg-info/top_level.txt
--rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.1/requirements.txt
--rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 12:15:06.724962 liah-0.1.1/setup.cfg
--rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 12:14:53.000000 liah-0.1.1/setup.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.791067 liah-0.1.2/
+-rw-r--r--   0 melvin     (501) staff       (20)     1080 2024-04-06 16:08:56.000000 liah-0.1.2/LICENSE
+-rw-r--r--   0 melvin     (501) staff       (20)       48 2024-04-06 16:08:56.000000 liah-0.1.2/MANIFEST.in
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:28:22.790793 liah-0.1.2/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)     1380 2024-04-09 12:07:14.000000 liah-0.1.2/README.md
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.786965 liah-0.1.2/liah/
+-rw-r--r--   0 melvin     (501) staff       (20)     5124 2024-04-09 12:14:00.000000 liah-0.1.2/liah/Liah.py
+-rw-r--r--   0 melvin     (501) staff       (20)       23 2024-04-09 12:26:18.000000 liah-0.1.2/liah/__init__.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.789786 liah-0.1.2/liah/dataset/
+-rw-r--r--   0 melvin     (501) staff       (20)       59 2024-04-03 16:37:16.000000 liah-0.1.2/liah/dataset/README.md
+-rw-r--r--   0 melvin     (501) staff       (20)   604855 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset/daughter_of_the_dawn.txt
+-rw-r--r--   0 melvin     (501) staff       (20)    36325 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset/when_everybody_knew.txt
+-rw-r--r--   0 melvin     (501) staff       (20)     8668 2024-04-06 16:08:56.000000 liah-0.1.2/liah/dataset_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     3359 2024-04-09 12:14:23.000000 liah-0.1.2/liah/evaluator.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1928 2024-04-06 16:08:56.000000 liah-0.1.2/liah/plot_utils.py
+-rw-r--r--   0 melvin     (501) staff       (20)     1339 2024-04-06 16:08:56.000000 liah-0.1.2/liah/utils.py
+drwxr-xr-x   0 melvin     (501) staff       (20)        0 2024-04-09 12:28:22.790500 liah-0.1.2/liah.egg-info/
+-rw-r--r--   0 melvin     (501) staff       (20)     1891 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/PKG-INFO
+-rw-r--r--   0 melvin     (501) staff       (20)      395 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/SOURCES.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        1 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/dependency_links.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/requires.txt
+-rw-r--r--   0 melvin     (501) staff       (20)        5 2024-04-09 12:28:22.000000 liah-0.1.2/liah.egg-info/top_level.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       40 2024-04-06 09:10:37.000000 liah-0.1.2/requirements.txt
+-rw-r--r--   0 melvin     (501) staff       (20)       38 2024-04-09 12:28:22.791122 liah-0.1.2/setup.cfg
+-rw-r--r--   0 melvin     (501) staff       (20)      910 2024-04-09 12:28:18.000000 liah-0.1.2/setup.py
```

### Comparing `liah-0.1.1/LICENSE` & `liah-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/PKG-INFO` & `liah-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.1
+Version: 0.1.2
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
```

### Comparing `liah-0.1.1/README.md` & `liah-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/Liah.py` & `liah-0.1.2/liah/Liah.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/dataset/daughter_of_the_dawn.txt` & `liah-0.1.2/liah/dataset/daughter_of_the_dawn.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/dataset/when_everybody_knew.txt` & `liah-0.1.2/liah/dataset/when_everybody_knew.txt`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/dataset_utils.py` & `liah-0.1.2/liah/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/evaluator.py` & `liah-0.1.2/liah/evaluator.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/plot_utils.py` & `liah-0.1.2/liah/plot_utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah/utils.py` & `liah-0.1.2/liah/utils.py`

 * *Files identical despite different names*

### Comparing `liah-0.1.1/liah.egg-info/PKG-INFO` & `liah-0.1.2/liah.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liah
-Version: 0.1.1
+Version: 0.1.2
 Summary: Insert a Lie in a Haystack and evaluate the model's ability to detect it.
 Home-page: https://github.com/melvinebenezer/Liah-Lie_in_a_haystack
 Author: James Melvin Priyarajan
 Author-email: melvinebenezer@gmail.com
 License: Apache 2.0
 Keywords: llm,needle in a haystack
 Requires-Python: >=3.6
```

### Comparing `liah-0.1.1/setup.py` & `liah-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 print(current_directory)
 requirements_path = os.path.join(current_directory, "requirements.txt")
 with open(requirements_path, "r") as file:
     requirements = file.read().splitlines()
 
 setup(
     name="liah",
-    version="0.1.1",
+    version="0.1.2",
     author="James Melvin Priyarajan",
     author_email="melvinebenezer@gmail.com",
     description="Insert a Lie in a Haystack and evaluate the model's ability to detect it.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/melvinebenezer/Liah-Lie_in_a_haystack",
     packages=find_packages(),
```

