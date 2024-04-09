# Comparing `tmp/chaturbate_poller-0.3.2.tar.gz` & `tmp/chaturbate_poller-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.3.2.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.3.3.tar", max compression
```

## Comparing `chaturbate_poller-0.3.2.tar` & `chaturbate_poller-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1071 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/LICENSE
--rw-r--r--   0        0        0     2692 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/README.md
--rw-r--r--   0        0        0     3129 2024-04-08 23:42:14.741685 chaturbate_poller-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      538 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     3838 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      669 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     2211 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     3441 2024-04-08 23:42:03.793641 chaturbate_poller-0.3.2/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2692 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/README.md
+-rw-r--r--   0        0        0     3129 2024-04-09 14:44:11.395914 chaturbate_poller-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      538 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     3838 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      669 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     2211 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     5578 2024-04-09 14:44:01.563545 chaturbate_poller-0.3.3/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 chaturbate_poller-0.3.3/PKG-INFO
```

### Comparing `chaturbate_poller-0.3.2/LICENSE` & `chaturbate_poller-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/README.md` & `chaturbate_poller-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/pyproject.toml` & `chaturbate_poller-0.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.3.2"
+version = "0.3.3"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.3.2/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.3.3/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/src/chaturbate_poller/chaturbate_poller.py` & `chaturbate_poller-0.3.3/src/chaturbate_poller/chaturbate_poller.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.3.3/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.3.3/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.3.2/PKG-INFO` & `chaturbate_poller-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.3.2
+Version: 0.3.3
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

