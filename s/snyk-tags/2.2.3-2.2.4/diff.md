# Comparing `tmp/snyk_tags-2.2.3.tar.gz` & `tmp/snyk_tags-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snyk_tags-2.2.3.tar", max compression
+gzip compressed data, was "snyk_tags-2.2.4.tar", max compression
```

## Comparing `snyk_tags-2.2.3.tar` & `snyk_tags-2.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2156 2024-03-05 21:00:26.826986 snyk_tags-2.2.3/LICENSE.md
--rw-r--r--   0        0        0     9120 2024-03-05 21:00:26.826986 snyk_tags-2.2.3/docs/README.md
--rw-r--r--   0        0        0      834 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/pyproject.toml
--rw-r--r--   0        0        0      206 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/__init__.py
--rw-r--r--   0        0        0      157 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/__main__.py
--rw-r--r--   0        0        0     4305 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/attribute.py
--rw-r--r--   0        0        0     6811 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/collection.py
--rw-r--r--   0        0        0     8283 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/component.py
--rw-r--r--   0        0        0    10380 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/files.py
--rw-r--r--   0        0        0     9437 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/github.py
--rw-r--r--   0        0        0        0 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/lib/__init__.py
--rw-r--r--   0        0        0     2836 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/lib/api.py
--rw-r--r--   0        0        0       48 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/lib/component/rules/__init__.py
--rw-r--r--   0        0        0     1235 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/lib/component/rules/matcher.py
--rw-r--r--   0        0        0     2553 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/lib/component/rules/model.py
--rw-r--r--   0        0        0     4615 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/list.py
--rw-r--r--   0        0        0     8988 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/remove.py
--rw-r--r--   0        0        0    17920 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/tag.py
--rw-r--r--   0        0        0     2127 2024-03-05 21:00:26.830986 snyk_tags-2.2.3/snyk_tags/tags.py
--rw-r--r--   0        0        0    10414 1970-01-01 00:00:00.000000 snyk_tags-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2156 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/LICENSE.md
+-rw-r--r--   0        0        0     9120 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/docs/README.md
+-rw-r--r--   0        0        0      858 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0      206 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/__main__.py
+-rw-r--r--   0        0        0     4305 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/attribute.py
+-rw-r--r--   0        0        0     6811 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/collection.py
+-rw-r--r--   0        0        0     8283 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/component.py
+-rw-r--r--   0        0        0    10380 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/files.py
+-rw-r--r--   0        0        0     9437 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/github.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/lib/__init__.py
+-rw-r--r--   0        0        0     2836 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/lib/api.py
+-rw-r--r--   0        0        0       48 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/lib/component/rules/__init__.py
+-rw-r--r--   0        0        0     1235 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/lib/component/rules/matcher.py
+-rw-r--r--   0        0        0     2553 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/lib/component/rules/model.py
+-rw-r--r--   0        0        0     4615 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/list.py
+-rw-r--r--   0        0        0     8988 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/remove.py
+-rw-r--r--   0        0        0    17920 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/tag.py
+-rw-r--r--   0        0        0     2127 2024-04-09 13:31:40.835586 snyk_tags-2.2.4/snyk_tags/tags.py
+-rw-r--r--   0        0        0    10453 1970-01-01 00:00:00.000000 snyk_tags-2.2.4/PKG-INFO
```

### Comparing `snyk_tags-2.2.3/LICENSE.md` & `snyk_tags-2.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/docs/README.md` & `snyk_tags-2.2.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/pyproject.toml` & `snyk_tags-2.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snyk-tags"
-version = "2.2.3"
+version = "2.2.4"
 description = "CLI tool designed to manage tags and attributes at scale"
 authors = ["EricFernandezSnyk <eric.fernandez@snyk.io>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/snyk-labs/snyk-tags-tool"
 keywords =["snyk"]
 
@@ -22,14 +22,15 @@
 pysnyk = "^0.9.13"
 backoff = "^2.2.1"
 pyyaml = "^6.0.1"
 jsonschema = "^4"
 certifi = "2023.7.22"
 pygments = "2.15.0"
 requests = "2.31.0"
+cryptography = "42.0.4"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^6.0.0"
 pytest-httpx = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `snyk_tags-2.2.3/snyk_tags/attribute.py` & `snyk_tags-2.2.4/snyk_tags/attribute.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/collection.py` & `snyk_tags-2.2.4/snyk_tags/collection.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/component.py` & `snyk_tags-2.2.4/snyk_tags/component.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/files.py` & `snyk_tags-2.2.4/snyk_tags/files.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/github.py` & `snyk_tags-2.2.4/snyk_tags/github.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/lib/api.py` & `snyk_tags-2.2.4/snyk_tags/lib/api.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/lib/component/rules/matcher.py` & `snyk_tags-2.2.4/snyk_tags/lib/component/rules/matcher.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/lib/component/rules/model.py` & `snyk_tags-2.2.4/snyk_tags/lib/component/rules/model.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/list.py` & `snyk_tags-2.2.4/snyk_tags/list.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/remove.py` & `snyk_tags-2.2.4/snyk_tags/remove.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/tag.py` & `snyk_tags-2.2.4/snyk_tags/tag.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/snyk_tags/tags.py` & `snyk_tags-2.2.4/snyk_tags/tags.py`

 * *Files identical despite different names*

### Comparing `snyk_tags-2.2.3/PKG-INFO` & `snyk_tags-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snyk-tags
-Version: 2.2.3
+Version: 2.2.4
 Summary: CLI tool designed to manage tags and attributes at scale
 Home-page: https://github.com/snyk-labs/snyk-tags-tool
 License: MIT
 Keywords: snyk
 Author: EricFernandezSnyk
 Author-email: eric.fernandez@snyk.io
 Requires-Python: >=3.7,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyGithub (>=1.55,<2.0)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: certifi (==2023.7.22)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
+Requires-Dist: cryptography (==42.0.4)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: jsonschema (>=4,<5)
 Requires-Dist: pygments (==2.15.0)
 Requires-Dist: pysnyk (>=0.9.13,<0.10.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (>=10.11.0)
```

