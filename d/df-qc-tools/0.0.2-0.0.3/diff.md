# Comparing `tmp/df_qc_tools-0.0.2.tar.gz` & `tmp/df_qc_tools-0.0.3.tar.gz`

## Comparing `df_qc_tools-0.0.2.tar` & `df_qc_tools-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/__init__.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/config.py
--rw-r--r--   0        0        0    19983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/qc.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/src/df_qc_tools/qualityflags.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/test_config.py
--rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/test_qc.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/conf/conf_base.yaml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/resources/data_velocity_acc.csv
--rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/tests/resources/df_outliers.csv
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/.gitignore
--rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/LICENSE
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/README.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/src/df_qc_tools/__init__.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/src/df_qc_tools/config.py
+-rw-r--r--   0        0        0    20077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/src/df_qc_tools/qc.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/src/df_qc_tools/qualityflags.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/tests/test_config.py
+-rw-r--r--   0        0        0    29601 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/tests/test_qc.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/tests/conf/conf_base.yaml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/tests/resources/data_velocity_acc.csv
+-rw-r--r--   0        0        0  1417615 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/tests/resources/df_outliers.csv
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/.gitignore
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 df_qc_tools-0.0.3/PKG-INFO
```

### Comparing `df_qc_tools-0.0.2/Makefile` & `df_qc_tools-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/src/df_qc_tools/config.py` & `df_qc_tools-0.0.3/src/df_qc_tools/config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/src/df_qc_tools/qc.py` & `df_qc_tools-0.0.3/src/df_qc_tools/qc.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,18 @@
 
     def grad_function(group):
         nb_row, nb_columns = group.shape
         if nb_row < 2:
             group[Df.GRADIENT] = None
             return group
         g = np.gradient(
-            group.result, group.phenomenonTime.astype("datetime64[s]").astype("int64")
+            # group.result, group.phenomenonTime.astype("datetime64[s]").astype("int64")
+            group.result, group.phenomenonTime.astype("datetime64[ns]").astype("int64")
         )
-        group[Df.GRADIENT] = g
+        group[Df.GRADIENT] = g*1e9
         return group
 
     df_tmp = df.sort_values(Df.TIME)
     df_grouped = df.groupby(by=[groupby], group_keys=False)
     df_tmp = df_grouped[[str(Df.RESULT), str(Df.TIME)]].apply(
         grad_function
     )  # casted to string to avoid type error
```

### Comparing `df_qc_tools-0.0.2/tests/test_config.py` & `df_qc_tools-0.0.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/tests/test_qc.py` & `df_qc_tools-0.0.3/tests/test_qc.py`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/tests/resources/data_velocity_acc.csv` & `df_qc_tools-0.0.3/tests/resources/data_velocity_acc.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/tests/resources/df_outliers.csv` & `df_qc_tools-0.0.3/tests/resources/df_outliers.csv`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/LICENSE` & `df_qc_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `df_qc_tools-0.0.2/pyproject.toml` & `df_qc_tools-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "df-qc-tools"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="nvds" },
 ]
 description = "Package for easy datarequests from sensortings"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `df_qc_tools-0.0.2/PKG-INFO` & `df_qc_tools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: df-qc-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for easy datarequests from sensortings
 Project-URL: Homepage, https://github.com/nvdsteen/pandassta
 Project-URL: Issues, https://github.com/nvdsteen/pandassta/issues
 Author: nvds
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Requires-Dist: hydra-core==1.3.2
 Requires-Dist: numpy==1.26.4
 Requires-Dist: omegaconf==2.3.0
 Requires-Dist: pandas==2.2.1
 Requires-Dist: pandassta>=0.0.2
 Requires-Dist: pytest==8.1.1
 Requires-Dist: scipy==1.12.0
-Requires-Dist: searegion-detection>=0.0.2
+Requires-Dist: searegion-detection>=0.0.3
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: xarray==2024.2.0
 Description-Content-Type: text/markdown
 
 # df-qc-tools
 
 Tools to perform basic quality checks on observations stored in a pandas dataframe.
```

