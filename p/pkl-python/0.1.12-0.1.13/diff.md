# Comparing `tmp/pkl-python-0.1.12.tar.gz` & `tmp/pkl-python-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkl-python-0.1.12.tar", last modified: Mon Apr  8 01:50:51 2024, max compression
+gzip compressed data, was "pkl-python-0.1.13.tar", last modified: Tue Apr  9 12:12:05 2024, max compression
```

## Comparing `pkl-python-0.1.12.tar` & `pkl-python-0.1.13.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1069 2024-03-29 10:49:37.000000 pkl-python-0.1.12/LICENSE
--rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5990 2024-04-08 01:50:51.334348 pkl-python-0.1.12/PKG-INFO
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     3849 2024-04-08 01:46:30.000000 pkl-python-0.1.12/README.md
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.330348 pkl-python-0.1.12/pkl/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        7 2024-04-08 01:49:57.000000 pkl-python-0.1.12/pkl/VERSION
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     3970 2024-04-06 04:01:45.000000 pkl-python-0.1.12/pkl/__init__.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)    12637 2024-04-06 04:02:48.000000 pkl-python-0.1.12/pkl/evaluator_manager.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     4841 2024-04-03 09:01:42.000000 pkl-python-0.1.12/pkl/evaluator_options.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     8111 2024-04-06 04:02:47.000000 pkl-python-0.1.12/pkl/msgapi.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     6260 2024-04-06 04:01:45.000000 pkl-python-0.1.12/pkl/parser.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1780 2024-04-03 06:30:38.000000 pkl-python-0.1.12/pkl/reader.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     4114 2024-04-04 07:59:33.000000 pkl-python-0.1.12/pkl/server.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      658 2024-04-05 18:01:12.000000 pkl-python-0.1.12/pkl/utils.py
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/pkl_python.egg-info/
--rw-r--r--   0 jwyang    (1002) jwyang    (1002)     5990 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/PKG-INFO
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      515 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/SOURCES.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        1 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/dependency_links.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)       79 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/requires.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)        4 2024-04-08 01:50:51.000000 pkl-python-0.1.12/pkl_python.egg-info/top_level.txt
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1131 2024-04-08 01:46:30.000000 pkl-python-0.1.12/pyproject.toml
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/scripts/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      978 2024-03-29 10:49:37.000000 pkl-python-0.1.12/scripts/download_binary.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      917 2024-03-29 10:49:37.000000 pkl-python-0.1.12/scripts/eval.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)       38 2024-04-08 01:50:51.334348 pkl-python-0.1.12/setup.cfg
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1939 2024-04-05 18:55:54.000000 pkl-python-0.1.12/setup.py
-drwxrwx---   0 jwyang    (1002) jwyang    (1002)        0 2024-04-08 01:50:51.334348 pkl-python-0.1.12/tests/
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      474 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_evaluator_manager.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      385 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_load.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      975 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_parser.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)     1756 2024-04-08 01:46:30.000000 pkl-python-0.1.12/tests/test_readers.py
--rw-rw----   0 jwyang    (1002) jwyang    (1002)      102 2024-04-02 21:06:36.000000 pkl-python-0.1.12/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:12:05.059921 pkl-python-0.1.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 12:11:49.000000 pkl-python-0.1.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-09 12:12:05.059921 pkl-python-0.1.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-09 12:11:49.000000 pkl-python-0.1.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-09 12:11:49.000000 pkl-python-0.1.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:12:05.059921 pkl-python-0.1.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 12:11:49.000000 pkl-python-0.1.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:12:05.051921 pkl-python-0.1.13/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:12:05.055921 pkl-python-0.1.13/src/pkl/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/evaluator_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/evaluator_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/msgapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 12:11:49.000000 pkl-python-0.1.13/src/pkl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:12:05.059921 pkl-python-0.1.13/src/pkl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 12:12:05.000000 pkl-python-0.1.13/src/pkl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:12:05.059921 pkl-python-0.1.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_evaluator_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 12:11:49.000000 pkl-python-0.1.13/tests/test_trace.py
```

### Comparing `pkl-python-0.1.12/LICENSE` & `pkl-python-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/PKG-INFO` & `pkl-python-0.1.13/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkl-python
-Version: 0.1.12
+Version: 0.1.13
 Summary: Python library for Apple's PKL.
 Author-email: Jungwoo Yang <jwyang0213@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jungwoo Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/jw-y/pkl
-Project-URL: Bug Reports, https://github.com/jw-y/pkl/issues
-Project-URL: Source, https://github.com/jw-y/pkl
+Project-URL: Homepage, https://github.com/jw-y/pkl-python
+Project-URL: Bug Reports, https://github.com/jw-y/pkl-python/issues
+Project-URL: Source, https://github.com/jw-y/pkl-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.8
@@ -64,29 +64,34 @@
 ### Basic Usage
 Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
-print(config)
+```
+
+### Code Generation
+As Python is a dynamic language, codegen is not strictly necessary.
+However, codegen lets you expect contents of pkl files within Python modules.
+
+```
+pkl-gen-python path/to/pkl/example_module.pkl
 ```
 
 ### Status
-* Evaluator API: fully functional
-* Code Generation: in development
+* Evaluator API: functional
+* Code Generation: functional, but needs refining
 
 ### TODO
-* [ ] (codgen) pip binary installation
-* [ ] (codgen) fix class order
+* [x] (codgen) pip binary installation
+* [ ] (codgen) gatherer depth-first ordering
 * [ ] (codgen) clean up code
 
 
-## Usage
-
 ## Advanced Features
 For details on the parameters, refer [Message Passing API](https://pkl-lang.org/main/current/bindings-specification/message-passing-api.html).
 
 ```python
 import pkl
 
 config = pkl.load("./tests/types.pkl")
```

### Comparing `pkl-python-0.1.12/README.md` & `pkl-python-0.1.13/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,29 +17,34 @@
 ### Basic Usage
 Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
-print(config)
+```
+
+### Code Generation
+As Python is a dynamic language, codegen is not strictly necessary.
+However, codegen lets you expect contents of pkl files within Python modules.
+
+```
+pkl-gen-python path/to/pkl/example_module.pkl
 ```
 
 ### Status
-* Evaluator API: fully functional
-* Code Generation: in development
+* Evaluator API: functional
+* Code Generation: functional, but needs refining
 
 ### TODO
-* [ ] (codgen) pip binary installation
-* [ ] (codgen) fix class order
+* [x] (codgen) pip binary installation
+* [ ] (codgen) gatherer depth-first ordering
 * [ ] (codgen) clean up code
 
 
-## Usage
-
 ## Advanced Features
 For details on the parameters, refer [Message Passing API](https://pkl-lang.org/main/current/bindings-specification/message-passing-api.html).
 
 ```python
 import pkl
 
 config = pkl.load("./tests/types.pkl")
```

### Comparing `pkl-python-0.1.12/pkl/__init__.py` & `pkl-python-0.1.13/src/pkl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,29 @@
             break
 
     if str(cur_path) == "/":
         cur_path = Path(module_path).parent
     return str(cur_path.absolute())
 
 
+def _parse_module_uri(module_uri, module_text):
+    parsed = urlparse(str(module_uri))
+
+    def is_uri(_uri: ParseResult):
+        return bool(_uri.scheme) and (bool(_uri.netloc) or bool(_uri.path))
+
+    if module_text:
+        source = ModuleSource.from_text(module_text)
+    elif is_uri(parsed):
+        source = ModuleSource.from_uri(module_uri)
+    else:
+        source = ModuleSource.from_path(module_uri)
+    return source
+
+
 def load(
     module_uri: Union[str, Path],
     *,
     module_text: Optional[str] = None,
     expr: Optional[str] = None,
     project_dir: str = PKL_DEFAULT,
     evaluator_options: EvaluatorOptions = PreconfiguredOptions(),
@@ -67,25 +82,15 @@
         The result of the module or expression evaluation, depending on the inputs and configuration.
 
     This function provides a flexible interface for loading and evaluating Pkl modules
     with a variety of customization options, including custom module and resource readers,
     environmental configurations, and support for complex project dependencies.
     """
 
-    parsed = urlparse(str(module_uri))
-
-    def is_uri(_uri: ParseResult):
-        return bool(_uri.scheme) and (bool(_uri.netloc) or bool(_uri.path))
-
-    if module_text:
-        source = ModuleSource.from_text(module_text)
-    elif is_uri(parsed):
-        source = ModuleSource.from_uri(module_uri)
-    else:
-        source = ModuleSource.from_path(module_uri)
+    source = _parse_module_uri(module_uri, module_text)
 
     if project_dir is PKL_DEFAULT:
         project_dir = _search_project_dir(str(module_uri))
 
     with EvaluatorManager(debug=debug) as manager:
         if (Path(project_dir) / "PklProject").exists():
             evaluator = manager.new_project_evaluator(
```

### Comparing `pkl-python-0.1.12/pkl/evaluator_manager.py` & `pkl-python-0.1.13/src/pkl/evaluator_manager.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/evaluator_options.py` & `pkl-python-0.1.13/src/pkl/evaluator_options.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/msgapi.py` & `pkl-python-0.1.13/src/pkl/msgapi.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/parser.py` & `pkl-python-0.1.13/src/pkl/parser.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/reader.py` & `pkl-python-0.1.13/src/pkl/reader.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/server.py` & `pkl-python-0.1.13/src/pkl/server.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl/utils.py` & `pkl-python-0.1.13/src/pkl/utils.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/pkl_python.egg-info/PKG-INFO` & `pkl-python-0.1.13/src/pkl_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkl-python
-Version: 0.1.12
+Version: 0.1.13
 Summary: Python library for Apple's PKL.
 Author-email: Jungwoo Yang <jwyang0213@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jungwoo Yang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/jw-y/pkl
-Project-URL: Bug Reports, https://github.com/jw-y/pkl/issues
-Project-URL: Source, https://github.com/jw-y/pkl
+Project-URL: Homepage, https://github.com/jw-y/pkl-python
+Project-URL: Bug Reports, https://github.com/jw-y/pkl-python/issues
+Project-URL: Source, https://github.com/jw-y/pkl-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: msgpack>=1.0.8
@@ -64,29 +64,34 @@
 ### Basic Usage
 Here's how you can start using `pkl-python` to load a PKL module:
 
 ```python
 import pkl
 
 config = pkl.load("path/to/pkl/example_module.pkl")
-print(config)
+```
+
+### Code Generation
+As Python is a dynamic language, codegen is not strictly necessary.
+However, codegen lets you expect contents of pkl files within Python modules.
+
+```
+pkl-gen-python path/to/pkl/example_module.pkl
 ```
 
 ### Status
-* Evaluator API: fully functional
-* Code Generation: in development
+* Evaluator API: functional
+* Code Generation: functional, but needs refining
 
 ### TODO
-* [ ] (codgen) pip binary installation
-* [ ] (codgen) fix class order
+* [x] (codgen) pip binary installation
+* [ ] (codgen) gatherer depth-first ordering
 * [ ] (codgen) clean up code
 
 
-## Usage
-
 ## Advanced Features
 For details on the parameters, refer [Message Passing API](https://pkl-lang.org/main/current/bindings-specification/message-passing-api.html).
 
 ```python
 import pkl
 
 config = pkl.load("./tests/types.pkl")
```

### Comparing `pkl-python-0.1.12/pyproject.toml` & `pkl-python-0.1.13/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -14,45 +14,53 @@
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "msgpack >= 1.0.8"
+    "msgpack >= 1.0.8",
 ]
 
 [tool.setuptools.packages.find]
-include = ["pkl"]
+where = ["src"]
 
 [tool.setuptools.dynamic]
-version = {file = "pkl/VERSION"}
+version = {file = "src/pkl/VERSION"}
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "black",
     "isort",
     "mypy",
     "pylint",
     "pytest",
     "pytest-cov",
     "tox",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/jw-y/pkl"
-"Bug Reports" = "https://github.com/jw-y/pkl/issues"
-"Source" = "https://github.com/jw-y/pkl"
+"Homepage" = "https://github.com/jw-y/pkl-python"
+"Bug Reports" = "https://github.com/jw-y/pkl-python/issues"
+"Source" = "https://github.com/jw-y/pkl-python"
+
+[project.scripts]
+pkl-gen-python = "pkl_gen_python:main"
 
 [tool.twine]
 repository = "pypi"
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
+force-exclude = 'codegen/snippet-tests/output/'
 
 [tool.isort]
 profile = "black"
+skip = ["codegen/snippet-tests/output/*"]
+
+[tool.autoflake]
+exclude = ["codegen/snippet-tests/output/*"]
 
 [tool.pytest.ini_options]
 addopts = "-ra -q"
```

### Comparing `pkl-python-0.1.12/setup.py` & `pkl-python-0.1.13/setup.py`

 * *Files identical despite different names*

### Comparing `pkl-python-0.1.12/tests/test_parser.py` & `pkl-python-0.1.13/tests/test_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,9 +50,9 @@
 
 def test_lib1():
     file = base_path / "lib1.pkl"
     _ = pkl.load(file)
 
 
 def test_types():
-    file = Path("./tests") / "types.pkl"
+    file = Path("./tests/pkls") / "types.pkl"
     _ = pkl.load(file)
```

### Comparing `pkl-python-0.1.12/tests/test_readers.py` & `pkl-python-0.1.13/tests/test_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         def list_elements(self, url: str) -> List[PathElement]:
             return [PathElement("foo.pkl", False)]
 
     opts = PreconfiguredOptions(
         moduleReaders=[TestModuleReader("customfs", True, True, True)]
     )
     opts.allowedModules.append("customfs:")
-    _ = pkl.load("./tests/myModule.pkl", evaluator_options=opts)
+    _ = pkl.load("./tests/pkls/myModule.pkl", evaluator_options=opts)
 
 
 def test_read_modules_error():
     class TestModuleReader(ModuleReader):
         def read(self, url) -> str:
             raise FileNotFoundError("foo.pkl not found")
 
@@ -36,15 +36,15 @@
             return [PathElement("foo.pkl", False)]
 
     opts = PreconfiguredOptions(
         moduleReaders=[TestModuleReader("customfs", True, True, True)]
     )
     opts.allowedModules.append("customfs:")
     with pytest.raises(PklError):
-        _ = pkl.load("./tests/myModule.pkl", evaluator_options=opts)
+        _ = pkl.load("./tests/pkls/myModule.pkl", evaluator_options=opts)
 
 
 def test_read_resources():
     class TestResourceReader(ResourceReader):
         def read(self, url) -> bytes:
             return b"Hello, World!"
 
@@ -56,8 +56,8 @@
             TestResourceReader(
                 scheme="customfs", hasHierarchicalUris=True, isGlobbable=True
             )
         ]
     )
     opts.allowedResources.append("customfs:")
 
-    _ = pkl.load("./tests/with_read.pkl", evaluator_options=opts)
+    _ = pkl.load("./tests/pkls/with_read.pkl", evaluator_options=opts)
```

