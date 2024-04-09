# Comparing `tmp/sweecrypt-1.0.tar.gz` & `tmp/sweecrypt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweecrypt-1.0.tar", last modified: Thu Apr  4 23:32:45 2024, max compression
+gzip compressed data, was "sweecrypt-1.0.1.tar", last modified: Tue Apr  9 00:02:17 2024, max compression
```

## Comparing `sweecrypt-1.0.tar` & `sweecrypt-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:32:45.261178 sweecrypt-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 23:32:39.000000 sweecrypt-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 23:32:45.261178 sweecrypt-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-04 23:32:39.000000 sweecrypt-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:32:45.261178 sweecrypt-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-04 23:32:39.000000 sweecrypt-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:32:45.257177 sweecrypt-1.0/sweecrypt/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:32:39.000000 sweecrypt-1.0/sweecrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-04 23:32:39.000000 sweecrypt-1.0/sweecrypt/sweecrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:32:45.261178 sweecrypt-1.0/sweecrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 23:32:45.000000 sweecrypt-1.0/sweecrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-04 23:32:45.000000 sweecrypt-1.0/sweecrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:32:45.000000 sweecrypt-1.0/sweecrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 23:32:45.000000 sweecrypt-1.0/sweecrypt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:02:17.192373 sweecrypt-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-09 00:02:03.000000 sweecrypt-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 00:02:17.192373 sweecrypt-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-09 00:02:03.000000 sweecrypt-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:02:17.192373 sweecrypt-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 00:02:03.000000 sweecrypt-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:02:17.192373 sweecrypt-1.0.1/sweecrypt/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 00:02:03.000000 sweecrypt-1.0.1/sweecrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 00:02:03.000000 sweecrypt-1.0.1/sweecrypt/sweecryptt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:02:17.192373 sweecrypt-1.0.1/sweecrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 00:02:17.000000 sweecrypt-1.0.1/sweecrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 00:02:17.000000 sweecrypt-1.0.1/sweecrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:02:17.000000 sweecrypt-1.0.1/sweecrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 00:02:17.000000 sweecrypt-1.0.1/sweecrypt.egg-info/top_level.txt
```

### Comparing `sweecrypt-1.0/LICENSE` & `sweecrypt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweecrypt-1.0/sweecrypt/sweecrypt.py` & `sweecrypt-1.0.1/sweecrypt/sweecryptt.py`

 * *Files identical despite different names*

