# Comparing `tmp/ABSQL-0.5.3.tar.gz` & `tmp/ABSQL-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSQL-0.5.3.tar", last modified: Sat Apr  6 14:26:34 2024, max compression
+gzip compressed data, was "ABSQL-0.6.0.tar", last modified: Mon Apr  8 23:05:50 2024, max compression
```

## Comparing `ABSQL-0.5.3.tar` & `ABSQL-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.228448 ABSQL-0.5.3/
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.227195 ABSQL-0.5.3/ABSQL.egg-info/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-06 14:26:34.000000 ABSQL-0.5.3/ABSQL.egg-info/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-06 14:26:34.000000 ABSQL-0.5.3/ABSQL.egg-info/SOURCES.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-06 14:26:34.000000 ABSQL-0.5.3/ABSQL.egg-info/dependency_links.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-06 14:26:34.000000 ABSQL-0.5.3/ABSQL.egg-info/requires.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-06 14:26:34.000000 ABSQL-0.5.3/ABSQL.egg-info/top_level.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.5.3/LICENSE
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-06 14:26:34.227793 ABSQL-0.5.3/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.5.3/README.md
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.219774 ABSQL-0.5.3/absql/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.5.3/absql/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.220572 ABSQL-0.5.3/absql/files/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 ABSQL-0.5.3/absql/files/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.5.3/absql/files/loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3213 2024-04-06 14:26:22.000000 ABSQL-0.5.3/absql/files/parsers.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.221675 ABSQL-0.5.3/absql/functions/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.5.3/absql/functions/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.5.3/absql/functions/db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.5.3/absql/functions/env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.5.3/absql/functions/time.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.221947 ABSQL-0.5.3/absql/render/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3068 2024-04-06 01:03:31.000000 ABSQL-0.5.3/absql/render/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.222240 ABSQL-0.5.3/absql/text/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.5.3/absql/text/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.222508 ABSQL-0.5.3/absql/utils/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.5.3/absql/utils/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-06 14:26:34.228560 ABSQL-0.5.3/setup.cfg
--rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-06 14:26:22.000000 ABSQL-0.5.3/setup.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 14:26:34.226753 ABSQL-0.5.3/tests/
--rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_copy.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_funcs_db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_funcs_env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_funcs_time.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      909 2024-01-03 15:37:15.000000 ABSQL-0.5.3/tests/test_parse_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.5.3/tests/test_partial_kwargs.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.5.3/tests/test_render.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.5.3/tests/test_render_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1269 2024-04-06 14:26:22.000000 ABSQL-0.5.3/tests/test_render_file_return_dict.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_render_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_set.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.5.3/tests/test_utils.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.149817 ABSQL-0.6.0/
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.148357 ABSQL-0.6.0/ABSQL.egg-info/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       74 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/requires.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-08 23:05:50.000000 ABSQL-0.6.0/ABSQL.egg-info/top_level.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.6.0/LICENSE
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9797 2024-04-08 23:05:50.149073 ABSQL-0.6.0/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.6.0/README.md
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.138519 ABSQL-0.6.0/absql/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.6.0/absql/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.139696 ABSQL-0.6.0/absql/files/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      790 2024-04-06 14:26:22.000000 ABSQL-0.6.0/absql/files/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.6.0/absql/files/loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3297 2024-04-08 22:30:40.000000 ABSQL-0.6.0/absql/files/parsers.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141226 ABSQL-0.6.0/absql/functions/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.6.0/absql/functions/db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/functions/time.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141503 ABSQL-0.6.0/absql/render/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3084 2024-04-08 13:55:50.000000 ABSQL-0.6.0/absql/render/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.141797 ABSQL-0.6.0/absql/text/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/text/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.142103 ABSQL-0.6.0/absql/utils/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.6.0/absql/utils/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-08 23:05:50.149938 ABSQL-0.6.0/setup.cfg
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      846 2024-04-08 22:22:37.000000 ABSQL-0.6.0/setup.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-08 23:05:50.147827 ABSQL-0.6.0/tests/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_copy.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_funcs_time.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      923 2024-04-08 22:22:07.000000 ABSQL-0.6.0/tests/test_parse_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.6.0/tests/test_partial_kwargs.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.6.0/tests/test_render.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.6.0/tests/test_render_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1393 2024-04-08 22:31:38.000000 ABSQL-0.6.0/tests/test_render_file_return_dict.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_render_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_set.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.6.0/tests/test_utils.py
```

### Comparing `ABSQL-0.5.3/ABSQL.egg-info/PKG-INFO` & `ABSQL-0.6.0/ABSQL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.3
+Version: 0.6.0
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.3/ABSQL.egg-info/SOURCES.txt` & `ABSQL-0.6.0/ABSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/LICENSE` & `ABSQL-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/PKG-INFO` & `ABSQL-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.3
+Version: 0.6.0
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.3/README.md` & `ABSQL-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/__init__.py` & `ABSQL-0.6.0/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/files/__init__.py` & `ABSQL-0.6.0/absql/files/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/files/loader.py` & `ABSQL-0.6.0/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/files/parsers.py` & `ABSQL-0.6.0/absql/files/parsers.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,35 +49,36 @@
 
 
 def parse_yml(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
     raw_content = frontmatter_load(file_path, loader=loader)
     file_content = raw_content["metadata"] or raw_content["content"]
+    file_content["absql_body"] = file_content.get("sql", "")
     return file_content
 
 
 def parse_sql(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
     raw_content = frontmatter_load(file_path, loader=loader)
     file_content = raw_content["metadata"]
-    file_content["sql"] = raw_content["content"]
+    file_content["absql_body"] = raw_content["content"]
     return file_content
 
 
 def parse_js(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
     raw_content = frontmatter_load(file_path, loader=loader)
     file_content = raw_content["metadata"]
-    file_content["js"] = raw_content["content"]
+    file_content["absql_body"] = raw_content["content"]
     return file_content
 
 
 def parse_py(file_path, loader=None):
     if loader is None:
         loader = generate_loader()
     raw_content = jupytext.read(file_path)["cells"]
     file_content = yaml.load(raw_content[0]["source"].replace("---", ""), Loader=loader)
-    file_content["py"] = raw_content[1]["source"]
+    file_content["absql_body"] = raw_content[1]["source"]
     return file_content
```

### Comparing `ABSQL-0.5.3/absql/functions/__init__.py` & `ABSQL-0.6.0/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/functions/db.py` & `ABSQL-0.6.0/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/functions/env.py` & `ABSQL-0.6.0/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/render/__init__.py` & `ABSQL-0.6.0/absql/render/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,28 +78,28 @@
     the vars in the file and any extras passed to extra_context.
     """
     if loader is None:
         loader = generate_loader(extra_constructors or [])
 
     file_contents = parse(file_path, loader=loader)
 
-    sql = file_contents.pop("sql", "")
+    text = file_contents.get("absql_body", "")
 
     if file_context_from:
         file_contents.update(file_contents.get(file_context_from, {}))
         file_contents.pop(file_context_from, {})
 
     rendered_context = render_context(extra_context, file_contents, partial_kwargs)
 
     rendered = render_text(
-        text=sql,
+        text=text,
         replace_only=replace_only,
         pretty_encode=pretty_encode,
         partial_kwargs=partial_kwargs,
         **rendered_context,
     )
 
     if return_dict:
-        rendered_context["sql"] = rendered
+        rendered_context["absql_body"] = rendered
         return rendered_context
 
     return rendered
```

### Comparing `ABSQL-0.5.3/absql/text/__init__.py` & `ABSQL-0.6.0/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/absql/utils/__init__.py` & `ABSQL-0.6.0/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/setup.py` & `ABSQL-0.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.5.3",
+    version="0.6.0",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pipeline-tools/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `ABSQL-0.5.3/tests/test_copy.py` & `ABSQL-0.6.0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_funcs_db.py` & `ABSQL-0.6.0/tests/test_funcs_db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_funcs_env.py` & `ABSQL-0.6.0/tests/test_funcs_env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_funcs_time.py` & `ABSQL-0.6.0/tests/test_funcs_time.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_loader.py` & `ABSQL-0.6.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_parse_file.py` & `ABSQL-0.6.0/tests/test_parse_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 @pytest.fixture
 def simple_sql_path():
     return "tests/files/simple.sql"
 
 
 def test_simple_sql(simple_sql_path):
     res = parse(simple_sql_path)
-    assert "sql" in res.keys()
+    assert "absql_body" in res.keys()
     assert "my_table_placeholder" in res.keys()
     assert res["my_table_placeholder"] == "my_table"
-    assert res["sql"] == "SELECT * FROM {{my_table_placeholder}}"
+    assert res["absql_body"] == "SELECT * FROM {{my_table_placeholder}}"
 
 
 @pytest.mark.parametrize(
     argnames="yml_path",
     argvalues=[
         pytest.param("tests/files/simple.yml", id="simple_yml"),
         pytest.param(
```

### Comparing `ABSQL-0.5.3/tests/test_partial_kwargs.py` & `ABSQL-0.6.0/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_render.py` & `ABSQL-0.6.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_render_file.py` & `ABSQL-0.6.0/tests/test_render_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_render_file_return_dict.py` & `ABSQL-0.6.0/tests/test_render_file_return_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,28 +18,29 @@
 
 
 def test_render_file_return_dict(simple_yml_path):
     file_as_dict = r.render_file(simple_yml_path, return_dict=True)
     print(file_as_dict)
     assert file_as_dict["my_table_placeholder"] == "my_table"
     assert file_as_dict["sql"] == "SELECT * FROM my_table"
+    assert file_as_dict["absql_body"] == "SELECT * FROM my_table"
 
 
 def test_runner_return_dict(simple_yml_path):
     runner = r()
     file_as_dict = runner.render(simple_yml_path, return_dict=True)
     assert file_as_dict["my_table_placeholder"] == "my_table"
     assert file_as_dict["sql"] == "SELECT * FROM my_table"
+    assert file_as_dict["absql_body"] == "SELECT * FROM my_table"
 
 
 def test_render_file_return_dict_js(simple_js_path):
     file_as_dict = r.render_file(simple_js_path, return_dict=True)
-    print(file_as_dict)
     assert file_as_dict["foo"] == "bar"
-    assert file_as_dict["js"] == "console.log('hello')"
+    assert file_as_dict["absql_body"] == "console.log('hello')"
 
 
 def test_render_file_return_dict_py(simple_py_path):
     file_as_dict = r.render_file(simple_py_path, return_dict=True)
     print(file_as_dict)
     assert file_as_dict["foo"] == "bar"
-    assert file_as_dict["py"] == 'print("hello")'
+    assert file_as_dict["absql_body"] == 'print("hello")'
```

### Comparing `ABSQL-0.5.3/tests/test_render_text.py` & `ABSQL-0.6.0/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_text.py` & `ABSQL-0.6.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.3/tests/test_utils.py` & `ABSQL-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

