# Comparing `tmp/tenzir_platform-0.1.0.tar.gz` & `tmp/tenzir_platform-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenzir_platform-0.1.0.tar", max compression
+gzip compressed data, was "tenzir_platform-0.2.0.tar", max compression
```

## Comparing `tenzir_platform-0.1.0.tar` & `tenzir_platform-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/README.md
--rw-r--r--   0        0        0     1211 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/helpers/__init__.py
--rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/helpers/auth_rule.py
--rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/helpers/cache.py
--rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/helpers/client.py
--rw-r--r--   0        0        0      887 2024-04-05 16:27:40.856682 tenzir_platform-0.1.0/tenzir_platform/helpers/environment.py
--rw-r--r--   0        0        0     5660 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/helpers/oidc.py
--rw-r--r--   0        0        0     6287 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/subcommand_admin.py
--rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.1.0/tenzir_platform/subcommand_auth.py
--rw-r--r--   0        0        0     4360 2024-04-08 15:25:27.364492 tenzir_platform-0.1.0/tenzir_platform/subcommand_node.py
--rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.1.0/tenzir_platform/subcommand_workspace.py
--rw-r--r--   0        0        0     1668 2024-04-05 14:04:00.536799 tenzir_platform-0.1.0/tenzir_platform/tenzir_platform.py
--rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/README.md
+-rw-r--r--   0        0        0      878 2024-04-09 10:47:05.809062 tenzir_platform-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/helpers/__init__.py
+-rw-r--r--   0        0        0     1195 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/helpers/auth_rule.py
+-rw-r--r--   0        0        0     1196 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/helpers/cache.py
+-rw-r--r--   0        0        0     3216 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/helpers/client.py
+-rw-r--r--   0        0        0      887 2024-04-05 16:27:40.856682 tenzir_platform-0.2.0/tenzir_platform/helpers/environment.py
+-rw-r--r--   0        0        0     5625 2024-04-09 10:41:29.120882 tenzir_platform-0.2.0/tenzir_platform/helpers/oidc.py
+-rw-r--r--   0        0        0     6287 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/subcommand_admin.py
+-rw-r--r--   0        0        0      585 2024-04-05 14:04:00.532799 tenzir_platform-0.2.0/tenzir_platform/subcommand_auth.py
+-rw-r--r--   0        0        0     6221 2024-04-09 10:48:28.185131 tenzir_platform-0.2.0/tenzir_platform/subcommand_node.py
+-rw-r--r--   0        0        0     1741 2024-04-05 14:04:00.536799 tenzir_platform-0.2.0/tenzir_platform/subcommand_workspace.py
+-rw-r--r--   0        0        0     1668 2024-04-09 10:42:45.944905 tenzir_platform-0.2.0/tenzir_platform/tenzir_platform.py
+-rw-r--r--   0        0        0     1110 1970-01-01 00:00:00.000000 tenzir_platform-0.2.0/PKG-INFO
```

### Comparing `tenzir_platform-0.1.0/pyproject.toml` & `tenzir_platform-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,38 @@
 [tool.poetry]
 name = "tenzir-platform"
-version = "0.1.0"
+version = "0.2.0"
 description = "Tenzir CLI"
 authors = ["Tenzir <engineering@tenzir.com>"]
 readme = "README.md"
 packages = [{ include = "tenzir_platform" }]
 
 [tool.poetry.scripts]
 tenzir-platform = "tenzir_platform.tenzir_platform:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-
 structlog = "^23.1.0"
 requests = "^2.31.0"
 docopt = "^0.6.2"
 types-docopt = "^0.6.11.4"
 pydantic-settings = "^2.2.1"
 pyjwt = {extras = ["crypto"], version = "^2.8.0"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
 isort = "^5.12.0"
 mypy = "^1.5.1"
 werkzeug = "^2.3.7"
 
-[tool.poetry.group.cli.dependencies]
-auth0-python = "^4.7.0"
-cytoolz = "^0.12.2"
-invoke = "^2.2.0"
-pytimeparse = "^1.1.8"
-tabulate = "^0.9.0"
-
 # Additional type stubs for mypy.
 [tool.poetry.group.types.dependencies]
 types-requests = "^2.31.0.2"
 types-tabulate = "^0.9.0.3"
 
 [tool.mypy]
 python_version = "3.10"
 warn_unused_configs = true
 
-[[tool.mypy.overrides]]
-module = [
-  "auth0.*",
-  "docker",
-  "pytimeparse",
-  "segment.*",
-  "toolz.*",
-  "troposphere",
-  "troposphere.*",
-  "websocket",
-]
-ignore_missing_imports = true
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tenzir_platform-0.1.0/tenzir_platform/helpers/auth_rule.py` & `tenzir_platform-0.2.0/tenzir_platform/helpers/auth_rule.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/helpers/cache.py` & `tenzir_platform-0.2.0/tenzir_platform/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/helpers/client.py` & `tenzir_platform-0.2.0/tenzir_platform/helpers/client.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/helpers/environment.py` & `tenzir_platform-0.2.0/tenzir_platform/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/helpers/oidc.py` & `tenzir_platform-0.2.0/tenzir_platform/helpers/oidc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import hashlib
 import os
 import time
 
 import jwt
 import requests
-from invoke.exceptions import Exit
 from jwt import PyJWKClient
 from typing import Optional, Any
 from tenzir_platform.helpers.cache import filename_in_cache
 from tenzir_platform.helpers.environment import PlatformEnvironment
 
 
 class INVALID_API_KEY(Exception):
```

### Comparing `tenzir_platform-0.1.0/tenzir_platform/subcommand_admin.py` & `tenzir_platform-0.2.0/tenzir_platform/subcommand_admin.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/subcommand_auth.py` & `tenzir_platform-0.2.0/tenzir_platform/subcommand_auth.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/subcommand_workspace.py` & `tenzir_platform-0.2.0/tenzir_platform/subcommand_workspace.py`

 * *Files identical despite different names*

### Comparing `tenzir_platform-0.1.0/tenzir_platform/tenzir_platform.py` & `tenzir_platform-0.2.0/tenzir_platform/tenzir_platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from tenzir_platform.subcommand_admin import admin_subcommand
 from tenzir_platform.helpers.environment import PlatformEnvironment
 
 
 def main():
     if len(sys.argv) == 1:
         sys.argv.append("--help")
-    arguments = docopt(__doc__, version="Tenzir Platform CLI 1.0", options_first=True)
+    arguments = docopt(__doc__, version="Tenzir Platform CLI 0.2", options_first=True)
     platform = PlatformEnvironment.load()
     argv = [arguments["<command>"]] + arguments["<args>"]
     if arguments["<command>"] == "auth":
         auth_subcommand(platform, argv)
     elif arguments["<command>"] == "workspace":
         workspace_subcommand(platform, argv)
     elif arguments["<command>"] == "node":
```

### Comparing `tenzir_platform-0.1.0/PKG-INFO` & `tenzir_platform-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenzir-platform
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tenzir CLI
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

