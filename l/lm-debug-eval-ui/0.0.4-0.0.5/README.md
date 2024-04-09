# Comparing `tmp/lm-debug-eval-ui-0.0.4.tar.gz` & `tmp/lm-debug-eval-ui-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm-debug-eval-ui-0.0.4.tar", last modified: Mon Apr  8 15:09:08 2024, max compression
+gzip compressed data, was "lm-debug-eval-ui-0.0.5.tar", last modified: Tue Apr  9 14:52:00 2024, max compression
```

## Comparing `lm-debug-eval-ui-0.0.4.tar` & `lm-debug-eval-ui-0.0.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.124696 lm-debug-eval-ui-0.0.4/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1060 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/LICENSE
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       53 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/MANIFEST.in
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-08 15:09:08.124467 lm-debug-eval-ui-0.0.4/PKG-INFO
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5062 2024-04-04 17:34:15.000000 lm-debug-eval-ui-0.0.4/README.md
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      891 2024-04-08 15:08:40.000000 lm-debug-eval-ui-0.0.4/pyproject.toml
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      347 2024-04-08 14:14:57.000000 lm-debug-eval-ui-0.0.4/requirements.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       38 2024-04-08 15:09:08.124745 lm-debug-eval-ui-0.0.4/setup.cfg
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.105235 lm-debug-eval-ui-0.0.4/src/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.108111 lm-debug-eval-ui-0.0.4/src/aiconfig/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     8949 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/ChatCompletion.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    18471 2024-04-01 20:58:56.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/Config.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1308 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3821 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/callback.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.110589 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11434 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/anyscale_endpoint.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1190 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/azure.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     9750 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/claude.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7928 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/dalle.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    23342 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/gemini.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11552 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/hf.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    27081 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    17343 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai_vision.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    15916 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/palm.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5177 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/parameterized_model_parser.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.110911 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.111064 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104186 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104245 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.111555 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3879 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2129 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/test.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      760 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/example_aiconfig_model_registry.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.112681 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2721 2024-04-02 21:15:07.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/eval_server_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1389 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/queue_iterator.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    41688 2024-04-05 15:50:20.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1879 2024-03-26 19:51:54.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_file_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    16623 2024-04-02 14:03:39.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_utils.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.113267 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      662 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/asset-manifest.json
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.113431 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2899 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/aiconfigLogo.png
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      590 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/index.html
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      189 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/manifest.json
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       67 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/robots.txt
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.104736 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.116052 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1233 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4134 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    12294 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    46289 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2639 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7710 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map
--rw-r--r--   0 ryanholinshead   (501) staff       (20)  1436262 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2941 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)  6185212 2024-04-08 15:08:33.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120442 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       13 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/__init__.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120572 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      540 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7073 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/common.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14071 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/lib.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14051 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/metrics.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3299 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/eval/openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    10115 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/model_parser.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     5125 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/registry.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    39682 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/schema.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120835 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11459 2024-04-04 21:31:56.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/aiconfig_cli.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.120951 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     7897 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/rage.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     1377 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/run_aiconfig.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.121322 lm-debug-eval-ui-0.0.4/src/aiconfig/util/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/__init__.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2529 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/config_utils.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    11610 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/src/aiconfig/util/params.py
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.124140 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/PKG-INFO
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3043 2024-04-08 15:09:08.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/SOURCES.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        1 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/dependency_links.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)       64 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/entry_points.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      327 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/requires.txt
--rw-r--r--   0 ryanholinshead   (501) staff       (20)        9 2024-04-08 15:09:07.000000 lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/top_level.txt
-drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-08 15:09:08.123800 lm-debug-eval-ui-0.0.4/tests/
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      614 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_chatcompletion_mock_wrapper.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      902 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_dataclass.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    13053 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_eval.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4423 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_eval_model_graded_openai.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     2428 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_library_helpers.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     4567 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_load_config.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    14213 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_parameter_api.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)    24865 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_programmatically_create_an_AIConfig.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     6020 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_registry.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)      991 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_resolve.py
--rw-r--r--   0 ryanholinshead   (501) staff       (20)     3759 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.4/tests/test_run_config.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.293084 lm-debug-eval-ui-0.0.5/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1060 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/LICENSE
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       53 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/MANIFEST.in
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-09 14:52:00.292777 lm-debug-eval-ui-0.0.5/PKG-INFO
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5062 2024-04-04 17:34:15.000000 lm-debug-eval-ui-0.0.5/README.md
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      891 2024-04-09 14:51:31.000000 lm-debug-eval-ui-0.0.5/pyproject.toml
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      347 2024-04-08 14:14:57.000000 lm-debug-eval-ui-0.0.5/requirements.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       38 2024-04-09 14:52:00.293142 lm-debug-eval-ui-0.0.5/setup.cfg
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.273490 lm-debug-eval-ui-0.0.5/src/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.276743 lm-debug-eval-ui-0.0.5/src/aiconfig/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     8949 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/ChatCompletion.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    18471 2024-04-01 20:58:56.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/Config.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1308 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3821 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/callback.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.278976 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11434 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/anyscale_endpoint.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1190 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/azure.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     9750 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/claude.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7928 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/dalle.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    23342 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/gemini.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11552 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/hf.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    27081 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    17343 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/openai_vision.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    15916 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/palm.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5177 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/parameterized_model_parser.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.279225 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.279439 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.272458 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.272520 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.280099 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/python/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3879 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2129 2024-01-10 20:05:37.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/python/test.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      760 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/example_aiconfig_model_registry.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.280990 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2721 2024-04-02 21:15:07.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/eval_server_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1389 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/queue_iterator.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    41714 2024-04-09 14:24:51.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1879 2024-03-26 19:51:54.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server_file_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    16623 2024-04-02 14:03:39.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server_utils.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.281581 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      662 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/asset-manifest.json
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.281709 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/images/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2899 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/images/aiconfigLogo.png
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      590 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/index.html
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      189 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/manifest.json
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       67 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/robots.txt
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.272936 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.283880 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1233 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4134 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    12294 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    46289 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2639 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7710 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)  1436262 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2941 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)  6185212 2024-04-09 14:51:19.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.288718 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       13 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/__init__.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.288879 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/api/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      540 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/api/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7073 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/common.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14071 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/lib.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14051 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/metrics.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3299 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/eval/openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    10115 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/model_parser.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     5125 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/registry.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    39682 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/schema.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.289198 lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11459 2024-04-04 21:31:56.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/aiconfig_cli.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.289355 lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/rage/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     7897 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/rage/rage.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     1377 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/run_aiconfig.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.289775 lm-debug-eval-ui-0.0.5/src/aiconfig/util/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        0 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/util/__init__.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2529 2024-03-14 13:26:51.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/util/config_utils.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    11610 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/src/aiconfig/util/params.py
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.292476 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6159 2024-04-09 14:51:59.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/PKG-INFO
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3043 2024-04-09 14:52:00.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        1 2024-04-09 14:51:59.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)       64 2024-04-09 14:51:59.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/entry_points.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      327 2024-04-09 14:51:59.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/requires.txt
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)        9 2024-04-09 14:51:59.000000 lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/top_level.txt
+drwxr-xr-x   0 ryanholinshead   (501) staff       (20)        0 2024-04-09 14:52:00.292269 lm-debug-eval-ui-0.0.5/tests/
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      614 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_chatcompletion_mock_wrapper.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      902 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_dataclass.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    13053 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_eval.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4423 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_eval_model_graded_openai.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     2428 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_library_helpers.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     4567 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_load_config.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    14213 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_parameter_api.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)    24865 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_programmatically_create_an_AIConfig.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     6020 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_registry.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)      991 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_resolve.py
+-rw-r--r--   0 ryanholinshead   (501) staff       (20)     3759 2024-03-14 13:26:50.000000 lm-debug-eval-ui-0.0.5/tests/test_run_config.py
```

### Comparing `lm-debug-eval-ui-0.0.4/LICENSE` & `lm-debug-eval-ui-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/PKG-INFO` & `lm-debug-eval-ui-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-debug-eval-ui
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLM Application Debug/Eval UI on top of AIConfig
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lm-debug-eval-ui-0.0.4/README.md` & `lm-debug-eval-ui-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/pyproject.toml` & `lm-debug-eval-ui-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "lm-debug-eval-ui"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="LastMile AI" },
 ]
 description = "LLM Application Debug/Eval UI on top of AIConfig"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/ChatCompletion.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/ChatCompletion.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/Config.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/Config.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/__init__.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/callback.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/callback.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/anyscale_endpoint.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/anyscale_endpoint.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/azure.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/azure.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/claude.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/claude.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/dalle.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/dalle.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/gemini.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/gemini.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/hf.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/hf.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/openai_vision.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/openai_vision.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/palm.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/palm.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/default_parsers/parameterized_model_parser.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/default_parsers/parameterized_model_parser.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/client/node_modules/flatted/python/test.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/client/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/example_aiconfig_model_registry.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/example_aiconfig_model_registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/eval_server_utils.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/eval_server_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/queue_iterator.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/queue_iterator.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             path = aiconfig.file_path
 
     res_path_val = get_validated_path(path, allow_create=True)
     match res_path_val:
         case Ok(path_ok):
             _op = make_op_run_method(MethodName("save"))
             op_args: Result[OpArgs, str] = result.Ok(
-                OpArgs({"config_filepath": path_ok})
+                OpArgs({"config_filepath": path_ok, "include_outputs": False})
             )
             return run_aiconfig_operation_with_op_args(
                 aiconfig, "save", _op, op_args
             )
 
         case Err(e):
             return HttpResponseWithAIConfig(
```

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_file_utils.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server_file_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/server_utils.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/server_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/asset-manifest.json` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/images/aiconfigLogo.png` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/images/aiconfigLogo.png`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/index.html` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/index.html`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/302.6a4a934a.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/450.3ec30143.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/647.2d46acf1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map` & `lm-debug-eval-ui-0.0.5/src/aiconfig/editor/server/static/static/js/main.26b0450c.js.map`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/api/__init__.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/eval/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/common.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/eval/common.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/lib.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/eval/lib.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/metrics.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/eval/openai.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/eval/openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/model_parser.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/model_parser.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/registry.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/schema.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/schema.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/aiconfig_cli.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/aiconfig_cli.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/rage/rage.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/rage/rage.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/scripts/run_aiconfig.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/scripts/run_aiconfig.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/util/config_utils.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/aiconfig/util/params.py` & `lm-debug-eval-ui-0.0.5/src/aiconfig/util/params.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/PKG-INFO` & `lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-debug-eval-ui
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLM Application Debug/Eval UI on top of AIConfig
 Author: LastMile AI
 Project-URL: Homepage, https://github.com/lastmile-ai/aiconfig
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lm-debug-eval-ui-0.0.4/src/lm_debug_eval_ui.egg-info/SOURCES.txt` & `lm-debug-eval-ui-0.0.5/src/lm_debug_eval_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_chatcompletion_mock_wrapper.py` & `lm-debug-eval-ui-0.0.5/tests/test_chatcompletion_mock_wrapper.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_dataclass.py` & `lm-debug-eval-ui-0.0.5/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_eval.py` & `lm-debug-eval-ui-0.0.5/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_eval_model_graded_openai.py` & `lm-debug-eval-ui-0.0.5/tests/test_eval_model_graded_openai.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_library_helpers.py` & `lm-debug-eval-ui-0.0.5/tests/test_library_helpers.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_load_config.py` & `lm-debug-eval-ui-0.0.5/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_parameter_api.py` & `lm-debug-eval-ui-0.0.5/tests/test_parameter_api.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_programmatically_create_an_AIConfig.py` & `lm-debug-eval-ui-0.0.5/tests/test_programmatically_create_an_AIConfig.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_registry.py` & `lm-debug-eval-ui-0.0.5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_resolve.py` & `lm-debug-eval-ui-0.0.5/tests/test_resolve.py`

 * *Files identical despite different names*

### Comparing `lm-debug-eval-ui-0.0.4/tests/test_run_config.py` & `lm-debug-eval-ui-0.0.5/tests/test_run_config.py`

 * *Files identical despite different names*

