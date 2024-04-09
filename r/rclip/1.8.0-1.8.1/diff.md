# Comparing `tmp/rclip-1.8.0.tar.gz` & `tmp/rclip-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rclip-1.8.0.tar", max compression
+gzip compressed data, was "rclip-1.8.1.tar", max compression
```

## Comparing `rclip-1.8.0.tar` & `rclip-1.8.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-04-09 08:37:51.278678 rclip-1.8.0/LICENSE
--rw-r--r--   0        0        0     7269 2024-04-09 08:37:51.278678 rclip-1.8.0/README.md
--rw-r--r--   0        0        0     1747 2024-04-09 08:37:51.282678 rclip-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      158 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/const.py
--rw-r--r--   0        0        0     3830 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/db.py
--rw-r--r--   0        0        0      993 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/fs.py
--rw-r--r--   0        0        0     7002 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/main.py
--rw-r--r--   0        0        0     5412 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/model.py
--rw-r--r--   0        0        0     7043 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/helpers.py
--rw-r--r--   0        0        0     1169 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/preview.py
--rw-r--r--   0        0        0     1726 2024-04-09 08:37:51.282678 rclip-1.8.0/rclip/utils/snap.py
--rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-09 09:05:38.267740 rclip-1.8.1/LICENSE
+-rw-r--r--   0        0        0     7269 2024-04-09 09:05:38.267740 rclip-1.8.1/README.md
+-rw-r--r--   0        0        0     1747 2024-04-09 09:05:38.267740 rclip-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/const.py
+-rw-r--r--   0        0        0     3830 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/db.py
+-rw-r--r--   0        0        0      993 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/fs.py
+-rw-r--r--   0        0        0     7002 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/main.py
+-rw-r--r--   0        0        0     5412 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/model.py
+-rw-r--r--   0        0        0     7043 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/utils/helpers.py
+-rw-r--r--   0        0        0     1169 2024-04-09 09:05:38.267740 rclip-1.8.1/rclip/utils/preview.py
+-rw-r--r--   0        0        0     1726 2024-04-09 09:05:38.271740 rclip-1.8.1/rclip/utils/snap.py
+-rw-r--r--   0        0        0     8911 1970-01-01 00:00:00.000000 rclip-1.8.1/PKG-INFO
```

### Comparing `rclip-1.8.0/LICENSE` & `rclip-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/README.md` & `rclip-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/pyproject.toml` & `rclip-1.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rclip"
-version = "1.8.0"
+version = "1.8.1"
 description = "AI-Powered Command-Line Photo Search Tool"
 authors = ["Yurij Mikhalevich <yurij@mikhalevi.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/yurijmikhalevich/rclip"
 keywords = ["image search", "computer vision", "photography"]
 classifiers = [
```

### Comparing `rclip-1.8.0/rclip/db.py` & `rclip-1.8.1/rclip/db.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/fs.py` & `rclip-1.8.1/rclip/fs.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/main.py` & `rclip-1.8.1/rclip/main.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/model.py` & `rclip-1.8.1/rclip/model.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/utils/helpers.py` & `rclip-1.8.1/rclip/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/utils/preview.py` & `rclip-1.8.1/rclip/utils/preview.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/rclip/utils/snap.py` & `rclip-1.8.1/rclip/utils/snap.py`

 * *Files identical despite different names*

### Comparing `rclip-1.8.0/PKG-INFO` & `rclip-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rclip
-Version: 1.8.0
+Version: 1.8.1
 Summary: AI-Powered Command-Line Photo Search Tool
 Home-page: https://github.com/yurijmikhalevich/rclip
 License: MIT
 Keywords: image search,computer vision,photography
 Author: Yurij Mikhalevich
 Author-email: yurij@mikhalevi.ch
 Requires-Python: >=3.9,<3.13
```

