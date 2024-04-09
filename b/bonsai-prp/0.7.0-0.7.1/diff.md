# Comparing `tmp/bonsai-prp-0.7.0.tar.gz` & `tmp/bonsai-prp-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonsai-prp-0.7.0.tar", last modified: Mon Mar 25 13:23:51 2024, max compression
+gzip compressed data, was "bonsai-prp-0.7.1.tar", last modified: Tue Apr  9 11:34:10 2024, max compression
```

## Comparing `bonsai-prp-0.7.0.tar` & `bonsai-prp-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/bonsai_prp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-25 13:23:51.000000 bonsai-prp-0.7.0/bonsai_prp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.148148 bonsai-prp-0.7.0/prp/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.148148 bonsai-prp-0.7.0/prp/models/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/phenotype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/prp/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/prp/parse/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/mykrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/resfinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/serotypefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/tbprofiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/phenotype/virulencefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/qc.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/species.py
--rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/prp/parse/variant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:23:51.152148 bonsai-prp-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-03-25 13:23:37.000000 bonsai-prp-0.7.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.082589 bonsai-prp-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/bonsai_prp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 11:34:10.000000 bonsai-prp-0.7.1/bonsai_prp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.074589 bonsai-prp-0.7.1/prp/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/phenotype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/prp/parse/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/mykrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/resfinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/serotypefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/tbprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/phenotype/virulencefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/qc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7067 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/prp/parse/variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:34:10.082589 bonsai-prp-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:34:10.078589 bonsai-prp-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-09 11:33:56.000000 bonsai-prp-0.7.1/tests/test_cli.py
```

### Comparing `bonsai-prp-0.7.0/LICENSE` & `bonsai-prp-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/PKG-INFO` & `bonsai-prp-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai-prp-0.7.0/README.md` & `bonsai-prp-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/bonsai_prp.egg-info/PKG-INFO` & `bonsai-prp-0.7.1/bonsai_prp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonsai-prp
-Version: 0.7.0
+Version: 0.7.1
 Summary: Pipline result processing program for the JASEN pipeline and Bonsai tool.
 Author-email: Markus Johansson <markus.h.johansson@skane.se>, Ryan Kennedy <Ryan.Kennedy@skane.se>
 Project-URL: Repository, https://github.com/Clinical-Genomics-Lund/
 Project-URL: Issues, https://github.com/Clinical-Genomics-Lund/bonsai-prp/issues
 Project-URL: Changelog, https://github.com/Clinical-Genomics-Lund/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `bonsai-prp-0.7.0/bonsai_prp.egg-info/SOURCES.txt` & `bonsai-prp-0.7.1/bonsai_prp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/cli.py` & `bonsai-prp-0.7.1/prp/cli.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/metadata.py` & `bonsai-prp-0.7.1/prp/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/phenotype.py` & `bonsai-prp-0.7.1/prp/models/phenotype.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/qc.py` & `bonsai-prp-0.7.1/prp/models/qc.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     reference_gc: float
     duplication_ratio: float
 
 
 class PostAlignQcResult(BaseModel):
     """Alignment QC metrics."""
 
-    ins_size: int
-    ins_size_dev: int
+    ins_size: int | None = None
+    ins_size_dev: int | None = None
     mean_cov: int
     pct_above_x: Dict[str, float]
     n_reads: int
     n_mapped_reads: int
     n_read_pairs: int
     coverage_uniformity: float | None = None
     quartile1: float
```

### Comparing `bonsai-prp-0.7.0/prp/models/sample.py` & `bonsai-prp-0.7.1/prp/models/sample.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/species.py` & `bonsai-prp-0.7.1/prp/models/species.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/tags.py` & `bonsai-prp-0.7.1/prp/models/tags.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/models/typing.py` & `bonsai-prp-0.7.1/prp/models/typing.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/__init__.py` & `bonsai-prp-0.7.1/prp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/metadata.py` & `bonsai-prp-0.7.1/prp/parse/metadata.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/amrfinder.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/mykrobe.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/mykrobe.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/resfinder.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/resfinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/serotypefinder.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/serotypefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/tbprofiler.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/tbprofiler.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/phenotype/virulencefinder.py` & `bonsai-prp-0.7.1/prp/parse/phenotype/virulencefinder.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/qc.py` & `bonsai-prp-0.7.1/prp/parse/qc.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         self.bam = bam
         self.bed = bed
         self.sample_id = sample_id
         self.cpus = cpus
         self.baits = baits
         self.reference = reference
         self.paired = self.is_paired()
+        self.rm_files = True
 
     def write_json_result(self, json_result: dict, output_filepath: str) -> None:
         """Write out json file"""
         with open(output_filepath, "w", encoding="utf-8") as json_file:
             json.dump(json_result, json_file, indent=4)
 
     def convert2intervals(self, bed_baits: str, dict_file: str) -> None:
@@ -104,17 +105,20 @@
         self.results["quartile1"] = quartile1
         self.results["median_cov"] = median_cov
         self.results["quartile3"] = quartile3
 
     def is_paired(self) -> bool:
         """Check if reads are paired"""
         bam_file = pysam.AlignmentFile(self.bam)
-        for read in bam_file:
-            return read.is_paired
-        # If no reads are found or read is None, return False
+        for i, read in enumerate(bam_file):
+            if read.is_paired:
+                return True
+            if i >= 1000:
+                break
+        # If no paired reads are found in the first 1000 reads or read is None, return False
         return False
 
     def system_p(self, cmd: list) -> None:
         """Execute subprocess"""
         LOG.info("RUNNING: %s", " ".join(cmd))
         result = subprocess.run(cmd, check=True, text=True)
         if result.stderr:
@@ -189,17 +193,18 @@
                 "1000000",
             ]
             self.system_p(cmd)
 
             # Parse ismetrics output file
             self.parse_ismetrics(f"{self.bam}.inssize")
 
-            # Remove ismetrics files after parsing
-            os.remove(f"{self.bam}.inssize")
-            os.remove(f"{self.bam}.ins.pdf")
+            if self.rm_files:
+                # Remove ismetrics files
+                os.remove(f"{self.bam}.inssize")
+                os.remove(f"{self.bam}.ins.pdf")
 
         out_prefix = f"{self.bam}_postalnQC"
         thresholds = ["1", "10", "30", "100", "250", "500", "1000"]
 
         # Index bam file if .bai does not exist
         if not os.path.exists(f"{self.bam}.bai"):
             LOG.info("Indexing bam file: %s.bai", self.bam)
@@ -214,15 +219,17 @@
         if self.bed:
             sambamba_depth_cmd.extend(["-L", self.bed])
         sambamba_depth_cmd.extend([self.bam, "-o", f"{out_prefix}.basecov.bed"])
         self.system_p(sambamba_depth_cmd)
 
         # Parse base coverage file
         self.parse_basecov_bed(f"{out_prefix}.basecov.bed", thresholds)
-        os.remove(f"{out_prefix}.basecov.bed")
+        if self.rm_files:
+            # Remove base coverage file
+            os.remove(f"{out_prefix}.basecov.bed")
 
         self.results["n_reads"] = n_reads
         self.results["n_mapped_reads"] = n_mapped_reads
         self.results["n_read_pairs"] = n_read_pairs
         self.results["n_dup_reads"] = n_dup_reads
         self.results["dup_pct"] = n_dup_reads / n_mapped_reads
         self.results["sample_id"] = self.sample_id
@@ -264,22 +271,22 @@
 
     Returns:
         PostAlignQc: list of key-value pairs
     """
     LOG.info("Parsing json file: %s", input_file.name)
     qc_dict = json.load(input_file)
     qc_res = PostAlignQcResult(
-        ins_size=int(float(qc_dict["ins_size"])),
-        ins_size_dev=int(float(qc_dict["ins_size_dev"])),
+        ins_size=None if "ins_size" not in qc_dict else int(float(qc_dict["ins_size"])),
+        ins_size_dev=None if "ins_size_dev" not in qc_dict else int(float(qc_dict["ins_size_dev"])),
         mean_cov=int(qc_dict["mean_cov"]),
         pct_above_x=qc_dict["pct_above_x"],
         n_reads=int(qc_dict["n_reads"]),
         n_mapped_reads=int(qc_dict["n_mapped_reads"]),
         n_read_pairs=int(qc_dict["n_read_pairs"]),
-        coverage_uniformity=float(qc_dict["coverage_uniformity"]),
+        coverage_uniformity=float(qc_dict["coverage_uniformity"]) if qc_dict.get("coverage_uniformity") is not None else None,
         quartile1=float(qc_dict["quartile1"]),
         median_cov=float(qc_dict["median_cov"]),
         quartile3=float(qc_dict["quartile3"]),
     )
     return QcMethodIndex(software=QcSoftware.POSTALIGNQC, result=qc_res)
```

### Comparing `bonsai-prp-0.7.0/prp/parse/species.py` & `bonsai-prp-0.7.1/prp/parse/species.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/typing.py` & `bonsai-prp-0.7.1/prp/parse/typing.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/utils.py` & `bonsai-prp-0.7.1/prp/parse/utils.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/prp/parse/variant.py` & `bonsai-prp-0.7.1/prp/parse/variant.py`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/pyproject.toml` & `bonsai-prp-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bonsai-prp-0.7.0/tests/test_cli.py` & `bonsai-prp-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

