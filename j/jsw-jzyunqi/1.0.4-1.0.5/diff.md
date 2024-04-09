# Comparing `tmp/jsw_jzyunqi-1.0.4.tar.gz` & `tmp/jsw_jzyunqi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsw_jzyunqi-1.0.4.tar", max compression
+gzip compressed data, was "jsw_jzyunqi-1.0.5.tar", max compression
```

## Comparing `jsw_jzyunqi-1.0.4.tar` & `jsw_jzyunqi-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.4/README.md
--rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.4/jsw_jzyunqi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/__init__.py
--rw-r--r--   0        0        0     2420 2024-04-08 03:32:05.313865 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/publish_article.py
--rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/settings.py
--rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/spider_auth.py
--rw-r--r--   0        0        0      447 2024-04-08 03:32:17.313625 jsw_jzyunqi-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      188 2024-04-08 02:55:52.224430 jsw_jzyunqi-1.0.5/README.md
+-rw-r--r--   0        0        0      174 2024-04-08 02:36:08.077700 jsw_jzyunqi-1.0.5/jsw_jzyunqi/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.5/jsw_jzyunqi/gzip/__init__.py
+-rw-r--r--   0        0        0     2558 2024-04-09 05:46:17.887895 jsw_jzyunqi-1.0.5/jsw_jzyunqi/gzip/gz.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:31:23.925330 jsw_jzyunqi-1.0.5/jsw_jzyunqi/mbw/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-08 03:32:05.313865 jsw_jzyunqi-1.0.5/jsw_jzyunqi/mbw/publish_article.py
+-rw-r--r--   0        0        0       90 2024-04-08 02:41:02.347157 jsw_jzyunqi-1.0.5/jsw_jzyunqi/mbw/settings.py
+-rw-r--r--   0        0        0      438 2024-04-08 02:41:10.685917 jsw_jzyunqi-1.0.5/jsw_jzyunqi/mbw/spider_auth.py
+-rw-r--r--   0        0        0      484 2024-04-09 05:47:02.057467 jsw_jzyunqi-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      906 1970-01-01 00:00:00.000000 jsw_jzyunqi-1.0.5/PKG-INFO
```

### Comparing `jsw_jzyunqi-1.0.4/jsw_jzyunqi/mbw/publish_article.py` & `jsw_jzyunqi-1.0.5/jsw_jzyunqi/mbw/publish_article.py`

 * *Files identical despite different names*

### Comparing `jsw_jzyunqi-1.0.4/PKG-INFO` & `jsw_jzyunqi-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: jsw-jzyunqi
-Version: 1.0.4
+Version: 1.0.5
 Summary: python tools for jzyunqi.
 Home-page: https://js.work
 Author: aric
 Author-email: 1290657123@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyzipper (>=0.3.6,<0.4.0)
+Requires-Dist: rarfile (>=4.2,<5.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/aric-pypi/jsw-jzyunqi
 Description-Content-Type: text/markdown
 
 # jsw-jzyunqi
 > python tools for jzyunqi.
```

