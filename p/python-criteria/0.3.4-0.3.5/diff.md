# Comparing `tmp/python-criteria-0.3.4.tar.gz` & `tmp/python-criteria-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.3.4.tar", last modified: Mon Apr  8 23:01:39 2024, max compression
+gzip compressed data, was "python-criteria-0.3.5.tar", last modified: Tue Apr  9 00:21:23 2024, max compression
```

## Comparing `python-criteria-0.3.4.tar` & `python-criteria-0.3.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.992851 python-criteria-0.3.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.992851 python-criteria-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 23:01:33.000000 python-criteria-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 23:01:38.996851 python-criteria-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 23:01:33.000000 python-criteria-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 23:01:33.000000 python-criteria-0.3.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:01:38.996851 python-criteria-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 00:21:18.000000 python-criteria-0.3.5/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 00:21:18.000000 python-criteria-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 00:21:23.011006 python-criteria-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-09 00:21:18.000000 python-criteria-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 00:21:18.000000 python-criteria-0.3.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-09 00:21:18.000000 python-criteria-0.3.5/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:23.011006 python-criteria-0.3.5/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 00:21:22.000000 python-criteria-0.3.5/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-09 00:21:23.000000 python-criteria-0.3.5/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:21:22.000000 python-criteria-0.3.5/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 00:21:22.000000 python-criteria-0.3.5/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:21:23.011006 python-criteria-0.3.5/setup.cfg
```

### Comparing `python-criteria-0.3.4/.devcontainer/devcontainer.json` & `python-criteria-0.3.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/.devcontainer/docker-compose.yml` & `python-criteria-0.3.5/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/.github/workflows/python-publish.yml` & `python-criteria-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/.gitignore` & `python-criteria-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/.pylintrc` & `python-criteria-0.3.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/.vscode/tasks.json` & `python-criteria-0.3.5/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/LICENSE` & `python-criteria-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/pyproject.toml` & `python-criteria-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/python_criteria/clauses.py` & `python-criteria-0.3.5/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/python_criteria/entity.py` & `python-criteria-0.3.5/python_criteria/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import ChainMap
 from typing import Any, dataclass_transform
 
 from .filter import FilterableAttribute, Value
 
 type AnnotatedObject = Any
 
 
@@ -48,15 +49,22 @@
             exclude = set()
 
         if include is None:
             include = set()
 
         result: dict[str, Any] = {}
 
-        for name, _ in _object.__annotations__.items():
+        annotations = ChainMap(
+            *(
+                c.__annotations__
+                for c in _object.__mro__
+                if "__annotations__" in c.__dict__
+            )
+        )
+        for name, _ in annotations.items():
             if name in exclude:
                 continue
 
             if include and name not in include:
                 continue
 
             value = getattr(_object, name)
```

### Comparing `python-criteria-0.3.4/python_criteria/filter.py` & `python-criteria-0.3.5/python_criteria/filter.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/python_criteria/sqlalchemy.py` & `python-criteria-0.3.5/python_criteria/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/python_criteria/visitor.py` & `python-criteria-0.3.5/python_criteria/visitor.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.4/python_criteria.egg-info/SOURCES.txt` & `python-criteria-0.3.5/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

