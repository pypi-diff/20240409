# Comparing `tmp/devopsdriver-0.1.40.tar.gz` & `tmp/devopsdriver-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.40.tar", last modified: Sun Apr  7 15:42:17 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.41.tar", last modified: Mon Apr  8 22:44:00 2024, max compression
```

## Comparing `devopsdriver-0.1.40.tar` & `devopsdriver-0.1.41.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.480128 devopsdriver-0.1.40/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.40/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-07 15:42:17.479895 devopsdriver-0.1.40/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-07 15:40:12.000000 devopsdriver-0.1.40/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.476151 devopsdriver-0.1.40/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-07 15:40:04.000000 devopsdriver-0.1.40/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.477252 devopsdriver-0.1.40/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      423 2024-04-07 14:46:43.000000 devopsdriver-0.1.40/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     1882 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/azdo/clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.40/devopsdriver/azdo/timestamp.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.477724 devopsdriver-0.1.40/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2963 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     7792 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1658 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/azdo/workitem/workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.40/devopsdriver/manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.40/devopsdriver/settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.40/devopsdriver/template.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.478003 devopsdriver-0.1.40/devopsdriver/templates/
--rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.40/devopsdriver/templates/manage_settings.txt.mako
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.479304 devopsdriver-0.1.40/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      926 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/entry_points.txt
--rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-07 15:42:17.000000 devopsdriver-0.1.40/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1608 2024-04-06 22:25:43.000000 devopsdriver-0.1.40/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-07 15:42:17.480171 devopsdriver-0.1.40/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-07 15:42:17.479143 devopsdriver-0.1.40/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     5347 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     9547 2024-04-07 15:39:41.000000 devopsdriver-0.1.40/tests/test_azure_timestamp.py
--rw-r--r--   0 marcp      (501) staff       (20)     4736 2024-04-06 17:54:48.000000 devopsdriver-0.1.40/tests/test_azure_workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.40/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2391 2024-04-05 02:01:31.000000 devopsdriver-0.1.40/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.40/tests/test_manage_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.40/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.40/tests/test_settings.py
--rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.40/tests/test_template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881957 devopsdriver-0.1.41/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.41/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-08 22:44:00.881720 devopsdriver-0.1.41/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     8101 2024-04-08 22:36:24.000000 devopsdriver-0.1.41/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.878256 devopsdriver-0.1.41/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      216 2024-04-08 22:36:08.000000 devopsdriver-0.1.41/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879306 devopsdriver-0.1.41/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      434 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1882 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3777 2024-04-07 15:39:41.000000 devopsdriver-0.1.41/devopsdriver/azdo/timestamp.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879764 devopsdriver-0.1.41/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)       29 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2963 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     8771 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1658 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/azdo/workitem/workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1227 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     3002 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    12276 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1077 2024-04-06 21:50:31.000000 devopsdriver-0.1.41/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.879874 devopsdriver-0.1.41/devopsdriver/templates/
+-rw-r--r--   0 marcp      (501) staff       (20)      483 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/devopsdriver/templates/manage_settings.txt.mako
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881261 devopsdriver-0.1.41/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10951 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)      926 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       63 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/entry_points.txt
+-rw-r--r--   0 marcp      (501) staff       (20)      163 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-08 22:44:00.000000 devopsdriver-0.1.41/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1669 2024-04-08 16:56:00.000000 devopsdriver-0.1.41/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-08 22:44:00.881995 devopsdriver-0.1.41/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-08 22:44:00.881074 devopsdriver-0.1.41/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     5347 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     9547 2024-04-07 15:39:41.000000 devopsdriver-0.1.41/tests/test_azure_timestamp.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4736 2024-04-06 17:54:48.000000 devopsdriver-0.1.41/tests/test_azure_workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.41/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2881 2024-04-08 22:35:57.000000 devopsdriver-0.1.41/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2624 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/tests/test_manage_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4466 2024-04-06 20:27:22.000000 devopsdriver-0.1.41/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    10203 2024-04-06 22:13:48.000000 devopsdriver-0.1.41/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 20:14:20.000000 devopsdriver-0.1.41/tests/test_template.py
```

### Comparing `devopsdriver-0.1.40/LICENSE` & `devopsdriver-0.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/PKG-INFO` & `devopsdriver-0.1.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.40
+Version: 0.1.41
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -43,28 +43,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: keyring==25.0.0
-Requires-Dist: setuptools==69.0.2
+Requires-Dist: keyring==25.1.0
+Requires-Dist: setuptools==69.2.0
 Requires-Dist: azure-devops==7.1.0b4
 Requires-Dist: Mako==1.3.2
 Provides-Extra: dev
 Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.40&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.40/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.40/README.md` & `devopsdriver-0.1.41/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.40&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.40/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.40/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.41/devopsdriver/azdo/clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/azdo/timestamp.py` & `devopsdriver-0.1.41/devopsdriver/azdo/timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.41/devopsdriver/azdo/workitem/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.41/devopsdriver/azdo/workitem/wiql.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,23 +129,58 @@
     """Compare a field to a value"""
 
     def __init__(
         self,
         field: Field | str,
         value: Value | str | date | datetime | int | float,
         operator: str,
+        value_is_computed=False,
     ):
         self.left = field if isinstance(field, Field) else Field(field)
-        self.right = value if isinstance(value, Value) else Value(value)
+        self.right = (
+            value if value_is_computed or isinstance(value, Value) else Value(value)
+        )
         self.operator = operator
 
     def __str__(self) -> str:
         return f"{str(self.left)} {self.operator} {str(self.right)}"
 
 
+class In(Compare):  # pylint: disable=too-few-public-methods
+    """checks for field in a list of values"""
+
+    def __init__(
+        self,
+        field: Field | str,
+        *values: list[Value | str | date | datetime | int | float],
+    ):
+        super().__init__(
+            field,
+            f"({', '.join(str(v if isinstance(v, Value) else Value(v)) for v in values)})",
+            "IN",
+            value_is_computed=True,
+        )
+
+
+class NotIn(Compare):  # pylint: disable=too-few-public-methods
+    """checks for field in a list of values"""
+
+    def __init__(
+        self,
+        field: Field | str,
+        *values: list[Value | str | date | datetime | int | float],
+    ):
+        super().__init__(
+            field,
+            f"({', '.join(str(v if isinstance(v, Value) else Value(v)) for v in values)})",
+            "NOT IN",
+            value_is_computed=True,
+        )
+
+
 class Equal(Compare):  # pylint: disable=too-few-public-methods
     """checks for equality"""
 
     def __init__(
         self, field: Field | str, value: Value | str | date | datetime | int | float
     ):
         super().__init__(field, value, "=")
```

### Comparing `devopsdriver-0.1.40/devopsdriver/azdo/workitem/workitem.py` & `devopsdriver-0.1.41/devopsdriver/azdo/workitem/workitem.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/manage_settings.py` & `devopsdriver-0.1.41/devopsdriver/manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/sendmail.py` & `devopsdriver-0.1.41/devopsdriver/sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/settings.py` & `devopsdriver-0.1.41/devopsdriver/settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver/template.py` & `devopsdriver-0.1.41/devopsdriver/template.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/devopsdriver.egg-info/PKG-INFO` & `devopsdriver-0.1.41/devopsdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopsdriver
-Version: 0.1.40
+Version: 0.1.41
 Summary: DevOps tools
 Author-email: Marc Page <marcallenpage@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -43,28 +43,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: keyring==25.0.0
-Requires-Dist: setuptools==69.0.2
+Requires-Dist: keyring==25.1.0
+Requires-Dist: setuptools==69.2.0
 Requires-Dist: azure-devops==7.1.0b4
 Requires-Dist: Mako==1.3.2
 Provides-Extra: dev
 Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest>=8.1.1; extra == "test"
 Requires-Dist: coverage>=7.4.4; extra == "test"
 Provides-Extra: doc
 
 ![status sheild](https://img.shields.io/static/v1?label=status&message=beta&color=blue&style=plastic)
-[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.40&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.40/)
+[![status sheild](https://img.shields.io/static/v1?label=released&message=v0.1.41&color=active&style=plastic)](https://pypi.org/project/devopsdriver/0.1.41/)
 [![GitHub](https://img.shields.io/github/license/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver?tab=Unlicense-1-ov-file#readme)
 [![GitHub contributors](https://img.shields.io/github/contributors/marcpage/devops-driver?style=flat)](https://github.com/marcpage/devops-driver/graphs/contributors)
 [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)
 
 [![commit sheild](https://img.shields.io/github/last-commit/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![activity sheild](https://img.shields.io/github/commit-activity/m/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver/commits)
 [![GitHub top language](https://img.shields.io/github/languages/top/marcpage/devops-driver?style=plastic)](https://github.com/marcpage/devops-driver)
```

### Comparing `devopsdriver-0.1.40/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.41/devopsdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/pyproject.toml` & `devopsdriver-0.1.41/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 description = "DevOps tools"
 readme = "README.md"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 requires-python = ">= 3.10"
 dependencies = [
   "PyYAML==6.0.1",
-  "keyring==25.0.0",
-  "setuptools==69.0.2",  # neded for azure-devops to use 7.1 API
+  "keyring==25.1.0",
+  "setuptools==69.2.0",  # neded for azure-devops to use 7.1 API
   "azure-devops==7.1.0b4",
   "Mako==1.3.2",
 ]
 keywords = ["azure", "devops", "jira", "confluence", "email", "pipelines", "tools"]
 classifiers=[
     "Development Status :: 1 - Planning",
     "Environment :: Console",
@@ -30,14 +30,17 @@
 
 [project.scripts]
 settings = "devopsdriver.manage_settings:main"
 
 [tool.setuptools.package-data]
 "*" = ["*.mako"]
 
+[tool.setuptools.packages.find]
+include = ["devopsdriver*"]
+
 [project.optional-dependencies]
 dev = [
     "black>=24.3.0",
     "pylint>=3.1.0",
 ]
 test = [
     "pytest>=8.1.1",
```

### Comparing `devopsdriver-0.1.40/tests/test_azure_clients.py` & `devopsdriver-0.1.41/tests/test_azure_clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_azure_timestamp.py` & `devopsdriver-0.1.41/tests/test_azure_timestamp.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_azure_workitem.py` & `devopsdriver-0.1.41/tests/test_azure_workitem.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.41/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.41/tests/test_azure_workitem_wiql.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """ Test work item query language """
 
 from datetime import date, datetime
 
 from devopsdriver.azdo import Wiql
 from devopsdriver.azdo import Ascending, Descending, Value
-from devopsdriver.azdo import IsEmpty, IsNotEmpty, And, Or
+from devopsdriver.azdo import IsEmpty, IsNotEmpty, And, Or, In, NotIn
 from devopsdriver.azdo import GreaterThan, LessThan, Equal, NotEqual
 from devopsdriver.azdo import GreaterThanOrEqual, LessThanOrEqual
 
 
 def test_no_params() -> None:
     """Test empty, default wiql"""
     assert str(Wiql()) == "SELECT [System.Id] FROM workitems", str(Wiql())
@@ -61,11 +61,25 @@
     try:
         assert str(Value(test_no_params)) is None, str(Value(test_no_params))
 
     except AssertionError:
         pass
 
 
+def test_in_and_not_in() -> None:
+    """Test in and not in operators"""
+    builder = Wiql().where(
+        And(In("State", "New", "Ready for Development"), NotIn("Priority", 1, 2))
+    )
+    expected = (
+        """SELECT [System.Id] FROM workitems WHERE [System.State] """
+        + """IN ("New", "Ready for Development") AND [Microsoft.VSTS.Common.Priority] """
+        + """NOT IN (1, 2)"""
+    )
+    assert str(builder) == expected, str(builder)
+
+
 if __name__ == "__main__":
+    test_in_and_not_in()
     test_invalid_value_type()
     test_expressions()
     test_no_params()
```

### Comparing `devopsdriver-0.1.40/tests/test_manage_settings.py` & `devopsdriver-0.1.41/tests/test_manage_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_sendmail.py` & `devopsdriver-0.1.41/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_settings.py` & `devopsdriver-0.1.41/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.40/tests/test_template.py` & `devopsdriver-0.1.41/tests/test_template.py`

 * *Files identical despite different names*

