# Comparing `tmp/graal-0.4.9rc1.tar.gz` & `tmp/graal-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graal-0.4.9rc1.tar", max compression
+gzip compressed data, was "graal-1.0.0rc1.tar", max compression
```

## Comparing `graal-0.4.9rc1.tar` & `graal-1.0.0rc1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      240 2023-05-17 12:51:56.128811 graal-0.4.9rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-05-17 12:51:56.132812 graal-0.4.9rc1/LICENSE
--rw-r--r--   0        0        0     1831 2023-05-17 12:51:56.132812 graal-0.4.9rc1/NEWS
--rw-r--r--   0        0        0    13761 2023-05-17 12:51:56.132812 graal-0.4.9rc1/README.md
--rw-r--r--   0        0        0      876 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/__init__.py
--rw-r--r--   0        0        0       91 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/_version.py
--rw-r--r--   0        0        0      876 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/__init__.py
--rw-r--r--   0        0        0      883 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/__init__.py
--rw-r--r--   0        0        0     1192 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/analyzer.py
--rw-r--r--   0        0        0     4594 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/bandit.py
--rw-r--r--   0        0        0     4543 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/cloc.py
--rw-r--r--   0        0        0     2479 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/flake8.py
--rw-r--r--   0        0        0     2317 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/jadolint.py
--rw-r--r--   0        0        0     2243 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/linguist.py
--rw-r--r--   0        0        0     5383 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/lizard.py
--rw-r--r--   0        0        0     2360 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/nomos.py
--rw-r--r--   0        0        0     2852 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/pylint.py
--rw-r--r--   0        0        0     2620 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/reverse.py
--rw-r--r--   0        0        0     4563 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/scancode.py
--rw-r--r--   0        0        0     4504 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/analyzers/scc.py
--rw-r--r--   0        0        0    11691 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/cocom.py
--rw-r--r--   0        0        0     8463 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/codep.py
--rw-r--r--   0        0        0     6344 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/colang.py
--rw-r--r--   0        0        0     8182 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/colic.py
--rw-r--r--   0        0        0     9186 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/coqua.py
--rw-r--r--   0        0        0     5662 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/backends/core/covuln.py
--rwxr-xr-x   0        0        0     4425 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/bin/graal.py
--rw-r--r--   0        0        0    23643 2023-05-17 12:51:56.132812 graal-0.4.9rc1/graal/graal.py
--rw-r--r--   0        0        0     1584 2023-05-17 12:51:56.132812 graal-0.4.9rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 12:51:56.132812 graal-0.4.9rc1/tests/__init__.py
--rw-r--r--   0        0        0     2072 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/base_analyzer.py
--rw-r--r--   0        0        0     2056 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/base_repo.py
--rw-r--r--   0        0        0     1575 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/data/Dockerfile
--rw-r--r--   0        0        0   132358 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/data/graaltest-dockerfile.zip
--rw-r--r--   0        0        0   126651 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/data/graaltest.zip
--rw-r--r--   0        0        0     4482 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/data/sample_code.py
--rwxr-xr-x   0        0        0     1174 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/run_tests.py
--rw-r--r--   0        0        0     1222 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_analyzer.py
--rw-r--r--   0        0        0     5650 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_bandit.py
--rw-r--r--   0        0        0     3341 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_cloc.py
--rw-r--r--   0        0        0    14713 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_cocom.py
--rw-r--r--   0        0        0    14625 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_codep.py
--rw-r--r--   0        0        0     8707 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_colang.py
--rw-r--r--   0        0        0    13445 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_colic.py
--rw-r--r--   0        0        0    20057 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_coqua.py
--rw-r--r--   0        0        0     7611 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_covuln.py
--rw-r--r--   0        0        0     2846 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_flake8.py
--rw-r--r--   0        0        0    29236 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_graal.py
--rw-r--r--   0        0        0     6391 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_jadolint.py
--rw-r--r--   0        0        0     2456 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_linguist.py
--rw-r--r--   0        0        0     4980 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_lizard.py
--rw-r--r--   0        0        0     2321 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_nomos.py
--rw-r--r--   0        0        0     3181 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_pylint.py
--rw-r--r--   0        0        0     2481 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_reverse.py
--rw-r--r--   0        0        0     3538 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_scancode.py
--rw-r--r--   0        0        0     4022 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/test_scc.py
--rw-r--r--   0        0        0     1191 2023-05-17 12:51:56.136812 graal-0.4.9rc1/tests/utils.py
--rw-r--r--   0        0        0    15214 1970-01-01 00:00:00.000000 graal-0.4.9rc1/PKG-INFO
+-rw-r--r--   0        0        0      276 2024-04-09 16:14:50.336855 graal-1.0.0rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-04-09 16:14:50.336855 graal-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3373 2024-04-09 16:14:50.336855 graal-1.0.0rc1/NEWS
+-rw-r--r--   0        0        0    13761 2024-04-09 16:14:50.336855 graal-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      876 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/_version.py
+-rw-r--r--   0        0        0      876 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/__init__.py
+-rw-r--r--   0        0        0      883 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/__init__.py
+-rw-r--r--   0        0        0     1192 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/analyzer.py
+-rw-r--r--   0        0        0     4594 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/bandit.py
+-rw-r--r--   0        0        0     4543 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/cloc.py
+-rw-r--r--   0        0        0     2479 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/flake8.py
+-rw-r--r--   0        0        0     2317 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/jadolint.py
+-rw-r--r--   0        0        0     2243 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/linguist.py
+-rw-r--r--   0        0        0     5383 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/lizard.py
+-rw-r--r--   0        0        0     2360 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/nomos.py
+-rw-r--r--   0        0        0     2852 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/pylint.py
+-rw-r--r--   0        0        0     2620 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/reverse.py
+-rw-r--r--   0        0        0     4563 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/scancode.py
+-rw-r--r--   0        0        0     4504 2024-04-09 16:14:50.336855 graal-1.0.0rc1/graal/backends/core/analyzers/scc.py
+-rw-r--r--   0        0        0    11691 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/cocom.py
+-rw-r--r--   0        0        0     8463 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/codep.py
+-rw-r--r--   0        0        0     6344 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/colang.py
+-rw-r--r--   0        0        0     8182 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/colic.py
+-rw-r--r--   0        0        0     9186 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/coqua.py
+-rw-r--r--   0        0        0     5662 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/backends/core/covuln.py
+-rwxr-xr-x   0        0        0     4425 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/bin/graal.py
+-rw-r--r--   0        0        0    23643 2024-04-09 16:14:50.340855 graal-1.0.0rc1/graal/graal.py
+-rw-r--r--   0        0        0     1596 2024-04-09 16:14:50.340855 graal-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     2072 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/base_analyzer.py
+-rw-r--r--   0        0        0     2056 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/base_repo.py
+-rw-r--r--   0        0        0     1575 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/data/Dockerfile
+-rw-r--r--   0        0        0   132358 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/data/graaltest-dockerfile.zip
+-rw-r--r--   0        0        0   126651 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/data/graaltest.zip
+-rw-r--r--   0        0        0     4482 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/data/sample_code.py
+-rwxr-xr-x   0        0        0     1174 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     1222 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_analyzer.py
+-rw-r--r--   0        0        0     5650 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_bandit.py
+-rw-r--r--   0        0        0     3341 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_cloc.py
+-rw-r--r--   0        0        0    14713 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_cocom.py
+-rw-r--r--   0        0        0    14625 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_codep.py
+-rw-r--r--   0        0        0     8707 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_colang.py
+-rw-r--r--   0        0        0    13445 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_colic.py
+-rw-r--r--   0        0        0    20057 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_coqua.py
+-rw-r--r--   0        0        0     7611 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_covuln.py
+-rw-r--r--   0        0        0     2846 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_flake8.py
+-rw-r--r--   0        0        0    29236 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_graal.py
+-rw-r--r--   0        0        0     6391 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_jadolint.py
+-rw-r--r--   0        0        0     2456 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_linguist.py
+-rw-r--r--   0        0        0     4980 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_lizard.py
+-rw-r--r--   0        0        0     2321 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_nomos.py
+-rw-r--r--   0        0        0     3181 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_pylint.py
+-rw-r--r--   0        0        0     2481 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_reverse.py
+-rw-r--r--   0        0        0     3538 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_scancode.py
+-rw-r--r--   0        0        0     4022 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/test_scc.py
+-rw-r--r--   0        0        0     1191 2024-04-09 16:14:50.340855 graal-1.0.0rc1/tests/utils.py
+-rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 graal-1.0.0rc1/PKG-INFO
```

### Comparing `graal-0.4.9rc1/LICENSE` & `graal-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/README.md` & `graal-1.0.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 and **latest_items** returns only those commits which are new since the last fetch operation. Graal includes additional parameters to drive
 the analysis to filter in/out files and directories in the repository (**in_paths** and **out_paths**), set the **entrypoint**
 and define the **details** level of the analysis (useful when analyzing large software projects).
 
 ## Requirements
 
 
- * Python >= 3.7
+ * Python >= 3.8
  * Poetry >= 1.2
  * [github-linguist](https://github.com/github/linguist)
  * [FOSSology](https://github.com/fossology/fossology)
  * [cloc](https://github.com/AlDanial/cloc)
  * [scc](https://github.com/boyter/scc)
  * [ScanCode toolkit](https://github.com/nexB/scancode-toolkit)
  * [crossJadoLint](https://github.com/crossminer/crossJadolint/)
```

### Comparing `graal-0.4.9rc1/graal/__init__.py` & `graal-1.0.0rc1/graal/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/__init__.py` & `graal-1.0.0rc1/graal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/__init__.py` & `graal-1.0.0rc1/graal/backends/core/__init__.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/analyzer.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/bandit.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/cloc.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/flake8.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/jadolint.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/linguist.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/lizard.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/nomos.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/pylint.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/reverse.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/scancode.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/analyzers/scc.py` & `graal-1.0.0rc1/graal/backends/core/analyzers/scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/cocom.py` & `graal-1.0.0rc1/graal/backends/core/cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/codep.py` & `graal-1.0.0rc1/graal/backends/core/codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/colang.py` & `graal-1.0.0rc1/graal/backends/core/colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/colic.py` & `graal-1.0.0rc1/graal/backends/core/colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/coqua.py` & `graal-1.0.0rc1/graal/backends/core/coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/backends/core/covuln.py` & `graal-1.0.0rc1/graal/backends/core/covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/bin/graal.py` & `graal-1.0.0rc1/graal/bin/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/graal/graal.py` & `graal-1.0.0rc1/graal/graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/pyproject.toml` & `graal-1.0.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graal"
-version = "0.4.9-rc.1"
+version = "1.0.0-rc.1"
 description = "A generic source code analyzer"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -25,45 +25,45 @@
 include = [
     { path = "AUTHORS", format = "sdist" },
     { path = "README.md", format = "sdist" },
     { path = "NEWS", format = "sdist" },
 ]
 
 classifiers = [
-   "Development Status :: 4 - Beta",
+   "Development Status :: 5 - Production/Stable",
    "Intended Audience :: Developers",
    "Intended Audience :: Science/Research",
    "Topic :: Software Development",
    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
    "Programming Language :: Python :: 3"
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/chaoss/grimoirelab-graal/issues"
 
 [tool.poetry.scripts]
 graal = 'graal.bin.graal:main'
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 lizard = "1.16.6"
 pylint = ">=1.8.4"
 flake8 = "^4.0.1"
 networkx = ">=2.1"
 pydot = ">=1.2.4"
 bandit = ">=1.4.0"
 perceval = { version = ">=0.19", allow-prereleases = true }
 grimoirelab-toolkit = { version = ">=0.3", allow-prereleases = true}
 cloc = "^0.2.5"
 execnet = "^1.9.0"
 
-# Pinned because 'myst-parser = ^0.15.2' in Perceval
-markdown-it-py = "^1.0.0"
+# Pinned because 'myst-parser = ^1.0.0' in Perceval
+markdown-it-py = "^2.0.0"
 
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
-coverage = "^6.3.2"
+coverage = "^7.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `graal-0.4.9rc1/tests/base_analyzer.py` & `graal-1.0.0rc1/tests/base_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/base_repo.py` & `graal-1.0.0rc1/tests/base_repo.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/data/Dockerfile` & `graal-1.0.0rc1/tests/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/data/graaltest-dockerfile.zip` & `graal-1.0.0rc1/tests/data/graaltest-dockerfile.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/data/graaltest.zip` & `graal-1.0.0rc1/tests/data/graaltest.zip`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/data/sample_code.py` & `graal-1.0.0rc1/tests/data/sample_code.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/run_tests.py` & `graal-1.0.0rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_analyzer.py` & `graal-1.0.0rc1/tests/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_bandit.py` & `graal-1.0.0rc1/tests/test_bandit.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_cloc.py` & `graal-1.0.0rc1/tests/test_cloc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_cocom.py` & `graal-1.0.0rc1/tests/test_cocom.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_codep.py` & `graal-1.0.0rc1/tests/test_codep.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_colang.py` & `graal-1.0.0rc1/tests/test_colang.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_colic.py` & `graal-1.0.0rc1/tests/test_colic.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_coqua.py` & `graal-1.0.0rc1/tests/test_coqua.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_covuln.py` & `graal-1.0.0rc1/tests/test_covuln.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_flake8.py` & `graal-1.0.0rc1/tests/test_flake8.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_graal.py` & `graal-1.0.0rc1/tests/test_graal.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_jadolint.py` & `graal-1.0.0rc1/tests/test_jadolint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_linguist.py` & `graal-1.0.0rc1/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_lizard.py` & `graal-1.0.0rc1/tests/test_lizard.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_nomos.py` & `graal-1.0.0rc1/tests/test_nomos.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_pylint.py` & `graal-1.0.0rc1/tests/test_pylint.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_reverse.py` & `graal-1.0.0rc1/tests/test_reverse.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_scancode.py` & `graal-1.0.0rc1/tests/test_scancode.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/test_scc.py` & `graal-1.0.0rc1/tests/test_scc.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/tests/utils.py` & `graal-1.0.0rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `graal-0.4.9rc1/PKG-INFO` & `graal-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: graal
-Version: 0.4.9rc1
+Version: 1.0.0rc1
 Summary: A generic source code analyzer
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: bandit (>=1.4.0)
 Requires-Dist: cloc (>=0.2.5,<0.3.0)
 Requires-Dist: execnet (>=1.9.0,<2.0.0)
 Requires-Dist: flake8 (>=4.0.1,<5.0.0)
 Requires-Dist: grimoirelab-toolkit (>=0.3)
 Requires-Dist: lizard (==1.16.6)
-Requires-Dist: markdown-it-py (>=1.0.0,<2.0.0)
+Requires-Dist: markdown-it-py (>=2.0.0,<3.0.0)
 Requires-Dist: networkx (>=2.1)
 Requires-Dist: perceval (>=0.19)
 Requires-Dist: pydot (>=1.2.4)
 Requires-Dist: pylint (>=1.8.4)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-graal/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-graal
 Description-Content-Type: text/markdown
@@ -55,15 +53,15 @@
 and **latest_items** returns only those commits which are new since the last fetch operation. Graal includes additional parameters to drive
 the analysis to filter in/out files and directories in the repository (**in_paths** and **out_paths**), set the **entrypoint**
 and define the **details** level of the analysis (useful when analyzing large software projects).
 
 ## Requirements
 
 
- * Python >= 3.7
+ * Python >= 3.8
  * Poetry >= 1.2
  * [github-linguist](https://github.com/github/linguist)
  * [FOSSology](https://github.com/fossology/fossology)
  * [cloc](https://github.com/AlDanial/cloc)
  * [scc](https://github.com/boyter/scc)
  * [ScanCode toolkit](https://github.com/nexB/scancode-toolkit)
  * [crossJadoLint](https://github.com/crossminer/crossJadolint/)
```

