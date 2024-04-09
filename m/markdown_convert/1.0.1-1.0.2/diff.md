# Comparing `tmp/markdown_convert-1.0.1.tar.gz` & `tmp/markdown_convert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-1.0.1.tar", max compression
+gzip compressed data, was "markdown_convert-1.0.2.tar", max compression
```

## Comparing `markdown_convert-1.0.1.tar` & `markdown_convert-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.1/LICENSE
--rw-r--r--   0        0        0     1553 2024-04-09 10:23:30.361958 markdown_convert-1.0.1/README.md
--rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.1/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-1.0.1/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.1/markdown_convert/code.css
--rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-1.0.1/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.1/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.1/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     5853 2024-04-09 10:47:07.601350 markdown_convert-1.0.1/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-1.0.1/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-1.0.1/markdown_convert/modules/utils_strings.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.1/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-09 10:33:59.945828 markdown_convert-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1553 2024-04-09 10:23:30.361958 markdown_convert-1.0.2/README.md
+-rw-r--r--   0        0        0      197 2024-04-09 10:46:16.220929 markdown_convert-1.0.2/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2815 2024-04-09 12:12:31.637276 markdown_convert-1.0.2/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-1.0.2/markdown_convert/code.css
+-rw-r--r--   0        0        0     5433 2024-04-09 12:35:37.486669 markdown_convert-1.0.2/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-1.0.2/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-1.0.2/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     5984 2024-04-09 12:18:10.414947 markdown_convert-1.0.2/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2258 2024-04-09 12:12:32.309271 markdown_convert-1.0.2/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      541 2024-04-09 12:13:03.121058 markdown_convert-1.0.2/markdown_convert/modules/utils.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-1.0.2/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-09 12:15:25.468079 markdown_convert-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 markdown_convert-1.0.2/PKG-INFO
```

### Comparing `markdown_convert-1.0.1/LICENSE` & `markdown_convert-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.1/README.md` & `markdown_convert-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.1/markdown_convert/__main__.py` & `markdown_convert-1.0.2/markdown_convert/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from sys import exit as sys_exit
 
 from argsdict import args
 from .modules.constants import RED, OPTIONS, OPTIONS_MODES
 from .modules.convert import convert, live_convert
 from .modules.resources import get_css_path, get_output_path, get_usage
-from .modules.utils_strings import color
+from .modules.utils import color
 from .modules.validate import (validate_css_path, validate_markdown_path,
                                validate_output_path)
 
 
 def main():
     """
     Convert a markdown file to a pdf file.
```

### Comparing `markdown_convert-1.0.1/markdown_convert/code.css` & `markdown_convert-1.0.2/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.1/markdown_convert/default.css` & `markdown_convert-1.0.2/markdown_convert/default.css`

 * *Files 6% similar despite different names*

```diff
@@ -202,16 +202,15 @@
   border-radius: 0.3em;
 }
 
 h1 code,
 h2 code,
 h3 code,
 h4 code,
-h5 code,
-h6 code {
+h5 code {
   font-size: 0.8em; /* Adjust the font size as needed */
 }
 
 .sourceCode {
   background-color: #eee;
   padding: 0.3em 0.4em;
   border-radius: 0.3em;
@@ -243,29 +242,29 @@
   font-size: 10px;
   border-collapse: collapse;
   margin-top: 1em;
   text-align: left;
   table-layout: auto;
 }
 
-table thead {
+thead {
   background-color: #eee;
 }
 
-table thead th,
-table tbody td {
+tbody {
+  color: #666;
+}
+
+th,
+td {
   padding: 0.5em 0.75em;
   border: 1px solid #ccc;
   white-space: nowrap;
 }
 
-table tbody td {
-  color: #666;
-}
-
 col {
   width: auto !important;
 }
 
 /* Page breaks */
 .pagebreak {
   clear: both;
```

### Comparing `markdown_convert-1.0.1/markdown_convert/modules/convert.py` & `markdown_convert-1.0.2/markdown_convert/modules/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathlib import Path
 
 import markdown2
 import weasyprint
 
 
 from .resources import get_css_path, get_code_css_path, get_output_path
+from .utils import drop_duplicates
 
 
 def convert(md_path, css_path=None, output_path=None,
             *, extend_default_css=True):
     """
     Convert a markdown file to a pdf file.
 
@@ -30,17 +31,19 @@
     if css_path is None:
         css_path = get_css_path()
 
     if output_path is None:
         output_path = get_output_path(md_path, None)
 
     if extend_default_css:
-        css_sources = set([css_path, get_css_path(), get_code_css_path()])
+        css_sources = [get_code_css_path(), get_css_path(), css_path]
     else:
-        css_sources = set([css_path, get_code_css_path()])
+        css_sources = [get_code_css_path(), css_path]
+
+    css_sources = drop_duplicates(css_sources)
 
     try:
         html = markdown2.markdown_path(md_path,
                                        extras=["fenced-code-blocks",
                                                "toc",
                                                "tables"])
 
@@ -85,26 +88,27 @@
         md_text (str): Markdown text.
         css_text (str=None): CSS text.
         extend_default_css (bool=True): Extend the default CSS file.
 
     Returns:
         PDF file as bytes.
     """
-    default_css = Path(get_css_path()).read_text()
-    code_css = Path(get_code_css_path()).read_text()
+    default_css = Path(get_css_path()).read_text(encoding='utf-8')
+    code_css = Path(get_code_css_path()).read_text(encoding='utf-8')
 
     if css_text is None:
         css_text = default_css
 
     if extend_default_css:
-        css_sources = set([css_text, default_css, code_css])
+        css_sources = [code_css, default_css, css_text]
     else:
-        css_sources = set([css_text, code_css])
+        css_sources = [code_css, css_text]
 
-    css_sources = [weasyprint.CSS(string=css) for css in css_sources]
+    css_sources = [weasyprint.CSS(string=css)
+                   for css in drop_duplicates(css_sources)]
 
     try:
         html = markdown2.markdown(md_text,
                                   extras=["fenced-code-blocks",
                                           "toc",
                                           "tables"])
```

### Comparing `markdown_convert-1.0.1/markdown_convert/modules/resources.py` & `markdown_convert-1.0.2/markdown_convert/modules/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from pathlib import Path
 
 import pkg_resources
 
 from .constants import BLUE, CYAN, GREEN, YELLOW, OPTIONS, OPTIONS_MODES
-from .utils_strings import color
+from .utils import color
 
 
 def get_output_path(md_path, output_dir=None):
     """
     Get the output path for the pdf file.
 
     Args:
```

### Comparing `markdown_convert-1.0.1/markdown_convert/modules/validate.py` & `markdown_convert-1.0.2/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-1.0.1/pyproject.toml` & `markdown_convert-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "1.0.1"
+version = "1.0.2"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-1.0.1/PKG-INFO` & `markdown_convert-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

