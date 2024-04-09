# Comparing `tmp/dpkits-1.0.tar.gz` & `tmp/dpkits-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpkits-1.0.tar", last modified: Fri Mar 29 07:31:03 2024, max compression
+gzip compressed data, was "dpkits-1.1.tar", last modified: Tue Apr  9 06:18:32 2024, max compression
```

## Comparing `dpkits-1.0.tar` & `dpkits-1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 07:31:03.917850 dpkits-1.0/
--rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.0/LICENSE
--rw-rw-rw-   0        0        0    12194 2024-03-29 07:31:03.916845 dpkits-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.0/README.md
--rw-rw-rw-   0        0        0      624 2024-03-29 07:29:47.000000 dpkits-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 07:31:03.918846 dpkits-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 07:31:03.860009 dpkits-1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 07:31:03.884031 dpkits-1.0/src/dpkits/
--rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.0/src/dpkits/__init__.py
--rw-rw-rw-   0        0        0    28970 2024-03-29 03:25:00.000000 dpkits-1.0/src/dpkits/ap_data_converter.py
--rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.0/src/dpkits/calculate_lsm.py
--rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.0/src/dpkits/codeframe_reader.py
--rw-rw-rw-   0        0        0     5104 2024-01-09 08:11:30.000000 dpkits-1.0/src/dpkits/data_analysis.py
--rw-rw-rw-   0        0        0     2719 2024-03-01 03:33:56.000000 dpkits-1.0/src/dpkits/data_processing.py
--rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.0/src/dpkits/data_transpose.py
--rw-rw-rw-   0        0        0    25579 2023-12-01 07:03:09.000000 dpkits-1.0/src/dpkits/table_formater.py
--rw-rw-rw-   0        0        0    66033 2024-02-16 09:11:09.000000 dpkits-1.0/src/dpkits/table_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-29 07:31:03.914399 dpkits-1.0/src/dpkits.egg-info/
--rw-rw-rw-   0        0        0    12194 2024-03-29 07:31:03.000000 dpkits-1.0/src/dpkits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-03-29 07:31:03.000000 dpkits-1.0/src/dpkits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 07:31:03.000000 dpkits-1.0/src/dpkits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 07:31:03.000000 dpkits-1.0/src/dpkits.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-09 06:18:32.645693 dpkits-1.1/
+-rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.1/LICENSE
+-rw-rw-rw-   0        0        0    12194 2024-04-09 06:18:32.643589 dpkits-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.1/README.md
+-rw-rw-rw-   0        0        0      624 2024-04-09 06:17:14.000000 dpkits-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-09 06:18:32.645693 dpkits-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-09 06:18:32.576515 dpkits-1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-09 06:18:32.610625 dpkits-1.1/src/dpkits/
+-rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.1/src/dpkits/__init__.py
+-rw-rw-rw-   0        0        0    28970 2024-03-29 03:25:00.000000 dpkits-1.1/src/dpkits/ap_data_converter.py
+-rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.1/src/dpkits/calculate_lsm.py
+-rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.1/src/dpkits/codeframe_reader.py
+-rw-rw-rw-   0        0        0     5104 2024-01-09 08:11:30.000000 dpkits-1.1/src/dpkits/data_analysis.py
+-rw-rw-rw-   0        0        0     2792 2024-04-09 06:15:56.000000 dpkits-1.1/src/dpkits/data_processing.py
+-rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.1/src/dpkits/data_transpose.py
+-rw-rw-rw-   0        0        0    25579 2023-12-01 07:03:09.000000 dpkits-1.1/src/dpkits/table_formater.py
+-rw-rw-rw-   0        0        0    66033 2024-02-16 09:11:09.000000 dpkits-1.1/src/dpkits/table_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-09 06:18:32.642056 dpkits-1.1/src/dpkits.egg-info/
+-rw-rw-rw-   0        0        0    12194 2024-04-09 06:18:32.000000 dpkits-1.1/src/dpkits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-04-09 06:18:32.000000 dpkits-1.1/src/dpkits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-09 06:18:32.000000 dpkits-1.1/src/dpkits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-09 06:18:32.000000 dpkits-1.1/src/dpkits.egg-info/top_level.txt
```

### Comparing `dpkits-1.0/LICENSE` & `dpkits-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/PKG-INFO` & `dpkits-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.0
+Version: 1.1
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpkits-1.0/README.md` & `dpkits-1.1/README.md`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/pyproject.toml` & `dpkits-1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpkits"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="Hung Dao", email="hung.daotuan.1991@gmail.com" },
 ]
 description = "A small package for data processing"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dpkits-1.0/src/dpkits/__init__.py` & `dpkits-1.1/src/dpkits/__init__.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/ap_data_converter.py` & `dpkits-1.1/src/dpkits/ap_data_converter.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/calculate_lsm.py` & `dpkits-1.1/src/dpkits/calculate_lsm.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/codeframe_reader.py` & `dpkits-1.1/src/dpkits/codeframe_reader.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/data_analysis.py` & `dpkits-1.1/src/dpkits/data_analysis.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/data_processing.py` & `dpkits-1.1/src/dpkits/data_processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import numpy as np
 
 
 
 class DataProcessing:
 
     @staticmethod
-    def add_qres(df_data: pd.DataFrame, df_info: pd.DataFrame, dict_add_new_qres: dict) -> (pd.DataFrame, pd.DataFrame):
+    def add_qres(df_data: pd.DataFrame, df_info: pd.DataFrame, dict_add_new_qres: dict, is_add_oe_col: bool = False) -> (pd.DataFrame, pd.DataFrame):
         info_col_name = ['var_name', 'var_lbl', 'var_type', 'val_lbl']
 
         for key, val in dict_add_new_qres.items():
 
             if val[1] in ['MA']:
                 qre_ma_name, max_col = str(key).rsplit('|', 1)
 
                 for i in range(1, int(max_col) + 1):
                     df_info = pd.concat([df_info, pd.DataFrame(columns=info_col_name, data=[[f'{qre_ma_name}_{i}', val[0], val[1], val[2]]])], axis=0, ignore_index=True)
 
-                    if '_OE' not in key:
+                    if '_OE' not in key and not is_add_oe_col:
                         df_data = pd.concat([df_data, pd.DataFrame(columns=[f'{qre_ma_name}_{i}'], data=[val[-1]] * df_data.shape[0])], axis=1)
 
             else:
                 df_info = pd.concat([df_info, pd.DataFrame(columns=info_col_name, data=[[key, val[0], val[1], val[2]]])], axis=0, ignore_index=True)
 
-                if '_OE' not in key:
+                if '_OE' not in key and not is_add_oe_col:
                     df_data = pd.concat([df_data, pd.DataFrame(columns=[key], data=[val[-1]] * df_data.shape[0])], axis=1)
 
         
         df_data.reset_index(drop=True, inplace=True)
         df_info.reset_index(drop=True, inplace=True)
```

### Comparing `dpkits-1.0/src/dpkits/data_transpose.py` & `dpkits-1.1/src/dpkits/data_transpose.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/table_formater.py` & `dpkits-1.1/src/dpkits/table_formater.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits/table_generator.py` & `dpkits-1.1/src/dpkits/table_generator.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.0/src/dpkits.egg-info/PKG-INFO` & `dpkits-1.1/src/dpkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.0
+Version: 1.1
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

