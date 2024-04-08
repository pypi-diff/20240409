# Comparing `tmp/dump_psql_roles_grants-0.2.0.tar.gz` & `tmp/dump_psql_roles_grants-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dump_psql_roles_grants-0.2.0.tar", max compression
+gzip compressed data, was "dump_psql_roles_grants-0.3.0.tar", max compression
```

## Comparing `dump_psql_roles_grants-0.2.0.tar` & `dump_psql_roles_grants-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      777 2024-04-08 17:27:08.740395 dump_psql_roles_grants-0.2.0/README.md
--rw-r--r--   0        0        0      290 2024-04-08 17:42:38.046059 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/__main__.py
--rw-r--r--   0        0        0      429 2024-04-08 18:06:17.285657 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/classes.py
--rw-r--r--   0        0        0     3236 2024-04-08 19:52:23.941260 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/cli.py
--rw-r--r--   0        0        0     3674 2024-04-08 17:42:38.046584 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/commands.py
--rw-r--r--   0        0        0      920 2024-04-08 19:52:23.941352 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/config.py
--rwxr-xr-x   0        0        0     7698 2024-04-08 19:54:29.340722 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/get_data.py
--rw-r--r--   0        0        0     5560 2024-04-08 19:54:44.133063 dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/table.py
--rw-r--r--   0        0        0      710 2024-04-08 19:56:27.627818 dump_psql_roles_grants-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 dump_psql_roles_grants-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/README.md
+-rw-r--r--   0        0        0      290 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/__main__.py
+-rw-r--r--   0        0        0      429 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/classes.py
+-rw-r--r--   0        0        0     3248 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/cli.py
+-rw-r--r--   0        0        0     3674 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/commands.py
+-rw-r--r--   0        0        0      920 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/config.py
+-rwxr-xr-x   0        0        0     7698 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/get_data.py
+-rw-r--r--   0        0        0     5560 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/table.py
+-rw-r--r--   0        0        0      856 2024-04-08 23:01:56.101219 dump_psql_roles_grants-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 dump_psql_roles_grants-0.3.0/PKG-INFO
```

### Comparing `dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/cli.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # from table import get_table_formats
 
 
 @click.group()
 # @click.option("-v", "--verbose", count=True)
 def cli():
-    """CLI group function"""
+    """Dump Postgres Roles and Grants"""
 
 
 @cli.command()
 @click.option(
     "--print/--no-print",
     "print_",
     is_flag=True,
```

### Comparing `dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/commands.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/commands.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/config.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/config.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/get_data.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/get_data.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.0/dump_psql_roles_grants/table.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/table.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.0/pyproject.toml` & `dump_psql_roles_grants-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [tool.poetry]
 name = "dump-psql-roles-grants"
-version = "0.2.0"
-description = "Dump Postgres Roles Grants"
+version = "0.3.0"
+description = "Dump Postgres Roles and Grants"
 authors = ["Roman Geraskin <roman.n.geraskin@gmail.com>"]
 readme = "README.md"
+license = "MIT"
+repository = "https://github.com/rgeraskin/dump_psql_roles_grants"
+keywords = ["postgres", "psql", "roles", "grants", "dump"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 icecream = "^2.1.3"
 pytablewriter = "^1.2.0"
 click = "^8.1.7"
 rich = "^13.7.1"
```

### Comparing `dump_psql_roles_grants-0.2.0/PKG-INFO` & `dump_psql_roles_grants-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,58 @@
 Metadata-Version: 2.1
 Name: dump-psql-roles-grants
-Version: 0.2.0
-Summary: Dump Postgres Roles Grants
+Version: 0.3.0
+Summary: Dump Postgres Roles and Grants
+Home-page: https://github.com/rgeraskin/dump_psql_roles_grants
+License: MIT
+Keywords: postgres,psql,roles,grants,dump
 Author: Roman Geraskin
 Author-email: roman.n.geraskin@gmail.com
 Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: icecream (>=2.1.3,<3.0.0)
 Requires-Dist: psycopg-binary (>=3.1.18,<4.0.0)
 Requires-Dist: psycopg-infdate (>=1.0.3,<2.0.0)
 Requires-Dist: pytablewriter (>=1.2.0,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
+Project-URL: Repository, https://github.com/rgeraskin/dump_psql_roles_grants
 Description-Content-Type: text/markdown
 
 # Dump Postgres Roles and Grants
 
-## Build
+## Install
+
+### pipx
+
+```shell
+pipx install dump-psql-roles-grants
+dump-psql-roles-grants --help
+```
+
+### pip
+
+```shell
+pip install dump-psql-roles-grants
+python -m dump_psql_roles_grants --help
+```
+
+### docker
 
 ```shell
-docker buildx build -t dump_psql_roles_grants .
+docker pull rgeraskin/dump_psql_roles_grants
+docker run --name dump_psql_roles_grants --rm rgeraskin/dump_psql_roles_grants --help
 ```
 
 ## Usage
 
+1. Generate an example config file `dump_psql_roles_grants gen-example-config -o config.yaml`
 1. Place instances connection info to `_inputs` dir
 
    ```shell
    _inputs/
    ├── dev.yaml
    ├── prod.yaml
    ├── stage.yaml
@@ -53,10 +76,10 @@
    ```
 
 1. Review `config.yaml`
 
 1. Run
 
    ```shell
-   docker run -it --rm -v ${PWD}/_inputs:/app/_inputs -v ${PWD}/_results:/app/_results dump_psql_roles_grants -- --help
+   dump_psql_roles_grants --help
    ```
```

