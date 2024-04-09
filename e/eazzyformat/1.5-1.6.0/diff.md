# Comparing `tmp/eazzyformat-1.5.tar.gz` & `tmp/eazzyformat-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eazzyformat-1.5.tar", last modified: Sun Nov 21 09:25:42 2021, max compression
+gzip compressed data, was "eazzyformat-1.6.0.tar", max compression
```

## Comparing `eazzyformat-1.5.tar` & `eazzyformat-1.6.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxrwxrwx   0        0        0        0 2021-11-21 09:25:42.820314 eazzyformat-1.5/
--rw-rw-rw-   0        0        0      344 2021-11-21 09:25:42.821314 eazzyformat-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-11-21 09:25:42.820314 eazzyformat-1.5/eazzyformat/
--rw-rw-rw-   0        0        0      445 2021-08-27 14:58:36.300535 eazzyformat-1.5/eazzyformat/__init__.py
--rw-rw-rw-   0        0        0     3727 2021-11-21 09:22:43.394245 eazzyformat-1.5/eazzyformat/parser.py
--rw-rw-rw-   0        0        0     1848 2021-08-27 11:31:07.198332 eazzyformat-1.5/eazzyformat/string_iterators.py
--rw-rw-rw-   0        0        0      404 2021-11-21 09:25:36.687430 eazzyformat-1.5/setup.py
+-rw-r--r--   0        0        0    35149 2024-04-09 10:12:39.935548 eazzyformat-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      784 2024-04-09 10:12:39.935548 eazzyformat-1.6.0/README.md
+-rw-r--r--   0        0        0      445 2024-04-09 10:12:39.935548 eazzyformat-1.6.0/eazzyformat/__init__.py
+-rw-r--r--   0        0        0     3727 2024-04-09 10:12:39.935548 eazzyformat-1.6.0/eazzyformat/parser.py
+-rw-r--r--   0        0        0     1850 2024-04-09 10:14:03.083088 eazzyformat-1.6.0/eazzyformat/string_iterators.py
+-rw-r--r--   0        0        0      272 2024-04-09 10:17:08.370064 eazzyformat-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1177 1970-01-01 00:00:00.000000 eazzyformat-1.6.0/PKG-INFO
```

### Comparing `eazzyformat-1.5/eazzyformat/parser.py` & `eazzyformat-1.6.0/eazzyformat/parser.py`

 * *Files identical despite different names*

### Comparing `eazzyformat-1.5/eazzyformat/string_iterators.py` & `eazzyformat-1.6.0/eazzyformat/string_iterators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from collections import Iterator
 from typing import Container
 
 
-class StringIteratorWithIndex(Iterator):
+class StringIteratorWithIndex:
+
+    def __iter__(self):
+        return self
 
     def __init__(self, string: str, index=0):
         self.string = string
         self.index = index
 
     def __next__(self):
         try:
```

