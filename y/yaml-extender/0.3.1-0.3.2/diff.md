# Comparing `tmp/yaml-extender-0.3.1.tar.gz` & `tmp/yaml-extender-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-extender-0.3.1.tar", last modified: Thu Oct 12 17:22:16 2023, max compression
+gzip compressed data, was "yaml-extender-0.3.2.tar", last modified: Tue Apr  9 17:17:09 2024, max compression
```

## Comparing `yaml-extender-0.3.1.tar` & `yaml-extender-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.438975 yaml-extender-0.3.1/
--rw-rw-rw-   0        0        0     2584 2023-10-12 17:21:22.000000 yaml-extender-0.3.1/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9271 2023-10-12 17:22:16.437974 yaml-extender-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6813 2023-08-31 17:43:33.000000 yaml-extender-0.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.412951 yaml-extender-0.3.1/docs/
--rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.3.1/docs/conf.py
--rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-12 17:22:16.438975 yaml-extender-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.401409 yaml-extender-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.417955 yaml-extender-0.3.1/src/yaml_extender/
--rw-rw-rw-   0        0        0       68 2023-10-12 17:11:59.000000 yaml-extender-0.3.1/src/yaml_extender/__init__.py
--rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.3.1/src/yaml_extender/__main__.py
--rw-rw-rw-   0        0        0     1552 2023-08-18 15:41:34.000000 yaml-extender-0.3.1/src/yaml_extender/cli.py
--rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.3.1/src/yaml_extender/logger.py
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.436972 yaml-extender-0.3.1/src/yaml_extender/resolver/
--rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/__init__.py
--rw-rw-rw-   0        0        0     5898 2023-08-31 17:43:33.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/include_resolver.py
--rw-rw-rw-   0        0        0     2577 2023-08-18 16:09:52.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/inline_loop_resolver.py
--rw-rw-rw-   0        0        0     3748 2023-10-10 17:19:58.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/loop_resolver.py
--rw-rw-rw-   0        0        0     8097 2023-10-12 16:46:32.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/reference_resolver.py
--rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.3.1/src/yaml_extender/resolver/resolver.py
--rw-rw-rw-   0        0        0      680 2023-08-31 17:43:33.000000 yaml-extender-0.3.1/src/yaml_extender/xyml_exception.py
--rw-rw-rw-   0        0        0     2198 2023-08-18 16:34:41.000000 yaml-extender-0.3.1/src/yaml_extender/xyml_file.py
--rw-rw-rw-   0        0        0     1412 2023-08-17 17:16:14.000000 yaml-extender-0.3.1/src/yaml_extender/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-10-12 17:22:16.432969 yaml-extender-0.3.1/src/yaml_extender.egg-info/
--rw-rw-rw-   0        0        0     9271 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      802 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-10-12 17:22:16.000000 yaml-extender-0.3.1/src/yaml_extender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.200619 yaml-extender-0.3.2/
+-rw-rw-rw-   0        0        0     2616 2023-10-12 17:26:13.000000 yaml-extender-0.3.2/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1507 2023-01-31 17:42:46.000000 yaml-extender-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      364 2022-11-12 09:32:28.000000 yaml-extender-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     9271 2024-04-09 17:17:09.200619 yaml-extender-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6813 2023-08-31 17:43:33.000000 yaml-extender-0.3.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.135925 yaml-extender-0.3.2/docs/
+-rw-rw-rw-   0        0        0     6717 2022-11-12 09:32:28.000000 yaml-extender-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1373 2023-01-31 18:53:09.000000 yaml-extender-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 17:17:09.200619 yaml-extender-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.126918 yaml-extender-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.161562 yaml-extender-0.3.2/src/yaml_extender/
+-rw-rw-rw-   0        0        0       68 2024-04-09 17:15:47.000000 yaml-extender-0.3.2/src/yaml_extender/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-02-02 18:58:26.000000 yaml-extender-0.3.2/src/yaml_extender/__main__.py
+-rw-rw-rw-   0        0        0     1596 2024-04-09 17:13:38.000000 yaml-extender-0.3.2/src/yaml_extender/cli.py
+-rw-rw-rw-   0        0        0      796 2022-11-12 14:08:22.000000 yaml-extender-0.3.2/src/yaml_extender/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.198617 yaml-extender-0.3.2/src/yaml_extender/resolver/
+-rw-rw-rw-   0        0        0        0 2022-11-17 17:18:02.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/__init__.py
+-rw-rw-rw-   0        0        0     5898 2023-08-31 17:43:33.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/include_resolver.py
+-rw-rw-rw-   0        0        0     2577 2023-08-18 16:09:52.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/inline_loop_resolver.py
+-rw-rw-rw-   0        0        0     3748 2023-10-10 17:19:58.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/loop_resolver.py
+-rw-rw-rw-   0        0        0     8767 2024-04-09 17:14:39.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/reference_resolver.py
+-rw-rw-rw-   0        0        0      683 2023-02-27 18:52:59.000000 yaml-extender-0.3.2/src/yaml_extender/resolver/resolver.py
+-rw-rw-rw-   0        0        0      680 2023-08-31 17:43:33.000000 yaml-extender-0.3.2/src/yaml_extender/xyml_exception.py
+-rw-rw-rw-   0        0        0     2198 2023-08-18 16:34:41.000000 yaml-extender-0.3.2/src/yaml_extender/xyml_file.py
+-rw-rw-rw-   0        0        0     1412 2023-08-17 17:16:14.000000 yaml-extender-0.3.2/src/yaml_extender/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-09 17:17:09.199618 yaml-extender-0.3.2/src/yaml_extender.egg-info/
+-rw-rw-rw-   0        0        0     9271 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-09 17:17:09.000000 yaml-extender-0.3.2/src/yaml_extender.egg-info/top_level.txt
```

### Comparing `yaml-extender-0.3.1/CHANGELOG.rst` & `yaml-extender-0.3.2/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Changelog
 =========
 
 Version 0.3.1, 2023-10-12
 -----------------------
 
-- Bugfix: Using references as default values works now as expected.
-- Bugfix: For loops should now resolve correctly if given as part of a dictionary.
-- Bugfix: For loops will not reverse the order of the elements.
-- Bugfix: Referencing lists in other lists will now extend the lists correctly.
+- Bugfix: Using references as default values works now as expected. Issue#6
+- Bugfix: For loops should now resolve correctly if given as part of a dictionary. Issue#2
+- Bugfix: For loops will not reverse the order of the elements. Issue#4
+- Bugfix: Referencing lists in other lists will now extend the lists correctly. Issue#5
 
 Tests:
 - Added: Added tests for above fixes
 - Bugfix: Fixed problem with system test being cwd dependent.
 
 Version 0.3.0, 2023-08-31
 -----------------------
```

### Comparing `yaml-extender-0.3.1/LICENSE` & `yaml-extender-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/PKG-INFO` & `yaml-extender-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.3.1/README.rst` & `yaml-extender-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/docs/conf.py` & `yaml-extender-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/pyproject.toml` & `yaml-extender-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/cli.py` & `yaml-extender-0.3.2/src/yaml_extender/cli.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import argparse
-import sys
-
-from pathlib import Path
-from typing import List, Dict
-
-from yaml_extender import yaml_loader
-from yaml_extender.resolver import reference_resolver
-from yaml_extender.xyml_file import XYmlFile
-from yaml_extender.logger import get_logger
-
-LOGGER = get_logger()
-
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument("input", help="Input yaml file to be parsed", type=Path)
-    parser.add_argument("output", help="Output file to save to", type=Path)
-    parser.add_argument("-i", "--include", help="Include paths", type=Path, action="append")
-    parser.add_argument("--sort-keys", help="When set output file will have keys sorted", action="store_true")
-    args, unknown_args = parser.parse_known_args()
-
-    if not args.input.is_file:
-        raise FileNotFoundError(f"Path {args.input} is no valid file.")
-    additional_args = parse_unknown_args(unknown_args)
-    LOGGER.info("Additional parameters:\n" + "\n".join([f"{k}: {v}" for k, v in additional_args.items()]))
-    xyml_file = XYmlFile(args.input, additional_args, args.include)
-    output_dir: Path = args.output.parent
-    output_dir.mkdir(exist_ok=True, parents=True)
-    xyml_file.save(args.output, args.sort_keys)
-    return 0
-
-
-def parse_unknown_args(args: List) -> Dict:
-    arg_dict = dict(zip(args[:-1:2], args[1::2]))
-    ret_val = {}
-    # Parse numbers from strings
-    for k, v in arg_dict.items():
-        ret_val[k.strip("-")] = yaml_loader.parse_any_value(v)
-    return ret_val
-
-
-if __name__ == "__main__":
-    sys.exit(main())
+import argparse
+import sys
+
+from pathlib import Path
+from typing import List, Dict
+
+from yaml_extender import yaml_loader
+from yaml_extender.resolver import reference_resolver
+from yaml_extender.xyml_file import XYmlFile
+from yaml_extender.logger import get_logger
+
+LOGGER = get_logger()
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument("input", help="Input yaml file to be parsed", type=Path)
+    parser.add_argument("output", help="Output file to save to", type=Path)
+    parser.add_argument("-i", "--include", help="Include paths", type=Path, action="append")
+    parser.add_argument("--sort-keys", help="When set output file will have keys sorted", action="store_true")
+    args, unknown_args = parser.parse_known_args()
+
+    if not args.input.is_file:
+        raise FileNotFoundError(f"Path {args.input} is no valid file.")
+    additional_args = parse_unknown_args(unknown_args)
+    LOGGER.info("Additional parameters:\n" + "\n".join([f"{k}: {v}" for k, v in additional_args.items()]))
+    xyml_file = XYmlFile(args.input, additional_args, args.include)
+    output_dir: Path = args.output.parent
+    output_dir.mkdir(exist_ok=True, parents=True)
+    xyml_file.save(args.output, args.sort_keys)
+    return 0
+
+
+def parse_unknown_args(args: List) -> Dict:
+    arg_dict = dict(zip(args[:-1:2], args[1::2]))
+    ret_val = {}
+    # Parse numbers from strings
+    for k, v in arg_dict.items():
+        ret_val[k.strip("-")] = yaml_loader.parse_any_value(v)
+    return ret_val
+
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `yaml-extender-0.3.1/src/yaml_extender/logger.py` & `yaml-extender-0.3.2/src/yaml_extender/logger.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/resolver/include_resolver.py` & `yaml-extender-0.3.2/src/yaml_extender/resolver/include_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/resolver/inline_loop_resolver.py` & `yaml-extender-0.3.2/src/yaml_extender/resolver/inline_loop_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/resolver/loop_resolver.py` & `yaml-extender-0.3.2/src/yaml_extender/resolver/loop_resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/resolver/reference_resolver.py` & `yaml-extender-0.3.2/src/yaml_extender/resolver/reference_resolver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,193 +1,202 @@
-from __future__ import annotations
-
-import re
-from pathlib import Path
-from typing import Any, Optional
-
-from yaml_extender import yaml_loader
-from yaml_extender.resolver.resolver import Resolver
-from yaml_extender.xyml_exception import RecursiveReferenceError, ReferenceNotFoundError, ExtYamlSyntaxError
-
-REFERENCE_REGEX = r'\{\{(.+?)(?::(.*))?\}\}'
-ARRAY_REGEX = r'(.*)?\[(\d*)\]'
-LIST_FLATTEN_CHARACTER = " "
-
-MAXIMUM_REFERENCE_DEPTH = 30
-
-
-class ArithmeticOperation:
-
-    SUPPORTED_FUNCS = {"+": lambda x, y: x + y,
-                       "-": lambda x, y: x - y,
-                       "*": lambda x, y: x * y,
-                       "/": lambda x, y: x / y}
-    ARITHMETIC_REGEX = r'(.+)([' + ''.join(["\\" + k for k in SUPPORTED_FUNCS.keys()]) + r'])\s*(\d+)'
-
-    def __init__(self, reference: str, operation: str, value: str):
-        self.reference = reference.strip()
-        self.operation = operation.strip()
-        self.value = yaml_loader.parse_numeric_value(value.strip())
-
-    def __repr__(self):
-        return f"{self.reference} {self.operation} {self.value}"
-
-    def apply(self, value):
-        num_val = yaml_loader.parse_numeric_value(value)
-        return ArithmeticOperation.SUPPORTED_FUNCS[self.operation](self.value, num_val)
-
-    @staticmethod
-    def parse(expression: str) -> Optional[ArithmeticOperation]:
-        match = re.search(ArithmeticOperation.ARITHMETIC_REGEX, expression)
-        if match:
-            return ArithmeticOperation(match[1], match[2], match[3])
-        else:
-            return None
-
-
-class ReferenceResolver(Resolver):
-
-    def __init__(self, fail_on_resolve: bool = True):
-        super().__init__(fail_on_resolve)
-
-    def _Resolver__resolve(self, cur_value: Any, config: dict):
-        """Resolves all references in a given value using the provided content dict"""
-        new_value = cur_value
-        if isinstance(cur_value, dict):
-            for k in cur_value.keys():
-                cur_value[k] = self._Resolver__resolve(cur_value[k], config)
-        elif isinstance(cur_value, list):
-            new_list = []
-            for i, x in enumerate(cur_value):
-                resolved_value = self._Resolver__resolve(x, config)
-                if isinstance(resolved_value, list):
-                    # If the returned value is also a list, extend the current list with it
-                    new_list.extend(resolved_value)
-                else:
-                    new_list.append(self._Resolver__resolve(x, config))
-            new_value = new_list
-        else:
-            new_value = self.resolve_reference(cur_value, config)
-        return new_value
-
-    @staticmethod
-    def parse_references(value: str):
-        """
-        Returns a tuple (full_match, ref_name, default_value) for each occurrence of a xyml reference statement.
-        Excludes nested statements
-        """
-        # Todo: If this would be a generator function would it increase performance?
-        findings = []
-        start_idx = value.find("{{")
-        while start_idx != -1:
-            start_idx += 2
-            start_idx_2 = value.find("{{", start_idx)
-            end_idx = value.find("}}", start_idx)
-            while start_idx_2 != -1 and start_idx_2 < end_idx:
-                end_idx = value.find("}}", end_idx + 2)
-                start_idx_2 = value.find("{{", start_idx_2 + 2)
-            # Store finding
-            full_ref = value[start_idx-2:end_idx+2]
-            ref = value[start_idx:end_idx]    # +2 to strip brackets
-            if ":" in ref:
-                findings.append([full_ref] + [x.strip() for x in ref.split(":", maxsplit=1)])
-            else:
-                findings.append([full_ref, ref.strip(), None])
-            # Continue finding refs
-            start_idx = value.find("{{", end_idx)
-        return findings
-
-    def resolve_reference(self, value: Any, config: dict, depth: int = 0) -> Any:
-        if not isinstance(value, str) or "{" not in value:
-            return value
-        if depth > 30:
-            raise RecursiveReferenceError(value)
-        new_value = value
-        # In order to store the full match the whole regex is packed into a group
-        for ref_match in ReferenceResolver.parse_references(value):
-            ref = ref_match[1]
-            default_value = ref_match[2]
-            if default_value is not None:
-                default_value = yaml_loader.parse_any_value(default_value.strip())
-            # Resolve arithmetic operation
-            operation = ArithmeticOperation.parse(ref)
-            if operation:
-                ref = operation.reference
-            # Resolve reference, including subrefs
-            try:
-                ref_val = self.resolve_subrefs(ref, config)
-            except ReferenceNotFoundError as ref_err:
-                if default_value is not None:
-                    ref_val = default_value
-                elif self.fail_on_resolve:
-                    raise ref_err
-                else:
-                    ref_val = None
-
-            if ref_val is not None:
-                if operation:
-                    ref_val = operation.apply(ref_val)
-                # Check if the reference to be resolved is part of a string.
-                if ref_match[0] == value:
-                    # Preserve float & int and list types if reference is part of a string
-                    new_value = ref_val
-                else:
-                    # If resolved value is of type list, flatten it
-                    if isinstance(ref_val, list):
-                        ref_val = LIST_FLATTEN_CHARACTER.join(ref_val)
-                    # Replace the reference string within the value
-                    new_value = new_value.replace(ref_match[0], str(ref_val))
-
-        if new_value == value:
-            if self.fail_on_resolve:
-                raise ReferenceNotFoundError(value)
-            else:
-                return value
-
-        # Resolve recursive references
-        new_value = self.resolve_reference(new_value, config, depth + 1)
-        return new_value
-
-    def resolve_subrefs(self, fullref: str, current_config: dict):
-        if not fullref:
-            return current_config
-        if "." in fullref:
-            ref, sub_ref = fullref.split(".", maxsplit=1)
-        else:
-            ref = fullref
-            sub_ref = None
-        # If subref is specifying more than config can resolve, e.g. for include parameter dicts
-        # And the resolved value is another reference, append the subref and resolve later
-        if isinstance(current_config, str):
-            match = re.match(REFERENCE_REGEX, current_config)
-            if match:
-                # If the current config represents another reference and there are more subrefs specified
-                # then extend the reference by the remaining subref
-                current_config = match.group(1).strip()
-                if match.group(2):
-                    current_config += f":{match.group(2)}"
-                return "{{" + current_config + f".{fullref}" + "}}"
-            else:
-                # Fail, because the reference specifies more than can be resolved
-                raise ReferenceNotFoundError(fullref)
-        elif isinstance(current_config, list):
-            if ref.isdigit():
-                if len(current_config) > int(ref):
-                    current_config = current_config[int(ref)]
-                else:
-                    raise ReferenceNotFoundError(fullref, ref)
-            else:
-                # Resolve list of dicts
-                value_list = []
-                for elem in current_config:
-                    try:
-                        value_list.append(self.resolve_subrefs(fullref, elem))
-                    except ReferenceNotFoundError:
-                        pass
-                return value_list
-        else:
-            if ref in current_config:
-                current_config = current_config[ref]
-            else:
-                # Fail, because the reference cannot be found in config
-                raise ReferenceNotFoundError(fullref)
-        return self.resolve_subrefs(sub_ref, current_config)
+from __future__ import annotations
+
+import re
+from pathlib import Path
+from typing import Any, Optional
+
+from yaml_extender import yaml_loader
+# from yaml_extender.resolver.inline_loop_resolver import LOOP_KEY
+from yaml_extender.resolver.resolver import Resolver
+from yaml_extender.xyml_exception import RecursiveReferenceError, ReferenceNotFoundError, ExtYamlSyntaxError
+
+REFERENCE_REGEX = r'\{\{(.+?)(?::(.*))?\}\}'
+ARRAY_REGEX = r'(.*)?\[(\d*)\]'
+LIST_FLATTEN_CHARACTER = " "
+LOOP_KEY = "xyml.for"
+
+MAXIMUM_REFERENCE_DEPTH = 30
+
+
+class ArithmeticOperation:
+
+    SUPPORTED_FUNCS = {"+": lambda x, y: x + y,
+                       "-": lambda x, y: x - y,
+                       "*": lambda x, y: x * y,
+                       "/": lambda x, y: x / y}
+    ARITHMETIC_REGEX = r'(.+)([' + ''.join(["\\" + k for k in SUPPORTED_FUNCS.keys()]) + r'])\s*(\d+)'
+
+    def __init__(self, reference: str, operation: str, value: str):
+        self.reference = reference.strip()
+        self.operation = operation.strip()
+        self.value = yaml_loader.parse_numeric_value(value.strip())
+
+    def __repr__(self):
+        return f"{self.reference} {self.operation} {self.value}"
+
+    def apply(self, value):
+        num_val = yaml_loader.parse_numeric_value(value)
+        return ArithmeticOperation.SUPPORTED_FUNCS[self.operation](self.value, num_val)
+
+    @staticmethod
+    def parse(expression: str) -> Optional[ArithmeticOperation]:
+        match = re.search(ArithmeticOperation.ARITHMETIC_REGEX, expression)
+        if match:
+            return ArithmeticOperation(match[1], match[2], match[3])
+        else:
+            return None
+
+
+class ReferenceResolver(Resolver):
+
+    def __init__(self, fail_on_resolve: bool = True):
+        super().__init__(fail_on_resolve)
+
+    def _Resolver__resolve(self, cur_value: Any, config: dict):
+        """Resolves all references in a given value using the provided content dict"""
+        new_value = cur_value
+        if isinstance(cur_value, dict):
+            for k in cur_value.keys():
+                cur_value[k] = self._Resolver__resolve(cur_value[k], config)
+        elif isinstance(cur_value, list):
+            new_list = []
+            for i, x in enumerate(cur_value):
+                resolved_value = self._Resolver__resolve(x, config)
+                if isinstance(resolved_value, list):
+                    # If the returned value is also a list, extend the current list with it
+                    new_list.extend(resolved_value)
+                else:
+                    new_list.append(self._Resolver__resolve(x, config))
+            new_value = new_list
+        else:
+            new_value = self.resolve_reference(cur_value, config)
+        return new_value
+
+    @staticmethod
+    def parse_references(value: str):
+        """
+        Returns a tuple (full_match, ref_name, default_value) for each occurrence of a xyml reference statement.
+        Excludes nested statements
+        """
+        # Todo: If this would be a generator function would it increase performance?
+        findings = []
+        start_idx = value.find("{{")
+        while start_idx != -1:
+            start_idx += 2
+            start_idx_2 = value.find("{{", start_idx)
+            end_idx = value.find("}}", start_idx)
+            while start_idx_2 != -1 and start_idx_2 < end_idx:
+                end_idx = value.find("}}", end_idx + 2)
+                start_idx_2 = value.find("{{", start_idx_2 + 2)
+            # Store finding
+            full_ref = value[start_idx-2:end_idx+2]
+            ref = value[start_idx:end_idx]    # +2 to strip brackets
+            if ":" in ref:
+                findings.append([full_ref] + [x.strip() for x in ref.split(":", maxsplit=1)])
+            else:
+                findings.append([full_ref, ref.strip(), None])
+            # Continue finding refs
+            start_idx = value.find("{{", end_idx)
+        return findings
+
+    def resolve_reference(self, value: Any, config: dict, depth: int = 0) -> Any:
+        if not isinstance(value, str) or "{" not in value:
+            return value
+        if depth > 30:
+            raise RecursiveReferenceError(value)
+        new_value = value
+        count_loop_refs = 0
+        # In order to store the full match the whole regex is packed into a group
+        ref_matches = ReferenceResolver.parse_references(value)
+        for ref_match in ref_matches:
+            ref = ref_match[1]
+            if ref == LOOP_KEY:
+                # an inline loop is a special reference, don't try to resolve now
+                count_loop_refs += 1
+                continue
+            default_value = ref_match[2]
+            if default_value is not None:
+                default_value = yaml_loader.parse_any_value(default_value.strip())
+            # Resolve arithmetic operation
+            operation = ArithmeticOperation.parse(ref)
+            if operation:
+                ref = operation.reference
+            # Resolve reference, including subrefs
+            try:
+                ref_val = self.resolve_subrefs(ref, config)
+            except ReferenceNotFoundError as ref_err:
+                if default_value is not None:
+                    ref_val = default_value
+                elif self.fail_on_resolve:
+                    raise ref_err
+                else:
+                    ref_val = None
+
+            if ref_val is not None:
+                if operation:
+                    ref_val = operation.apply(ref_val)
+                # Check if the reference to be resolved is part of a string.
+                if ref_match[0] == value:
+                    # Preserve float & int and list types if reference is part of a string
+                    new_value = ref_val
+                else:
+                    # If resolved value is of type list, flatten it
+                    if isinstance(ref_val, list):
+                        ref_val = LIST_FLATTEN_CHARACTER.join(ref_val)
+                    # Replace the reference string within the value
+                    new_value = new_value.replace(ref_match[0], str(ref_val))
+
+        if new_value == value:
+            if self.fail_on_resolve and len(ref_matches) > count_loop_refs:
+                # if the amount of references is the same as amount of inline loops, its not an error
+                raise ReferenceNotFoundError(value)
+            else:
+                return value
+
+        # Resolve recursive references
+        new_value = self.resolve_reference(new_value, config, depth + 1)
+        return new_value
+
+    def resolve_subrefs(self, fullref: str, current_config: dict):
+        if not fullref:
+            return current_config
+        if "." in fullref:
+            ref, sub_ref = fullref.split(".", maxsplit=1)
+        else:
+            ref = fullref
+            sub_ref = None
+        # If subref is specifying more than config can resolve, e.g. for include parameter dicts
+        # And the resolved value is another reference, append the subref and resolve later
+        if isinstance(current_config, str):
+            match = re.match(REFERENCE_REGEX, current_config)
+            if match:
+                # If the current config represents another reference and there are more subrefs specified
+                # then extend the reference by the remaining subref
+                current_config = match.group(1).strip()
+                if match.group(2):
+                    current_config += f":{match.group(2)}"
+                return "{{" + current_config + f".{fullref}" + "}}"
+            else:
+                # Fail, because the reference specifies more than can be resolved
+                raise ReferenceNotFoundError(fullref)
+        elif isinstance(current_config, list):
+            if ref.isdigit():
+                if len(current_config) > int(ref):
+                    current_config = current_config[int(ref)]
+                else:
+                    raise ReferenceNotFoundError(fullref, ref)
+            else:
+                # Resolve list of dicts
+                value_list = []
+                for elem in current_config:
+                    try:
+                        value_list.append(self.resolve_subrefs(fullref, elem))
+                    except ReferenceNotFoundError:
+                        pass
+                return value_list
+        else:
+            if ref in current_config:
+                current_config = current_config[ref]
+            else:
+                # Fail, because the reference cannot be found in config
+                raise ReferenceNotFoundError(fullref)
+        return self.resolve_subrefs(sub_ref, current_config)
```

### Comparing `yaml-extender-0.3.1/src/yaml_extender/resolver/resolver.py` & `yaml-extender-0.3.2/src/yaml_extender/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/xyml_exception.py` & `yaml-extender-0.3.2/src/yaml_extender/xyml_exception.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/xyml_file.py` & `yaml-extender-0.3.2/src/yaml_extender/xyml_file.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender/yaml_loader.py` & `yaml-extender-0.3.2/src/yaml_extender/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `yaml-extender-0.3.1/src/yaml_extender.egg-info/PKG-INFO` & `yaml-extender-0.3.2/src/yaml_extender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-extender
-Version: 0.3.1
+Version: 0.3.2
 Summary: Extends the common .yaml syntax to provide more complex configuration options
 Author-email: Simon Gallitscher <adun.sg@gmx.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Simon Gallitscher
         All rights reserved.
```

### Comparing `yaml-extender-0.3.1/src/yaml_extender.egg-info/SOURCES.txt` & `yaml-extender-0.3.2/src/yaml_extender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

