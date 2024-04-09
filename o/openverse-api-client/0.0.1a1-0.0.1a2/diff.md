# Comparing `tmp/openverse_api_client-0.0.1a1.tar.gz` & `tmp/openverse_api_client-0.0.1a2.tar.gz`

## Comparing `openverse_api_client-0.0.1a1.tar` & `openverse_api_client-0.0.1a2.tar`

### file list

```diff
@@ -1,41 +1,22 @@
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.prettierrc.toml
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/justfile
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/.npmignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/LICENSE
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/package.json
--rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/pnpm-lock.yaml
--rw-r--r--   0        0        0    12392 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tsconfig.json
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tsconfig.prod.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/vitest.config.mts
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/src/client.ts
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/src/index.ts
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tests/client.test.ts
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/packages/openverse-api-client/tests/mock-thumbnail.bin
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/__about__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/__init__.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/auth.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/meta.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/__init__.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/auth.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/base.py
--rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/media.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/base.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/python.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/generate/typescript.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/python/client.py.jinja
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/types.ts.jinja
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/helpers/interface.ts.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/conftest.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/mock-thumbnail.bin
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/test_async.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/tests/test_sync.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/README.rst
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/__about__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/__init__.py
+-rw-r--r--   0        0        0    24665 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/async_client.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/auth.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/meta.py
+-rw-r--r--   0        0        0    24263 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/sync_client.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_generate/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_generate/base.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_generate/python.py
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_generate/typescript.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_templates/python/client.py.jinja
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_templates/typescript/types.ts.jinja
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/_templates/typescript/helpers/interface.ts.jinja
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/endpoints/__init__.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/endpoints/auth.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/endpoints/base.py
+-rw-r--r--   0        0        0     6117 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/openverse_api_client/endpoints/media.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/LICENSE
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/README.rst
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 openverse_api_client-0.0.1a2/PKG-INFO
```

### Comparing `openverse_api_client-0.0.1a1/packages/openverse-api-client/LICENSE` & `openverse_api_client-0.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/auth.py` & `openverse_api_client-0.0.1a2/openverse_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/auth.py` & `openverse_api_client-0.0.1a2/openverse_api_client/endpoints/auth.py`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/endpoints/media.py` & `openverse_api_client-0.0.1a2/openverse_api_client/endpoints/media.py`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/generate/__init__.py` & `openverse_api_client-0.0.1a2/openverse_api_client/_generate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 import argparse
 
-from openverse_api_client.generate.python import generate_python
-from openverse_api_client.generate.typescript import generate_typescript
+from openverse_api_client._generate.python import generate_python
+from openverse_api_client._generate.typescript import generate_typescript
 
 
 arg_parser = argparse.ArgumentParser(
     prog="generate-openverse-api-client",
     description="Generate Openverse API clients for various languages.",
     epilog="If no language flags are passed, all languages will be generated. Otherwise, only the languages whose flags are passed will be generated.",
 )
```

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/generate/python.py` & `openverse_api_client-0.0.1a2/openverse_api_client/_generate/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from typing import TypedDict, get_args
 
 from openverse_api_client import endpoints
-from openverse_api_client.generate.base import template_env, is_bytes
+from openverse_api_client._generate.base import template_env, is_bytes
 from openverse_api_client.meta import empty
 
 
 client_template = template_env.get_template("python/client.py.jinja")
 
 
 def type_to_string(t) -> str:
```

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/generate/typescript.py` & `openverse_api_client-0.0.1a2/openverse_api_client/_generate/typescript.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing_extensions import Set, TypedDict, get_args, _TypedDictMeta, is_typeddict  # type: ignore[attr-defined]
 from types import UnionType, NoneType
 from decimal import Decimal
 from dataclasses import dataclass, asdict
 
 
 from openverse_api_client import endpoints
-from openverse_api_client.generate.base import template_env, is_bytes
+from openverse_api_client._generate.base import template_env, is_bytes
 
 
 TypeScriptFiles = TypedDict(
     "TypeScriptFiles",
     {
         "types.ts": str,
     },
```

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/templates/python/client.py.jinja` & `openverse_api_client-0.0.1a2/openverse_api_client/_templates/python/client.py.jinja`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/src/openverse_api_client/templates/typescript/types.ts.jinja` & `openverse_api_client-0.0.1a2/openverse_api_client/_templates/typescript/types.ts.jinja`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/README.rst` & `openverse_api_client-0.0.1a2/README.rst`

 * *Files identical despite different names*

### Comparing `openverse_api_client-0.0.1a1/pyproject.toml` & `openverse_api_client-0.0.1a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,19 +39,27 @@
 [project.urls]
 Homepage = "https://sr.ht/~sara/openverse-api-client/#openverse-api-client"
 Documentation = "https://git.sr.ht/~sara/openverse-api-client#readme"
 Issues = "https://todo.sr.ht/~sara/openverse-api-client"
 Source = "https://git.sr.ht/~sara/openverse-api-client"
 
 [project.scripts]
-generate-openverse-api-client = "openverse_api_client.generate:generate_cli"
+generate-openverse-api-client = "openverse_api_client._generate:generate_cli"
 
 [tool.hatch.version]
 path = "src/openverse_api_client/__about__.py"
 
+[tool.hatch.build.targets.sdist]
+packages = ["src/openverse_api_client"]
+artifacts = ["*client.py"]
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/openverse_api_client"]
+artifacts = ["*client.py"]
+
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "mypy>=1.0.0",
   "typing_extensions",
   "pytest",
   "pytest-asyncio",
```

### Comparing `openverse_api_client-0.0.1a1/PKG-INFO` & `openverse_api_client-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openverse-api-client
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Python client for the Openverse API
 Project-URL: Homepage, https://sr.ht/~sara/openverse-api-client/#openverse-api-client
 Project-URL: Documentation, https://git.sr.ht/~sara/openverse-api-client#readme
 Project-URL: Issues, https://todo.sr.ht/~sara/openverse-api-client
 Project-URL: Source, https://git.sr.ht/~sara/openverse-api-client
 Author-email: sarayourfriend <git@sarayourfriend.pictures>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
```

