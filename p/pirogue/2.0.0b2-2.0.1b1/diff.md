# Comparing `tmp/pirogue-2.0.0b2.tar.gz` & `tmp/pirogue-2.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pirogue-2.0.0b2.tar", last modified: Tue Apr  9 06:10:14 2024, max compression
+gzip compressed data, was "pirogue-2.0.1b1.tar", last modified: Tue Apr  9 05:51:43 2024, max compression
```

## Comparing `pirogue-2.0.0b2.tar` & `pirogue-2.0.1b1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.494770 pirogue-2.0.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.486770 pirogue-2.0.0b2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.490770 pirogue-2.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 06:10:14.494770 pirogue-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.490770 pirogue-2.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.490770 pirogue-2.0.0b2/pirogue/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4482 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/information_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    24522 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/simple_joins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/single_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pirogue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.494770 pirogue-2.0.0b2/pirogue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 06:10:14.000000 pirogue-2.0.0b2/pirogue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:10:14.494770 pirogue-2.0.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:10:14.494770 pirogue-2.0.0b2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/demo_data.sql
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/multiple_inheritance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/simple_joins.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/simple_joins_based_on_view.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/test_multiple_inheritance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/test_simple_inheritance.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 06:09:53.000000 pirogue-2.0.0b2/test/test_simple_joins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.531676 pirogue-2.0.1b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.523676 pirogue-2.0.1b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.523676 pirogue-2.0.1b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 05:51:43.531676 pirogue-2.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.523676 pirogue-2.0.1b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.527675 pirogue-2.0.1b1/pirogue/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4482 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/information_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24940 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/simple_joins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/single_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pirogue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.527675 pirogue-2.0.1b1/pirogue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 05:51:43.000000 pirogue-2.0.1b1/pirogue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:51:43.531676 pirogue-2.0.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:43.527675 pirogue-2.0.1b1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/demo_data.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/multiple_inheritance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/simple_joins.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/simple_joins_based_on_view.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/test_multiple_inheritance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/test_simple_inheritance.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-09 05:51:30.000000 pirogue-2.0.1b1/test/test_simple_joins.py
```

### Comparing `pirogue-2.0.0b2/.github/workflows/docs.yml` & `pirogue-2.0.1b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/.github/workflows/release.yml` & `pirogue-2.0.1b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/.github/workflows/test.yml` & `pirogue-2.0.1b1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/.github/workflows/wheel.yml` & `pirogue-2.0.1b1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/.pre-commit-config.yaml` & `pirogue-2.0.1b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/LICENSE` & `pirogue-2.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/PKG-INFO` & `pirogue-2.0.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pirogue
-Version: 2.0.0b2
+Version: 2.0.1b1
 Summary: pirogue let you dynamically and easily create views in PostgreSQL for inheritance or join scenarios.
 Author-email: Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pirogue/
 Project-URL: repository, https://github.com/opengisch/pirogue
 Project-URL: tracker, https://github.com/opengisch/pirogue/issues
 Keywords: postgres
```

### Comparing `pirogue-2.0.0b2/docs/Makefile` & `pirogue-2.0.1b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/docs/conf.py` & `pirogue-2.0.1b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/docs/index.rst` & `pirogue-2.0.1b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue/cli.py` & `pirogue-2.0.1b1/pirogue/cli.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue/information_schema.py` & `pirogue-2.0.1b1/pirogue/information_schema.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue/multiple_inheritance.py` & `pirogue-2.0.1b1/pirogue/multiple_inheritance.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,16 +446,19 @@
                     )
                     for alias, table_def in sorted_joins
                 ]
             ),
             raise_notice=(
                 "NULL;"
                 if self.allow_parent_only
-                else "RAISE NOTICE '{vn} type not known (%)', NEW.{type_name}; -- ERROR".format(
+                else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR".format(
                     vn=self.view_name,
+                    percent_char=(
+                        "%%" if self.variables else "%"
+                    ),  # if variables, % should be escaped because cursor.execute is run with variables
                     type_name=self.type_name,
                 )
             ),
             insert_trigger_post=self.insert_trigger.get("post", ""),
         )
         return sql
 
@@ -579,16 +582,19 @@
                     )
                     for alias, table_def in sorted_joins
                 ]
             ),
             raise_notice=(
                 "NULL;"
                 if self.allow_parent_only
-                else "RAISE NOTICE '{vn} type not known (%)', NEW.{type_name}; -- ERROR".format(
+                else "RAISE NOTICE '{vn} type not known ({percent_char})', NEW.{type_name}; -- ERROR".format(
                     vn=self.view_name,
+                    percent_char=(
+                        "%%" if self.variables else "%"
+                    ),  # if variables, % should be escaped because cursor.execute is run with variables
                     type_name=self.type_name,
                 )
             ),
             update_trigger_post=self.update_trigger.get("post", ""),
         )
         return sql
```

### Comparing `pirogue-2.0.0b2/pirogue/simple_joins.py` & `pirogue-2.0.1b1/pirogue/simple_joins.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue/single_inheritance.py` & `pirogue-2.0.1b1/pirogue/single_inheritance.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue/utils.py` & `pirogue-2.0.1b1/pirogue/utils.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pirogue.egg-info/PKG-INFO` & `pirogue-2.0.1b1/pirogue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pirogue
-Version: 2.0.0b2
+Version: 2.0.1b1
 Summary: pirogue let you dynamically and easily create views in PostgreSQL for inheritance or join scenarios.
 Author-email: Denis Rouzaud <info@opengis.ch>
 License: MIT License
 Project-URL: homepage, https://opengisch.github.io/pirogue/
 Project-URL: repository, https://github.com/opengisch/pirogue
 Project-URL: tracker, https://github.com/opengisch/pirogue/issues
 Keywords: postgres
```

### Comparing `pirogue-2.0.0b2/pirogue.egg-info/SOURCES.txt` & `pirogue-2.0.1b1/pirogue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/pyproject.toml` & `pirogue-2.0.1b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/test/demo_data.sql` & `pirogue-2.0.1b1/test/demo_data.sql`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/test/test_multiple_inheritance.py` & `pirogue-2.0.1b1/test/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/test/test_simple_inheritance.sh` & `pirogue-2.0.1b1/test/test_simple_inheritance.sh`

 * *Files identical despite different names*

### Comparing `pirogue-2.0.0b2/test/test_simple_joins.py` & `pirogue-2.0.1b1/test/test_simple_joins.py`

 * *Files identical despite different names*

