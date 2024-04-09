# Comparing `tmp/fitrequest-0.7.0.tar.gz` & `tmp/fitrequest-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitrequest-0.7.0.tar", max compression
+gzip compressed data, was "fitrequest-0.7.1.tar", max compression
```

## Comparing `fitrequest-0.7.0.tar` & `fitrequest-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-08 15:50:28.676231 fitrequest-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     7207 2024-04-08 15:50:28.676231 fitrequest-0.7.0/README.md
--rw-r--r--   0        0        0    10174 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/client.py
--rw-r--r--   0        0        0     4947 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/method_generator.py
--rw-r--r--   0        0        0     2701 2024-04-08 15:50:28.676231 fitrequest-0.7.0/fitrequest/utils.py
--rw-r--r--   0        0        0     1350 2024-04-08 15:50:28.680231 fitrequest-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     8290 1970-01-01 00:00:00.000000 fitrequest-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-09 08:57:23.290626 fitrequest-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0     7207 2024-04-09 08:57:23.290626 fitrequest-0.7.1/README.md
+-rw-r--r--   0        0        0    10211 2024-04-09 08:57:23.290626 fitrequest-0.7.1/fitrequest/client.py
+-rw-r--r--   0        0        0     4947 2024-04-09 08:57:23.290626 fitrequest-0.7.1/fitrequest/method_generator.py
+-rw-r--r--   0        0        0     2701 2024-04-09 08:57:23.290626 fitrequest-0.7.1/fitrequest/utils.py
+-rw-r--r--   0        0        0     1350 2024-04-09 08:57:23.290626 fitrequest-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     8290 1970-01-01 00:00:00.000000 fitrequest-0.7.1/PKG-INFO
```

### Comparing `fitrequest-0.7.0/LICENSE.md` & `fitrequest-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.0/README.md` & `fitrequest-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.0/fitrequest/client.py` & `fitrequest-0.7.1/fitrequest/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 
     def __init__(
         self, username=None, password=None, response_log_level=None, *args, **kwargs
     ):
         self.base_url = self.base_url or os.environ['CLIENT_BASE_URL']
         self.response_log_level = response_log_level
         if all((AWS_CREDENTIALS, kwargs.get('credentials_from_aws'))):
-            default_secret_path = f"/{self.env or ''}/{self.base_client_name.lower()}"
+            default_secret_path = (
+                f"{f'/{self.env}' or ''}/{self.base_client_name.lower()}"
+            )
             username = (
                 username
                 or AWSSecret(
                     **kwargs.get(
                         'username_secret',
                         {'type': 'ssm', 'path': f'{default_secret_path}/username'},
                     )
```

### Comparing `fitrequest-0.7.0/fitrequest/method_generator.py` & `fitrequest-0.7.1/fitrequest/method_generator.py`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.0/fitrequest/utils.py` & `fitrequest-0.7.1/fitrequest/utils.py`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.0/pyproject.toml` & `fitrequest-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fitrequest"
-version = "0.7.0"
+version = "0.7.1"
 description = "Python class that allow to create client for REST API with dynamic code generation"
 homepage = "https://skillcorner.com/"
 repository = "https://gitlab.com/public-corner/fitrequest"
 documentation = "https://fitrequest.readthedocs.io/en/latest/"
 authors = ["Skillcorner"]
 readme = "README.md"
```

### Comparing `fitrequest-0.7.0/PKG-INFO` & `fitrequest-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitrequest
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python class that allow to create client for REST API with dynamic code generation
 Home-page: https://skillcorner.com/
 Author: Skillcorner
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

