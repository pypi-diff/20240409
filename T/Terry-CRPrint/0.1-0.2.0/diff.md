# Comparing `tmp/Terry-CRPrint-0.1.tar.gz` & `tmp/Terry-CRPrint-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Terry-CRPrint-0.1.tar", last modified: Tue Apr  9 03:10:31 2024, max compression
+gzip compressed data, was "Terry-CRPrint-0.2.0.tar", last modified: Tue Apr  9 03:12:51 2024, max compression
```

## Comparing `Terry-CRPrint-0.1.tar` & `Terry-CRPrint-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 03:10:31.486902 Terry-CRPrint-0.1/
--rw-rw-rw-   0        0        0       58 2024-04-09 03:10:31.486408 Terry-CRPrint-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2024-04-09 02:23:04.000000 Terry-CRPrint-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 03:10:31.482936 Terry-CRPrint-0.1/Terry_CRPrint.egg-info/
--rw-rw-rw-   0        0        0       58 2024-04-09 03:10:31.000000 Terry-CRPrint-0.1/Terry_CRPrint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-09 03:10:31.000000 Terry-CRPrint-0.1/Terry_CRPrint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 03:10:31.000000 Terry-CRPrint-0.1/Terry_CRPrint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 03:10:31.000000 Terry-CRPrint-0.1/Terry_CRPrint.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 03:10:31.485416 Terry-CRPrint-0.1/crprint/
--rw-rw-rw-   0        0        0       89 2024-04-09 02:22:59.000000 Terry-CRPrint-0.1/crprint/__init__.py
--rw-rw-rw-   0        0        0     5944 2024-04-09 02:22:00.000000 Terry-CRPrint-0.1/crprint/main.py
--rw-rw-rw-   0        0        0       42 2024-04-09 03:10:31.486902 Terry-CRPrint-0.1/setup.cfg
--rw-rw-rw-   0        0        0      224 2024-04-09 03:10:23.000000 Terry-CRPrint-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-09 03:12:51.051230 Terry-CRPrint-0.2.0/
+-rw-rw-rw-   0        0        0     1114 2024-04-09 03:12:51.050733 Terry-CRPrint-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2024-04-09 02:23:04.000000 Terry-CRPrint-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 03:12:51.046269 Terry-CRPrint-0.2.0/Terry_CRPrint.egg-info/
+-rw-rw-rw-   0        0        0     1114 2024-04-09 03:12:50.000000 Terry-CRPrint-0.2.0/Terry_CRPrint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-09 03:12:50.000000 Terry-CRPrint-0.2.0/Terry_CRPrint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 03:12:50.000000 Terry-CRPrint-0.2.0/Terry_CRPrint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-09 03:12:50.000000 Terry-CRPrint-0.2.0/Terry_CRPrint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 03:12:51.049246 Terry-CRPrint-0.2.0/crprint/
+-rw-rw-rw-   0        0        0       89 2024-04-09 02:22:59.000000 Terry-CRPrint-0.2.0/crprint/__init__.py
+-rw-rw-rw-   0        0        0     5944 2024-04-09 02:22:00.000000 Terry-CRPrint-0.2.0/crprint/main.py
+-rw-rw-rw-   0        0        0       42 2024-04-09 03:12:51.051725 Terry-CRPrint-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      313 2024-04-09 03:12:46.000000 Terry-CRPrint-0.2.0/setup.py
```

### Comparing `Terry-CRPrint-0.1/README.md` & `Terry-CRPrint-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `Terry-CRPrint-0.1/crprint/main.py` & `Terry-CRPrint-0.2.0/crprint/main.py`

 * *Files identical despite different names*

