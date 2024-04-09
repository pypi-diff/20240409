# Comparing `tmp/segmentation_skeleton_metrics-4.0.1.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.0.1.tar", last modified: Tue Mar 26 22:08:21 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.0.tar", last modified: Tue Apr  9 02:12:09 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.0.1.tar` & `segmentation_skeleton_metrics-4.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.586038 segmentation_skeleton_metrics-4.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.590038 segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.590038 segmentation_skeleton_metrics-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.590038 segmentation_skeleton_metrics-4.0.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.590038 segmentation_skeleton_metrics-4.0.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.590038 segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.602038 segmentation_skeleton_metrics-4.0.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.614039 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.586038 segmentation_skeleton_metrics-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-03-26 22:08:21.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-26 22:08:21.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 22:08:21.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 22:08:21.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 22:08:21.000000 segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 22:08:21.618039 segmentation_skeleton_metrics-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 22:08:06.000000 segmentation_skeleton_metrics-4.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.753924 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.765924 segmentation_skeleton_metrics-4.1.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.749925 segmentation_skeleton_metrics-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.781924 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 02:12:09.000000 segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 02:12:09.777924 segmentation_skeleton_metrics-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 02:11:55.000000 segmentation_skeleton_metrics-4.1.0/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.0/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/.gitignore` & `segmentation_skeleton_metrics-4.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/LICENSE` & `segmentation_skeleton_metrics-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/PKG-INFO` & `segmentation_skeleton_metrics-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.0.1
+Version: 4.1.0
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.0.1/README.md` & `segmentation_skeleton_metrics-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/pyproject.toml` & `segmentation_skeleton_metrics-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.0/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.0/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.0/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,7 +229,25 @@
     -------
     int
         Leaf node of "graph"
 
     """
     leafs = [i for i in graph.nodes if graph.degree[i] == 1]
     return sample(leafs, 1)[0]
+
+
+def sample_node(graph):
+    """
+    Samples a node from "graph".
+
+    Parameters
+    ----------
+    graph : networkx.Graph
+        Graph to be sampled from.
+
+    Returns
+    -------
+    int
+        Node.
+
+    """
+    return sample(list(graph.nodes), 1)[0]
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 import tensorstore as ts
 from scipy.spatial import KDTree
 
 from segmentation_skeleton_metrics import graph_utils as gutils
 from segmentation_skeleton_metrics import split_detection, swc_utils, utils
 from segmentation_skeleton_metrics.swc_utils import save, to_graph
 
-INTERSECTION_THRESHOLD = 10
-MERGE_DIST_THRESHOLD = 40
+CLOSE_DIST_THRESHOLD = 5
+INTERSECTION_THRESHOLD = 16
+MERGE_DIST_THRESHOLD = 30
 
 
 class SkeletonMetric:
     """
     Class that evaluates the quality of a predicted segmentation by comparing
     the ground truth skeletons to the predicted segmentation mask. The
     accuracy is then quantified by detecting splits and merges, then computing
@@ -43,15 +44,15 @@
         self,
         pred_labels,
         pred_swc_paths,
         target_swc_paths,
         anisotropy=[1.0, 1.0, 1.0],
         black_holes_xyz_id=None,
         black_hole_radius=24,
-        equivalent_ids=None,
+        connections_path=None,
         ignore_boundary_mistakes=False,
         output_dir=None,
         valid_size_threshold=25,
         save_swc=False,
     ):
         """
         Constructs skeleton metric object that evaluates the quality of a
@@ -71,16 +72,17 @@
             If swc files are on local machine, list of paths to swc files where
             each file corresponds to a neuron in the prediction. If swc files
             are on cloud, then dict with keys "bucket_name" and "path".
         black_holes_xyz_id : list, optional
             ...
         black_hole_radius : float, optional
             ...
-        equivalent_ids : ...
-            ...
+        connections_path : list[tuple]
+            Path to a txt file containing pairs of swc ids from the prediction
+            that were predicted to be connected.
         ignore_boundary_mistakes : bool, optional
             Indication of whether to ignore mistakes near boundary of bounding
             box. The default is False.
         output_dir : str, optional
             Path to directory that each mistake site is written to. The default
             is None.
         valid_size_threshold : int, optional
@@ -101,29 +103,43 @@
         self.ignore_boundary_mistakes = ignore_boundary_mistakes
         self.output_dir = output_dir
         self.save = save_swc
 
         self.init_black_holes(black_holes_xyz_id)
         self.black_hole_radius = black_hole_radius
 
-        # Build Graphs
+        # Labels
         self.label_mask = pred_labels
         self.valid_labels = swc_utils.parse(
-            pred_swc_paths, valid_size_threshold, anisotropy=anisotropy
+            pred_swc_paths, valid_size_threshold, anisotropy
         )
+        self.init_equiv_labels(connections_path)
 
+        # Build Graphs
         self.target_graphs = self.init_graphs(target_swc_paths, anisotropy)
-        self.labeled_target_graphs = self.init_labeled_target_graphs()
+        self.init_labeled_target_graphs()
 
         # Build kdtree
         self.init_xyz_to_id_node()
         self.init_kdtree()
-        self.rm_spurious_intersections()
 
     # -- Initialize and Label Graphs --
+    def init_equiv_labels(self, path):
+        if path:
+            self.equiv_labels_map = utils.equiv_class_mappings(
+                path, self.valid_labels
+            )
+            valid_labels = dict()
+            for label, values in self.valid_labels.items():
+                equiv_label = self.equiv_labels_map[label]
+                valid_labels[equiv_label] = values
+            self.valid_labels = valid_labels
+        else:
+            self.equiv_labels_map = None
+
     def init_graphs(self, paths, anisotropy):
         """
         Initializes "self.target_graphs" by iterating over "paths" which
         correspond to neurons in the ground truth.
 
         Parameters
         ----------
@@ -158,25 +174,24 @@
         Returns
         -------
         None
 
         """
         print("Labelling Target Graphs...")
         t0 = time()
-        labeled_target_graphs = dict()
+        self.labeled_target_graphs = dict()
         self.id_to_label_nodes = dict()  # {target_id: {label: nodes}}
         for cnt, (target_id, graph) in enumerate(self.target_graphs.items()):
             utils.progress_bar(cnt + 1, len(self.target_graphs))
             labeled_target_graph, id_to_label_nodes = self.label_graph(graph)
-            labeled_target_graphs[target_id] = labeled_target_graph
+            self.labeled_target_graphs[target_id] = labeled_target_graph
             self.id_to_label_nodes[target_id] = id_to_label_nodes
 
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
-        return labeled_target_graphs
 
     def label_graph(self, target_graph):
         """
         Iterates over nodes in "target_graph" and stores the label in the
         predicted segmentation mask (i.e. "self.label_mask") which coincides
         with each node as a node-level attribute called "label".
 
@@ -225,43 +240,56 @@
            Label of voxel at "img_coord".
 
         """
         # Read label
         if self.in_black_hole(img_coord):
             label = -1
         else:
-            label = self.__read_label(img_coord)
+            label = self.read_label(img_coord)
 
-        # Validate label
+        # Adjust label
+        label = self.equivalent_label(label)
+        label = self.validate(label)
         if return_node:
-            return return_node, self.is_valid(label)
+            return return_node, label
         else:
-            return self.is_valid(label)
+            return label
 
-    def __read_label(self, coord):
+    def read_label(self, coord):
         """
         Gets label at image coordinates "xyz".
 
         Parameters
         ----------
         coord : tuple[int]
             Coordinates that indexes into "self.label_mask".
 
         Returns
         -------
         int
            Label at image coordinates "xyz".
 
         """
+        # Read image label
         if type(self.label_mask) == ts.TensorStore:
             return int(self.label_mask[coord].read().result())
         else:
             return self.label_mask[coord]
 
-    def is_valid(self, label):
+    def equivalent_label(self, label):
+        # Equivalent label
+        if self.equiv_labels_map:
+            if label in self.equiv_labels_map.keys():
+                return self.equiv_labels_map[label]
+            else:
+                return 0
+        else:
+            return label
+
+    def validate(self, label):
         """
         Validates label by checking whether it is contained in
         "self.valid_labels".
 
         Parameters
         ----------
         label : int
@@ -286,43 +314,14 @@
             for i in graph.nodes:
                 xyz = tuple(graph.nodes[i]["xyz"])
                 if xyz in self.xyz_to_id_node.keys():
                     self.xyz_to_id_node[xyz][target_id] = i
                 else:
                     self.xyz_to_id_node[xyz] = {target_id: i}
 
-    def rm_spurious_intersections(self):
-        for label in [label for label in self.get_all_labels() if label > 0]:
-            # Compute label intersect target_graphs
-            hit_target_ids = dict()
-            multi_hits = set()
-            for xyz in self.get_pred_coords(label):
-                hat_xyz, d = self.get_projection(xyz)
-                if d < 5:
-                    hits = list(self.xyz_to_id_node[hat_xyz].keys())
-                    if len(hits) > 1:
-                        multi_hits.add(hat_xyz)
-                    else:
-                        hat_i = self.xyz_to_id_node[hat_xyz][hits[0]]
-                        hit_target_ids = utils.append_dict_value(
-                            hit_target_ids, hits[0], hat_i
-                        )
-            hit_target_ids = utils.resolve(
-                multi_hits, hit_target_ids, self.xyz_to_id_node
-            )
-
-            # Remove spurious intersections
-            for target_id in self.target_graphs.keys():
-                if target_id in hit_target_ids.keys():
-                    n_hits = len(hit_target_ids[target_id])
-                    if n_hits < INTERSECTION_THRESHOLD:
-                        self.zero_nodes(target_id, label)
-                elif label in self.id_to_label_nodes[target_id]:
-                    self.zero_nodes(target_id, label)
-
     def get_pred_coords(self, label):
         if label in self.valid_labels.keys():
             return self.valid_labels[label]
         else:
             return []
 
     # -- Final Constructor Routines --
@@ -343,22 +342,21 @@
             black_holes_id = [bh_dict["swc_id"] for bh_dict in black_holes]
             self.black_holes = KDTree(black_holes_xyz)
             self.black_hole_labels = set(black_holes_id)
         else:
             self.black_holes = None
             self.black_hole_labels = set()
 
-    def in_black_hole(self, xyz, print_nn=False):
-        # Check whether black_holes exists
-        if self.black_holes is None:
-            return False
-        else:
+    def in_black_hole(self, xyz):
+        if self.black_holes:
             radius = self.black_hole_radius
             pts = self.black_holes.query_ball_point(xyz, radius)
             return True if len(pts) > 0 else False
+        else:
+            return False
 
     # -- Evaluation --
     def compute_metrics(self):
         """
         Computes skeleton-based metrics.
 
         Parameters
@@ -483,18 +481,19 @@
         None
 
         Returns
         -------
         None
 
         """
-        # Initilize counts
+        # Initilizations
         self.merge_cnts = self.init_counter()
         self.merged_cnts = self.init_counter()
         self.merged_percents = self.init_counter()
+        # self.rm_spurious_intersections()
 
         # Run detection
         t0 = time()
         detected_merges = set()
         for cnt, target_id_1 in enumerate(self.labeled_target_graphs.keys()):
             utils.progress_bar(cnt + 1, len(self.target_graphs))
             for target_id_2 in self.labeled_target_graphs.keys():
@@ -508,15 +507,17 @@
                 intersection = labels_1.intersection(labels_2)
                 for label in intersection:
                     # Process merge
                     merge = (frozenset((target_id_1, target_id_2)), label)
                     if merge not in detected_merges:
                         detected_merges.add(merge)
                         if self.save:
-                            site, d = self.locate(target_id_1, target_id_2, label)
+                            site, d = self.localize_site(
+                                target_id_1, target_id_2, label
+                            )
                             if d < MERGE_DIST_THRESHOLD:
                                 self.save_swc(site[0], site[1], "merge")
 
         # Update graph
         for (target_ids, label) in detected_merges:
             target_id_1, target_id_2 = tuple(target_ids)
             self.process_merge(target_id_1, label)
@@ -524,15 +525,44 @@
             self.merge_cnts[target_id_1] += 1
             self.merge_cnts[target_id_2] += 1
 
         # Report Runtime
         t, unit = utils.time_writer(time() - t0)
         print(f"\nRuntime: {round(t, 2)} {unit}\n")
 
-    def locate(self, target_id_1, target_id_2, label):
+    def rm_spurious_intersections(self):
+        for label in [label for label in self.get_all_labels() if label > 0]:
+            # Compute label intersect target_graphs
+            hit_target_ids = dict()
+            multi_hits = set()
+            for xyz in self.self.get_pred_coords(label):
+                hat_xyz, d = self.get_projection(xyz)
+                if d < CLOSE_DIST_THRESHOLD:
+                    hits = list(self.xyz_to_id_node[hat_xyz].keys())
+                    if len(hits) > 1:
+                        multi_hits.add(hat_xyz)
+                    else:
+                        hat_i = self.xyz_to_id_node[hat_xyz][hits[0]]
+                        hit_target_ids = utils.append_dict_value(
+                            hit_target_ids, hits[0], hat_i
+                        )
+            hit_target_ids = utils.resolve(
+                multi_hits, hit_target_ids, self.xyz_to_id_node
+            )
+
+            # Remove spurious intersections
+            for target_id in self.target_graphs.keys():
+                if target_id in hit_target_ids.keys():
+                    n_hits = len(hit_target_ids[target_id])
+                    if n_hits < INTERSECTION_THRESHOLD:
+                        self.zero_nodes(target_id, label)
+                elif label in self.id_to_label_nodes[target_id]:
+                    self.zero_nodes(target_id, label)
+
+    def localize_site(self, target_id_1, target_id_2, label):
         # Get merged nodes
         merged_1 = self.id_to_label_nodes[target_id_1][label]
         merged_2 = self.id_to_label_nodes[target_id_2][label]
 
         # Find closest pair
         min_dist = np.inf
         xyz_pair = [None, None]
@@ -544,14 +574,28 @@
                     min_dist = utils.dist(xyz_1, xyz_2)
                     xyz_pair = [xyz_1, xyz_2]
                     if min_dist < MERGE_DIST_THRESHOLD:
                         return xyz_pair, min_dist
         return xyz_pair, min_dist
 
     def near_bdd(self, xyz):
+        """
+        Determines whether "xyz" is near the boundary of the image.
+
+        Parameters
+        ----------
+        xyz : numpy.ndarray
+            xyz coordinate to be checked
+
+        Returns
+        -------
+        near_bdd_bool : bool
+            Indication of whether "xyz" is near the boundary of the image.
+
+        """
         near_bdd_bool = False
         if self.ignore_boundary_mistakes:
             mask_shape = self.label_mask.shape
             above = [xyz[i] >= mask_shape[i] - 32 for i in range(3)]
             below = [xyz[i] < 32 for i in range(3)]
             near_bdd_bool = True if any(above) or any(below) else False
         return near_bdd_bool
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,31 @@
 import networkx as nx
 
 from segmentation_skeleton_metrics import graph_utils as gutils
 from segmentation_skeleton_metrics import utils
 
 
 def run(target_graph, labeled_graph):
+    """
+    Detected splits in a predicted segmentation.
+
+    Parameters
+    ----------
+    target_graph : networkx.Graph
+        Graph built from a ground truth swc file.
+    labeled_graph : networkx.Graph
+        Labeled graph built from a ground truth swc file, where each node has
+        an attribute called 'label'.
+
+    Returns
+    -------
+    labeled_graph : networkx.Graph
+        Labeled graph with omit and split edges removed.
+
+    """
     r = gutils.sample_leaf(target_graph)
     dfs_edges = list(nx.dfs_edges(target_graph, source=r))
     while len(dfs_edges) > 0:
         # Visit edge
         (i, j) = dfs_edges.pop(0)
         label_i = labeled_graph.nodes[i]["label"]
         label_j = labeled_graph.nodes[j]["label"]
@@ -39,17 +56,18 @@
     Determines whether zero-valued labels correspond to a split or
     misalignment between "target_graph" and the predicted segmentation
     mask.
 
     Parameters
     ----------
     target_graph : networkx.Graph
-        ...
+        Graph built from a ground truth swc file.
     labeled_graph : networkx.Graph
-        ...
+        Labeled graph built from a ground truth swc file, where each node has
+        an attribute called 'label'.
     dfs_edges : list[tuple]
         List of edges to be processed for split detection.
     nb : int
         Neighbor of "root".
     root : int
         Node where possible split starts (i.e. zero-valued label).
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import networkx as nx
 import numpy as np
 from google.cloud import storage
 
 from segmentation_skeleton_metrics import utils
 
 
-def parse(swc_paths, min_size, anisotropy=[1.0, 1.0, 1.0]):
+def parse(swc_paths, min_size, anisotropy):
     """
     Reads swc files and extracts the xyz coordinates.
 
     Paramters
     ---------
     swc_paths : list or dict
         If swc files are on local machine, list of paths to swc files where
@@ -34,35 +34,81 @@
     anisotropy : list[float]
         Image to World scaling factors applied to xyz coordinates to account
         for anisotropy of the microscope.
 
     Returns
     -------
     dict
-        ...
+        Dictionary where each item is an swc_id and an array of the xyz
+        coordinates read from cooresponding swc file.
+
     """
     if type(swc_paths) == list:
         return parse_local_paths(swc_paths, min_size, anisotropy)
     elif type(swc_paths) == dict:
         return parse_cloud_paths(swc_paths, min_size, anisotropy)
     else:
         return None
 
 
-def parse_local_paths(pred_swc_paths, min_size, anisotropy):
+def parse_local_paths(swc_paths, min_size, anisotropy):
+    """
+    Reads swc files from local machine and extracts the xyz coordinates.
+
+    Paramters
+    ---------
+    swc_paths : list or dict
+        If swc files are on local machine, list of paths to swc files where
+        each file corresponds to a neuron in the prediction. If swc files are
+        on cloud, then dict with keys "bucket_name" and "path".
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
+    anisotropy : list[float]
+        Image to World scaling factors applied to xyz coordinates to account
+        for anisotropy of the microscope.
+
+    Returns
+    -------
+    valid_labels : dict
+        Dictionary where each item is an swc_id and an array of the xyz
+        coordinates read from cooresponding swc file.
+
+    """
     valid_labels = dict()
-    for path in pred_swc_paths:
+    for path in swc_paths:
         contents = read_from_local(path)
         if len(contents) > min_size:
             swc_id = int(utils.get_swc_id(path))
             valid_labels[swc_id] = get_coords(contents, anisotropy)
     return valid_labels
 
 
 def parse_cloud_paths(cloud_dict, min_size, anisotropy):
+    """
+    Reads swc files from a GCS bucket and extracts the xyz coordinates.
+
+    Parameters
+    ----------
+    cloud_dict : dict
+        Dictionary where keys are "bucket_name" and "path".
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
+    anisotropy : list[float]
+        Image to World scaling factors applied to xyz coordinates to account
+        for anisotropy of the microscope.
+
+    Returns
+    -------
+    valid_labels : dict
+        Dictionary where each item is an swc_id and an array of the xyz
+        coordinates read from cooresponding swc file.
+
+    """
     # Initializations
     bucket = storage.Client().bucket(cloud_dict["bucket_name"])
     zip_paths = utils.list_gcs_filenames(bucket, cloud_dict["path"], ".zip")
     chunk_size = int(len(zip_paths) * 0.02)
 
     # Parse
     cnt = 1
@@ -78,14 +124,38 @@
     # Report Results
     print("\n#Valid Labels:", len(valid_labels))
     print("")
     return valid_labels
 
 
 def download(bucket, zip_path, min_size, anisotropy):
+    """
+    Downloads the contents from each swc file contained in the zip file at
+    "zip_path".
+
+    Parameters
+    ----------
+    bucket : str
+        Name of GCS bucket containing swc files to be read.
+    zip_path : str
+        Path to zip file contained in GCS bucket.
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
+    anisotropy : list[float]
+        Image to World scaling factors applied to xyz coordinates to account
+        for anisotropy of the microscope.
+
+    Returns
+    -------
+    valid_labels : dict
+        Dictionary where each item is an swc_id and an array of the xyz
+        coordinates read from cooresponding swc file.
+
+    """
     zip_content = bucket.blob(zip_path).download_as_bytes()
     with ZipFile(BytesIO(zip_content)) as zip_file:
         with ThreadPoolExecutor() as executor:
             # Assign threads
             threads = []
             for path in utils.list_files_in_gcs_zip(zip_content):
                 threads.append(
@@ -98,29 +168,51 @@
             valid_labels = dict()
             for thread in as_completed(threads):
                 valid_labels.update(thread.result())
     return valid_labels
 
 
 def parse_gcs_zip(zip_file, path, min_size, anisotropy):
+    """
+    Reads swc file stored at "path" which points to a file in a GCS bucket.
+
+    Parameters
+    ----------
+    zip_file : ZipFile
+        Zip file containing swc file to be read.
+    path : str
+        Path to swc file to be read.
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
+    anisotropy : list[float]
+        Image to World scaling factors applied to xyz coordinates to account
+        for anisotropy of the microscope.
+
+    Returns
+    -------
+    list
+        List such that each entry is a line from the swc file.
+
+    """
     contents = read_from_cloud(zip_file, path)
     if len(contents) > min_size:
         swc_id = int(utils.get_swc_id(path))
         return {swc_id: get_coords(contents, anisotropy)}
     else:
         return dict()
 
 
 def read_from_local(path):
     """
     Reads swc file stored at "path" on local machine.
 
     Parameters
     ----------
-    Path : str
+    path : str
         Path to swc file to be read.
 
     Returns
     -------
     list
         List such that each entry is a line from the swc file.
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 import os
 from io import BytesIO
 from time import time
 from zipfile import ZipFile
 
+import networkx as nx
 import numpy as np
 import tensorstore as ts
 from scipy.spatial import distance
 
 SUPPORTED_DRIVERS = ["neuroglancer_precomputed", "n5", "zarr"]
 
 
@@ -139,14 +140,33 @@
     Reads the content of an swc file from a zip file in a GCS bucket.
 
     """
     with zip_file.open(path) as text_file:
         return text_file.read().decode("utf-8").splitlines()
 
 
+def read_txt(path):
+    """
+    Reads txt file stored at "path".
+
+    Parameters
+    ----------
+    path : str
+        Path where txt file is stored.
+
+    Returns
+    -------
+    str
+        Contents of txt file.
+
+    """
+    with open(path, "r") as f:
+        return f.readlines()
+
+
 def list_gcs_filenames(bucket, cloud_path, extension):
     """
     Lists all files in a GCS bucket with the given extension.
 
     """
     blobs = bucket.list_blobs(prefix=cloud_path)
     return [blob.name for blob in blobs if extension in blob.name]
@@ -303,19 +323,49 @@
     return best_key
 
 
 def get_swc_id(path):
     """
     Gets segment id of the swc file at "path".
 
+    Parameters
+    ----------
+    path : str
+        Path to an swc file
+
+    Return
+    ------
+    Segment id of swc file.
+
     """
     filename = path.split("/")[-1]
     return filename.split(".")[0]
 
 
+def equiv_class_mappings(connections_path, labels):
+    label_to_class = {0: 0}
+    labels_graph = build_labels_graph(connections_path, labels)
+    for i, component in enumerate(nx.connected_components(labels_graph)):
+        i += 1
+        for label in component:
+            label_to_class[label] = i
+    return label_to_class
+
+
+def build_labels_graph(connections_path, labels):
+    labels_graph = nx.Graph()
+    labels_graph.add_nodes_from(list(labels.keys()))
+    for line in read_txt(connections_path):
+        ids = line.split(",")
+        id_1 = int(ids[0])
+        id_2 = int(ids[1])
+        labels_graph.add_edge(id_1, id_2)
+    return labels_graph
+
+
 # -- runtime --
 def time_writer(t, unit="seconds"):
     """
     Converts runtime "t" to its proper unit.
 
     Parameters
     ----------
@@ -340,14 +390,29 @@
         t /= 60
         unit = upd_unit[unit]
         t, unit = time_writer(t, unit=unit)
     return t, unit
 
 
 def init_timers():
+    """
+    Initializes two timers.
+
+    Parameters
+    ----------
+    None
+
+    Returns
+    -------
+    time.time
+        Timer.
+    time.time
+        Timer.
+
+    """
     return time(), time()
 
 
 def progress_bar(current, total, bar_length=50):
     """
     Reports the progress of completing some process.
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.0.1
+Version: 4.1.0
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.0.1/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.0/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

