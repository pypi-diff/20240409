# Comparing `tmp/honeycomb_opentelemetry-0.4.0b0.tar.gz` & `tmp/honeycomb_opentelemetry-0.4.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeycomb_opentelemetry-0.4.0b0.tar", max compression
+gzip compressed data, was "honeycomb_opentelemetry-0.4.1b0.tar", max compression
```

## Comparing `honeycomb_opentelemetry-0.4.0b0.tar` & `honeycomb_opentelemetry-0.4.1b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-07 17:08:06.551852 honeycomb_opentelemetry-0.4.0b0/LICENSE
--rw-r--r--   0        0        0     1698 2024-03-07 17:08:06.551852 honeycomb_opentelemetry-0.4.0b0/README.md
--rw-r--r--   0        0        0     1305 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/pyproject.toml
--rw-r--r--   0        0        0      128 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/__init__.py
--rw-r--r--   0        0        0     1416 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/baggage.py
--rw-r--r--   0        0        0     2750 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/distro.py
--rw-r--r--   0        0        0     3161 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/local_exporter.py
--rw-r--r--   0        0        0     1664 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/metrics.py
--rw-r--r--   0        0        0    15746 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/options.py
--rw-r--r--   0        0        0      842 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/resource.py
--rw-r--r--   0        0        0     3266 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/sampler.py
--rw-r--r--   0        0        0     2223 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/trace.py
--rw-r--r--   0        0        0      101 2024-03-07 17:08:06.555853 honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/version.py
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.4.0b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-09 17:54:24.213929 honeycomb_opentelemetry-0.4.1b0/LICENSE
+-rw-r--r--   0        0        0     1698 2024-04-09 17:54:24.213929 honeycomb_opentelemetry-0.4.1b0/README.md
+-rw-r--r--   0        0        0     1309 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/baggage.py
+-rw-r--r--   0        0        0     2750 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/distro.py
+-rw-r--r--   0        0        0     3161 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/local_exporter.py
+-rw-r--r--   0        0        0     1664 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/metrics.py
+-rw-r--r--   0        0        0    15746 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/options.py
+-rw-r--r--   0        0        0      842 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/resource.py
+-rw-r--r--   0        0        0     3266 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/sampler.py
+-rw-r--r--   0        0        0     2223 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/trace.py
+-rw-r--r--   0        0        0      101 2024-04-09 17:54:24.217929 honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/version.py
+-rw-r--r--   0        0        0     2666 1970-01-01 00:00:00.000000 honeycomb_opentelemetry-0.4.1b0/PKG-INFO
```

### Comparing `honeycomb_opentelemetry-0.4.0b0/LICENSE` & `honeycomb_opentelemetry-0.4.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/README.md` & `honeycomb_opentelemetry-0.4.1b0/README.md`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/pyproject.toml` & `honeycomb_opentelemetry-0.4.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "honeycomb-opentelemetry"
-version = "0.4.0b0"
+version = "0.4.1b0"
 description = "Honeycomb OpenTelemetry Distro for Python"
 authors = ["Honeycomb <support@honeycomb.io>"]
 readme = "README.md"
 packages = [{include = "honeycomb", from = "src" }]
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -17,18 +17,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7, >= 3.7.2"
-opentelemetry-api = "1.22.0"
-opentelemetry-sdk = "1.22.0"
-opentelemetry-exporter-otlp = "1.22.0"
-opentelemetry-instrumentation = "0.43b0"
+opentelemetry-api = "^1.22.0"
+opentelemetry-sdk = "^1.22.0"
+opentelemetry-exporter-otlp = "^1.22.0"
+opentelemetry-instrumentation = "~0.43b0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = ">=6.5,<8.0"
 pytest = "^7.2.0"
 pylint = "^2.16.0"
 pycodestyle = "^2.10.0"
 importlib-metadata = { version = ">=0.12", python = "<3.8" }
```

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/baggage.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/baggage.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/distro.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/distro.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/local_exporter.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/local_exporter.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/metrics.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/options.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/options.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/resource.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/resource.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/sampler.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/sampler.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/src/honeycomb/opentelemetry/trace.py` & `honeycomb_opentelemetry-0.4.1b0/src/honeycomb/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `honeycomb_opentelemetry-0.4.0b0/PKG-INFO` & `honeycomb_opentelemetry-0.4.1b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeycomb-opentelemetry
-Version: 0.4.0b0
+Version: 0.4.1b0
 Summary: Honeycomb OpenTelemetry Distro for Python
 License: Apache-2.0
 Author: Honeycomb
 Author-email: support@honeycomb.io
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Typing :: Typed
-Requires-Dist: opentelemetry-api (==1.22.0)
-Requires-Dist: opentelemetry-exporter-otlp (==1.22.0)
-Requires-Dist: opentelemetry-instrumentation (==0.43b0)
-Requires-Dist: opentelemetry-sdk (==1.22.0)
+Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp (>=1.22.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (>=0.43b0,<0.44)
+Requires-Dist: opentelemetry-sdk (>=1.22.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Honeycomb OpenTelemetry Distro for Python
 
 [![OSS Lifecycle](https://img.shields.io/osslifecycle/honeycombio/honeycomb-opentelemetry-python)](https://github.com/honeycombio/home/blob/main/honeycomb-oss-lifecycle-and-practices.md)
 [![CircleCI](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python.svg?style=shield)](https://circleci.com/gh/honeycombio/honeycomb-opentelemetry-python)
 [![PyPi](https://img.shields.io/pypi/v/honeycomb-opentelemetry)](https://pypi.org/project/honeycomb-opentelemetry/)
```

