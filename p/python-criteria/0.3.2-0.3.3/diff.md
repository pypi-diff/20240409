# Comparing `tmp/python-criteria-0.3.2.tar.gz` & `tmp/python-criteria-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-criteria-0.3.2.tar", last modified: Sun Apr  7 21:38:01 2024, max compression
+gzip compressed data, was "python-criteria-0.3.3.tar", last modified: Mon Apr  8 00:48:05 2024, max compression
```

## Comparing `python-criteria-0.3.2.tar` & `python-criteria-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.devcontainer/postCreateCommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.husky/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.husky/pre-commit
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-07 21:37:57.000000 python-criteria-0.3.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 21:37:57.000000 python-criteria-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 21:38:01.139004 python-criteria-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 21:37:57.000000 python-criteria-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-07 21:37:57.000000 python-criteria-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/python_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-07 21:37:57.000000 python-criteria-0.3.2/python_criteria/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:38:01.139004 python-criteria-0.3.2/python_criteria.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 21:38:01.000000 python-criteria-0.3.2/python_criteria.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:38:01.139004 python-criteria-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.devcontainer/postCreateCommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.511868 python-criteria-0.3.3/.husky/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.husky/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-08 00:47:58.000000 python-criteria-0.3.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 00:47:58.000000 python-criteria-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 00:48:05.515868 python-criteria-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-08 00:47:58.000000 python-criteria-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-08 00:47:58.000000 python-criteria-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/python_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-08 00:47:58.000000 python-criteria-0.3.3/python_criteria/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:48:05.515868 python-criteria-0.3.3/python_criteria.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 00:48:05.000000 python-criteria-0.3.3/python_criteria.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:48:05.515868 python-criteria-0.3.3/setup.cfg
```

### Comparing `python-criteria-0.3.2/.devcontainer/devcontainer.json` & `python-criteria-0.3.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/.devcontainer/docker-compose.yml` & `python-criteria-0.3.3/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/.github/workflows/python-publish.yml` & `python-criteria-0.3.3/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jobs:
     pypi-publish:
       name: Upload release to PyPI
       runs-on: ubuntu-latest
   
       environment:
         name: pypi
-        url: https://pypi.org/p/heptagon
+        url: https://pypi.org/p/python-criteria
   
       permissions:
         id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
   
       steps:
       # retrieve your distributions here
       - uses: actions/checkout@v4.1.1
```

### Comparing `python-criteria-0.3.2/.gitignore` & `python-criteria-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/.pylintrc` & `python-criteria-0.3.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/.vscode/tasks.json` & `python-criteria-0.3.3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/LICENSE` & `python-criteria-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/pyproject.toml` & `python-criteria-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/python_criteria/clauses.py` & `python-criteria-0.3.3/python_criteria/clauses.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/python_criteria/entity.py` & `python-criteria-0.3.3/python_criteria/entity.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/python_criteria/filter.py` & `python-criteria-0.3.3/python_criteria/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,8 +105,10 @@
     def like(self, other):
         return Like(self, other)
 
     def not_like(self, other):
         return NotLike(self, other)
 
 
-type Attribute[T] = FilterableAttribute[T]  # pylint: disable=unsubscriptable-object
+type Attribute[T] = FilterableAttribute[
+    T
+] | Any  # pylint: disable=unsubscriptable-object
```

### Comparing `python-criteria-0.3.2/python_criteria/sqlalchemy.py` & `python-criteria-0.3.3/python_criteria/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/python_criteria/visitor.py` & `python-criteria-0.3.3/python_criteria/visitor.py`

 * *Files identical despite different names*

### Comparing `python-criteria-0.3.2/python_criteria.egg-info/SOURCES.txt` & `python-criteria-0.3.3/python_criteria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

