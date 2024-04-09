# Comparing `tmp/llmreader-0.2.4.tar.gz` & `tmp/llmreader-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreader-0.2.4.tar", last modified: Thu Apr  4 02:25:48 2024, max compression
+gzip compressed data, was "llmreader-0.2.5.tar", last modified: Tue Apr  9 02:17:56 2024, max compression
```

## Comparing `llmreader-0.2.4.tar` & `llmreader-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-04 02:25:48.662382 llmreader-0.2.4/
--rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.4/LICENSE
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-04 02:25:48.662263 llmreader-0.2.4/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.4/README.md
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-04 02:25:48.661323 llmreader-0.2.4/llmreader/
--rw-r--r--   0 ethanhou   (501) staff       (20)       54 2024-04-04 02:21:26.000000 llmreader-0.2.4/llmreader/__init__.py
--rw-r--r--   0 ethanhou   (501) staff       (20)      935 2024-04-04 02:21:46.000000 llmreader-0.2.4/llmreader/inject.py
-drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-04 02:25:48.662098 llmreader-0.2.4/llmreader.egg-info/
--rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-04 02:25:48.000000 llmreader-0.2.4/llmreader.egg-info/PKG-INFO
--rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-04 02:25:48.000000 llmreader-0.2.4/llmreader.egg-info/SOURCES.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-04 02:25:48.000000 llmreader-0.2.4/llmreader.egg-info/dependency_links.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-04 02:25:48.000000 llmreader-0.2.4/llmreader.egg-info/requires.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-04 02:25:48.000000 llmreader-0.2.4/llmreader.egg-info/top_level.txt
--rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-04 02:25:48.662430 llmreader-0.2.4/setup.cfg
--rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-04 02:22:28.000000 llmreader-0.2.4/setup.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-09 02:17:56.860119 llmreader-0.2.5/
+-rw-r--r--   0 ethanhou   (501) staff       (20)     1068 2024-04-03 05:22:35.000000 llmreader-0.2.5/LICENSE
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-09 02:17:56.859994 llmreader-0.2.5/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)       56 2024-04-03 21:45:53.000000 llmreader-0.2.5/README.md
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-09 02:17:56.858943 llmreader-0.2.5/llmreader/
+-rw-r--r--   0 ethanhou   (501) staff       (20)       54 2024-04-04 02:21:26.000000 llmreader-0.2.5/llmreader/__init__.py
+-rw-r--r--   0 ethanhou   (501) staff       (20)     3173 2024-04-09 02:16:57.000000 llmreader-0.2.5/llmreader/inject.py
+drwxr-xr-x   0 ethanhou   (501) staff       (20)        0 2024-04-09 02:17:56.859800 llmreader-0.2.5/llmreader.egg-info/
+-rw-r--r--   0 ethanhou   (501) staff       (20)      308 2024-04-09 02:17:56.000000 llmreader-0.2.5/llmreader.egg-info/PKG-INFO
+-rw-r--r--   0 ethanhou   (501) staff       (20)      232 2024-04-09 02:17:56.000000 llmreader-0.2.5/llmreader.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        1 2024-04-09 02:17:56.000000 llmreader-0.2.5/llmreader.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)        7 2024-04-09 02:17:56.000000 llmreader-0.2.5/llmreader.egg-info/requires.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       10 2024-04-09 02:17:56.000000 llmreader-0.2.5/llmreader.egg-info/top_level.txt
+-rw-r--r--   0 ethanhou   (501) staff       (20)       38 2024-04-09 02:17:56.860169 llmreader-0.2.5/setup.cfg
+-rw-r--r--   0 ethanhou   (501) staff       (20)      532 2024-04-09 02:17:05.000000 llmreader-0.2.5/setup.py
```

### Comparing `llmreader-0.2.4/LICENSE` & `llmreader-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmreader-0.2.4/setup.py` & `llmreader-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="llmreader",
-    version="0.2.4",
+    version="0.2.5",
     description="Intercept OpenAI inputs",
     author="Ethan Hou",
     author_email="ethanfhou10@gmail.com",
     packages=find_packages(),
     install_requires=[
         'openai'
     ],
```

