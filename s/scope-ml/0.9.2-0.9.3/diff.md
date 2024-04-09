# Comparing `tmp/scope_ml-0.9.2.tar.gz` & `tmp/scope_ml-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scope_ml-0.9.2.tar", max compression
+gzip compressed data, was "scope_ml-0.9.3.tar", max compression
```

## Comparing `scope_ml-0.9.2.tar` & `scope_ml-0.9.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1082 2024-04-03 18:46:56.705888 scope_ml-0.9.2/LICENSE
--rw-r--r--   0        0        0     1427 2024-04-03 18:46:56.705888 scope_ml-0.9.2/README.md
--rw-r--r--   0        0        0    55490 2024-04-03 18:46:56.717888 scope_ml-0.9.2/config.defaults.yaml
--rw-r--r--   0        0        0     3370 2024-04-03 18:46:56.773888 scope_ml-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2755 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/__init__.py
--rw-r--r--   0        0        0      597 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/_instantiate.py
--rwxr-xr-x   0        0        0    13601 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/fritz.py
--rw-r--r--   0        0        0      883 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/models.py
--rw-r--r--   0        0        0    21602 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/nn.py
--rwxr-xr-x   0        0        0   113350 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/scope_class.py
--rw-r--r--   0        0        0    45857 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/utils.py
--rw-r--r--   0        0        0    20264 2024-04-03 18:46:56.773888 scope_ml-0.9.2/scope/xgb.py
--rw-r--r--   0        0        0     4163 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/DNN_AL_mapper.json
--rw-r--r--   0        0        0     4163 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/XGB_AL_mapper.json
--rwxr-xr-x   0        0        0     4346 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/analyze_logs.py
--rwxr-xr-x   0        0        0    11378 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/combine_preds.py
--rw-r--r--   0        0        0     3775 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/alertstats.py
--rw-r--r--   0        0        0     5460 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/external_xmatch.py
--rw-r--r--   0        0        0    12658 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/lcstats.py
--rw-r--r--   0        0        0    19686 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/periodsearch.py
--rw-r--r--   0        0        0        0 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/__init__.py
--rw-r--r--   0        0        0    29593 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aov.f90
--rw-r--r--   0        0        0      545 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aovconst.f90
--rw-r--r--   0        0        0     9369 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/aovsub.f90
--rw-r--r--   0        0        0      218 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/featureGeneration/pyaov/build.sh
--rw-r--r--   0        0        0     3983 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/fritz_mapper.json
--rwxr-xr-x   0        0        0    56855 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features.py
--rwxr-xr-x   0        0        0    12036 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features_job_submission.py
--rwxr-xr-x   0        0        0    18816 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/generate_features_slurm.py
--rwxr-xr-x   0        0        0    18067 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/get_features.py
--rwxr-xr-x   0        0        0    17448 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/get_quad_ids.py
--rw-r--r--   0        0        0     4334 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/golden_dataset_mapper.json
--rwxr-xr-x   0        0        0    28896 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/inference.py
--rw-r--r--   0        0        0       92 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/local_scope_radec.csv
--rw-r--r--   0        0        0       77 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/local_scope_ztfid.csv
--rwxr-xr-x   0        0        0     2652 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_inference_job_submission.py
--rwxr-xr-x   0        0        0     6219 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_inference_slurm.py
--rwxr-xr-x   0        0        0    12544 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/run_scope_local.py
--rwxr-xr-x   0        0        0    30136 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_download_classification.py
--rwxr-xr-x   0        0        0     6900 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_download_gcn_sources.py
--rwxr-xr-x   0        0        0     8254 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_manage_annotation.py
--rwxr-xr-x   0        0        0    34114 2024-04-03 18:46:56.777888 scope_ml-0.9.2/tools/scope_upload_classification.py
--rw-r--r--   0        0        0     3121 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/scope_upload_disagreements.py
--rwxr-xr-x   0        0        0     3873 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/taxonomy.py
--rwxr-xr-x   0        0        0     8018 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/train_algorithm_job_submission.py
--rwxr-xr-x   0        0        0     8380 2024-04-03 18:46:56.781888 scope_ml-0.9.2/tools/train_algorithm_slurm.py
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 scope_ml-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-09 01:08:30.317262 scope_ml-0.9.3/LICENSE
+-rw-r--r--   0        0        0     1427 2024-04-09 01:08:30.317262 scope_ml-0.9.3/README.md
+-rw-r--r--   0        0        0    55490 2024-04-09 01:08:30.329262 scope_ml-0.9.3/config.defaults.yaml
+-rw-r--r--   0        0        0     3527 2024-04-09 01:08:30.385262 scope_ml-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2755 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/_instantiate.py
+-rwxr-xr-x   0        0        0    13601 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/fritz.py
+-rw-r--r--   0        0        0      883 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/models.py
+-rw-r--r--   0        0        0    21602 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/nn.py
+-rwxr-xr-x   0        0        0   113350 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/scope_class.py
+-rw-r--r--   0        0        0    45857 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/utils.py
+-rw-r--r--   0        0        0    20264 2024-04-09 01:08:30.385262 scope_ml-0.9.3/scope/xgb.py
+-rw-r--r--   0        0        0     4163 2024-04-09 01:08:30.385262 scope_ml-0.9.3/tools/DNN_AL_mapper.json
+-rw-r--r--   0        0        0     4163 2024-04-09 01:08:30.385262 scope_ml-0.9.3/tools/XGB_AL_mapper.json
+-rwxr-xr-x   0        0        0     4346 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/analyze_logs.py
+-rwxr-xr-x   0        0        0    11647 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/combine_preds.py
+-rwxr-xr-x   0        0        0     4338 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/combine_preds_slurm.py
+-rw-r--r--   0        0        0     3775 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/alertstats.py
+-rw-r--r--   0        0        0     5460 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/external_xmatch.py
+-rw-r--r--   0        0        0    12658 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/lcstats.py
+-rw-r--r--   0        0        0    19686 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/periodsearch.py
+-rw-r--r--   0        0        0        0 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/__init__.py
+-rw-r--r--   0        0        0    29593 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aov.f90
+-rw-r--r--   0        0        0      545 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aovconst.f90
+-rw-r--r--   0        0        0     9369 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/aovsub.f90
+-rw-r--r--   0        0        0      218 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/featureGeneration/pyaov/build.sh
+-rw-r--r--   0        0        0     3983 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/fritz_mapper.json
+-rwxr-xr-x   0        0        0    56855 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features.py
+-rwxr-xr-x   0        0        0    12036 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features_job_submission.py
+-rwxr-xr-x   0        0        0    20587 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/generate_features_slurm.py
+-rwxr-xr-x   0        0        0    18037 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/get_features.py
+-rwxr-xr-x   0        0        0    17448 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/get_quad_ids.py
+-rw-r--r--   0        0        0     4334 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/golden_dataset_mapper.json
+-rwxr-xr-x   0        0        0    28896 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/inference.py
+-rw-r--r--   0        0        0       92 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/local_scope_radec.csv
+-rw-r--r--   0        0        0       77 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/local_scope_ztfid.csv
+-rwxr-xr-x   0        0        0     2652 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_inference_job_submission.py
+-rwxr-xr-x   0        0        0     6811 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_inference_slurm.py
+-rwxr-xr-x   0        0        0    12544 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/run_scope_local.py
+-rwxr-xr-x   0        0        0    30136 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_download_classification.py
+-rwxr-xr-x   0        0        0     6900 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_download_gcn_sources.py
+-rwxr-xr-x   0        0        0     8254 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_manage_annotation.py
+-rwxr-xr-x   0        0        0    34114 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_upload_classification.py
+-rw-r--r--   0        0        0     3121 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/scope_upload_disagreements.py
+-rwxr-xr-x   0        0        0     3873 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/taxonomy.py
+-rwxr-xr-x   0        0        0     8018 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/train_algorithm_job_submission.py
+-rwxr-xr-x   0        0        0     8971 2024-04-09 01:08:30.389263 scope_ml-0.9.3/tools/train_algorithm_slurm.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 scope_ml-0.9.3/PKG-INFO
```

### Comparing `scope_ml-0.9.2/LICENSE` & `scope_ml-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/README.md` & `scope_ml-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/config.defaults.yaml` & `scope_ml-0.9.3/config.defaults.yaml`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/pyproject.toml` & `scope_ml-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.black]
 target-version = ['py39', 'py310', 'py311']
 skip-string-normalization = true
 
 [tool.poetry]
 name = "scope-ml"
-version = "0.9.2"
+version = "0.9.3"
 description = "SCoPe: ZTF Source Classification Project"
 readme = "README.md"
 authors = ["Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al."]
 maintainers = ["Brian F. Healy <healyb@umn.edu>"]
 license = "MIT"
 repository = "https://github.com/ZwickyTransientFacility/scope"
 documentation = "https://zwickytransientfacility.github.io/scope-docs/"
@@ -28,15 +28,15 @@
 deepdiff = ">=5.0"
 gsutil = ">=4.60"
 keras-tuner = ">=1.0.2"
 matplotlib = ">=3.3"
 questionary = ">=1.8.1"
 scikit-learn = ">=0.24.1"
 tensorflow = ">=2.14.0,<=2.15.0"
-wandb = ">=0.12.1"
+wandb = ">=0.16.6"
 h5py = ">=3.10.0"
 astropy = ">=5.2.2"
 fast-histogram = ">=0.11"
 healpy = ">=1.16.2"
 jinja2 = "<=3.1"
 myst-parser = ">=0.18.1"
 pandas = ">=1.2"
@@ -47,14 +47,15 @@
 numba = ">=0.56.4"
 numpy = ">=1.23,<1.24"
 cesium = ">=0.11.1"
 xgboost = ">=1.7.5"
 seaborn = ">=0.12.2"
 pydot = ">=1.4.2"
 notebook = ">=7.0.6"
+cython = ">=3.0.10"
 tables = ">=3.7,<3.9.2"
 
 [tool.poetry.dev-dependencies]
 pre-commit = ">=3.5.0"
 pytest = ">=6.1.2"
 sphinx = ">=4.2"
 sphinx-press-theme = ">=0.8.0"
@@ -74,17 +75,19 @@
 scope-test = "scope._instantiate:test"
 scope-download-classification = "tools.scope_download_classification:main"
 scope-upload-classification = "tools.scope_upload_classification:main"
 scope-manage-annotation = "tools.scope_manage_annotation:main"
 post-taxonomy = "tools.taxonomy:main"
 generate-features = "tools.generate_features:main"
 generate-features-slurm = "tools.generate_features_slurm:main"
+check-quads-for-sources = "tools.generate_features_slurm:check_quads_for_sources"
 generate-features-job-submission = "tools.generate_features_job_submission:main"
 train-algorithm-slurm = "tools.train_algorithm_slurm:main"
 train-algorithm-job-submission = "tools.train_algorithm_job_submission:main"
 run-inference = "tools.inference:main"
 run-inference-slurm = "tools.run_inference_slurm:main"
 run-inference-job-submission = "tools.run_inference_job_submission:main"
 combine-preds = "tools.combine_preds:main"
+combine-preds-slurm = "tools.combine_preds_slurm:main"
 get-quad-ids = "tools.get_quad_ids:main"
 run-scope-local = "tools.run_scope_local:main"
 analyze-logs = "tools.analyze_logs:main"
```

### Comparing `scope_ml-0.9.2/scope/__init__.py` & `scope_ml-0.9.3/scope/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import shutil
 import os
 import site
 
 # Below code adapted from https://github.com/skyportal/skyportal/blob/main/skyportal/__init__.py
 # 2022-10-18
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 if "dev" in __version__:
     # Append last commit date and hash to dev version information, if available
 
     import subprocess
     import os.path
```

### Comparing `scope_ml-0.9.2/scope/_instantiate.py` & `scope_ml-0.9.3/scope/_instantiate.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/fritz.py` & `scope_ml-0.9.3/scope/fritz.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/models.py` & `scope_ml-0.9.3/scope/models.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/nn.py` & `scope_ml-0.9.3/scope/nn.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/scope_class.py` & `scope_ml-0.9.3/scope/scope_class.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/utils.py` & `scope_ml-0.9.3/scope/utils.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/scope/xgb.py` & `scope_ml-0.9.3/scope/xgb.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/DNN_AL_mapper.json` & `scope_ml-0.9.3/tools/DNN_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/XGB_AL_mapper.json` & `scope_ml-0.9.3/tools/XGB_AL_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/analyze_logs.py` & `scope_ml-0.9.3/tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/combine_preds.py` & `scope_ml-0.9.3/tools/combine_preds.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,26 +104,32 @@
     if save:
         os.makedirs(path_to_preds / combined_preds_dirname, exist_ok=True)
 
     done_fields = [
         str(x).split("/")[-1].split(".")[0]
         for x in (path_to_preds / combined_preds_dirname).glob("field_*.parquet")
     ]
-    done_fields.sort()
+    fields_to_list = done_fields.copy()
+
+    if fields_to_exclude is not None:
+        fields_to_list.extend(fields_to_exclude)
+
+    fields_to_do = list(set(fields_dnn_dict).difference(done_fields))
+    fields_to_list.extend(fields_to_do)
+
+    fields_to_list.sort()
 
     if save:
         # Write json file containing field list
         with open(path_to_preds / combined_preds_dirname / "fields.json", "w") as f:
-            json.dump(done_fields, f)
+            json.dump(fields_to_list, f)
 
     preds_to_save = None
     counter = 0
-    print(
-        f"Processing {len(set(fields_dnn_dict).difference(done_fields))} fields/files..."
-    )
+    print(f"Processing {len(fields_to_do)} fields/files...")
 
     for field in fields_dnn_dict.keys():
         if field not in done_fields:
             if field in fields_xgb_dict.keys():
                 try:
                     dnn_preds = read_parquet(
                         fields_dnn_dict[field] / f"{field}.parquet"
@@ -216,16 +222,17 @@
                             'w',
                         ) as f:
                             json.dump(meta_dict, f)
 
     return preds_to_save
 
 
-def get_parser():
-    parser = argparse.ArgumentParser()
+def get_parser(**kwargs):
+    add_help = kwargs.get("add_help", True)
+    parser = argparse.ArgumentParser(add_help=add_help)
     parser.add_argument(
         "--path-to-preds",
         type=pathlib.PosixPath,
         default=DEFAULT_PREDS_PATH,
         help="path to directories of existing and combined preds",
     )
     parser.add_argument(
```

### Comparing `scope_ml-0.9.2/tools/featureGeneration/alertstats.py` & `scope_ml-0.9.3/tools/featureGeneration/alertstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/external_xmatch.py` & `scope_ml-0.9.3/tools/featureGeneration/external_xmatch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/lcstats.py` & `scope_ml-0.9.3/tools/featureGeneration/lcstats.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/periodsearch.py` & `scope_ml-0.9.3/tools/featureGeneration/periodsearch.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/pyaov/aov.f90` & `scope_ml-0.9.3/tools/featureGeneration/pyaov/aov.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/pyaov/aovconst.f90` & `scope_ml-0.9.3/tools/featureGeneration/pyaov/aovconst.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/featureGeneration/pyaov/aovsub.f90` & `scope_ml-0.9.3/tools/featureGeneration/pyaov/aovsub.f90`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/fritz_mapper.json` & `scope_ml-0.9.3/tools/fritz_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/generate_features.py` & `scope_ml-0.9.3/tools/generate_features.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/generate_features_job_submission.py` & `scope_ml-0.9.3/tools/generate_features_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/generate_features_slurm.py` & `scope_ml-0.9.3/tools/generate_features_slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,24 @@
     :param filename: filename of saved results (str)
 
     :return field_dct: dictionary containing quadrants having at least one source (and optionally, number of sources per quad)
     :return has_sources: boolean stating whether each field in fields has sources
     :return missing_ccd_quad: boolean stating whether each field in fields has no sources in at least one ccd/quad
     """
 
+    parser = get_check_quads_parser()
+    args, _ = parser.parse_known_args()
+
+    fields = args.fields
+    catalog = args.catalog
+    count_sources = args.count_sources
+    minobs = args.minobs
+    save = args.save
+    filename = args.filename
+
     running_total_sources = 0
     has_sources = np.zeros(len(fields), dtype=bool)
     missing_ccd_quad = np.zeros(len(fields), dtype=bool)
     field_dct = {}
 
     if save and (os.path.isfile(BASE_DIR / f'{filename}.json')):
         with open(BASE_DIR / f'{filename}.json', 'r') as f:
@@ -172,14 +182,55 @@
     print(f"Sources found in {np.sum(has_sources)} fields.")
     if count_sources:
         print(f"Found {running_total_sources} sources.")
 
     return field_dct, has_sources, missing_ccd_quad
 
 
+def get_check_quads_parser():
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "--fields",
+        type=int,
+        nargs="+",
+        default=np.arange(0, 2000),
+        help="list of integer field numbers to query",
+    )
+    parser.add_argument(
+        "--catalog",
+        type=str,
+        default=source_catalog,
+        help="name of source catalog to query",
+    )
+    parser.add_argument(
+        "--count-sources",
+        action="store_true",
+        help="if set, count number of sources per quad and return",
+    )
+    parser.add_argument(
+        "--minobs",
+        type=int,
+        default=0,
+        help="minimum number of observations needed to count a source",
+    )
+    parser.add_argument(
+        "--save",
+        action="store_true",
+        help="if set, save results dictionary in json format",
+    )
+    parser.add_argument(
+        "--filename",
+        type=str,
+        default="catalog_completeness",
+        help="filename of saved results",
+    )
+
+    return parser
+
+
 def get_slurm_parser():
 
     fg_parser = get_parser(add_help=False)
     parser = argparse.ArgumentParser(parents=[fg_parser])
     parser.add_argument(
         "--job-name",
         type=str,
@@ -421,14 +472,20 @@
     fid.write(f'#SBATCH -A {args.account_name}\n')
 
     if args.cluster_name in ['Expanse', 'expanse', 'EXPANSE']:
         fid.write('module purge\n')
         fid.write('module add gpu/0.15.4\n')
         fid.write('module add cuda\n')
         fid.write(f'source activate {args.python_env_name}\n')
+    elif args.cluster_name in ['Delta', 'delta', 'DELTA']:
+        fid.write('module purge\n')
+        fid.write('module add anaconda3_gpu\n')
+        fid.write('module add cuda\n')
+        fid.write('module add gcc-runtime\n')
+        fid.write(f'source activate {args.python_env_name}\n')
 
     if args.doQuadrantFile:
         qid = '$QID'
         if args.quadrant_index is not None:
             qid = args.quadrant_index
         fid.write(
             'generate-features --source-catalog %s --alerts-catalog %s --gaia-catalog %s --bright-star-query-radius-arcsec %s --xmatch-radius-arcsec %s --query-size-limit %s --period-batch-size %s --samples-per-peak %s --Ncore %s --min-n-lc-points %s --min-cadence-minutes %s --dirname %s --filename %s --top-n-periods %s --max-freq %s --max-timestamp-hjd %s --doQuadrantFile --quadrant-file %s --quadrant-index %s %s %s\n'
@@ -498,14 +555,18 @@
     fid.write('#SBATCH --mail-type=ALL\n')
     fid.write(f'#SBATCH --mail-user={args.mail_user}\n')
 
     if args.cluster_name in ['Expanse', 'expanse', 'EXPANSE']:
         fid.write('module purge\n')
         fid.write('module add slurm\n')
         fid.write(f'source activate {args.python_env_name}\n')
+    elif args.cluster_name in ['Delta', 'delta', 'DELTA']:
+        fid.write('module purge\n')
+        fid.write('module add anaconda3_cpu\n')
+        fid.write(f'source activate {args.python_env_name}\n')
 
     if not args.doSubmitLoop:
         if args.runParallel:
             fid.write(
                 'generate-features-job-submission --dirname %s --filename %s --doSubmit --runParallel --max-instances %s --wait-time-minutes %s --user %s --submit-interval-minutes %s\n'
                 % (
                     dirpath,
```

### Comparing `scope_ml-0.9.2/tools/get_features.py` & `scope_ml-0.9.3/tools/get_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,27 +155,27 @@
     Stores the features in a file at the following location:
         features/field_<field>/field_<field>.parquet
     or  features/field_<field>/field_<field>.csv
     """
 
     if not whole_field:
         outfile = (
-            os.path.dirname(__file__)
-            + "/../features/field_"
+            str(BASE_DIR)
+            + "/features/field_"
             + str(field)
             + "/ccd_"
             + str(ccd).zfill(2)
             + "_quad_"
             + str(quad)
         )
 
     else:
         outfile = (
-            os.path.dirname(__file__)
-            + "/../features/field_"
+            str(BASE_DIR)
+            + "/features/field_"
             + str(field)
             + "/"
             + "field_"
             + str(field)
         )
 
     if suffix is not None:
```

### Comparing `scope_ml-0.9.2/tools/get_quad_ids.py` & `scope_ml-0.9.3/tools/get_quad_ids.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/golden_dataset_mapper.json` & `scope_ml-0.9.3/tools/golden_dataset_mapper.json`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/inference.py` & `scope_ml-0.9.3/tools/inference.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/run_inference_job_submission.py` & `scope_ml-0.9.3/tools/run_inference_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/run_inference_slurm.py` & `scope_ml-0.9.3/tools/train_algorithm_slurm.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,43 +2,66 @@
 import argparse
 import pathlib
 import os
 from scope.utils import parse_load_config
 
 
 BASE_DIR = pathlib.Path.cwd()
-BASE_DIR_PREDS = BASE_DIR
-
 config = parse_load_config()
 
-path_to_preds = config['inference']['path_to_preds']
-if path_to_preds is not None:
-    BASE_DIR_PREDS = pathlib.Path(path_to_preds)
+
+def parse_training_script(script_path):
+    with open(script_path, 'r') as f:
+        lines = f.readlines()
+
+    # Set defaults
+    tags = []
+    group = 'experiment'
+    algorithm = 'dnn'
+
+    for line in lines:
+        if 'scope-train' in line:
+            line_info = line.removeprefix('scope-train').split()
+            for arg in line_info.copy():
+                if '--tag' in arg:
+                    tag = arg.split('=')[1]
+                    tags += [tag]
+                    line_info.remove(arg)
+
+                if '--group' in arg:
+                    group = arg.split('=')[1]
+                    line_info.remove(arg)
+
+                if '--algorithm' in arg:
+                    algorithm = arg.split('=')[1]
+                    line_info.remove(arg)
+
+    return tags, group, algorithm, line_info
 
 
 def get_parser():
 
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--scriptname",
         type=str,
-        default='get_all_preds.sh',
-        help="Inference script filename within scope directory",
+        default='train_script.sh',
+        help="Training script filename within scope directory",
     )
     parser.add_argument(
         "--dirname",
         type=str,
-        default='inference',
+        default='training',
         help="Directory name for slurm scripts/logs",
     )
     parser.add_argument(
         "--job-name",
         type=str,
-        default='run_inference',
+        default='train',
         help="job name",
     )
     parser.add_argument(
         "--cluster-name",
         type=str,
         default='Expanse',
         help="Name of HPC cluster",
@@ -59,15 +82,15 @@
         "--nodes",
         type=int,
         default=1,
         help="Number of nodes to request for computing",
     )
     parser.add_argument(
         "--Ncore",
-        default=8,
+        default=4,
         type=int,
         help="number of cores to request for computing",
     )
     parser.add_argument(
         "--submit-nodes",
         type=int,
         default=1,
@@ -96,15 +119,15 @@
         type=int,
         default=16,
         help="Memory allocation to request for job submission",
     )
     parser.add_argument(
         "--time",
         type=str,
-        default='24:00:00',
+        default='12:00:00',
         help="Walltime for instance",
     )
     parser.add_argument(
         "--mail-user",
         type=str,
         default='healyb@umn.edu',
         help="contact email address",
@@ -118,51 +141,77 @@
     parser.add_argument(
         "--python-env-name",
         type=str,
         default='scope-env',
         help="Name of python environment to activate",
     )
     parser.add_argument(
+        "--generateTrainingFile",
+        action='store_true',
+        default=False,
+        help="if set, generate a list of labels and job numbers, save to slurm.dat",
+    )
+    parser.add_argument(
         "--user",
         type=str,
         default="bhealy",
         help="HPC username",
     )
     parser.add_argument(
-        "--algorithm",
-        type=str,
-        default="dnn",
-        help="dnn or xgb",
+        "--max-instances",
+        type=int,
+        default=20,
+        help="Max number of instances to run in parallel",
+    )
+    parser.add_argument(
+        "--wait-time-minutes",
+        type=float,
+        default=5.0,
+        help="Time to wait between job status checks (minutes)",
+    )
+    parser.add_argument(
+        "--submit-interval-seconds",
+        type=float,
+        default=5.0,
+        help="Time to wait between job submissions (seconds)",
+    )
+    parser.add_argument(
+        "--sweep",
+        action='store_true',
+        default=False,
+        help="If set, job submission runs filter_completed in different directory",
     )
 
     return parser
 
 
 def main():
     parser = get_parser()
     args, _ = parser.parse_known_args()
 
     scriptname = args.scriptname
-    script_path = BASE_DIR / scriptname
 
-    algorithm = args.algorithm
+    script_path = BASE_DIR / scriptname
+    _, _, algorithm, line_info = parse_training_script(script_path)
 
     dirname = f"{algorithm}_{args.dirname}"
     jobname = f"{args.job_name}_{algorithm}"
+    if args.sweep:
+        jobname += "_sweep"
 
-    dirpath = BASE_DIR_PREDS / dirname
+    dirpath = BASE_DIR / dirname
     os.makedirs(dirpath, exist_ok=True)
 
     slurmDir = os.path.join(dirpath, 'slurm')
     os.makedirs(slurmDir, exist_ok=True)
 
     logsDir = os.path.join(dirpath, 'logs')
     os.makedirs(logsDir, exist_ok=True)
 
-    # Main script to run feature generation
+    # Main script to run training
     fid = open(os.path.join(slurmDir, 'slurm.sub'), 'w')
     fid.write('#!/bin/bash\n')
     fid.write(f'#SBATCH --job-name={jobname}.job\n')
     fid.write(f'#SBATCH --output={dirname}/logs/{jobname}_%A_%a.out\n')
     fid.write(f'#SBATCH --error={dirname}/logs/{jobname}_%A_%a.err\n')
     fid.write(f'#SBATCH -p {args.partition_type}\n')
     fid.write(f'#SBATCH --nodes {args.nodes}\n')
@@ -176,19 +225,28 @@
 
     if args.cluster_name in ['Expanse', 'expanse', 'EXPANSE']:
         fid.write('module purge\n')
         if args.gpus > 0:
             fid.write('module add gpu/0.15.4\n')
             fid.write('module add cuda\n')
         fid.write(f'source activate {args.python_env_name}\n')
+    elif args.cluster_name in ['Delta', 'delta', 'DELTA']:
+        fid.write('module purge\n')
+        if args.gpus > 0:
+            fid.write('module add anaconda3_gpu\n')
+            fid.write('module add cuda\n')
+            fid.write('module add gcc-runtime\n')
+        else:
+            fid.write('module add anaconda3_cpu\n')
+        fid.write(f'source activate {args.python_env_name}\n')
 
-    fid.write(f"{script_path} $FID" + '\n')
+    fid.write("scope-train " + "--tag $TID " + " ".join(line_info) + '\n')
     fid.close()
 
-    # Secondary script to manage job submission using run_inference_job_submission.py
+    # Secondary script to manage job submission using train_algorithm_job_submission.py
     # (Python code can also be run interactively)
     fid = open(os.path.join(slurmDir, 'slurm_submission.sub'), 'w')
     fid.write('#!/bin/bash\n')
     fid.write(f'#SBATCH --job-name={jobname}_submit.job\n')
     fid.write(f'#SBATCH --output={dirname}/logs/{jobname}_submit_%A_%a.out\n')
     fid.write(f'#SBATCH --error={dirname}/logs/{jobname}_submit_%A_%a.err\n')
     fid.write(f'#SBATCH -p {args.submit_partition_type}\n')
@@ -200,18 +258,37 @@
     fid.write('#SBATCH --mail-type=ALL\n')
     fid.write(f'#SBATCH --mail-user={args.mail_user}\n')
 
     if args.cluster_name in ['Expanse', 'expanse', 'EXPANSE']:
         fid.write('module purge\n')
         fid.write('module add slurm\n')
         fid.write(f'source activate {args.python_env_name}\n')
+    elif args.cluster_name in ['Delta', 'delta', 'DELTA']:
+        fid.write('module purge\n')
+        fid.write('module add anaconda3_cpu\n')
+        fid.write(f'source activate {args.python_env_name}\n')
 
-    fid.write(
-        'run-inference-job-submission --dirname %s --scriptname %s --user %s --algorithm %s\n'
-        % (
-            dirname,
-            scriptname,
-            args.user,
-            algorithm,
+    if args.sweep:
+        fid.write(
+            'train-algorithm-job-submission --dirname %s --scriptname %s --user %s --max-instances %s --wait-time-minutes %s --submit-interval-seconds %s --sweep\n'
+            % (
+                dirname,
+                scriptname,
+                args.user,
+                args.max_instances,
+                args.wait_time_minutes,
+                args.submit_interval_seconds,
+            )
+        )
+    else:
+        fid.write(
+            'train-algorithm-job-submission --dirname %s --scriptname %s --user %s --max-instances %s --wait-time-minutes %s --submit-interval-seconds %s\n'
+            % (
+                dirname,
+                scriptname,
+                args.user,
+                args.max_instances,
+                args.wait_time_minutes,
+                args.submit_interval_seconds,
+            )
         )
-    )
     fid.close()
```

### Comparing `scope_ml-0.9.2/tools/run_scope_local.py` & `scope_ml-0.9.3/tools/run_scope_local.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/scope_download_classification.py` & `scope_ml-0.9.3/tools/scope_download_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/scope_download_gcn_sources.py` & `scope_ml-0.9.3/tools/scope_download_gcn_sources.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/scope_manage_annotation.py` & `scope_ml-0.9.3/tools/scope_manage_annotation.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/scope_upload_classification.py` & `scope_ml-0.9.3/tools/scope_upload_classification.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/scope_upload_disagreements.py` & `scope_ml-0.9.3/tools/scope_upload_disagreements.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/taxonomy.py` & `scope_ml-0.9.3/tools/taxonomy.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/tools/train_algorithm_job_submission.py` & `scope_ml-0.9.3/tools/train_algorithm_job_submission.py`

 * *Files identical despite different names*

### Comparing `scope_ml-0.9.2/PKG-INFO` & `scope_ml-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: scope-ml
-Version: 0.9.2
+Version: 0.9.3
 Summary: SCoPe: ZTF Source Classification Project
 Home-page: https://github.com/ZwickyTransientFacility/scope
 License: MIT
 Author: Brian F. Healy, Michael W. Coughlin, Ashish A. Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A. Hillenbrand, Jan van Roestel, Paula Szkody et al.
 Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=5.2.2)
 Requires-Dist: cesium (>=0.11.1)
+Requires-Dist: cython (>=3.0.10)
 Requires-Dist: deepdiff (>=5.0)
 Requires-Dist: fast-histogram (>=0.11)
 Requires-Dist: gsutil (>=4.60)
 Requires-Dist: h5py (>=3.10.0)
 Requires-Dist: healpy (>=1.16.2)
 Requires-Dist: jinja2 (<=3.1)
 Requires-Dist: keras-tuner (>=1.0.2)
@@ -34,15 +35,15 @@
 Requires-Dist: pyyaml (>=5.3.1)
 Requires-Dist: questionary (>=1.8.1)
 Requires-Dist: scikit-learn (>=0.24.1)
 Requires-Dist: seaborn (>=0.12.2)
 Requires-Dist: tables (>=3.7,<3.9.2)
 Requires-Dist: tdtax (>=0.1.6)
 Requires-Dist: tensorflow (>=2.14.0,<=2.15.0)
-Requires-Dist: wandb (>=0.12.1)
+Requires-Dist: wandb (>=0.16.6)
 Requires-Dist: xgboost (>=1.7.5)
 Project-URL: Documentation, https://zwickytransientfacility.github.io/scope-docs/
 Project-URL: Repository, https://github.com/ZwickyTransientFacility/scope
 Description-Content-Type: text/markdown
 
 # SCoPe: ZTF Source Classification Project
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: scope-ml Version: 0.9.2 Summary: SCoPe: ZTF Source
+Metadata-Version: 2.1 Name: scope-ml Version: 0.9.3 Summary: SCoPe: ZTF Source
 Classification Project Home-page: https://github.com/ZwickyTransientFacility/
 scope License: MIT Author: Brian F. Healy, Michael W. Coughlin, Ashish A.
 Mahabal, Theophile J. du Laz, Andrew Drake, Matthew J. Graham, Lynne A.
 Hillenbrand, Jan van Roestel, Paula Szkody et al. Maintainer: Brian F. Healy
 Maintainer-email: healyb@umn.edu Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: astropy (>=5.2.2) Requires-Dist: cesium
-(>=0.11.1) Requires-Dist: deepdiff (>=5.0) Requires-Dist: fast-histogram
-(>=0.11) Requires-Dist: gsutil (>=4.60) Requires-Dist: h5py (>=3.10.0)
-Requires-Dist: healpy (>=1.16.2) Requires-Dist: jinja2 (<=3.1) Requires-Dist:
-keras-tuner (>=1.0.2) Requires-Dist: matplotlib (>=3.3) Requires-Dist: myst-
-parser (>=0.18.1) Requires-Dist: notebook (>=7.0.6) Requires-Dist: numba
-(>=0.56.4) Requires-Dist: numpy (>=1.23,<1.24) Requires-Dist: pandas (>=1.2)
-Requires-Dist: penquins (>=2.4.0) Requires-Dist: pyarrow (>=9.0.0) Requires-
-Dist: pydot (>=1.4.2) Requires-Dist: pyyaml (>=5.3.1) Requires-Dist:
-questionary (>=1.8.1) Requires-Dist: scikit-learn (>=0.24.1) Requires-Dist:
-seaborn (>=0.12.2) Requires-Dist: tables (>=3.7,<3.9.2) Requires-Dist: tdtax
-(>=0.1.6) Requires-Dist: tensorflow (>=2.14.0,<=2.15.0) Requires-Dist: wandb
-(>=0.12.1) Requires-Dist: xgboost (>=1.7.5) Project-URL: Documentation, https:/
-/zwickytransientfacility.github.io/scope-docs/ Project-URL: Repository, https:/
-/github.com/ZwickyTransientFacility/scope Description-Content-Type: text/
-markdown # SCoPe: ZTF Source Classification Project [![PyPI version](https://
-badge.fury.io/py/scope-ml.svg)](https://badge.fury.io/py/scope-ml) [![arXiv]
-(https://img.shields.io/badge/arXiv-2102.11304-blue)](https://arxiv.org/abs/
-2102.11304) [![arXiv](https://img.shields.io/badge/arXiv-2009.14071-blue)]
-(https://arxiv.org/abs/2009.14071) [![arXiv](https://img.shields.io/badge/
-arXiv-2312.00143-blue)](https://arxiv.org/abs/2312.00143) `scope-ml` uses
-machine learning to classify light curves from the Zwicky Transient Facility (
-[ZTF](https://www.ztf.caltech.edu)). The documentation is hosted at [https://
-zwickytransientfacility.github.io/scope-docs/](https://
+(>=0.11.1) Requires-Dist: cython (>=3.0.10) Requires-Dist: deepdiff (>=5.0)
+Requires-Dist: fast-histogram (>=0.11) Requires-Dist: gsutil (>=4.60) Requires-
+Dist: h5py (>=3.10.0) Requires-Dist: healpy (>=1.16.2) Requires-Dist: jinja2
+(<=3.1) Requires-Dist: keras-tuner (>=1.0.2) Requires-Dist: matplotlib (>=3.3)
+Requires-Dist: myst-parser (>=0.18.1) Requires-Dist: notebook (>=7.0.6)
+Requires-Dist: numba (>=0.56.4) Requires-Dist: numpy (>=1.23,<1.24) Requires-
+Dist: pandas (>=1.2) Requires-Dist: penquins (>=2.4.0) Requires-Dist: pyarrow
+(>=9.0.0) Requires-Dist: pydot (>=1.4.2) Requires-Dist: pyyaml (>=5.3.1)
+Requires-Dist: questionary (>=1.8.1) Requires-Dist: scikit-learn (>=0.24.1)
+Requires-Dist: seaborn (>=0.12.2) Requires-Dist: tables (>=3.7,<3.9.2)
+Requires-Dist: tdtax (>=0.1.6) Requires-Dist: tensorflow (>=2.14.0,<=2.15.0)
+Requires-Dist: wandb (>=0.16.6) Requires-Dist: xgboost (>=1.7.5) Project-URL:
+Documentation, https://zwickytransientfacility.github.io/scope-docs/ Project-
+URL: Repository, https://github.com/ZwickyTransientFacility/scope Description-
+Content-Type: text/markdown # SCoPe: ZTF Source Classification Project [![PyPI
+version](https://badge.fury.io/py/scope-ml.svg)](https://badge.fury.io/py/
+scope-ml) [![arXiv](https://img.shields.io/badge/arXiv-2102.11304-blue)](https:
+//arxiv.org/abs/2102.11304) [![arXiv](https://img.shields.io/badge/arXiv-
+2009.14071-blue)](https://arxiv.org/abs/2009.14071) [![arXiv](https://
+img.shields.io/badge/arXiv-2312.00143-blue)](https://arxiv.org/abs/2312.00143)
+`scope-ml` uses machine learning to classify light curves from the Zwicky
+Transient Facility ([ZTF](https://www.ztf.caltech.edu)). The documentation is
+hosted at [https://zwickytransientfacility.github.io/scope-docs/](https://
 zwickytransientfacility.github.io/scope-docs/). To generate HTML files of the
 documentation locally, clone the repository and run `scope-doc` after
 installing. ## Funding We gratefully acknowledge previous and current support
 from the U.S. National Science Foundation (NSF) Harnessing the Data Revolution
 (HDR) Institute for _A_c_c_e_l_e_r_a_t_e_d_ _A_I_ _A_l_g_o_r_i_t_h_m_s_ _f_o_r_ _D_a_t_a_-_D_r_i_v_e_n_ _D_i_s_c_o_v_e_r_y_ _(_A_3_D_3_)
 under Cooperative Agreement No. _P_H_Y_-_2_1_1_7_9_9_7.
                                   [A3D3][NSF]
```

