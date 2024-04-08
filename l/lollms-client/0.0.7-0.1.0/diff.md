# Comparing `tmp/lollms_client-0.0.7.tar.gz` & `tmp/lollms_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.0.7.tar", last modified: Sun Mar 31 23:27:08 2024, max compression
+gzip compressed data, was "lollms_client-0.1.0.tar", last modified: Mon Apr  8 23:34:05 2024, max compression
```

## Comparing `lollms_client-0.0.7.tar` & `lollms_client-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 23:27:08.010355 lollms_client-0.0.7/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     3286 2024-03-31 23:27:08.009356 lollms_client-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2808 2024-03-30 20:09:03.000000 lollms_client-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 23:27:07.986353 lollms_client-0.0.7/lollms_client/
--rw-rw-rw-   0        0        0     1693 2024-03-31 23:26:03.000000 lollms_client-0.0.7/lollms_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 23:27:08.008352 lollms_client-0.0.7/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3286 2024-03-31 23:27:07.000000 lollms_client-0.0.7/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-03-31 23:27:07.000000 lollms_client-0.0.7/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 23:27:07.000000 lollms_client-0.0.7/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 23:27:07.000000 lollms_client-0.0.7/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-31 23:27:07.000000 lollms_client-0.0.7/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 23:27:08.010355 lollms_client-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-03-31 23:26:26.000000 lollms_client-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.410728 lollms_client-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-08 23:34:05.409720 lollms_client-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.395691 lollms_client-0.1.0/lollms_client/
+-rw-rw-rw-   0        0        0     6583 2024-04-08 23:32:07.000000 lollms_client-0.1.0/lollms_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 23:34:05.408212 lollms_client-0.1.0/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-08 23:34:05.000000 lollms_client-0.1.0/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 23:34:05.410728 lollms_client-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-07 10:55:31.000000 lollms_client-0.1.0/setup.py
```

### Comparing `lollms_client-0.0.7/LICENSE` & `lollms_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.0.7/setup.py` & `lollms_client-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lollms_client",
-    version="0.0.7",
+    version="0.1.0",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

