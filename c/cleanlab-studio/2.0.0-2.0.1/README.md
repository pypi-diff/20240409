# Comparing `tmp/cleanlab-studio-2.0.0.tar.gz` & `tmp/cleanlab-studio-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-2.0.0.tar", last modified: Tue Apr  9 11:07:03 2024, max compression
+gzip compressed data, was "cleanlab-studio-2.0.1.tar", last modified: Tue Apr  9 19:10:11 2024, max compression
```

## Comparing `cleanlab-studio-2.0.0.tar` & `cleanlab-studio-2.0.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.341770 cleanlab-studio-2.0.0/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24226 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    26845 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.040750 cleanlab-studio-2.0.1/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.044750 cleanlab-studio-2.0.1/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24245 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24094 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26845 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 19:10:11.000000 cleanlab-studio-2.0.1/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:10:11.048750 cleanlab-studio-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 19:09:59.000000 cleanlab-studio-2.0.1/setup.py
```

### Comparing `cleanlab-studio-2.0.0/LICENSE` & `cleanlab-studio-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/PKG-INFO` & `cleanlab-studio-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.0
+Version: 2.0.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-2.0.0/README.md` & `cleanlab-studio-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/main.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/types.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/cli/util.py` & `cleanlab-studio-2.0.1/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/errors.py` & `cleanlab-studio-2.0.1/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/api/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         cleanset_pyspark = cleanset_pyspark.withColumnRenamed("id", id_col)
         cleanset_pyspark = cleanset_pyspark.sort(id_col)
         return cleanset_pyspark
 
     cleanset_json_io = io.StringIO(cleanset_json)
     cleanset_pd: pd.DataFrame = pd.read_json(cleanset_json_io, orient="table")
     cleanset_pd.rename(columns={"id": id_col}, inplace=True)
-    cleanset_pd.sort_values(by=id_col, inplace=True)
+    cleanset_pd.sort_values(by=id_col, inplace=True, ignore_index=True)
     return cleanset_pd
 
 
 def download_array(
     api_key: str, cleanset_id: str, name: str
 ) -> Union[npt.NDArray[np.float_], pd.DataFrame]:
     check_uuid_well_formed(cleanset_id, "cleanset ID")
```

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/clean_helpers.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/constants.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/settings.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/concurrency.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/concurrency.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/validation.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/tlm/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/internal/util.py` & `cleanlab-studio-2.0.1/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/studio/inference.py` & `cleanlab-studio-2.0.1/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/studio/studio.py` & `cleanlab-studio-2.0.1/cleanlab_studio/studio/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,19 +134,14 @@
         rows_df = api.download_cleanlab_columns(
             self._api_key,
             cleanset_id,
             include_cleanlab_columns=include_cleanlab_columns,
             include_project_details=include_project_details,
             to_spark=to_spark,
         )
-        if "cleanlab_row_ID" in rows_df.columns:
-            if to_spark:
-                rows_df.sort("cleanlab_row_ID")
-            else:
-                rows_df.sort_values(by="cleanlab_row_ID")
         return rows_df
 
     def apply_corrections(self, cleanset_id: str, dataset: Any, keep_excluded: bool = False) -> Any:
         """
         Applies corrections from a Cleanlab Studio cleanset to your dataset. This function takes in your local copy of the original dataset, as well as the `cleanset_id` for the cleanset generated from this dataset in the Project web interface. The function returns a copy of your original dataset, where the label column has been substituted with corrected labels that you selected (either manually or via auto-fix) in the Cleanlab Studio web interface Project, and the rows you marked as excluded will be excluded from the returned copy of your original dataset. Corrections should have been made by viewing your Project in the Cleanlab Studio web interface (see [Cleanlab Studio web quickstart](/guide/quickstart/web#review-issues-detected-in-your-dataset-and-correct-them)).
 
         The intended workflow is: create a Project, correct your Dataset automatically/manually in the web interface to generate a Cleanset (cleaned dataset), then call this function to make your original dataset locally look like the current Cleanset.
```

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab-studio-2.0.1/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio/utils/synthetic.py` & `cleanlab-studio-2.0.1/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-2.0.1/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.0
+Version: 2.0.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-2.0.0/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-2.0.1/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-2.0.0/setup.py` & `cleanlab-studio-2.0.1/setup.py`

 * *Files identical despite different names*

