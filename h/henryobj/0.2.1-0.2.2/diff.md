# Comparing `tmp/henryobj-0.2.1.tar.gz` & `tmp/henryobj-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.1.tar", last modified: Sat Mar 30 16:10:22 2024, max compression
+gzip compressed data, was "henryobj-0.2.2.tar", last modified: Tue Apr  9 07:09:00 2024, max compression
```

## Comparing `henryobj-0.2.1.tar` & `henryobj-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-03-30 16:10:22.601708 henryobj-0.2.1/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-03-30 16:10:22.601567 henryobj-0.2.1/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.1/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-03-30 16:10:22.600497 henryobj-0.2.1/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      135 2024-03-30 15:20:39.000000 henryobj-0.2.1/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    21017 2024-03-30 16:01:52.000000 henryobj-0.2.1/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1475 2024-03-30 15:45:13.000000 henryobj-0.2.1/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    15087 2024-03-30 15:15:07.000000 henryobj-0.2.1/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    24819 2024-03-30 16:01:22.000000 henryobj-0.2.1/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14268 2024-03-30 15:59:40.000000 henryobj-0.2.1/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-03-30 16:10:22.601375 henryobj-0.2.1/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-03-30 16:10:22.000000 henryobj-0.2.1/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-03-30 16:10:22.000000 henryobj-0.2.1/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-03-30 16:10:22.000000 henryobj-0.2.1/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-03-30 16:10:22.000000 henryobj-0.2.1/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-03-30 16:10:22.000000 henryobj-0.2.1/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-03-30 16:10:22.601757 henryobj-0.2.1/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      575 2024-03-30 16:10:20.000000 henryobj-0.2.1/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:09:00.000698 henryobj-0.2.2/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-09 07:09:00.000568 henryobj-0.2.2/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.2/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:08:59.999588 henryobj-0.2.2/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.2/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    21017 2024-03-30 16:01:52.000000 henryobj-0.2.2/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1475 2024-03-30 15:45:13.000000 henryobj-0.2.2/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    15087 2024-03-30 15:15:07.000000 henryobj-0.2.2/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    24819 2024-03-30 16:01:22.000000 henryobj-0.2.2/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14268 2024-03-30 15:59:40.000000 henryobj-0.2.2/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-09 07:09:00.000399 henryobj-0.2.2/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-09 07:08:59.000000 henryobj-0.2.2/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-09 07:09:00.000742 henryobj-0.2.2/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-09 07:07:08.000000 henryobj-0.2.2/setup.py
```

### Comparing `henryobj-0.2.1/PKG-INFO` & `henryobj-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: henryobj
-Version: 0.2.1
-Home-page: https://github.com/HenryObj/mypip
-Description-Content-Type: text/markdown
-
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
 
 ## Module Descriptions
 
 ### `web.py`
@@ -49,8 +43,8 @@
 ### `__init__.py`
 
 - **Purpose:** Serves as the package initializer, importing all necessary modules for user accessibility.
 - **Interactions:** Critical for package integrity, enabling module imports upon package usage without housing direct functionality.
 
 ## Additional Notes
 
-This ReadME was generated automatically. See gpt.py to use it for your repos.
+This ReadME was generated automatically. See gpt.py to use it for your repos.
```

### Comparing `henryobj-0.2.1/README.md` & `henryobj-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: henryobj
+Version: 0.2.2
+Home-page: https://github.com/HenryObj/mypip
+Description-Content-Type: text/markdown
+
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
 
 ## Module Descriptions
 
 ### `web.py`
@@ -43,8 +49,8 @@
 ### `__init__.py`
 
 - **Purpose:** Serves as the package initializer, importing all necessary modules for user accessibility.
 - **Interactions:** Critical for package integrity, enabling module imports upon package usage without housing direct functionality.
 
 ## Additional Notes
 
-This ReadME was generated automatically. See gpt.py to use it for your repos.
+This ReadME was generated automatically. See gpt.py to use it for your repos.
```

### Comparing `henryobj-0.2.1/henryobj/base.py` & `henryobj-0.2.2/henryobj/base.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.1/henryobj/config.py` & `henryobj-0.2.2/henryobj/config.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.1/henryobj/gpt.py` & `henryobj-0.2.2/henryobj/gpt.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.1/henryobj/oai.py` & `henryobj-0.2.2/henryobj/oai.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.1/henryobj/web.py` & `henryobj-0.2.2/henryobj/web.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.1/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.2/henryobj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.1/setup.py` & `henryobj-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.01", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.2", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

