# Comparing `tmp/pylearningstandards-0.2.1.tar.gz` & `tmp/pylearningstandards-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylearningstandards-0.2.1.tar", max compression
+gzip compressed data, was "pylearningstandards-0.2.2.tar", max compression
```

## Comparing `pylearningstandards-0.2.1.tar` & `pylearningstandards-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1812 2024-02-16 21:19:55.487949 pylearningstandards-0.2.1/LICENSE
--rw-r--r--   0        0        0      920 2024-02-16 21:19:55.487949 pylearningstandards-0.2.1/LICENSE_HEADER
--rw-r--r--   0        0        0        0 2024-04-02 21:28:52.185732 pylearningstandards-0.2.1/README.md
--rw-r--r--   0        0        0     3569 2024-04-08 21:53:25.125732 pylearningstandards-0.2.1/py_learning_standards/__init__.py
--rw-r--r--   0        0        0      572 2024-04-08 21:53:25.125732 pylearningstandards-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 pylearningstandards-0.2.1/setup.py
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 pylearningstandards-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1812 2024-02-16 21:19:55.487949 pylearningstandards-0.2.2/LICENSE
+-rw-r--r--   0        0        0      920 2024-02-16 21:19:55.487949 pylearningstandards-0.2.2/LICENSE_HEADER
+-rw-r--r--   0        0        0        0 2024-04-02 21:28:52.185732 pylearningstandards-0.2.2/README.md
+-rw-r--r--   0        0        0     3690 2024-04-09 07:40:56.305732 pylearningstandards-0.2.2/py_learning_standards/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-09 07:41:17.925732 pylearningstandards-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 pylearningstandards-0.2.2/setup.py
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 pylearningstandards-0.2.2/PKG-INFO
```

### Comparing `pylearningstandards-0.2.1/LICENSE` & `pylearningstandards-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylearningstandards-0.2.1/LICENSE_HEADER` & `pylearningstandards-0.2.2/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `pylearningstandards-0.2.1/py_learning_standards/__init__.py` & `pylearningstandards-0.2.2/py_learning_standards/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     return {"en-us": raw_string}
 
 
 @dataclass
 class Competency(BaseJSONLDObject):
 
     ctid: Optional[str] = json_field(f"{NAMESPACE_CEASN}:ctid", all=True, default=None)
+    competency_label: Optional[Dict[str,str]] = json_field(f"{NAMESPACE_CEASN}:competencyLabel", all=True, default=None)
     competency_text: Optional[Dict[str, str]] = json_field(
         f"{NAMESPACE_CEASN}:competencyText", all=True, default=None
     )
     relevance: Optional[float] = json_field("relevance", all=True, default=None)
 
 
 @dataclass
```

### Comparing `pylearningstandards-0.2.1/pyproject.toml` & `pylearningstandards-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylearningstandards"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Daniel Auerbach <auerbach@ict.usc.edu>"]
 readme = "README.md"
 packages = [{include = "py_learning_standards"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.4"
```

### Comparing `pylearningstandards-0.2.1/setup.py` & `pylearningstandards-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dataclass-wizard>=0.22.3,<0.23.0', 'pyld>=2.0.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'pylearningstandards',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
     'long_description': '',
     'author': 'Daniel Auerbach',
     'author_email': 'auerbach@ict.usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

