# Comparing `tmp/hst_funcs-0.0.1.tar.gz` & `tmp/hst_funcs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hst_funcs-0.0.1.tar", last modified: Fri Apr  5 07:31:57 2024, max compression
+gzip compressed data, was "hst_funcs-0.0.2.tar", last modified: Tue Apr  9 05:58:59 2024, max compression
```

## Comparing `hst_funcs-0.0.1.tar` & `hst_funcs-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 07:31:57.083799 hst_funcs-0.0.1/
--rw-rw-rw-   0        0        0      416 2024-04-05 07:31:57.081059 hst_funcs-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-04-05 07:30:25.000000 hst_funcs-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 07:31:57.052234 hst_funcs-0.0.1/hst_funcs/
--rw-rw-rw-   0        0        0        0 2023-09-11 08:09:44.000000 hst_funcs-0.0.1/hst_funcs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:31:57.076993 hst_funcs-0.0.1/hst_funcs/math/
--rw-rw-rw-   0        0        0     1428 2024-04-05 00:02:55.000000 hst_funcs-0.0.1/hst_funcs/math/calculus.py
-drwxrwxrwx   0        0        0        0 2024-04-05 07:31:57.080070 hst_funcs-0.0.1/hst_funcs.egg-info/
--rw-rw-rw-   0        0        0      416 2024-04-05 07:31:57.000000 hst_funcs-0.0.1/hst_funcs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-05 07:31:57.000000 hst_funcs-0.0.1/hst_funcs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 07:31:57.000000 hst_funcs-0.0.1/hst_funcs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 07:31:57.000000 hst_funcs-0.0.1/hst_funcs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      378 2024-04-05 07:30:28.000000 hst_funcs-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 07:31:57.083799 hst_funcs-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.177948 hst_funcs-0.0.2/
+-rw-rw-rw-   0        0        0      416 2024-04-09 05:58:59.176950 hst_funcs-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2024-04-05 07:30:25.000000 hst_funcs-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.157595 hst_funcs-0.0.2/hst_funcs/
+-rw-rw-rw-   0        0        0        0 2023-09-11 08:09:44.000000 hst_funcs-0.0.2/hst_funcs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.141638 hst_funcs-0.0.2/hst_funcs/finanace/
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.170942 hst_funcs-0.0.2/hst_funcs/finanace/Equity/
+-rw-rw-rw-   0        0        0     2506 2024-04-09 05:58:23.000000 hst_funcs-0.0.2/hst_funcs/finanace/Equity/KIBarrier.py
+-rw-rw-rw-   0        0        0     1737 2024-04-09 05:43:06.000000 hst_funcs-0.0.2/hst_funcs/finanace/Equity/vanilla.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.172948 hst_funcs-0.0.2/hst_funcs/math/
+-rw-rw-rw-   0        0        0     1428 2024-04-05 00:02:55.000000 hst_funcs-0.0.2/hst_funcs/math/calculus.py
+drwxrwxrwx   0        0        0        0 2024-04-09 05:58:59.174949 hst_funcs-0.0.2/hst_funcs.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-04-09 05:58:59.000000 hst_funcs-0.0.2/hst_funcs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-09 05:58:59.000000 hst_funcs-0.0.2/hst_funcs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 05:58:59.000000 hst_funcs-0.0.2/hst_funcs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-09 05:58:59.000000 hst_funcs-0.0.2/hst_funcs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      378 2024-04-09 05:58:18.000000 hst_funcs-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 05:58:59.177948 hst_funcs-0.0.2/setup.cfg
```

### Comparing `hst_funcs-0.0.1/hst_funcs/math/calculus.py` & `hst_funcs-0.0.2/hst_funcs/math/calculus.py`

 * *Files identical despite different names*

