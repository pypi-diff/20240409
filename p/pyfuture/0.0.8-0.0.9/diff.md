# Comparing `tmp/pyfuture-0.0.8.tar.gz` & `tmp/pyfuture-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfuture-0.0.8.tar", last modified: Tue Nov 21 15:40:46 2023, max compression
+gzip compressed data, was "pyfuture-0.0.9.tar", last modified: Thu Dec  7 06:24:47 2023, max compression
```

## Comparing `pyfuture-0.0.8.tar` & `pyfuture-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0       63 2023-11-21 15:40:34.453661 pyfuture-0.0.8/README.md
--rw-r--r--   0        0        0      347 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pdm_build.py
--rw-r--r--   0        0        0       37 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/__init__.py
--rw-r--r--   0        0        0     2675 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/__main__.py
--rw-r--r--   0        0        0       21 2023-11-21 15:40:46.977660 pyfuture-0.0.8/pyfuture/__version__.py
--rw-r--r--   0        0        0       70 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/codemod/__init__.py
--rw-r--r--   0        0        0     6925 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/codemod/transform_type_parameters.py
--rw-r--r--   0        0        0     2034 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/codemod/utils.py
--rw-r--r--   0        0        0       40 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/transformer/__init__.py
--rw-r--r--   0        0        0      329 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/transformer/replace.py
--rw-r--r--   0        0        0     1379 2023-11-21 15:40:34.453661 pyfuture-0.0.8/pyfuture/utils.py
--rw-r--r--   0        0        0      827 2023-11-21 15:40:46.981660 pyfuture-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 pyfuture-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      383 2023-12-07 06:24:31.008769 pyfuture-0.0.9/README.md
+-rw-r--r--   0        0        0      950 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pdm_build.py
+-rw-r--r--   0        0        0       37 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/__init__.py
+-rw-r--r--   0        0        0     2646 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/__main__.py
+-rw-r--r--   0        0        0       21 2023-12-07 06:24:47.428859 pyfuture-0.0.9/pyfuture/__version__.py
+-rw-r--r--   0        0        0       70 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/codemod/__init__.py
+-rw-r--r--   0        0        0     6812 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/codemod/transform_type_parameters.py
+-rw-r--r--   0        0        0     2379 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/codemod/utils.py
+-rw-r--r--   0        0        0       40 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/transformer/__init__.py
+-rw-r--r--   0        0        0      362 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/transformer/replace.py
+-rw-r--r--   0        0        0     1322 2023-12-07 06:24:31.008769 pyfuture-0.0.9/pyfuture/utils.py
+-rw-r--r--   0        0        0     1253 2023-12-07 06:24:47.428859 pyfuture-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-07 06:24:31.008769 pyfuture-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     1086 2023-12-07 06:24:31.008769 pyfuture-0.0.9/tests/test_transformer.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 pyfuture-0.0.9/PKG-INFO
```

### Comparing `pyfuture-0.0.8/pyfuture/__main__.py` & `pyfuture-0.0.9/pyfuture/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-from loguru import logger
-import typer
-from pyfuture.utils import transfer_file
-from pathlib import Path
+from __future__ import annotations
 
+from pathlib import Path
 
-def str2tuple(version: str) -> tuple[int, int]:
-    """
-    Convert a string to a tuple of integers.
-    """
-    version_info: tuple[int, ...] = tuple(map(int, version.split(".")))
-    assert len(version_info) >= 2, "Version must be at least major.minor"
-    return version_info[0], version_info[1]
+import typer
+from loguru import logger
 
+from pyfuture.utils import transfer_file
 
 app = typer.Typer()
 
 
 @app.command()
 def transfer(
     src_file: Path,
     tgt_file: Path,
     *,
-    target: str = "3.8",
+    target: str = "3.6",
 ):
     """
     Transfer code from src_file and write to tgt_file.
     """
-
-    transfer_file(src_file, tgt_file, target=str2tuple(target))
+    assert target == "3.6", "PyFuture is very early stage, not support target argument yet"
+    transfer_file(src_file, tgt_file)
 
 
 @app.command()
 def watch(
     src_file: Path,
     tgt_file: Path,
     *,
-    target: str = "3.8",
+    target: str = "3.6",
 ):
     """
     Transfer all python files in src_dir to build_dir, and watch for changes.
     """
+    assert target == "3.6", "PyFuture is very early stage, not support target argument yet"
+    transfer_file(src_file, tgt_file)
 
-    transfer_file(src_file, tgt_file, target=str2tuple(target))
-
-    from watchfiles import watch, Change
+    from watchfiles import Change, watch
 
     for changes in watch(src_file):
         for mode, path in changes:
             match mode:
                 case Change.modified:
                     logger.info("Source file has been modified")
-                    transfer_file(Path(path), tgt_file, target=str2tuple(target))
+                    transfer_file(Path(path), tgt_file)
                 case Change.deleted:
                     logger.info("Source file has been deleted")
                     break
 
 
 @app.command()
 def transfer_dir(
     src_dir: Path,
     build_dir: Path,
     *,
-    target: str = "3.8",
+    target: str = "3.6",
 ):
     """
     Transfer all python files in src_dir to build_dir.
     """
+    assert target == "3.6", "PyFuture is very early stage, not support target argument yet"
 
     for src_file in src_dir.glob("**/*.py"):
         tgt_file = build_dir / src_file.relative_to(src_dir)
-        transfer_file(src_file, tgt_file, target=str2tuple(target))
+        transfer_file(src_file, tgt_file)
 
 
 @app.command()
 def watch_dir(
     src_dir: Path,
     build_dir: Path,
     *,
-    target: str = "3.8",
+    target: str = "3.6",
 ):
     """
     Transfer all python files in src_dir to build_dir, and watch for changes.
     """
-
+    assert target == "3.6", "PyFuture is very early stage, not support target argument yet"
     transfer_dir(src_dir, build_dir, target=target)
 
-    from watchfiles import watch, Change, PythonFilter
+    from watchfiles import Change, PythonFilter, watch
 
     for changes in watch(src_dir, watch_filter=PythonFilter()):
         for mode, path in changes:
             match mode:
                 case Change.added | Change.modified:
                     logger.info(f"Created: {path}")
                     tgt_file = build_dir / Path(path).relative_to(src_dir)
-                    transfer_file(Path(path), tgt_file, target=str2tuple(target))
+                    transfer_file(Path(path), tgt_file)
                 case Change.deleted:
                     logger.info(f"Deleted: {path}")
                     tgt_file = build_dir / Path(path).relative_to(src_dir)
                     tgt_file.unlink()
 
 
 if __name__ == "__main__":
```

### Comparing `pyfuture-0.0.8/pyfuture/codemod/transform_type_parameters.py` & `pyfuture-0.0.9/pyfuture/codemod/transform_type_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,85 @@
-import libcst as cst
+from __future__ import annotations
+
+from typing import Any
+
 from libcst import (
-    Name,
-    FunctionDef,
+    Arg,
     Assign,
-    Call,
     AssignTarget,
-    Arg,
-    SimpleStatementLine,
-    FlattenSentinel,
+    Call,
     ClassDef,
+    FlattenSentinel,
+    FunctionDef,
+    Index,
+    Name,
+    SimpleStatementLine,
     Subscript,
     SubscriptElement,
-    Index
 )
 from libcst.codemod import (
     CodemodContext,
     VisitorBasedCodemodCommand,
 )
 from libcst.codemod.visitors import AddImportsVisitor
-from libcst import matchers
-from libcst.metadata import MetadataWrapper, ScopeProvider, Assignment, Scope
-from typing import Any
+from libcst.metadata import Scope, ScopeProvider
 
 from ..transformer import ReplaceTransformer
 from .utils import gen_func_wrapper, gen_type_param
 
+
 class TransformTypeParametersCommand(VisitorBasedCodemodCommand):
-    METADATA_DEPENDENCIES = (ScopeProvider, )
+    METADATA_DEPENDENCIES = (ScopeProvider,)
 
     def __init__(self, context: CodemodContext) -> None:
         self.node_to_wrapper: dict[FunctionDef | ClassDef, Any] = {}
         super().__init__(context)
 
-    def remove_type_parameters[T: FunctionDef| ClassDef](self, node: T, prefix:str="", suffix:str="") -> tuple[list[SimpleStatementLine], T]:
+    def remove_type_parameters[T: FunctionDef | ClassDef](
+        self, node: T, prefix: str = "", suffix: str = ""
+    ) -> tuple[list[SimpleStatementLine], T]:
         type_params = node.type_parameters
         if type_params is None:
             return [], node
         statements = []
-        new_node = node.with_changes(
-            type_parameters = None
-        )
+        new_node = node.with_changes(type_parameters=None)
 
         slices = []
         for type_param in type_params.params:
             new_name = type_param.param.name.with_changes(value=f"{prefix}{type_param.param.name.value}{suffix}")
-            
+
             AddImportsVisitor.add_needed_import(self.context, "typing", type_param.param.__class__.__name__)
             statements.append(gen_type_param(type_param.param, new_name))
             slices.append(
                 SubscriptElement(
-                    slice=Index(
-                        value=new_name
-                    ),
+                    slice=Index(value=new_name),
                 ),
             )
-        
+
         if isinstance(new_node, ClassDef) and slices:
             AddImportsVisitor.add_needed_import(self.context, "typing", "Generic")
             generic_base = Arg(
-                value= Subscript(
+                value=Subscript(
                     value=Name(
-                        value='Generic',
+                        value="Generic",
                         lpar=[],
                         rpar=[],
                     ),
-                    slice=slices
-            ))
-            new_node = new_node.with_changes(
-                bases = [*new_node.bases, generic_base]
+                    slice=slices,
+                )
             )
+            new_node = new_node.with_changes(bases=[*new_node.bases, generic_base])
 
         return statements, new_node
 
     def visit_FunctionDef(self, node: FunctionDef):
         type_params = node.type_parameters
         if type_params is None:
             return False
-        
+
         node_scope = self.get_metadata(ScopeProvider, type_params)
         body_scope = self.get_metadata(ScopeProvider, node.body)
         replacemences = {}
         prefix = f"__{node.name.value}_"
         for type_param in type_params.params:
             for scope in [node_scope, body_scope]:
                 assert isinstance(scope, Scope)
@@ -97,23 +96,25 @@
             self.node_to_wrapper[node] = wrapper
         return False
 
     def leave_FunctionDef(self, original_node: FunctionDef, updated_node: FunctionDef):
         wrapper = self.node_to_wrapper.get(original_node, None)
         if wrapper is None:
             return updated_node
-        func = SimpleStatementLine([Assign(
-            targets=[AssignTarget(updated_node.name)],
-            value=Call(
-                func=Name(
-                    value=f'__wrapper_func_{updated_node.name.value}'
-                ),
-                args=[],
-            ),
-        )])
+        func = SimpleStatementLine(
+            [
+                Assign(
+                    targets=[AssignTarget(updated_node.name)],
+                    value=Call(
+                        func=Name(value=f"__wrapper_func_{updated_node.name.value}"),
+                        args=[],
+                    ),
+                )
+            ]
+        )
 
         return FlattenSentinel([wrapper, func])
 
     def visit_ClassDef(self, node: ClassDef):
         type_params = node.type_parameters
         replacemences = {}
         scopes = []
@@ -125,33 +126,33 @@
                 scopes.append(subnode_body_scope)
 
                 subnode_type_params = subnode.type_parameters
                 if subnode_type_params is None:
                     continue
                 subnode_type_scope = self.get_metadata(ScopeProvider, subnode_type_params)
                 scopes.append(subnode_type_scope)
-                
+
                 prefix = f"__{node.name.value}_{subnode.name.value}_"
                 for type_param in subnode_type_params.params:
                     for scope in [subnode_type_scope, subnode_body_scope]:
                         assert isinstance(scope, Scope)
                         for access in set(scope.accesses[type_param.param.name]):
                             assert isinstance(access.node, Name)
                             replacemences[access.node] = Name(value=f"{prefix}{type_param.param.name.value}")
-        
+
         prefix = f"__{node.name.value}_"
         if type_params is not None:
             scopes.append(self.get_metadata(ScopeProvider, type_params))
             for type_param in type_params.params:
                 for scope in scopes:
                     assert isinstance(scope, Scope)
                     for access in set(scope.accesses[type_param.param.name]):
                         assert isinstance(access.node, Name)
                         replacemences[access.node] = Name(value=f"{prefix}{type_param.param.name.value}")
-        
+
         new_node = node.visit(ReplaceTransformer(replacemences))
         assert isinstance(new_node, ClassDef)
 
         type_vars, new_node = self.remove_type_parameters(new_node, prefix=prefix)
 
         self.node_to_wrapper[node] = new_node, type_vars
         # TODO: Maybe `class in class` need True?
@@ -163,13 +164,10 @@
         new_node, type_vars = self.node_to_wrapper[original_node]
         replacemences = {}
         for subnode in new_node.body.body:
             if isinstance(subnode, FunctionDef):
                 prefix = f"__{new_node.name.value}_{subnode.name.value}_"
                 sub_type_vars, new_subnode = self.remove_type_parameters(subnode, prefix=prefix)
                 replacemences[subnode] = FlattenSentinel([*sub_type_vars, new_subnode])
-        
+
         new_node = new_node.visit(ReplaceTransformer(replacemences))
         return FlattenSentinel([*type_vars, new_node])
-
-
-
```

### Comparing `pyfuture-0.0.8/pyfuture/codemod/utils.py` & `pyfuture-0.0.9/pyfuture/codemod/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,72 @@
+from __future__ import annotations
+
 import libcst as cst
 
 
-def gen_type_param(type_param: cst.TypeVar | cst.TypeVarTuple | cst.ParamSpec, type_name: cst.Name|None=None) -> cst.SimpleStatementLine:
+def gen_type_param(
+    type_param: cst.TypeVar | cst.TypeVarTuple | cst.ParamSpec, type_name: cst.Name | None = None
+) -> cst.SimpleStatementLine:
     """
     To generate the following code:
         T = cst.TypeVar("T")
         P = cst.ParamSpec("P")
         Ts = cst.TypeVarTuple("Ts")
     """
     type_name = type_param.name if type_name is None else type_name
     match type_param:
         case cst.TypeVar(_, bound):
             args = [
                 cst.Arg(cst.SimpleString(f'"{type_name.value}"')),
             ]
             if bound is not None:
                 args.append(cst.Arg(bound, keyword=cst.Name("bound")))
-            return cst.SimpleStatementLine([cst.Assign(
-                targets=[cst.AssignTarget(type_name)],
-                value=cst.Call(
-                    func=cst.Name("TypeVar"),
-                    args=args,
-                ),
-            )])
-        case _: # cst.TypeVarTuple | cst.ParamSpec
-            return cst.SimpleStatementLine([cst.Assign(
-                targets=[cst.AssignTarget(type_name)],
-                value=cst.Call(
-                    func=cst.Name(type_param.__class__.__name__),
-                    args=[
-                        cst.Arg(cst.SimpleString(f'"{type_name.value}"')),
-                    ],
-                ),
-            )])
+            return cst.SimpleStatementLine(
+                [
+                    cst.Assign(
+                        targets=[cst.AssignTarget(type_name)],
+                        value=cst.Call(
+                            func=cst.Name("TypeVar"),
+                            args=args,
+                        ),
+                    )
+                ]
+            )
+        case _:  # cst.TypeVarTuple | cst.ParamSpec
+            return cst.SimpleStatementLine(
+                [
+                    cst.Assign(
+                        targets=[cst.AssignTarget(type_name)],
+                        value=cst.Call(
+                            func=cst.Name(type_param.__class__.__name__),
+                            args=[
+                                cst.Arg(cst.SimpleString(f'"{type_name.value}"')),
+                            ],
+                        ),
+                    )
+                ]
+            )
 
 
 def gen_func_wrapper(node: cst.FunctionDef, type_vars: list[cst.SimpleStatementLine]) -> cst.FunctionDef:
     wrapper = cst.FunctionDef(
-        name=cst.Name(
-            value=f'__wrapper_func_{node.name.value}'
-        ),
+        name=cst.Name(value=f"__wrapper_func_{node.name.value}"),
         params=cst.Parameters(),
         body=cst.IndentedBlock(
             body=[
                 *type_vars,
                 node,
-                cst.SimpleStatementLine([
-                    cst.Return(
-                        value=cst.Name(
-                            value=node.name.value,
-                            lpar=[],
-                            rpar=[],
-                        )
-                    ),
-                ])
+                cst.SimpleStatementLine(
+                    [
+                        cst.Return(
+                            value=cst.Name(
+                                value=node.name.value,
+                                lpar=[],
+                                rpar=[],
+                            )
+                        ),
+                    ]
+                ),
             ]
-        )
+        ),
     )
     return wrapper
```

### Comparing `pyfuture-0.0.8/pyfuture/utils.py` & `pyfuture-0.0.9/pyfuture/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from libcst.codemod import CodemodContext, Codemod
-import libcst as cst
+from __future__ import annotations
+
 from pathlib import Path
 
+import libcst as cst
+from libcst.codemod import Codemod, CodemodContext
+
 
 def transform_code(
     transformers: list[Codemod],
     code: str,
 ) -> str:
     """
     Transform code with some transformers, and return the transformed code.
@@ -21,34 +24,34 @@
     *,
     target: tuple[int, int] = (3, 8),
 ) -> str:
     """
     Transfer code to specified target version of python.
     """
     from .codemod import TransformTypeParametersCommand
-    assert target >= (3, 8), "Only support transfer to python 3.8+"
-    new_code = code
-    if target <= (3, 11):
-        new_code = transform_code(
-            transformers=[
-                TransformTypeParametersCommand(CodemodContext()),
-                # TODO: Add more codemods here
-            ],
-            code=code,
-        )
+
+    assert target[0] == 3, "Only support python3"
+    new_code = transform_code(
+        transformers=[
+            TransformTypeParametersCommand(CodemodContext()),
+            # TODO: Add more codemods here
+        ],
+        code=code,
+    )
     return new_code
 
+
 def transfer_file(
     src_file: Path,
     tgt_file: Path,
     *,
     target: tuple[int, int] = (3, 8),
 ):
     """
     Transfer code from src_file and write to tgt_file.
     """
     with src_file.open("r") as f:
         code = f.read()
-    
+
     tgt_file.parent.mkdir(parents=True, exist_ok=True)
     with tgt_file.open("w") as f:
         f.write(transfer_code(code, target=target))
```

