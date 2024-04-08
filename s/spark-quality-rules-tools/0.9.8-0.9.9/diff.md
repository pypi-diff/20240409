# Comparing `tmp/spark_quality_rules_tools-0.9.8.tar.gz` & `tmp/spark_quality_rules_tools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.9.8.tar", last modified: Wed Sep  6 08:47:40 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.9.9.tar", last modified: Wed Sep  6 09:34:51 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.9.8.tar` & `spark_quality_rules_tools-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.731419 spark_quality_rules_tools-0.9.8/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.8/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-09-06 08:47:40.732419 spark_quality_rules_tools-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.9.8/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.9.8/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-09-06 08:47:40.738423 spark_quality_rules_tools-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1214 2023-09-06 08:47:19.000000 spark_quality_rules_tools-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.701164 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2792 2023-07-29 17:25:05.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.727418 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    56531 2023-09-06 08:47:19.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.729418 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.731419 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-09-06 08:47:40.726418 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-09-06 08:47:40.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-09-06 08:47:40.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-06 08:47:40.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-09-06 08:47:40.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-09-06 08:47:40.000000 spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.085944 spark_quality_rules_tools-0.9.9/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-09-06 09:34:51.085944 spark_quality_rules_tools-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.9.9/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.9.9/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-09-06 09:34:51.086944 spark_quality_rules_tools-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2023-09-06 09:34:35.000000 spark_quality_rules_tools-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.063938 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2792 2023-07-29 17:25:05.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.080942 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    56852 2023-09-06 09:32:29.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.082944 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.084943 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    26115 2023-07-29 02:06:11.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-09-06 09:34:51.079943 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-09-06 09:34:51.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-09-06 09:34:51.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-06 09:34:51.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-09-06 09:34:51.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-09-06 09:34:51.000000 spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.9.8/LICENSE` & `spark_quality_rules_tools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/PKG-INFO` & `spark_quality_rules_tools-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.9.8/README.md` & `spark_quality_rules_tools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/pyproject.toml` & `spark_quality_rules_tools-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/setup.py` & `spark_quality_rules_tools-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.9.8',
+    version='0.9.9',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -927,15 +927,16 @@
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
 
 
-def dq_validate_artifactory_with_rules(file_conf=None,
+def dq_validate_artifactory_with_rules(table_name=None,
+                                       file_conf=None,
                                        rules_id=None,
                                        uuaa=None):
     import sys
     import os
     from spark_quality_rules_tools import get_validate_rules
 
     is_windows = sys.platform.startswith('win')
@@ -950,20 +951,22 @@
     id_split = str(rules_id).split("_")
     rule_country = str(id_split[0])
     rule_type = str(id_split[1])
     rule_id = str(id_split[-2])
     rule_correlative = str(id_split[-1])
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_ruleid_generated.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
 
 
-def dq_validate_file_with_rules(file_conf=None,
+def dq_validate_file_with_rules(table_name=None,
+                                file_conf=None,
                                 rules_id=None,
                                 uuaa=None):
     import sys
     import os
     from spark_quality_rules_tools import get_validate_rules
 
     is_windows = sys.platform.startswith('win')
@@ -977,14 +980,15 @@
     id_split = str(rules_id).split("_")
     rule_country = str(id_split[0])
     rule_type = str(id_split[1])
     rule_id = str(id_split[-2])
     rule_correlative = str(id_split[-1])
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
+    dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{table_name}_ruleid_generated.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
 
 
 def dq_get_rules_list():
     import os
```

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.9.8
+Version: 0.9.9
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.9.8/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.9.9/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

