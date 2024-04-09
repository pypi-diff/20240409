# Comparing `tmp/pycep_parser-0.5.1a1.tar.gz` & `tmp/pycep_parser-0.5.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycep_parser-0.5.1a1.tar", max compression
+gzip compressed data, was "pycep_parser-0.5.1a2.tar", max compression
```

## Comparing `pycep_parser-0.5.1a1.tar` & `pycep_parser-0.5.1a2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10834 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/LICENSE
--rw-r--r--   0        0        0     1400 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/README.md
--rw-r--r--   0        0        0       57 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/__init__.py
--rw-r--r--   0        0        0    13703 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/bicep.lark
--rw-r--r--   0        0        0     1854 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/main.py
--rw-r--r--   0        0        0        0 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/py.typed
--rw-r--r--   0        0        0    59494 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/transformer.py
--rw-r--r--   0        0        0    26006 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/typing.py
--rw-r--r--   0        0        0      274 2023-11-05 20:34:30.617313 pycep_parser-0.5.1a1/pycep/validator.py
--rw-r--r--   0        0        0     1392 2023-11-05 20:34:39.937299 pycep_parser-0.5.1a1/pyproject.toml
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pycep_parser-0.5.1a1/PKG-INFO
+-rw-r--r--   0        0        0    10834 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/LICENSE
+-rw-r--r--   0        0        0     1400 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/README.md
+-rw-r--r--   0        0        0       57 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/__init__.py
+-rw-r--r--   0        0        0    13703 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/bicep.lark
+-rw-r--r--   0        0        0     1833 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/py.typed
+-rw-r--r--   0        0        0    59445 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/transformer.py
+-rw-r--r--   0        0        0    26006 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/typing.py
+-rw-r--r--   0        0        0      274 2024-04-09 12:33:25.568819 pycep_parser-0.5.1a2/pycep/validator.py
+-rw-r--r--   0        0        0     1921 2024-04-09 12:33:38.008909 pycep_parser-0.5.1a2/pyproject.toml
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pycep_parser-0.5.1a2/PKG-INFO
```

### Comparing `pycep_parser-0.5.1a1/LICENSE` & `pycep_parser-0.5.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a1/README.md` & `pycep_parser-0.5.1a2/README.md`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a1/pycep/bicep.lark` & `pycep_parser-0.5.1a2/pycep/bicep.lark`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a1/pycep/main.py` & `pycep_parser-0.5.1a2/pycep/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,11 +43,11 @@
             bicep_text = file_path.read_text()
         else:
             raise TypeError("Either 'text' or 'file_path' has to be set")
 
         if not BicepValidator.is_valid(bicep_text):
             if file_path:
                 raise ValueError(f"{file_path} file content is invalid")
-            else:
-                raise ValueError("Text is invalid")
+
+            raise ValueError("Text is invalid")
 
         return self.lark_parser.parse(bicep_text)
```

### Comparing `pycep_parser-0.5.1a1/pycep/transformer.py` & `pycep_parser-0.5.1a2/pycep/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 
 VALID_TARGET_SCOPES = {"resourceGroup", "subscription", "managementGroup", "tenant"}
 
 
 class BicepElement(str):
     """An alias to differentiate between a string and a Bicep element."""
 
-    pass
-
 
 class BicepToJson(Transformer[Token, pycep_typing.BicepJson]):
     def __init__(self, add_line_numbers: bool) -> None:
         self.add_line_numbers = add_line_numbers
 
         self.child_resources: list[pycep_typing.ResourceResponse] = []
 
@@ -194,15 +192,15 @@
         result: pycep_typing.ResourceResponse = {
             "resources": {
                 "__name__": name_str,
                 "__attrs__": {
                     "decorators": decorators if decorators else [],
                     "type": type_api_pair["type"],
                     "api_version": type_api_pair["api_version"],
-                    "existing": True if existing else False,
+                    "existing": bool(existing),
                     "config": config,
                 },
             }
         }
 
         if self.add_line_numbers:
             result["resources"]["__attrs__"]["__start_line__"] = meta.line
@@ -218,15 +216,15 @@
 
         result: pycep_typing.Resource = {
             "__name__": str(name),
             "__attrs__": {
                 "decorators": [],
                 "type": str(type_name)[1:-1],
                 "api_version": "",  # will be set later with the parent resource api version
-                "existing": True if existing else False,
+                "existing": bool(existing),
                 "config": config,
             },
         }
 
         if self.add_line_numbers:
             result["__attrs__"]["__start_line__"] = meta.line
             # remove one line, because the new line is counted for child resources
@@ -492,15 +490,15 @@
 
     def deco_metadata(self, args: tuple[dict[str, Any]]) -> pycep_typing.DecoratorMetadata:
         return {
             "type": "metadata",
             "argument": args[0],
         }
 
-    def deco_secure(self, _: Any) -> pycep_typing.DecoratorSecure:
+    def deco_secure(self, _: Any) -> pycep_typing.DecoratorSecure:  # noqa: ANN401
         return {
             "type": "secure",
         }
 
     ####################
     #
     # functions
@@ -1761,16 +1759,15 @@
     ####################
     #
     # data types
     #
     ####################
 
     def array(self, args: list[bool | int | Token]) -> list[bool | int | str]:
-        result = [item.value if isinstance(item, Token) else item for item in args]
-        return result
+        return [item.value if isinstance(item, Token) else item for item in args]
 
     def object(self, args: list[tuple[str, Any]]) -> dict[str, Any]:
         return dict(args)
 
     def pair(self, args: tuple[str, bool | int | Token]) -> tuple[str, bool | int | str]:
         key, value = args
         return key, value.value if isinstance(value, Token) else value
@@ -1778,29 +1775,27 @@
     def key(self, arg: tuple[Token]) -> str:
         return str(arg[0])
 
     def int(self, arg: tuple[Token]) -> int:
         return int(arg[0])
 
     def string(self, arg: tuple[Token]) -> str:
-        result = self.transform_string_token(arg[0])
-        return result
+        return self.transform_string_token(arg[0])
 
     def multi_line_string(self, arg: tuple[Token]) -> str:
         value = str(arg[0])[3:-3]
-        value = value[1:] if value.startswith("\n") else value
-        return value
+        return value[1:] if value.startswith("\n") else value
 
-    def true(self, _: Any) -> Literal[True]:
+    def true(self, _: Any) -> Literal[True]:  # noqa: ANN401
         return True
 
-    def false(self, _: Any) -> Literal[False]:
+    def false(self, _: Any) -> Literal[False]:  # noqa: ANN401
         return False
 
-    def null(self, _: Any) -> None:
+    def null(self, _: Any) -> None:  # noqa: ANN401
         return None
 
     ####################
     #
     # helper methods
     #
     ####################
@@ -1808,15 +1803,15 @@
     def process_child_resource(
         self, parent_resource_name: str, parent_type_api_pair: pycep_typing.ApiTypeVersion, config: dict[str, Any]
     ) -> None:
         """Extracts child resources from a resource config.
 
         Beware that this method is not idempotent, it modifies the passed in `config`.
         """
-        if "__child_resource__" in config.keys():
+        if "__child_resource__" in config:
             child_resource = config.pop("__child_resource__")
 
             # prefix the resource name with the parent to prevent overlap
             child_resource["__name__"] = f"{parent_resource_name}__{child_resource['__name__']}"
 
             # inherit type and api version info from parent resource
             child_type_api_pair: pycep_typing.ApiTypeVersion = {
```

### Comparing `pycep_parser-0.5.1a1/pycep/typing.py` & `pycep_parser-0.5.1a2/pycep/typing.py`

 * *Files identical despite different names*

### Comparing `pycep_parser-0.5.1a1/PKG-INFO` & `pycep_parser-0.5.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycep-parser
-Version: 0.5.1a1
+Version: 0.5.1a2
 Summary: A Python based Bicep parser
 Home-page: https://github.com/gruebel/pycep
 License: Apache-2.0
 Keywords: bicep,parser,lark
 Author: Anton Grübel
 Author-email: anton.gruebel@gmail.com
 Requires-Python: >=3.8,<4.0
```

