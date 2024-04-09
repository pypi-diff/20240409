# Comparing `tmp/fixms-0.2.3.tar.gz` & `tmp/fixms-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.2.3.tar", max compression
+gzip compressed data, was "fixms-0.2.4.tar", max compression
```

## Comparing `fixms-0.2.3.tar` & `fixms-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-02-16 02:52:49.670709 fixms-0.2.3/LICENSE
--rw-r--r--   0        0        0     4935 2024-02-16 02:52:49.670709 fixms-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-02-16 02:52:49.670709 fixms-0.2.3/fixms/__init__.py
--rw-r--r--   0        0        0     1812 2024-02-16 02:52:49.670709 fixms-0.2.3/fixms/fix_ms.py
--rw-r--r--   0        0        0    20122 2024-02-16 02:52:49.670709 fixms-0.2.3/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    14376 2024-02-16 02:52:49.670709 fixms-0.2.3/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0     5105 2024-02-16 02:52:49.674709 fixms-0.2.3/fixms/logger.py
--rw-r--r--   0        0        0      882 2024-02-16 02:52:49.674709 fixms-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5639 1970-01-01 00:00:00.000000 fixms-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 08:59:49.808570 fixms-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4935 2024-04-09 08:59:49.808570 fixms-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms.py
+-rw-r--r--   0        0        0    20122 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    14376 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0     5105 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/logger.py
+-rw-r--r--   0        0        0      886 2024-04-09 08:59:49.808570 fixms-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5631 1970-01-01 00:00:00.000000 fixms-0.2.4/PKG-INFO
```

### Comparing `fixms-0.2.3/LICENSE` & `fixms-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/README.md` & `fixms-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/fixms/fix_ms.py` & `fixms-0.2.4/fixms/fix_ms.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/fixms/fix_ms_corrs.py` & `fixms-0.2.4/fixms/fix_ms_corrs.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/fixms/fix_ms_dir.py` & `fixms-0.2.4/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/fixms/logger.py` & `fixms-0.2.4/fixms/logger.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.3/pyproject.toml` & `fixms-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "fixms"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8"
 numpy = "<1.26"
-astropy = "^5"
+astropy = ">=5"
 python-casacore = "*"
 tqdm = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
-black = "^23.3.0"
+isort = ">=5.12.0"
+black = ">=23.3.0"
 sphinx = "*"
 numpydoc = "*"
 myst_parser = "*"
 autoapi = "*"
 sphinx-autoapi = "*"
 pytest = "*"
 pre-commit = "*"
```

### Comparing `fixms-0.2.3/PKG-INFO` & `fixms-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
-Requires-Dist: astropy (>=5,<6)
+Requires-Dist: astropy (>=5)
 Requires-Dist: numpy (<1.26)
 Requires-Dist: python-casacore
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 [![rtd](https://readthedocs.org/projects/fixms/badge/?version=latest)](https://fixms.readthedocs.io/) [![Tests](https://github.com/AlecThomson/FixMS/actions/workflows/test.yml/badge.svg)](https://github.com/AlecThomson/FixMS/actions/workflows/test.yml) [![PyPi](https://github.com/AlecThomson/FixMS/actions/workflows/publish.yml/badge.svg)](https://pypi.org/project/fixms/) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/FixMS/main.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/FixMS/main)
```

