# Comparing `tmp/datatransformationsbertas-0.7.4.tar.gz` & `tmp/datatransformationsbertas-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatransformationsbertas-0.7.4.tar", max compression
+gzip compressed data, was "datatransformationsbertas-0.7.5.tar", max compression
```

## Comparing `datatransformationsbertas-0.7.4.tar` & `datatransformationsbertas-0.7.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.7.4/LICENSE
--rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.7.4/README.md
--rw-r--r--   0        0        0      341 2024-04-09 09:34:47.967896 datatransformationsbertas-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     2529 2024-04-09 09:33:26.422757 datatransformationsbertas-0.7.4/src/datatransformationsbertas/__init__.py
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1046 2024-04-02 10:05:27.898453 datatransformationsbertas-0.7.5/LICENSE
+-rw-r--r--   0        0        0     1315 2024-04-08 11:25:17.968534 datatransformationsbertas-0.7.5/README.md
+-rw-r--r--   0        0        0      341 2024-04-09 09:37:08.783543 datatransformationsbertas-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     2529 2024-04-09 09:36:39.205282 datatransformationsbertas-0.7.5/src/datatransformationsbertas/__init__.py
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 datatransformationsbertas-0.7.5/PKG-INFO
```

### Comparing `datatransformationsbertas-0.7.4/LICENSE` & `datatransformationsbertas-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.7.4/README.md` & `datatransformationsbertas-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.7.4/src/datatransformationsbertas/__init__.py` & `datatransformationsbertas-0.7.5/src/datatransformationsbertas/__init__.py`

 * *Files identical despite different names*

### Comparing `datatransformationsbertas-0.7.4/PKG-INFO` & `datatransformationsbertas-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataTransformationsBertas
-Version: 0.7.4
+Version: 0.7.5
 Summary: Tool to automate data scientist daily work
 License: MIT
 Author: Bertoldas
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```

