# Comparing `tmp/uptrain-0.6.8.tar.gz` & `tmp/uptrain-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.6.8.tar", last modified: Mon Mar 18 10:17:55 2024, max compression
+gzip compressed data, was "uptrain-0.6.9.tar", last modified: Wed Mar 20 18:23:13 2024, max compression
```

## Comparing `uptrain-0.6.8.tar` & `uptrain-0.6.9.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.517465 uptrain-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 10:17:46.000000 uptrain-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-03-18 10:17:55.517465 uptrain-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20102 2024-03-18 10:17:46.000000 uptrain-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-18 10:17:46.000000 uptrain-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 10:17:55.517465 uptrain-0.6.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.501465 uptrain-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30403 2024-03-18 10:17:46.000000 uptrain-0.6.8/tests/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-18 10:17:46.000000 uptrain-0.6.8/tests/test_custom_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-03-18 10:17:46.000000 uptrain-0.6.8/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.501465 uptrain-0.6.8/uptrain/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.497465 uptrain-0.6.8/uptrain/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.501465 uptrain-0.6.8/uptrain/dashboard/backend/
--rw-r--r--   0 runner    (1001) docker     (127)    32102 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/dashboard/backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/dashboard/backend/nest_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.505465 uptrain-0.6.8/uptrain/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/evalllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/evals.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/rca_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    28392 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/framework/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.505465 uptrain-0.6.8/uptrain/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/integrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/integrations/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/integrations/promptfoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/integrations/promptfoo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.509465 uptrain-0.6.8/uptrain/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.509465 uptrain-0.6.8/uptrain/operators/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/code/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/code/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/drift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.509465 uptrain-0.6.8/uptrain/operators/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/embedding/vector_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/embs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.509465 uptrain-0.6.8/uptrain/operators/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/bq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/duck.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/io/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.513465 uptrain-0.6.8/uptrain/operators/language/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/bleu.py
--rw-r--r--   0 runner    (1001) docker     (127)    26151 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/context_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/factual_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/guideline.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/jailbreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/language_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/meteor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/model_grade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.497465 uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.513465 uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/completion_fns/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.513465 uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/elsuite/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/openai_evals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.513465 uptrain-0.6.8/uptrain/operators/language/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/prompts/classic.py
--rw-r--r--   0 runner    (1001) docker     (127)    41167 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/prompts/few_shots.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/prompts/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/prompts/output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/question_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/response_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/rouge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/tone.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/language/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.513465 uptrain-0.6.8/uptrain/operators/rca/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/rca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/rca/rag_with_citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/operators/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.517465 uptrain-0.6.8/uptrain/st_classic/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/st_classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/st_classic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/st_classic/st_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/st_classic/st_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/st_classic/st_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.517465 uptrain-0.6.8/uptrain/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/app_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/prompt_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/sql_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/sqlglot_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.517465 uptrain-0.6.8/uptrain/validation_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/validation_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-18 10:17:46.000000 uptrain-0.6.8/uptrain/validation_wrapper/validation_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 10:17:55.517465 uptrain-0.6.8/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21494 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 10:17:55.000000 uptrain-0.6.8/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 18:23:01.000000 uptrain-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-03-20 18:23:13.271146 uptrain-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28085 2024-03-20 18:23:01.000000 uptrain-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-03-20 18:23:01.000000 uptrain-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 18:23:13.271146 uptrain-0.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30080 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_custom_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-03-20 18:23:01.000000 uptrain-0.6.9/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.251146 uptrain-0.6.9/uptrain/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/dashboard/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)    32102 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/dashboard/backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/dashboard/backend/nest_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/evalllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/evals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/rca_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28392 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.259146 uptrain-0.6.9/uptrain/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/promptfoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/integrations/promptfoo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/code/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/drift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embedding/vector_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.263146 uptrain-0.6.9/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/bq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/duck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/io/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26151 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/context_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/factual_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13521 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7501 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/guideline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/jailbreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/language_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20512 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/model_grade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.255146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/openai_evals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/language/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)    19906 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41167 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/few_shots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/prompts/output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/question_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36147 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/response_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/tone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/language/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.267146 uptrain-0.6.9/uptrain/operators/rca/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/rca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/rca/rag_with_citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/operators/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/st_classic/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/st_classic/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/app_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/prompt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/sqlglot_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-03-20 18:23:01.000000 uptrain-0.6.9/uptrain/validation_wrapper/validation_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 18:23:13.271146 uptrain-0.6.9/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29448 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 18:23:13.000000 uptrain-0.6.9/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.6.8/LICENSE` & `uptrain-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/pyproject.toml` & `uptrain-0.6.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "uptrain"
-version = "0.6.8"
+version = "0.6.9"
 description = "UpTrain - tool to evaluate LLM applications on aspects like factual accuracy, response quality, retrieval quality, tonality, etc."
 readme = "README.md"
 maintainers = [{ name = "UpTrain AI Team", email = "oss@uptrain.ai" }]
 license = {text = "Apache-2.0"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 keywords = ["uptrain", "ai", "LLM", "evaluation", "hallucinations", "observability", "response quality"]
 dependencies = [
     "pydantic",
@@ -30,15 +29,16 @@
     "numpy>=1.23.0",
     "httpx>=0.24.1",
     "plotly>=5.0.0",
     "aiolimiter>=1.1",
     "openai>=1.6.1",
     "fsspec",
     "litellm",
-    "pyyaml"
+    "pyyaml",
+    "json5"
 ]
 
 [project.urls]
 Homepage = "https://uptrain.ai"
 Repository = "https://github.com/uptrain-ai/uptrain"
 
 [project.scripts]
```

### Comparing `uptrain-0.6.8/tests/test_builtins.py` & `uptrain-0.6.9/tests/test_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,33 +160,26 @@
 
 def test_check_response_consistency():
     check = CheckResponseConsistency()
     output = check.setup(settings).run(dataset)
     assert isinstance(output, pl.DataFrame)
     assert (
         "score_response_consistency" in output.columns
-        and "argument_response_consistency" in output.columns
+        and "explanation_response_consistency" in output.columns
     )     
     assert (
         output["score_response_consistency"].dtype == pl.Float64 
         and len(output["score_response_consistency"]) 
         - output["score_response_consistency"].null_count() > 0
     )
     assert (
-        output["argument_response_consistency"].dtype == pl.Utf8 
-        and len(output["argument_response_consistency"]) 
-        - output["argument_response_consistency"].null_count() > 0
+        output["explanation_response_consistency"].dtype == pl.Utf8 
+        and len(output["explanation_response_consistency"]) 
+        - output["explanation_response_consistency"].null_count() > 0
     )
-    if settings.eval_type == "cot":
-        assert "reasoning_response_consistency" in output.columns
-        assert (
-            output["reasoning_response_consistency"].dtype == pl.Utf8 
-            and len(output["reasoning_response_consistency"]) 
-            - output["reasoning_response_consistency"].null_count() > 0
-        )
 
 
 response_matching_dataset = pl.DataFrame(
     {
         "question": [
             "Do both Ronaldo and Messi play in the Spanish League?",
         ],
```

### Comparing `uptrain-0.6.8/tests/test_custom_ops.py` & `uptrain-0.6.9/tests/test_custom_ops.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/tests/test_operators.py` & `uptrain-0.6.9/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/__init__.pyi` & `uptrain-0.6.9/uptrain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/cli.py` & `uptrain-0.6.9/uptrain/cli.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/dashboard/backend/app.py` & `uptrain-0.6.9/uptrain/dashboard/backend/app.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/dashboard/backend/nest_asyncio.py` & `uptrain-0.6.9/uptrain/dashboard/backend/nest_asyncio.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/__init__.pyi` & `uptrain-0.6.9/uptrain/framework/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/base.py` & `uptrain-0.6.9/uptrain/framework/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/builtins.py` & `uptrain-0.6.9/uptrain/framework/builtins.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/checks.py` & `uptrain-0.6.9/uptrain/framework/checks.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/evalllm.py` & `uptrain-0.6.9/uptrain/framework/evalllm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,30 @@
 import httpx
 import polars as pl
 import pandas as pd
 import pydantic
 import copy
 import os
 import httpx
-from uptrain.utilities.utils import get_current_datetime, parse_prompt
+from uptrain.operators.base import ColumnOp
+from uptrain.utilities.utils import get_current_datetime, parse_prompt, check_openai_api_key
 from uptrain.framework.remote import APIClientWithoutAuth, DataSchema
 from uptrain.framework.base import Settings
+from uptrain.framework.checks import Check
 from uptrain.framework.evals import (
     Evals,
     JailbreakDetection,
     ParametricEval,
     CritiqueTone,
     GuidelineAdherence,
     ResponseMatching,
     ConversationSatisfaction,
 )
 from uptrain.operators import (
+    TransformOp,
     ResponseFactualScore,
     ContextRelevance,
     ResponseCompleteness,
     ResponseCompletenessWrtContext,
     ResponseConciseness,
     ResponseConsistency,
     ResponseMatchingScore,
@@ -83,14 +86,19 @@
         if (openai_api_key is None) and (settings is None):
             raise Exception("Please provide OpenAI API Key")
 
         if settings is None:
             self.settings = Settings(openai_api_key=openai_api_key)
         else:
             self.settings = settings
+        if self.settings.openai_api_key is not None and len(self.settings.openai_api_key):
+            response = check_openai_api_key(self.settings.openai_api_key)
+            if not response:
+                raise Exception("OpenAI API Key is invalid")
+
         self.executor = APIClientWithoutAuth(self.settings)
 
     ####
     def perform_root_cause_analysis(
         self,
         data: t.Union[list[dict], pl.DataFrame, pd.DataFrame],
         rca_template: RcaTemplate,
@@ -181,26 +189,29 @@
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results.
         """
 
         if isinstance(data, pl.DataFrame):
             data = data.to_dicts()
+        elif isinstance(data, pd.DataFrame):
+            data = data.to_dict(orient="records")
 
         if schema is None:
             schema = DataSchema()
         elif isinstance(schema, dict):
             schema = DataSchema(**schema)
 
         if metadata is None:
             metadata = {}
 
         checks = [Evals(m) if isinstance(m, str) else m for m in checks]
         for m in checks:
-            assert isinstance(m, (Evals, ParametricEval))
+            assert isinstance(m, (Evals, ParametricEval, TransformOp, ColumnOp, list))
+            # TODO: Check type of each element in the list - should be transformOp
 
         req_attrs, ser_checks = set(), []
         for idx, m in enumerate(checks):
             if m in [Evals.SUB_QUERY_COMPLETENESS]:
                 req_attrs.update([schema.sub_questions, schema.question])
             elif m in [Evals.CONTEXT_CONCISENESS]:
                 req_attrs.update(
@@ -250,14 +261,22 @@
             if isinstance(m, ParametricEval):
                 dictm = m.model_dump()
                 dictm.update({"scenario_description": this_scenario_description})
                 ser_checks.append({"check_name": m.__class__.__name__, **dictm})
             elif isinstance(m, Evals):
                 dictm = {"scenario_description": this_scenario_description}
                 ser_checks.append({"check_name": m.value, **dictm})
+            elif isinstance(m, TransformOp):
+                dictm = m.model_dump()
+                ser_checks.append({"check_name": m.__class__.__name__, **dictm})
+            elif isinstance(m, ColumnOp):
+                dictm = m.model_dump()
+                ser_checks.append({"check_name": m.__class__.__name__, **dictm})
+            elif isinstance(m, list):
+                ser_checks.append({"check_name": "dummy_list_ops"})
             else:
                 raise ValueError(f"Invalid metric: {m}")
 
         for idx, row in enumerate(data):
             if not req_attrs.issubset(row.keys()):
                 raise ValueError(
                     f"Row {idx} is missing required all required attributes for evaluation: {req_attrs}"
@@ -288,14 +307,33 @@
                         else scenario_description[idx]
                     )
                     res = (
                         op.setup(self.settings)
                         .run(pl.DataFrame(data))["output"]
                         .to_dicts()
                     )
+                elif isinstance(check, TransformOp):
+                    op = check
+                    res = (
+                        op.setup(self.settings)
+                        .run(pl.DataFrame(data))["output"]
+                        .to_dicts()
+                    )
+                elif isinstance(check, ColumnOp):
+                    op = Check(name = "dummy", operators = [check])
+                    res = (
+                        op.setup(self.settings)
+                        .run(pl.DataFrame(data))
+                    ).to_dicts()
+                elif isinstance(check, list):
+                    op = Check(name = "dummy", operators = check)
+                    res = (
+                        op.setup(self.settings)
+                        .run(pl.DataFrame(data))
+                    ).to_dicts()
                 else:
                     res = self.evaluate_on_server(data, [ser_checks[idx]], schema)
                 for idx, row in enumerate(res):
                     results[idx].update(row)
         else:
             results = self.evaluate_on_server(data, ser_checks, schema)
         ## local server calls
```

### Comparing `uptrain-0.6.8/uptrain/framework/evals.py` & `uptrain-0.6.9/uptrain/framework/evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/remote.py` & `uptrain-0.6.9/uptrain/framework/remote.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/framework/signal.py` & `uptrain-0.6.9/uptrain/framework/signal.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/integrations/llama_index.py` & `uptrain-0.6.9/uptrain/integrations/llama_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 import os
 import typing as t
 
 from loguru import logger
+import pandas as pd
 import polars as pl
 from uptrain import Settings
 from uptrain.framework.evals import Evals, ParametricEval
 from uptrain.framework.evalllm import EvalLLM
 from uptrain.framework.remote import APIClient
 from uptrain.framework.remote import DataSchema
 
@@ -65,14 +66,17 @@
             metadata: Attributes to attach to this dataset. Useful for filtering and grouping in the UI.
         Returns:
             results: List of dictionaries with each data point and corresponding evaluation results.
         """
 
         if isinstance(data, pl.DataFrame):
             data = data.to_dicts()
+        elif isinstance(data, pd.DataFrame):
+            data = data.to_dict(orient="records")
+
         import nest_asyncio
 
         nest_asyncio.apply()
 
         if schema is None:
             schema = DataSchema()
         elif isinstance(schema, dict):
```

### Comparing `uptrain-0.6.8/uptrain/integrations/promptfoo.py` & `uptrain-0.6.9/uptrain/integrations/promptfoo.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/integrations/promptfoo_utils.py` & `uptrain-0.6.9/uptrain/integrations/promptfoo_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/__init__.pyi` & `uptrain-0.6.9/uptrain/operators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/base.py` & `uptrain-0.6.9/uptrain/operators/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/chart.py` & `uptrain-0.6.9/uptrain/operators/chart.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/clustering.py` & `uptrain-0.6.9/uptrain/operators/clustering.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/code/detection.py` & `uptrain-0.6.9/uptrain/operators/code/detection.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/code/sql.py` & `uptrain-0.6.9/uptrain/operators/code/sql.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/drift.py` & `uptrain-0.6.9/uptrain/operators/drift.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/embedding/embedding.py` & `uptrain-0.6.9/uptrain/operators/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/embedding/vector_search.py` & `uptrain-0.6.9/uptrain/operators/embedding/vector_search.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/embs.py` & `uptrain-0.6.9/uptrain/operators/embs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/io/base.py` & `uptrain-0.6.9/uptrain/operators/io/base.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/io/bq.py` & `uptrain-0.6.9/uptrain/operators/io/bq.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/io/duck.py` & `uptrain-0.6.9/uptrain/operators/io/duck.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/io/excel.py` & `uptrain-0.6.9/uptrain/operators/io/excel.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/io/mongodb.py` & `uptrain-0.6.9/uptrain/operators/io/mongodb.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/bleu.py` & `uptrain-0.6.9/uptrain/operators/language/bleu.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/context_quality.py` & `uptrain-0.6.9/uptrain/operators/language/context_quality.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/conversation.py` & `uptrain-0.6.9/uptrain/operators/language/conversation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/factual_accuracy.py` & `uptrain-0.6.9/uptrain/operators/language/factual_accuracy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Implement operators to evaluate factual correctness of the response.
 """
 
 from __future__ import annotations
 import typing as t
-import json
 
 from loguru import logger
 import polars as pl
 import numpy as np
 
 from uptrain.utilities.prompt_utils import parse_scenario_description
 
@@ -16,15 +15,15 @@
     from uptrain.framework import Settings
 from uptrain.operators.base import (
     register_op,
     ColumnOp,
     TYPE_TABLE_OUTPUT,
 )
 from uptrain.utilities import polars_to_json_serializable_dict
-from uptrain.operators.language.llm import LLMMulticlient
+from uptrain.operators.language.llm import LLMMulticlient, parse_json
 
 from uptrain.operators.language.prompts.classic import (
     FACT_EVAL_PROMPT_TEMPLATE,
     FACT_GENERATE_PROMPT_TEMPLATE,
 )
 from uptrain.operators.language.prompts.few_shots import (
     FACT_EVAL_FEW_SHOT__CLASSIFY,
@@ -170,15 +169,15 @@
             input_payloads, self.fact_generate_validate_func
         )
 
         fact_results = []
         for res in output_payloads:
             idx = res.metadata["index"]
             try:
-                facts = json.loads(res.response.choices[0].message.content)
+                facts = parse_json(res.response.choices[0].message.content)
                 fact_results.append((idx, facts))
             except Exception:
                 logger.error(
                     f"Error when processing payload at index {idx}: {res.error}"
                 )
                 fact_results.append((idx, []))
         fact_results = [val for _, val in sorted(fact_results, key=lambda x: x[0])]
@@ -227,19 +226,18 @@
         for res in output_payloads:
             idx = res.metadata["index"]
             output = {
                 "score_factual_accuracy": None,
                 "explanation_factual_accuracy": None,
             }
             try:
-                result = json.loads(res.response.choices[0].message.content)["Result"]
-                judgements = [x["Judgement"] for x in result]
+                judgements = [x["Judgement"] for x in parse_json(res.response.choices[0].message.content)["Result"]]
                 score = np.mean([self.score_mapping[x.lower()] for x in judgements])
                 output["score_factual_accuracy"] = float(score)
-                output["explanation_factual_accuracy"] = result
+                output["explanation_factual_accuracy"] = res.response.choices[0].message.content
             except Exception:
                 logger.error(
                     f"Error when processing payload at index {idx}: {res.error}"
                 )
             results.append((idx, output))
         results = [val for _, val in sorted(results, key=lambda x: x[0])]
```

### Comparing `uptrain-0.6.8/uptrain/operators/language/generation.py` & `uptrain-0.6.9/uptrain/operators/language/generation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/grammar.py` & `uptrain-0.6.9/uptrain/operators/language/grammar.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/guideline.py` & `uptrain-0.6.9/uptrain/operators/language/guideline.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/jailbreak.py` & `uptrain-0.6.9/uptrain/operators/language/jailbreak.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/language_quality.py` & `uptrain-0.6.9/uptrain/operators/language/language_quality.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/llm.py` & `uptrain-0.6.9/uptrain/operators/language/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 import random
 import typing as t
-import json
+import json5
 
 from loguru import logger
 from pydantic import BaseModel, Field
 
 if t.TYPE_CHECKING:
     from uptrain.framework import Settings
 from uptrain.utilities import lazy_load_dep
@@ -46,15 +46,15 @@
 
 
 def parse_json(json_str: str) -> dict:
     first_brace_index = json_str.find('{')
     last_brace_index = json_str.rfind('}')
     json_str = json_str[first_brace_index:last_brace_index + 1]
     try:
-        return json.loads(json_str)
+        return json5.loads(json_str)
     except Exception as e:
         logger.error(f"Error when parsing JSON: {e}")
         return {}
 
 def run_validation(llm_output, validation_func):
     llm_output = parse_json(llm_output)
     try:
```

### Comparing `uptrain-0.6.8/uptrain/operators/language/meteor.py` & `uptrain-0.6.9/uptrain/operators/language/meteor.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/model_grade.py` & `uptrain-0.6.9/uptrain/operators/language/model_grade.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py` & `uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/completion_fns/dummy.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py` & `uptrain-0.6.9/uptrain/operators/language/openai_eval_custom/elsuite/model_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/openai_evals.py` & `uptrain-0.6.9/uptrain/operators/language/openai_evals.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/prompts/classic.py` & `uptrain-0.6.9/uptrain/operators/language/prompts/classic.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/prompts/few_shots.py` & `uptrain-0.6.9/uptrain/operators/language/prompts/few_shots.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/prompts/output_format.py` & `uptrain-0.6.9/uptrain/operators/language/prompts/output_format.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/question_quality.py` & `uptrain-0.6.9/uptrain/operators/language/question_quality.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/response_quality.py` & `uptrain-0.6.9/uptrain/operators/language/response_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -478,23 +478,23 @@
         )
 
         results = []
         for res in output_payloads:
             idx = res.metadata["index"]
             output = {
                 "score_response_consistency": None,
-                "argument_response_consistency": None,
+                "explanation_response_consistency": None,
             }
             try:
                 parsed_output = json.loads(res.response.choices[0].message.content)
                 score = parsed_output["Score"]
                 output["score_response_consistency"] = float(score)
-                output["argument_response_consistency"] = parsed_output["Argument"]
+                output["explanation_response_consistency"] = parsed_output["Argument"]
                 if self.settings.eval_type == "cot":
-                    output["reasoning_response_consistency"] = parsed_output[
+                    output["explanation_response_consistency"] += "\n" + parsed_output[
                         "Reasoning"
                     ]
             except Exception:
                 logger.error(
                     f"Error when processing payload at index {idx}: {res.error}"
                 )
             results.append((idx, output))
```

### Comparing `uptrain-0.6.8/uptrain/operators/language/rouge.py` & `uptrain-0.6.9/uptrain/operators/language/rouge.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/subquery.py` & `uptrain-0.6.9/uptrain/operators/language/subquery.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/text.py` & `uptrain-0.6.9/uptrain/operators/language/text.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/tone.py` & `uptrain-0.6.9/uptrain/operators/language/tone.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/language/topic.py` & `uptrain-0.6.9/uptrain/operators/language/topic.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/metrics.py` & `uptrain-0.6.9/uptrain/operators/metrics.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/rca/rag_with_citation.py` & `uptrain-0.6.9/uptrain/operators/rca/rag_with_citation.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/similarity.py` & `uptrain-0.6.9/uptrain/operators/similarity.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/operators/table.py` & `uptrain-0.6.9/uptrain/operators/table.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/st_classic/st_helpers.py` & `uptrain-0.6.9/uptrain/st_classic/st_helpers.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/st_classic/st_run.py` & `uptrain-0.6.9/uptrain/st_classic/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/st_classic/st_setup.py` & `uptrain-0.6.9/uptrain/st_classic/st_setup.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/__init__.py` & `uptrain-0.6.9/uptrain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/app_schema.py` & `uptrain-0.6.9/uptrain/utilities/app_schema.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/db.py` & `uptrain-0.6.9/uptrain/utilities/db.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/prompt_utils.py` & `uptrain-0.6.9/uptrain/utilities/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/sql_utils.py` & `uptrain-0.6.9/uptrain/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/sql_utils_test.py` & `uptrain-0.6.9/uptrain/utilities/sql_utils_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/sqlglot_test.py` & `uptrain-0.6.9/uptrain/utilities/sqlglot_test.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain/utilities/utils.py` & `uptrain-0.6.9/uptrain/utilities/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,27 @@
     GuidelineAdherence,
     ConversationSatisfaction,
     JailbreakDetection,
     CritiqueTone,
 )
 from uptrain.utilities import lazy_load_dep
 
+def check_openai_api_key(api_key):
+    import openai
+    client = openai.OpenAI(api_key=api_key)
+    try:
+        client.models.list()
+    except openai.AuthenticationError:
+        return False
+    else:
+        return True
+    
 def _get_fsspec_filesystem(database_path) -> fsspec.AbstractFileSystem:
     return DirFileSystem(database_path, auto_mkdir=True)
 
-
-
 fsspec.config.conf["file"] = {"auto_mkdir": True}
 
 evals_mapping = {
     "context_relevance": Evals.CONTEXT_RELEVANCE,
     "factual_accuracy": Evals.FACTUAL_ACCURACY,
     "response_relevance": Evals.RESPONSE_RELEVANCE,
     "critique_language": Evals.CRITIQUE_LANGUAGE,
```

### Comparing `uptrain-0.6.8/uptrain/validation_wrapper/validation_manager.py` & `uptrain-0.6.9/uptrain/validation_wrapper/validation_manager.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.6.8/uptrain.egg-info/SOURCES.txt` & `uptrain-0.6.9/uptrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

