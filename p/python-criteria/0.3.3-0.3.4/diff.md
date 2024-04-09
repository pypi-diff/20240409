# Comparing `tmp/python-criteria-0.3.3.tar.gz` & `tmp/python-criteria-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.3.3.tar", last modified: Mon Apr  8 00:48:05 2024, max compression
+gzip compressed data, was "python-criteria-0.3.4.tar", last modified: Mon Apr  8 23:01:39 2024, max compression
```

## Comparing `python-criteria-0.3.3.tar` & `python-criteria-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 00:47:58.000000 python-criteria-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 00:48:05.515868 python-criteria-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 00:47:58.000000 python-criteria-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 00:47:58.000000 python-criteria-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:48:05.515868 python-criteria-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.992851 python-criteria-0.3.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.992851 python-criteria-0.3.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-08 23:01:33.000000 python-criteria-0.3.4/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 23:01:33.000000 python-criteria-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 23:01:38.996851 python-criteria-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 23:01:33.000000 python-criteria-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 23:01:33.000000 python-criteria-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-08 23:01:33.000000 python-criteria-0.3.4/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:01:38.996851 python-criteria-0.3.4/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 23:01:38.000000 python-criteria-0.3.4/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:01:38.996851 python-criteria-0.3.4/setup.cfg
```

### Comparing `python-criteria-0.3.3/.devcontainer/devcontainer.json` & `python-criteria-0.3.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/.devcontainer/docker-compose.yml` & `python-criteria-0.3.4/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/.github/workflows/python-publish.yml` & `python-criteria-0.3.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/.gitignore` & `python-criteria-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/.pylintrc` & `python-criteria-0.3.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/.vscode/tasks.json` & `python-criteria-0.3.4/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/LICENSE` & `python-criteria-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/pyproject.toml` & `python-criteria-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/python_criteria/clauses.py` & `python-criteria-0.3.4/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/python_criteria/entity.py` & `python-criteria-0.3.4/python_criteria/entity.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/python_criteria/filter.py` & `python-criteria-0.3.4/python_criteria/filter.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/python_criteria/sqlalchemy.py` & `python-criteria-0.3.4/python_criteria/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.3/python_criteria/visitor.py` & `python-criteria-0.3.4/python_criteria/visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         _object: Any,
         _filter: Filter,
     ):
         if not isinstance(_filter, Filter):
             raise ValueError("_filter argument should be an instance of Filter.")
 
         clause = _filter.clause
+        if clause is None:
+            return None
+
         name = clause.__class__.__name__.lower()
         method = getattr(self, "visit_" + name)
 
         if isinstance(clause, BooleanClauseList):
             comparisons = []
             for item in clause.clause_list:
                 comparisons.append(self.visit(_object, Filter(item)))
```

### Comparing `python-criteria-0.3.3/python_criteria.egg-info/SOURCES.txt` & `python-criteria-0.3.4/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

