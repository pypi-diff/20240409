# Comparing `tmp/metricflow_to_zenlytic-0.1.4.tar.gz` & `tmp/metricflow_to_zenlytic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricflow_to_zenlytic-0.1.4.tar", max compression
+gzip compressed data, was "metricflow_to_zenlytic-0.1.5.tar", max compression
```

## Comparing `metricflow_to_zenlytic-0.1.4.tar` & `metricflow_to_zenlytic-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1079 2023-10-14 00:34:10.476175 metricflow_to_zenlytic-0.1.4/LICENSE
--rw-r--r--   0        0        0      869 2023-10-14 14:21:50.637879 metricflow_to_zenlytic-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-10-11 22:47:53.796432 metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/__init__.py
--rw-r--r--   0        0        0      854 2023-10-14 01:46:48.880082 metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/cli.py
--rw-r--r--   0        0        0    14600 2024-03-30 17:06:17.413830 metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/metricflow_to_zenlytic.py
--rw-r--r--   0        0        0      125 2023-10-12 22:01:42.278516 metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/metricflow_types.py
--rw-r--r--   0        0        0      889 2024-03-30 17:06:41.244278 metricflow_to_zenlytic-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 metricflow_to_zenlytic-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-10-14 00:34:10.476175 metricflow_to_zenlytic-0.1.5/LICENSE
+-rw-r--r--   0        0        0      869 2023-10-14 14:21:50.637879 metricflow_to_zenlytic-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-10-11 22:47:53.796432 metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/__init__.py
+-rw-r--r--   0        0        0      854 2023-10-14 01:46:48.880082 metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/cli.py
+-rw-r--r--   0        0        0    14762 2024-04-09 21:53:02.510999 metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/metricflow_to_zenlytic.py
+-rw-r--r--   0        0        0      125 2023-10-12 22:01:42.278516 metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/metricflow_types.py
+-rw-r--r--   0        0        0      889 2024-04-09 21:55:35.051960 metricflow_to_zenlytic-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 metricflow_to_zenlytic-0.1.5/PKG-INFO
```

### Comparing `metricflow_to_zenlytic-0.1.4/LICENSE` & `metricflow_to_zenlytic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metricflow_to_zenlytic-0.1.4/README.md` & `metricflow_to_zenlytic-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/cli.py` & `metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/cli.py`

 * *Files identical despite different names*

### Comparing `metricflow_to_zenlytic-0.1.4/metricflow_to_zenlytic/metricflow_to_zenlytic.py` & `metricflow_to_zenlytic-0.1.5/metricflow_to_zenlytic/metricflow_to_zenlytic.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     mf_metrics = mf_semantic_model.get("metrics", [])
 
     if original_file_path:
         zenlytic_data["original_file_path"] = original_file_path
 
     # Get view-level values
     zenlytic_data["name"] = mf_semantic_model["name"]
-    zenlytic_data["sql_table_name"] = extract_inner_text(mf_semantic_model["model"])
+    if "sql_table_name" in mf_semantic_model.get("meta", {}):
+        zenlytic_data["sql_table_name"] = mf_semantic_model["meta"]["sql_table_name"]
+    else:
+        zenlytic_data["sql_table_name"] = extract_inner_text(mf_semantic_model["model"])
     zenlytic_data["description"] = mf_semantic_model.get("description", None)
     default_date = mf_semantic_model.get("defaults", {}).get("agg_time_dimension")
 
     if default_date:
         zenlytic_data["default_date"] = default_date
 
     # dimensions to fields.dimensions
```

### Comparing `metricflow_to_zenlytic-0.1.4/pyproject.toml` & `metricflow_to_zenlytic-0.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metricflow-to-zenlytic"
-version = "0.1.4"
+version = "0.1.5"
 description = "Adapter for Metricflow to Zenlytic"
 authors = ["Paul Blankley <paul@zenlytic.com>"]
 keywords = ["Metrics Layer", "Business Intelligence", "Analytics"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Zenlytic/zenlytic-adapters"
 repository = "https://github.com/Zenlytic/zenlytic-adapters"
```

### Comparing `metricflow_to_zenlytic-0.1.4/PKG-INFO` & `metricflow_to_zenlytic-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metricflow-to-zenlytic
-Version: 0.1.4
+Version: 0.1.5
 Summary: Adapter for Metricflow to Zenlytic
 Home-page: https://github.com/Zenlytic/zenlytic-adapters
 License: MIT
 Keywords: Metrics Layer,Business Intelligence,Analytics
 Author: Paul Blankley
 Author-email: paul@zenlytic.com
 Requires-Python: >=3.8.1,<3.14
```

