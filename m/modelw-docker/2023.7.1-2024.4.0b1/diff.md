# Comparing `tmp/modelw_docker-2023.7.1.tar.gz` & `tmp/modelw_docker-2024.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2023.7.1.tar", max compression
+gzip compressed data, was "modelw_docker-2024.4.0b1.tar", max compression
```

## Comparing `modelw_docker-2023.7.1.tar` & `modelw_docker-2024.4.0b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2023-07-13 07:57:58.042105 modelw_docker-2023.7.1/LICENSE
--rw-r--r--   0        0        0     4666 2023-07-13 07:57:58.042105 modelw_docker-2023.7.1/README.md
--rw-r--r--   0        0        0     1199 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1494 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5229 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5865 2023-07-13 07:57:58.046105 modelw_docker-2023.7.1/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 modelw_docker-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0      484 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/LICENSE
+-rw-r--r--   0        0        0     4666 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/README.md
+-rw-r--r--   0        0        0     1201 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5810 1970-01-01 00:00:00.000000 modelw_docker-2024.4.0b1/PKG-INFO
```

### Comparing `modelw_docker-2023.7.1/README.md` & `modelw_docker-2024.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/pyproject.toml` & `modelw_docker-2024.4.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2023.7.1"
+version = "2024.4.0b1"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
 homepage = "https://github.com/ModelW/docker/"
 keywords = ["docker", "django", "nuxt", "dockerfile"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Utilities",
     "Framework :: Django",
     "Framework :: Wagtail",
 ]
 
 [tool.poetry.scripts]
 modelw-docker = "model_w.docker.__main__:__main__"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 setuptools = "*"
-psutil = "^5.9.4"
+psutil = "^5.9.5"
 colorama = "^0.4.6"
-tomli = { version = "^2.0.1", python = "<3.11" }
-typefit = "^0.4.2"
+tomli = { version = "^2.0.1", python = "<3.12" }
+typefit = "^0.5.5"
 
 
 [tool.poetry.group.dev.dependencies]
 monoformat = "^0.1.0b3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/__main__.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/build.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/build.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/config.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/install.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/install.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/output.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/platform.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/run.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/src/model_w/docker/serve.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/serve.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2023.7.1/PKG-INFO` & `modelw_docker-2024.4.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2023.7.1
+Version: 2024.4.0b1
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Framework :: Wagtail
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: setuptools
-Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
-Requires-Dist: typefit (>=0.4.2,<0.5.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.12"
+Requires-Dist: typefit (>=0.5.5,<0.6.0)
 Project-URL: Documentation, https://github.com/ModelW/docker/
 Project-URL: Repository, https://github.com/ModelW/docker/
 Description-Content-Type: text/markdown
 
 # Model W Docker
 
 A tool so that your Dockerfile looks like this:
```

