# Comparing `tmp/inline_snapshot-0.7.0.tar.gz` & `tmp/inline_snapshot-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.7.0.tar", max compression
+gzip compressed data, was "inline_snapshot-0.8.0.tar", max compression
```

## Comparing `inline_snapshot-0.7.0.tar` & `inline_snapshot-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.7.0/LICENSE
--rw-r--r--   0        0        0     4300 2024-02-22 21:02:35.561482 inline_snapshot-0.7.0/README.md
--rw-r--r--   0        0        0      176 2024-02-27 19:20:04.768585 inline_snapshot-0.7.0/inline_snapshot/__init__.py
--rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_config.py
--rw-r--r--   0        0        0     4944 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_external.py
--rw-r--r--   0        0        0     2779 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_find_external.py
--rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_format.py
--rw-r--r--   0        0        0    17642 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     5713 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.7.0/inline_snapshot/py.typed
--rw-r--r--   0        0        0     6355 2024-02-27 19:20:04.768585 inline_snapshot-0.7.0/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     2567 2024-02-27 19:20:04.768585 inline_snapshot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6169 1970-01-01 00:00:00.000000 inline_snapshot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-02-18 19:11:48.706993 inline_snapshot-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4300 2024-04-06 14:15:44.827781 inline_snapshot-0.8.0/README.md
+-rw-r--r--   0        0        0      176 2024-04-09 10:01:42.306682 inline_snapshot-0.8.0/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_align.py
+-rw-r--r--   0        0        0     5733 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_change.py
+-rw-r--r--   0        0        0      539 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_config.py
+-rw-r--r--   0        0        0     4944 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_external.py
+-rw-r--r--   0        0        0     2779 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_find_external.py
+-rw-r--r--   0        0        0      372 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    21488 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0      452 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_location.py
+-rw-r--r--   0        0        0     5911 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0       64 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_sentinels.py
+-rw-r--r--   0        0        0     3565 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-27 18:46:50.343219 inline_snapshot-0.8.0/inline_snapshot/py.typed
+-rw-r--r--   0        0        0     6477 2024-04-09 10:01:00.849766 inline_snapshot-0.8.0/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     2618 2024-04-09 10:01:42.330682 inline_snapshot-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6169 1970-01-01 00:00:00.000000 inline_snapshot-0.8.0/PKG-INFO
```

### Comparing `inline_snapshot-0.7.0/LICENSE` & `inline_snapshot-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.7.0/README.md` & `inline_snapshot-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.7.0/inline_snapshot/_config.py` & `inline_snapshot-0.8.0/inline_snapshot/_config.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.7.0/inline_snapshot/_external.py` & `inline_snapshot-0.8.0/inline_snapshot/_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.7.0/inline_snapshot/_find_external.py` & `inline_snapshot-0.8.0/inline_snapshot/_find_external.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.7.0/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.8.0/inline_snapshot/_inline_snapshot.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 import ast
 import copy
 import inspect
-import io
 import sys
-import token
 import tokenize
-from collections import namedtuple
+from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Dict  # noqa
+from typing import Iterator
 from typing import overload
 from typing import Tuple  # noqa
 from typing import TypeVar
 
 from executing import Source
 
+from ._align import add_x
+from ._align import align
+from ._change import apply_all
+from ._change import Change
+from ._change import Delete
+from ._change import DictInsert
+from ._change import ListInsert
+from ._change import Replace
 from ._format import format_code
 from ._rewrite_code import ChangeRecorder
 from ._rewrite_code import end_of
 from ._rewrite_code import start_of
+from ._sentinels import undefined
+from ._utils import ignore_tokens
+from ._utils import normalize_strings
+from ._utils import simple_token
+from ._utils import value_to_token
 
 
-# sentinels
-class Undefined:
+class NotImplementedYet(Exception):
     pass
 
 
-undefined = Undefined()
-
 snapshots = {}  # type: Dict[Tuple[int, int], Snapshot]
 
 _active = False
 
 _files_with_snapshots = set()
 
 
@@ -66,23 +75,40 @@
     return _update_flags.fix or _update_flags.update
 
 
 class GenericValue:
     _new_value: Any
     _old_value: Any
     _current_op = "undefined"
+    _ast_node: ast.Expr
+    _source: Source
 
-    def _needs_trim(self):
-        return False
+    def _token_of_node(self, node):
 
-    def _needs_create(self):
-        return self._old_value == undefined
+        return list(
+            normalize_strings(
+                [
+                    simple_token(t.type, t.string)
+                    for t in self._source.asttokens().get_tokens(node)
+                    if t.type not in ignore_tokens
+                ]
+            )
+        )
 
-    def _needs_fix(self):
-        raise NotImplemented
+    def _format(self, text):
+        if self._source is None:
+            return text
+        else:
+            return format_code(text, Path(self._source.filename))
+
+    def _token_to_code(self, tokens):
+        return self._format(tokenize.untokenize(tokens)).strip()
+
+    def _value_to_code(self, value):
+        return self._token_to_code(value_to_token(value))
 
     def _ignore_old(self):
         return (
             _update_flags.fix
             or _update_flags.update
             or _update_flags.create
             or self._old_value is undefined
@@ -90,16 +116,19 @@
 
     def _visible_value(self):
         if self._ignore_old():
             return self._new_value
         else:
             return self._old_value
 
-    def get_result(self, flags):
-        return self._old_value
+    def _get_changes(self) -> Iterator[Change]:
+        raise NotImplementedYet()
+
+    def _new_code(self):
+        raise NotImplementedYet()
 
     def __repr__(self):
         return repr(self._visible_value())
 
     def _type_error(self, op):
         __tracebackhide__ = True
         raise TypeError(
@@ -124,23 +153,48 @@
 
     def __getitem__(self, _item):
         __tracebackhide__ = True
         self._type_error("snapshot[key]")
 
 
 class UndecidedValue(GenericValue):
-    def __init__(self, _old_value):
-        self._old_value = _old_value
+    def __init__(self, old_value, ast_node, source):
+        self._old_value = old_value
         self._new_value = undefined
+        self._ast_node = ast_node
+        self._source = source
 
     def _change(self, cls):
         self.__class__ = cls
 
-    def _needs_fix(self):
-        return False
+    def _new_code(self):
+        return ""
+
+    def _get_changes(self) -> Iterator[Change]:
+        # generic fallback
+        new_token = value_to_token(self._old_value)
+
+        if (
+            self._ast_node is not None
+            and self._token_of_node(self._ast_node) != new_token
+        ):
+            flag = "update"
+        else:
+            return
+
+        new_code = self._token_to_code(new_token)
+
+        yield Replace(
+            node=self._ast_node,
+            source=self._source,
+            new_code=new_code,
+            flag=flag,
+            old_value=self._old_value,
+            new_value=self._old_value,
+        )
 
     # functions which determine the type
 
     def __eq__(self, other):
         self._change(EqValue)
         return self == other
 
@@ -157,32 +211,177 @@
         return other in self
 
     def __getitem__(self, item):
         self._change(DictValue)
         return self[item]
 
 
+try:
+    import dirty_equals  # type: ignore
+except:
+
+    def update_allowed(value):
+        return True
+
+else:
+
+    def update_allowed(value):
+        return not isinstance(value, dirty_equals.DirtyEquals)
+
+
 class EqValue(GenericValue):
     _current_op = "x == snapshot"
 
     def __eq__(self, other):
         other = copy.deepcopy(other)
 
         if self._new_value is undefined:
             self._new_value = other
 
         return self._visible_value() == other
 
-    def _needs_fix(self):
-        return self._old_value is not undefined and self._old_value != self._new_value
+    def _new_code(self):
+        return self._value_to_code(self._new_value)
 
-    def get_result(self, flags):
-        if flags.fix and self._needs_fix() or flags.create and self._needs_create():
-            return self._new_value
-        return self._old_value
+    def _get_changes(self) -> Iterator[Change]:
+
+        assert self._old_value is not undefined
+
+        def check(old_value, old_node, new_value):
+
+            if (
+                isinstance(old_node, ast.List)
+                and isinstance(new_value, list)
+                and isinstance(old_value, list)
+                or isinstance(old_node, ast.Tuple)
+                and isinstance(new_value, tuple)
+                and isinstance(old_value, tuple)
+            ):
+                diff = add_x(align(old_value, new_value))
+                old = zip(old_value, old_node.elts)
+                new = iter(new_value)
+                old_position = 0
+                to_insert = defaultdict(list)
+                for c in diff:
+                    if c in "mx":
+                        old_value_element, old_node_element = next(old)
+                        new_value_element = next(new)
+                        yield from check(
+                            old_value_element, old_node_element, new_value_element
+                        )
+                        old_position += 1
+                    elif c == "i":
+                        new_value_element = next(new)
+                        new_code = self._value_to_code(new_value_element)
+                        to_insert[old_position].append((new_code, new_value_element))
+                    elif c == "d":
+                        old_value_element, old_node_element = next(old)
+                        yield Delete(
+                            "fix", self._source, old_node_element, old_value_element
+                        )
+                        old_position += 1
+                    else:
+                        assert False
+
+                for position, code_values in to_insert.items():
+                    yield ListInsert(
+                        "fix", self._source, old_node, position, *zip(*code_values)
+                    )
+
+                return
+
+            elif (
+                isinstance(old_node, ast.Dict)
+                and isinstance(new_value, dict)
+                and isinstance(old_value, dict)
+                and len(old_value) == len(old_node.keys)
+            ):
+                for value, node in zip(old_value.keys(), old_node.keys):
+                    assert node is not None
+
+                    try:
+                        # this is just a sanity check, dicts should be ordered
+                        node_value = ast.literal_eval(node)
+                    except:
+                        continue
+                    assert node_value == value
+
+                for key, node in zip(old_value.keys(), old_node.values):
+                    if key in new_value:
+                        # check values with same keys
+                        yield from check(old_value[key], node, new_value[key])
+                    else:
+                        # delete entries
+                        yield Delete("fix", self._source, node, old_value[key])
+
+                to_insert = []
+                insert_pos = 0
+                for key, new_value_element in new_value.items():
+                    if key not in old_value:
+                        # add new values
+                        to_insert.append((key, new_value_element))
+                    else:
+                        if to_insert:
+                            new_code = [
+                                (self._value_to_code(k), self._value_to_code(v))
+                                for k, v in to_insert
+                            ]
+                            yield DictInsert(
+                                "fix",
+                                self._source,
+                                old_node,
+                                insert_pos,
+                                new_code,
+                                to_insert,
+                            )
+                            to_insert = []
+                        insert_pos += 1
+
+                if to_insert:
+                    new_code = [
+                        (self._value_to_code(k), self._value_to_code(v))
+                        for k, v in to_insert
+                    ]
+                    yield DictInsert(
+                        "fix",
+                        self._source,
+                        old_node,
+                        len(old_node.values),
+                        new_code,
+                        to_insert,
+                    )
+
+                return
+
+            # generic fallback
+            new_token = value_to_token(new_value)
+
+            if not old_value == new_value:
+                flag = "fix"
+            elif (
+                self._ast_node is not None
+                and self._token_of_node(old_node) != new_token
+                and update_allowed(old_value)
+            ):
+                flag = "update"
+            else:
+                return
+
+            new_code = self._token_to_code(new_token)
+
+            yield Replace(
+                node=old_node,
+                source=self._source,
+                new_code=new_code,
+                flag=flag,
+                old_value=old_value,
+                new_value=new_value,
+            )
+
+        yield from check(self._old_value, self._ast_node, self._new_value)
 
 
 class MinMaxValue(GenericValue):
     """Generic implementation for <=, >="""
 
     @staticmethod
     def cmp(a, b):
@@ -196,36 +395,41 @@
         else:
             self._new_value = (
                 self._new_value if self.cmp(self._new_value, other) else other
             )
 
         return self.cmp(self._visible_value(), other)
 
-    def _needs_trim(self):
-        if self._old_value is undefined:
-            return False
-
-        return not self.cmp(self._new_value, self._old_value)
-
-    def _needs_fix(self):
-        if self._old_value is undefined:
-            return False
-        return not self.cmp(self._old_value, self._new_value)
-
-    def get_result(self, flags):
-        if flags.create and self._needs_create():
-            return self._new_value
+    def _new_code(self):
+        return self._value_to_code(self._new_value)
 
-        if flags.fix and self._needs_fix():
-            return self._new_value
+    def _get_changes(self) -> Iterator[Change]:
+        new_token = value_to_token(self._new_value)
+        if not self.cmp(self._old_value, self._new_value):
+            flag = "fix"
+        elif not self.cmp(self._new_value, self._old_value):
+            flag = "trim"
+        elif (
+            self._ast_node is not None
+            and self._token_of_node(self._ast_node) != new_token
+        ):
+            flag = "update"
+        else:
+            return
 
-        if flags.trim and self._needs_trim():
-            return self._new_value
+        new_code = self._token_to_code(new_token)
 
-        return self._old_value
+        yield Replace(
+            node=self._ast_node,
+            source=self._source,
+            new_code=new_code,
+            flag=flag,
+            old_value=self._old_value,
+            new_value=self._new_value,
+        )
 
 
 class MinValue(MinMaxValue):
     """
     handles:
 
     >>> snapshot(5) <= 6
@@ -279,88 +483,130 @@
                 self._new_value.append(item)
 
         if ignore_old_value() or self._old_value is undefined:
             return True
         else:
             return item in self._old_value
 
-    def _needs_trim(self):
-        if self._old_value is undefined:
-            return False
-        return any(item not in self._new_value for item in self._old_value)
-
-    def _needs_fix(self):
-        if self._old_value is undefined:
-            return False
-        return any(item not in self._old_value for item in self._new_value)
+    def _new_code(self):
+        return self._value_to_code(self._new_value)
 
-    def get_result(self, flags):
-        if (flags.fix and flags.trim) or (flags.create and self._needs_create()):
-            return self._new_value
+    def _get_changes(self) -> Iterator[Change]:
 
-        if self._old_value is not undefined:
-            if flags.fix:
-                return self._old_value + [
-                    v for v in self._new_value if v not in self._old_value
-                ]
+        if self._ast_node is None:
+            elements = [None] * len(self._old_value)
+        else:
+            assert isinstance(self._ast_node, ast.List)
+            elements = self._ast_node.elts
+
+        for old_value, old_node in zip(self._old_value, elements):
+            if old_value not in self._new_value:
+                yield Delete(
+                    flag="trim", source=self._source, node=old_node, old_value=old_value
+                )
+                continue
 
-            if flags.trim:
-                return [v for v in self._old_value if v in self._new_value]
+            # check for update
+            new_token = value_to_token(old_value)
 
-        return self._old_value
+            if old_node is not None and self._token_of_node(old_node) != new_token:
+                new_code = self._token_to_code(new_token)
+
+                yield Replace(
+                    node=old_node,
+                    source=self._source,
+                    new_code=new_code,
+                    flag="update",
+                    old_value=old_value,
+                    new_value=old_value,
+                )
+
+        new_values = [v for v in self._new_value if v not in self._old_value]
+        if new_values:
+            yield ListInsert(
+                flag="fix",
+                source=self._source,
+                node=self._ast_node,
+                position=len(self._old_value),
+                new_code=[self._value_to_code(v) for v in new_values],
+                new_values=new_values,
+            )
 
 
 class DictValue(GenericValue):
     _current_op = "snapshot[key]"
 
     def __getitem__(self, index):
         if self._new_value is undefined:
             self._new_value = {}
 
         old_value = self._old_value
         if old_value is undefined:
             old_value = {}
 
+        child_node = None
+        if self._ast_node is not None:
+            assert isinstance(self._ast_node, ast.Dict)
+            if index in old_value:
+                pos = list(old_value.keys()).index(index)
+                child_node = self._ast_node.values[pos]
+
         if index not in self._new_value:
-            self._new_value[index] = UndecidedValue(old_value.get(index, undefined))
+            self._new_value[index] = UndecidedValue(
+                old_value.get(index, undefined), child_node, self._source
+            )
 
         return self._new_value[index]
 
-    def _needs_fix(self):
-        if self._old_value is not undefined and self._new_value is not undefined:
-            if any(v._needs_fix() for v in self._new_value.values()):
-                return True
-
-        return False
-
-    def _needs_trim(self):
-        if self._old_value is not undefined and self._new_value is not undefined:
-            if any(v._needs_trim() for v in self._new_value.values()):
-                return True
-
-            return any(item not in self._new_value for item in self._old_value)
-        return False
-
-    def _needs_create(self):
-        if super()._needs_create():
-            return True
-
-        return any(item not in self._old_value for item in self._new_value)
+    def _new_code(self):
+        return (
+            "{"
+            + ", ".join(
+                [
+                    f"{self._value_to_code(k)}: {v._new_code()}"
+                    for k, v in self._new_value.items()
+                ]
+            )
+            + "}"
+        )
 
-    def get_result(self, flags):
-        result = {k: v.get_result(flags) for k, v in self._new_value.items()}
+    def _get_changes(self) -> Iterator[Change]:
 
-        result = {k: v for k, v in result.items() if v is not undefined}
+        assert self._old_value is not undefined
 
-        if not flags.trim and self._old_value is not undefined:
-            for k, v in self._old_value.items():
-                if k not in result:
-                    result[k] = v
+        if self._ast_node is None:
+            values = [None] * len(self._old_value)
+        else:
+            assert isinstance(self._ast_node, ast.Dict)
+            values = self._ast_node.values
 
-        return result
+        for key, node in zip(self._old_value.keys(), values):
+            if key in self._new_value:
+                # check values with same keys
+                yield from self._new_value[key]._get_changes()
+            else:
+                # delete entries
+                yield Delete("trim", self._source, node, self._old_value[key])
+
+        to_insert = []
+        for key, new_value_element in self._new_value.items():
+            if key not in self._old_value:
+                # add new values
+                to_insert.append((key, new_value_element._new_code()))
+
+        if to_insert:
+            new_code = [(self._value_to_code(k), v) for k, v in to_insert]
+            yield DictInsert(
+                "create",
+                self._source,
+                self._ast_node,
+                len(self._old_value),
+                new_code,
+                to_insert,
+            )
 
 
 T = TypeVar("T")
 
 found_snapshots = []
 
 
@@ -406,15 +652,15 @@
     The generated value will be inserted as argument to `snapshot()`
 
     >>> assert 5 == snapshot(5)
 
     `snapshot(value)` has the semantic of an noop which returns `value`.
     """
     if not _active:
-        if isinstance(obj, Undefined):
+        if obj is undefined:
             raise AssertionError(
                 "your snapshot is missing a value run pytest with --inline-snapshot=create"
             )
         else:
             return obj
 
     frame = inspect.currentframe().f_back.f_back
@@ -436,72 +682,14 @@
             assert node.func.id == "snapshot"
             snapshots[key] = Snapshot(obj, expr)
         found_snapshots.append(snapshots[key])
 
     return snapshots[key]._value
 
 
-ignore_tokens = (token.NEWLINE, token.ENDMARKER, token.NL)
-
-
-# based on ast.unparse
-def _str_literal_helper(string, *, quote_types):
-    """Helper for writing string literals, minimizing escapes.
-
-    Returns the tuple (string literal to write, possible quote types).
-    """
-
-    def escape_char(c):
-        # \n and \t are non-printable, but we only escape them if
-        # escape_special_whitespace is True
-        if c in "\n\t":
-            return c
-        # Always escape backslashes and other non-printable characters
-        if c == "\\" or not c.isprintable():
-            return c.encode("unicode_escape").decode("ascii")
-        if c == extra:
-            return "\\" + c
-        return c
-
-    extra = ""
-    if "'''" in string and '"""' in string:
-        extra = '"' if string.count("'") >= string.count('"') else "'"
-
-    escaped_string = "".join(map(escape_char, string))
-
-    possible_quotes = [q for q in quote_types if q not in escaped_string]
-
-    if escaped_string:
-        # Sort so that we prefer '''"''' over """\""""
-        possible_quotes.sort(key=lambda q: q[0] == escaped_string[-1])
-        # If we're using triple quotes and we'd need to escape a final
-        # quote, escape it
-        if possible_quotes[0][0] == escaped_string[-1]:
-            assert len(possible_quotes[0]) == 3
-            escaped_string = escaped_string[:-1] + "\\" + escaped_string[-1]
-    return escaped_string, possible_quotes
-
-
-def triple_quote(string):
-    """Write string literal value with a best effort attempt to avoid
-    backslashes."""
-    string, quote_types = _str_literal_helper(string, quote_types=['"""', "'''"])
-    quote_type = quote_types[0]
-
-    string = "\\\n" + string
-
-    if not string.endswith("\n"):
-        string = string + "\\\n"
-
-    return f"{quote_type}{string}{quote_type}"
-
-
-simple_token = namedtuple("simple_token", "type,string")
-
-
 def used_externals(tree):
     if sys.version_info < (3, 8):
         return [
             n.args[0].s
             for n in ast.walk(tree)
             if isinstance(n, ast.Call)
             and isinstance(n.func, ast.Name)
@@ -520,146 +708,57 @@
             and isinstance(n.args[0], ast.Constant)
         ]
 
 
 class Snapshot:
     def __init__(self, value, expr):
         self._expr = expr
-        self._value = UndecidedValue(value)
+        node = expr.node.args[0] if expr is not None and expr.node.args else None
+        source = expr.source if expr is not None else None
+        self._value = UndecidedValue(value, node, source)
         self._uses_externals = []
 
     @property
     def _filename(self):
         return self._expr.source.filename
 
-    def _format(self, text):
-        return format_code(text, Path(self._filename))
-
-    def _value_to_token(self, value):
-        if value is undefined:
-            return []
-        input = io.StringIO(self._format(repr(value)))
-
-        def map_string(tok):
-            """Convert strings with newlines in triple quoted strings."""
-            if tok.type == token.STRING:
-                s = ast.literal_eval(tok.string)
-                if isinstance(s, str) and "\n" in s:
-                    # unparse creates a triple quoted string here,
-                    # because it thinks that the string should be a docstring
-                    tripple_quoted_string = triple_quote(s)
-
-                    assert ast.literal_eval(tripple_quoted_string) == s
-
-                    return simple_token(tok.type, tripple_quoted_string)
-
-            return simple_token(tok.type, tok.string)
-
-        return [
-            map_string(t)
-            for t in tokenize.generate_tokens(input.readline)
-            if t.type not in ignore_tokens
-        ]
-
     def _change(self):
-        assert self._expr is not None
-
-        change = ChangeRecorder.current.new_change()
-
-        tokens = list(self._expr.source.asttokens().get_tokens(self._expr.node))
-        assert tokens[0].string == "snapshot"
-        assert tokens[1].string == "("
-        assert tokens[-1].string == ")"
-
-        change.set_tags("inline_snapshot")
-
-        needs_fix = self._value._needs_fix()
-        needs_create = self._value._needs_create()
-        needs_trim = self._value._needs_trim()
-        needs_update = self._needs_update()
-
-        if (
-            _update_flags.update
-            and needs_update
-            or _update_flags.fix
-            and needs_fix
-            or _update_flags.create
-            and needs_create
-            or _update_flags.trim
-            and needs_trim
-        ):
-            new_value = self._value.get_result(_update_flags)
 
-            text = self._format(
-                tokenize.untokenize(self._value_to_token(new_value))
-            ).strip()
-
-            try:
-                tree = ast.parse(text)
-            except:
+        if self._value._old_value is undefined:
+            if _update_flags.create:
+                new_code = self._value._new_code()
+                try:
+                    ast.parse(new_code)
+                except:
+                    return
+            else:
                 return
 
-            self._uses_externals = used_externals(tree)
+            assert self._expr is not None
 
+            tokens = list(self._expr.source.asttokens().get_tokens(self._expr.node))
+            assert tokens[0].string == "snapshot"
+            assert tokens[1].string == "("
+            assert tokens[-1].string == ")"
+
+            change = ChangeRecorder.current.new_change()
+            change.set_tags("inline_snapshot")
             change.replace(
                 (end_of(tokens[1]), start_of(tokens[-1])),
-                text,
+                new_code,
                 filename=self._filename,
             )
+            return
 
-    def _current_tokens(self):
-        if not self._expr.node.args:
-            return []
-
-        return [
-            simple_token(t.type, t.string)
-            for t in self._expr.source.asttokens().get_tokens(self._expr.node.args[0])
-            if t.type not in ignore_tokens
-        ]
-
-    def _normalize_strings(self, token_sequence):
-        """Normalize string concattenanion.
-
-        "a" "b" -> "ab"
-        """
-
-        current_string = None
-        for t in token_sequence:
-            if (
-                t.type == token.STRING
-                and not t.string.startswith(("'''", '"""', "b'''", 'b"""'))
-                and t.string.startswith(("'", '"', "b'", 'b"'))
-            ):
-                if current_string is None:
-                    current_string = ast.literal_eval(t.string)
-                else:
-                    current_string += ast.literal_eval(t.string)
-
-                continue
-
-            if current_string is not None:
-                yield (token.STRING, repr(current_string))
-                current_string = None
-
-            yield t
-
-        if current_string is not None:
-            yield (token.STRING, repr(current_string))
-
-    def _needs_update(self):
-        return self._expr is not None and [] != list(
-            self._normalize_strings(self._current_tokens())
-        ) != list(self._normalize_strings(self._value_to_token(self._value._old_value)))
+        changes = self._value._get_changes()
+        apply_all(
+            [change for change in changes if change.flag in _update_flags.to_set()]
+        )
 
     @property
     def _flags(self):
-        s = set()
-        if self._value._needs_fix():
-            s.add("fix")
-        if self._value._needs_trim():
-            s.add("trim")
-        if self._value._needs_create():
-            s.add("create")
-        if self._value._old_value is not undefined and self._needs_update():
-            s.add("update")
 
-        return s
+        if self._value._old_value is undefined:
+            return {"create"}
+
+        changes = self._value._get_changes()
+        return {change.flag for change in changes}
```

### Comparing `inline_snapshot-0.7.0/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.8.0/inline_snapshot/_rewrite_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,41 +113,49 @@
     def delete(self, node, *, filename):
         self.replace(node, "", filename=filename)
 
     def insert(self, node, new_content, *, filename):
         self.replace(start_of(node), new_content, filename=filename)
 
     def _replace(self, filename, range, new_contend):
-        self.change_recorder.get_source(filename).replacements.append(
+        source = self.change_recorder.get_source(filename)
+        source.replacements.append(
             Replacement(range=range, text=new_contend, change_id=self.change_id)
         )
+        source._check()
 
 
 class SourceFile:
     def __init__(self, filename):
         self.replacements: list[Replacement] = []
         self.filename = filename
 
     def rewrite(self):
         new_code = self.new_code()
 
         with open(self.filename, "bw") as code:
             code.write(new_code.encode())
 
-    def new_code(self):
-        """Returns the new file contend or None if there are no replacepents to
-        apply."""
+    def _check(self):
         replacements = list(self.replacements)
         replacements.sort()
 
         for r in replacements:
-            assert r.range.start <= r.range.end
+            assert r.range.start <= r.range.end, r
 
         for lhs, rhs in pairwise(replacements):
-            assert lhs.range.end <= rhs.range.start
+            assert lhs.range.end <= rhs.range.start, (lhs, rhs)
+
+    def new_code(self):
+        """Returns the new file contend or None if there are no replacepents to
+        apply."""
+        replacements = list(self.replacements)
+        replacements.sort()
+
+        self._check()
 
         code = self.filename.read_text("utf-8")
 
         is_formatted = code == format_code(code, self.filename)
 
         if not is_formatted:
             logging.info(f"file is not formatted with black: {self.filename}")
@@ -185,15 +193,15 @@
     @contextlib.contextmanager
     def activate(self):
         old_recorder = ChangeRecorder.current
         ChangeRecorder.current = self
         yield self
         ChangeRecorder.current = old_recorder
 
-    def get_source(self, filename):
+    def get_source(self, filename) -> SourceFile:
         filename = pathlib.Path(filename)
         if filename not in self._source_files:
             self._source_files[filename] = SourceFile(filename)
 
         return self._source_files[filename]
 
     def change_set(self):
```

### Comparing `inline_snapshot-0.7.0/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.8.0/inline_snapshot/pytest_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import ast
 from pathlib import Path
 
 import pytest
 
 from . import _config
 from . import _external
 from . import _find_external
 from . import _inline_snapshot
 from ._find_external import ensure_import
 from ._inline_snapshot import undefined
+from ._inline_snapshot import used_externals
 from ._rewrite_code import ChangeRecorder
 
 
 def pytest_addoption(parser):
     group = parser.getgroup("inline-snapshot")
 
     group.addoption(
@@ -158,24 +160,27 @@
 
         for snapshot in _inline_snapshot.snapshots.values():
             for flag in snapshot._flags:
                 assert flag in ("create", "fix", "trim", "update"), flag
                 count[flag] += 1
             snapshot._change()
 
-        ensure_external = set()
+        test_files = set()
         for snapshot in _inline_snapshot.snapshots.values():
-            if snapshot._uses_externals:
-                ensure_external.add(snapshot._filename)
+            test_files.add(Path(snapshot._filename))
 
-            for external_name in snapshot._uses_externals:
-                _external.storage.persist(external_name)
+        for test_file in test_files:
+            tree = ast.parse(recorder.get_source(test_file).new_code())
+            used = used_externals(tree)
+
+            if used:
+                ensure_import(test_file, {"inline_snapshot": ["external"]})
 
-        for filename in ensure_external:
-            ensure_import(filename, {"inline_snapshot": ["external"]})
+            for external_name in used:
+                _external.storage.persist(external_name)
 
         recorder.fix_all()
 
         def report_change(flags, msg):
             if count[flags]:
                 terminalreporter.write(msg.format(num=count[flags]) + "\n")
```

### Comparing `inline_snapshot-0.7.0/pyproject.toml` & `inline_snapshot-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -45,33 +45,35 @@
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 keywords = ["pytest", "testing", "snapshot", "approval", "golden-master"]
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.7.0"
+version = "0.8.0"
 
 [tool.poetry.dependencies]
 asttokens = ">=2.0.5"
 black = ">=23.3.0"
 click = ">=8.1.4"
 executing = ">=2.0.0"
 python = ">=3.7"
 toml = ">=0.10.2"
 types-toml = ">=0.10.8.7"
 
 [tool.poetry.group.dev.dependencies]
 coverage = ">=7.2.3"
 coverage-enable-subprocess = ">=1.0"
+dirty-equals = ">=0.7.0"
 hypothesis = ">=6.75.5"
 mypy = ">=1.2.0"
 pytest = ">=7.1"
 pytest-subtests = ">=0.11.0"
 pytest-xdist = {extras = ["psutil"], version = ">=3.2.1"}
+time-machine = ">=2.10.0"
 
 [tool.poetry.group.doc.dependencies]
 mkdocs = ">=1.4.2"
 mkdocs-material = {extras = ["imaging"], version = ">=8.5.10"}
 mkdocstrings = {extras = ["python-legacy"], version = ">=0.19.0"}
 
 [tool.poetry.plugins.pytest11]
```

### Comparing `inline_snapshot-0.7.0/PKG-INFO` & `inline_snapshot-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.7.0
+Version: 0.8.0
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Keywords: pytest,testing,snapshot,approval,golden-master
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7
```

