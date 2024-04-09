# Comparing `tmp/cleanlab-studio-1.3.2.tar.gz` & `tmp/cleanlab-studio-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.3.2.tar", last modified: Fri Apr  5 17:09:34 2024, max compression
+gzip compressed data, was "cleanlab-studio-2.0.0.tar", last modified: Tue Apr  9 11:07:03 2024, max compression
```

## Comparing `cleanlab-studio-1.3.2.tar` & `cleanlab-studio-2.0.0.tar`

### file list

```diff
@@ -1,76 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.128367 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.132367 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 17:09:34.000000 cleanlab-studio-1.3.2/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:09:34.136367 cleanlab-studio-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-05 17:09:23.000000 cleanlab-studio-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.341770 cleanlab-studio-2.0.0/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.345770 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.349769 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24226 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24292 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26845 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 11:07:03.000000 cleanlab-studio-2.0.0/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:07:03.353770 cleanlab-studio-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-09 11:06:53.000000 cleanlab-studio-2.0.0/setup.py
```

### Comparing `cleanlab-studio-1.3.2/LICENSE` & `cleanlab-studio-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/PKG-INFO` & `cleanlab-studio-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.3.2
+Version: 2.0.0
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-1.3.2/README.md` & `cleanlab-studio-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/main.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/types.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/cli/util.py` & `cleanlab-studio-2.0.0/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/errors.py` & `cleanlab-studio-2.0.0/cleanlab_studio/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from asyncio import Handle
+
+
 class HandledError(Exception):
     pass
 
 
 class InvalidUUIDError(HandledError):
     pass
 
@@ -30,14 +33,18 @@
     pass
 
 
 class SettingsError(HandledError):
     pass
 
 
+class ValidationError(HandledError):
+    pass
+
+
 class UploadError(HandledError):
     pass
 
 
 class VersionError(HandledError):
     pass
 
@@ -59,24 +66,30 @@
         return f"{self.error_type}: {self.message}"
 
 
 class APITimeoutError(HandledError):
     pass
 
 
-class RateLimitError(APIError):
+class RateLimitError(HandledError):
     def __init__(self, message: str, retry_after: int):
         self.message = message
         self.retry_after = retry_after
 
 
-class TlmBadRequest(APIError):
+class TlmBadRequest(HandledError):
     pass
 
 
+class TlmServerError(APIError):
+    def __init__(self, message: str, status_code: int) -> None:
+        self.message = message
+        self.status_code = status_code
+
+
 class UnsupportedVersionError(HandledError):
     def __init__(self) -> None:
         super().__init__(
             "cleanlab-studio is out of date and must be upgraded. Run 'pip install --upgrade cleanlab-studio'."
         )
```

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import asyncio
 import io
-from math import e
 import os
 import time
 from typing import Callable, cast, List, Optional, Tuple, Dict, Union, Any
+
 from cleanlab_studio.errors import (
     APIError,
     IngestionError,
     InvalidProjectConfiguration,
     RateLimitError,
     TlmBadRequest,
+    TlmServerError,
 )
-from cleanlab_studio.internal.util import get_basic_info, obfuscate_stack_trace
+from cleanlab_studio.internal.tlm.concurrency import TlmRateHandler
 
 import aiohttp
+import aiohttp.client_exceptions
 import requests
 from tqdm import tqdm
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
 
 try:
@@ -84,26 +86,48 @@
     """Catches 429 (rate limit) errors."""
     if resp.status == 429:
         raise RateLimitError(
             f"Rate limit exceeded on {resp.url}", int(resp.headers.get("Retry-After", 0))
         )
 
 
-async def handle_tlm_client_error_from_resp(resp: aiohttp.ClientResponse) -> None:
+async def handle_tlm_client_error_from_resp(
+    resp: aiohttp.ClientResponse, batch_index: Optional[int]
+) -> None:
     """Catches 4XX (client error) errors."""
     if 400 <= resp.status < 500:
         try:
             res_json = await resp.json()
             error_message = res_json["error"]
         except Exception:
-            error_message = "Client error occurred."
+            error_message = "TLM query failed. Please try again and contact support@cleanlab.ai if the problem persists."
+
+        if batch_index is not None:
+            error_message = f"Error executing query at index {batch_index}:\n{error_message}"
 
         raise TlmBadRequest(error_message)
 
 
+async def handle_tlm_api_error_from_resp(
+    resp: aiohttp.ClientResponse, batch_index: Optional[int]
+) -> None:
+    """Catches 5XX (server error) errors."""
+    if 500 <= resp.status < 600:
+        try:
+            res_json = await resp.json()
+            error_message = res_json["error"]
+        except Exception:
+            error_message = "TLM query failed. Please try again and contact support@cleanlab.ai if the problem persists."
+
+        if batch_index is not None:
+            error_message = f"Error executing query at index {batch_index}:\n{error_message}"
+
+        raise TlmServerError(error_message, resp.status)
+
+
 def validate_api_key(api_key: str) -> bool:
     res = requests.get(
         cli_base_url + "/validate",
         json=dict(api_key=api_key),
         headers=_construct_headers(api_key),
     )
     handle_api_error(res)
@@ -552,14 +576,17 @@
         error_message = ""
 
         num_try = 0
         while num_try <= retries:
             await asyncio.sleep(sleep_time)
             try:
                 return await func(*args, **kwargs)
+            except aiohttp.client_exceptions.ClientConnectorError as e:
+                # note: we don't increment num_try here, because we don't want connection errors to count against the total number of retries
+                sleep_time = 2**num_try
             except RateLimitError as e:
                 # note: we don't increment num_try here, because we don't want rate limit retries to count against the total number of retries
                 sleep_time = e.retry_after
             except TlmBadRequest as e:
                 # dont retry for client-side errors
                 raise e
             except Exception as e:
@@ -574,45 +601,51 @@
 
 @tlm_retry
 async def tlm_prompt(
     api_key: str,
     prompt: str,
     quality_preset: str,
     options: Optional[JSONDict],
+    rate_handler: TlmRateHandler,
     client_session: Optional[aiohttp.ClientSession] = None,
+    batch_index: Optional[int] = None,
 ) -> JSONDict:
     """
     Prompt Trustworthy Language Model with a question, and get back its answer along with a confidence score
 
     Args:
         api_key (str): studio API key for auth
         prompt (str): prompt for TLM to respond to
         quality_preset (str): quality preset to use to generate response
         options (JSONDict): additional parameters for TLM
+        rate_handler (TlmRateHandler): concurrency handler used to manage TLM request rate
         client_session (aiohttp.ClientSession): client session used to issue TLM request
+        batch_index (Optional[int], optional): index of prompt in batch, used for error messages. Defaults to None if not in batch.
 
     Returns:
         JSONDict: dictionary with TLM response and confidence score
     """
     local_scoped_client = False
     if not client_session:
         client_session = aiohttp.ClientSession()
         local_scoped_client = True
 
     try:
-        res = await client_session.post(
-            f"{tlm_base_url}/prompt",
-            json=dict(prompt=prompt, quality=quality_preset, options=options or {}),
-            headers=_construct_headers(api_key),
-        )
-        res_json = await res.json()
+        async with rate_handler:
+            res = await client_session.post(
+                f"{tlm_base_url}/prompt",
+                json=dict(prompt=prompt, quality=quality_preset, options=options or {}),
+                headers=_construct_headers(api_key),
+            )
 
-        handle_rate_limit_error_from_resp(res)
-        await handle_tlm_client_error_from_resp(res)
-        handle_api_error_from_json(res_json)
+            res_json = await res.json()
+
+            handle_rate_limit_error_from_resp(res)
+            await handle_tlm_client_error_from_resp(res, batch_index)
+            await handle_tlm_api_error_from_resp(res, batch_index)
 
     finally:
         if local_scoped_client:
             await client_session.close()
 
     return cast(JSONDict, res_json)
 
@@ -620,51 +653,54 @@
 @tlm_retry
 async def tlm_get_confidence_score(
     api_key: str,
     prompt: str,
     response: str,
     quality_preset: str,
     options: Optional[JSONDict],
+    rate_handler: TlmRateHandler,
     client_session: Optional[aiohttp.ClientSession] = None,
+    batch_index: Optional[int] = None,
 ) -> JSONDict:
     """
     Query Trustworthy Language Model for a confidence score for the prompt-response pair.
 
     Args:
         api_key (str): studio API key for auth
         prompt (str): prompt for TLM to get confidence score for
         response (str): response for TLM to get confidence score for
         quality_preset (str): quality preset to use to generate confidence score
         options (JSONDict): additional parameters for TLM
+        rate_handler (TlmRateHandler): concurrency handler used to manage TLM request rate
         client_session (aiohttp.ClientSession): client session used to issue TLM request
+        batch_index (Optional[int], optional): index of prompt in batch, used for error messages. Defaults to None if not in batch.
 
     Returns:
         JSONDict: dictionary with TLM confidence score
     """
     local_scoped_client = False
     if not client_session:
         client_session = aiohttp.ClientSession()
         local_scoped_client = True
 
     try:
-        res = await client_session.post(
-            f"{tlm_base_url}/get_confidence_score",
-            json=dict(
-                prompt=prompt, response=response, quality=quality_preset, options=options or {}
-            ),
-            headers=_construct_headers(api_key),
-        )
-        res_json = await res.json()
+        async with rate_handler:
+            res = await client_session.post(
+                f"{tlm_base_url}/get_confidence_score",
+                json=dict(
+                    prompt=prompt, response=response, quality=quality_preset, options=options or {}
+                ),
+                headers=_construct_headers(api_key),
+            )
 
-        if local_scoped_client:
-            await client_session.close()
+            res_json = await res.json()
 
-        handle_rate_limit_error_from_resp(res)
-        await handle_tlm_client_error_from_resp(res)
-        handle_api_error_from_json(res_json)
+            handle_rate_limit_error_from_resp(res)
+            await handle_tlm_client_error_from_resp(res, batch_index)
+            await handle_tlm_api_error_from_resp(res, batch_index)
 
     finally:
         if local_scoped_client:
             await client_session.close()
 
     return cast(JSONDict, res_json)
```

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/clean_helpers.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/settings.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/internal/util.py` & `cleanlab-studio-2.0.0/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/studio/inference.py` & `cleanlab-studio-2.0.0/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/studio/studio.py` & `cleanlab-studio-2.0.0/cleanlab_studio/studio/studio.py`

 * *Files 8% similar despite different names*

```diff
@@ -386,28 +386,49 @@
 
             3. If there are rows flagged as `is_not_analyzed`, the rows of the feature embeddings will correspond to the rows of the original dataset after filtering out the rows that are not analyzed.
         """
         return np.asarray(api.download_array(self._api_key, cleanset_id, "embeddings"))
 
     def TLM(
         self,
-        *,
         quality_preset: TLMQualityPreset = "medium",
-        **kwargs: Any,
+        *,
+        options: Optional[trustworthy_language_model.TLMOptions] = None,
+        timeout: Optional[float] = None,
+        verbose: Optional[bool] = None,
     ) -> trustworthy_language_model.TLM:
-        """Gets Trustworthy Language Model (TLM) object to prompt.
+        """Gets a configured instance of Trustworthy Language Model (TLM).
+
+        The returned TLM object can then be used as a drop-in replacement for an LLM, for estimating trustworthiness scores for LLM prompt/response pairs, and more. See the documentation for the [TLM](../trustworthy_language_model#class-TLM) class for more on what you can do with TLM.
+
+        For advanced use cases, TLM supports a number of configuration options. The documentation below summarizes the options, and the [TLM tutorial](/tutorials/tlm) explains the tradeoffs in more detail.
 
         Args:
-            quality_preset: quality preset to use for prompts
-            kwargs (Any): additional kwargs to pass to TLM class
+            quality_preset (TLMQualityPreset): quality preset to use for TLM queries, which will determine the quality of the output responses and trustworthiness scores.
+            Supported presets include "best", "high", "medium", "low", "base".
+            The "best" and "high" presets will improve the LLM responses themselves, with "best" also returning the most reliable trustworthiness scores.
+            The "medium" and "low" presets will return standard LLM responses along with associated confidence scores,
+            with "medium" producing more reliable trustworthiness scores than low.
+            The "base" preset will not return any confidence score, just a standard LLM output response, this option is similar to using your favorite LLM API.
+            Higher presets have increased runtime and cost.
+
+            options (TLMOptions, optional): a typed dict of advanced configuration options.
+            Options that can be passed in include "model", "max_tokens", "num_candidate_responses", "num_consistency_samples", "use_self_reflection".
+            For more details about the options, see the documentation for [TLMOptions](../trustworthy_language_model#class-tlmoptions).
+
+            timeout (float, optional): timeout (in seconds) to apply to each method call. If a result is not produced within the timeout, a TimeoutError will be raised. Defaults to None, which does not apply a timeout.
+
+            verbose (bool, optional): whether to run in verbose mode, i.e., whether to show a tqdm progress bar when TLM is prompted with batches of data. If None, this will be determined automatically based on whether the code is running in an interactive environment such as a notebook.
 
         Returns:
             TLM: the [Trustworthy Language Model](../trustworthy_language_model#class-tlm) object
         """
-        return trustworthy_language_model.TLM(self._api_key, quality_preset, **kwargs)
+        return trustworthy_language_model.TLM(
+            self._api_key, quality_preset, options=options, timeout=timeout, verbose=verbose
+        )
 
     def poll_cleanset_status(self, cleanset_id: str, timeout: Optional[int] = None) -> bool:
         """
         This method has been deprecated, instead use: `wait_until_cleanset_ready()`
 
         Repeatedly polls for cleanset status while the cleanset is being generated. Blocks until cleanset is ready, there is a cleanset error, or `timeout` is exceeded.
```

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio/utils/synthetic.py` & `cleanlab-studio-2.0.0/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-2.0.0/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.3.2
+Version: 2.0.0
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab-studio-1.3.2/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-2.0.0/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -48,13 +48,16 @@
 cleanlab_studio/internal/dataset_source/__init__.py
 cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
 cleanlab_studio/internal/dataset_source/dataset_source.py
 cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
 cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
 cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
 cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+cleanlab_studio/internal/tlm/__init__.py
+cleanlab_studio/internal/tlm/concurrency.py
+cleanlab_studio/internal/tlm/validation.py
 cleanlab_studio/studio/__init__.py
 cleanlab_studio/studio/inference.py
 cleanlab_studio/studio/studio.py
 cleanlab_studio/studio/trustworthy_language_model.py
 cleanlab_studio/utils/__init__.py
 cleanlab_studio/utils/synthetic.py
```

### Comparing `cleanlab-studio-1.3.2/setup.py` & `cleanlab-studio-2.0.0/setup.py`

 * *Files identical despite different names*

