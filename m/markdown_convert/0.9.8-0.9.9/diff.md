# Comparing `tmp/markdown_convert-0.9.8.tar.gz` & `tmp/markdown_convert-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_convert-0.9.8.tar", max compression
+gzip compressed data, was "markdown_convert-0.9.9.tar", max compression
```

## Comparing `markdown_convert-0.9.8.tar` & `markdown_convert-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-0.9.8/LICENSE
--rw-r--r--   0        0        0     1531 2024-04-08 21:24:43.477483 markdown_convert-0.9.8/README.md
--rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-0.9.8/markdown_convert/__init__.py
--rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-0.9.8/markdown_convert/__main__.py
--rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-0.9.8/markdown_convert/code.css
--rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-0.9.8/markdown_convert/default.css
--rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-0.9.8/markdown_convert/modules/__init__.py
--rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-0.9.8/markdown_convert/modules/constants.py
--rw-r--r--   0        0        0     3900 2024-04-08 19:10:52.451331 markdown_convert-0.9.8/markdown_convert/modules/convert.py
--rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-0.9.8/markdown_convert/modules/resources.py
--rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-0.9.8/markdown_convert/modules/utils_strings.py
--rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-0.9.8/markdown_convert/modules/validate.py
--rw-r--r--   0        0        0      658 2024-04-08 21:30:39.962970 markdown_convert-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 markdown_convert-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-10-23 17:37:06.761873 markdown_convert-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1531 2024-04-08 21:24:43.477483 markdown_convert-0.9.9/README.md
+-rw-r--r--   0        0        0      183 2024-04-08 21:28:46.972862 markdown_convert-0.9.9/markdown_convert/__init__.py
+-rwxr-xr-x   0        0        0     2823 2024-04-08 14:55:19.194948 markdown_convert-0.9.9/markdown_convert/__main__.py
+-rw-r--r--   0        0        0     4935 2024-04-08 12:12:18.468503 markdown_convert-0.9.9/markdown_convert/code.css
+-rw-r--r--   0        0        0     5481 2024-04-08 19:33:11.286944 markdown_convert-0.9.9/markdown_convert/default.css
+-rw-r--r--   0        0        0       49 2024-04-08 21:28:56.305028 markdown_convert-0.9.9/markdown_convert/modules/__init__.py
+-rw-r--r--   0        0        0      331 2024-04-08 16:04:22.238325 markdown_convert-0.9.9/markdown_convert/modules/constants.py
+-rw-r--r--   0        0        0     4062 2024-04-08 21:48:34.445200 markdown_convert-0.9.9/markdown_convert/modules/convert.py
+-rw-r--r--   0        0        0     2266 2024-04-08 19:10:22.667055 markdown_convert-0.9.9/markdown_convert/modules/resources.py
+-rw-r--r--   0        0        0      316 2024-04-08 14:38:44.344993 markdown_convert-0.9.9/markdown_convert/modules/utils_strings.py
+-rw-r--r--   0        0        0     1487 2024-04-08 14:48:42.000577 markdown_convert-0.9.9/markdown_convert/modules/validate.py
+-rw-r--r--   0        0        0      658 2024-04-08 21:49:00.461550 markdown_convert-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2401 1970-01-01 00:00:00.000000 markdown_convert-0.9.9/PKG-INFO
```

### Comparing `markdown_convert-0.9.8/LICENSE` & `markdown_convert-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/README.md` & `markdown_convert-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/markdown_convert/__main__.py` & `markdown_convert-0.9.9/markdown_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/markdown_convert/code.css` & `markdown_convert-0.9.9/markdown_convert/code.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/markdown_convert/default.css` & `markdown_convert-0.9.9/markdown_convert/default.css`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/markdown_convert/modules/convert.py` & `markdown_convert-0.9.9/markdown_convert/modules/convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,19 +120,25 @@
 
         except KeyboardInterrupt:
             if self.loud:
                 print("\nInterrupted by user.\n", flush=True)
             return
 
 
-def live_convert(md_path, css_path, output_path):
+def live_convert(md_path, css_path=None, output_path=None):
     """
     Convert a markdown file to a pdf file and watch for changes.
 
     Args:
         md_path (str): Path to the markdown file.
-        css_path (str): Path to the CSS file.
-        output_path (str): Path to the output file.
+        css_path (str=None): Path to the CSS file.
+        output_path (str=None): Path to the output file.
     """
+    if css_path is None:
+        css_path = get_css_path()
+
+    if output_path is None:
+        output_path = get_output_path(md_path, None)
+
     live_converter = LiveConverter(md_path, css_path, output_path,
                                    loud=True)
     live_converter.observe()
```

### Comparing `markdown_convert-0.9.8/markdown_convert/modules/resources.py` & `markdown_convert-0.9.9/markdown_convert/modules/resources.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/markdown_convert/modules/validate.py` & `markdown_convert-0.9.9/markdown_convert/modules/validate.py`

 * *Files identical despite different names*

### Comparing `markdown_convert-0.9.8/pyproject.toml` & `markdown_convert-0.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "markdown_convert"
-version = "0.9.8"
+version = "0.9.9"
 description = "Convert Markdown files to PDF from your command line."
 authors = ["Julio Cabria <juliocabria@tutanota.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 homepage = "https://github.com/Julynx/markdown_convert"
 include = ["markdown_convert/default.css", "markdown_convert/code.css"]
```

### Comparing `markdown_convert-0.9.8/PKG-INFO` & `markdown_convert-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_convert
-Version: 0.9.8
+Version: 0.9.9
 Summary: Convert Markdown files to PDF from your command line.
 Home-page: https://github.com/Julynx/markdown_convert
 License: GPL-2.0-only
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

