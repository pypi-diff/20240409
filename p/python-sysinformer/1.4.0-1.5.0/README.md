# Comparing `tmp/python_sysinformer-1.4.0.tar.gz` & `tmp/python_sysinformer-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sysinformer-1.4.0.tar", max compression
+gzip compressed data, was "python_sysinformer-1.5.0.tar", max compression
```

## Comparing `python_sysinformer-1.4.0.tar` & `python_sysinformer-1.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-09 07:30:00.598635 python_sysinformer-1.4.0/LICENSE
--rw-r--r--   0        0        0     5341 2024-04-09 07:30:00.598635 python_sysinformer-1.4.0/README.md
--rw-r--r--   0        0        0     1593 2024-04-09 07:30:27.818693 python_sysinformer-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/config/__init__.py
--rw-r--r--   0        0        0     1102 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/config/config_parser.py
--rw-r--r--   0        0        0     1233 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/config/default_config.py
--rw-r--r--   0        0        0      221 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/constants.py
--rw-r--r--   0        0        0        0 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/containers.py
--rw-r--r--   0        0        0     5666 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/cpu.py
--rw-r--r--   0        0        0     2041 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/disks.py
--rw-r--r--   0        0        0     3745 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/latency.py
--rw-r--r--   0        0        0     2739 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/memory.py
--rw-r--r--   0        0        0     2597 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/networking.py
--rw-r--r--   0        0        0     2764 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/processes.py
--rw-r--r--   0        0        0     2605 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/services.py
--rw-r--r--   0        0        0     4035 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/core/system.py
--rw-r--r--   0        0        0     4417 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/main.py
--rw-r--r--   0        0        0        0 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/utilities/__init__.py
--rw-r--r--   0        0        0      442 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/utilities/exceptions.py
--rw-r--r--   0        0        0      560 2024-04-09 07:30:00.602635 python_sysinformer-1.4.0/src/utilities/utils.py
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 python_sysinformer-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 19:13:21.563897 python_sysinformer-1.5.0/LICENSE
+-rw-r--r--   0        0        0     5341 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/README.md
+-rw-r--r--   0        0        0     1593 2024-04-09 19:13:48.107782 python_sysinformer-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/__init__.py
+-rw-r--r--   0        0        0     1102 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/config_parser.py
+-rw-r--r--   0        0        0     1233 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/default_config.py
+-rw-r--r--   0        0        0      221 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/constants.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/containers.py
+-rw-r--r--   0        0        0     5666 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/cpu.py
+-rw-r--r--   0        0        0     2041 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/disks.py
+-rw-r--r--   0        0        0     3745 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/latency.py
+-rw-r--r--   0        0        0     4335 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/memory.py
+-rw-r--r--   0        0        0     2597 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/networking.py
+-rw-r--r--   0        0        0     2764 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/processes.py
+-rw-r--r--   0        0        0     2605 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/services.py
+-rw-r--r--   0        0        0     4035 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/system.py
+-rw-r--r--   0        0        0     4417 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/exceptions.py
+-rw-r--r--   0        0        0      560 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/utils.py
+-rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 python_sysinformer-1.5.0/PKG-INFO
```

### Comparing `python_sysinformer-1.4.0/LICENSE` & `python_sysinformer-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/README.md` & `python_sysinformer-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/pyproject.toml` & `python_sysinformer-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-SysInformer"
-version = "1.4.0"
+version = "1.5.0"
 description = "A simple system information tool for Linux"
 authors = ["Timothy Bryant <timothybryant3@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src", from = "."}]
 # classifiers = ["Private :: Do not Upload"]
 
 [tool.poetry.dependencies]
```

### Comparing `python_sysinformer-1.4.0/src/config/config_parser.py` & `python_sysinformer-1.5.0/src/config/config_parser.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/config/default_config.py` & `python_sysinformer-1.5.0/src/config/default_config.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/containers.py` & `python_sysinformer-1.5.0/src/core/containers.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/cpu.py` & `python_sysinformer-1.5.0/src/core/cpu.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/disks.py` & `python_sysinformer-1.5.0/src/core/disks.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/latency.py` & `python_sysinformer-1.5.0/src/core/latency.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/networking.py` & `python_sysinformer-1.5.0/src/core/networking.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/processes.py` & `python_sysinformer-1.5.0/src/core/processes.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/services.py` & `python_sysinformer-1.5.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/core/system.py` & `python_sysinformer-1.5.0/src/core/system.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/main.py` & `python_sysinformer-1.5.0/src/main.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/src/utilities/utils.py` & `python_sysinformer-1.5.0/src/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.4.0/PKG-INFO` & `python_sysinformer-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sysinformer
-Version: 1.4.0
+Version: 1.5.0
 Summary: A simple system information tool for Linux
 Author: Timothy Bryant
 Author-email: timothybryant3@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

