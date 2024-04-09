# Comparing `tmp/docker_inspector-0.1.5.tar.gz` & `tmp/docker_inspector-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_inspector-0.1.5.tar", max compression
+gzip compressed data, was "docker_inspector-0.1.6.tar", max compression
```

## Comparing `docker_inspector-0.1.5.tar` & `docker_inspector-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.5/docker_inspector/__init__.py
--rw-r--r--   0        0        0     1294 2024-04-09 12:30:54.917084 docker_inspector-0.1.5/docker_inspector/app.py
--rw-r--r--   0        0        0      187 2024-04-09 12:30:14.806720 docker_inspector-0.1.5/docker_inspector/styles/main.css
--rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.5/docker_inspector/widgets/__init__.py
--rw-r--r--   0        0        0     6897 2024-04-09 12:27:36.809824 docker_inspector-0.1.5/docker_inspector/widgets/container_list.py
--rw-r--r--   0        0        0      479 2024-04-09 12:36:48.908259 docker_inspector-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      689 2024-04-09 11:28:40.022961 docker_inspector-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-09 10:57:59.841162 docker_inspector-0.1.6/docker_inspector/__init__.py
+-rw-r--r--   0        0        0     1294 2024-04-09 12:42:19.181678 docker_inspector-0.1.6/docker_inspector/app.py
+-rw-r--r--   0        0        0      141 2024-04-09 12:42:08.220790 docker_inspector-0.1.6/docker_inspector/styles/main.css
+-rw-r--r--   0        0        0        0 2024-04-08 22:32:53.733342 docker_inspector-0.1.6/docker_inspector/widgets/__init__.py
+-rw-r--r--   0        0        0     6897 2024-04-09 12:27:36.809824 docker_inspector-0.1.6/docker_inspector/widgets/container_list.py
+-rw-r--r--   0        0        0      479 2024-04-09 12:42:58.696885 docker_inspector-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 docker_inspector-0.1.6/PKG-INFO
```

### Comparing `docker_inspector-0.1.5/README.md` & `docker_inspector-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.5/docker_inspector/app.py` & `docker_inspector-0.1.6/docker_inspector/app.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.5/docker_inspector/widgets/container_list.py` & `docker_inspector-0.1.6/docker_inspector/widgets/container_list.py`

 * *Files identical despite different names*

### Comparing `docker_inspector-0.1.5/PKG-INFO` & `docker_inspector-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-inspector
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

