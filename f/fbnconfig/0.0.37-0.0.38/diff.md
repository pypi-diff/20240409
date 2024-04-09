# Comparing `tmp/fbnconfig-0.0.37.tar.gz` & `tmp/fbnconfig-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fbnconfig-0.0.37.tar", max compression
+gzip compressed data, was "fbnconfig-0.0.38.tar", max compression
```

## Comparing `fbnconfig-0.0.37.tar` & `fbnconfig-0.0.38.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      176 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/__init__.py
--rw-r--r--   0        0        0     6600 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/access.py
--rw-r--r--   0        0        0     6513 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/configuration.py
--rw-r--r--   0        0        0     4113 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/deploy.py
--rw-r--r--   0        0        0     8124 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/drive.py
--rw-r--r--   0        0        0     7488 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/identity.py
--rw-r--r--   0        0        0     1057 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig/load_module.py
--rw-r--r--   0        0        0     9681 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/log.py
--rw-r--r--   0        0        0     8126 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/main.py
--rw-r--r--   0        0        0      771 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/resource_abc.py
--rw-r--r--   0        0        0    14708 2024-04-08 09:05:30.818543 fbnconfig-0.0.37/fbnconfig/scheduler.py
--rw-r--r--   0        0        0     8107 2024-04-08 09:05:30.817543 fbnconfig-0.0.37/fbnconfig.md
--rw-r--r--   0        0        0     1070 2024-04-08 09:09:43.374110 fbnconfig-0.0.37/pyproject.toml
--rw-r--r--   0        0        0     8639 1970-01-01 00:00:00.000000 fbnconfig-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/access.py
+-rw-r--r--   0        0        0     6513 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/configuration.py
+-rw-r--r--   0        0        0     4167 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/deploy.py
+-rw-r--r--   0        0        0     8124 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/drive.py
+-rw-r--r--   0        0        0     7488 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/identity.py
+-rw-r--r--   0        0        0     1057 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/load_module.py
+-rw-r--r--   0        0        0     9681 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/log.py
+-rw-r--r--   0        0        0     8126 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/main.py
+-rw-r--r--   0        0        0     6618 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/property.py
+-rw-r--r--   0        0        0      771 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/resource_abc.py
+-rw-r--r--   0        0        0    14708 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig/scheduler.py
+-rw-r--r--   0        0        0     8107 2024-04-09 09:55:16.000000 fbnconfig-0.0.38/fbnconfig.md
+-rw-r--r--   0        0        0     1070 2024-04-09 09:58:52.151540 fbnconfig-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0     8639 1970-01-01 00:00:00.000000 fbnconfig-0.0.38/PKG-INFO
```

### Comparing `fbnconfig-0.0.37/fbnconfig/access.py` & `fbnconfig-0.0.38/fbnconfig/access.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/configuration.py` & `fbnconfig-0.0.38/fbnconfig/configuration.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/deploy.py` & `fbnconfig-0.0.38/fbnconfig/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # import all resources here, so they are available in globals()
 from .drive import FolderResource, FileResource  # noqa: F401
 from .scheduler import ImageResource, JobResource, ScheduleResource  # noqa: F401
 from .access import PolicyResource, RoleResource  # noqa: F401
 from .identity import IdentityRoleResource, UserResource, RoleAssignment  # noqa: F401
 from .configuration import SetResource, ItemResource # noqa: F401
+from .property import DefinitionResource # noqa: F401
 
 Deployment = NamedTuple("Deployment", [("id", str), ("resources", List[Union[Resource, Ref]])])
 deployments = []
 
 
 def deployment(id, resources):
     d = Deployment(id, resources)
```

### Comparing `fbnconfig-0.0.37/fbnconfig/drive.py` & `fbnconfig-0.0.38/fbnconfig/drive.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/identity.py` & `fbnconfig-0.0.38/fbnconfig/identity.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/load_module.py` & `fbnconfig-0.0.38/fbnconfig/load_module.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/log.py` & `fbnconfig-0.0.38/fbnconfig/log.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/main.py` & `fbnconfig-0.0.38/fbnconfig/main.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/resource_abc.py` & `fbnconfig-0.0.38/fbnconfig/resource_abc.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig/scheduler.py` & `fbnconfig-0.0.38/fbnconfig/scheduler.py`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/fbnconfig.md` & `fbnconfig-0.0.38/fbnconfig.md`

 * *Files identical despite different names*

### Comparing `fbnconfig-0.0.37/pyproject.toml` & `fbnconfig-0.0.38/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fbnconfig"
-version = "0.0.37"
+version = "0.0.38"
 description = "fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment"
 authors = ["FINBOURNE Technology <engineering@finbourne.com>"]
 readme = "fbnconfig.md"
 
 [tool.poetry.scripts]
 fbnconfig = 'fbnconfig.main:cli'
```

### Comparing `fbnconfig-0.0.37/PKG-INFO` & `fbnconfig-0.0.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbnconfig
-Version: 0.0.37
+Version: 0.0.38
 Summary: fbnconfig is a python library (and commandline tool) to allow a declarative description of a LUSID environment
 Author: FINBOURNE Technology
 Author-email: engineering@finbourne.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

