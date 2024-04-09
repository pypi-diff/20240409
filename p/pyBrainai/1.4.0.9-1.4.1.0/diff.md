# Comparing `tmp/pyBrainai-1.4.0.9.tar.gz` & `tmp/pyBrainai-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBrainai-1.4.0.9.tar", last modified: Sun Mar 31 04:36:12 2024, max compression
+gzip compressed data, was "pyBrainai-1.4.1.0.tar", last modified: Tue Apr  9 10:01:34 2024, max compression
```

## Comparing `pyBrainai-1.4.0.9.tar` & `pyBrainai-1.4.1.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/
--rw-rw-r--   0 root         (0) root         (0)     1088 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      728 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      223 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/
--rw-rw-r--   0 root         (0) root         (0)     2989 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2659 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/_openai_scripts.py
--rw-rw-r--   0 root         (0) root         (0)    26948 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_requestor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/api_resources/
--rw-rw-r--   0 root         (0) root         (0)     1099 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/api_resources/abstract/
--rw-rw-r--   0 root         (0) root         (0)      659 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5628 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2677 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/createable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     1676 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/deletable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)    10530 2024-03-31 04:32:00.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/engine_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2785 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/listable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     5810 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/nested_resource_class_methods.py
--rw-rw-r--   0 root         (0) root         (0)     3590 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/paginatable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      551 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/abstract/updateable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     7955 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/audio.py
--rw-rw-r--   0 root         (0) root         (0)     4182 2024-03-31 04:31:15.000000 pyBrainai-1.4.0.9/brainai/api_resources/brainos_completion.py
--rw-rw-r--   0 root         (0) root         (0)     2988 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/chat_completion.py
--rw-rw-r--   0 root         (0) root         (0)     1668 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/completion.py
--rw-rw-r--   0 root         (0) root         (0)      560 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/customer.py
--rw-rw-r--   0 root         (0) root         (0)     4177 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/deployment.py
--rw-rw-r--   0 root         (0) root         (0)     2025 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/edit.py
--rw-rw-r--   0 root         (0) root         (0)     3536 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/embedding.py
--rw-rw-r--   0 root         (0) root         (0)     1718 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/engine.py
--rw-rw-r--   0 root         (0) root         (0)      925 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/error_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/api_resources/experimental/
--rw-rw-r--   0 root         (0) root         (0)      108 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/experimental/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      286 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/experimental/completion_config.py
--rw-rw-r--   0 root         (0) root         (0)     8728 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/file.py
--rw-rw-r--   0 root         (0) root         (0)     5480 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/fine_tune.py
--rw-rw-r--   0 root         (0) root         (0)     2354 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/fine_tuning.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/image.py
--rw-rw-r--   0 root         (0) root         (0)      175 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/model.py
--rw-rw-r--   0 root         (0) root         (0)     1425 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/api_resources/moderation.py
--rw-rw-r--   0 root         (0) root         (0)    11147 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/brainai_object.py
--rw-rw-r--   0 root         (0) root         (0)      870 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/brainai_response.py
--rw-rw-r--   0 root         (0) root         (0)    50559 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/datalib/
--rw-rw-r--   0 root         (0) root         (0)      666 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/datalib/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      277 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/datalib/common.py
--rw-rw-r--   0 root         (0) root         (0)      336 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/datalib/numpy_helper.py
--rw-rw-r--   0 root         (0) root         (0)      345 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/datalib/pandas_helper.py
--rw-rw-r--   0 root         (0) root         (0)     8851 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/embeddings_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4485 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/error.py
--rw-rw-r--   0 root         (0) root         (0)      445 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/object_classes.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.537467 pyBrainai-1.4.0.9/brainai/test/
--rw-rw-r--   0 root         (0) root         (0)      654 2024-03-31 01:12:30.000000 pyBrainai-1.4.0.9/brainai/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10503 2024-03-31 04:23:18.000000 pyBrainai-1.4.0.9/brainai/test/brainos_test.py
--rw-rw-r--   0 root         (0) root         (0)     1881 2024-03-31 01:12:30.000000 pyBrainai-1.4.0.9/brainai/test/models_test.py
--rw-rw-r--   0 root         (0) root         (0)     4176 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/test/other_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/brainai/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/brainai/tests/asyncio/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/asyncio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2464 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/asyncio/test_endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     3691 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_api_requestor.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1209 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1459 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_file_cli.py
--rw-rw-r--   0 root         (0) root         (0)     2073 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_long_examples_validator.py
--rw-rw-r--   0 root         (0) root         (0)     6737 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_url_composition.py
--rw-rw-r--   0 root         (0) root         (0)     1851 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/tests/test_util.py
--rw-rw-r--   0 root         (0) root         (0)     1240 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/upload_progress.py
--rw-rw-r--   0 root         (0) root         (0)     5540 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/util.py
--rw-rw-r--   0 root         (0) root         (0)    35135 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/validators.py
--rw-rw-r--   0 root         (0) root         (0)       17 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/version.py
--rw-rw-r--   0 root         (0) root         (0)    10692 2024-03-30 23:49:47.000000 pyBrainai-1.4.0.9/brainai/wandb_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/pyBrainai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      728 2024-03-31 04:36:12.000000 pyBrainai-1.4.0.9/pyBrainai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2262 2024-03-31 04:36:12.000000 pyBrainai-1.4.0.9/pyBrainai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 04:36:12.000000 pyBrainai-1.4.0.9/pyBrainai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-31 04:36:12.000000 pyBrainai-1.4.0.9/pyBrainai.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      510 2024-03-31 04:35:02.000000 pyBrainai-1.4.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 04:36:12.541467 pyBrainai-1.4.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/
+-rw-rw-r--   0 root         (0) root         (0)     1088 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      223 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/
+-rw-rw-r--   0 root         (0) root         (0)     2989 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2659 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/_openai_scripts.py
+-rw-rw-r--   0 root         (0) root         (0)    27749 2024-04-09 09:56:37.000000 pyBrainai-1.4.1.0/brainai/api_requestor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/
+-rw-rw-r--   0 root         (0) root         (0)     1099 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/abstract/
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5628 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2677 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/createable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     1676 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/deletable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)    10530 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/engine_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2785 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/listable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     5810 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/nested_resource_class_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     3590 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/paginatable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/updateable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     7955 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/audio.py
+-rw-rw-r--   0 root         (0) root         (0)     4182 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/brainos_completion.py
+-rw-rw-r--   0 root         (0) root         (0)     2988 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/chat_completion.py
+-rw-rw-r--   0 root         (0) root         (0)     1668 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/completion.py
+-rw-rw-r--   0 root         (0) root         (0)      560 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/customer.py
+-rw-rw-r--   0 root         (0) root         (0)     4177 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     2025 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/edit.py
+-rw-rw-r--   0 root         (0) root         (0)     3536 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/embedding.py
+-rw-rw-r--   0 root         (0) root         (0)     1718 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/engine.py
+-rw-rw-r--   0 root         (0) root         (0)      925 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/error_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/experimental/
+-rw-rw-r--   0 root         (0) root         (0)      108 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/experimental/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      286 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/experimental/completion_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8728 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/file.py
+-rw-rw-r--   0 root         (0) root         (0)     5480 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/fine_tune.py
+-rw-rw-r--   0 root         (0) root         (0)     2354 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/fine_tuning.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/image.py
+-rw-rw-r--   0 root         (0) root         (0)      175 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/model.py
+-rw-rw-r--   0 root         (0) root         (0)     1425 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/moderation.py
+-rw-rw-r--   0 root         (0) root         (0)    11147 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/brainai_object.py
+-rw-rw-r--   0 root         (0) root         (0)      870 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/brainai_response.py
+-rw-rw-r--   0 root         (0) root         (0)    50559 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/datalib/
+-rw-rw-r--   0 root         (0) root         (0)      666 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/datalib/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      277 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/common.py
+-rw-rw-r--   0 root         (0) root         (0)      336 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/numpy_helper.py
+-rw-rw-r--   0 root         (0) root         (0)      345 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/pandas_helper.py
+-rw-rw-r--   0 root         (0) root         (0)     8851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/embeddings_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4485 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/error.py
+-rw-rw-r--   0 root         (0) root         (0)      445 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/object_classes.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/test/
+-rw-rw-r--   0 root         (0) root         (0)      654 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/test/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12225 2024-04-09 09:47:58.000000 pyBrainai-1.4.1.0/brainai/test/brainos_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2141 2024-04-09 09:41:03.000000 pyBrainai-1.4.1.0/brainai/test/models_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4176 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/test/other_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/tests/asyncio/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/asyncio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2464 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/asyncio/test_endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     3691 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_api_requestor.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1209 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1459 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_file_cli.py
+-rw-rw-r--   0 root         (0) root         (0)     2073 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_long_examples_validator.py
+-rw-rw-r--   0 root         (0) root         (0)     6737 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_url_composition.py
+-rw-rw-r--   0 root         (0) root         (0)     1851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1240 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/upload_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     5540 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/util.py
+-rw-rw-r--   0 root         (0) root         (0)    35135 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/brainai/validators.py
+-rw-rw-r--   0 root         (0) root         (0)       17 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/brainai/version.py
+-rw-rw-r--   0 root         (0) root         (0)    10692 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/wandb_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/pyBrainai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      510 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/setup.cfg
```

### Comparing `pyBrainai-1.4.0.9/LICENSE` & `pyBrainai-1.4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/PKG-INFO` & `pyBrainai-1.4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainai
-Version: 1.4.0.9
+Version: 1.4.1.0
 Summary: Python version of brainai SDK
 Author-email: yaojianqu <game781120@126.com>
 Project-URL: Homepage, https://github.com/yaojianqu/py-brainai-sdk
 Project-URL: Issues, https://github.com/yaojianqu/py-brainai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyBrainai-1.4.0.9/brainai/__init__.py` & `pyBrainai-1.4.1.0/brainai/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/_openai_scripts.py` & `pyBrainai-1.4.1.0/brainai/_openai_scripts.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_requestor.py` & `pyBrainai-1.4.1.0/brainai/api_requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,19 +604,29 @@
                 data=data,
                 files=files,
                 stream=stream,
                 timeout=request_timeout if request_timeout else TIMEOUT_SECS,
                 proxies=_thread_context.session.proxies,
             )
         except requests.exceptions.Timeout as e:
-            raise error.Timeout("Request timed out: {}".format(e)) from e
+            r = requests.Response()
+            r.status_code = 400
+            r.headers["content-type"] = "application/json"
+            r._content = json.dumps({"msg":"Request timed out"}).encode("utf-8")
+            return r
+            #raise error.Timeout("Request timed out: {}".format(e)) from e
         except requests.exceptions.RequestException as e:
-            raise error.APIConnectionError(
-                "Error communicating with brainai: {}".format(e)
-            ) from e
+            r = requests.Response()
+            r.status_code = 400
+            r.headers["content-type"] = "application/json"
+            r._content = json.dumps({"msg":"Error communicating with brainai"}).encode("utf-8")
+            return r
+            #raise error.APIConnectionError(
+            #    "Error communicating with brainai: {}".format(e)
+            #) from e
         util.log_debug(
             "brainai API response",
             path=abs_url,
             response_code=result.status_code,
             processing_ms=result.headers.get("brainai-Processing-Ms"),
             request_id=result.headers.get("X-Request-Id"),
         )
@@ -734,15 +744,15 @@
                     stream=False,
                 ),
                 False,
             )
 
     def _interpret_response_line(
         self, rbody: str, rcode: int, rheaders, stream: bool
-    ) -> brainaiResponse:
+    ) -> brainaiResponse | error.APIError:
         # HTTP 204 response code does not have any content in the body.
         if rcode == 204:
             return brainaiResponse(None, rheaders)
 
         if rcode == 503:
             raise error.ServiceUnavailableError(
                 "The server is overloaded or not ready yet.",
@@ -756,14 +766,23 @@
             else:
                 data = json.loads(rbody)
         except (JSONDecodeError, UnicodeDecodeError) as e:
             raise error.APIError(
                 f"HTTP code {rcode} from API ({rbody})", rbody, rcode, headers=rheaders
             ) from e
         resp = brainaiResponse(data, rheaders)
+        if rcode == 504 or rcode == 400:
+            return error.APIError(
+                    message=None,
+                    http_body=rbody,
+                    http_status=rcode,
+                    json_body=None,
+                    headers=None,
+                    code=None)
+
         # In the future, we might add a "status" parameter to errors
         # to better handle the "error while streaming" case.
         stream_error = stream and "error" in resp.data
         if stream_error or not 200 <= rcode < 300:
             raise self.handle_error_response(
                 rbody, rcode, resp.data, rheaders, stream_error=stream_error
             )
```

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/__init__.py` & `pyBrainai-1.4.1.0/brainai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/__init__.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/createable_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/deletable_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/engine_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/listable_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/nested_resource_class_methods.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/paginatable_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/paginatable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/abstract/updateable_api_resource.py` & `pyBrainai-1.4.1.0/brainai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/audio.py` & `pyBrainai-1.4.1.0/brainai/api_resources/audio.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/brainos_completion.py` & `pyBrainai-1.4.1.0/brainai/api_resources/brainos_completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/chat_completion.py` & `pyBrainai-1.4.1.0/brainai/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/completion.py` & `pyBrainai-1.4.1.0/brainai/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/customer.py` & `pyBrainai-1.4.1.0/brainai/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/deployment.py` & `pyBrainai-1.4.1.0/brainai/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/edit.py` & `pyBrainai-1.4.1.0/brainai/api_resources/edit.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/embedding.py` & `pyBrainai-1.4.1.0/brainai/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/engine.py` & `pyBrainai-1.4.1.0/brainai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/error_object.py` & `pyBrainai-1.4.1.0/brainai/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/file.py` & `pyBrainai-1.4.1.0/brainai/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/fine_tune.py` & `pyBrainai-1.4.1.0/brainai/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/fine_tuning.py` & `pyBrainai-1.4.1.0/brainai/api_resources/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/image.py` & `pyBrainai-1.4.1.0/brainai/api_resources/image.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/api_resources/moderation.py` & `pyBrainai-1.4.1.0/brainai/api_resources/moderation.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/brainai_object.py` & `pyBrainai-1.4.1.0/brainai/brainai_object.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/brainai_response.py` & `pyBrainai-1.4.1.0/brainai/brainai_response.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/cli.py` & `pyBrainai-1.4.1.0/brainai/cli.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/datalib/__init__.py` & `pyBrainai-1.4.1.0/brainai/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/embeddings_utils.py` & `pyBrainai-1.4.1.0/brainai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/error.py` & `pyBrainai-1.4.1.0/brainai/error.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/test/__init__.py` & `pyBrainai-1.4.1.0/brainai/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/test/brainos_test.py` & `pyBrainai-1.4.1.0/brainai/test/brainos_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import time
 from urllib.parse import urlparse, parse_qs
 
 import brainai
 import json
 
-help_api_key = "Ub8cWZ9JzKMzfXOl5783167765Ed4376B1BbA06d0fF10755"
-help_api_base = "http://10.0.36.13:8888/brain"
-app_id = "1765183287868731300"
+# help_api_key = "Ub8cWZ9JzKMzfXOl5783167765Ed4376B1BbA06d0fF10755"
+# help_api_base = "http://10.0.36.13:8888/brain"
+help_api_key = "iFt20LWHsmzSLsM71638Ef67A3694eF893EeD834228aE459"
+help_api_base = "https://brain.thundersoft.com/brain"
+
+app_id = "1777633445126377472"
 user_id = "test-13011033796"
 
-common_parameters ={
-        "api_key": help_api_key,
-        "api_base": help_api_base,
-        "headers": {
-            "appId": app_id,
-            "userId": user_id,
-        }
+common_parameters = {
+    "api_key": help_api_key,
+    "api_base": help_api_base,
+    "headers": {
+        "appId": app_id,
+        "userId": user_id,
+    }
 }
+
+
 def read_files():
-    file_paths = ["D:\\file\\研发经理任职资格体系介绍.docx",]  # 要上传的文件路径列表
+    file_paths = ["D:\\file\\研发经理任职资格体系介绍.docx", ]  # 要上传的文件路径列表
     # 构建 multipart/form-data 请求体
     files = []
     for file_path in file_paths:
         # 获取文件的 MIME 类型
-        #mime_type = "application/octet-stream"
+        # mime_type = "application/octet-stream"
         # 打开文件并读取内容
         with open(file_path, "rb") as file:
             file_data = file.read()
         # 构建文件对象
         files.append(("files", (file_path, file_data)))
     return files
 
@@ -40,58 +45,76 @@
         "description": "这个团队空间只为测试而用......",
         "visible_state": 2,
         "space_users": {
             "287": "0",
         },
     }
     kwargs.update(common_parameters)
-    json_str = json.dumps(kwargs,indent=4,ensure_ascii=False)
+    json_str = json.dumps(kwargs, indent=4, ensure_ascii=False)
     print(f"json={json_str}")
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 获取空间列表
 def knowledge_list():
     kwargs = {
         "object_name": "knowledge.api.knowledge.pub_knowledge_list?app_type=0",
         "filter_type": 4,  # PERSON = 1  #个人  TEAM = 2  #团队  COMPANY = 3  #企业  ALL = 4  #全部
         "keyword": "",
         "search_type": 1,  # 1 个人（我的）空间  2 团队空间  3 企业空间
         "page": 1,
         "size": 20,
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 删除空间
 def delete_knowledge():
     knowledge_id = 1767821415425376258
     kwargs = {
         "object_name": f"knowledge.api.knowledge.pub_delete_knowledge.{knowledge_id}",
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 上传文件
 def upload_files():
     kwargs = {
         "api_key": help_api_key,
         "api_base": help_api_base,
         "object_name": "dandelion.api.v1.file",
         "files": read_files(),
     }
     response = brainai.BrainOsCompletion.uploadFiles(**kwargs)
     data = json.loads(response.text)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 文件学习
 def files_learn():
     kwargs = {
         "object_name": "knowledge.api.file.pub_learning",
         "group_id": "0",
         "knowledge_id": "1764985334501867521",
         "type": 0,
@@ -102,51 +125,74 @@
                 "originUrl": "http://127.0.0.1:9000/dandelion/test/20240305/24d88d2157286e6f8b42df5e43dbf9d3.docx",
                 "customFileType": "NORMAL"
             }
         ]
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 获取文件列表
 def file_list():
     kwargs = {
         "object_name": f"dandelion.api.v1.dataset.files.listByUserId?userId={user_id}",
         "method": "GET",
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
 
+
 # 删除文件列表
 def delete_file_list():
     knowledge_id = 1764985334501867521
     kwargs = {
         "object_name": f"knowledge.api.knowledge.pub_delete_files?knowledge_id={knowledge_id}&action=delete",
         "file_ids": ["1764987438054375426", "1764987438054375427"]
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 添加对话(助手聊天)
 def add_chat():
     kwargs = {
         "object_name": "brain.api-public.v1.chat",
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
+
+
 # 获取对话历史
 def history_chat():
     chat_id = 1765199189163061248
     kwargs = {
         "object_name": f"brain.api-public.v1.history.{chat_id}?pageSize=20&pageNum=0&id=0",
         "method": "GET",
     }
@@ -200,40 +246,51 @@
             res = {
                 "code": -1,
                 "data": "",
                 "message": "'id' parameter error!"
             }
             return json.dumps(res)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
 
+
 # brain下基于模型的对话
 def llm_chat():
     stream = True
     kwargs = {
         "object_name": "brain.api-public.v1.completions",
         "chatId": "",
         "reGenerate": 0,
         "messagesId": 321324354675,
         "message": "中国最好的画家是谁?",
         "ignoreHistory": 0,  # 1是不保存,0是保存
         "stream": stream
     }
     kwargs.update(common_parameters)
     response = brainai.ChatCompletion.create(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     if not stream:
         print(f"response type={response}")
         data = json.loads(response)
-        print(f"{json.dumps(data,indent=4 ,ensure_ascii=False)}")
+        print(f"{json.dumps(data, indent=4, ensure_ascii=False)}")
     else:
         for chunk in response:
             data = json.loads(chunk)
-            print(f"{json.dumps(data,indent=4, ensure_ascii=False)}")
+            print(f"{json.dumps(data, indent=4, ensure_ascii=False)}")
+
+
 # brain下带知识库的对话
 def knowledge_chat():
     chat_id = 1765199189163061248
     knowledge_id = 1764985334501867521
     stream = True
     kwargs = {
         "object_name": "brain.api-public.v1.qa.completions",
@@ -249,48 +306,62 @@
         "messagesId": 0,
         "message": "项目经理的职责是什么？",
         "ignoreHistory": 0,
         "stream": stream
     }
     kwargs.update(common_parameters)
     response = brainai.ChatCompletion.create(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     if not stream:
-        print("----"+response)
-        #data = json.loads(response)
-        #print(f"{json.dumps(data,indent=4 ,ensure_ascii=False)}")
+        print("----" + response)
+        # data = json.loads(response)
+        # print(f"{json.dumps(data,indent=4 ,ensure_ascii=False)}")
     else:
         for chunk in response:
             data = json.loads(chunk)
-            print(f"{json.dumps(data,indent=4, ensure_ascii=False)}")
+            print(f"{json.dumps(data, indent=4, ensure_ascii=False)}")
+
 
 # 删除对话
 def delete_chat():
     chat_id = 1765199189163061248
     kwargs = {
         "object_name": f"brain.api-public.v1.chat.{chat_id}",
         "method": "DELETE",
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
+
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
 
+
 # 获取对话列表
 def chat_list():
     kwargs = {
         "object_name": f"brain.api-public.v1.chat.list",
         "method": "GET",
     }
     kwargs.update(common_parameters)
     response = brainai.BrainOsCompletion.dealRequest(**kwargs)
+    if type(response) == brainai.error.APIError:
+        print(f"{response.http_status},{response.http_body}")
+        return
     data = json.loads(response)
     json_data = json.dumps(data, indent=4, ensure_ascii=False)
     print(json_data)
 
+
 if __name__ == '__main__':
     # 创建知识库
     create_knowledge()
     # # 获取空间列表
     # knowledge_list()
     # # 删除空间
     # delete_knowledge()
@@ -310,10 +381,7 @@
     # llm_chat()
     # # brain下带知识库的对话
     # knowledge_chat()
     # # 删除对话
     # delete_chat()
     # # 获取对话列表
     # #chat_list()
-
-
-
```

### Comparing `pyBrainai-1.4.0.9/brainai/test/other_test.py` & `pyBrainai-1.4.1.0/brainai/test/other_test.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/asyncio/test_endpoints.py` & `pyBrainai-1.4.1.0/brainai/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_api_requestor.py` & `pyBrainai-1.4.1.0/brainai/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_endpoints.py` & `pyBrainai-1.4.1.0/brainai/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_exceptions.py` & `pyBrainai-1.4.1.0/brainai/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_file_cli.py` & `pyBrainai-1.4.1.0/brainai/tests/test_file_cli.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_long_examples_validator.py` & `pyBrainai-1.4.1.0/brainai/tests/test_long_examples_validator.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_url_composition.py` & `pyBrainai-1.4.1.0/brainai/tests/test_url_composition.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/tests/test_util.py` & `pyBrainai-1.4.1.0/brainai/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/upload_progress.py` & `pyBrainai-1.4.1.0/brainai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/util.py` & `pyBrainai-1.4.1.0/brainai/util.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/validators.py` & `pyBrainai-1.4.1.0/brainai/validators.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/brainai/wandb_logger.py` & `pyBrainai-1.4.1.0/brainai/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.0.9/pyBrainai.egg-info/PKG-INFO` & `pyBrainai-1.4.1.0/pyBrainai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainai
-Version: 1.4.0.9
+Version: 1.4.1.0
 Summary: Python version of brainai SDK
 Author-email: yaojianqu <game781120@126.com>
 Project-URL: Homepage, https://github.com/yaojianqu/py-brainai-sdk
 Project-URL: Issues, https://github.com/yaojianqu/py-brainai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyBrainai-1.4.0.9/pyBrainai.egg-info/SOURCES.txt` & `pyBrainai-1.4.1.0/pyBrainai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

