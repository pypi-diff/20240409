# Comparing `tmp/markdown_convert-0.9.9.tar.gz` & `tmp/markdown_convert-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-0.9.9.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.0.tar", max compression
```

## Comparing `markdown_convert-0.9.9.tar` & `markdown_convert-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-0.9.9/LICENSE
--rw-r--r--   0        0        0     1531 2024-04-08 21:24:43.477483 markdown_convert-0.9.9/README.md
--rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-0.9.9/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-0.9.9/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-0.9.9/markdown_convert/code.css
--rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-0.9.9/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-0.9.9/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-0.9.9/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     4062 2024-04-08 21:48:34.445200 markdown_convert-0.9.9/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-0.9.9/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-0.9.9/markdown_convert/modules/utils_strings.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-0.9.9/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-08 21:49:00.461550 markdown_convert-0.9.9/pyproject.toml
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 markdown_convert-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-08 21:59:41.383922 markdown_convert-1.0.0/README.md
+-rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-1.0.0/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-1.0.0/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.0/markdown_convert/code.css
+-rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-1.0.0/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.0/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.0/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     4062 2024-04-08 21:48:34.445200 markdown_convert-1.0.0/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-1.0.0/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-1.0.0/markdown_convert/modules/utils_strings.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.0/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-08 22:00:04.060328 markdown_convert-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.0/PKG-INFO
```

### Comparing `markdown_convert-0.9.9/LICENSE` & `markdown_convert-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/README.md` & `markdown_convert-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
 
 It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
 
 ### Features
 
-- Supports live compilation, so you can preview your PDF in real-time as you type.
-- Comes with beautiful CSS out of the box, making your documents look great from the start.
-- Syntax highlighting for code blocks included.
-- Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
+- ⚡️ Supports live compilation, so you can preview your PDF in real-time as you type.
+- 🌸 Comes with beautiful CSS out of the box, making your documents look great from the start.
+- 🎨 Syntax highlighting for code blocks included.
+- 🪐 Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
 
 ### Usage
 
 Run `markdown-convert -h` right from your terminal to check out the available options:
 
 ```bash
 Usage:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `markdown_convert-0.9.9/markdown_convert/__main__.py` & `markdown_convert-1.0.0/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/markdown_convert/code.css` & `markdown_convert-1.0.0/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/markdown_convert/default.css` & `markdown_convert-1.0.0/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/markdown_convert/modules/convert.py` & `markdown_convert-1.0.0/markdown_convert/modules/convert.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/markdown_convert/modules/resources.py` & `markdown_convert-1.0.0/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/markdown_convert/modules/validate.py` & `markdown_convert-1.0.0/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.9/pyproject.toml` & `markdown_convert-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "0.9.9"
+version = "1.0.0"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-0.9.9/PKG-INFO` & `markdown_convert-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 0.9.9
+Version: 1.0.0
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -29,18 +29,18 @@
 
 `markdown-convert` is an elegant command-line tool that converts Markdown files to PDF.
 
 It is powered by the amazing `markdown2` and `weasyprint` libraries, and unlike other similar tools, it relies solely on Python packages to do the job, eliminating the need for any external system-level dependencies.
 
 ### Features
 
-- Supports live compilation, so you can preview your PDF in real-time as you type.
-- Comes with beautiful CSS out of the box, making your documents look great from the start.
-- Syntax highlighting for code blocks included.
-- Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
+- ⚡️ Supports live compilation, so you can preview your PDF in real-time as you type.
+- 🌸 Comes with beautiful CSS out of the box, making your documents look great from the start.
+- 🎨 Syntax highlighting for code blocks included.
+- 🪐 Designed for the 21st century, with relative links, pipe tables, and modern CSS paged media features.
 
 ### Usage
 
 Run `markdown-convert -h` right from your terminal to check out the available options:
 
 ```bash
 Usage:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

