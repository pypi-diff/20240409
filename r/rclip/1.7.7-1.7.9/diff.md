# Comparing `tmp/rclip-1.7.7.tar.gz` & `tmp/rclip-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.7.7.tar", max compression
+gzip compressed data, was "rclip-1.7.9.tar", max compression
```

## Comparing `rclip-1.7.7.tar` & `rclip-1.7.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-01-13 11:59:29.157629 rclip-1.7.7/LICENSE
--rw-r--r--   0        0        0     7402 2024-01-13 11:59:29.157629 rclip-1.7.7/README.md
--rw-r--r--   0        0        0     1747 2024-01-13 11:59:29.161629 rclip-1.7.7/pyproject.toml
--rw-r--r--   0        0        0      158 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/const.py
--rw-r--r--   0        0        0     3830 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/db.py
--rw-r--r--   0        0        0      993 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/fs.py
--rw-r--r--   0        0        0     6655 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/model.py
--rw-r--r--   0        0        0     7043 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1153 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-01-13 11:59:29.161629 rclip-1.7.7/rclip/utils/snap.py
--rw-r--r--   0        0        0     9043 1970-01-01 00:00:00.000000 rclip-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-01-13 13:49:16.192258 rclip-1.7.9/LICENSE
+-rw-r--r--   0        0        0     7402 2024-01-13 13:49:16.192258 rclip-1.7.9/README.md
+-rw-r--r--   0        0        0     1747 2024-01-13 13:49:16.192258 rclip-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/const.py
+-rw-r--r--   0        0        0     3830 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/fs.py
+-rw-r--r--   0        0        0     6655 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/model.py
+-rw-r--r--   0        0        0     7043 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1153 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-01-13 13:49:16.192258 rclip-1.7.9/rclip/utils/snap.py
+-rw-r--r--   0        0        0     9043 1970-01-01 00:00:00.000000 rclip-1.7.9/PKG-INFO
```

### Comparing `rclip-1.7.7/LICENSE` & `rclip-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/README.md` & `rclip-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/pyproject.toml` & `rclip-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.7.7"
+version = "1.7.9"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.7.7/rclip/db.py` & `rclip-1.7.9/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/fs.py` & `rclip-1.7.9/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/main.py` & `rclip-1.7.9/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/model.py` & `rclip-1.7.9/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/utils/helpers.py` & `rclip-1.7.9/rclip/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/utils/preview.py` & `rclip-1.7.9/rclip/utils/preview.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/rclip/utils/snap.py` & `rclip-1.7.9/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.7.7/PKG-INFO` & `rclip-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.7.7
+Version: 1.7.9
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.8,<3.12
```

