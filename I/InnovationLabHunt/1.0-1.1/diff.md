# Comparing `tmp/InnovationLabHunt-1.0.tar.gz` & `tmp/InnovationLabHunt-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InnovationLabHunt-1.0.tar", last modified: Tue Apr  9 12:58:54 2024, max compression
+gzip compressed data, was "InnovationLabHunt-1.1.tar", last modified: Tue Apr  9 13:03:15 2024, max compression
```

## Comparing `InnovationLabHunt-1.0.tar` & `InnovationLabHunt-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 12:58:54.425719 InnovationLabHunt-1.0/
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 12:58:54.424718 InnovationLabHunt-1.0/InnovationLabHunt/
--rw-r--r--   0 monish    (1000) monish    (1000)        0 2024-04-09 11:58:27.000000 InnovationLabHunt-1.0/InnovationLabHunt/__init__.py
--rw-r--r--   0 monish    (1000) monish    (1000)     6308 2024-04-09 12:33:09.000000 InnovationLabHunt-1.0/InnovationLabHunt/hunt.py
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 12:58:54.425719 InnovationLabHunt-1.0/InnovationLabHunt.egg-info/
--rw-r--r--   0 monish    (1000) monish    (1000)      144 2024-04-09 12:58:54.000000 InnovationLabHunt-1.0/InnovationLabHunt.egg-info/PKG-INFO
--rw-r--r--   0 monish    (1000) monish    (1000)      228 2024-04-09 12:58:54.000000 InnovationLabHunt-1.0/InnovationLabHunt.egg-info/SOURCES.txt
--rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-09 12:58:54.000000 InnovationLabHunt-1.0/InnovationLabHunt.egg-info/dependency_links.txt
--rw-r--r--   0 monish    (1000) monish    (1000)       18 2024-04-09 12:58:54.000000 InnovationLabHunt-1.0/InnovationLabHunt.egg-info/top_level.txt
--rw-r--r--   0 monish    (1000) monish    (1000)      144 2024-04-09 12:58:54.425719 InnovationLabHunt-1.0/PKG-INFO
--rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-09 12:58:54.425719 InnovationLabHunt-1.0/setup.cfg
--rw-r--r--   0 monish    (1000) monish    (1000)      333 2024-04-09 12:58:50.000000 InnovationLabHunt-1.0/setup.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 13:03:15.189141 InnovationLabHunt-1.1/
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 13:03:15.188141 InnovationLabHunt-1.1/InnovationLabHunt/
+-rw-r--r--   0 monish    (1000) monish    (1000)      120 2024-04-09 13:03:04.000000 InnovationLabHunt-1.1/InnovationLabHunt/__init__.py
+-rw-r--r--   0 monish    (1000) monish    (1000)     6308 2024-04-09 12:33:09.000000 InnovationLabHunt-1.1/InnovationLabHunt/hunt.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-09 13:03:15.188141 InnovationLabHunt-1.1/InnovationLabHunt.egg-info/
+-rw-r--r--   0 monish    (1000) monish    (1000)      144 2024-04-09 13:03:15.000000 InnovationLabHunt-1.1/InnovationLabHunt.egg-info/PKG-INFO
+-rw-r--r--   0 monish    (1000) monish    (1000)      228 2024-04-09 13:03:15.000000 InnovationLabHunt-1.1/InnovationLabHunt.egg-info/SOURCES.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-09 13:03:15.000000 InnovationLabHunt-1.1/InnovationLabHunt.egg-info/dependency_links.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)       18 2024-04-09 13:03:15.000000 InnovationLabHunt-1.1/InnovationLabHunt.egg-info/top_level.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)      144 2024-04-09 13:03:15.189141 InnovationLabHunt-1.1/PKG-INFO
+-rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-09 13:03:15.189141 InnovationLabHunt-1.1/setup.cfg
+-rw-r--r--   0 monish    (1000) monish    (1000)      333 2024-04-09 13:03:11.000000 InnovationLabHunt-1.1/setup.py
```

### Comparing `InnovationLabHunt-1.0/InnovationLabHunt/hunt.py` & `InnovationLabHunt-1.1/InnovationLabHunt/hunt.py`

 * *Files identical despite different names*

