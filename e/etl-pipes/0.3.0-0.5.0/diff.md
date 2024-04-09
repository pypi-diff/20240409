# Comparing `tmp/etl_pipes-0.3.0.tar.gz` & `tmp/etl_pipes-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipes-0.3.0.tar", max compression
+gzip compressed data, was "etl_pipes-0.5.0.tar", max compression
```

## Comparing `etl_pipes-0.3.0.tar` & `etl_pipes-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.3.0/etl_pipes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.3.0/etl_pipes/actors/__init__.py
--rw-r--r--   0        0        0     2049 2024-03-31 18:15:41.761652 etl_pipes-0.3.0/etl_pipes/actors/actor.py
--rw-r--r--   0        0        0     8182 2024-03-31 18:15:41.762013 etl_pipes-0.3.0/etl_pipes/actors/actor_system.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.3.0/etl_pipes/actors/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.3.0/etl_pipes/actors/common/logging.py
--rw-r--r--   0        0        0     1434 2024-03-31 18:15:41.762619 etl_pipes-0.3.0/etl_pipes/actors/common/types.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.3.0/etl_pipes/common/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.3.0/etl_pipes/common/utils/__init__.py
--rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.3.0/etl_pipes/common/utils/type_hints.py
--rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.3.0/etl_pipes/domain/__init__.py
--rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.3.0/etl_pipes/domain/types.py
--rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.3.0/etl_pipes/pipes/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-30 18:10:45.704990 etl_pipes-0.3.0/etl_pipes/pipes/base_pipe.py
--rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.3.0/etl_pipes/pipes/broadcast_parallel.py
--rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.3.0/etl_pipes/pipes/map_reduce.py
--rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.3.0/etl_pipes/pipes/maybe.py
--rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.3.0/etl_pipes/pipes/parallel.py
--rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.3.0/etl_pipes/pipes/pipeline/__init__.py
--rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.3.0/etl_pipes/pipes/pipeline/exceptions.py
--rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.3.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
--rw-r--r--   0        0        0     1750 2024-03-30 18:10:45.707479 etl_pipes-0.3.0/etl_pipes/pipes/pipeline/pipeline.py
--rw-r--r--   0        0        0     1334 2024-04-01 15:13:19.970748 etl_pipes-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7430 2023-11-18 10:28:00.879518 etl_pipes-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.5.0/etl_pipes/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.5.0/etl_pipes/actors/__init__.py
+-rw-r--r--   0        0        0     2049 2024-03-31 18:15:41.761652 etl_pipes-0.5.0/etl_pipes/actors/actor.py
+-rw-r--r--   0        0        0     8182 2024-03-31 18:15:41.762013 etl_pipes-0.5.0/etl_pipes/actors/actor_system.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.5.0/etl_pipes/actors/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.5.0/etl_pipes/actors/common/logging.py
+-rw-r--r--   0        0        0     1434 2024-03-31 18:15:41.762619 etl_pipes-0.5.0/etl_pipes/actors/common/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.5.0/etl_pipes/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.5.0/etl_pipes/common/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.5.0/etl_pipes/common/utils/type_hints.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.5.0/etl_pipes/context.py
+-rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.5.0/etl_pipes/domain/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.5.0/etl_pipes/domain/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.5.0/etl_pipes/pipes/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.5.0/etl_pipes/pipes/base_pipe.py
+-rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.5.0/etl_pipes/pipes/broadcast_parallel.py
+-rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.5.0/etl_pipes/pipes/map_reduce.py
+-rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.5.0/etl_pipes/pipes/maybe.py
+-rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.5.0/etl_pipes/pipes/parallel.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/__init__.py
+-rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/exceptions.py
+-rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py
+-rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1133 2024-04-08 19:43:30.227481 etl_pipes-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7748 1970-01-01 00:00:00.000000 etl_pipes-0.5.0/PKG-INFO
```

### Comparing `etl_pipes-0.3.0/README.md` & `etl_pipes-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/actors/actor.py` & `etl_pipes-0.5.0/etl_pipes/actors/actor.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/actors/actor_system.py` & `etl_pipes-0.5.0/etl_pipes/actors/actor_system.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/actors/common/logging.py` & `etl_pipes-0.5.0/etl_pipes/actors/common/logging.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/actors/common/types.py` & `etl_pipes-0.5.0/etl_pipes/actors/common/types.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/base_pipe.py` & `etl_pipes-0.5.0/etl_pipes/pipes/base_pipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import copy
 import inspect
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, fields
 from typing import Any, assert_never
 
+from etl_pipes.context import Context, ContextPart
 from etl_pipes.domain.types import AnyFunc
 
 
 @dataclass
 class PipeOutput:
     is_modified: bool = field(init=False, default=False)
     pos: int | slice | tuple[int, ...] = field(
@@ -20,14 +21,33 @@
 class Pipe:
     is_void: bool = field(init=False, default=False)
     f: AnyFunc | None = field(init=False, default=None)
     out: PipeOutput = field(init=False, default_factory=PipeOutput)
 
     __original_func: AnyFunc | None = field(init=False, default=None)
 
+    def apply_context(self, context: Context | None) -> None:
+        if context is None:
+            return
+
+        context_class = context.__class__
+        for dc_field in fields(self):
+            f_name = dc_field.name
+            f_type = dc_field.type
+            f_default = dc_field.default
+
+            if f_type == context_class and f_default == context_class:
+                setattr(self, f_name, context)
+
+            if context.has_part(f_name, f_type):
+                if isinstance(f_default, ContextPart):
+                    context_part = f_default
+                    if context_part.is_part_of(context_class):
+                        setattr(self, f_name, context.get_part(f_name))
+
     async def __call__(self, *args: Any) -> Any:
         if self.f is None:
             raise NotImplementedError(
                 "Pipe must be initialized with a coroutine function"
             )
         return await self.f(*args)
```

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/map_reduce.py` & `etl_pipes-0.5.0/etl_pipes/pipes/map_reduce.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/maybe.py` & `etl_pipes-0.5.0/etl_pipes/pipes/maybe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/parallel.py` & `etl_pipes-0.5.0/etl_pipes/pipes/parallel.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/pipeline/exceptions.py` & `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py` & `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipe_welding_validator.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.3.0/etl_pipes/pipes/pipeline/pipeline.py` & `etl_pipes-0.5.0/etl_pipes/pipes/pipeline/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, assert_never
 
+from etl_pipes.context import Context
 from etl_pipes.pipes.base_pipe import Pipe
 from etl_pipes.pipes.pipeline.pipe_welding_validator import PipeWeldingValidator
 
 
 @dataclass
 class Pipeline(Pipe):
     pipes: list[Pipe] = field(default_factory=list)
     validator: PipeWeldingValidator = field(default_factory=PipeWeldingValidator)
-    ignore_validation: bool = field(default=False)
+    ignore_validation: bool = field(default=True)
+    context: Context | None = field(default=None)
 
     def __post_init__(self) -> None:
+        self.apply_context(self.context)
+
         self._validate()
 
+    def apply_context(self, context: Context | None) -> None:
+        if context:
+            for pipe in self.pipes:
+                pipe.apply_context(context)
+
     async def __call__(self, *args: Any) -> Any:
         self._validate()
 
         data = args
         prev_pipe = None
 
         for pipe in self.pipes:
```

### Comparing `etl_pipes-0.3.0/pyproject.toml` & `etl_pipes-0.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,56 @@
+[build-system]
+requires = [ "poetry-core",]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "etl-pipes"
-version = "0.3.0"
+version = "0.5.0"
 description = ""
-authors = ["Tikhon Zaikin <th@thevhs.club>"]
+authors = [ "Tikhon Zaikin <th@thevhs.club>",]
 readme = "README.md"
 
-[tool.poetry.dependencies]
-python = "^3.11"
-pip = "^23.2"
-
-[tool.poetry.group.dev.dependencies]
-ruff = "^0.0.277"
-black = "^23.3.0"
-mypy = "^1.4.1"
-pytest = "^7.4.0"
-pre-commit = "^3.4.0"
-coverage = "^7.3.1"
-pytest-asyncio = "^0.21.1"
-fastapi = "^0.103.1"
-unicorn = {extras = ["standard"], version = "^2.0.1.post1"}
-sqlalchemy = { version = "^2.0.21", extras = ["mypy"] }
-uvicorn = "^0.23.2"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.ruff]
-select = [
-  "E",   # pycodestyle
-  "F",   # pyflakes
-  "UP",  # pyupgrade
-  "W",   # warnings
-  "I",   # import order
-  "N",   # pep8 naming
-  "PL",  # pylint
-  "RUF", # ruff
-  "PTH", # path
-]
+select = [ "E", "F", "UP", "W", "I", "N", "PL", "RUF", "PTH",]
 
 [tool.black]
 line-length = 88
-target-version = ['py3.11']
-include = '\.pyi?$'
+target-version = [ "py3.11",]
+include = "\\.pyi?$"
 
 [tool.mypy]
-plugins = [
-  # "pydantic.mypy"
-]
-
+plugins = []
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
-
-# for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 
-# [tool.pydantic-mypy]
-# init_forbid_extra = true
-# init_typed = true
-# warn_required_dynamic_aliases = true
+[tool.poetry.dependencies]
+python = "^3.11"
+pip = "^23.2"
 
 [tool.ruff.pylint]
-max-returns = 10
+max-returns = 10
+
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.277"
+black = "^23.3.0"
+mypy = "^1.4.1"
+pytest = "^7.4.0"
+pre-commit = "^3.4.0"
+coverage = "^7.3.1"
+pytest-asyncio = "^0.21.1"
+fastapi = "^0.103.1"
+uvicorn = "^0.23.2"
+typer = "^0.12.2"
+toml = "^0.10.2"
+
+[tool.poetry.group.dev.dependencies.unicorn]
+extras = [ "standard",]
+version = "^2.0.1.post1"
+
+[tool.poetry.group.dev.dependencies.sqlalchemy]
+version = "^2.0.21"
+extras = [ "mypy",]
```

### Comparing `etl_pipes-0.3.0/PKG-INFO` & `etl_pipes-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-pipes
-Version: 0.3.0
+Version: 0.5.0
 Summary: 
 Author: Tikhon Zaikin
 Author-email: th@thevhs.club
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pip (>=23.2,<24.0)
```

