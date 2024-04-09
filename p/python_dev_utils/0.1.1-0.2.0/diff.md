# Comparing `tmp/python_dev_utils-0.1.1.tar.gz` & `tmp/python_dev_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-0.1.1.tar", last modified: Thu Apr  4 10:38:52 2024, max compression
+gzip compressed data, was "python_dev_utils-0.2.0.tar", last modified: Tue Apr  9 13:32:55 2024, max compression
```

## Comparing `python_dev_utils-0.1.1.tar` & `python_dev_utils-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-0.1.1/LICENCE
--rw-r--r--   0        0        0     2038 2024-04-04 09:26:57.087717 python_dev_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-0.1.1/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-0.1.1/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-04 10:15:44.718260 python_dev_utils-0.1.1/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-0.1.1/dev_utils/core/exc.py
--rw-r--r--   0        0        0      229 2024-03-26 14:07:13.958342 python_dev_utils-0.1.1/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-01 13:22:15.897317 python_dev_utils-0.1.1/dev_utils/core/logging.py
--rw-r--r--   0        0        0      776 2024-03-28 08:22:11.212881 python_dev_utils-0.1.1/dev_utils/core/utils.py
--rw-r--r--   0        0        0      210 2024-03-28 10:44:02.392930 python_dev_utils-0.1.1/dev_utils/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-03-29 13:52:13.342131 python_dev_utils-0.1.1/dev_utils/profiling/containers.py
--rw-r--r--   0        0        0     2850 2024-04-04 09:56:53.374155 python_dev_utils-0.1.1/dev_utils/profiling/middlewares.py
--rw-r--r--   0        0        0     9754 2024-04-04 10:02:43.937276 python_dev_utils-0.1.1/dev_utils/profiling/profilers.py
--rw-r--r--   0        0        0      936 2024-04-04 09:55:26.621868 python_dev_utils-0.1.1/dev_utils/profiling/utils.py
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-0.1.1/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16331 2024-04-04 08:59:51.727121 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1562 2024-03-26 14:07:50.698059 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-03-29 14:18:20.445990 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-03-25 07:02:41.449042 python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0    12623 2024-03-26 08:35:25.401470 python_dev_utils-0.1.1/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     2962 2024-04-04 10:38:52.009451 python_dev_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     9104 2024-04-01 13:25:07.596658 python_dev_utils-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-0.1.1/tests/core/__init__.py
--rw-r--r--   0        0        0     1589 2024-04-04 10:35:52.893988 python_dev_utils-0.1.1/tests/core/test_abstract.py
--rw-r--r--   0        0        0      508 2024-03-26 14:08:33.510730 python_dev_utils-0.1.1/tests/core/test_guards.py
--rw-r--r--   0        0        0      933 2024-03-29 06:21:02.987051 python_dev_utils-0.1.1/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-0.1.1/tests/profiling/__init__.py
--rw-r--r--   0        0        0      349 2024-03-29 13:58:08.366680 python_dev_utils-0.1.1/tests/profiling/test_middlewares.py
--rw-r--r--   0        0        0     3027 2024-04-04 10:01:48.346733 python_dev_utils-0.1.1/tests/profiling/test_profilers.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-0.1.1/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    17186 2024-03-29 13:24:07.386873 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-03-26 14:08:03.098964 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-03-25 06:40:32.137462 python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0     7366 2024-03-25 06:19:19.846082 python_dev_utils-0.1.1/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      820 2024-03-29 06:17:35.440257 python_dev_utils-0.1.1/tests/types.py
--rw-r--r--   0        0        0     7174 2024-03-29 06:15:40.110095 python_dev_utils-0.1.1/tests/utils.py
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 python_dev_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-0.2.0/LICENCE
+-rw-r--r--   0        0        0     1962 2024-04-05 12:10:37.518458 python_dev_utils-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-0.2.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-0.2.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-04 10:15:44.718260 python_dev_utils-0.2.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-0.2.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      229 2024-03-26 14:07:13.958342 python_dev_utils-0.2.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-01 13:22:15.897317 python_dev_utils-0.2.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-0.2.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      776 2024-03-28 08:22:11.212881 python_dev_utils-0.2.0/dev_utils/core/utils.py
+-rw-r--r--   0        0        0      210 2024-03-28 10:44:02.392930 python_dev_utils-0.2.0/dev_utils/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-03-29 13:52:13.342131 python_dev_utils-0.2.0/dev_utils/profiling/containers.py
+-rw-r--r--   0        0        0     2850 2024-04-04 09:56:53.374155 python_dev_utils-0.2.0/dev_utils/profiling/middlewares.py
+-rw-r--r--   0        0        0     9754 2024-04-04 10:02:43.937276 python_dev_utils-0.2.0/dev_utils/profiling/profilers.py
+-rw-r--r--   0        0        0      940 2024-04-05 07:27:22.705464 python_dev_utils-0.2.0/dev_utils/profiling/utils.py
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-0.2.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16331 2024-04-04 08:59:51.727121 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1562 2024-03-26 14:07:50.698059 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-03-29 14:18:20.445990 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-03-25 07:02:41.449042 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0    12623 2024-03-26 08:35:25.401470 python_dev_utils-0.2.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     2962 2024-04-09 13:32:55.342253 python_dev_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     9104 2024-04-01 13:25:07.596658 python_dev_utils-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-0.2.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     1589 2024-04-04 10:35:52.893988 python_dev_utils-0.2.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      508 2024-03-26 14:08:33.510730 python_dev_utils-0.2.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-09 13:22:59.336479 python_dev_utils-0.2.0/tests/core/test_results.py
+-rw-r--r--   0        0        0      933 2024-03-29 06:21:02.987051 python_dev_utils-0.2.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-0.2.0/tests/profiling/__init__.py
+-rw-r--r--   0        0        0      349 2024-03-29 13:58:08.366680 python_dev_utils-0.2.0/tests/profiling/test_middlewares.py
+-rw-r--r--   0        0        0     3027 2024-04-04 10:01:48.346733 python_dev_utils-0.2.0/tests/profiling/test_profilers.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-0.2.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    17186 2024-03-29 13:24:07.386873 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-03-26 14:08:03.098964 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-03-25 06:40:32.137462 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0     7366 2024-03-25 06:19:19.846082 python_dev_utils-0.2.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      820 2024-03-29 06:17:35.440257 python_dev_utils-0.2.0/tests/types.py
+-rw-r--r--   0        0        0     7174 2024-03-29 06:15:40.110095 python_dev_utils-0.2.0/tests/utils.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 python_dev_utils-0.2.0/PKG-INFO
```

### Comparing `python_dev_utils-0.1.1/LICENCE` & `python_dev_utils-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/README.md` & `python_dev_utils-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Dev utils
 
-> Templated repository pattern implementation for your declarative models.
-
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
 working with sqlalchemy, FastAPI and other libs.
 
 ## Profiling
```

### Comparing `python_dev_utils-0.1.1/dev_utils/core/abstract.py` & `python_dev_utils-0.2.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/core/exc.py` & `python_dev_utils-0.2.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/core/logging.py` & `python_dev_utils-0.2.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/core/utils.py` & `python_dev_utils-0.2.0/dev_utils/core/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/profiling/containers.py` & `python_dev_utils-0.2.0/dev_utils/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/profiling/middlewares.py` & `python_dev_utils-0.2.0/dev_utils/profiling/middlewares.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/profiling/profilers.py` & `python_dev_utils-0.2.0/dev_utils/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/profiling/utils.py` & `python_dev_utils-0.2.0/dev_utils/profiling/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
     Make string from information to log it.
     """
     query_template = (
         'index: {query_index}\n'
         'query text: {query_text}\n'
         'query params: {query_params}\n'
-        'query duration: {query_duration}'
-        'query rowcount (may be incorrect): {query_rowcount}'
+        'query duration: {query_duration}\n'
+        'query rowcount (may be incorrect): {query_rowcount}\n'
     )
     if not isinstance(info, Sequence):
         info = [info]
     return '\n'.join(
         query_template.format(
             query_index=idx,
             query_text=query.text,
```

### Comparing `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-0.2.0/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/pyproject.toml` & `python_dev_utils-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "0.1.1"
+version = "0.2.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-0.1.1/tests/conftest.py` & `python_dev_utils-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/core/test_abstract.py` & `python_dev_utils-0.2.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/core/test_utils.py` & `python_dev_utils-0.2.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/profiling/test_profilers.py` & `python_dev_utils-0.2.0/tests/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/sqlalchemy/test_utils.py` & `python_dev_utils-0.2.0/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/types.py` & `python_dev_utils-0.2.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/tests/utils.py` & `python_dev_utils-0.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.1.1/PKG-INFO` & `python_dev_utils-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 0.1.1
+Version: 0.2.0
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy_filters
 Requires-Dist: fastapi>=0.110.0; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "sqlalchemy-filters"
 Description-Content-Type: text/markdown
 
 # Dev utils
 
-> Templated repository pattern implementation for your declarative models.
-
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
 working with sqlalchemy, FastAPI and other libs.
 
 ## Profiling
```

