# Comparing `tmp/izihawa_pdftools-1.0.8.tar.gz` & `tmp/izihawa_pdftools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "izihawa_pdftools-1.0.8.tar", max compression
+gzip compressed data, was "izihawa_pdftools-1.0.9.tar", max compression
```

## Comparing `izihawa_pdftools-1.0.8.tar` & `izihawa_pdftools-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       21 2023-11-24 08:41:50.733970 izihawa_pdftools-1.0.8/README.md
--rw-r--r--   0        0        0       58 2023-12-10 19:54:02.096444 izihawa_pdftools-1.0.8/izihawa_pdftools/__init__.py
--rw-r--r--   0        0        0      211 2024-01-09 08:46:27.190127 izihawa_pdftools-1.0.8/izihawa_pdftools/cleaner-cli.py
--rw-r--r--   0        0        0     2021 2024-01-09 08:46:47.252618 izihawa_pdftools-1.0.8/izihawa_pdftools/cleaner.py
--rw-r--r--   0        0        0      343 2023-11-27 07:00:01.898852 izihawa_pdftools-1.0.8/izihawa_pdftools/exceptions.py
--rw-r--r--   0        0        0     1003 2023-12-10 19:54:02.159146 izihawa_pdftools-1.0.8/izihawa_pdftools/text_collector.py
--rw-r--r--   0        0        0    29695 2024-01-22 15:18:50.341949 izihawa_pdftools-1.0.8/izihawa_pdftools/watermarks.py
--rw-r--r--   0        0        0      463 2024-01-22 15:19:05.118084 izihawa_pdftools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 izihawa_pdftools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-11-24 08:41:50.733970 izihawa_pdftools-1.0.9/README.md
+-rw-r--r--   0        0        0       58 2023-12-10 19:54:02.096444 izihawa_pdftools-1.0.9/izihawa_pdftools/__init__.py
+-rw-r--r--   0        0        0      211 2024-01-09 08:46:27.190127 izihawa_pdftools-1.0.9/izihawa_pdftools/cleaner-cli.py
+-rw-r--r--   0        0        0     2021 2024-01-09 08:46:47.252618 izihawa_pdftools-1.0.9/izihawa_pdftools/cleaner.py
+-rw-r--r--   0        0        0      343 2023-11-27 07:00:01.898852 izihawa_pdftools-1.0.9/izihawa_pdftools/exceptions.py
+-rw-r--r--   0        0        0     1003 2023-12-10 19:54:02.159146 izihawa_pdftools-1.0.9/izihawa_pdftools/text_collector.py
+-rw-r--r--   0        0        0    29695 2024-01-22 15:18:50.341949 izihawa_pdftools-1.0.9/izihawa_pdftools/watermarks.py
+-rw-r--r--   0        0        0      462 2024-01-25 17:00:10.504688 izihawa_pdftools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 izihawa_pdftools-1.0.9/PKG-INFO
```

### Comparing `izihawa_pdftools-1.0.8/izihawa_pdftools/cleaner.py` & `izihawa_pdftools-1.0.9/izihawa_pdftools/cleaner.py`

 * *Files identical despite different names*

### Comparing `izihawa_pdftools-1.0.8/izihawa_pdftools/text_collector.py` & `izihawa_pdftools-1.0.9/izihawa_pdftools/text_collector.py`

 * *Files identical despite different names*

### Comparing `izihawa_pdftools-1.0.8/izihawa_pdftools/watermarks.py` & `izihawa_pdftools-1.0.9/izihawa_pdftools/watermarks.py`

 * *Files identical despite different names*

### Comparing `izihawa_pdftools-1.0.8/PKG-INFO` & `izihawa_pdftools-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: izihawa_pdftools
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cryptography (>=41.0.7,<42.0.0)
 Requires-Dist: ebooklib (>=0.18,<0.19)
 Requires-Dist: izihawa-utils (>=1.2.1,<2.0.0)
-Requires-Dist: pypdf (>=3.17.2,<4.0.0)
+Requires-Dist: pypdf (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # izihawa_textparser
```

