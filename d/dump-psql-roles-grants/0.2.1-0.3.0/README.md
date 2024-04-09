# Comparing `tmp/dump_psql_roles_grants-0.2.1.tar.gz` & `tmp/dump_psql_roles_grants-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dump_psql_roles_grants-0.2.1.tar", max compression
+gzip compressed data, was "dump_psql_roles_grants-0.3.0.tar", max compression
```

## Comparing `dump_psql_roles_grants-0.2.1.tar` & `dump_psql_roles_grants-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/README.md
--rw-r--r--   0        0        0      290 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/__main__.py
--rw-r--r--   0        0        0      429 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/classes.py
--rw-r--r--   0        0        0     3248 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/cli.py
--rw-r--r--   0        0        0     3674 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/commands.py
--rw-r--r--   0        0        0      920 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/config.py
--rwxr-xr-x   0        0        0     7698 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/get_data.py
--rw-r--r--   0        0        0     5560 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/table.py
--rw-r--r--   0        0        0      855 2024-04-09 10:44:06.897403 dump_psql_roles_grants-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 dump_psql_roles_grants-0.2.1/PKG-INFO
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

### Comparing `dump_psql_roles_grants-0.2.1/README.md` & `dump_psql_roles_grants-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/cli.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/cli.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/commands.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/commands.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/config.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/config.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/get_data.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/get_data.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/dump_psql_roles_grants/table.py` & `dump_psql_roles_grants-0.3.0/dump_psql_roles_grants/table.py`

 * *Files identical despite different names*

### Comparing `dump_psql_roles_grants-0.2.1/pyproject.toml` & `dump_psql_roles_grants-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dump-psql-roles-grants"
-version = "0.2.1"
+version = "0.3.0"
 description = "Dump Postgres Roles and Grants"
 authors = ["Roman Geraskin <roman.n.geraskin@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/rgeraskin/dump_psql_roles_grants"
 keywords = ["postgres", "psql", "roles", "grants", "dump"]
 
@@ -17,14 +17,15 @@
 psycopg-binary = "^3.1.18"
 psycopg-infdate = "^1.0.3"
 PyYAML = "^6.0.1"
 
 [tool.poetry.scripts]
 dump_psql_roles_grants = "dump_psql_roles_grants.cli:cli"
 
+
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 [build-system]
```

### Comparing `dump_psql_roles_grants-0.2.1/PKG-INFO` & `dump_psql_roles_grants-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dump-psql-roles-grants
-Version: 0.2.1
+Version: 0.3.0
 Summary: Dump Postgres Roles and Grants
 Home-page: https://github.com/rgeraskin/dump_psql_roles_grants
 License: MIT
 Keywords: postgres,psql,roles,grants,dump
 Author: Roman Geraskin
 Author-email: roman.n.geraskin@gmail.com
 Requires-Python: >=3.12,<4.0
```

