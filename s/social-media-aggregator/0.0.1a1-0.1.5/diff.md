# Comparing `tmp/social_media_aggregator-0.0.1a1.tar.gz` & `tmp/social_media_aggregator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_media_aggregator-0.0.1a1.tar", max compression
+gzip compressed data, was "social_media_aggregator-0.1.5.tar", max compression
```

## Comparing `social_media_aggregator-0.0.1a1.tar` & `social_media_aggregator-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-07 10:36:29.856145 social_media_aggregator-0.0.1a1/LICENSE
--rw-r--r--   0        0        0      608 2024-04-09 12:06:08.539860 social_media_aggregator-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 23:10:55.495484 social_media_aggregator-0.0.1a1/src/social_media_aggregator/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 23:10:55.495537 social_media_aggregator-0.0.1a1/src/social_media_aggregator/exceptions/__init__.py
--rw-r--r--   0        0        0      743 2024-04-09 12:06:08.540350 social_media_aggregator-0.0.1a1/src/social_media_aggregator/exceptions/logger.py
--rw-r--r--   0        0        0     1005 2024-04-09 12:06:08.540564 social_media_aggregator-0.0.1a1/src/social_media_aggregator/exceptions/meta.py
--rw-r--r--   0        0        0     1689 2024-04-09 12:06:08.540807 social_media_aggregator-0.0.1a1/src/social_media_aggregator/helpers/helpers.py
--rw-r--r--   0        0        0     1755 2024-04-09 12:06:08.541383 social_media_aggregator-0.0.1a1/src/social_media_aggregator/logger.py
--rw-r--r--   0        0        0     5858 2024-04-09 12:06:08.541710 social_media_aggregator-0.0.1a1/src/social_media_aggregator/meta.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 social_media_aggregator-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-07 10:36:29.856145 social_media_aggregator-0.1.5/LICENSE
+-rw-r--r--   0        0        0      603 2024-04-07 23:10:55.493472 social_media_aggregator-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 23:10:55.495484 social_media_aggregator-0.1.5/src/social_media_aggregator/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 23:10:55.495537 social_media_aggregator-0.1.5/src/social_media_aggregator/exceptions/__init__.py
+-rw-r--r--   0        0        0      519 2024-04-09 12:05:27.245285 social_media_aggregator-0.1.5/src/social_media_aggregator/exceptions/logger.py
+-rw-r--r--   0        0        0     1178 2024-04-09 12:05:27.246126 social_media_aggregator-0.1.5/src/social_media_aggregator/exceptions/meta.py
+-rw-r--r--   0        0        0     1888 2024-04-09 12:05:27.246637 social_media_aggregator-0.1.5/src/social_media_aggregator/logger.py
+-rw-r--r--   0        0        0     3652 2024-04-09 12:05:27.247438 social_media_aggregator-0.1.5/src/social_media_aggregator/meta.py
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 social_media_aggregator-0.1.5/PKG-INFO
```

### Comparing `social_media_aggregator-0.0.1a1/LICENSE` & `social_media_aggregator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `social_media_aggregator-0.0.1a1/pyproject.toml` & `social_media_aggregator-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "social_media_aggregator"
-version = "0.0.1a1"
+version = "0.1.5"
 
 [tool.setuptools]
 packages = { find = { where = ["src"] } }
 
 [tool.poetry]
 name = "social_media_aggregator"
-version = "0.0.1a1"
+version = "0.1.5"
 description = "This is a project that aggregates several social media accounts into a single space"
 authors = ["José Viegas <jviegas6@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest-cov = "^5.0.0"
-# Add your development dependencies here
+# Add your development dependencies here
```

### Comparing `social_media_aggregator-0.0.1a1/src/social_media_aggregator/exceptions/logger.py` & `social_media_aggregator-0.1.5/src/social_media_aggregator/exceptions/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 class BaseLoggerException(BaseException):
     def __init__(self, message):
-        self.message = f"Logger error. {message}"
+        self.message = message
         super().__init__(self.message)
 
 
-class LoggerInvalidArguments(BaseLoggerException):
-    def __init__(self, message="Incorrect number of arguments provided"):
+class LoggerInvalidNameException(BaseLoggerException):
+    def __init__(self, message="Logger name is required"):
         self.message = message
         super().__init__(self.message)
 
 
-# class LoggerInvalidNameException(BaseLoggerException):
-#     def __init__(self, message="Logger name is required"):
-#         self.message = message
-#         super().__init__(self.message)
-
-
 class LoggerInvalidLevelException(BaseLoggerException):
     def __init__(self, message="Logger level is required"):
         self.message = message
         super().__init__(self.message)
```

### Comparing `social_media_aggregator-0.0.1a1/src/social_media_aggregator/exceptions/meta.py` & `social_media_aggregator-0.1.5/src/social_media_aggregator/exceptions/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 class BaseMetaException(BaseException):
     def __init__(self, message):
         self.message = f"Meta error. {message}"
         super().__init__(self.message)
 
 
-class MetaInvalidArguments(BaseMetaException):
-    def __init__(self, message="Incorrect number of arguments provided"):
+class MetaInvalidEndpointException(BaseMetaException):
+    def __init__(self, message="API endpoint is required"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class MetaInvalidTokenException(BaseMetaException):
+    def __init__(self, message="API key is required"):
         self.message = message
         super().__init__(self.message)
 
 
 class MetaApiException(BaseMetaException):
     def __init__(self, status_code, reason, response_payload=None):
         self.status_code = status_code
```

### Comparing `social_media_aggregator-0.0.1a1/src/social_media_aggregator/logger.py` & `social_media_aggregator-0.1.5/src/social_media_aggregator/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 import logging
-from .exceptions.logger import LoggerInvalidArguments, LoggerInvalidLevelException
-from .helpers.helpers import validate_arguments
+from .exceptions.logger import (
+    LoggerInvalidLevelException,
+    LoggerInvalidNameException,
+)
 
 
 class CustomLogger:
     """
     Class with methods to create a custom logger
     and contains the following methods:
+    
     - _validate_logger: validates the logger name and level
     - _create_formatter: creates a custom formatter for the logger
     - _create_handler: creates a custom handler for the logger
     - create_logger: creates a custom logger
     - return_logger: returns the custom logger
     """
 
-    @validate_arguments(
-        (str, True), (int, True), exception_class=LoggerInvalidArguments
-    )
     def __init__(self, logger_name: str, logger_level: int):
         self.logger_name = logger_name
         self.logger_level = logger_level
 
+    def _validate_logger(self):
+        if not isinstance(self.logger_name, str):
+            raise LoggerInvalidNameException("Logger name is required")
+        if len(self.logger_name) == 0:
+            raise LoggerInvalidNameException("Logger name is required")
+
+        if self.logger_level not in [
+            logging.DEBUG,
+            logging.INFO,
+            logging.WARNING,
+            logging.ERROR,
+            logging.CRITICAL,
+        ]:
+            raise LoggerInvalidLevelException("Logger level is required")
+
     def _create_formatter(self):
+        self._validate_logger
         return logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
     def _create_handler(self):
+        self._validate_logger
         handler = logging.StreamHandler()
         handler.setFormatter(self._create_formatter())
         return handler
 
     def create_logger(self):
-        if self.logger_level not in [
-            logging.CRITICAL,
-            logging.ERROR,
-            logging.WARNING,
-            logging.INFO,
-            logging.DEBUG,
-        ]:
-            raise LoggerInvalidLevelException(
-                f"Argument 'logger_level' with value '{self.logger_level}' is not a valid logging level."
-            )
-
+        self._validate_logger
         logger = logging.getLogger(self.logger_name)
         logger.setLevel(self.logger_level)
         logger.handlers.clear()
         logger.addHandler(self._create_handler())
         self.logger = logger
 
     def return_logger(self):
```

### Comparing `social_media_aggregator-0.0.1a1/PKG-INFO` & `social_media_aggregator-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social_media_aggregator
-Version: 0.0.1a1
+Version: 0.1.5
 Summary: This is a project that aggregates several social media accounts into a single space
 License: MIT
 Author: José Viegas
 Author-email: jviegas6@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

