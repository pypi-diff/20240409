# Comparing `tmp/ArtisanPrint-0.0.3.tar.gz` & `tmp/ArtisanPrint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArtisanPrint-0.0.3.tar", last modified: Wed Nov  1 14:14:38 2023, max compression
+gzip compressed data, was "ArtisanPrint-1.0.0.tar", last modified: Tue Apr  9 18:52:13 2024, max compression
```

## Comparing `ArtisanPrint-0.0.3.tar` & `ArtisanPrint-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-01 14:14:38.911620 ArtisanPrint-0.0.3/
--rw-rw-rw-   0        0        0     1086 2023-11-01 11:38:34.000000 ArtisanPrint-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      785 2023-11-01 14:14:38.911620 ArtisanPrint-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-11-01 12:29:50.000000 ArtisanPrint-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-11-01 11:30:01.000000 ArtisanPrint-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      648 2023-11-01 14:14:38.920920 ArtisanPrint-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-01 14:14:38.871483 ArtisanPrint-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-11-01 14:14:38.879617 ArtisanPrint-0.0.3/src/ArtisanPrint/
--rw-rw-rw-   0        0        0     8648 2023-11-01 14:11:54.000000 ArtisanPrint-0.0.3/src/ArtisanPrint/ColorPrint.py
--rw-rw-rw-   0        0        0       44 2023-11-01 13:30:59.000000 ArtisanPrint-0.0.3/src/ArtisanPrint/__init__.py
--rw-rw-rw-   0        0        0      148 2023-11-01 08:22:57.000000 ArtisanPrint-0.0.3/src/ArtisanPrint/custom_exceptions.py
-drwxrwxrwx   0        0        0        0 2023-11-01 14:14:38.911620 ArtisanPrint-0.0.3/src/ArtisanPrint.egg-info/
--rw-rw-rw-   0        0        0      785 2023-11-01 14:14:38.000000 ArtisanPrint-0.0.3/src/ArtisanPrint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-11-01 14:14:38.000000 ArtisanPrint-0.0.3/src/ArtisanPrint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-01 14:14:38.000000 ArtisanPrint-0.0.3/src/ArtisanPrint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-11-01 14:14:38.000000 ArtisanPrint-0.0.3/src/ArtisanPrint.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 18:52:13.558896 ArtisanPrint-1.0.0/
+drwxrwxrwx   0        0        0        0 2024-04-09 18:52:13.548722 ArtisanPrint-1.0.0/ArtisanPrint/
+-rw-rw-rw-   0        0        0     8648 2023-11-01 14:11:54.000000 ArtisanPrint-1.0.0/ArtisanPrint/ColorPrint.py
+-rw-rw-rw-   0        0        0       44 2023-11-01 13:30:59.000000 ArtisanPrint-1.0.0/ArtisanPrint/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-11-01 08:22:57.000000 ArtisanPrint-1.0.0/ArtisanPrint/custom_exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-09 18:52:13.558896 ArtisanPrint-1.0.0/ArtisanPrint.egg-info/
+-rw-rw-rw-   0        0        0     2477 2024-04-09 18:52:13.000000 ArtisanPrint-1.0.0/ArtisanPrint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-09 18:52:13.000000 ArtisanPrint-1.0.0/ArtisanPrint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 18:52:13.000000 ArtisanPrint-1.0.0/ArtisanPrint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-09 18:52:13.000000 ArtisanPrint-1.0.0/ArtisanPrint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-11-01 11:38:34.000000 ArtisanPrint-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2477 2024-04-09 18:52:13.558896 ArtisanPrint-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-04-09 18:29:06.000000 ArtisanPrint-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-09 18:52:13.558896 ArtisanPrint-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-04-09 18:15:25.000000 ArtisanPrint-1.0.0/setup.py
```

### Comparing `ArtisanPrint-0.0.3/LICENSE` & `ArtisanPrint-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ArtisanPrint-0.0.3/src/ArtisanPrint/ColorPrint.py` & `ArtisanPrint-1.0.0/ArtisanPrint/ColorPrint.py`

 * *Files identical despite different names*

