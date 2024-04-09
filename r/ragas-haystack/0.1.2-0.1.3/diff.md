# Comparing `tmp/ragas_haystack-0.1.2.tar.gz` & `tmp/ragas_haystack-0.1.3.tar.gz`

## Comparing `ragas_haystack-0.1.2.tar` & `ragas_haystack-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/example/example.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/pydoc/config.yml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/src/haystack_integrations/components/evaluators/ragas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/src/haystack_integrations/components/evaluators/ragas/evaluator.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/src/haystack_integrations/components/evaluators/ragas/metrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/tests/test_evaluator.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/tests/test_metrics.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/README.md
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ragas_haystack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/example/example.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/pydoc/config.yml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/evaluator.py
+-rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/metrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    13780 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/test_evaluator.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/tests/test_metrics.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/README.md
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 ragas_haystack-0.1.3/PKG-INFO
```

### Comparing `ragas_haystack-0.1.2/example/example.py` & `ragas_haystack-0.1.3/example/example.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/pydoc/config.yml` & `ragas_haystack-0.1.3/pydoc/config.yml`

 * *Files 19% similar despite different names*

```diff
@@ -22,11 +22,12 @@
   excerpt: Ragas integration for Haystack
   category_slug: integrations-api
   title: Ragas
   slug: integrations-ragas
   order: 220
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_ragas.md
```

### Comparing `ragas_haystack-0.1.2/src/haystack_integrations/components/evaluators/ragas/evaluator.py` & `ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/evaluator.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/src/haystack_integrations/components/evaluators/ragas/metrics.py` & `ragas_haystack-0.1.3/src/haystack_integrations/components/evaluators/ragas/metrics.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/tests/test_evaluator.py` & `ragas_haystack-0.1.3/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/.gitignore` & `ragas_haystack-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/LICENSE.txt` & `ragas_haystack-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/README.md` & `ragas_haystack-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ragas_haystack-0.1.2/pyproject.toml` & `ragas_haystack-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["haystack-ai>=2.0.0b6", "ragas==0.1.1"]
+dependencies = ["haystack-ai", "ragas==0.1.1"]
 
 [project.urls]
 Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ragas"
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/ragas/README.md"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 
 [tool.hatch.build.targets.wheel]
@@ -57,20 +57,20 @@
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
 all = ["style", "typing"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -128,27 +128,28 @@
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
-source_pkgs = ["src", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
-[tool.coverage.paths]
-ragas_haystack = [
-  "src/haystack_integrations",
-  "*/ragas-haystack/src/ragas_haystack",
-]
-tests = ["tests"]
 
 [tool.coverage.report]
-exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
+exclude_lines = [
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
+]
+
 
 [[tool.mypy.overrides]]
 module = [
   "haystack.*",
   "pytest.*",
   "ragas.*",
   "numpy",
```

### Comparing `ragas_haystack-0.1.2/PKG-INFO` & `ragas_haystack-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ragas-haystack
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration of Ragas LLM evaluation framework with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/ragas
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/ragas/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: haystack-ai>=2.0.0b6
+Requires-Dist: haystack-ai
 Requires-Dist: ragas==0.1.1
 Description-Content-Type: text/markdown
 
 # ragas-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/ragas-haystack.svg)](https://pypi.org/project/ragas-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ragas-haystack.svg)](https://pypi.org/project/ragas-haystack)
```

