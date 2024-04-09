# Comparing `tmp/idc_index_data-17.0.1.tar.gz` & `tmp/idc_index_data-17.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idc_index_data-17.0.1.tar", last modified: Tue Apr  9 12:41:39 2024, max compression
+gzip compressed data, was "idc_index_data-17.0.2.tar", last modified: Tue Apr  9 19:24:52 2024, max compression
```

## Comparing `idc_index_data-17.0.1.tar` & `idc_index_data-17.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      125 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.gitattributes
--rw-r--r--   0        0        0     2858 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1089 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2217 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      313 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.github/workflows/keep-alive.yml
--rw-r--r--   0        0        0     2264 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.gitignore
--rw-r--r--   0        0        0     2313 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1352 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/CMakeLists.txt
--rw-r--r--   0        0        0     1054 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/LICENSE
--rw-r--r--   0        0        0     2293 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/README.md
--rw-r--r--   0        0        0      849 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/docs/conf.py
--rw-r--r--   0        0        0      201 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/docs/index.md
--rw-r--r--   0        0        0     5359 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/noxfile.py
--rw-r--r--   0        0        0     4173 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/pyproject.toml
--rw-r--r--   0        0        0     4920 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/scripts/python/idc_index_data_manager.py
--rwxr-xr-x   0        0        0     2653 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/scripts/python/update_idc_index_version.py
--rw-r--r--   0        0        0     1403 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/scripts/sql/idc_index.sql
--rw-r--r--   0        0        0     1058 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/src/idc_index_data/__init__.py
--rw-r--r--   0        0        0       49 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/src/idc_index_data/_version.pyi
--rw-r--r--   0        0        0        0 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/src/idc_index_data/py.typed
--rw-r--r--   0        0        0      745 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/tests/test_package.py
--rw-r--r--   0        0        0     5352 2024-04-09 12:41:39.000000 idc_index_data-17.0.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.gitattributes
+-rw-r--r--   0        0        0     2858 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1089 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2217 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      313 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.github/workflows/keep-alive.yml
+-rw-r--r--   0        0        0     2264 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.gitignore
+-rw-r--r--   0        0        0     2338 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1352 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1054 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/LICENSE
+-rw-r--r--   0        0        0     2293 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/README.md
+-rw-r--r--   0        0        0      849 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/docs/conf.py
+-rw-r--r--   0        0        0      201 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/docs/index.md
+-rw-r--r--   0        0        0     5359 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/noxfile.py
+-rw-r--r--   0        0        0     4198 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5034 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/python/idc_index_data_manager.py
+-rwxr-xr-x   0        0        0     2653 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/python/update_idc_index_version.py
+-rw-r--r--   0        0        0     1349 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/scripts/sql/idc_index.sql
+-rw-r--r--   0        0        0     1058 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/__init__.py
+-rw-r--r--   0        0        0       49 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/_version.pyi
+-rw-r--r--   0        0        0        0 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/src/idc_index_data/py.typed
+-rw-r--r--   0        0        0     1206 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/tests/test_package.py
+-rw-r--r--   0        0        0     5431 2024-04-09 19:24:52.000000 idc_index_data-17.0.2/PKG-INFO
```

### Comparing `idc_index_data-17.0.1/.github/CONTRIBUTING.md` & `idc_index_data-17.0.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/.github/matchers/pylint.json` & `idc_index_data-17.0.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/.github/workflows/cd.yml` & `idc_index_data-17.0.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/.github/workflows/ci.yml` & `idc_index_data-17.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/.gitignore` & `idc_index_data-17.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/.pre-commit-config.yaml` & `idc_index_data-17.0.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     rev: "v1.8.0"
     hooks:
       - id: mypy
         files: src|tests
         args: []
         additional_dependencies:
           - pytest
+          - pandas-stubs
 
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
```

### Comparing `idc_index_data-17.0.1/CMakeLists.txt` & `idc_index_data-17.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/LICENSE` & `idc_index_data-17.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/README.md` & `idc_index_data-17.0.2/README.md`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/docs/conf.py` & `idc_index_data-17.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/noxfile.py` & `idc_index_data-17.0.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/pyproject.toml` & `idc_index_data-17.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "requests"
 ]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "idc-index-data"
-version = "17.0.1"
+version = "17.0.2"
 authors = [
   { name = "Andrey Fedorov", email = "andrey.fedorov@gmail.com" },
   { name = "Vamsi Thiriveedhi", email = "vthiriveedhi@mgh.harvard.edu" },
   { name = "Jean-Christophe Fillion-Robin", email = "jchris.fillionr@kitware.com" },
 ]
 description = "ImagingDataCommons index to query and download data."
 readme = "README.md"
@@ -40,14 +40,16 @@
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 dependencies = []
 
 [project.optional-dependencies]
 test = [
+  "pandas",
+  "pyarrow",
   "pytest >=6",
   "pytest-cov >=3",
 ]
 dev = [
   "pytest >=6",
   "pytest-cov >=3",
 ]
```

### Comparing `idc_index_data-17.0.1/scripts/python/idc_index_data_manager.py` & `idc_index_data-17.0.2/scripts/python/idc_index_data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         Returns:
             Tuple[pd.DataFrame, str]: A tuple containing the DataFrame with query results,
             the output basename.
         """
         with Path(file_path).open("r") as file:
             sql_query = file.read()
         index_df = self.client.query(sql_query).to_dataframe()
+        if "StudyDate" in index_df.columns:
+            index_df["StudyDate"] = index_df["StudyDate"].astype(str)
         output_basename = Path(file_path).name.split(".")[0]
         logger.debug("Executed SQL query from file: %s", file_path)
         return index_df, output_basename
 
     def generate_index_data_files(
         self, generate_compressed_csv: bool = True, generate_parquet: bool = False
     ) -> None:
```

### Comparing `idc_index_data-17.0.1/scripts/python/update_idc_index_version.py` & `idc_index_data-17.0.2/scripts/python/update_idc_index_version.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/scripts/sql/idc_index.sql` & `idc_index_data-17.0.2/scripts/sql/idc_index.sql`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   ANY_VALUE(ManufacturerModelName) AS ManufacturerModelName,
   ANY_VALUE(SAFE_CAST(SeriesDate AS STRING)) AS SeriesDate,
   ANY_VALUE(SeriesDescription) AS SeriesDescription,
   ANY_VALUE(SeriesNumber) AS SeriesNumber,
   COUNT(dicom_all.SOPInstanceUID) AS instanceCount,
   ANY_VALUE(license_short_name) as license_short_name,
   # download related attributes
-  ANY_VALUE(CONCAT("s3://", SPLIT(aws_url,"/")[SAFE_OFFSET(2)], "/", crdc_series_uuid, "/*")) AS series_aws_url,
+  ANY_VALUE(CONCAT(series_aws_url,"*")) AS series_aws_url,
   ROUND(SUM(SAFE_CAST(instance_size AS float64))/1000000, 2) AS series_size_MB,
 FROM
   `bigquery-public-data.idc_v17.dicom_all` AS dicom_all
 JOIN
   `bigquery-public-data.idc_v17.dicom_metadata_curated` AS dicom_curated
 ON
   dicom_all.SOPInstanceUID = dicom_curated.SOPInstanceUID
```

### Comparing `idc_index_data-17.0.1/src/idc_index_data/__init__.py` & `idc_index_data-17.0.2/src/idc_index_data/__init__.py`

 * *Files identical despite different names*

### Comparing `idc_index_data-17.0.1/PKG-INFO` & `idc_index_data-17.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idc-index-data
-Version: 17.0.1
+Version: 17.0.2
 Summary: ImagingDataCommons index to query and download data.
 Author-Email: Andrey Fedorov <andrey.fedorov@gmail.com>, Vamsi Thiriveedhi <vthiriveedhi@mgh.harvard.edu>, Jean-Christophe Fillion-Robin <jchris.fillionr@kitware.com>
 License: Copyright 2024 Andrey Fedorov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
@@ -41,14 +41,16 @@
 Project-URL: Bug tracker, https://github.com/ImagingDataCommons/idc-index-data/issues
 Project-URL: Discussions, https://discourse.canceridc.dev/
 Project-URL: Changelog, https://github.com/ImagingDataCommons/idc-index-data/releases
 Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
+Requires-Dist: pandas; extra == "test"
+Requires-Dist: pyarrow; extra == "test"
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: pytest-cov>=3; extra == "test"
 Requires-Dist: pytest>=6; extra == "dev"
 Requires-Dist: pytest-cov>=3; extra == "dev"
 Requires-Dist: sphinx>=7.0; extra == "docs"
 Requires-Dist: myst_parser>=0.13; extra == "docs"
 Requires-Dist: sphinx_copybutton; extra == "docs"
```

