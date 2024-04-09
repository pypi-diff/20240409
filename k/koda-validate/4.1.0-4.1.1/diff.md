# Comparing `tmp/koda_validate-4.1.0.tar.gz` & `tmp/koda_validate-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koda_validate-4.1.0.tar", max compression
+gzip compressed data, was "koda_validate-4.1.1.tar", max compression
```

## Comparing `koda_validate-4.1.0.tar` & `koda_validate-4.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2022-11-03 18:16:51.567158 koda_validate-4.1.0/LICENSE
--rw-r--r--   0        0        0     2232 2024-03-01 06:09:43.188765 koda_validate-4.1.0/README.md
--rw-r--r--   0        0        0     4047 2023-01-26 17:18:47.114550 koda_validate-4.1.0/koda_validate/__init__.py
--rw-r--r--   0        0        0      530 2023-01-06 17:18:37.761331 koda_validate-4.1.0/koda_validate/_generics.py
--rw-r--r--   0        0        0     9711 2024-01-05 06:25:05.217385 koda_validate-4.1.0/koda_validate/_internal.py
--rw-r--r--   0        0        0     6660 2023-02-15 05:59:52.040690 koda_validate-4.1.0/koda_validate/base.py
--rw-r--r--   0        0        0      710 2023-01-26 17:18:47.115821 koda_validate-4.1.0/koda_validate/boolean.py
--rw-r--r--   0        0        0     1078 2023-01-26 17:18:47.116685 koda_validate-4.1.0/koda_validate/bytes.py
--rw-r--r--   0        0        0     1021 2023-01-26 17:18:47.117371 koda_validate-4.1.0/koda_validate/coerce.py
--rw-r--r--   0        0        0    10575 2023-06-02 04:23:57.311418 koda_validate-4.1.0/koda_validate/dataclasses.py
--rw-r--r--   0        0        0     1149 2023-01-26 17:18:47.118653 koda_validate-4.1.0/koda_validate/decimal.py
--rw-r--r--   0        0        0    37827 2023-01-26 17:18:47.119280 koda_validate-4.1.0/koda_validate/dictionary.py
--rw-r--r--   0        0        0     2745 2023-01-26 17:18:47.121473 koda_validate-4.1.0/koda_validate/errors.py
--rw-r--r--   0        0        0      717 2023-01-26 17:18:47.122263 koda_validate-4.1.0/koda_validate/float.py
--rw-r--r--   0        0        0     8800 2023-01-26 17:18:47.122699 koda_validate-4.1.0/koda_validate/generic.py
--rw-r--r--   0        0        0      703 2023-01-26 17:18:47.123314 koda_validate-4.1.0/koda_validate/integer.py
--rw-r--r--   0        0        0      870 2023-01-26 17:18:47.123562 koda_validate-4.1.0/koda_validate/is_type.py
--rw-r--r--   0        0        0     5238 2024-01-05 06:23:26.443766 koda_validate-4.1.0/koda_validate/list.py
--rw-r--r--   0        0        0     1882 2023-01-06 17:18:37.764592 koda_validate-4.1.0/koda_validate/maybe.py
--rw-r--r--   0        0        0    10489 2023-10-16 05:51:19.383326 koda_validate-4.1.0/koda_validate/namedtuple.py
--rw-r--r--   0        0        0     2252 2023-01-26 17:18:47.125138 koda_validate-4.1.0/koda_validate/none.py
--rw-r--r--   0        0        0        0 2022-11-03 18:16:51.571853 koda_validate-4.1.0/koda_validate/py.typed
--rw-r--r--   0        0        0      391 2023-01-06 17:18:37.765156 koda_validate-4.1.0/koda_validate/serialization/__init__.py
--rw-r--r--   0        0        0      207 2023-01-06 17:18:37.765285 koda_validate-4.1.0/koda_validate/serialization/base.py
--rw-r--r--   0        0        0     7836 2023-10-16 05:51:19.383535 koda_validate-4.1.0/koda_validate/serialization/errors.py
--rw-r--r--   0        0        0    18918 2023-01-06 17:18:37.765683 koda_validate-4.1.0/koda_validate/serialization/json_schema.py
--rw-r--r--   0        0        0     5670 2023-01-26 17:18:47.125990 koda_validate-4.1.0/koda_validate/set.py
--rw-r--r--   0        0        0    18981 2023-06-02 04:23:57.311920 koda_validate-4.1.0/koda_validate/signature.py
--rw-r--r--   0        0        0     1536 2023-01-26 17:18:47.127516 koda_validate-4.1.0/koda_validate/string.py
--rw-r--r--   0        0        0     1898 2023-01-26 17:18:47.127962 koda_validate-4.1.0/koda_validate/time.py
--rw-r--r--   0        0        0    19128 2023-02-15 05:59:52.041629 koda_validate-4.1.0/koda_validate/tuple.py
--rw-r--r--   0        0        0     9980 2023-01-26 17:18:47.129305 koda_validate-4.1.0/koda_validate/typeddict.py
--rw-r--r--   0        0        0     7653 2023-01-26 17:18:47.129793 koda_validate-4.1.0/koda_validate/typehints.py
--rw-r--r--   0        0        0     6796 2023-02-15 05:59:52.047051 koda_validate-4.1.0/koda_validate/union.py
--rw-r--r--   0        0        0     1055 2023-01-26 17:18:47.130250 koda_validate-4.1.0/koda_validate/uuid.py
--rw-r--r--   0        0        0     1667 2024-03-01 06:09:43.189959 koda_validate-4.1.0/koda_validate/valid.py
--rw-r--r--   0        0        0     2750 2024-03-01 06:09:43.190445 koda_validate-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 koda_validate-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-09 16:50:30.314818 koda_validate-4.1.1/LICENSE
+-rw-r--r--   0        0        0     2232 2024-04-09 16:50:30.314975 koda_validate-4.1.1/README.md
+-rw-r--r--   0        0        0     4047 2024-04-09 16:50:30.326056 koda_validate-4.1.1/koda_validate/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-09 16:50:30.326147 koda_validate-4.1.1/koda_validate/_generics.py
+-rw-r--r--   0        0        0     9711 2024-04-09 16:50:30.326306 koda_validate-4.1.1/koda_validate/_internal.py
+-rw-r--r--   0        0        0     6660 2024-04-09 16:50:30.326411 koda_validate-4.1.1/koda_validate/base.py
+-rw-r--r--   0        0        0      710 2024-04-09 16:50:30.326538 koda_validate-4.1.1/koda_validate/boolean.py
+-rw-r--r--   0        0        0     1078 2024-04-09 16:50:30.326651 koda_validate-4.1.1/koda_validate/bytes.py
+-rw-r--r--   0        0        0     1021 2024-04-09 16:50:30.326776 koda_validate-4.1.1/koda_validate/coerce.py
+-rw-r--r--   0        0        0    10575 2024-04-09 16:50:30.326892 koda_validate-4.1.1/koda_validate/dataclasses.py
+-rw-r--r--   0        0        0     1149 2024-04-09 16:50:30.326992 koda_validate-4.1.1/koda_validate/decimal.py
+-rw-r--r--   0        0        0    37827 2024-04-09 16:50:30.327135 koda_validate-4.1.1/koda_validate/dictionary.py
+-rw-r--r--   0        0        0     2897 2024-04-09 16:50:30.329023 koda_validate-4.1.1/koda_validate/errors.py
+-rw-r--r--   0        0        0      717 2024-04-09 16:50:30.329092 koda_validate-4.1.1/koda_validate/float.py
+-rw-r--r--   0        0        0     8800 2024-04-09 16:50:30.329236 koda_validate-4.1.1/koda_validate/generic.py
+-rw-r--r--   0        0        0      703 2024-04-09 16:50:30.329387 koda_validate-4.1.1/koda_validate/integer.py
+-rw-r--r--   0        0        0      870 2024-04-09 16:50:30.329472 koda_validate-4.1.1/koda_validate/is_type.py
+-rw-r--r--   0        0        0     5238 2024-04-09 16:50:30.329593 koda_validate-4.1.1/koda_validate/list.py
+-rw-r--r--   0        0        0     1882 2024-04-09 16:50:30.329701 koda_validate-4.1.1/koda_validate/maybe.py
+-rw-r--r--   0        0        0    10489 2024-04-09 16:50:30.329865 koda_validate-4.1.1/koda_validate/namedtuple.py
+-rw-r--r--   0        0        0     2252 2024-04-09 16:50:30.329987 koda_validate-4.1.1/koda_validate/none.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:50:30.330064 koda_validate-4.1.1/koda_validate/py.typed
+-rw-r--r--   0        0        0      391 2024-04-09 16:50:30.330164 koda_validate-4.1.1/koda_validate/serialization/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-09 16:50:30.330264 koda_validate-4.1.1/koda_validate/serialization/base.py
+-rw-r--r--   0        0        0     7836 2024-04-09 16:50:30.330380 koda_validate-4.1.1/koda_validate/serialization/errors.py
+-rw-r--r--   0        0        0    18918 2024-04-09 16:50:30.330503 koda_validate-4.1.1/koda_validate/serialization/json_schema.py
+-rw-r--r--   0        0        0     5670 2024-04-09 16:50:30.330876 koda_validate-4.1.1/koda_validate/set.py
+-rw-r--r--   0        0        0    19197 2024-04-09 16:50:30.330997 koda_validate-4.1.1/koda_validate/signature.py
+-rw-r--r--   0        0        0     1528 2024-04-09 17:24:45.436029 koda_validate-4.1.1/koda_validate/string.py
+-rw-r--r--   0        0        0     1898 2024-04-09 16:50:30.331240 koda_validate-4.1.1/koda_validate/time.py
+-rw-r--r--   0        0        0    19128 2024-04-09 16:50:30.331359 koda_validate-4.1.1/koda_validate/tuple.py
+-rw-r--r--   0        0        0     9980 2024-04-09 16:50:30.332274 koda_validate-4.1.1/koda_validate/typeddict.py
+-rw-r--r--   0        0        0     7653 2024-04-09 16:50:30.332397 koda_validate-4.1.1/koda_validate/typehints.py
+-rw-r--r--   0        0        0     6780 2024-04-09 16:50:30.332514 koda_validate-4.1.1/koda_validate/union.py
+-rw-r--r--   0        0        0     1055 2024-04-09 16:50:30.332597 koda_validate-4.1.1/koda_validate/uuid.py
+-rw-r--r--   0        0        0     1667 2024-04-09 16:50:30.332712 koda_validate-4.1.1/koda_validate/valid.py
+-rw-r--r--   0        0        0     2758 2024-04-09 17:24:45.436645 koda_validate-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 koda_validate-4.1.1/PKG-INFO
```

### Comparing `koda_validate-4.1.0/LICENSE` & `koda_validate-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/README.md` & `koda_validate-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/__init__.py` & `koda_validate-4.1.1/koda_validate/__init__.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/_generics.py` & `koda_validate-4.1.1/koda_validate/_generics.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/_internal.py` & `koda_validate-4.1.1/koda_validate/_internal.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/base.py` & `koda_validate-4.1.1/koda_validate/base.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/boolean.py` & `koda_validate-4.1.1/koda_validate/boolean.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/bytes.py` & `koda_validate-4.1.1/koda_validate/bytes.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/coerce.py` & `koda_validate-4.1.1/koda_validate/coerce.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/dataclasses.py` & `koda_validate-4.1.1/koda_validate/dataclasses.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/decimal.py` & `koda_validate-4.1.1/koda_validate/decimal.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/dictionary.py` & `koda_validate-4.1.1/koda_validate/dictionary.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/errors.py` & `koda_validate-4.1.1/koda_validate/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,13 +157,15 @@
     CoercionErr,
     ContainerErr,
     ExtraKeysErr,
     IndexErrs,
     KeyErrs,
     MapErr,
     MissingKeyErr,
-    PredicateErrs,
+    # This seems like a type exception worth making..., but that might change in the
+    # future. This is backwards compatible with existing code
+    PredicateErrs[Any],
     SetErrs,
     TypeErr,
     ValidationErrBase,
     UnionErrs,
 ]
```

### Comparing `koda_validate-4.1.0/koda_validate/float.py` & `koda_validate-4.1.1/koda_validate/float.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/generic.py` & `koda_validate-4.1.1/koda_validate/generic.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/integer.py` & `koda_validate-4.1.1/koda_validate/integer.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/is_type.py` & `koda_validate-4.1.1/koda_validate/is_type.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/list.py` & `koda_validate-4.1.1/koda_validate/list.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/maybe.py` & `koda_validate-4.1.1/koda_validate/maybe.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/namedtuple.py` & `koda_validate-4.1.1/koda_validate/namedtuple.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/none.py` & `koda_validate-4.1.1/koda_validate/none.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/serialization/errors.py` & `koda_validate-4.1.1/koda_validate/serialization/errors.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/serialization/json_schema.py` & `koda_validate-4.1.1/koda_validate/serialization/json_schema.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/set.py` & `koda_validate-4.1.1/koda_validate/set.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/signature.py` & `koda_validate-4.1.1/koda_validate/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,19 +377,21 @@
         typehint_resolver=typehint_resolver,
         overrides=overrides or {},
     )
 
     if func is None:
 
         def inner(func_inner: _DecoratedFunc) -> _DecoratedFunc:
-            return _wrap_fn_partial(func_inner)
+            # there may be a good way to replace this cast with ParamSpec in the future
+            return cast(_DecoratedFunc, _wrap_fn_partial(func_inner))
 
         return inner
     else:
-        return _wrap_fn_partial(func)
+        # there may be a good way to replace this cast with ParamSpec in the future
+        return cast(_DecoratedFunc, _wrap_fn_partial(func))
 
 
 def _trunc_str(s: str, max_chars: int) -> str:
     ellip = "..."
     ellip_len = len(ellip)
     if max_chars < ellip_len:
         raise AssertionError(f"max_chars must be greater than or equal to {ellip_len}")
```

### Comparing `koda_validate-4.1.0/koda_validate/string.py` & `koda_validate-4.1.1/koda_validate/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 
 @dataclass
 class RegexPredicate(Predicate[str]):
     pattern: Pattern[str]
 
     def __call__(self, val: str) -> bool:
-        return re.match(self.pattern, val) is not None
+        return self.pattern.match(val) is not None
 
 
 @dataclass
 class EmailPredicate(Predicate[str]):
     pattern: Pattern[str] = re.compile("[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\\.[a-zA-Z0-9-.]+")
 
     def __call__(self, val: str) -> bool:
-        return re.match(self.pattern, val) is not None
+        return self.pattern.match(val) is not None
```

### Comparing `koda_validate-4.1.0/koda_validate/time.py` & `koda_validate-4.1.1/koda_validate/time.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/tuple.py` & `koda_validate-4.1.1/koda_validate/tuple.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/typeddict.py` & `koda_validate-4.1.1/koda_validate/typeddict.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/typehints.py` & `koda_validate-4.1.1/koda_validate/typehints.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/union.py` & `koda_validate-4.1.1/koda_validate/union.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
                 validator_5,
                 validator_6,
                 validator_7,
                 validator_8,
             ]
             if v
         ]
-        return UnionValidator(validator_1, *validators)  # type: ignore
+        return UnionValidator(validator_1, *validators)
 
     @staticmethod
     def untyped(
         validator_1: Validator[Any], *validators: Validator[Any]
     ) -> "UnionValidator[Any]":
         r"""
         Can handle any number of variant :class:`Validator<koda_validate.Validator>``\s
```

### Comparing `koda_validate-4.1.0/koda_validate/uuid.py` & `koda_validate-4.1.1/koda_validate/uuid.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/koda_validate/valid.py` & `koda_validate-4.1.1/koda_validate/valid.py`

 * *Files identical despite different names*

### Comparing `koda_validate-4.1.0/pyproject.toml` & `koda_validate-4.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koda-validate"
-version = "4.1.0"
+version = "4.1.1"
 readme = "README.md"
 description = "Typesafe, composable validation"
 documentation = "https://koda-validate.readthedocs.io/en/stable/"
 authors = ["Keith Philpott"]
 license = "MIT"
 homepage = "https://github.com/keithasaurus/koda-validate"
 keywords = ["validation", "type hints", "asyncio", "serialization", "typesafe", "validate", "validators", "predicate", "processor"]
@@ -23,36 +23,36 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 koda = "1.4.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.4.2"
-pyright = "1.1.329"
+pytest = "8.0.2"
+pyright = "1.1.352"
 pytest-cov = "4.1.0"
-isort = "5.12.0"
-flake8 = "6.1.0"
+isort = "5.13.2"
+flake8 = "7.0.0"
 pre-commit = "3.4.0"
-mypy = "1.5.1"
-pydantic = "2.4.1"
-pytest-asyncio = "0.21.1"
-voluptuous = "0.13.1"
-ssort = "0.11.6"
-jsonschema = "4.19.1"
-types-jsonschema = "4.19.0.3"
+mypy = "1.8.0"
+pydantic = "2.6.3"
+pytest-asyncio = "0.23.5"
+voluptuous = "0.14.2"
+ssort = "0.12.4"
+jsonschema = "4.21.1"
+types-jsonschema = "4.21.0.20240118"
 sphinx = "6.2.1"
 furo = "2023.9.10"
-flask = {version = "2.3.3", extras = ["async"]}
-django = "4.2.5"
-django-stubs = "4.2.4"
-pytest-django = "4.5.2"
+flask = {version = "3.0.2", extras = ["async"]}
+django = "4.2.10"
+django-stubs = "4.2.7"
+pytest-django = "4.8.0"
 sphinx-autodoc-typehints = "1.23.0"
 darglint = "1.8.1"
-black = "23.9.1"
+black = "24.2.0"
 
 [tool.mypy]
 exclude = ["build", "bench"]
 allow_redefinition = false
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
```

### Comparing `koda_validate-4.1.0/PKG-INFO` & `koda_validate-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koda-validate
-Version: 4.1.0
+Version: 4.1.1
 Summary: Typesafe, composable validation
 Home-page: https://github.com/keithasaurus/koda-validate
 License: MIT
 Keywords: validation,type hints,asyncio,serialization,typesafe,validate,validators,predicate,processor
 Author: Keith Philpott
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

