# Comparing `tmp/markdown_convert-1.0.0.tar.gz` & `tmp/markdown_convert-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.0.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.1.tar", max compression
```

## Comparing `markdown_convert-1.0.0.tar` & `markdown_convert-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.0/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-08 21:59:41.383922 markdown_convert-1.0.0/README.md
--rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-1.0.0/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-1.0.0/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.0/markdown_convert/code.css
--rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-1.0.0/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.0/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.0/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     4062 2024-04-08 21:48:34.445200 markdown_convert-1.0.0/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-1.0.0/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-1.0.0/markdown_convert/modules/utils_strings.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.0/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-08 22:00:04.060328 markdown_convert-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-09 10:23:30.361958 markdown_convert-1.0.1/README.md
+-rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.1/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-1.0.1/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.1/markdown_convert/code.css
+-rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-1.0.1/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.1/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.1/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5853 2024-04-09 10:47:07.601350 markdown_convert-1.0.1/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-1.0.1/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-1.0.1/markdown_convert/modules/utils_strings.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.1/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-09 10:33:59.945828 markdown_convert-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.1/PKG-INFO
```

### Comparing `markdown_convert-1.0.0/LICENSE` & `markdown_convert-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/README.md` & `markdown_convert-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,12 +35,12 @@
 
 ...or import any of the functions from the package to use them in your own code:
 
 ```python
 from markdown_convert import convert, live_convert
 
 # Convert your Markdown file to PDF once
-convert('README.md', "style.css", 'README.pdf')
+convert('README.md', 'style.css', 'README.pdf')
 
 # Convert your Markdown file to PDF every time it changes
-live_convert('README.md', "style.css", 'README.pdf')
+live_convert('README.md', 'style.css', 'README.pdf')
 ```
```

### Comparing `markdown_convert-1.0.0/markdown_convert/__main__.py` & `markdown_convert-1.0.1/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/markdown_convert/code.css` & `markdown_convert-1.0.1/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/markdown_convert/default.css` & `markdown_convert-1.0.1/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/markdown_convert/modules/resources.py` & `markdown_convert-1.0.1/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/markdown_convert/modules/validate.py` & `markdown_convert-1.0.1/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.0/pyproject.toml` & `markdown_convert-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.0"
+version = "1.0.1"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.0.0/PKG-INFO` & `markdown_convert-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -57,13 +57,13 @@
 
 ...or import any of the functions from the package to use them in your own code:
 
 ```python
 from markdown_convert import convert, live_convert
 
 # Convert your Markdown file to PDF once
-convert('README.md', "style.css", 'README.pdf')
+convert('README.md', 'style.css', 'README.pdf')
 
 # Convert your Markdown file to PDF every time it changes
-live_convert('README.md', "style.css", 'README.pdf')
+live_convert('README.md', 'style.css', 'README.pdf')
 ```
```

