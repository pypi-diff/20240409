# Comparing `tmp/function_schema-0.3.0.tar.gz` & `tmp/function_schema-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function_schema-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "function_schema-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `function_schema-0.3.0.tar` & `function_schema-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     4208 2024-04-05 06:20:44.476863 function_schema-0.3.0/README.md
--rw-r--r--   0        0        0      192 2024-04-05 06:20:44.476863 function_schema-0.3.0/function_schema/__init__.py
--rw-r--r--   0        0        0     1338 2024-04-05 06:20:44.480863 function_schema-0.3.0/function_schema/cli.py
--rw-r--r--   0        0        0     5032 2024-04-05 06:20:44.480863 function_schema-0.3.0/function_schema/core.py
--rw-r--r--   0        0        0      872 2024-04-05 06:20:44.480863 function_schema-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 function_schema-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4208 2024-04-09 06:48:17.632099 function_schema-0.3.3/README.md
+-rw-r--r--   0        0        0      192 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/__init__.py
+-rw-r--r--   0        0        0     1338 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/cli.py
+-rw-r--r--   0        0        0     5964 2024-04-09 06:48:17.632099 function_schema-0.3.3/function_schema/core.py
+-rw-r--r--   0        0        0      872 2024-04-09 06:48:17.632099 function_schema-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 function_schema-0.3.3/PKG-INFO
```

### Comparing `function_schema-0.3.0/README.md` & `function_schema-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `function_schema-0.3.0/function_schema/cli.py` & `function_schema-0.3.3/function_schema/cli.py`

 * *Files identical despite different names*

### Comparing `function_schema-0.3.0/function_schema/core.py` & `function_schema-0.3.3/function_schema/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import enum
 import typing
 import inspect
+import platform
+import packaging.version
 
+current_version = packaging.version.parse(platform.python_version())
+py_310 = packaging.version.parse("3.10")
 
-class SchemaFormat(str, enum.Enum):
-    openai = "openai"
-    claude = "claude"
+if current_version >= py_310:
+    import types
+    from types import UnionType
+else:
+    UnionType = typing.Union  # type: ignore
 
 
 def get_function_schema(
     func: typing.Annotated[typing.Callable, "The function to get the schema for"],
     format: typing.Annotated[
-        typing.Optional[str], SchemaFormat, "The format of the schema to return"
+        typing.Optional[typing.Literal["openai", "claude"]],
+        "The format of the schema to return",
     ] = "openai",
 ) -> typing.Annotated[dict[str, typing.Any], "The JSON schema for the given function"]:
     """
     Returns a JSON schema for the given function.
 
     You can annotate your function parameters with the special Annotated type.
     Then get the schema for the function without writing the schema by hand.
@@ -62,15 +69,15 @@
     schema = {
         "type": "object",
         "properties": {},
         "required": [],
     }
     for name, param in params.items():
         param_args = typing.get_args(param.annotation)
-        is_annotated = len(param_args) > 1
+        is_annotated = typing.get_origin(param.annotation) is typing.Annotated
 
         enum_ = None
         default_value = inspect._empty
 
         if is_annotated:
             # first arg is type
             (T, *_) = param_args
@@ -80,40 +87,47 @@
                 (arg for arg in param_args if isinstance(arg, str)),
                 f"The {name} parameter",
             )
 
             # find enum in param_args tuple
             enum_ = next(
                 (
-                    arg
+                    [e.name for e in arg]
                     for arg in param_args
                     if isinstance(arg, type) and issubclass(arg, enum.Enum)
                 ),
-                None,
+                # use typing.Literal as enum if no enum found
+                typing.get_origin(T) is typing.Literal and typing.get_args(T) or None,
             )
         else:
             T = param.annotation
             description = f"The {name} parameter"
+            if typing.get_origin(T) is typing.Literal:
+                enum_ = typing.get_args(T)
 
         # find default value for param
         if param.default is not inspect._empty:
             default_value = param.default
 
         schema["properties"][name] = {
             "type": guess_type(T),
             "description": description,  # type: ignore
         }
 
         if enum_ is not None:
-            schema["properties"][name]["enum"] = [t.name for t in enum_]
+            schema["properties"][name]["enum"] = [t for t in enum_]
 
         if default_value is not inspect._empty:
             schema["properties"][name]["default"] = default_value
 
-        if not isinstance(None, T) and default_value is inspect._empty:
+        if (
+            typing.get_origin(T) is not typing.Literal
+            and not isinstance(None, T)
+            and default_value is inspect._empty
+        ):
             schema["required"].append(name)
 
     parms_key = "input_schema" if format == "claude" else "parameters"
 
     return {
         "name": func.__name__,
         "description": inspect.getdoc(func),
@@ -124,30 +138,43 @@
 def guess_type(
     T: typing.Annotated[type, "The type to guess the JSON schema type for"],
 ) -> typing.Annotated[
     typing.Union[str, list[str]], "str | list of str that representing JSON schema type"
 ]:
     """Guesses the JSON schema type for the given python type."""
 
+    # special case
+    if T is typing.Any:
+        return {}
+
+    origin = typing.get_origin(T)
+
     # hacking around typing modules, `typing.Union` and `types.UnitonType`
-    union_types = typing.get_args(T)
-    if len(union_types) > 1:
+    if origin is typing.Union or origin is UnionType:
+        union_types = [t for t in typing.get_args(T) if t is not type(None)]
         _types = []
         for union_type in union_types:
             _types.append(guess_type(union_type))
         _types = [t for t in _types if t is not None]  # exclude None
 
         # number contains integer in JSON schema
         if "number" in _types and "integer" in _types:
             _types.remove("integer")
 
         if len(_types) == 1:
             return _types[0]
         return _types
 
+    if origin is typing.Literal:
+        return "string"
+    elif origin is list or origin is tuple:
+        return "array"
+    elif origin is dict:
+        return "object"
+
     if not isinstance(T, type):
         return
 
     if T.__name__ == "NoneType":
         return
 
     if issubclass(T, str):
```

### Comparing `function_schema-0.3.0/pyproject.toml` & `function_schema-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "function-schema"
-version = "0.3.0"
+version = "0.3.3"
 requires-python = ">= 3.9"
 description = "A small utility to generate JSON schemas for python functions."
 readme = "README.md"
 license = {text = "MIT License"}
 authors = [
   {name = "Changkyun Kim", email = "comfuture@gmail.com"}
 ]
```

### Comparing `function_schema-0.3.0/PKG-INFO` & `function_schema-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-schema
-Version: 0.3.0
+Version: 0.3.3
 Summary: A small utility to generate JSON schemas for python functions.
 Keywords: json-schema,function,documentation,openai,utility
 Author-email: Changkyun Kim <comfuture@gmail.com>
 Maintainer-email: Changkyun Kim <comfuture@gmail.com>
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```
