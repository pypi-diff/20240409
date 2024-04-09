# Comparing `tmp/refvars-0.1.tar.gz` & `tmp/refvars-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refvars-0.1.tar", last modified: Thu Mar 14 11:41:21 2024, max compression
+gzip compressed data, was "refvars-0.2.tar", last modified: Tue Apr  9 05:58:05 2024, max compression
```

## Comparing `refvars-0.1.tar` & `refvars-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 11:41:21.489863 refvars-0.1/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 refvars-0.1/LICENCE
--rw-rw-rw-   0        0        0      138 2024-03-14 11:41:21.488782 refvars-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-03-14 11:15:25.000000 refvars-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 11:41:21.482343 refvars-0.1/refvars/
--rw-rw-rw-   0        0        0      502 2024-03-14 11:13:28.000000 refvars-0.1/refvars/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 11:41:21.487782 refvars-0.1/refvars.egg-info/
--rw-rw-rw-   0        0        0      138 2024-03-14 11:41:21.000000 refvars-0.1/refvars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-03-14 11:41:21.000000 refvars-0.1/refvars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 11:41:21.000000 refvars-0.1/refvars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 11:41:21.000000 refvars-0.1/refvars.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 11:41:21.489863 refvars-0.1/setup.cfg
--rw-rw-rw-   0        0        0      146 2024-03-14 11:40:57.000000 refvars-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:05.703948 refvars-0.2/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 refvars-0.2/LICENCE
+-rw-rw-rw-   0        0        0      783 2024-04-09 05:58:05.702928 refvars-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1480 2024-04-02 03:02:47.000000 refvars-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:05.698831 refvars-0.2/refvars/
+-rw-rw-rw-   0        0        0     3520 2024-04-02 02:58:50.000000 refvars-0.2/refvars/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:05.701905 refvars-0.2/refvars.egg-info/
+-rw-rw-rw-   0        0        0      783 2024-04-09 05:58:05.000000 refvars-0.2/refvars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-04-09 05:58:05.000000 refvars-0.2/refvars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:58:05.000000 refvars-0.2/refvars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:58:05.000000 refvars-0.2/refvars.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:58:05.703948 refvars-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2376 2024-04-09 05:58:03.000000 refvars-0.2/setup.py
```

### Comparing `refvars-0.1/LICENCE` & `refvars-0.2/LICENCE`

 * *Files identical despite different names*

