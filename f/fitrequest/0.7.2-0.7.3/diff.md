# Comparing `tmp/fitrequest-0.7.2.tar.gz` & `tmp/fitrequest-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitrequest-0.7.2.tar", max compression
+gzip compressed data, was "fitrequest-0.7.3.tar", max compression
```

## Comparing `fitrequest-0.7.2.tar` & `fitrequest-0.7.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-09 13:38:40.946681 fitrequest-0.7.2/LICENSE.md
--rw-r--r--   0        0        0     7207 2024-04-09 13:38:40.946681 fitrequest-0.7.2/README.md
--rw-r--r--   0        0        0    10190 2024-04-09 13:38:40.946681 fitrequest-0.7.2/fitrequest/client.py
--rw-r--r--   0        0        0     4947 2024-04-09 13:38:40.946681 fitrequest-0.7.2/fitrequest/method_generator.py
--rw-r--r--   0        0        0     2701 2024-04-09 13:38:40.946681 fitrequest-0.7.2/fitrequest/utils.py
--rw-r--r--   0        0        0     1350 2024-04-09 13:38:40.950681 fitrequest-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     8290 1970-01-01 00:00:00.000000 fitrequest-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-09 15:51:38.413096 fitrequest-0.7.3/LICENSE.md
+-rw-r--r--   0        0        0     7207 2024-04-09 15:51:38.413096 fitrequest-0.7.3/README.md
+-rw-r--r--   0        0        0    10122 2024-04-09 15:51:38.413096 fitrequest-0.7.3/fitrequest/client.py
+-rw-r--r--   0        0        0     4947 2024-04-09 15:51:38.413096 fitrequest-0.7.3/fitrequest/method_generator.py
+-rw-r--r--   0        0        0     2701 2024-04-09 15:51:38.413096 fitrequest-0.7.3/fitrequest/utils.py
+-rw-r--r--   0        0        0     1350 2024-04-09 15:51:38.413096 fitrequest-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     8290 1970-01-01 00:00:00.000000 fitrequest-0.7.3/PKG-INFO
```

### Comparing `fitrequest-0.7.2/LICENSE.md` & `fitrequest-0.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.2/README.md` & `fitrequest-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.2/fitrequest/client.py` & `fitrequest-0.7.3/fitrequest/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,39 +39,37 @@
 class FitRequest(metaclass=_MethodsGenerator):
     _docstring_template: Optional[str] = None
     _methods_binding: Optional[List[dict]] = None
     _retry: Optional[Retry] = None
     _session: Optional[Session] = None
     base_client_name: str
     base_url: Optional[str] = None
+    default_secret_path: Optional[str] = None
 
     def __init__(
         self, username=None, password=None, response_log_level=None, *args, **kwargs
     ):
         self.base_url = self.base_url or os.environ['CLIENT_BASE_URL']
         self.response_log_level = response_log_level
         if all((AWS_CREDENTIALS, kwargs.get('credentials_from_aws'))):
-            default_secret_path = (
-                f"{f'/{self.env}' or ''}/{self.base_client_name.lower()}"
-            )
             username = (
                 username
                 or AWSSecret(
                     **kwargs.get(
                         'username_secret',
-                        {'type': 'ssm', 'path': f'{default_secret_path}/username'},
+                        {'type': 'ssm', 'path': f'{self.default_secret_path}/username'},
                     )
                 ).value
             )
             password = AWSSecret(
                 **kwargs.get(
                     'password_secret',
                     {
                         'type': 'secretsmanager',
-                        'path': f'{default_secret_path}/password',
+                        'path': f'{self.default_secret_path}/password',
                     },
                 )
             ).value
         else:
             username = username or os.environ.get(
                 f'{self.base_client_name.upper()}_USERNAME', ''
             )
```

### Comparing `fitrequest-0.7.2/fitrequest/method_generator.py` & `fitrequest-0.7.3/fitrequest/method_generator.py`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.2/fitrequest/utils.py` & `fitrequest-0.7.3/fitrequest/utils.py`

 * *Files identical despite different names*

### Comparing `fitrequest-0.7.2/pyproject.toml` & `fitrequest-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fitrequest"
-version = "0.7.2"
+version = "0.7.3"
 description = "Python class that allow to create client for REST API with dynamic code generation"
 homepage = "https://skillcorner.com/"
 repository = "https://gitlab.com/public-corner/fitrequest"
 documentation = "https://fitrequest.readthedocs.io/en/latest/"
 authors = ["Skillcorner"]
 readme = "README.md"
```

### Comparing `fitrequest-0.7.2/PKG-INFO` & `fitrequest-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitrequest
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python class that allow to create client for REST API with dynamic code generation
 Home-page: https://skillcorner.com/
 Author: Skillcorner
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

