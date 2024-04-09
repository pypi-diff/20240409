# Comparing `tmp/immunopipe-1.3.4.post1.tar.gz` & `tmp/immunopipe-1.3.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immunopipe-1.3.4.post1.tar", max compression
+gzip compressed data, was "immunopipe-1.3.4.post2.tar", max compression
```

## Comparing `immunopipe-1.3.4.post1.tar` & `immunopipe-1.3.4.post2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35128 2024-04-08 23:53:51.638916 immunopipe-1.3.4.post1/LICENSE
--rw-r--r--   0        0        0     1448 2024-04-08 23:53:51.638916 immunopipe-1.3.4.post1/README.md
--rw-r--r--   0        0        0      143 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/__init__.py
--rw-r--r--   0        0        0      109 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/__main__.py
--rw-r--r--   0        0        0     7461 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/inhouse.py
--rw-r--r--   0        0        0      503 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/pipeline.py
--rw-r--r--   0        0        0    33594 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/processes.py
--rw-r--r--   0        0        0     1581 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/CloneHeterogeneity.svelte
--rw-r--r--   0        0        0      683 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/MarkersOverlapping.svelte
--rw-r--r--   0        0        0      101 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/reports/TCellSelection.svelte
--rw-r--r--   0        0        0     4769 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/CloneHeterogeneity.R
--rw-r--r--   0        0        0     2029 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/MarkersOverlapping.R
--rw-r--r--   0        0        0    15647 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/scripts/TCellSelection.R
--rw-r--r--   0        0        0     3281 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/validate_config.py
--rw-r--r--   0        0        0       28 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/immunopipe/version.py
--rw-r--r--   0        0        0     1127 2024-04-08 23:53:51.694917 immunopipe-1.3.4.post1/pyproject.toml
--rw-r--r--   0        0        0     2470 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post1/setup.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post1/PKG-INFO
+-rw-r--r--   0        0        0    35128 2024-04-09 00:21:53.827057 immunopipe-1.3.4.post2/LICENSE
+-rw-r--r--   0        0        0     1448 2024-04-09 00:21:53.827057 immunopipe-1.3.4.post2/README.md
+-rw-r--r--   0        0        0      143 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/__main__.py
+-rw-r--r--   0        0        0     7461 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/inhouse.py
+-rw-r--r--   0        0        0      503 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/pipeline.py
+-rw-r--r--   0        0        0    33594 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/processes.py
+-rw-r--r--   0        0        0     1581 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/reports/CloneHeterogeneity.svelte
+-rw-r--r--   0        0        0      683 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/reports/MarkersOverlapping.svelte
+-rw-r--r--   0        0        0      101 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/reports/TCellSelection.svelte
+-rw-r--r--   0        0        0     4769 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/scripts/CloneHeterogeneity.R
+-rw-r--r--   0        0        0     2029 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/scripts/MarkersOverlapping.R
+-rw-r--r--   0        0        0    15647 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/scripts/TCellSelection.R
+-rw-r--r--   0        0        0     3281 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/validate_config.py
+-rw-r--r--   0        0        0       28 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/immunopipe/version.py
+-rw-r--r--   0        0        0     1127 2024-04-09 00:21:53.883058 immunopipe-1.3.4.post2/pyproject.toml
+-rw-r--r--   0        0        0     2470 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post2/setup.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 immunopipe-1.3.4.post2/PKG-INFO
```

### Comparing `immunopipe-1.3.4.post1/LICENSE` & `immunopipe-1.3.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/README.md` & `immunopipe-1.3.4.post2/README.md`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/inhouse.py` & `immunopipe-1.3.4.post2/immunopipe/inhouse.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/processes.py` & `immunopipe-1.3.4.post2/immunopipe/processes.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/reports/CloneHeterogeneity.svelte` & `immunopipe-1.3.4.post2/immunopipe/reports/CloneHeterogeneity.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/reports/MarkersOverlapping.svelte` & `immunopipe-1.3.4.post2/immunopipe/reports/MarkersOverlapping.svelte`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/scripts/CloneHeterogeneity.R` & `immunopipe-1.3.4.post2/immunopipe/scripts/CloneHeterogeneity.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/scripts/MarkersOverlapping.R` & `immunopipe-1.3.4.post2/immunopipe/scripts/MarkersOverlapping.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/scripts/TCellSelection.R` & `immunopipe-1.3.4.post2/immunopipe/scripts/TCellSelection.R`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/immunopipe/validate_config.py` & `immunopipe-1.3.4.post2/immunopipe/validate_config.py`

 * *Files identical despite different names*

### Comparing `immunopipe-1.3.4.post1/pyproject.toml` & `immunopipe-1.3.4.post2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "immunopipe"
 description = "A pipeline for integrative analysis for scTCR- and scRNA-seq data"
 authors = [ "pwwang <pwwang@pwwang.com>",]
-version = "1.3.4-post1"
+version = "1.3.4-post2"
 license = "GNU General Public License v3.0"
 readme = "README.md"
 homepage = "https://github.com/pwwang/immunopipe"
 repository = "https://github.com/pwwang/immunopipe"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `immunopipe-1.3.4.post1/setup.py` & `immunopipe-1.3.4.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'runinfo': ['pipen-runinfo>=0.6,<0.7']}
 
 entry_points = \
 {'console_scripts': ['immunopipe = immunopipe.pipeline:main']}
 
 setup_kwargs = {
     'name': 'immunopipe',
-    'version': '1.3.4.post1',
+    'version': '1.3.4.post2',
     'description': 'A pipeline for integrative analysis for scTCR- and scRNA-seq data',
     'long_description': '<p align="center">\n  <img height="120" style="height: 120px" src="https://github.com/pwwang/immunopipe/blob/dev/docs/logo.png?raw=true" />\n</p>\n<p align="center">Integrative analysis for single-cell RNA sequencing and single-cell TCR sequencing data</p>\n<hr />\n\n`immunopipe` is a pipeline based on [`pipen`](https://github.com/pwwang/pipen) framework. It includes a set of processes for scTCR- and scRNA-seq data analysis in `R`, `python` and `bash`. The pipeline is designed to be flexible and configurable.\n\n<p align="center">\n  <img src="https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.ms.png?raw=true" />\n</p>\n\nSee a more detailed flowchart [here](https://github.com/pwwang/immunopipe/blob/dev/docs/immunopipe.flowchart.png?raw=true).\n\n## Documentaion\n\n[https://pwwang.github.io/immunopipe](https://pwwang.github.io/immunopipe)\n\n## Proposing more analyses\n\nIf you have any suggestions for more analyses, please feel free to open an issue [here](https://github.com/pwwang/immunopipe/issues/new)\n\n## Example\n\n[https://github.com/pwwang/immunopipe-example](https://github.com/pwwang/immunopipe-example)\n\n## Gallery\n\nThere are some datasets with both scRNA-seq and scTCR-seq data available in the publications. The data were reanalyzed using `immunopipe` with the configurations provided in each repository, where the results are also available.\n\nCheck out the [gallery](https://pwwang.github.io/immunopipe/gallery) for more details.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/immunopipe',
```

### Comparing `immunopipe-1.3.4.post1/PKG-INFO` & `immunopipe-1.3.4.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immunopipe
-Version: 1.3.4.post1
+Version: 1.3.4.post2
 Summary: A pipeline for integrative analysis for scTCR- and scRNA-seq data
 Home-page: https://github.com/pwwang/immunopipe
 License: GNU General Public License v3.0
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

