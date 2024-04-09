# Comparing `tmp/itranslator-0.0.2.tar.gz` & `tmp/itranslator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itranslator-0.0.2.tar", last modified: Mon Mar 18 18:28:20 2024, max compression
+gzip compressed data, was "itranslator-0.0.3.tar", last modified: Tue Apr  9 13:57:55 2024, max compression
```

## Comparing `itranslator-0.0.2.tar` & `itranslator-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 funlife   (1000) users      (100)        0 2024-03-18 18:28:20.367899 itranslator-0.0.2/
--rw-r--r--   0 funlife   (1000) users      (100)    35149 2024-03-18 15:32:04.000000 itranslator-0.0.2/LICENSE
--rw-r--r--   0 funlife   (1000) users      (100)      466 2024-03-18 18:28:20.367899 itranslator-0.0.2/PKG-INFO
--rw-r--r--   0 funlife   (1000) users      (100)       72 2024-03-18 15:32:04.000000 itranslator-0.0.2/README.md
-drwxr-xr-x   0 funlife   (1000) users      (100)        0 2024-03-18 18:28:20.367899 itranslator-0.0.2/itranslator/
--rw-r--r--   0 funlife   (1000) users      (100)       36 2024-03-18 17:59:06.000000 itranslator-0.0.2/itranslator/__init__.py
--rw-r--r--   0 funlife   (1000) users      (100)       98 2024-03-18 17:25:16.000000 itranslator-0.0.2/itranslator/exceptions.py
--rw-r--r--   0 funlife   (1000) users      (100)     2001 2024-03-18 17:58:09.000000 itranslator-0.0.2/itranslator/itranslator.py
-drwxr-xr-x   0 funlife   (1000) users      (100)        0 2024-03-18 18:28:20.367899 itranslator-0.0.2/itranslator.egg-info/
--rw-r--r--   0 funlife   (1000) users      (100)      466 2024-03-18 18:28:20.000000 itranslator-0.0.2/itranslator.egg-info/PKG-INFO
--rw-r--r--   0 funlife   (1000) users      (100)      277 2024-03-18 18:28:20.000000 itranslator-0.0.2/itranslator.egg-info/SOURCES.txt
--rw-r--r--   0 funlife   (1000) users      (100)        1 2024-03-18 18:28:20.000000 itranslator-0.0.2/itranslator.egg-info/dependency_links.txt
--rw-r--r--   0 funlife   (1000) users      (100)       20 2024-03-18 18:28:20.000000 itranslator-0.0.2/itranslator.egg-info/requires.txt
--rw-r--r--   0 funlife   (1000) users      (100)       12 2024-03-18 18:28:20.000000 itranslator-0.0.2/itranslator.egg-info/top_level.txt
--rw-r--r--   0 funlife   (1000) users      (100)       38 2024-03-18 18:28:20.367899 itranslator-0.0.2/setup.cfg
--rw-r--r--   0 funlife   (1000) users      (100)      635 2024-03-18 18:28:00.000000 itranslator-0.0.2/setup.py
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:57:55.137827 itranslator-0.0.3/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)    35149 2024-03-23 16:53:33.000000 itranslator-0.0.3/LICENSE
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     1398 2024-04-09 13:57:55.137827 itranslator-0.0.3/PKG-INFO
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      485 2024-04-09 13:43:24.000000 itranslator-0.0.3/README.md
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:57:55.135826 itranslator-0.0.3/itranslator/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       36 2024-03-23 16:53:33.000000 itranslator-0.0.3/itranslator/__init__.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       98 2024-03-23 16:53:33.000000 itranslator-0.0.3/itranslator/exceptions.py
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     2001 2024-03-23 16:53:33.000000 itranslator-0.0.3/itranslator/itranslator.py
+drwxr-xr-x   0 funlife   (1000) funlife   (1000)        0 2024-04-09 13:57:55.136826 itranslator-0.0.3/itranslator.egg-info/
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     1398 2024-04-09 13:57:55.000000 itranslator-0.0.3/itranslator.egg-info/PKG-INFO
+-rw-r--r--   0 funlife   (1000) funlife   (1000)      287 2024-04-09 13:57:55.000000 itranslator-0.0.3/itranslator.egg-info/SOURCES.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)        1 2024-04-09 13:57:55.000000 itranslator-0.0.3/itranslator.egg-info/dependency_links.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       20 2024-04-09 13:57:55.000000 itranslator-0.0.3/itranslator.egg-info/requires.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       12 2024-04-09 13:57:55.000000 itranslator-0.0.3/itranslator.egg-info/top_level.txt
+-rw-r--r--   0 funlife   (1000) funlife   (1000)       38 2024-04-09 13:57:55.137827 itranslator-0.0.3/setup.cfg
+-rw-r--r--   0 funlife   (1000) funlife   (1000)     1206 2024-04-09 13:57:42.000000 itranslator-0.0.3/setup.py
```

### Comparing `itranslator-0.0.2/LICENSE` & `itranslator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `itranslator-0.0.2/itranslator/itranslator.py` & `itranslator-0.0.3/itranslator/itranslator.py`

 * *Files identical despite different names*

