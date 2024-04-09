# Comparing `tmp/lm-debug-eval-ui-0.0.3.tar.gz` & `tmp/lm-debug-eval-ui-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm-debug-eval-ui-0.0.3.tar", last modified: Fri Apr  5 20:59:58 2024, max compression
+gzip compressed data, was "lm-debug-eval-ui-0.0.4.tar", last modified: Mon Apr  8 15:09:08 2024, max compression
```

## Comparing `lm-debug-eval-ui-0.0.3.tar` & `lm-debug-eval-ui-0.0.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.005024 lm-debug-eval-ui-0.0.3/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1060 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/LICENSE
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       53 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/MANIFEST.in
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6129 2024-04-05 20:59:58.004802 lm-debug-eval-ui-0.0.3/PKG-INFO
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5062 2024-04-04 17:34:15.000000 lm-debug-eval-ui-0.0.3/README.md
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      891 2024-04-05 20:57:40.000000 lm-debug-eval-ui-0.0.3/pyproject.toml
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      331 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/requirements.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       38 2024-04-05 20:59:58.005068 lm-debug-eval-ui-0.0.3/setup.cfg
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.986945 lm-debug-eval-ui-0.0.3/src/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.988921 lm-debug-eval-ui-0.0.3/src/aiconfig/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     8949 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/ChatCompletion.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    18471 2024-04-01 20:58:56.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/Config.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1308 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3821 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/callback.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.990900 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11434 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/anyscale_endpoint.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1190 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/azure.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     9750 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/claude.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7928 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/dalle.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    23342 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/gemini.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11552 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/hf.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    27081 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    17343 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/openai_vision.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    15916 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/palm.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5177 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/parameterized_model_parser.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.991280 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.991466 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.986023 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.986078 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.991755 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/python/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3879 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2129 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/python/test.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      760 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/example_aiconfig_model_registry.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.992729 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2721 2024-04-02 21:15:07.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/eval_server_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1389 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/queue_iterator.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    41688 2024-04-05 15:50:20.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1879 2024-03-26 19:51:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server_file_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    16623 2024-04-02 14:03:39.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server_utils.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.993275 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      662 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/asset-manifest.json
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.993420 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/images/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2899 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/images/aiconfigLogo.png
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      590 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/index.html
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      189 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/manifest.json
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       67 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/robots.txt
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.986397 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:57.995877 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1233 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4134 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    12294 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    46289 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2639 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7710 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)  1435888 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2941 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js.LICENSE.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)  6183646 2024-04-05 20:58:54.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js.map
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.000570 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       13 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.000748 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/api/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      540 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/api/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7073 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/common.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14071 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/lib.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14051 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/metrics.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3299 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/eval/openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    10115 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/model_parser.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5125 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/registry.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    39682 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/schema.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.001061 lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11459 2024-04-04 21:31:56.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/aiconfig_cli.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.001294 lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/rage/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7897 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/rage/rage.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1377 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/run_aiconfig.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.001824 lm-debug-eval-ui-0.0.3/src/aiconfig/util/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/util/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2529 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/util/config_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11610 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/src/aiconfig/util/params.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.004483 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6129 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/PKG-INFO
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3043 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/SOURCES.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        1 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/dependency_links.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       64 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/entry_points.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      312 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/requires.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        9 2024-04-05 20:59:57.000000 lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/top_level.txt
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-05 20:59:58.004288 lm-debug-eval-ui-0.0.3/tests/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      614 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_chatcompletion_mock_wrapper.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      902 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_dataclass.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    13053 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_eval.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4423 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_eval_model_graded_openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2428 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_library_helpers.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4567 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_load_config.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14213 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_parameter_api.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    24865 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_programmatically_create_an_AIConfig.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6020 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_registry.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      991 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_resolve.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3759 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.3/tests/test_run_config.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.124696 lm-debug-eval-ui-0.0.4/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1060 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/LICENSE
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       53 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/MANIFEST.in
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-08 15:09:08.124467 lm-debug-eval-ui-0.0.4/PKG-INFO
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5062 2024-04-04 17:34:15.000000 lm-debug-eval-ui-0.0.4/README.md
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      891 2024-04-08 15:08:40.000000 lm-debug-eval-ui-0.0.4/pyproject.toml
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      347 2024-04-08 14:14:57.000000 lm-debug-eval-ui-0.0.4/requirements.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       38 2024-04-08 15:09:08.124745 lm-debug-eval-ui-0.0.4/setup.cfg
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.105235 lm-debug-eval-ui-0.0.4/src/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.108111 lm-debug-eval-ui-0.0.4/src/aiconfig/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     8949 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/ChatCompletion.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    18471 2024-04-01 20:58:56.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/Config.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1308 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3821 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/callback.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.110589 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11434 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/anyscale_endpoint.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1190 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/azure.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     9750 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/claude.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7928 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/dalle.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    23342 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/gemini.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11552 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/hf.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    27081 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    17343 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai_vision.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    15916 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/palm.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5177 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/parameterized_model_parser.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.110911 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.111064 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104186 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104245 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.111555 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3879 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2129 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/test.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      760 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/example_aiconfig_model_registry.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.112681 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2721 2024-04-02 21:15:07.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/eval_server_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1389 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/queue_iterator.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    41688 2024-04-05 15:50:20.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1879 2024-03-26 19:51:54.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_file_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    16623 2024-04-02 14:03:39.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_utils.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.113267 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      662 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/asset-manifest.json
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.113431 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2899 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/aiconfigLogo.png
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      590 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/index.html
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      189 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/manifest.json
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       67 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/robots.txt
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104736 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.116052 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1233 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4134 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    12294 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    46289 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2639 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7710 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)  1436262 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2941 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)  6185212 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120442 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       13 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120572 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      540 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7073 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/common.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14071 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/lib.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14051 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/metrics.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3299 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    10115 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/model_parser.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5125 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/registry.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    39682 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/schema.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120835 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11459 2024-04-04 21:31:56.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/aiconfig_cli.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120951 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7897 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/rage.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1377 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/run_aiconfig.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.121322 lm-debug-eval-ui-0.0.4/src/aiconfig/util/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2529 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/config_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11610 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/params.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.124140 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/PKG-INFO
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3043 2024-04-08 15:09:08.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        1 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       64 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/entry_points.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      327 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/requires.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        9 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/top_level.txt
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.123800 lm-debug-eval-ui-0.0.4/tests/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      614 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_chatcompletion_mock_wrapper.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      902 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_dataclass.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    13053 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_eval.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4423 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_eval_model_graded_openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2428 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_library_helpers.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4567 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_load_config.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14213 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_parameter_api.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    24865 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_programmatically_create_an_AIConfig.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6020 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_registry.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      991 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_resolve.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3759 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_run_config.py
```

### Comparing `lm-debug-eval-ui-0.0.3/LICENSE` & `lm-debug-eval-ui-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/PKG-INFO` & `lm-debug-eval-ui-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-debug-eval-ui
-Version: 0.0.3
+Version: 0.0.4
 Summary: LLM Application Debug/Eval UI on top of AIConfig
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -30,14 +30,15 @@
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: result
 Requires-Dist: ruamel.yaml
+Requires-Dist: peewee==3.17.1
 
 LLM application debugger / evaluation UI built on top of [AIConfig](https://github.com/lastmile-ai/aiconfig)
 
 
 ## Quickstart
 
 1. `pip3 install lm-debug-eval-ui`
```

### Comparing `lm-debug-eval-ui-0.0.3/README.md` & `lm-debug-eval-ui-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/pyproject.toml` & `lm-debug-eval-ui-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lm-debug-eval-ui"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="LastMile AI" },
 ]
 description = "LLM Application Debug/Eval UI on top of AIConfig"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/ChatCompletion.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/ChatCompletion.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/Config.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/Config.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/__init__.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/callback.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/callback.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/anyscale_endpoint.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/anyscale_endpoint.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/azure.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/azure.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/claude.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/claude.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/dalle.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/dalle.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/gemini.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/gemini.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/hf.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/hf.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/openai.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/openai_vision.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai_vision.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/palm.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/palm.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/default_parsers/parameterized_model_parser.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/parameterized_model_parser.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/client/node_modules/flatted/python/test.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/example_aiconfig_model_registry.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/example_aiconfig_model_registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/eval_server_utils.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/eval_server_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/queue_iterator.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/queue_iterator.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server_file_utils.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_file_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/server_utils.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/images/aiconfigLogo.png` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/aiconfigLogo.png`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/index.html` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>AIConfig Editor</title><script defer="defer" src="/static/js/main.02a86820.js"></script></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/logo192.png"/><link rel="manifest" href="/manifest.json"/><title>AIConfig Editor</title><script defer="defer" src="/static/js/main.26b0450c.js"></script></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.02a86820.js.LICENSE.txt */
+/*! For license information please see main.26b0450c.js.LICENSE.txt */
 (() => {
     var e = {
             7600: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => fe
                 });
@@ -69047,15 +69047,15 @@
                     },
                     mantineTableBodyRowProps: e => {
                         let {
                             row: t
                         } = e;
                         return {
                             onClick: () => {
-                                n(t.id)
+                                n(t.original)
                             },
                             sx: {
                                 cursor: "pointer"
                             }
                         }
                     },
                     state: {
@@ -69078,73 +69078,98 @@
                 table: d
             })
         }
         const Xz = 50;
 
         function Jz(e) {
             let {
-                evaluationSetId: t,
+                evaluationSet: t,
                 getEvaluationResults: n,
                 onSelectEvaluationResult: o
             } = e;
-            const [a, i] = (0, r.useState)(!0), [l, s] = (0, r.useState)([]), [c, u] = (0, r.useState)([]), [d, f] = (0, r.useState)(null);
+            const [a, i] = (0, r.useState)(!0), [l, s] = (0, r.useState)([]), [c, u] = (0, r.useState)([]), [d, f] = (0, r.useState)(null), p = t.id, m = t.status;
             (0, r.useEffect)((() => {
-                n(t).then((e => {
+                n(p).then((e => {
                     s(e.results), f(null), u(e.columns)
                 })).catch((e => {
                     f("Failed to get evaluation results: ".concat(e.message))
                 })).finally((() => {
                     i(!1)
                 }))
-            }), [t, n]);
-            const p = (0, r.useMemo)((() => 0 === c.length ? [] : c.map((e => ({
+            }), [p, n]);
+            const g = (0, r.useMemo)((() => 0 === c.length ? [] : c.map((e => ({
                     header: e.name,
                     accessorKey: e.key,
                     size: Xz
                 })))), [c]),
-                m = rz({
-                    columns: p,
-                    data: l,
-                    enableColumnOrdering: !0,
-                    enableRowSelection: !1,
-                    getRowId: e => e.id,
-                    initialState: {
-                        density: "xs"
-                    },
-                    mantineTableBodyRowProps: e => {
-                        let {
-                            row: t
-                        } = e;
-                        return {
-                            onClick: () => {
-                                o(t.id)
-                            },
-                            sx: {
-                                cursor: "pointer"
-                            }
+                h = d ? {
+                    enableColumnOrdering: !1,
+                    enableDensityToggle: !1,
+                    enableFilters: !1,
+                    enableFullScreenToggle: !1,
+                    enableHiding: !1
+                } : {},
+                [v, b] = (0, r.useState)(0);
+            (0, r.useEffect)((() => {
+                if ("running" !== m) return;
+                const e = setInterval((() => {
+                    b((e => {
+                        const t = 20 * Math.random();
+                        return Math.min(e + t, 100)
+                    }))
+                }), 1e3);
+                return () => clearInterval(e)
+            }), [m]);
+            const y = rz({
+                columns: g,
+                data: l,
+                enableColumnOrdering: !0,
+                enableRowSelection: !1,
+                getRowId: e => e.id,
+                initialState: {
+                    density: "xs"
+                },
+                mantineProgressProps: e => {
+                    let {
+                        isTopToolbar: t
+                    } = e;
+                    return {
+                        color: "blue",
+                        value: v,
+                        sx: {
+                            display: t ? "block" : "none"
                         }
-                    },
-                    state: {
-                        isLoading: a && null == d,
-                        showAlertBanner: null != d
-                    },
-                    mantineToolbarAlertBannerProps: d ? {
-                        color: "red",
-                        children: d
-                    } : void 0,
-                    ...d ? {
-                        enableColumnOrdering: !1,
-                        enableDensityToggle: !1,
-                        enableFilters: !1,
-                        enableFullScreenToggle: !1,
-                        enableHiding: !1
-                    } : {}
-                });
+                    }
+                },
+                mantineTableBodyRowProps: e => {
+                    let {
+                        row: t
+                    } = e;
+                    return {
+                        onClick: () => {
+                            o(t.id)
+                        },
+                        sx: {
+                            cursor: "pointer"
+                        }
+                    }
+                },
+                state: {
+                    isLoading: a && null == d,
+                    showAlertBanner: null != d,
+                    showProgressBars: "running" === m && null == d
+                },
+                mantineToolbarAlertBannerProps: d ? {
+                    color: "red",
+                    children: d
+                } : void 0,
+                ...h
+            });
             return (0, hl.jsx)(Zz, {
-                table: m
+                table: y
             })
         }
         const Qz = 50;
 
         function eM(e) {
             let {
                 evaluationResultId: t,
@@ -70343,15 +70368,15 @@
                     getEvaluationResultDetails: l
                 })]
             }) : null != c && (v = (0, hl.jsxs)(hl.Fragment, {
                 children: [(0, hl.jsx)(je.A, {
                     onClick: () => u(null),
                     children: (0, hl.jsx)(BC, {})
                 }), (0, hl.jsx)(Jz, {
-                    evaluationSetId: c,
+                    evaluationSet: c,
                     getEvaluationResults: i,
                     onSelectEvaluationResult: f
                 })]
             })), (0, hl.jsx)(y, {
                 fluid: !0,
                 children: v
             })
@@ -70477,8 +70502,8 @@
             })
         }
         o.createRoot(document.getElementById("root")).render((0, hl.jsx)(r.StrictMode, {
             children: (0, hl.jsx)(UL, {})
         }))
     })()
 })();
-//# sourceMappingURL=main.02a86820.js.map
+//# sourceMappingURL=main.26b0450c.js.map
```

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js.LICENSE.txt` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/editor/server/static/static/js/main.02a86820.js.map` & `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8566963466968013%*

 * *Differences: {"'file'": "'static/js/main.26b0450c.js'",*

 * * "'mappings'": "';uGAAA,SAASA,EAAgBC,EAAKC,EAAKC,GAYjC,OAXID,KAAOD,EACTG,OAAOC,eAAeJ,EAAKC,EAAK,CAC9BC,MAAOA,EACPG,YAAY,EACZC,cAAc,EACdC,UAAU,IAGZP,EAAIC,GAAOC,EAGNF,CACT,CAEA,SAASQ,EAAQC,EAAQC,GACvB,IAAIC,EAAOR,OAAOQ,KAAKF,GAEvB,GAAIN,OAAOS,sBAAuB,CAChC,IAAIC,EAAUV,OAAOS,sBAAsBH,GACvCC,IAAgBG,EAAUA,EAAQC,QAAO,SAAUC,GACrD,OAAOZ,OAAOa,yBAAyBP,EAAQM,GAAKV,UACtD,KACAM,EAAKM,KAAKC,MAAMP,EAAME,EACxB,CAEA,OAAOF,CACT,CAEA,SAASQ,EAAeC,GACtB,IAAK,IAAIC,EAAI,EAAGA,EAAIC,UAAU […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.02a86820.js",
+    "file": "static/js/main.26b0450c.js",
     "names": [
         "_defineProperty",
         "obj",
         "key",
         "value",
         "Object",
         "defineProperty",
@@ -11449,21 +11449,27 @@
         "getEvaluationSets",
         "onSelectEvaluationSet",
         "evaluationSets",
         "setEvaluationSets",
         "sets",
         "SM_COLUMN_SIZE",
         "EvaluationSetAnalysisTable",
-        "evaluationSetId",
+        "evaluationSet",
         "getEvaluationResults",
         "onSelectEvaluationResult",
         "evaluationResults",
         "setEvaluationResults",
         "tableColumns",
         "setTableColumns",
+        "evaluationSetId",
+        "evaluationSetStatus",
+        "globalElementConfig",
+        "setProgress",
+        "oldProgress",
+        "newProgress",
         "EvaluationResultTable",
         "evaluationResultId",
         "getEvaluationResultDetails",
         "evaluationResultDetails",
         "setEvaluationResultDetails",
         "customizations",
         "_cellValue$cell_color",
@@ -13789,16 +13795,16 @@
         "import { Box } from '@mantine/core';\nimport { MRT_TableFooterCell } from './MRT_TableFooterCell';\nimport {\n  type MRT_Header,\n  type MRT_HeaderGroup,\n  type MRT_TableInstance,\n  type MRT_VirtualItem,\n} from '../types';\n\ninterface Props<TData extends Record<string, any> = {}> {\n  footerGroup: MRT_HeaderGroup<TData>;\n  table: MRT_TableInstance<TData>;\n  virtualColumns?: MRT_VirtualItem[];\n  virtualPaddingLeft?: number;\n  virtualPaddingRight?: number;\n}\n\nexport const MRT_TableFooterRow = <TData extends Record<string, any> = {}>({\n  footerGroup,\n  table,\n  virtualColumns,\n  virtualPaddingLeft,\n  virtualPaddingRight,\n}: Props<TData>) => {\n  const {\n    options: { layoutMode, mantineTableFooterRowProps },\n  } = table;\n\n  // if no content in row, skip row\n  if (\n    !footerGroup.headers?.some(\n      (header) =>\n        (typeof header.column.columnDef.footer === 'string' &&\n          !!header.column.columnDef.footer) ||\n        header.column.columnDef.Footer,\n    )\n  )\n    return null;\n\n  const tableRowProps =\n    mantineTableFooterRowProps instanceof Function\n      ? mantineTableFooterRowProps({ footerGroup, table })\n      : mantineTableFooterRowProps;\n\n  return (\n    <Box\n      component=\"tr\"\n      {...tableRowProps}\n      sx={(theme) => ({\n        backgroundColor: theme.fn.lighten(\n          theme.colorScheme === 'dark' ? theme.colors.dark[7] : theme.white,\n          0.06,\n        ),\n        display: layoutMode === 'grid' ? 'flex' : 'table-row',\n        width: '100%',\n        ...(tableRowProps?.sx instanceof Function\n          ? tableRowProps?.sx(theme)\n          : (tableRowProps?.sx as any)),\n      })}\n    >\n      {virtualPaddingLeft ? (\n        <th style={{ display: 'flex', width: virtualPaddingLeft }} />\n      ) : null}\n      {(virtualColumns ?? footerGroup.headers).map((footerOrVirtualFooter) => {\n        const footer = virtualColumns\n          ? footerGroup.headers[footerOrVirtualFooter.index]\n          : (footerOrVirtualFooter as MRT_Header<TData>);\n\n        return (\n          <MRT_TableFooterCell footer={footer} key={footer.id} table={table} />\n        );\n      })}\n      {virtualPaddingRight ? (\n        <th style={{ display: 'flex', width: virtualPaddingRight }} />\n      ) : null}\n    </Box>\n  );\n};\n",
         "import { Box } from '@mantine/core';\nimport { MRT_TableFooterRow } from './MRT_TableFooterRow';\nimport { type MRT_TableInstance, type MRT_VirtualItem } from '../types';\n\ninterface Props<TData extends Record<string, any> = {}> {\n  table: MRT_TableInstance<TData>;\n  virtualColumns?: MRT_VirtualItem[];\n  virtualPaddingLeft?: number;\n  virtualPaddingRight?: number;\n}\n\nexport const MRT_TableFooter = <TData extends Record<string, any> = {}>({\n  table,\n  virtualColumns,\n  virtualPaddingLeft,\n  virtualPaddingRight,\n}: Props<TData>) => {\n  const {\n    getFooterGroups,\n    getState,\n    options: { enableStickyFooter, layoutMode, mantineTableFooterProps },\n  } = table;\n  const { isFullScreen } = getState();\n\n  const tableFooterProps =\n    mantineTableFooterProps instanceof Function\n      ? mantineTableFooterProps({ table })\n      : mantineTableFooterProps;\n\n  const stickFooter =\n    (isFullScreen || enableStickyFooter) && enableStickyFooter !== false;\n\n  return (\n    <Box\n      component=\"tfoot\"\n      {...tableFooterProps}\n      sx={(theme) => ({\n        bottom: stickFooter ? 0 : undefined,\n        display: layoutMode === 'grid' ? 'grid' : 'table-row-group',\n        opacity: stickFooter ? 0.97 : undefined,\n        outline: stickFooter\n          ? theme.colorScheme === 'light'\n            ? `1px solid ${theme.colors.gray[3]}`\n            : `1px solid ${theme.colors.gray[7]}`\n          : undefined,\n        position: stickFooter ? 'sticky' : undefined,\n        zIndex: stickFooter ? 1 : undefined,\n        ...(tableFooterProps?.sx instanceof Function\n          ? tableFooterProps?.sx(theme)\n          : (tableFooterProps?.sx as any)),\n      })}\n    >\n      {getFooterGroups().map((footerGroup) => (\n        <MRT_TableFooterRow\n          footerGroup={footerGroup as any}\n          key={footerGroup.id}\n          table={table}\n          virtualColumns={virtualColumns}\n          virtualPaddingLeft={virtualPaddingLeft}\n          virtualPaddingRight={virtualPaddingRight}\n        />\n      ))}\n    </Box>\n  );\n};\n",
         "import { useCallback, useMemo } from 'react';\nimport {\n  defaultRangeExtractor,\n  type Range,\n  useVirtualizer,\n} from '@tanstack/react-virtual';\nimport { Table } from '@mantine/core';\nimport { MRT_TableHead } from '../head/MRT_TableHead';\nimport { Memo_MRT_TableBody, MRT_TableBody } from '../body/MRT_TableBody';\nimport { MRT_TableFooter } from '../footer/MRT_TableFooter';\nimport { parseCSSVarId } from '../column.utils';\nimport { type MRT_TableInstance, type MRT_Virtualizer } from '../types';\n\ninterface Props<TData extends Record<string, any> = {}> {\n  table: MRT_TableInstance<TData>;\n}\n\nexport const MRT_Table = <TData extends Record<string, any> = {}>({\n  table,\n}: Props<TData>) => {\n  const {\n    getFlatHeaders,\n    getState,\n    options: {\n      columnVirtualizerInstanceRef,\n      columnVirtualizerProps,\n      columns,\n      enableColumnResizing,\n      enableColumnVirtualization,\n      enablePinning,\n      enableTableFooter,\n      enableTableHead,\n      layoutMode,\n      mantineTableProps,\n      memoMode,\n    },\n    refs: { tableContainerRef },\n  } = table;\n  const {\n    columnPinning,\n    columnSizing,\n    columnSizingInfo,\n    columnVisibility,\n    density,\n  } = getState();\n\n  const tableProps =\n    mantineTableProps instanceof Function\n      ? mantineTableProps({ table })\n      : mantineTableProps;\n\n  const vProps =\n    columnVirtualizerProps instanceof Function\n      ? columnVirtualizerProps({ table })\n      : columnVirtualizerProps;\n\n  const columnSizeVars = useMemo(() => {\n    const headers = getFlatHeaders();\n    const colSizes: { [key: string]: number } = {};\n    for (let i = 0; i < headers.length; i++) {\n      const header = headers[i];\n      const colSize = header.getSize();\n      colSizes[`--header-${parseCSSVarId(header.id)}-size`] = colSize;\n      colSizes[`--col-${parseCSSVarId(header.column.id)}-size`] = colSize;\n    }\n    return colSizes;\n  }, [columns, columnSizing, columnSizingInfo, columnVisibility]);\n\n  //get first 16 column widths and average them\n  const averageColumnWidth = useMemo(() => {\n    if (!enableColumnVirtualization) return 0;\n    const columnsWidths =\n      table\n        .getRowModel()\n        .rows[0]?.getCenterVisibleCells()\n        ?.slice(0, 16)\n        ?.map((cell) => cell.column.getSize() * 1.2) ?? [];\n    return columnsWidths.reduce((a, b) => a + b, 0) / columnsWidths.length;\n  }, [table.getRowModel().rows, columnPinning, columnVisibility]);\n\n  const [leftPinnedIndexes, rightPinnedIndexes] = useMemo(\n    () =>\n      enableColumnVirtualization && enablePinning\n        ? [\n            table.getLeftLeafColumns().map((c) => c.getPinnedIndex()),\n            table\n              .getRightLeafColumns()\n              .map(\n                (c) =>\n                  table.getVisibleLeafColumns().length - c.getPinnedIndex() - 1,\n              ),\n          ]\n        : [[], []],\n    [columnPinning, enableColumnVirtualization, enablePinning],\n  );\n\n  const columnVirtualizer:\n    | MRT_Virtualizer<HTMLDivElement, HTMLTableCellElement>\n    | undefined = enableColumnVirtualization\n    ? useVirtualizer({\n        count: table.getVisibleLeafColumns().length,\n        estimateSize: () => averageColumnWidth,\n        getScrollElement: () => tableContainerRef.current,\n        horizontal: true,\n        overscan: 3,\n        rangeExtractor: useCallback(\n          (range: Range) => [\n            ...new Set([\n              ...leftPinnedIndexes,\n              ...defaultRangeExtractor(range),\n              ...rightPinnedIndexes,\n            ]),\n          ],\n          [leftPinnedIndexes, rightPinnedIndexes],\n        ),\n        ...vProps,\n      })\n    : undefined;\n\n  if (columnVirtualizerInstanceRef && columnVirtualizer) {\n    columnVirtualizerInstanceRef.current = columnVirtualizer;\n  }\n\n  const virtualColumns = columnVirtualizer\n    ? columnVirtualizer.getVirtualItems()\n    : undefined;\n\n  let virtualPaddingLeft: number | undefined;\n  let virtualPaddingRight: number | undefined;\n\n  if (columnVirtualizer && virtualColumns?.length) {\n    virtualPaddingLeft = virtualColumns[leftPinnedIndexes.length]?.start ?? 0;\n    virtualPaddingRight =\n      columnVirtualizer.getTotalSize() -\n      (virtualColumns[virtualColumns.length - 1 - rightPinnedIndexes.length]\n        ?.end ?? 0);\n  }\n\n  const props = {\n    columnVirtualizer,\n    enableHover: tableProps?.highlightOnHover,\n    isStriped: tableProps?.striped,\n    table,\n    virtualColumns,\n    virtualPaddingLeft,\n    virtualPaddingRight,\n  };\n\n  return (\n    <Table\n      highlightOnHover\n      horizontalSpacing={density}\n      verticalSpacing={density}\n      {...tableProps}\n      sx={(theme) => ({\n        display: layoutMode === 'grid' ? 'grid' : 'table',\n        tableLayout:\n          layoutMode !== 'grid' && enableColumnResizing ? 'fixed' : undefined,\n        '& tr:first-of-type td': {\n          borderTop: `1px solid ${\n            theme.colors.gray[theme.colorScheme === 'dark' ? 8 : 3]\n          }`,\n        },\n        '& tr:last-of-type td': {\n          borderBottom: `1px solid ${\n            theme.colors.gray[theme.colorScheme === 'dark' ? 8 : 3]\n          }`,\n        },\n        ...(tableProps?.sx instanceof Function\n          ? tableProps.sx(theme)\n          : (tableProps?.sx as any)),\n      })}\n      style={{ ...columnSizeVars, ...tableProps?.style }}\n    >\n      {enableTableHead && <MRT_TableHead {...props} />}\n      {memoMode === 'table-body' || columnSizingInfo.isResizingColumn ? (\n        <Memo_MRT_TableBody {...props} />\n      ) : (\n        <MRT_TableBody {...props} />\n      )}\n      {enableTableFooter && <MRT_TableFooter {...props} />}\n    </Table>\n  );\n};\n",
         "import { Flex, Modal, Stack } from '@mantine/core';\nimport { MRT_EditActionButtons } from '../buttons/MRT_EditActionButtons';\nimport { MRT_EditCellTextInput } from '../inputs/MRT_EditCellTextInput';\nimport { type MRT_Row, type MRT_TableInstance } from '../types';\n\ninterface Props<TData extends Record<string, any> = {}> {\n  open: boolean;\n  table: MRT_TableInstance<TData>;\n}\n\nexport const MRT_EditRowModal = <TData extends Record<string, any> = {}>({\n  open,\n  table,\n}: Props<TData>) => {\n  const {\n    getState,\n    options: {\n      onEditingRowCancel,\n      onCreatingRowCancel,\n      renderEditRowModalContent,\n      renderCreateRowModalContent,\n      mantineCreateRowModalProps,\n      mantineEditRowModalProps,\n    },\n    setEditingRow,\n    setCreatingRow,\n  } = table;\n  const { creatingRow, editingRow } = getState();\n  const row = (creatingRow ?? editingRow) as MRT_Row<TData>;\n\n  const createModalProps =\n    mantineCreateRowModalProps instanceof Function\n      ? mantineCreateRowModalProps({ row, table })\n      : mantineCreateRowModalProps;\n\n  const editModalProps =\n    mantineEditRowModalProps instanceof Function\n      ? mantineEditRowModalProps({ row, table })\n      : mantineEditRowModalProps;\n\n  const modalProps = {\n    ...editModalProps,\n    ...(creatingRow && createModalProps),\n  };\n\n  const internalEditComponents = row\n    .getAllCells()\n    .filter((cell) => cell.column.columnDef.columnDefType === 'data')\n    .map((cell) => (\n      <MRT_EditCellTextInput cell={cell} key={cell.id} table={table} />\n    ));\n\n  const handleCancel = () => {\n    if (creatingRow) {\n      onCreatingRowCancel?.({ row, table });\n      setCreatingRow(null);\n    } else {\n      onEditingRowCancel?.({ row, table });\n      setEditingRow(null);\n    }\n    row._valuesCache = {} as any; //reset values cache\n    modalProps.onClose?.();\n  };\n\n  return (\n    <Modal\n      opened={open}\n      withCloseButton={false}\n      {...modalProps}\n      onClose={handleCancel}\n      key={row.id}\n    >\n      {((creatingRow &&\n        renderCreateRowModalContent?.({\n          row,\n          table,\n          internalEditComponents,\n        })) ||\n        renderEditRowModalContent?.({\n          row,\n          table,\n          internalEditComponents,\n        })) ?? (\n        <>\n          <form onSubmit={(e) => e.preventDefault()}>\n            <Stack\n              sx={{\n                gap: '24px',\n                paddingTop: '16px',\n                width: '100%',\n              }}\n            >\n              {internalEditComponents}\n            </Stack>\n          </form>\n          <Flex sx={{ paddingTop: '24px', justifyContent: 'flex-end' }}>\n            <MRT_EditActionButtons row={row} table={table} variant=\"text\" />\n          </Flex>\n        </>\n      )}\n    </Modal>\n  );\n};\n",
         "import { useEffect, useLayoutEffect, useState } from 'react';\nimport { Box, LoadingOverlay } from '@mantine/core';\nimport { MRT_Table } from './MRT_Table';\nimport { MRT_EditRowModal } from '../modals';\nimport { type MRT_TableInstance } from '../types';\n\nconst useIsomorphicLayoutEffect =\n  typeof window !== 'undefined' ? useLayoutEffect : useEffect;\n\ninterface Props<TData extends Record<string, any> = {}> {\n  table: MRT_TableInstance<TData>;\n}\n\nexport const MRT_TableContainer = <TData extends Record<string, any> = {}>({\n  table,\n}: Props<TData>) => {\n  const {\n    getState,\n    options: {\n      createDisplayMode,\n      editDisplayMode,\n      enableStickyHeader,\n      mantineLoadingOverlayProps,\n      mantineTableContainerProps,\n    },\n    refs: { tableContainerRef, bottomToolbarRef, topToolbarRef },\n  } = table;\n  const {\n    isFullScreen,\n    isLoading,\n    showLoadingOverlay,\n    creatingRow,\n    editingRow,\n  } = getState();\n\n  const [totalToolbarHeight, setTotalToolbarHeight] = useState(0);\n\n  const tableContainerProps =\n    mantineTableContainerProps instanceof Function\n      ? mantineTableContainerProps({ table })\n      : mantineTableContainerProps;\n\n  const loadingOverlayProps =\n    mantineLoadingOverlayProps instanceof Function\n      ? mantineLoadingOverlayProps({ table })\n      : mantineLoadingOverlayProps;\n\n  useIsomorphicLayoutEffect(() => {\n    const topToolbarHeight =\n      typeof document !== 'undefined'\n        ? topToolbarRef.current?.offsetHeight ?? 0\n        : 0;\n\n    const bottomToolbarHeight =\n      typeof document !== 'undefined'\n        ? bottomToolbarRef?.current?.offsetHeight ?? 0\n        : 0;\n\n    setTotalToolbarHeight(topToolbarHeight + bottomToolbarHeight);\n  });\n\n  const createModalOpen = createDisplayMode === 'modal' && creatingRow;\n  const editModalOpen = editDisplayMode === 'modal' && editingRow;\n\n  return (\n    <Box\n      {...tableContainerProps}\n      ref={(node: HTMLDivElement) => {\n        if (node) {\n          tableContainerRef.current = node;\n          if (tableContainerProps?.ref) {\n            //@ts-ignore\n            tableContainerProps.ref.current = node;\n          }\n        }\n      }}\n      sx={(theme) => ({\n        maxWidth: '100%',\n        maxHeight: enableStickyHeader\n          ? `clamp(350px, calc(100vh - ${totalToolbarHeight}px), 9999px)`\n          : undefined,\n        overflow: 'auto',\n        position: 'relative',\n        ...(tableContainerProps?.sx instanceof Function\n          ? tableContainerProps.sx(theme)\n          : (tableContainerProps?.sx as any)),\n      })}\n      style={{\n        maxHeight: isFullScreen\n          ? `calc(100vh - ${totalToolbarHeight}px)`\n          : undefined,\n        ...tableContainerProps?.style,\n      }}\n    >\n      <LoadingOverlay\n        visible={isLoading || showLoadingOverlay}\n        {...loadingOverlayProps}\n      />\n      <MRT_Table table={table} />\n      {(createModalOpen || editModalOpen) && (\n        <MRT_EditRowModal open table={table} />\n      )}\n    </Box>\n  );\n};\n",
         "import { Paper } from '@mantine/core';\nimport { MRT_TopToolbar } from '../toolbar/MRT_TopToolbar';\nimport { MRT_BottomToolbar } from '../toolbar/MRT_BottomToolbar';\nimport { MRT_TableContainer } from './MRT_TableContainer';\nimport { type MRT_TableInstance } from '../types';\n\ninterface Props<TData extends Record<string, any> = {}> {\n  table: MRT_TableInstance<TData>;\n}\n\nexport const MRT_TablePaper = <TData extends Record<string, any> = {}>({\n  table,\n}: Props<TData>) => {\n  const {\n    getState,\n    options: {\n      enableBottomToolbar,\n      enableTopToolbar,\n      mantinePaperProps,\n      renderBottomToolbar,\n      renderTopToolbar,\n    },\n    refs: { tablePaperRef },\n  } = table;\n  const { isFullScreen } = getState();\n\n  const tablePaperProps =\n    mantinePaperProps instanceof Function\n      ? mantinePaperProps({ table })\n      : mantinePaperProps;\n\n  return (\n    <Paper\n      shadow=\"xs\"\n      withBorder\n      {...tablePaperProps}\n      ref={(ref: HTMLDivElement) => {\n        tablePaperRef.current = ref;\n        if (tablePaperProps?.ref) {\n          tablePaperProps.ref.current = ref;\n        }\n      }}\n      sx={(theme) => ({\n        overflow: 'hidden',\n        transition: 'all 100ms ease-in-out',\n        ...(tablePaperProps?.sx instanceof Function\n          ? tablePaperProps?.sx(theme)\n          : (tablePaperProps?.sx as any)),\n      })}\n      style={{\n        ...(isFullScreen\n          ? {\n              bottom: 0,\n              height: '100vh',\n              left: 0,\n              margin: 0,\n              maxHeight: '100vh',\n              maxWidth: '100vw',\n              padding: 0,\n              position: 'fixed',\n              right: 0,\n              top: 0,\n              width: '100vw',\n              zIndex: 100,\n            }\n          : {}),\n        ...tablePaperProps?.style,\n      }}\n    >\n      {enableTopToolbar &&\n        (renderTopToolbar instanceof Function\n          ? renderTopToolbar({ table })\n          : renderTopToolbar ?? <MRT_TopToolbar table={table} />)}\n      <MRT_TableContainer table={table} />\n      {enableBottomToolbar &&\n        (renderBottomToolbar instanceof Function\n          ? renderBottomToolbar({ table })\n          : renderBottomToolbar ?? <MRT_BottomToolbar table={table} />)}\n    </Paper>\n  );\n};\n",
         "import { useMantineReactTable } from './useMantineReactTable';\nimport { MRT_TablePaper } from './table/MRT_TablePaper';\nimport {\n  type MRT_TableOptions,\n  type MRT_TableInstance,\n  type Xor,\n} from './types';\n\ntype TableInstanceProp<TData extends Record<string, any> = {}> = {\n  table: MRT_TableInstance<TData>;\n};\n\ntype Props<TData extends Record<string, any> = {}> = Xor<\n  TableInstanceProp<TData>,\n  MRT_TableOptions<TData>\n>;\n\nconst isTableInstanceProp = <TData extends Record<string, any> = {}>(\n  props: Props<TData>,\n): props is TableInstanceProp<TData> =>\n  (props as TableInstanceProp<TData>).table !== undefined;\n\nexport const MantineReactTable = <TData extends Record<string, any> = {}>(\n  props: Props<TData>,\n) => {\n  let table: MRT_TableInstance<TData>;\n\n  if (isTableInstanceProp(props)) {\n    table = props.table;\n  } else {\n    table = useMantineReactTable(props);\n  }\n\n  return <MRT_TablePaper table={table} />;\n};\n",
-        "import { Text } from \"@mantine/core\";\nimport {\n  MRT_Cell,\n  MRT_ColumnDef,\n  MantineReactTable,\n  useMantineReactTable,\n} from \"mantine-react-table\";\nimport { useEffect, useMemo, useState } from \"react\";\nimport { EvaluationSet, EvaluationSetDetails } from \"./types\";\n\ntype Props = {\n  getEvaluationSets: (search?: string) => Promise<EvaluationSet[]>;\n  onSelectEvaluationSet: (evaluationSetId: string) => void;\n};\n\nexport default function EvaluationSetsTable({\n  getEvaluationSets,\n  onSelectEvaluationSet,\n}: Props) {\n  const [isLoading, setIsLoading] = useState(true);\n  const [evaluationSets, setEvaluationSets] = useState<EvaluationSet[]>([]);\n  const [error, setError] = useState<string | null>(null);\n\n  useEffect(() => {\n    getEvaluationSets()\n      .then((sets) => {\n        setEvaluationSets(sets);\n        setError(null);\n      })\n      .catch((error) => {\n        setError(`Failed to get evaluation sets: ${error.message}`);\n      })\n      .finally(() => {\n        setIsLoading(false);\n      });\n  }, [getEvaluationSets]);\n\n  const columns = useMemo<MRT_ColumnDef<EvaluationSet>[]>(\n    () => [\n      { header: \"Set\", accessorKey: \"name\" },\n      {\n        header: \"Created\",\n        accessorKey: \"created\",\n        Cell: ({ cell }) => (\n          <Text>\n            {new Date(cell.getValue<number>() * 1000).toLocaleString()}\n          </Text>\n        ),\n      },\n      { header: \"Status\", accessorKey: \"status\" },\n      {\n        header: \"Details\",\n        accessorKey: \"details\",\n        Cell: ({ cell }: { cell: MRT_Cell<EvaluationSet> }) => (\n          <Text>{JSON.stringify(cell.getValue<EvaluationSetDetails>())}</Text>\n        ),\n      },\n    ],\n    []\n  );\n\n  // If an error is shown, hide the global UI elements so they don't overlap\n  // the error banner\n  const globalElementConfig = error\n    ? {\n        enableColumnOrdering: false, // for show/hide column button\n        enableDensityToggle: false,\n        enableFilters: false,\n        enableFullScreenToggle: false,\n        enableHiding: false, // for show/hide columns button\n      }\n    : {};\n\n  const table = useMantineReactTable({\n    columns,\n    data: evaluationSets,\n    enableColumnOrdering: true,\n    enableRowSelection: false,\n    getRowId: (row) => row.id,\n    initialState: {\n      density: \"xs\",\n    },\n    mantineTableBodyRowProps: ({ row }) => ({\n      onClick: () => {\n        onSelectEvaluationSet(row.id);\n      },\n      sx: {\n        cursor: \"pointer\",\n      },\n    }),\n    state: {\n      isLoading: isLoading && error == null,\n      showAlertBanner: error != null,\n    },\n    mantineToolbarAlertBannerProps: error\n      ? { color: \"red\", children: error }\n      : undefined,\n    ...globalElementConfig,\n  });\n\n  return <MantineReactTable table={table} />;\n}\n",
-        "import { useEffect, useMemo, useState } from \"react\";\nimport {\n  MRT_ColumnDef,\n  MantineReactTable,\n  useMantineReactTable,\n} from \"mantine-react-table\";\nimport { EvaluationResult, TableColumn } from \"./types\";\n\ntype Props = {\n  evaluationSetId: string;\n  getEvaluationResults: (\n    evaluationSetId: string\n  ) => Promise<{ columns: TableColumn[]; results: EvaluationResult[] }>;\n  onSelectEvaluationResult: (evaluationResultId: string) => void;\n};\n\nconst SM_COLUMN_SIZE = 50;\n\nexport default function EvaluationSetAnalysisTable({\n  evaluationSetId,\n  getEvaluationResults,\n  onSelectEvaluationResult,\n}: Props) {\n  const [isLoading, setIsLoading] = useState(true);\n  const [evaluationResults, setEvaluationResults] = useState<\n    EvaluationResult[]\n  >([]);\n  const [tableColumns, setTableColumns] = useState<TableColumn[]>([]);\n  const [error, setError] = useState<string | null>(null);\n\n  useEffect(() => {\n    getEvaluationResults(evaluationSetId)\n      .then((res) => {\n        setEvaluationResults(res.results);\n        setError(null);\n        setTableColumns(res.columns);\n      })\n      .catch((error) => {\n        setError(`Failed to get evaluation results: ${error.message}`);\n      })\n      .finally(() => {\n        setIsLoading(false);\n      });\n  }, [evaluationSetId, getEvaluationResults]);\n\n  const columns = useMemo<MRT_ColumnDef<EvaluationResult>[]>(() => {\n    if (tableColumns.length === 0) {\n      return [];\n    } else {\n      return tableColumns.map((col) => ({\n        header: col.name,\n        accessorKey: col.key,\n        size: SM_COLUMN_SIZE,\n      }));\n    }\n  }, [tableColumns]);\n\n  // If an error is shown, hide the global UI elements so they don't overlap\n  // the error banner\n  const globalElementConfig = error\n    ? {\n        enableColumnOrdering: false, // for show/hide column button\n        enableDensityToggle: false,\n        enableFilters: false,\n        enableFullScreenToggle: false,\n        enableHiding: false, // for show/hide columns button\n      }\n    : {};\n\n  const table = useMantineReactTable({\n    columns,\n    data: evaluationResults,\n    enableColumnOrdering: true,\n    enableRowSelection: false,\n    getRowId: (row) => row.id,\n    initialState: {\n      density: \"xs\",\n    },\n    mantineTableBodyRowProps: ({ row }) => ({\n      onClick: () => {\n        onSelectEvaluationResult(row.id);\n      },\n      sx: {\n        cursor: \"pointer\",\n      },\n    }),\n    state: {\n      isLoading: isLoading && error == null,\n      showAlertBanner: error != null,\n    },\n    mantineToolbarAlertBannerProps: error\n      ? { color: \"red\", children: error }\n      : undefined,\n    ...globalElementConfig,\n  });\n\n  // TODO: Show a general overview of the selected evaluation set\n\n  return <MantineReactTable table={table} />;\n}\n",
+        "import { Text } from \"@mantine/core\";\nimport {\n  MRT_Cell,\n  MRT_ColumnDef,\n  MantineReactTable,\n  useMantineReactTable,\n} from \"mantine-react-table\";\nimport { useEffect, useMemo, useState } from \"react\";\nimport { EvaluationSet, EvaluationSetDetails } from \"./types\";\n\ntype Props = {\n  getEvaluationSets: (search?: string) => Promise<EvaluationSet[]>;\n  onSelectEvaluationSet: (evaluationSet: EvaluationSet) => void;\n};\n\nexport default function EvaluationSetsTable({\n  getEvaluationSets,\n  onSelectEvaluationSet,\n}: Props) {\n  const [isLoading, setIsLoading] = useState(true);\n  const [evaluationSets, setEvaluationSets] = useState<EvaluationSet[]>([]);\n  const [error, setError] = useState<string | null>(null);\n\n  useEffect(() => {\n    getEvaluationSets()\n      .then((sets) => {\n        setEvaluationSets(sets);\n        setError(null);\n      })\n      .catch((error) => {\n        setError(`Failed to get evaluation sets: ${error.message}`);\n      })\n      .finally(() => {\n        setIsLoading(false);\n      });\n  }, [getEvaluationSets]);\n\n  const columns = useMemo<MRT_ColumnDef<EvaluationSet>[]>(\n    () => [\n      { header: \"Set\", accessorKey: \"name\" },\n      {\n        header: \"Created\",\n        accessorKey: \"created\",\n        Cell: ({ cell }) => (\n          <Text>\n            {new Date(cell.getValue<number>() * 1000).toLocaleString()}\n          </Text>\n        ),\n      },\n      { header: \"Status\", accessorKey: \"status\" },\n      {\n        header: \"Details\",\n        accessorKey: \"details\",\n        Cell: ({ cell }: { cell: MRT_Cell<EvaluationSet> }) => (\n          <Text>{JSON.stringify(cell.getValue<EvaluationSetDetails>())}</Text>\n        ),\n      },\n    ],\n    []\n  );\n\n  // If an error is shown, hide the global UI elements so they don't overlap\n  // the error banner\n  const globalElementConfig = error\n    ? {\n        enableColumnOrdering: false, // for show/hide column button\n        enableDensityToggle: false,\n        enableFilters: false,\n        enableFullScreenToggle: false,\n        enableHiding: false, // for show/hide columns button\n      }\n    : {};\n\n  const table = useMantineReactTable({\n    columns,\n    data: evaluationSets,\n    enableColumnOrdering: true,\n    enableRowSelection: false,\n    getRowId: (row) => row.id,\n    initialState: {\n      density: \"xs\",\n    },\n    mantineTableBodyRowProps: ({ row }) => ({\n      onClick: () => {\n        onSelectEvaluationSet(row.original);\n      },\n      sx: {\n        cursor: \"pointer\",\n      },\n    }),\n    state: {\n      isLoading: isLoading && error == null,\n      showAlertBanner: error != null,\n    },\n    mantineToolbarAlertBannerProps: error\n      ? { color: \"red\", children: error }\n      : undefined,\n    ...globalElementConfig,\n  });\n\n  return <MantineReactTable table={table} />;\n}\n",
+        "import { useEffect, useMemo, useState } from \"react\";\nimport {\n  MRT_ColumnDef,\n  MantineReactTable,\n  useMantineReactTable,\n} from \"mantine-react-table\";\nimport { EvaluationResult, EvaluationSet, TableColumn } from \"./types\";\n\ntype Props = {\n  evaluationSet: EvaluationSet;\n  getEvaluationResults: (\n    evaluationSetId: string\n  ) => Promise<{ columns: TableColumn[]; results: EvaluationResult[] }>;\n  onSelectEvaluationResult: (evaluationResultId: string) => void;\n};\n\nconst SM_COLUMN_SIZE = 50;\n\nexport default function EvaluationSetAnalysisTable({\n  evaluationSet,\n  getEvaluationResults,\n  onSelectEvaluationResult,\n}: Props) {\n  const [isLoading, setIsLoading] = useState(true);\n  const [evaluationResults, setEvaluationResults] = useState<\n    EvaluationResult[]\n  >([]);\n  const [tableColumns, setTableColumns] = useState<TableColumn[]>([]);\n  const [error, setError] = useState<string | null>(null);\n  const evaluationSetId = evaluationSet.id;\n  const evaluationSetStatus = evaluationSet.status;\n\n  useEffect(() => {\n    getEvaluationResults(evaluationSetId)\n      .then((res) => {\n        setEvaluationResults(res.results);\n        setError(null);\n        setTableColumns(res.columns);\n      })\n      .catch((error) => {\n        setError(`Failed to get evaluation results: ${error.message}`);\n      })\n      .finally(() => {\n        setIsLoading(false);\n      });\n  }, [evaluationSetId, getEvaluationResults]);\n\n  const columns = useMemo<MRT_ColumnDef<EvaluationResult>[]>(() => {\n    if (tableColumns.length === 0) {\n      return [];\n    } else {\n      return tableColumns.map((col) => ({\n        header: col.name,\n        accessorKey: col.key,\n        size: SM_COLUMN_SIZE,\n      }));\n    }\n  }, [tableColumns]);\n\n  // If an error is shown, hide the global UI elements so they don't overlap\n  // the error banner\n  const globalElementConfig = error\n    ? {\n        enableColumnOrdering: false, // for show/hide column button\n        enableDensityToggle: false,\n        enableFilters: false,\n        enableFullScreenToggle: false,\n        enableHiding: false, // for show/hide columns button\n      }\n    : {};\n\n  const [progress, setProgress] = useState(0);\n\n  // random progress bar if viewing the evaluation set while still in progress\n  useEffect(() => {\n    if (evaluationSetStatus !== \"running\") {\n      return;\n    }\n    const interval = setInterval(() => {\n      setProgress((oldProgress) => {\n        const newProgress = Math.random() * 20;\n        return Math.min(oldProgress + newProgress, 100);\n      });\n    }, 1000);\n    return () => clearInterval(interval);\n  }, [evaluationSetStatus]);\n\n  const table = useMantineReactTable({\n    columns,\n    data: evaluationResults,\n    enableColumnOrdering: true,\n    enableRowSelection: false,\n    getRowId: (row) => row.id,\n    initialState: {\n      density: \"xs\",\n    },\n    mantineProgressProps: ({ isTopToolbar }) => ({\n      color: \"blue\",\n      value: progress, //value between 0 and 100\n      sx: {\n        display: isTopToolbar ? \"block\" : \"none\", //hide bottom progress bar\n      },\n    }),\n    mantineTableBodyRowProps: ({ row }) => ({\n      onClick: () => {\n        onSelectEvaluationResult(row.id);\n      },\n      sx: {\n        cursor: \"pointer\",\n      },\n    }),\n    state: {\n      isLoading: isLoading && error == null,\n      showAlertBanner: error != null,\n      showProgressBars: evaluationSetStatus === \"running\" && error == null,\n    },\n    mantineToolbarAlertBannerProps: error\n      ? { color: \"red\", children: error }\n      : undefined,\n    ...globalElementConfig,\n  });\n\n  // TODO: Show a general overview of the selected evaluation set\n\n  return <MantineReactTable table={table} />;\n}\n",
         "import { useEffect, useMemo, useState } from \"react\";\nimport { Text } from \"@mantine/core\";\nimport {\n  MRT_Cell,\n  MRT_ColumnDef,\n  MantineReactTable,\n  useMantineReactTable,\n} from \"mantine-react-table\";\nimport { EvaluationResultDetails, TableColumn } from \"./types\";\n\ntype Props = {\n  evaluationResultId: string;\n  getEvaluationResultDetails: (\n    evaluationResultId: string\n  ) => Promise<{ columns: TableColumn[]; details: EvaluationResultDetails[] }>;\n};\n\nconst SM_COLUMN_SIZE = 50;\n\nexport default function EvaluationResultTable({\n  evaluationResultId,\n  getEvaluationResultDetails,\n}: Props) {\n  const [isLoading, setIsLoading] = useState(true);\n  const [evaluationResultDetails, setEvaluationResultDetails] = useState<\n    EvaluationResultDetails[]\n  >([]);\n  const [tableColumns, setTableColumns] = useState<TableColumn[]>([]);\n  const [error, setError] = useState<string | null>(null);\n\n  useEffect(() => {\n    getEvaluationResultDetails(evaluationResultId)\n      .then((res) => {\n        setEvaluationResultDetails(res.details);\n        setError(null);\n        setTableColumns(res.columns);\n      })\n      .catch((error) => {\n        setError(`Failed to get evaluation result details: ${error.message}`);\n      })\n      .finally(() => {\n        setIsLoading(false);\n      });\n  }, [evaluationResultId, getEvaluationResultDetails]);\n\n  const columns = useMemo<MRT_ColumnDef<EvaluationResultDetails>[]>(() => {\n    if (tableColumns.length === 0) {\n      return [];\n    } else {\n      return tableColumns.map((col) => ({\n        header: col.name,\n        accessorKey: col.key,\n        size: SM_COLUMN_SIZE,\n        Cell: col.customizations\n          ? ({ cell }: { cell: MRT_Cell<EvaluationResultDetails> }) => {\n              const cellValue = cell.getValue<{\n                value?: string | number | null;\n                cell_color?: string | null;\n              }>();\n\n              const backgroundColor = cellValue?.cell_color ?? undefined;\n              return (\n                <div\n                  style={{\n                    backgroundColor,\n                    minHeight: backgroundColor ? \"1rem\" : undefined,\n                  }}\n                >\n                  <Text bg={backgroundColor}>\n                    {cell.getValue<{ value?: string | number | null }>()\n                      ?.value ?? \"\"}\n                  </Text>\n                </div>\n              );\n            }\n          : undefined,\n      }));\n    }\n  }, [tableColumns]);\n\n  // If an error is shown, hide the global UI elements so they don't overlap\n  // the error banner\n  const globalElementConfig = error\n    ? {\n        enableColumnOrdering: false, // for show/hide column button\n        enableDensityToggle: false,\n        enableFilters: false,\n        enableFullScreenToggle: false,\n        enableHiding: false, // for show/hide columns button\n      }\n    : {};\n\n  const table = useMantineReactTable({\n    columns,\n    data: evaluationResultDetails,\n    enableColumnOrdering: true,\n    enableColumnResizing: true,\n    enablePagination: false,\n    enableRowSelection: false,\n    initialState: {\n      density: \"md\",\n    },\n    state: {\n      isLoading: isLoading && error == null,\n      showAlertBanner: error != null,\n    },\n    mantineTableBodyCellProps: {\n      sx: {\n        borderRight: \"0.0625rem solid #373A40 !important\",\n      },\n    },\n    mantineToolbarAlertBannerProps: error\n      ? { color: \"red\", children: error }\n      : undefined,\n    ...globalElementConfig,\n  });\n\n  // TODO: Show a general overview of the selected evaluation set\n\n  return <MantineReactTable table={table} />;\n}\n",
         "import {\n  createStyles,\n  MantineColor,\n  MantineNumberSize,\n  getStylesRef,\n  rem,\n  getSize,\n} from '@mantine/styles';\n\nexport interface StepStylesParams {\n  color: MantineColor;\n  iconSize: number;\n  radius: MantineNumberSize;\n  allowStepClick: boolean;\n  iconPosition: 'right' | 'left';\n  orientation: 'vertical' | 'horizontal';\n}\n\nexport const iconSizes = {\n  xs: rem(34),\n  sm: rem(36),\n  md: rem(42),\n  lg: rem(48),\n  xl: rem(52),\n};\n\nexport default createStyles(\n  (\n    theme,\n    { color, iconSize, radius, allowStepClick, iconPosition, orientation }: StepStylesParams,\n    { size }\n  ) => {\n    const _iconSize = iconSize ? rem(iconSize) : getSize({ size, sizes: iconSizes });\n    const iconMargin = size === 'xl' || size === 'lg' ? theme.spacing.md : theme.spacing.sm;\n    const _radius = theme.fn.radius(radius);\n    const colors = theme.fn.variant({\n      variant: 'filled',\n      color: color || theme.primaryColor,\n      primaryFallback: false,\n    });\n    const separatorDistanceFromIcon = `calc(${theme.spacing.xs} / 2)`;\n\n    const verticalOrientationStyles = {\n      step: {\n        justifyContent: 'flex-start',\n        minHeight: `calc(${_iconSize} + ${theme.spacing.xl} + ${separatorDistanceFromIcon})`,\n        marginTop: separatorDistanceFromIcon,\n        overflow: 'hidden',\n        '&:first-of-type': {\n          marginTop: 0,\n        },\n        [`&:last-of-type .${getStylesRef('verticalSeparator')}`]: {\n          display: 'none',\n        },\n      },\n    } as const;\n\n    return {\n      stepLoader: {},\n\n      step: {\n        display: 'flex',\n        flexDirection: iconPosition === 'left' ? 'row' : 'row-reverse',\n        cursor: allowStepClick ? 'pointer' : 'default',\n        ...(orientation === 'vertical'\n          ? verticalOrientationStyles.step\n          : {\n              alignItems: 'center',\n            }),\n      },\n\n      stepWrapper: {\n        position: 'relative',\n      },\n\n      verticalSeparator: {\n        top: `calc(${_iconSize} + ${separatorDistanceFromIcon})`,\n        left: `calc(${_iconSize} / 2)`,\n        height: '100vh',\n        position: 'absolute',\n        borderLeft: `${rem(2)} solid ${\n          theme.colorScheme === 'dark' ? theme.colors.dark[5] : theme.colors.gray[1]\n        }`,\n        ref: getStylesRef('verticalSeparator'),\n      },\n\n      verticalSeparatorActive: {\n        borderColor: theme.fn.variant({ variant: 'filled', color }).background,\n      },\n\n      stepIcon: {\n        boxSizing: 'border-box',\n        height: _iconSize,\n        width: _iconSize,\n        minWidth: _iconSize,\n        borderRadius: _radius,\n        display: 'flex',\n        alignItems: 'center',\n        justifyContent: 'center',\n        backgroundColor: theme.colorScheme === 'dark' ? theme.colors.dark[5] : theme.colors.gray[1],\n        border: `${rem(2)} solid ${\n          theme.colorScheme === 'dark' ? theme.colors.dark[5] : theme.colors.gray[1]\n        }`,\n        transition: 'background-color 150ms ease, border-color 150ms ease',\n        position: 'relative',\n        fontWeight: 700,\n        color: theme.colorScheme === 'dark' ? theme.colors.dark[1] : theme.colors.gray[7],\n        fontSize: getSize({ size, sizes: theme.fontSizes }),\n\n        '&[data-progress]': {\n          borderColor: colors.background,\n        },\n\n        '&[data-completed]': {\n          backgroundColor: colors.background,\n          borderColor: colors.background,\n          color: theme.white,\n        },\n      },\n\n      stepCompletedIcon: {\n        ...theme.fn.cover(),\n        display: 'flex',\n        alignItems: 'center',\n        justifyContent: 'center',\n        color: theme.white,\n      },\n\n      stepBody: {\n        display: 'flex',\n        flexDirection: 'column',\n        marginLeft: iconPosition === 'left' ? iconMargin : undefined,\n        marginRight: iconPosition === 'right' ? iconMargin : undefined,\n        ...(orientation === 'vertical' ? { marginTop: `calc(${iconSize} / 4)` } : null),\n      },\n\n      stepLabel: {\n        textAlign: iconPosition,\n        fontWeight: 500,\n        fontSize: getSize({ size, sizes: theme.fontSizes }),\n        lineHeight: 1,\n      },\n\n      stepDescription: {\n        textAlign: iconPosition,\n        marginTop: `calc(${getSize({ size, sizes: theme.spacing })} / 3)`,\n        marginBottom: `calc(${getSize({ size, sizes: theme.spacing })} / 3)`,\n        fontSize: `calc(${getSize({ size, sizes: theme.fontSizes })} - ${rem(2)})`,\n        lineHeight: 1,\n      },\n    };\n  }\n);\n",
         "import React, { forwardRef, FunctionComponent } from 'react';\nimport {\n  DefaultProps,\n  MantineColor,\n  Selectors,\n  MantineSize,\n  MantineNumberSize,\n  useComponentDefaultProps,\n  getSize,\n} from '@mantine/styles';\nimport { Text } from '../../Text';\nimport { Loader } from '../../Loader';\nimport { CheckboxIcon } from '../../Checkbox';\nimport { UnstyledButton } from '../../UnstyledButton';\nimport { Transition } from '../../Transition';\nimport useStyles from './Step.styles';\n\nexport type StepStylesNames = Selectors<typeof useStyles>;\n\nexport type StepFragmentComponent = FunctionComponent<{ step: number }>;\n\nexport interface StepProps\n  extends DefaultProps<StepStylesNames>,\n    React.ComponentPropsWithoutRef<'button'> {\n  variant?: string;\n\n  /** Step index, controlled by Steps component **/\n  step?: number;\n\n  /** Step state, controlled by Steps component */\n  state?: 'stepInactive' | 'stepProgress' | 'stepCompleted';\n\n  /** Step color from theme.colors */\n  color?: MantineColor;\n\n  /** Should icon be displayed */\n  withIcon?: boolean;\n\n  /** Step icon, defaults to step index + 1 when rendered within Stepper */\n  icon?: React.ReactNode | StepFragmentComponent;\n\n  /** Step icon displayed when step is completed */\n  completedIcon?: React.ReactNode | StepFragmentComponent;\n\n  /** Step icon displayed when step is in progress */\n  progressIcon?: React.ReactNode | StepFragmentComponent;\n\n  /** Step label, render after icon */\n  label?: React.ReactNode | StepFragmentComponent;\n\n  /** Step description */\n  description?: React.ReactNode | StepFragmentComponent;\n\n  /** Icon wrapper size */\n  iconSize?: number;\n\n  /** Icon position relative to step body */\n  iconPosition?: 'right' | 'left';\n\n  /** Component size */\n  size?: MantineSize;\n\n  /** Key of theme.radius or any valid CSS value to set border-radius, \"xl\" by default */\n  radius?: MantineNumberSize;\n\n  /** Indicates loading state on step */\n  loading?: boolean;\n\n  /** Set to false to disable clicks on step */\n  allowStepClick?: boolean;\n\n  /** Should step selection be allowed */\n  allowStepSelect?: boolean;\n\n  /** Static selector base */\n  __staticSelector?: string;\n\n  /** Component orientation */\n  orientation?: 'vertical' | 'horizontal';\n}\n\nconst defaultIconSizes = {\n  xs: 16,\n  sm: 18,\n  md: 20,\n  lg: 22,\n  xl: 24,\n};\n\nconst defaultProps: Partial<StepProps> = {\n  withIcon: true,\n  size: 'md',\n  radius: 'xl',\n  allowStepClick: true,\n  iconPosition: 'left',\n  __staticSelector: 'Step',\n};\n\nconst getStepFragment = (Fragment: StepFragmentComponent | React.ReactNode, step: number) => {\n  if (typeof Fragment === 'function') {\n    return <Fragment step={step} />;\n  }\n\n  return Fragment;\n};\n\nexport const Step = forwardRef<HTMLButtonElement, StepProps>((props: StepProps, ref) => {\n  const {\n    className,\n    step,\n    state,\n    color,\n    icon,\n    completedIcon,\n    progressIcon,\n    label,\n    description,\n    withIcon,\n    iconSize,\n    size,\n    radius,\n    loading,\n    allowStepClick,\n    allowStepSelect,\n    iconPosition,\n    __staticSelector,\n    classNames,\n    styles,\n    unstyled,\n    orientation,\n    variant,\n    ...others\n  } = useComponentDefaultProps('StepperStep', defaultProps, props);\n\n  const { classes, cx } = useStyles(\n    { color, iconSize, radius, allowStepClick, iconPosition, orientation },\n    { name: __staticSelector, classNames, styles, unstyled, variant, size }\n  );\n\n  const _iconSize = getSize({ size, sizes: defaultIconSizes });\n  const _icon = state === 'stepCompleted' ? null : state === 'stepProgress' ? progressIcon : icon;\n  const dataAttributes = {\n    'data-progress': state === 'stepProgress' || undefined,\n    'data-completed': state === 'stepCompleted' || undefined,\n  };\n\n  return (\n    <UnstyledButton\n      className={cx(classes.step, className)}\n      tabIndex={allowStepClick ? 0 : -1}\n      ref={ref}\n      {...dataAttributes}\n      {...others}\n    >\n      {withIcon && (\n        <div className={classes.stepWrapper}>\n          <div className={classes.stepIcon} {...dataAttributes}>\n            <Transition mounted={state === 'stepCompleted'} transition=\"pop\" duration={200}>\n              {(transitionStyles) => (\n                <div className={classes.stepCompletedIcon} style={transitionStyles}>\n                  {loading ? (\n                    <Loader color=\"#fff\" size={_iconSize} className={classes.stepLoader} />\n                  ) : (\n                    getStepFragment(completedIcon, step) || (\n                      <CheckboxIcon indeterminate={false} width={_iconSize} height={_iconSize} />\n                    )\n                  )}\n                </div>\n              )}\n            </Transition>\n\n            {state !== 'stepCompleted' ? (\n              loading ? (\n                <Loader size={_iconSize} color={color} />\n              ) : (\n                getStepFragment(_icon || icon, step)\n              )\n            ) : null}\n          </div>\n          {orientation === 'vertical' && (\n            <div\n              className={cx(classes.verticalSeparator, {\n                [classes.verticalSeparatorActive]: state === 'stepCompleted',\n              })}\n            />\n          )}\n        </div>\n      )}\n\n      {(label || description) && (\n        <div className={classes.stepBody}>\n          {label && <Text className={classes.stepLabel}>{getStepFragment(label, step)}</Text>}\n          {description && (\n            <Text className={classes.stepDescription} color=\"dimmed\">\n              {getStepFragment(description, step)}\n            </Text>\n          )}\n        </div>\n      )}\n    </UnstyledButton>\n  );\n});\n\nStep.displayName = '@mantine/core/Step';\n",
         "/* eslint-disable react/no-unused-prop-types */\nimport React from 'react';\n\nexport interface StepCompletedProps {\n  /** Label content */\n  children: React.ReactNode;\n}\n\nexport function StepCompleted(\n  // Props should be kept for ts integration\n  // eslint-disable-next-line @typescript-eslint/no-unused-vars\n  props: StepCompletedProps\n) {\n  return null;\n}\n\nStepCompleted.displayName = '@mantine/core/StepCompleted';\n",
         "import {\n  createStyles,\n  MantineNumberSize,\n  MantineColor,\n  rem,\n  getBreakpointValue,\n  getSize,\n  em,\n} from '@mantine/styles';\nimport { iconSizes } from './Step/Step.styles';\n\nexport interface StepperStylesParams {\n  contentPadding: MantineNumberSize;\n  iconSize?: number;\n  color: MantineColor;\n  orientation: 'vertical' | 'horizontal';\n  iconPosition: 'right' | 'left';\n  breakpoint: MantineNumberSize;\n}\n\nexport default createStyles(\n  (\n    theme,\n    { contentPadding, color, orientation, iconPosition, iconSize, breakpoint }: StepperStylesParams,\n    { size }\n  ) => {\n    const shouldBeResponsive = typeof breakpoint !== 'undefined';\n    const breakpointValue = getBreakpointValue(\n      getSize({ size: breakpoint, sizes: theme.breakpoints })\n    );\n    const separatorOffset =\n      typeof iconSize !== 'undefined'\n        ? `calc(${rem(iconSize)} / 2 - ${rem(1)})`\n        : `calc(${getSize({ size, sizes: iconSizes })} / 2 - ${rem(1)})`;\n\n    const verticalOrientationStyles = {\n      steps: {\n        flexDirection: 'column',\n        alignItems: iconPosition === 'left' ? 'flex-start' : 'flex-end',\n      },\n\n      separator: {\n        width: rem(2),\n        minHeight: theme.spacing.xl,\n        marginLeft: iconPosition === 'left' ? separatorOffset : 0,\n        marginRight: iconPosition === 'right' ? separatorOffset : 0,\n        marginTop: `calc(${theme.spacing.xs} / 2)`,\n        marginBottom: `calc(${theme.spacing.xs} - ${rem(2)})`,\n      },\n    } as const;\n\n    const responsiveStyles = {\n      steps: {\n        [`@media (max-width: ${em(breakpointValue - 1)})`]: verticalOrientationStyles.steps,\n      },\n\n      separator: {\n        [`@media (max-width: ${em(breakpointValue - 1)})`]: verticalOrientationStyles.separator,\n      },\n    } as const;\n\n    return {\n      root: {},\n\n      steps: {\n        display: 'flex',\n        boxSizing: 'border-box',\n        alignItems: 'center',\n        ...(orientation === 'vertical' ? verticalOrientationStyles.steps : null),\n        ...(shouldBeResponsive ? responsiveStyles.steps : null),\n      },\n\n      separator: {\n        boxSizing: 'border-box',\n        transition: 'background-color 150ms ease',\n        flex: 1,\n        height: rem(2),\n        backgroundColor: theme.colorScheme === 'dark' ? theme.colors.dark[4] : theme.colors.gray[2],\n        marginLeft: theme.spacing.md,\n        marginRight: theme.spacing.md,\n        ...(orientation === 'vertical' ? verticalOrientationStyles.separator : null),\n        ...(shouldBeResponsive ? responsiveStyles.separator : null),\n      },\n\n      separatorActive: {\n        backgroundColor: theme.fn.variant({\n          variant: 'filled',\n          color: color || theme.primaryColor,\n          primaryFallback: false,\n        }).background,\n      },\n\n      content: {\n        ...theme.fn.fontStyles(),\n        paddingTop: getSize({ size: contentPadding, sizes: theme.spacing }),\n      },\n    };\n  }\n);\n",
         "import React, { forwardRef, Children, cloneElement } from 'react';\nimport {\n  MantineColor,\n  DefaultProps,\n  MantineNumberSize,\n  MantineSize,\n  Selectors,\n  useComponentDefaultProps,\n} from '@mantine/styles';\nimport { ForwardRefWithStaticComponents } from '@mantine/utils';\nimport { Box } from '../Box';\nimport { Step, StepStylesNames, StepFragmentComponent } from './Step/Step';\nimport { StepCompleted } from './StepCompleted/StepCompleted';\nimport useStyles from './Stepper.styles';\n\nexport type StepperStylesNames = Selectors<typeof useStyles> | StepStylesNames;\n\nexport interface StepperProps\n  extends DefaultProps<StepperStylesNames>,\n    React.ComponentPropsWithRef<'div'> {\n  variant?: string;\n\n  /** <Stepper.Step /> components only */\n  children: React.ReactNode;\n\n  /** Called when step is clicked */\n  onStepClick?(stepIndex: number): void;\n\n  /** Active step index */\n  active: number;\n\n  /** Step icon, defaults to step index + 1 when rendered within Stepper */\n  icon?: React.ReactNode | StepFragmentComponent;\n\n  /** Step icon displayed when step is completed */\n  completedIcon?: React.ReactNode | StepFragmentComponent;\n\n  /** Step icon displayed when step is in progress */\n  progressIcon?: React.ReactNode | StepFragmentComponent;\n\n  /** Active and progress Step colors from theme.colors */\n  color?: MantineColor;\n\n  /** Step icon size */\n  iconSize?: number;\n\n  /** Key of theme.spacing or any valid CSS value to set content padding-top */\n  contentPadding?: MantineNumberSize;\n\n  /** Component orientation */\n  orientation?: 'vertical' | 'horizontal';\n\n  /** Icon position relative to step body */\n  iconPosition?: 'right' | 'left';\n\n  /** Component size */\n  size?: MantineSize;\n\n  /** Key of theme.radius or any valid CSS value to set border-radius, \"xl\" by default */\n  radius?: MantineNumberSize;\n\n  /** Breakpoint at which orientation will change from horizontal to vertical */\n  breakpoint?: MantineNumberSize;\n\n  /** Whether to enable click on upcoming steps by default. Defaults to true **/\n  allowNextStepsSelect?: boolean;\n}\n\ntype StepperComponent = ForwardRefWithStaticComponents<\n  StepperProps,\n  {\n    Step: typeof Step;\n    Completed: typeof StepCompleted;\n  }\n>;\n\nconst defaultProps: Partial<StepperProps> = {\n  contentPadding: 'md',\n  size: 'md',\n  radius: 'xl',\n  orientation: 'horizontal',\n  iconPosition: 'left',\n  allowNextStepsSelect: true,\n};\n\nexport const Stepper: StepperComponent = forwardRef<HTMLDivElement, StepperProps>((props, ref) => {\n  const {\n    className,\n    children,\n    onStepClick,\n    active,\n    icon,\n    completedIcon,\n    progressIcon,\n    color,\n    iconSize,\n    contentPadding,\n    size,\n    radius,\n    orientation,\n    breakpoint,\n    iconPosition,\n    allowNextStepsSelect,\n    classNames,\n    styles,\n    unstyled,\n    variant,\n    ...others\n  } = useComponentDefaultProps('Stepper', defaultProps, props);\n\n  const { classes, cx } = useStyles(\n    { contentPadding, color, orientation, iconPosition, iconSize, breakpoint },\n    { name: 'Stepper', classNames, styles, unstyled, variant, size }\n  );\n\n  const convertedChildren = Children.toArray(children) as React.ReactElement[];\n  const _children = convertedChildren.filter((child) => child.type !== StepCompleted);\n  const completedStep = convertedChildren.find((item) => item.type === StepCompleted);\n\n  const items = _children.reduce<React.ReactElement[]>((acc, item, index) => {\n    const state =\n      active === index ? 'stepProgress' : active > index ? 'stepCompleted' : 'stepInactive';\n\n    const shouldAllowSelect = () => {\n      if (typeof onStepClick !== 'function') {\n        return false;\n      }\n\n      if (typeof item.props.allowStepSelect === 'boolean') {\n        return item.props.allowStepSelect;\n      }\n\n      return state === 'stepCompleted' || allowNextStepsSelect;\n    };\n\n    const isStepSelectionEnabled = shouldAllowSelect();\n\n    acc.push(\n      cloneElement(item, {\n        __staticSelector: 'Stepper',\n        icon: item.props.icon || icon || index + 1,\n        key: index,\n        step: index,\n        variant,\n        state,\n        onClick: () => isStepSelectionEnabled && onStepClick(index),\n        allowStepClick: isStepSelectionEnabled,\n        completedIcon: item.props.completedIcon || completedIcon,\n        progressIcon: item.props.progressIcon || progressIcon,\n        color: item.props.color || color,\n        iconSize,\n        size,\n        radius,\n        classNames,\n        styles,\n        iconPosition: item.props.iconPosition || iconPosition,\n        orientation,\n        unstyled,\n      })\n    );\n\n    if (orientation === 'horizontal' && index !== _children.length - 1) {\n      acc.push(\n        <div\n          className={cx(classes.separator, { [classes.separatorActive]: index < active })}\n          key={`separator-${index}`}\n        />\n      );\n    }\n\n    return acc;\n  }, []);\n\n  const stepContent = _children[active]?.props?.children;\n  const completedContent = completedStep?.props?.children;\n  const content = active > _children.length - 1 ? completedContent : stepContent;\n\n  return (\n    <Box className={cx(classes.root, className)} ref={ref} {...others}>\n      <div className={classes.steps}>{items}</div>\n      {content && <div className={classes.content}>{content}</div>}\n    </Box>\n  );\n}) as any;\n\nStepper.Step = Step;\nStepper.Completed = StepCompleted;\nStepper.displayName = '@mantine/core/Stepper';\n",
         "import type { FormErrors } from '../types';\n\nexport function filterErrors(errors: FormErrors): FormErrors {\n  if (errors === null || typeof errors !== 'object') {\n    return {};\n  }\n\n  return Object.keys(errors).reduce<FormErrors>((acc, key) => {\n    const errorValue = errors[key];\n\n    if (errorValue !== undefined && errorValue !== null && errorValue !== false) {\n      acc[key] = errorValue;\n    }\n\n    return acc;\n  }, {});\n}\n",
@@ -13817,13 +13823,13 @@
         "import { useCallback, useRef, useState } from 'react';\nimport isEqual from 'fast-deep-equal';\nimport { getInputOnChange } from './get-input-on-change';\nimport { getPath, insertPath, removePath, reorderPath, setPath } from './paths';\nimport { filterErrors } from './filter-errors';\nimport { shouldValidateOnChange, validateFieldValue, validateValues } from './validate';\nimport { getStatus } from './get-status';\nimport { changeErrorIndices, clearListState, reorderErrors } from './lists';\nimport {\n  _TransformValues,\n  ClearErrors,\n  ClearFieldDirty,\n  ClearFieldError,\n  GetFieldStatus,\n  GetInputProps,\n  GetTransformedValues,\n  InsertListItem,\n  IsValid,\n  OnReset,\n  OnSubmit,\n  RemoveListItem,\n  ReorderListItem,\n  Reset,\n  ResetDirty,\n  SetErrors,\n  SetFieldError,\n  SetFieldValue,\n  SetValues,\n  UseFormInput,\n  UseFormReturnType,\n  Validate,\n  ValidateField,\n} from './types';\n\nexport function useForm<\n  Values = Record<string, unknown>,\n  TransformValues extends _TransformValues<Values> = (values: Values) => Values\n>({\n  initialValues = {} as Values,\n  initialErrors = {},\n  initialDirty = {},\n  initialTouched = {},\n  clearInputErrorOnChange = true,\n  validateInputOnChange = false,\n  validateInputOnBlur = false,\n  transformValues = ((values: Values) => values) as any,\n  validate: rules,\n}: UseFormInput<Values, TransformValues> = {}): UseFormReturnType<Values, TransformValues> {\n  const [touched, setTouched] = useState(initialTouched);\n  const [dirty, setDirty] = useState(initialDirty);\n  const [values, _setValues] = useState(initialValues);\n  const [errors, _setErrors] = useState(filterErrors(initialErrors));\n\n  const valuesSnapshot = useRef<Values>(initialValues);\n  const setValuesSnapshot = (_values: Values) => {\n    valuesSnapshot.current = _values;\n  };\n\n  const resetTouched = useCallback(() => setTouched({}), []);\n  const resetDirty: ResetDirty<Values> = (_values) => {\n    const newSnapshot = _values ? { ...values, ..._values } : values;\n    setValuesSnapshot(newSnapshot);\n    setDirty({});\n  };\n\n  const setErrors: SetErrors = useCallback(\n    (errs) =>\n      _setErrors((current) => filterErrors(typeof errs === 'function' ? errs(current) : errs)),\n    []\n  );\n\n  const clearErrors: ClearErrors = useCallback(() => _setErrors({}), []);\n  const reset: Reset = useCallback(() => {\n    _setValues(initialValues);\n    clearErrors();\n    setValuesSnapshot(initialValues);\n    setDirty({});\n    resetTouched();\n  }, []);\n\n  const setFieldError: SetFieldError<Values> = useCallback(\n    (path, error) => setErrors((current) => ({ ...current, [path]: error })),\n    []\n  );\n\n  const clearFieldError: ClearFieldError = useCallback(\n    (path) =>\n      setErrors((current) => {\n        if (typeof path !== 'string') {\n          return current;\n        }\n\n        const clone = { ...current };\n        delete clone[path];\n        return clone;\n      }),\n    []\n  );\n\n  const clearFieldDirty: ClearFieldDirty = useCallback(\n    (path) =>\n      setDirty((current) => {\n        if (typeof path !== 'string') {\n          return current;\n        }\n\n        const result = clearListState(path, current);\n        delete result[path];\n        return result;\n      }),\n    []\n  );\n\n  const setFieldValue: SetFieldValue<Values> = useCallback((path, value) => {\n    const shouldValidate = shouldValidateOnChange(path, validateInputOnChange);\n    clearFieldDirty(path);\n    setTouched((currentTouched) => ({ ...currentTouched, [path]: true }));\n    _setValues((current) => {\n      const result = setPath(path, value, current);\n\n      if (shouldValidate) {\n        const validationResults = validateFieldValue(path, rules, result);\n        validationResults.hasError\n          ? setFieldError(path, validationResults.error)\n          : clearFieldError(path);\n      }\n\n      return result;\n    });\n\n    !shouldValidate && clearInputErrorOnChange && setFieldError(path, null);\n  }, []);\n\n  const setValues: SetValues<Values> = useCallback((payload) => {\n    _setValues((currentValues) => {\n      const valuesPartial = typeof payload === 'function' ? payload(currentValues) : payload;\n      return { ...currentValues, ...valuesPartial };\n    });\n    clearInputErrorOnChange && clearErrors();\n  }, []);\n\n  const reorderListItem: ReorderListItem<Values> = useCallback((path, payload) => {\n    clearFieldDirty(path);\n    _setValues((current) => reorderPath(path, payload, current));\n    _setErrors((errs) => reorderErrors(path, payload, errs));\n  }, []);\n\n  const removeListItem: RemoveListItem<Values> = useCallback((path, index) => {\n    clearFieldDirty(path);\n    _setValues((current) => removePath(path, index, current));\n    _setErrors((errs) => changeErrorIndices(path, index, errs, -1));\n  }, []);\n\n  const insertListItem: InsertListItem<Values> = useCallback((path, item, index) => {\n    clearFieldDirty(path);\n    _setValues((current) => insertPath(path, item, index, current));\n    _setErrors((errs) => changeErrorIndices(path, index, errs, 1));\n  }, []);\n\n  const validate: Validate = useCallback(() => {\n    const results = validateValues(rules, values);\n    _setErrors(results.errors);\n    return results;\n  }, [values, rules]);\n\n  const validateField: ValidateField<Values> = useCallback(\n    (path) => {\n      const results = validateFieldValue(path, rules, values);\n      results.hasError ? setFieldError(path, results.error) : clearFieldError(path);\n      return results;\n    },\n    [values, rules]\n  );\n\n  const getInputProps: GetInputProps<Values> = (\n    path,\n    { type = 'input', withError = true, withFocus = true } = {}\n  ) => {\n    const onChange = getInputOnChange((value) => setFieldValue(path, value as any));\n    const payload: any = { onChange };\n\n    if (withError) {\n      payload.error = errors[path];\n    }\n\n    if (type === 'checkbox') {\n      payload.checked = getPath(path, values);\n    } else {\n      payload.value = getPath(path, values);\n    }\n\n    if (withFocus) {\n      payload.onFocus = () => setTouched((current) => ({ ...current, [path]: true }));\n      payload.onBlur = () => {\n        if (shouldValidateOnChange(path, validateInputOnBlur)) {\n          const validationResults = validateFieldValue(path, rules, values);\n\n          validationResults.hasError\n            ? setFieldError(path, validationResults.error)\n            : clearFieldError(path);\n        }\n      };\n    }\n\n    return payload;\n  };\n\n  const onSubmit: OnSubmit<Values, TransformValues> =\n    (handleSubmit, handleValidationFailure) => (event) => {\n      event?.preventDefault();\n      const results = validate();\n\n      if (results.hasErrors) {\n        handleValidationFailure?.(results.errors, values, event);\n      } else {\n        handleSubmit?.(transformValues(values) as any, event);\n      }\n    };\n\n  const getTransformedValues: GetTransformedValues<Values, TransformValues> = (input) =>\n    (transformValues as any)(input || values);\n\n  const onReset: OnReset = useCallback((event) => {\n    event.preventDefault();\n    reset();\n  }, []);\n\n  const isDirty: GetFieldStatus<Values> = (path) => {\n    if (path) {\n      const overriddenValue = getPath(path, dirty);\n      if (typeof overriddenValue === 'boolean') {\n        return overriddenValue;\n      }\n\n      const sliceOfValues = getPath(path, values);\n      const sliceOfInitialValues = getPath(path, valuesSnapshot.current);\n      return !isEqual(sliceOfValues, sliceOfInitialValues);\n    }\n\n    const isOverridden = Object.keys(dirty).length > 0;\n    if (isOverridden) {\n      return getStatus(dirty);\n    }\n\n    return !isEqual(values, valuesSnapshot.current);\n  };\n\n  const isTouched: GetFieldStatus<Values> = useCallback(\n    (path) => getStatus(touched, path),\n    [touched]\n  );\n\n  const isValid: IsValid<Values> = useCallback(\n    (path) =>\n      path\n        ? !validateFieldValue(path, rules, values).hasError\n        : !validateValues(rules, values).hasErrors,\n    [values, rules]\n  );\n\n  return {\n    values,\n    errors,\n    setValues,\n    setErrors,\n    setFieldValue,\n    setFieldError,\n    clearFieldError,\n    clearErrors,\n    reset,\n    validate,\n    validateField,\n    reorderListItem,\n    removeListItem,\n    insertListItem,\n    getInputProps,\n    onSubmit,\n    onReset,\n    isDirty,\n    isTouched,\n    setTouched,\n    setDirty,\n    resetTouched,\n    resetDirty,\n    isValid,\n    getTransformedValues,\n  };\n}\n",
         "import { getPath } from './get-path';\nimport { setPath } from './set-path';\nimport { ReorderPayload } from '../types';\n\nexport function reorderPath<T>(path: unknown, { from, to }: ReorderPayload, values: T) {\n  const currentValue = getPath(path, values);\n\n  if (!Array.isArray(currentValue)) {\n    return values;\n  }\n\n  const cloned = [...currentValue];\n  const item = currentValue[from];\n  cloned.splice(from, 1);\n  cloned.splice(to, 0, item);\n\n  return setPath(path, cloned, values);\n}\n",
         "import { getPath } from './get-path';\nimport { setPath } from './set-path';\n\nexport function removePath<T>(path: unknown, index: number, values: T) {\n  const currentValue = getPath(path, values);\n\n  if (!Array.isArray(currentValue)) {\n    return values;\n  }\n\n  return setPath(\n    path,\n    currentValue.filter((_, itemIndex) => itemIndex !== index),\n    values\n  );\n}\n",
         "import { getPath } from './get-path';\nimport { setPath } from './set-path';\n\nexport function insertPath<T>(path: unknown, value: unknown, index: number, values: T) {\n  const currentValue = getPath(path, values);\n\n  if (!Array.isArray(currentValue)) {\n    return values;\n  }\n\n  const cloned = [...currentValue];\n  cloned.splice(typeof index === 'number' ? index : cloned.length, 0, value);\n\n  return setPath(path, cloned, values);\n}\n",
         "export function getInputOnChange<Value>(\n  setValue: (value: Value | ((current: Value) => Value)) => void\n) {\n  return (val: Value | React.ChangeEvent<unknown> | ((current: Value) => Value)) => {\n    if (!val) {\n      setValue(val as Value);\n    } else if (typeof val === 'function') {\n      setValue(val);\n    } else if (typeof val === 'object' && 'nativeEvent' in val) {\n      const { currentTarget } = val;\n      if (currentTarget instanceof HTMLInputElement) {\n        if (currentTarget.type === 'checkbox') {\n          setValue(currentTarget.checked as any);\n        } else {\n          setValue(currentTarget.value as any);\n        }\n      } else if (\n        currentTarget instanceof HTMLTextAreaElement ||\n        currentTarget instanceof HTMLSelectElement\n      ) {\n        setValue(currentTarget.value as any);\n      }\n    } else {\n      setValue(val);\n    }\n  };\n}\n",
         "import {\n  Button,\n  Flex,\n  Group,\n  Loader,\n  Stepper,\n  Text,\n  TextInput,\n} from \"@mantine/core\";\nimport { Suspense, lazy, memo, useEffect, useState } from \"react\";\nimport { useForm } from \"@mantine/form\";\nimport { CreateEvaluationSetParams } from \"../types\";\nimport { showNotification } from \"@mantine/notifications\";\n\n// EvaluationDataSelector is pretty heavy, so load it lazily and show spinner\n// This prevents UI from blocking when pressing \"Create Evaluation Set\" button\nconst EvaluationDataSelector = lazy(() => import(\"./EvaluationDataSelector\"));\n// Do the same for the other components just for good measure\nconst SpecificEvaluationDataConfiguration = lazy(\n  () => import(\"./SpecificEvaluationDataConfiguration\")\n);\nconst GeneralEvaluationDataConfiguration = lazy(\n  () => import(\"./GeneralEvaluationDataConfiguration\")\n);\n\ntype Props = {\n  getAIConfigFilePath: () => Promise<string>;\n  getEvaluationDataSources: (search?: string) => Promise<string[]>;\n  getEvaluationModels: (search?: string) => Promise<string[]>;\n  onCreateEvaluationSet: (params: CreateEvaluationSetParams) => void;\n};\n\nexport type GeneralDataConfiguration = {\n  model: string | null;\n  maxFields: number;\n  deepRun: boolean;\n  successOnly: boolean;\n  groupedBy: string;\n  tokenSize: number;\n  splitter: string;\n};\n\nexport default memo(function EvaluationDataSection({\n  getAIConfigFilePath,\n  getEvaluationDataSources,\n  getEvaluationModels,\n  onCreateEvaluationSet,\n}: Props) {\n  const [evaluationSetName, setEvaluationSetName] = useState<string>(\"\");\n  const [activeStep, setActiveStep] = useState(0);\n  const [selectedDataIds, setSelectedDataIds] = useState<string[]>([]);\n\n  const setStep: React.Dispatch<React.SetStateAction<number>> = (\n    step: number | ((prevState: number) => number)\n  ) => {\n    if (step === 1 || step === 2) {\n      if (selectedDataIds.length === 0) {\n        // need to select data first\n        return;\n      }\n    }\n    setActiveStep(step);\n  };\n\n  const nextStep = () =>\n    setStep((current) => (current < 2 ? current + 1 : current));\n  const prevStep = () =>\n    setStep((current) => (current > 0 ? current - 1 : current));\n\n  const [isLoadingPromptConfigFilePath, setIsLoadingPromptConfigFilePath] =\n    useState(true);\n  const [promptConfigFilePath, setPromptConfigFilePath] = useState<\n    string | null\n  >(null);\n\n  useEffect(() => {\n    getAIConfigFilePath()\n      .then((path) => {\n        setPromptConfigFilePath(path);\n      })\n      .catch((e) => {\n        showNotification({\n          title: \"Error loading prompt config file path\",\n          message: (e as { message?: string }).message,\n          color: \"red\",\n        });\n      })\n      .finally(() => {\n        setIsLoadingPromptConfigFilePath(false);\n      });\n  }, [getAIConfigFilePath]);\n\n  const evaluate = () => {\n    if (!promptConfigFilePath) {\n      return;\n    }\n    onCreateEvaluationSet({\n      evaluationSetName,\n      promptConfigFilePath,\n      dataIds: selectedDataIds.map((id) => ({\n        id,\n        ground_truth: specificDataConfigurations[id] ?? undefined,\n      })),\n      ...generalDataConfigurationForm.values,\n    });\n  };\n\n  const [specificDataConfigurations, setSpecificDataConfigurations] = useState<\n    Record<string, string | null>\n  >({});\n  const onConfigureSpecificData = (id: string, path: string | null) => {\n    setSpecificDataConfigurations((prev) => ({ ...prev, [id]: path }));\n  };\n\n  const generalDataConfigurationForm = useForm<GeneralDataConfiguration>({\n    initialValues: {\n      model: null,\n      maxFields: 0,\n      deepRun: false,\n      successOnly: false,\n      groupedBy: \"section\",\n      tokenSize: 0,\n      splitter: \"token_size\",\n    },\n    validate: {\n      model: (val: string | null) =>\n        val === null ? \"Model is required\" : null,\n    },\n  });\n\n  const isEvaluationDisabled = !(\n    evaluationSetName &&\n    promptConfigFilePath &&\n    generalDataConfigurationForm.isValid()\n  );\n\n  return (\n    <Flex direction=\"column\">\n      <TextInput\n        label=\"Evaluation Set Name\"\n        required\n        value={evaluationSetName}\n        onChange={(e) => setEvaluationSetName(e.currentTarget.value)}\n        mb=\"1em\"\n      />\n      <TextInput\n        label=\"Prompt Config File Path\"\n        value={promptConfigFilePath ?? \"\"}\n        onChange={(e) => setPromptConfigFilePath(e.target.value)}\n        required\n        disabled={isLoadingPromptConfigFilePath}\n        mb=\"1em\"\n      />\n      <Stepper active={activeStep} onStepClick={setStep} breakpoint=\"sm\">\n        <Stepper.Step label=\"Data Selection\">\n          {activeStep === 0 && (\n            <>\n              <Text mb=\"1em\">\n                Select data to include in the evaluation set. Evaluation will\n                run on each data source selected.\n              </Text>\n              <Suspense\n                fallback={\n                  <Flex justify=\"center\">\n                    <Loader />\n                  </Flex>\n                }\n              >\n                <EvaluationDataSelector\n                  getDataIds={getEvaluationDataSources}\n                  selectedDataIds={selectedDataIds}\n                  onSelectIds={setSelectedDataIds}\n                />\n              </Suspense>\n            </>\n          )}\n        </Stepper.Step>\n        <Stepper.Step label=\"Specific Data Configuration\">\n          {activeStep === 1 && (\n            <>\n              <Text mb=\"1em\">\n                Configure how evaluation will be run specifically on each data\n                source.\n              </Text>\n              <Suspense\n                fallback={\n                  <Flex justify=\"center\">\n                    <Loader />\n                  </Flex>\n                }\n              >\n                <SpecificEvaluationDataConfiguration\n                  dataIds={selectedDataIds}\n                  dataConfigurations={specificDataConfigurations}\n                  onConfigureData={onConfigureSpecificData}\n                />\n              </Suspense>\n            </>\n          )}\n        </Stepper.Step>\n        <Stepper.Step label=\"General Data Configuration\">\n          {activeStep === 2 && (\n            <>\n              <Text mb=\"1em\">\n                Configure how evaluation will be run across all data sources.\n              </Text>\n              <Suspense\n                fallback={\n                  <Flex justify=\"center\">\n                    <Loader />\n                  </Flex>\n                }\n              >\n                <GeneralEvaluationDataConfiguration\n                  configurationForm={generalDataConfigurationForm}\n                  getEvaluationModels={getEvaluationModels}\n                />\n              </Suspense>\n            </>\n          )}\n        </Stepper.Step>\n        <Stepper.Completed>\n          Completed, click back button to get to previous step\n        </Stepper.Completed>\n      </Stepper>\n\n      <Group position=\"center\" mt=\"xl\">\n        <Button\n          variant=\"default\"\n          onClick={prevStep}\n          disabled={activeStep === 0}\n        >\n          Back\n        </Button>\n        {activeStep === 2 ? (\n          <Button onClick={evaluate} disabled={isEvaluationDisabled}>\n            Evaluate\n          </Button>\n        ) : (\n          <Button onClick={nextStep} disabled={selectedDataIds.length === 0}>\n            Next step\n          </Button>\n        )}\n      </Group>\n    </Flex>\n  );\n});\n",
         "import { Button, Card, Container, Flex, Text } from \"@mantine/core\";\nimport { useCallback, useState } from \"react\";\nimport EvaluationDataSection from \"./data/EvaluationDataSection\";\nimport { CreateEvaluationSetParams } from \"./types\";\n\ntype Props = {\n  createEvaluationSet: (params: CreateEvaluationSetParams) => Promise<void>;\n  getAIConfigFilePath: () => Promise<string>;\n  getEvaluationDataSources: (search?: string) => Promise<string[]>;\n  getEvaluationModels: (search?: string) => Promise<string[]>;\n};\n\nexport default function EvaluationHeader({\n  createEvaluationSet,\n  getAIConfigFilePath,\n  getEvaluationDataSources,\n  getEvaluationModels,\n}: Props) {\n  const [isCreateEvaluationSetOpen, setIsCreateEvaluationSetOpen] =\n    useState(false);\n  const onCreateEvaluationSet = useCallback(\n    (params: CreateEvaluationSetParams) => {\n      createEvaluationSet(params);\n      setIsCreateEvaluationSetOpen(false);\n    },\n    [createEvaluationSet]\n  );\n\n  return (\n    <Container maw=\"80rem\" pt=\"1em\">\n      <Flex justify=\"space-between\" pt=\"md\" mb=\"xs\">\n        <Text>\n          Create and analyze evaluation sets by running your generation &\n          evaluation steps using the prompts in Prompt Iteration.\n        </Text>\n        <Button\n          onClick={() =>\n            setIsCreateEvaluationSetOpen(!isCreateEvaluationSetOpen)\n          }\n          color={isCreateEvaluationSetOpen ? \"red\" : \"blue\"}\n        >\n          {isCreateEvaluationSetOpen ? \"Cancel\" : \"Create Evaluation Set\"}\n        </Button>\n      </Flex>\n      {isCreateEvaluationSetOpen && (\n        <Card mb=\"2em\">\n          <EvaluationDataSection\n            getAIConfigFilePath={getAIConfigFilePath}\n            getEvaluationDataSources={getEvaluationDataSources}\n            getEvaluationModels={getEvaluationModels}\n            onCreateEvaluationSet={onCreateEvaluationSet}\n          />\n        </Card>\n      )}\n    </Container>\n  );\n}\n",
-        "import { useCallback, useState } from \"react\";\nimport EvaluationSetsTable from \"./EvaluationSetsTable\";\nimport EvaluationSetAnalysisTable from \"./EvaluationSetAnalysisTable\";\nimport { IconChevronLeft } from \"@tabler/icons-react\";\nimport { ActionIcon, Container } from \"@mantine/core\";\nimport {\n  CreateEvaluationSetParams,\n  EvaluationResult,\n  EvaluationResultDetails,\n  EvaluationSet,\n  TableColumn,\n} from \"./types\";\nimport EvaluationResultTable from \"./EvaluationResultTable\";\nimport CreateEvaluationSetHeader from \"./CreateEvaluationSetHeader\";\nimport { showNotification } from \"@mantine/notifications\";\n\ntype Props = {\n  createEvaluationSet: (params: CreateEvaluationSetParams) => Promise<string>;\n  getAIConfigFilePath: () => Promise<string>;\n  getEvaluationDataSources: (search?: string) => Promise<string[]>;\n  getEvaluationModels: (search?: string) => Promise<string[]>;\n  getEvaluationResults: (\n    evaluationSetId: string\n  ) => Promise<{ columns: TableColumn[]; results: EvaluationResult[] }>;\n  getEvaluationResultDetails: (\n    evaluationResultId: string\n  ) => Promise<{ columns: TableColumn[]; details: EvaluationResultDetails[] }>;\n  getEvaluationSets: (search?: string) => Promise<EvaluationSet[]>;\n};\n\nexport default function EvaluationTable({\n  createEvaluationSet,\n  getAIConfigFilePath,\n  getEvaluationDataSources,\n  getEvaluationModels,\n  getEvaluationResults,\n  getEvaluationResultDetails,\n  getEvaluationSets,\n}: Props) {\n  const [selectedEvalSet, setSelectedEvalSet] = useState<string | null>(null);\n  const [selectedEvalResult, setSelectedEvalResult] = useState<string | null>(\n    null\n  );\n\n  // Temporary state to immediately show the newly created evaluation set\n  const [submittedEvaluationSets, setSubmittedEvaluationSets] = useState<\n    EvaluationSet[]\n  >([]);\n\n  const onCreateEvaluationSet = useCallback(\n    async (params: CreateEvaluationSetParams) => {\n      try {\n        const setId = await createEvaluationSet(params);\n        // Add temporary row to the table\n        setSubmittedEvaluationSets((prev) => [\n          ...prev,\n          {\n            id: setId,\n            name: params.evaluationSetName,\n            created: Date.now(),\n            status: \"running\",\n            details: { docs: params.dataIds.map((d) => d.id) },\n          },\n        ]);\n      } catch (e) {\n        showNotification({\n          title: \"Error creating evaluation set\",\n          message: (e as { message?: string }).message,\n          color: \"red\",\n        });\n      }\n    },\n    [createEvaluationSet]\n  );\n\n  const getEvaluationSetsWithSubmitted = useCallback(async () => {\n    const sets = await getEvaluationSets();\n    const setsWithSubmitted = submittedEvaluationSets.reduce((acc, set) => {\n      if (acc.some((s) => s.id === set.id)) {\n        return acc;\n      }\n      return [...acc, set];\n    }, sets);\n    return setsWithSubmitted.sort((a, b) => b.created - a.created);\n  }, [getEvaluationSets, submittedEvaluationSets]);\n\n  let evaluationTable = null;\n  if (selectedEvalSet == null && selectedEvalResult == null) {\n    evaluationTable = (\n      <>\n        <CreateEvaluationSetHeader\n          createEvaluationSet={onCreateEvaluationSet}\n          getAIConfigFilePath={getAIConfigFilePath}\n          getEvaluationDataSources={getEvaluationDataSources}\n          getEvaluationModels={getEvaluationModels}\n        />\n        <EvaluationSetsTable\n          getEvaluationSets={getEvaluationSetsWithSubmitted}\n          onSelectEvaluationSet={setSelectedEvalSet}\n        />\n      </>\n    );\n  } else if (selectedEvalResult != null) {\n    evaluationTable = (\n      <>\n        <ActionIcon onClick={() => setSelectedEvalResult(null)}>\n          <IconChevronLeft />\n        </ActionIcon>\n        <EvaluationResultTable\n          evaluationResultId={selectedEvalResult}\n          getEvaluationResultDetails={getEvaluationResultDetails}\n        />\n      </>\n    );\n  } else if (selectedEvalSet != null) {\n    evaluationTable = (\n      <>\n        <ActionIcon onClick={() => setSelectedEvalSet(null)}>\n          <IconChevronLeft />\n        </ActionIcon>\n        <EvaluationSetAnalysisTable\n          evaluationSetId={selectedEvalSet}\n          getEvaluationResults={getEvaluationResults}\n          onSelectEvaluationResult={setSelectedEvalResult}\n        />\n      </>\n    );\n  }\n\n  return <Container fluid>{evaluationTable}</Container>;\n}\n",
+        "import { useCallback, useState } from \"react\";\nimport EvaluationSetsTable from \"./EvaluationSetsTable\";\nimport EvaluationSetAnalysisTable from \"./EvaluationSetAnalysisTable\";\nimport { IconChevronLeft } from \"@tabler/icons-react\";\nimport { ActionIcon, Container } from \"@mantine/core\";\nimport {\n  CreateEvaluationSetParams,\n  EvaluationResult,\n  EvaluationResultDetails,\n  EvaluationSet,\n  TableColumn,\n} from \"./types\";\nimport EvaluationResultTable from \"./EvaluationResultTable\";\nimport CreateEvaluationSetHeader from \"./CreateEvaluationSetHeader\";\nimport { showNotification } from \"@mantine/notifications\";\n\ntype Props = {\n  createEvaluationSet: (params: CreateEvaluationSetParams) => Promise<string>;\n  getAIConfigFilePath: () => Promise<string>;\n  getEvaluationDataSources: (search?: string) => Promise<string[]>;\n  getEvaluationModels: (search?: string) => Promise<string[]>;\n  getEvaluationResults: (\n    evaluationSetId: string\n  ) => Promise<{ columns: TableColumn[]; results: EvaluationResult[] }>;\n  getEvaluationResultDetails: (\n    evaluationResultId: string\n  ) => Promise<{ columns: TableColumn[]; details: EvaluationResultDetails[] }>;\n  getEvaluationSets: (search?: string) => Promise<EvaluationSet[]>;\n};\n\nexport default function EvaluationTable({\n  createEvaluationSet,\n  getAIConfigFilePath,\n  getEvaluationDataSources,\n  getEvaluationModels,\n  getEvaluationResults,\n  getEvaluationResultDetails,\n  getEvaluationSets,\n}: Props) {\n  const [selectedEvalSet, setSelectedEvalSet] = useState<EvaluationSet | null>(\n    null\n  );\n  const [selectedEvalResult, setSelectedEvalResult] = useState<string | null>(\n    null\n  );\n\n  // Temporary state to immediately show the newly created evaluation set\n  const [submittedEvaluationSets, setSubmittedEvaluationSets] = useState<\n    EvaluationSet[]\n  >([]);\n\n  const onCreateEvaluationSet = useCallback(\n    async (params: CreateEvaluationSetParams) => {\n      try {\n        const setId = await createEvaluationSet(params);\n        // Add temporary row to the table\n        setSubmittedEvaluationSets((prev) => [\n          ...prev,\n          {\n            id: setId,\n            name: params.evaluationSetName,\n            created: Date.now(),\n            status: \"running\",\n            details: { docs: params.dataIds.map((d) => d.id) },\n          },\n        ]);\n      } catch (e) {\n        showNotification({\n          title: \"Error creating evaluation set\",\n          message: (e as { message?: string }).message,\n          color: \"red\",\n        });\n      }\n    },\n    [createEvaluationSet]\n  );\n\n  const getEvaluationSetsWithSubmitted = useCallback(async () => {\n    const sets = await getEvaluationSets();\n    const setsWithSubmitted = submittedEvaluationSets.reduce((acc, set) => {\n      if (acc.some((s) => s.id === set.id)) {\n        return acc;\n      }\n      return [...acc, set];\n    }, sets);\n    return setsWithSubmitted.sort((a, b) => b.created - a.created);\n  }, [getEvaluationSets, submittedEvaluationSets]);\n\n  let evaluationTable = null;\n  if (selectedEvalSet == null && selectedEvalResult == null) {\n    evaluationTable = (\n      <>\n        <CreateEvaluationSetHeader\n          createEvaluationSet={onCreateEvaluationSet}\n          getAIConfigFilePath={getAIConfigFilePath}\n          getEvaluationDataSources={getEvaluationDataSources}\n          getEvaluationModels={getEvaluationModels}\n        />\n        <EvaluationSetsTable\n          getEvaluationSets={getEvaluationSetsWithSubmitted}\n          onSelectEvaluationSet={setSelectedEvalSet}\n        />\n      </>\n    );\n  } else if (selectedEvalResult != null) {\n    evaluationTable = (\n      <>\n        <ActionIcon onClick={() => setSelectedEvalResult(null)}>\n          <IconChevronLeft />\n        </ActionIcon>\n        <EvaluationResultTable\n          evaluationResultId={selectedEvalResult}\n          getEvaluationResultDetails={getEvaluationResultDetails}\n        />\n      </>\n    );\n  } else if (selectedEvalSet != null) {\n    evaluationTable = (\n      <>\n        <ActionIcon onClick={() => setSelectedEvalSet(null)}>\n          <IconChevronLeft />\n        </ActionIcon>\n        <EvaluationSetAnalysisTable\n          evaluationSet={selectedEvalSet}\n          getEvaluationResults={getEvaluationResults}\n          onSelectEvaluationResult={setSelectedEvalResult}\n        />\n      </>\n    );\n  }\n\n  return <Container fluid>{evaluationTable}</Container>;\n}\n",
         "import { Container, createStyles, MantineProvider, Tabs } from \"@mantine/core\";\nimport { LOCAL_THEME } from \"./themes/LocalTheme\";\nimport LocalEditor from \"./LocalEditor\";\nimport { useCallback, useState } from \"react\";\nimport PromptIterationHeader from \"./evaluation/PromptIterationHeader\";\nimport EvaluationTable from \"./evaluation/EvaluationTable\";\nimport { ufetch } from \"ufetch\";\nimport { EVALUATION_ROUTE_TABLE } from \"./utils/api\";\nimport {\n  CreateEvaluationSetParams,\n  EvaluationSet,\n  PromptIterationConfig,\n} from \"./evaluation/types\";\nimport urlJoin from \"url-join\";\nimport { Notifications } from \"@mantine/notifications\";\n\nconst useStyles = createStyles(() => ({\n  editorBackground: {\n    background:\n      \"radial-gradient(ellipse at top,#08122d,#030712),radial-gradient(ellipse at bottom,#030712,#030712)\",\n    margin: \"0 auto\",\n    minHeight: \"100vh\",\n  },\n}));\n\nexport default function AIConfigEvaluation() {\n  const { classes } = useStyles();\n  const [activeTab, setActiveTab] = useState<string | null>(\"evaluation\");\n\n  const createEvaluationSet = useCallback(\n    async (params: CreateEvaluationSetParams) => {\n      // TODO: Once eval params are generalized/schematized, can just spread params through\n      const res = await ufetch.post(\n        EVALUATION_ROUTE_TABLE.CREATE_EVALUATION_SET,\n        {\n          evaluation_set_name: params.evaluationSetName,\n          prompt_config_file_path: params.promptConfigFilePath,\n          data_ids: params.dataIds,\n          model: params.model,\n          max_fields: params.maxFields,\n          deep_run: params.deepRun,\n          success_only: params.successOnly,\n          grouped_by: params.groupedBy,\n          token_size: params.tokenSize,\n          splitter: params.splitter,\n        }\n      );\n      return res.evaluation_set_id;\n    },\n    []\n  );\n\n  const getEvaluationDataSources = useCallback(async (search?: string) => {\n    // For now, rely on caching and handle client-side search filtering\n    const res = await ufetch.get(\n      EVALUATION_ROUTE_TABLE.LIST_EVALUATION_DATA_SOURCES\n    );\n    const dataSources = res.data;\n    if (search && search.length > 0) {\n      const lowerCaseSearch = search.toLowerCase();\n      return dataSources.filter(\n        (source: string) =>\n          source.toLocaleLowerCase().indexOf(lowerCaseSearch) >= 0\n      );\n    }\n    return dataSources;\n  }, []);\n\n  const getEvaluationModels = useCallback(async (search?: string) => {\n    // For now, rely on caching and handle client-side search filtering\n    const res = await ufetch.get(EVALUATION_ROUTE_TABLE.LIST_EVALUATION_MODELS);\n    const models = res.data;\n    if (search && search.length > 0) {\n      const lowerCaseSearch = search.toLowerCase();\n      return models.filter(\n        (model: string) =>\n          model.toLocaleLowerCase().indexOf(lowerCaseSearch) >= 0\n      );\n    }\n    return models;\n  }, []);\n\n  const getEvaluationSets = useCallback(async (search?: string) => {\n    // For now, rely on caching and handle client-side search filtering\n    // TODO: This will need server-side filtering and pagination\n    const res = await ufetch.get(EVALUATION_ROUTE_TABLE.LIST_EVALUATION_SETS);\n    const evalSets = res.data;\n    if (search && search.length > 0) {\n      const lowerCaseSearch = search.toLowerCase();\n      return evalSets.filter(\n        (set: EvaluationSet) =>\n          set.name.toLocaleLowerCase().indexOf(lowerCaseSearch) >= 0\n      );\n    }\n    return evalSets;\n  }, []);\n\n  const getEvaluationResults = useCallback(async (evaluationSetId: string) => {\n    const res = await ufetch.get(\n      urlJoin(\n        EVALUATION_ROUTE_TABLE.LIST_EVALUATION_RESULTS,\n        `?evaluation_set_id=${evaluationSetId}`\n      )\n    );\n    // TODO: Add filtering, etc. Can probably be client-side since one set will\n    // likely not have a huge number of results\n    return {\n      columns: res.columns,\n      results: res.data,\n    };\n  }, []);\n\n  const getEvaluationResultDetails = useCallback(\n    async (evaluationResultId: string) => {\n      const res = await ufetch.get(\n        urlJoin(\n          EVALUATION_ROUTE_TABLE.EVALUATION_RESULT_DETAILS,\n          `?evaluation_result_id=${evaluationResultId}`\n        )\n      );\n      // TODO: Add filtering, etc. Can probably be client-side since one set will\n      // likely not have a huge number of results\n      return {\n        columns: res.columns,\n        details: res.data,\n      };\n    },\n    []\n  );\n\n  const getAIConfigFilePath = useCallback(async () => {\n    try {\n      const res = await ufetch.get(\n        EVALUATION_ROUTE_TABLE.GET_PROMPT_CONFIG_FILE_PATH\n      );\n      return res.file_path;\n    } catch (e) {\n      console.error(`Error obtaining config file path: ${e}`);\n    }\n  }, []);\n\n  const getPromptIterationConfig = useCallback(async () => {\n    const res = await ufetch.get(\n      EVALUATION_ROUTE_TABLE.GET_PROMPT_ITERATION_CONFIG\n    );\n    return res.data;\n  }, []);\n\n  const setPromptIterationConfig = useCallback(\n    async (config: PromptIterationConfig) => {\n      await ufetch.post(\n        EVALUATION_ROUTE_TABLE.SET_PROMPT_ITERATION_CONFIG,\n        config\n      );\n    },\n    []\n  );\n\n  const getPromptIterationDataSources = useCallback(async (search?: string) => {\n    // For now, rely on caching and handle client-side search filtering\n    const res = await ufetch.get(\n      EVALUATION_ROUTE_TABLE.LIST_PROMPT_ITERATION_DATA_SOURCES\n    );\n    const dataSources = res.data;\n    if (search && search.length > 0) {\n      const lowerCaseSearch = search.toLowerCase();\n      return dataSources.filter(\n        (source: string) =>\n          source.toLocaleLowerCase().indexOf(lowerCaseSearch) >= 0\n      );\n    }\n    return dataSources;\n  }, []);\n\n  return (\n    <MantineProvider withGlobalStyles withNormalizeCSS theme={LOCAL_THEME}>\n      <Notifications />\n      <div className={classes.editorBackground}>\n        <Tabs value={activeTab} onTabChange={setActiveTab} py=\"lg\">\n          <Tabs.List pl=\"2rem\" mb=\"lg\">\n            <Tabs.Tab value=\"evaluation\">Evaluation</Tabs.Tab>\n            <Tabs.Tab value=\"promptIteration\">Prompt Iteration</Tabs.Tab>\n          </Tabs.List>\n          <Tabs.Panel value=\"evaluation\">\n            {activeTab === \"evaluation\" && (\n              <Container fluid pb=\"1em\">\n                <EvaluationTable\n                  createEvaluationSet={createEvaluationSet}\n                  getAIConfigFilePath={getAIConfigFilePath}\n                  getEvaluationDataSources={getEvaluationDataSources}\n                  getEvaluationModels={getEvaluationModels}\n                  getEvaluationResults={getEvaluationResults}\n                  getEvaluationResultDetails={getEvaluationResultDetails}\n                  getEvaluationSets={getEvaluationSets}\n                />\n              </Container>\n            )}\n          </Tabs.Panel>\n          <Tabs.Panel value=\"promptIteration\">\n            {activeTab === \"promptIteration\" && (\n              <>\n                <PromptIterationHeader\n                  getDataSources={getPromptIterationDataSources}\n                  getPromptIterationConfig={getPromptIterationConfig}\n                  setPromptIterationConfig={setPromptIterationConfig}\n                />\n                <LocalEditor />\n              </>\n            )}\n          </Tabs.Panel>\n        </Tabs>\n      </div>\n    </MantineProvider>\n  );\n}\n",
         "import React from \"react\";\nimport ReactDOM from \"react-dom/client\";\nimport AIConfigEvaluation from \"./AIConfigEvaluation\";\n\nconst root = ReactDOM.createRoot(\n  document.getElementById(\"root\") as HTMLElement\n);\nroot.render(\n  <React.StrictMode>\n    <AIConfigEvaluation />\n  </React.StrictMode>\n);\n"
     ],
     "version": 3
 }
```

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/eval/api/__init__.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/eval/common.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/common.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/eval/lib.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/lib.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/eval/metrics.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/eval/openai.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/model_parser.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/model_parser.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/registry.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/schema.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/schema.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/aiconfig_cli.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/aiconfig_cli.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/rage/rage.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/rage.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/scripts/run_aiconfig.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/run_aiconfig.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/util/config_utils.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/aiconfig/util/params.py` & `lm-debug-eval-ui-0.0.4/src/aiconfig/util/params.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/PKG-INFO` & `lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-debug-eval-ui
-Version: 0.0.3
+Version: 0.0.4
 Summary: LLM Application Debug/Eval UI on top of AIConfig
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -30,14 +30,15 @@
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 Requires-Dist: python-dotenv
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: result
 Requires-Dist: ruamel.yaml
+Requires-Dist: peewee==3.17.1
 
 LLM application debugger / evaluation UI built on top of [AIConfig](https://github.com/lastmile-ai/aiconfig)
 
 
 ## Quickstart
 
 1. `pip3 install lm-debug-eval-ui`
```

### Comparing `lm-debug-eval-ui-0.0.3/src/lm_debug_eval_ui.egg-info/SOURCES.txt` & `lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
 src/aiconfig/editor/server/static/images/aiconfigLogo.png
 src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js
 src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map
 src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js
 src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map
 src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js
 src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map
-src/aiconfig/editor/server/static/static/js/main.02a86820.js
-src/aiconfig/editor/server/static/static/js/main.02a86820.js.LICENSE.txt
-src/aiconfig/editor/server/static/static/js/main.02a86820.js.map
+src/aiconfig/editor/server/static/static/js/main.26b0450c.js
+src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt
+src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map
 src/aiconfig/eval/__init__.py
 src/aiconfig/eval/common.py
 src/aiconfig/eval/lib.py
 src/aiconfig/eval/metrics.py
 src/aiconfig/eval/openai.py
 src/aiconfig/eval/api/__init__.py
 src/aiconfig/scripts/aiconfig_cli.py
```

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_chatcompletion_mock_wrapper.py` & `lm-debug-eval-ui-0.0.4/tests/test_chatcompletion_mock_wrapper.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_dataclass.py` & `lm-debug-eval-ui-0.0.4/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_eval.py` & `lm-debug-eval-ui-0.0.4/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_eval_model_graded_openai.py` & `lm-debug-eval-ui-0.0.4/tests/test_eval_model_graded_openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_library_helpers.py` & `lm-debug-eval-ui-0.0.4/tests/test_library_helpers.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_load_config.py` & `lm-debug-eval-ui-0.0.4/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_parameter_api.py` & `lm-debug-eval-ui-0.0.4/tests/test_parameter_api.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_programmatically_create_an_AIConfig.py` & `lm-debug-eval-ui-0.0.4/tests/test_programmatically_create_an_AIConfig.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_registry.py` & `lm-debug-eval-ui-0.0.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_resolve.py` & `lm-debug-eval-ui-0.0.4/tests/test_resolve.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.3/tests/test_run_config.py` & `lm-debug-eval-ui-0.0.4/tests/test_run_config.py`

 * *Files identical despite different names*
