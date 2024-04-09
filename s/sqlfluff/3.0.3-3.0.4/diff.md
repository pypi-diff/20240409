# Comparing `tmp/sqlfluff-3.0.3.tar.gz` & `tmp/sqlfluff-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff-3.0.3.tar", last modified: Fri Mar 22 11:58:27 2024, max compression
+gzip compressed data, was "sqlfluff-3.0.4.tar", last modified: Tue Apr  9 17:45:05 2024, max compression
```

## Comparing `sqlfluff-3.0.3.tar` & `sqlfluff-3.0.4.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.170480 sqlfluff-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)   493097 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-03-22 11:58:27.170480 sqlfluff-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 11:58:27.170480 sqlfluff-3.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.110480 sqlfluff-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.118480 sqlfluff-3.0.3/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.118480 sqlfluff-3.0.3/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.122480 sqlfluff-3.0.3/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    49059 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.122480 sqlfluff-3.0.3/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.122480 sqlfluff-3.0.3/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.122480 sqlfluff-3.0.3/src/sqlfluff/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/helpers/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/helpers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.126480 sqlfluff-3.0.3/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    45903 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.130480 sqlfluff-3.0.3/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.130480 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/match_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.130480 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48833 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/bracketed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/parser/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.134480 sqlfluff-3.0.3/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.134480 sqlfluff-3.0.3/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/rules/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.134480 sqlfluff-3.0.3/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46392 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.134480 sqlfluff-3.0.3/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.146480 sqlfluff-3.0.3/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137827 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22627 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    70381 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    33911 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    93118 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    19406 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_greenplum_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    82669 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28324 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)   190826 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    36994 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    72988 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   234732 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (127)   104740 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    17014 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    27893 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11213 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_trino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_trino_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   189300 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    65703 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_vertica.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_vertica_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.146480 sqlfluff-3.0.3/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.150480 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.150480 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.154480 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.154480 sqlfluff-3.0.3/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.154480 sqlfluff-3.0.3/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.158480 sqlfluff-3.0.3/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.158480 sqlfluff-3.0.3/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.162480 sqlfluff-3.0.3/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.162480 sqlfluff-3.0.3/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.162480 sqlfluff-3.0.3/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.162480 sqlfluff-3.0.3/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/analysis/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/analysis/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.166480 sqlfluff-3.0.3/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.166480 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.166480 sqlfluff-3.0.3/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.166480 sqlfluff-3.0.3/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 11:58:27.000000 sqlfluff-3.0.3/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 11:58:27.166480 sqlfluff-3.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-22 11:58:17.000000 sqlfluff-3.0.3/test/testing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)   499100 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.946646 sqlfluff-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.954646 sqlfluff-3.0.4/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.954646 sqlfluff-3.0.4/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49340 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.962646 sqlfluff-3.0.4/src/sqlfluff/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.962646 sqlfluff-3.0.4/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45903 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/match_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48833 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/bracketed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46392 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.974646 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.982646 sqlfluff-3.0.4/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138386 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22627 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70760 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35114 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93118 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82206 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28325 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   191205 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72987 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   240222 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104915 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27893 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189301 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65703 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.982646 sqlfluff-3.0.4/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.986646 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.986646 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.994646 sqlfluff-3.0.4/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.994646 sqlfluff-3.0.4/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 17:44:55.000000 sqlfluff-3.0.4/test/testing_test.py
```

### Comparing `sqlfluff-3.0.3/CHANGELOG.md` & `sqlfluff-3.0.4/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,70 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [3.0.4] - 2024-04-07
+
+## Highlights
+
+This is a standard bugfix release bringing a bunch of dialect improvements and
+bugfixes. Almost every dialect sees some improvements and it also includes
+quality of life improvements to the CLI, pre-commit hooks, docs and several
+rules.
+
+Thanks also to the **eight** new contributors whose first contributions are
+included in this release. 🎉🎉🏆🎉🎉
+
+## What’s Changed
+
+* TSQL: Move PROPERTY to unreserved [#5759](https://github.com/sqlfluff/sqlfluff/pull/5759) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Mysql: Add Character Set Literals [#5755](https://github.com/sqlfluff/sqlfluff/pull/5755) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Snowflake: Support ASOF Joins [#5756](https://github.com/sqlfluff/sqlfluff/pull/5756) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Mysql: Support scoped function calls [#5757](https://github.com/sqlfluff/sqlfluff/pull/5757) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Postgres: Support pgvector vector type [#5758](https://github.com/sqlfluff/sqlfluff/pull/5758) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* SQLite: Support RETURNING Clause [#5760](https://github.com/sqlfluff/sqlfluff/pull/5760) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Postgres: Allow return control structures in atomic functions [#5761](https://github.com/sqlfluff/sqlfluff/pull/5761) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* ST04: Retain comments when flattening `CASE` [#5753](https://github.com/sqlfluff/sqlfluff/pull/5753) [@keraion](https://github.com/keraion)
+* dbt templater: Raise UserError when using stdin [#5752](https://github.com/sqlfluff/sqlfluff/pull/5752) [@keraion](https://github.com/keraion)
+* SQLite: Add `GLOB`, `MATCH`. Improved `REGEXP` [#5745](https://github.com/sqlfluff/sqlfluff/pull/5745) [@keraion](https://github.com/keraion)
+* Databricks: Fix Aliases for Join-like objects [#5748](https://github.com/sqlfluff/sqlfluff/pull/5748) [@keraion](https://github.com/keraion)
+* Add missing README ref, and issues labels [#5741](https://github.com/sqlfluff/sqlfluff/pull/5741) [@WittierDinosaur](https://github.com/WittierDinosaur)
+* Qual: Add pre-commit to CI [#5730](https://github.com/sqlfluff/sqlfluff/pull/5730) [@mdeweerd](https://github.com/mdeweerd)
+* Added support for 'greater/less than or equal' on ANSI CASE statement [#5728](https://github.com/sqlfluff/sqlfluff/pull/5728) [@IliyanKostov9](https://github.com/IliyanKostov9)
+* Remove `--force` flag from pre-commit hook definition [#5739](https://github.com/sqlfluff/sqlfluff/pull/5739) [@borchero](https://github.com/borchero)
+* adding snake_case to CP01 extended_capitalisation_policy [#5736](https://github.com/sqlfluff/sqlfluff/pull/5736) [@alecsgonz](https://github.com/alecsgonz)
+* ST04: Ignore simplifying `CASE`s with different expressions [#5735](https://github.com/sqlfluff/sqlfluff/pull/5735) [@keraion](https://github.com/keraion)
+* Fix #5724 mysql: Allow Line comments without space after -- [#5731](https://github.com/sqlfluff/sqlfluff/pull/5731) [@mdeweerd](https://github.com/mdeweerd)
+* Fix spelling [#5729](https://github.com/sqlfluff/sqlfluff/pull/5729) [@mdeweerd](https://github.com/mdeweerd)
+* Fix implementation for view_column_name_list in BigQuery's CREATE VIEW [#5738](https://github.com/sqlfluff/sqlfluff/pull/5738) [@kzosabe](https://github.com/kzosabe)
+* CLI: Suppress tracebacks on render/fix/format [#5734](https://github.com/sqlfluff/sqlfluff/pull/5734) [@keraion](https://github.com/keraion)
+* Clickhouse: add parsing for select except clause [#5725](https://github.com/sqlfluff/sqlfluff/pull/5725) [@tojahech](https://github.com/tojahech)
+* Add array type support to Trino dialect [#5722](https://github.com/sqlfluff/sqlfluff/pull/5722) [@kirkhansen](https://github.com/kirkhansen)
+* Fix/snowflake unparsable tag in create stmt [#5720](https://github.com/sqlfluff/sqlfluff/pull/5720) [@mariq41](https://github.com/mariq41)
+* Fix/snowflake ext storage [#5714](https://github.com/sqlfluff/sqlfluff/pull/5714) [@mariq41](https://github.com/mariq41)
+* Clickhouse: add parsing for "distinct on" syntax [#5716](https://github.com/sqlfluff/sqlfluff/pull/5716) [@tojahech](https://github.com/tojahech)
+* added refresh mode init on create table statement [#5715](https://github.com/sqlfluff/sqlfluff/pull/5715) [@IliyanKostov9](https://github.com/IliyanKostov9)
+* added `ifNotExistsGrammar` to Snowflake procedure [#5709](https://github.com/sqlfluff/sqlfluff/pull/5709) [@IliyanKostov9](https://github.com/IliyanKostov9)
+* Trino: 'TIMESTAMP(p)' no longer triggers LT01 [#5711](https://github.com/sqlfluff/sqlfluff/pull/5711) [@rileymcdowell](https://github.com/rileymcdowell)
+* Snowflake: add support for streamlit [#5692](https://github.com/sqlfluff/sqlfluff/pull/5692) [@vgw-chriskruger](https://github.com/vgw-chriskruger)
+
+## New Contributors
+
+* [@vgw-chriskruger](https://github.com/vgw-chriskruger) made their first contribution in [#5692](https://github.com/sqlfluff/sqlfluff/pull/5692)
+* [@IliyanKostov9](https://github.com/IliyanKostov9) made their first contribution in [#5709](https://github.com/sqlfluff/sqlfluff/pull/5709)
+* [@tojahech](https://github.com/tojahech) made their first contribution in [#5716](https://github.com/sqlfluff/sqlfluff/pull/5716)
+* [@mariq41](https://github.com/mariq41) made their first contribution in [#5714](https://github.com/sqlfluff/sqlfluff/pull/5714)
+* [@kirkhansen](https://github.com/kirkhansen) made their first contribution in [#5722](https://github.com/sqlfluff/sqlfluff/pull/5722)
+* [@kzosabe](https://github.com/kzosabe) made their first contribution in [#5738](https://github.com/sqlfluff/sqlfluff/pull/5738)
+* [@mdeweerd](https://github.com/mdeweerd) made their first contribution in [#5729](https://github.com/sqlfluff/sqlfluff/pull/5729)
+* [@alecsgonz](https://github.com/alecsgonz) made their first contribution in [#5736](https://github.com/sqlfluff/sqlfluff/pull/5736)
+
 ## [3.0.3] - 2024-03-22
 
 ## Highlights
 
 This is a standard minor release fixing a set of dialect issues with Trino, BigQuery,
 Vertica and Snowflake.
 
@@ -187,15 +243,15 @@
 * DB2: Add support for `DECLARE GLOBAL TEMPORARY TABLES`, `OFFSET`, `CALL`, and non-bracketed `VALUES` [#5508](https://github.com/sqlfluff/sqlfluff/pull/5508) [@keraion](https://github.com/keraion)
 * DuckDB: Add CREATE OR REPLACE TABLE syntax [#5511](https://github.com/sqlfluff/sqlfluff/pull/5511) [@keraion](https://github.com/keraion)
 * TSQL: Top and Distinct in same query [#5491](https://github.com/sqlfluff/sqlfluff/pull/5491) [@greg-finley](https://github.com/greg-finley)
 * [Spark/Databricks] Fix: make COLUMNS in APPLY CHANGES INTO optional [#5498](https://github.com/sqlfluff/sqlfluff/pull/5498) [@rocwang](https://github.com/rocwang)
 * SparkSQL: exclamation mark as logical not [#5500](https://github.com/sqlfluff/sqlfluff/pull/5500) [@reata](https://github.com/reata)
 * SparkSQL: allow value in set_statement to be Java class name [#5504](https://github.com/sqlfluff/sqlfluff/pull/5504) [@reata](https://github.com/reata)
 * SparkSQL: allow distribute/sort/cluster by at end of set operation [#5502](https://github.com/sqlfluff/sqlfluff/pull/5502) [@reata](https://github.com/reata)
-* [CI] Add a few more mypy ckecks [#5505](https://github.com/sqlfluff/sqlfluff/pull/5505) [@Koyaani](https://github.com/Koyaani)
+* [CI] Add a few more mypy checks [#5505](https://github.com/sqlfluff/sqlfluff/pull/5505) [@Koyaani](https://github.com/Koyaani)
 * Snowflake dialect: Add support for DATABASE ROLE in GRANT/REVOKE [#5490](https://github.com/sqlfluff/sqlfluff/pull/5490) [@sfc-gh-dgupta](https://github.com/sfc-gh-dgupta)
 * DuckDB: Qualify and From-First [#5485](https://github.com/sqlfluff/sqlfluff/pull/5485) [@keraion](https://github.com/keraion)
 * MySql: create table: allow null/not null in any position [#5473](https://github.com/sqlfluff/sqlfluff/pull/5473) [@archer62](https://github.com/archer62)
 * Snowflake dialect: Support for CREATE DATABASE ROLE [#5475](https://github.com/sqlfluff/sqlfluff/pull/5475) [@sfc-gh-dgupta](https://github.com/sfc-gh-dgupta)
 * Clickhouse Dialect - Support BackQuoted Identifiers [#5457](https://github.com/sqlfluff/sqlfluff/pull/5457) [@kaiyannameighu](https://github.com/kaiyannameighu)
 * Change Color.lightgrey to have a white background - dark theme friendly [#5458](https://github.com/sqlfluff/sqlfluff/pull/5458) [@ryaminal](https://github.com/ryaminal)
 * Fix indentation for single cube clause [#5462](https://github.com/sqlfluff/sqlfluff/pull/5462) [@tunetheweb](https://github.com/tunetheweb)
@@ -378,15 +434,15 @@
 * DB2: Add support for `DECLARE GLOBAL TEMPORARY TABLES`, `OFFSET`, `CALL`, and non-bracketed `VALUES` [#5508](https://github.com/sqlfluff/sqlfluff/pull/5508) [@keraion](https://github.com/keraion)
 * DuckDB: Add CREATE OR REPLACE TABLE syntax [#5511](https://github.com/sqlfluff/sqlfluff/pull/5511) [@keraion](https://github.com/keraion)
 * TSQL: Top and Distinct in same query [#5491](https://github.com/sqlfluff/sqlfluff/pull/5491) [@greg-finley](https://github.com/greg-finley)
 * [Spark/Databricks] Fix: make COLUMNS in APPLY CHANGES INTO optional [#5498](https://github.com/sqlfluff/sqlfluff/pull/5498) [@rocwang](https://github.com/rocwang)
 * SparkSQL: exclamation mark as logical not [#5500](https://github.com/sqlfluff/sqlfluff/pull/5500) [@reata](https://github.com/reata)
 * SparkSQL: allow value in set_statement to be Java class name [#5504](https://github.com/sqlfluff/sqlfluff/pull/5504) [@reata](https://github.com/reata)
 * SparkSQL: allow distribute/sort/cluster by at end of set operation [#5502](https://github.com/sqlfluff/sqlfluff/pull/5502) [@reata](https://github.com/reata)
-* [CI] Add a few more mypy ckecks [#5505](https://github.com/sqlfluff/sqlfluff/pull/5505) [@Koyaani](https://github.com/Koyaani)
+* [CI] Add a few more mypy checks [#5505](https://github.com/sqlfluff/sqlfluff/pull/5505) [@Koyaani](https://github.com/Koyaani)
 * Snowflake dialect: Add support for DATABASE ROLE in GRANT/REVOKE [#5490](https://github.com/sqlfluff/sqlfluff/pull/5490) [@sfc-gh-dgupta](https://github.com/sfc-gh-dgupta)
 * DuckDB: Qualify and From-First [#5485](https://github.com/sqlfluff/sqlfluff/pull/5485) [@keraion](https://github.com/keraion)
 * MySql: create table: allow null/not null in any position [#5473](https://github.com/sqlfluff/sqlfluff/pull/5473) [@archer62](https://github.com/archer62)
 * Snowflake dialect: Support for CREATE DATABASE ROLE [#5475](https://github.com/sqlfluff/sqlfluff/pull/5475) [@sfc-gh-dgupta](https://github.com/sfc-gh-dgupta)
 * Clickhouse Dialect - Support BackQuoted Identifiers [#5457](https://github.com/sqlfluff/sqlfluff/pull/5457) [@kaiyannameighu](https://github.com/kaiyannameighu)
 * Change Color.lightgrey to have a white background - dark theme friendly [#5458](https://github.com/sqlfluff/sqlfluff/pull/5458) [@ryaminal](https://github.com/ryaminal)
 * Fix indentation for single cube clause [#5462](https://github.com/sqlfluff/sqlfluff/pull/5462) [@tunetheweb](https://github.com/tunetheweb)
@@ -612,15 +668,15 @@
 and CI/testing improvements.
 
 This release also sees a bumper crop of new contributors, thanks to
 [@dehume](https://github.com/dehume), [@andychannery](https://github.com/andychannery),
 [@Kylea650](https://github.com/Kylea650), [@robin-alphasophia](https://github.com/robin-alphasophia),
 [@jtbg](https://github.com/jtbg), [@r-petit](https://github.com/r-petit),
 [@bpfaust](https://github.com/bpfaust) & [@freewaydev](https://github.com/freewaydev)
-who all made the first contibutions in this release! 🎉🎉🎉
+who all made the first contributions in this release! 🎉🎉🎉
 
 ## What’s Changed
 
 * Oracle space between alias and column reference [#5313](https://github.com/sqlfluff/sqlfluff/pull/5313) [@joaostorrer](https://github.com/joaostorrer)
 * Don't apply LT05 on templated rebreak locations #5096 [#5318](https://github.com/sqlfluff/sqlfluff/pull/5318) [@alanmcruickshank](https://github.com/alanmcruickshank)
 * Disable JJ01 unless jinja active [#5319](https://github.com/sqlfluff/sqlfluff/pull/5319) [@alanmcruickshank](https://github.com/alanmcruickshank)
 * Cache the `BaseSegment` hash in reflow [#5320](https://github.com/sqlfluff/sqlfluff/pull/5320) [@alanmcruickshank](https://github.com/alanmcruickshank)
@@ -1099,15 +1155,15 @@
 * MySQL: ON UPDATE NOW [#4898](https://github.com/sqlfluff/sqlfluff/pull/4898) [@greg-finley](https://github.com/greg-finley)
 * Support ROLLUP/CUBE in AM06 [#4892](https://github.com/sqlfluff/sqlfluff/pull/4892) [@tunetheweb](https://github.com/tunetheweb)
 
 ## [2.1.1] - 2023-05-25
 
 ## Highlights
 
-This releases fixes a compatability issue with the latest version of dbt. It also ships various dialect improvements.
+This releases fixes a compatibility issue with the latest version of dbt. It also ships various dialect improvements.
 
 ## What’s Changed
 
 * profiles dir env var or default [#4886](https://github.com/sqlfluff/sqlfluff/pull/4886) [@JasonGluck](https://github.com/JasonGluck)
 * Bigquery: Allow empty `struct` in `TO_JSON` [#4879](https://github.com/sqlfluff/sqlfluff/pull/4879) [@dimitris-flyr](https://github.com/dimitris-flyr)
 * Set type of ARRAY function for BigQuery [#4880](https://github.com/sqlfluff/sqlfluff/pull/4880) [@tunetheweb](https://github.com/tunetheweb)
 * Full athena SHOW coverage [#4876](https://github.com/sqlfluff/sqlfluff/pull/4876) [@dogversioning](https://github.com/dogversioning)
@@ -1442,15 +1498,15 @@
 
 ## [2.0.1] - 2023-03-17
 
 ## Highlights
 
 This is mostly a bugfix release addressing some of the issues from the recent
 2.0 release. Notable fixes are:
-- Spacing for (as applied by `LT01`) for datatypes, hypenated identifiers and
+- Spacing for (as applied by `LT01`) for datatypes, hyphenated identifiers and
   casting operators.
 - Several bugs in the indentation routines (`LT02`), in particular with implicit
   indents.
 - Fixing a conflict between `LT09` and `LT02`, by only limiting `LT09` to bringing
   targets onto a single line if there is only one select target **and** that it
   contains no newlines.
 - Supporting arrays, and the new rules configuration more effectively in `pyproject.toml`.
@@ -3393,15 +3449,15 @@
 * Exasol: Overhaul drop statements [#2407](https://github.com/sqlfluff/sqlfluff/pull/2407) [@sti0](https://github.com/sti0)
 * L044, L045: Handle Exasol VALUES clause [#2400](https://github.com/sqlfluff/sqlfluff/pull/2400) [@barrywhart](https://github.com/barrywhart)
 * L060: Use COALESCE instead of IFNULL or NVL. [#2405](https://github.com/sqlfluff/sqlfluff/pull/2405) [@jpy-git](https://github.com/jpy-git)
 * Postgres: Fix Values alias regression [#2401](https://github.com/sqlfluff/sqlfluff/pull/2401) [@jpy-git](https://github.com/jpy-git)
 * Align line length in Python code to 88 characters [#2264](https://github.com/sqlfluff/sqlfluff/pull/2264) [@chwiese](https://github.com/chwiese)
 * Jinja templater: Allow "load_macros_from_path" to be a comma-separated list of paths [#2387](https://github.com/sqlfluff/sqlfluff/pull/2387) [@barrywhart](https://github.com/barrywhart)
 * Add "TRANS" keyword for T-SQL [#2399](https://github.com/sqlfluff/sqlfluff/pull/2399) [@fdw](https://github.com/fdw)
-* Docstrings: Replace double backtics with single quote for lint results. [#2386](https://github.com/sqlfluff/sqlfluff/pull/2386) [@jpy-git](https://github.com/jpy-git)
+* Docstrings: Replace double backticks with single quote for lint results. [#2386](https://github.com/sqlfluff/sqlfluff/pull/2386) [@jpy-git](https://github.com/jpy-git)
 * Spark3: Support for `INSERT OVERWRITE DIRECTORY` statements [#2385](https://github.com/sqlfluff/sqlfluff/pull/2385) [@R7L208](https://github.com/R7L208)
 * Fix unnecessary white underline in doc site [#2383](https://github.com/sqlfluff/sqlfluff/pull/2383) [@tunetheweb](https://github.com/tunetheweb)
 * Rolls back some code cleanup that caused coverage report to show gaps [#2384](https://github.com/sqlfluff/sqlfluff/pull/2384) [@barrywhart](https://github.com/barrywhart)
 * Fix "connection already closed" issue with dbt 1.0 and dbt_utils [#2382](https://github.com/sqlfluff/sqlfluff/pull/2382) [@barrywhart](https://github.com/barrywhart)
 * Spark3: Support for `INSERT [TABLE]` data manipulation statements [#2290](https://github.com/sqlfluff/sqlfluff/pull/2290) [@R7L208](https://github.com/R7L208)
 * Comment out line in bug report template [#2378](https://github.com/sqlfluff/sqlfluff/pull/2378) [@jpy-git](https://github.com/jpy-git)
 * Postgres: EXPLAIN statement updates [#2374](https://github.com/sqlfluff/sqlfluff/pull/2374) [@jpy-git](https://github.com/jpy-git)
@@ -3681,15 +3737,15 @@
 * Fix inline comment interactions with L052 [#2019](https://github.com/sqlfluff/sqlfluff/pull/2019) [@jpy-git](https://github.com/jpy-git)
 * Make Snowflake tags DRY [#1992](https://github.com/sqlfluff/sqlfluff/pull/1992) [@chwiese](https://github.com/chwiese)
 * Rename whitelist/blacklist to allowlist/denylist [#1989](https://github.com/sqlfluff/sqlfluff/pull/1989) [@jpy-git](https://github.com/jpy-git)
 * Fix issue with inline ignores not respecting comment lines [#1985](https://github.com/sqlfluff/sqlfluff/pull/1985) [@jpy-git](https://github.com/jpy-git)
 * Fix L009 FileSegment child + new create_before/create_after edit types [#1979](https://github.com/sqlfluff/sqlfluff/pull/1979) [@jpy-git](https://github.com/jpy-git)
 * Adds extra check to L054 to avoid weird error messages [#1988](https://github.com/sqlfluff/sqlfluff/pull/1988) [@tunetheweb](https://github.com/tunetheweb)
 * BigQuery: Allow keywords in column reference components [#1987](https://github.com/sqlfluff/sqlfluff/pull/1987) [@tunetheweb](https://github.com/tunetheweb)
-* L027: Remove unnessary crawl in get_select_statement_info [#1974](https://github.com/sqlfluff/sqlfluff/pull/1974) [@jpy-git](https://github.com/jpy-git)
+* L027: Remove unnecessary crawl in get_select_statement_info [#1974](https://github.com/sqlfluff/sqlfluff/pull/1974) [@jpy-git](https://github.com/jpy-git)
 * Add __all__ attributes to __init__.py files to resolve F401 [#1949](https://github.com/sqlfluff/sqlfluff/pull/1949) [@jpy-git](https://github.com/jpy-git)
 * Fix incorrect comment on L055 [#1967](https://github.com/sqlfluff/sqlfluff/pull/1967) [@jpy-git](https://github.com/jpy-git)
 * Docs: fix docker hub link to public URL [#1964](https://github.com/sqlfluff/sqlfluff/pull/1964) [@kevinmarsh](https://github.com/kevinmarsh)
 * Fix issue releasing dbt package: tox commands run relative to repo root [#1962](https://github.com/sqlfluff/sqlfluff/pull/1962) [@jpy-git](https://github.com/jpy-git)
 
 ## [0.8.2] - 2021-11-22
 
@@ -4806,15 +4862,15 @@
 
 - Bugfix, default config not included.
 
 ## [0.2.2] - 2019-12-02
 
 ### Changed
 
-- Tweek rule L005 to report more sensibly with newlines.
+- Tweak rule L005 to report more sensibly with newlines.
 - Rework testing of rules to be more modular.
 - Fix a config file bug if no root config file was present for some
   values. Thanks [@barrywhart](https://github.com/barrywhart).
 - Lexing rules are now part of the dialect rather than a
   global so that they can be overridden by other dialects
   when we get to that stage.
```

### Comparing `sqlfluff-3.0.3/LICENSE.md` & `sqlfluff-3.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/PKG-INFO` & `sqlfluff-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.3
+Version: 3.0.4
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -117,14 +117,15 @@
 - [Redshift](https://docs.aws.amazon.com/redshift/index.html)
 - [Snowflake](https://www.snowflake.com/)
 - [SOQL](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm)
 - [SparkSQL](https://spark.apache.org/docs/latest/)
 - [SQLite](https://www.sqlite.org/)
 - [Teradata](https://www.teradata.com/)
 - [Transact-SQL](https://docs.microsoft.com/en-us/sql/t-sql/language-reference) (aka T-SQL)
+- [Trino](https://trino.io/)
 - [Vertica](https://www.vertica.com/)
 
 We aim to make it easy to expand on the support of these dialects and also
 add other, currently unsupported, dialects. Please [raise issues](https://github.com/sqlfluff/sqlfluff/issues)
 (or upvote any existing issues) to let us know of demand for missing support.
 
 Pull requests from those that know the missing syntax or dialects are especially
```

### Comparing `sqlfluff-3.0.3/README.md` & `sqlfluff-3.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 - [Redshift](https://docs.aws.amazon.com/redshift/index.html)
 - [Snowflake](https://www.snowflake.com/)
 - [SOQL](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm)
 - [SparkSQL](https://spark.apache.org/docs/latest/)
 - [SQLite](https://www.sqlite.org/)
 - [Teradata](https://www.teradata.com/)
 - [Transact-SQL](https://docs.microsoft.com/en-us/sql/t-sql/language-reference) (aka T-SQL)
+- [Trino](https://trino.io/)
 - [Vertica](https://www.vertica.com/)
 
 We aim to make it easy to expand on the support of these dialects and also
 add other, currently unsupported, dialects. Please [raise issues](https://github.com/sqlfluff/sqlfluff/issues)
 (or upvote any existing issues) to let us know of demand for missing support.
 
 Pull requests from those that know the missing syntax or dialects are especially
```

### Comparing `sqlfluff-3.0.3/pyproject.toml` & `sqlfluff-3.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sqlfluff"
-version = "3.0.3"
+version = "3.0.4"
 description = "The SQL Linter for Humans"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
   {name = "Alan Cruickshank", email = "alan@designingoverload.com"},
 ]
 license = {file = "LICENSE.md"}
@@ -125,15 +125,15 @@
 sqlfluff_rules_convention = "sqlfluff.rules.convention"
 sqlfluff_rules_jinja = "sqlfluff.rules.jinja"
 sqlfluff_rules_tsql = "sqlfluff.rules.tsql"
 
 
 [tool.sqlfluff_docs]
 # NOTE: Stable version is used by docs/conf.py
-stable_version = "3.0.3"
+stable_version = "3.0.4"
 
 
 [tool.setuptools.package-data]
 sqlfluff = ["core/default_config.cfg", "py.typed"]
 
 
 [tool.importlinter]
@@ -160,15 +160,15 @@
     "sqlfluff.api",
 ]
 forbidden_modules = [
     "sqlfluff.cli",
 ]
 
 [[tool.importlinter.contracts]]
-name = "Helper methods must be internally indepentent"
+name = "Helper methods must be internally independent"
 type = "independence"
 modules = [
     "sqlfluff.core.helpers.string",
     "sqlfluff.core.helpers.slice",
     "sqlfluff.core.helpers.dict",
 ]
 
@@ -249,7 +249,32 @@
     "rules_suite: Marks the suite of rules tests. Also known as the yaml tests (part of integration).",
 ]
 
 
 [tool.doc8]
 # Ignore auto-generated docs
 ignore-path = "docs/source/partials/"
+
+
+[tool.codespell]
+# The configuration must be kept here to ensure that
+# `codespell` can be run as a standalone program from the CLI
+# with the appropriate default options.
+
+skip = "*/test/fixtures/*,*/.*,*/pyproject.toml"
+
+check-hidden = true
+quiet-level=2
+# ignore-regex = '\\[fnrstv]'
+builtin = "clear,rare,informal,names"
+
+ignore-words-list = "fo,ws,falsy,coo,inout,deque,crate,trough,ro,mange,identifers,statment"
+
+# ignore-words = "dev/tools/codespell/codespell-ignore.txt"
+# exclude-file = "dev/tools/codespell/codespell-lines-ignore.txt"
+uri-ignore-words-list="crate"
+
+# For future reference: it is not currently possible to specify
+# the standard dictionary and the custom dictionary in the configuration
+# file
+#  D = "-"
+#  dictionary = "dev/tools/codespell/codespell-dict.txt"
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/api/simple.py` & `sqlfluff-3.0.4/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-3.0.4/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/cli/commands.py` & `sqlfluff-3.0.4/src/sqlfluff/cli/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,16 @@
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         if exc_type is SQLFluffUserError:
             click.echo(
                 "\nUser Error: "
                 + self.formatter.colorize(
                     str(exc_val),
                     Color.red,
-                )
+                ),
+                err=True,
             )
             sys.exit(EXIT_ERROR)
 
 
 def common_options(f: Callable) -> Callable:
     """Add common options to commands via a decorator.
 
@@ -1078,30 +1079,31 @@
                 "The -f/--force option is deprecated as it is now the "
                 "default behaviour.",
                 Color.red,
             ),
             err=True,
         )
 
-    # handle stdin case. should output formatted sql to stdout and nothing else.
-    if fixing_stdin:
-        _stdin_fix(lnt, formatter, fix_even_unparsable)
-    else:
-        _paths_fix(
-            lnt,
-            formatter,
-            paths,
-            processes,
-            fix_even_unparsable,
-            fixed_suffix,
-            bench,
-            show_lint_violations,
-            check=check,
-            persist_timing=persist_timing,
-        )
+    with PathAndUserErrorHandler(formatter):
+        # handle stdin case. should output formatted sql to stdout and nothing else.
+        if fixing_stdin:
+            _stdin_fix(lnt, formatter, fix_even_unparsable)
+        else:
+            _paths_fix(
+                lnt,
+                formatter,
+                paths,
+                processes,
+                fix_even_unparsable,
+                fixed_suffix,
+                bench,
+                show_lint_violations,
+                check=check,
+                persist_timing=persist_timing,
+            )
 
 
 @cli.command(name="format")
 @common_options
 @core_options
 @lint_options
 @click.option(
@@ -1176,29 +1178,30 @@
     set_logging_level(
         verbosity=verbose,
         formatter=formatter,
         logger=logger,
         stderr_output=fixing_stdin,
     )
 
-    # handle stdin case. should output formatted sql to stdout and nothing else.
-    if fixing_stdin:
-        _stdin_fix(lnt, formatter, fix_even_unparsable=False)
-    else:
-        _paths_fix(
-            lnt,
-            formatter,
-            paths,
-            processes,
-            fix_even_unparsable=False,
-            fixed_suffix=fixed_suffix,
-            bench=bench,
-            show_lint_violations=False,
-            persist_timing=persist_timing,
-        )
+    with PathAndUserErrorHandler(formatter):
+        # handle stdin case. should output formatted sql to stdout and nothing else.
+        if fixing_stdin:
+            _stdin_fix(lnt, formatter, fix_even_unparsable=False)
+        else:
+            _paths_fix(
+                lnt,
+                formatter,
+                paths,
+                processes,
+                fix_even_unparsable=False,
+                fixed_suffix=fixed_suffix,
+                bench=bench,
+                show_lint_violations=False,
+                persist_timing=persist_timing,
+            )
 
 
 def quoted_presenter(dumper, data):
     """Re-presenter which always double quotes string values needing escapes."""
     if "\n" in data or "\t" in data or "'" in data:
         return dumper.represent_scalar("tag:yaml.org,2002:str", data, style='"')
     else:
@@ -1415,25 +1418,25 @@
             raw_sql = sys.stdin.read()
             fname = "stdin"
             file_config = lnt.config
         else:
             raw_sql, file_config, _ = lnt.load_raw_file_and_config(path, lnt.config)
             fname = path
 
-    # Get file specific config
-    file_config.process_raw_file_for_config(raw_sql, fname)
-    rendered = lnt.render_string(raw_sql, fname, file_config, "utf8")
-
-    if rendered.templater_violations:
-        for v in rendered.templater_violations:
-            click.echo(formatter.format_violation(v))
-        sys.exit(EXIT_FAIL)
-    else:
-        click.echo(rendered.templated_file.templated_str)
-        sys.exit(EXIT_SUCCESS)
+        # Get file specific config
+        file_config.process_raw_file_for_config(raw_sql, fname)
+        rendered = lnt.render_string(raw_sql, fname, file_config, "utf8")
+
+        if rendered.templater_violations:
+            for v in rendered.templater_violations:
+                click.echo(formatter.format_violation(v))
+            sys.exit(EXIT_FAIL)
+        else:
+            click.echo(rendered.templated_file.templated_str)
+            sys.exit(EXIT_SUCCESS)
 
 
 # This "__main__" handler allows invoking SQLFluff using "python -m", which
 # simplifies the use of cProfile, e.g.:
 # python -m cProfile -s cumtime -m sqlfluff.cli.commands lint slow_file.sql
 if __name__ == "__main__":
     cli.main(sys.argv[1:])  # pragma: no cover
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/cli/formatters.py` & `sqlfluff-3.0.4/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/cli/helpers.py` & `sqlfluff-3.0.4/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/cli/outputstream.py` & `sqlfluff-3.0.4/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/config.py` & `sqlfluff-3.0.4/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/default_config.cfg` & `sqlfluff-3.0.4/src/sqlfluff/core/default_config.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 exclude_rules = None
 # Below controls SQLFluff output, see max_line_length for SQL output
 output_line_length = 80
 # Number of passes to run before admitting defeat
 runaway_limit = 10
 # Ignore errors by category (one or more of the following, separated by commas: lexing,linting,parsing,templating)
 ignore = None
-# Warn only for rule codes (one of more rule codes, seperated by commas: e.g. LT01,LT02)
+# Warn only for rule codes (one of more rule codes, separated by commas: e.g. LT01,LT02)
 # Also works for templating and parsing errors by using TMP or PRS
 warnings = None
 # Whether to warn about unneeded '-- noqa:' comments.
 warn_unused_ignores = False
 # Ignore linting errors found within sections of code coming directly from
 # templated code (e.g. from within Jinja curly braces. Note that it does not
 # ignore errors from literal code found within template loops.
@@ -63,15 +63,15 @@
 indented_ctes = False
 indented_using_on = True
 indented_on_contents = True
 indented_then = True
 indented_then_contents = True
 allow_implicit_indents = False
 template_blocks_indent = True
-# This is a comma seperated list of elements to skip
+# This is a comma separated list of elements to skip
 # indentation edits to.
 skip_indentation_in = script_content
 # If comments are found at the end of long lines, we default to moving
 # them to the line _before_ their current location as the convention is
 # that a comment precedes the line it describes. However if you prefer
 # comments moved _after_, this configuration setting can be set to "after".
 trailing_comments = before
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/dialects/base.py` & `sqlfluff-3.0.4/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/dialects/common.py` & `sqlfluff-3.0.4/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/enums.py` & `sqlfluff-3.0.4/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/errors.py` & `sqlfluff-3.0.4/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/helpers/dict.py` & `sqlfluff-3.0.4/src/sqlfluff/core/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/helpers/file.py` & `sqlfluff-3.0.4/src/sqlfluff/core/helpers/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/helpers/slice.py` & `sqlfluff-3.0.4/src/sqlfluff/core/helpers/slice.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/helpers/string.py` & `sqlfluff-3.0.4/src/sqlfluff/core/helpers/string.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/common.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/fix.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/linter.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/patch.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/patch.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/linter/runner.py` & `sqlfluff-3.0.4/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/context.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         n_matches = 0
         # Keep track of the number of times each option has been matched.
         option_counter = {elem.cache_key(): 0 for elem in self._elements}
         # Keep track of how far we've got.
         matched_idx = idx
         # The working index is to cover non-code elements which aren't
         # claimed yet, but we should conditionally claim if the next
-        # match is succesful.
+        # match is successful.
         working_idx = idx
         matched = MatchResult.empty_at(idx)
         max_idx = len(segments)  # What is the limit
 
         if self.parse_mode == ParseMode.GREEDY:
             max_idx = trim_to_terminator(
                 segments,
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/markers.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/match_algorithms.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/match_algorithms.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/match_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/parser.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             return None
 
         # NOTE: This is the only time we use the parse context not in the
         # context of a context manager. That's because it's the initial
         # instantiation.
         ctx = ParseContext.from_config(config=self.config)
         # Kick off parsing with the root segment. The BaseFileSegment has
-        # a unique entry point to facilitate exaclty this. All other segments
+        # a unique entry point to facilitate exactly this. All other segments
         # will use the standard .match() route.
         root = self.RootSegment.root_parse(
             tuple(segments), fname=fname, parse_context=ctx
         )
 
         # Basic Validation, that we haven't dropped anything.
         check_still_complete(tuple(segments), (root,), ())
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/parsers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/bracketed.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/bracketed.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/common.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/file.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/keyword.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/keyword.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/raw.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/parser/types.py` & `sqlfluff-3.0.4/src/sqlfluff/core/parser/types.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-3.0.4/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/plugin/host.py` & `sqlfluff-3.0.4/src/sqlfluff/core/plugin/host.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-3.0.4/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/base.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/config_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,17 +56,18 @@
         "definition": "Types of quoted identifiers to flag violations for.",
     },
     "capitalisation_policy": {
         "validation": ["consistent", "upper", "lower", "capitalise"],
         "definition": "The capitalisation policy to enforce.",
     },
     "extended_capitalisation_policy": {
-        "validation": ["consistent", "upper", "lower", "pascal", "capitalise"],
+        "validation": ["consistent", "upper", "lower", "pascal", "capitalise", "snake"],
         "definition": (
-            "The capitalisation policy to enforce, extended with PascalCase. "
+            "The capitalisation policy to enforce, extended with PascalCase "
+            "and snake_case. "
             "This is separate from ``capitalisation_policy`` as it should not be "
             "applied to keywords."
         ),
     },
     "select_clause_trailing_comma": {
         "validation": ["forbid", "require"],
         "definition": (
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/context.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/fix.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/loader.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/noqa.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/noqa.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/rules/reference.py` & `sqlfluff-3.0.4/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/base.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/python.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/core/timing.py` & `sqlfluff-3.0.4/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,14 +410,15 @@
     ),
     OrReplaceGrammar=Sequence("OR", "REPLACE"),
     TemporaryTransientGrammar=OneOf("TRANSIENT", Ref("TemporaryGrammar")),
     TemporaryGrammar=OneOf("TEMP", "TEMPORARY"),
     IfExistsGrammar=Sequence("IF", "EXISTS"),
     IfNotExistsGrammar=Sequence("IF", "NOT", "EXISTS"),
     LikeGrammar=OneOf("LIKE", "RLIKE", "ILIKE"),
+    PatternMatchingGrammar=Nothing(),
     UnionGrammar=Sequence("UNION", OneOf("DISTINCT", "ALL", optional=True)),
     IsClauseGrammar=OneOf(
         Ref("NullLiteralSegment"),
         Ref("NanLiteralSegment"),
         Ref("BooleanLiteralGrammar"),
     ),
     InOperatorGrammar=Sequence(
@@ -1224,15 +1225,15 @@
     match_grammar: Matchable = Sequence(
         Ref("SignedSegmentGrammar"),
         Ref("NumericLiteralSegment"),
     )
 
 
 class AggregateOrderByClause(BaseSegment):
-    """An order by clause for an aggregate fucntion.
+    """An order by clause for an aggregate function.
 
     Defined as a class to allow a specific type for rule AM06
     """
 
     type = "aggregate_order_by"
     match_grammar: Matchable = Ref("OrderByClauseSegment")
 
@@ -1761,14 +1762,22 @@
         ),
         Dedent,
         terminators=[Ref("SelectClauseTerminatorGrammar")],
         parse_mode=ParseMode.GREEDY_ONCE_STARTED,
     )
 
 
+class MatchConditionSegment(BaseSegment):
+    """A stub segment to be used in Snowflake ASOF joins."""
+
+    type = "match_condition"
+
+    match_grammar: Matchable = Nothing()
+
+
 class JoinClauseSegment(BaseSegment):
     """Any number of join clauses, including the `JOIN` keyword."""
 
     type = "join_clause"
     match_grammar: Matchable = OneOf(
         # NB These qualifiers are optional
         Sequence(
@@ -1779,14 +1788,15 @@
             AnyNumberOf(Ref("NestedJoinGrammar")),
             Dedent,
             Sequence(
                 # Using nested sequence here so we only get the indents
                 # if we also have content.
                 Conditional(Indent, indented_using_on=True),
                 # NB: this is optional
+                Ref("MatchConditionSegment", optional=True),
                 OneOf(
                     # ON clause
                     Ref("JoinOnConditionSegment"),
                     # USING clause
                     Ref("JoinUsingConditionGrammar"),
                     # Unqualified joins *are* allowed. They just might not
                     # be a good idea.
@@ -1797,14 +1807,15 @@
         ),
         # Note NATURAL joins do not support Join conditions
         Sequence(
             Ref("UnconditionalJoinKeywordsGrammar"),
             Ref("JoinKeywordsGrammar"),
             Indent,
             Ref("FromExpressionElementSegment"),
+            Ref("MatchConditionSegment", optional=True),
             Dedent,
         ),
         # Sometimes, a natural join might already include the keyword
         Sequence(
             Ref("ExtendedNaturalJoinKeywordsGrammar"),
             Indent,
             Ref("FromExpressionElementSegment"),
@@ -1996,15 +2007,19 @@
                 optional=True,
                 reset_terminators=True,
                 terminators=[Ref.keyword("END")],
             ),
             Dedent,
             "END",
         ),
-        terminators=[Ref("CommaSegment"), Ref("BinaryOperatorGrammar")],
+        terminators=[
+            Ref("ComparisonOperatorGrammar"),
+            Ref("CommaSegment"),
+            Ref("BinaryOperatorGrammar"),
+        ],
     )
 
 
 ansi_dialect.add(
     # Expression_A_Grammar
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.html#a_expr
     # The upstream grammar is defined recursively, which if implemented naively
@@ -2080,14 +2095,18 @@
                 Sequence(
                     Ref.keyword("NOT", optional=True),
                     "BETWEEN",
                     Ref("Expression_B_Grammar"),
                     "AND",
                     Ref("Tail_Recurse_Expression_A_Grammar"),
                 ),
+                Sequence(
+                    Ref("PatternMatchingGrammar"),
+                    Ref("Expression_A_Grammar"),
+                ),
             )
         ),
     ),
     # Expression_B_Grammar: Does not directly feed into Expression_A_Grammar
     # but is used for a BETWEEN statement within Expression_A_Grammar.
     # https://www.cockroachlabs.com/docs/v20.2/sql-grammar.htm#b_expr
     #
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,15 +867,15 @@
         ),
         # Base function name
         OneOf(
             Ref("FunctionNameIdentifierSegment"),
             Ref("QuotedIdentifierSegment"),
             terminators=[Ref("BracketedSegment")],
         ),
-        # BigQuery allows whitespaces between the `.` of a function refrence or
+        # BigQuery allows whitespaces between the `.` of a function reference or
         # SAFE prefix. Keeping the explicit `allow_gaps=True` here to
         # make the distinction from `ansi.FunctionNameSegment` clear.
         allow_gaps=True,
     )
 
 
 class FunctionSegment(ansi.FunctionSegment):
@@ -1521,14 +1521,23 @@
         Ref("SingleIdentifierGrammar"),  # Column name
         Ref("DatatypeSegment"),  # Column type
         AnyNumberOf(Ref("ColumnConstraintSegment")),
         Ref("OptionsSegment", optional=True),
     )
 
 
+class ViewColumnDefinitionSegment(ansi.ColumnDefinitionSegment):
+    """A column definition, for view_column_name_list of CREATE VIEW statement."""
+
+    match_grammar: Matchable = Sequence(
+        Ref("SingleIdentifierGrammar"),  # Column name
+        Ref("OptionsSegment", optional=True),
+    )
+
+
 class CreateTableStatementSegment(ansi.CreateTableStatementSegment):
     """`CREATE TABLE` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_table_statement
     """
 
     match_grammar = Sequence(
@@ -1707,15 +1716,20 @@
     match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         "VIEW",
         Ref("IfNotExistsGrammar", optional=True),
         Ref("TableReferenceSegment"),
         # Optional list of column names
-        Ref("BracketedColumnReferenceListGrammar", optional=True),
+        Bracketed(
+            Delimited(
+                Ref("ViewColumnDefinitionSegment"),
+            ),
+            optional=True,
+        ),
         Ref("OptionsSegment", optional=True),
         "AS",
         OptionallyBracketed(Ref("SelectableGrammar")),
     )
 
 
 class AlterViewStatementSegment(BaseSegment):
@@ -1986,15 +2000,15 @@
 
 
 class MergeNotMatchedBySourceClauseSegment(ansi.MergeMatchedClauseSegment):
     """The `WHEN MATCHED BY SOURCE` clause within a `MERGE` statement.
 
     It inherits from `ansi.MergeMatchedClauseSegment` because NotMatchedBySource clause
     is conceptionally more close to a Matched clause than to NotMatched clause, i.e.
-    it get's combined with an UPDATE or DELETE, not with an INSERT.
+    it gets combined with an UPDATE or DELETE, not with an INSERT.
     """
 
     type = "merge_when_matched_clause"
     match_grammar: Matchable = Sequence(
         "WHEN",
         "NOT",
         "MATCHED",
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,60 @@
                 "KEYS",
             ),
         ),
         Dedent,
     )
 
 
+class WildcardExpressionSegment(ansi.WildcardExpressionSegment):
+    """An extension of the star expression for Clickhouse."""
+
+    match_grammar = ansi.WildcardExpressionSegment.match_grammar.copy(
+        insert=[
+            Ref("ExceptClauseSegment", optional=True),
+        ]
+    )
+
+
+class ExceptClauseSegment(BaseSegment):
+    """A Clickhouse SELECT EXCEPT clause.
+
+    https://clickhouse.com/docs/en/sql-reference/statements/select#except
+    """
+
+    type = "select_except_clause"
+    match_grammar = Sequence(
+        "EXCEPT",
+        OneOf(
+            Bracketed(Delimited(Ref("SingleIdentifierGrammar"))),
+            Ref("SingleIdentifierGrammar"),
+        ),
+    )
+
+
+class SelectClauseModifierSegment(ansi.SelectClauseModifierSegment):
+    """Things that come after SELECT but before the columns.
+
+    Overridden from ANSI to allow DISTINCT ON ()
+    https://clickhouse.com/docs/en/sql-reference/statements/select/distinct
+    """
+
+    match_grammar = OneOf(
+        Sequence(
+            "DISTINCT",
+            Sequence(
+                "ON",
+                Bracketed(Delimited(Ref("ExpressionSegment"))),
+                optional=True,
+            ),
+        ),
+        "ALL",
+    )
+
+
 class FromExpressionElementSegment(ansi.FromExpressionElementSegment):
     """A table expression.
 
     Overridden from ANSI to allow FINAL modifier.
     https://clickhouse.com/docs/en/sql-reference/statements/select/from#final-modifier
     """
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "DISTRIBUTED",
     "DROP",
     "ELSE",
     "END",
     "ENGINE",
     "EPHEMERAL",
     "EVENTS",
+    "EXCEPT",
     "EXISTS",
     "EXPLAIN",
     "EXPRESSION",
     "EXTRACT",
     "FETCHES",
     "FILE",
     "FILESYSTEM",
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 
 class CreateTableStatementSegment(postgres.CreateTableStatementSegment):
     """A `CREATE TABLE` statement.
 
     As specified in
     https://docs.vmware.com/en/VMware-Tanzu-Greenplum/6/greenplum-database/GUID-ref_guide-sql_commands-CREATE_TABLE.html
-    This is overriden from Postgres to add the `DISTRIBUTED` clause.
+    This is overridden from Postgres to add the `DISTRIBUTED` clause.
     """
 
     match_grammar = Sequence(
         "CREATE",
         OneOf(
             Sequence(
                 OneOf("GLOBAL", "LOCAL", optional=True),
@@ -255,15 +255,15 @@
 
 
 class CreateTableAsStatementSegment(postgres.CreateTableAsStatementSegment):
     """A `CREATE TABLE AS` statement.
 
     As specified in
     https://docs.vmware.com/en/VMware-Tanzu-Greenplum/6/greenplum-database/GUID-ref_guide-sql_commands-CREATE_TABLE_AS.html
-    This is overriden from Postgres to add the `DISTRIBUTED` clause.
+    This is overridden from Postgres to add the `DISTRIBUTED` clause.
     """
 
     match_grammar = Sequence(
         "CREATE",
         OneOf(
             Sequence(
                 OneOf("GLOBAL", "LOCAL", optional=True),
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_greenplum_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 ansi_dialect = load_raw_dialect("ansi")
 mysql_dialect = ansi_dialect.copy_as("mysql")
 
 mysql_dialect.patch_lexer_matchers(
     [
         RegexLexer(
             "inline_comment",
-            r"(-- |#)[^\n]*",
+            r"(^--|-- |#)[^\n]*",
             CommentSegment,
-            segment_kwargs={"trim_start": ("-- ", "#")},
+            segment_kwargs={"trim_start": ("--", "#")},
         ),
         # Pattern breakdown:
         # (?s)                     DOTALL (dot matches newline)
         #     (                    group1 start
         #         '                single quote (start)
         #         (?:              non-capturing group: begin
         #             \\'          MySQL escaped single-quote
@@ -1771,34 +1771,19 @@
 
 class CallStoredProcedureSegment(BaseSegment):
     """This is a CALL statement used to execute a stored procedure.
 
     https://dev.mysql.com/doc/refman/8.0/en/call.html
     """
 
-    type = "call_segment"
+    type = "call_statement"
 
     match_grammar = Sequence(
         "CALL",
-        OneOf(
-            Ref("SingleIdentifierGrammar"),
-            Ref("QuotedIdentifierSegment"),
-        ),
-        Bracketed(
-            AnyNumberOf(
-                Delimited(
-                    Ref("QuotedLiteralSegment"),
-                    Ref("NumericLiteralSegment"),
-                    Ref("DoubleQuotedLiteralSegment"),
-                    Ref("SessionVariableNameSegment"),
-                    Ref("LocalVariableNameSegment"),
-                    Ref("FunctionSegment"),
-                ),
-            ),
-        ),
+        Ref("FunctionSegment"),
     )
 
 
 class SelectPartitionClauseSegment(BaseSegment):
     """This is the body of a partition clause."""
 
     type = "partition_clause"
@@ -2641,15 +2626,15 @@
     match_grammar = Sequence(
         Ref.keyword("DEFAULT", optional=True),
         OneOf(
             Sequence(
                 "CHARACTER",
                 "SET",
                 Ref("EqualsSegment", optional=True),
-                Ref("NakedIdentifierSegment"),
+                OneOf(Ref("NakedIdentifierSegment"), Ref("QuotedLiteralSegment")),
             ),
             Sequence(
                 "COLLATE",
                 Ref("EqualsSegment", optional=True),
                 Ref("CollationReferenceSegment"),
             ),
             Sequence(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -772,15 +772,15 @@
         "START",
         "WITH",
         Ref("ExpressionSegment"),
     )
 
 
 class HierarchicalQueryClauseSegment(BaseSegment):
-    """Hiearchical Query.
+    """Hierarchical Query.
 
     https://docs.oracle.com/en/database/oracle/oracle-database/21/sqlrf/Hierarchical-Queries.html
     """
 
     type = "hierarchical_query_clause"
 
     match_grammar: Matchable = OneOf(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,14 +863,19 @@
                     "INT8RANGE",
                     "NUMRANGE",
                     "TSRANGE",
                     "TSTZRANGE",
                     "DATERANGE",
                     # pg_lsn type
                     "PG_LSN",
+                    # pgvector types
+                    Sequence(
+                        "VECTOR",
+                        Ref("BracketedArguments", optional=True),
+                    ),
                 ),
             ),
             # user defined data types
             Ref("DatatypeIdentifierSegment"),
         ),
         # array types
         OneOf(
@@ -1506,14 +1511,19 @@
                         Ref("UpdateStatementSegment"),
                         Ref("SemicolonSegment"),
                     ),
                     Sequence(
                         Ref("SelectStatementSegment"),
                         Ref("SemicolonSegment"),
                     ),
+                    Sequence(
+                        "RETURN",
+                        Ref("ExpressionSegment"),
+                        Ref("SemicolonSegment"),
+                    ),
                 ),
                 "END",
             ),
         ),
         Sequence(
             "WITH",
             Bracketed(Delimited(Ref("ParameterNameSegment"))),
@@ -2573,15 +2583,15 @@
 class PublicationObjectsSegment(BaseSegment):
     """Specification for one or more objects in a publication.
 
     Unlike the underlying PG grammar which has one object per PublicationObjSpec and
     so requires one to track the previous object type if it's a "continuation object
     type", this grammar groups together the continuation objects, e.g.
     "TABLE a, b, TABLE c, d" results in two segments: one containing references
-    "a, b", and the other contianing "c, d".
+    "a, b", and the other containing "c, d".
 
     https://www.postgresql.org/docs/15/sql-createpublication.html
     https://github.com/postgres/postgres/blob/4380c2509d51febad34e1fac0cfaeb98aaa716c5/src/backend/parser/gram.y#L10435-L10530
     """
 
     type = "publication_objects"
     match_grammar: Matchable = OneOf(
@@ -4245,15 +4255,15 @@
         Ref("IfExistsGrammar", optional=True),
         Delimited(Ref("SequenceReferenceSegment")),
         Ref("DropBehaviorGrammar", optional=True),
     )
 
 
 class StatisticsReferenceSegment(ansi.ObjectReferenceSegment):
-    """Statics Reference."""
+    """Statistics Reference."""
 
     type = "statistics_reference"
 
 
 class CreateStatisticsStatementSegment(BaseSegment):
     """Create Statistics Segment.
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1024,13 +1024,18 @@
 
 postgres_postgis_other_keywords = [
     ("GEOMETRY", "non-reserved"),
     ("GEOGRAPHY", "non-reserved"),
     ("EMPTY", "non-reserved"),
 ]
 
+postgres_pgvector_keywords = [
+    ("VECTOR", "non-reserved"),
+]
+
 postgres_keywords = priority_keyword_merge(
     postgres_docs_keywords,
     postgres_nondocs_keywords,
     postgres_postgis_datatype_keywords,
     postgres_postgis_other_keywords,
+    postgres_pgvector_keywords,
 )
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -1839,15 +1839,15 @@
 
 
 class GrantUsageDatashareStatementSegment(BaseSegment):
     """A `GRANT DATASHARES` statement.
 
     https://docs.aws.amazon.com/redshift/latest/dg/r_GRANT.html
     section "Granting datashare permissions"
-    Note: According to docummentation, multiple accounts and namespaces can be
+    Note: According to documentation, multiple accounts and namespaces can be
           specified. However, tests using redshift instance showed this causes a syntax
           error.
     """
 
     type = "grant_datashare_statement"
     match_grammar = Sequence(
         OneOf("GRANT", "REVOKE"),
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,14 +189,24 @@
 snowflake_dialect.sets("warehouse_scaling_policies").update(
     [
         "STANDARD",
         "ECONOMY",
     ],
 )
 
+snowflake_dialect.sets("refreshmode_types").clear()
+snowflake_dialect.sets("refreshmode_types").update(
+    ["AUTO", "FULL", "INCREMENTAL"],
+)
+
+snowflake_dialect.sets("initialize_types").clear()
+snowflake_dialect.sets("initialize_types").update(
+    ["ON_CREATE", "ON_SCHEDULE"],
+)
+
 snowflake_dialect.add(
     # In snowflake, these are case sensitive even though they're not quoted
     # so they need a different `name` and `type` so they're not picked up
     # by other rules.
     ParameterAssignerSegment=StringParser(
         "=>", SymbolSegment, type="parameter_assigner"
     ),
@@ -268,14 +278,27 @@
         ),
         MultiStringParser(
             [f"'{size}'" for size in snowflake_dialect.sets("warehouse_sizes")],
             CodeSegment,
             type="warehouse_size",
         ),
     ),
+    RefreshModeType=OneOf(
+        MultiStringParser(
+            snowflake_dialect.sets("refreshmode_types"),
+            KeywordSegment,
+        )
+    ),
+    InitializeType=OneOf(
+        MultiStringParser(
+            snowflake_dialect.sets("initialize_types"),
+            KeywordSegment,
+            type="initialize_type",
+        )
+    ),
     CompressionType=OneOf(
         MultiStringParser(
             snowflake_dialect.sets("compression_types"),
             KeywordSegment,
             type="compression_type",
         ),
         MultiStringParser(
@@ -693,14 +716,21 @@
         Sequence("ORDER", "BY"),
         "LIMIT",
         "QUALIFY",
         "WINDOW",
         "FETCH",
         "OFFSET",
     ),
+    NonStandardJoinTypeKeywordsGrammar=OneOf("ASOF"),
+    UnconditionalJoinKeywordsGrammar=OneOf(
+        Ref("NaturalJoinKeywordsGrammar"),
+        Ref("UnconditionalCrossJoinKeywordsGrammar"),
+        Ref("HorizontalJoinKeywordsGrammar"),
+        Ref("NonStandardJoinTypeKeywordsGrammar"),
+    ),
 )
 
 # Add all Snowflake keywords
 snowflake_dialect.sets("unreserved_keywords").clear()
 snowflake_dialect.update_keywords_set_from_multiline_string(
     "unreserved_keywords", snowflake_unreserved_keywords
 )
@@ -1241,28 +1271,31 @@
             Ref("AlterSessionStatementSegment"),
             Ref("AlterTaskStatementSegment"),
             Ref("SetAssignmentStatementSegment"),
             Ref("CallStoredProcedureSegment"),
             Ref("MergeStatementSegment"),
             Ref("CopyIntoTableStatementSegment"),
             Ref("CopyIntoLocationStatementSegment"),
+            Ref("CopyFilesIntoLocationStatementSegment"),
             Ref("FormatTypeOptions"),
             Ref("AlterWarehouseStatementSegment"),
             Ref("AlterShareStatementSegment"),
             Ref("CreateExternalTableSegment"),
             Ref("AlterExternalTableStatementSegment"),
             Ref("CreateSchemaStatementSegment"),
             Ref("AlterSchemaStatementSegment"),
             Ref("CreateFunctionStatementSegment"),
             Ref("AlterFunctionStatementSegment"),
             Ref("CreateExternalFunctionStatementSegment"),
             Ref("CreateStageSegment"),
             Ref("AlterStageSegment"),
             Ref("CreateStreamStatementSegment"),
+            Ref("CreateStreamlitStatementSegment"),
             Ref("AlterStreamStatementSegment"),
+            Ref("AlterStreamlitStatementSegment"),
             Ref("UnsetStatementSegment"),
             Ref("UndropStatementSegment"),
             Ref("CommentStatementSegment"),
             Ref("CallStatementSegment"),
             Ref("AlterViewStatementSegment"),
             Ref("AlterMaterializedViewStatementSegment"),
             Ref("DropProcedureStatementSegment"),
@@ -1381,14 +1414,22 @@
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/arrays#flattening_arrays
         Sequence("WITH", "OFFSET", Ref("AliasExpressionSegment"), optional=True),
         Ref("SamplingExpressionSegment", optional=True),
         Ref("PostTableExpressionGrammar", optional=True),
     )
 
 
+class MatchConditionSegment(ansi.MatchConditionSegment):
+    """A match condition for an ASOF join."""
+
+    type = "match_condition"
+
+    match_grammar = Sequence("MATCH_CONDITION", Bracketed(Ref("ExpressionSegment")))
+
+
 class PatternSegment(BaseSegment):
     """A `PATTERN` expression.
 
     https://docs.snowflake.com/en/sql-reference/constructs/match_recognize.html
     """
 
     type = "pattern_expression"
@@ -2617,14 +2658,15 @@
         "VIEW",
         "STAGE",
         "FUNCTION",
         "PROCEDURE",
         "ROUTINE",
         "SEQUENCE",
         "STREAM",
+        "STREAMLIT",
         "TASK",
         "PIPE",
     ]
 
     _schema_object_types = OneOf(
         *_schema_object_names,
         Sequence("MATERIALIZED", "VIEW"),
@@ -2870,14 +2912,15 @@
 
     type = "create_procedure_statement"
     match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         Sequence("SECURE", optional=True),
         "PROCEDURE",
+        Ref("IfNotExistsGrammar", optional=True),
         Ref("FunctionNameSegment"),
         Ref("FunctionParameterListGrammar"),
         Sequence("COPY", "GRANTS", optional=True),
         "RETURNS",
         OneOf(
             Ref("DatatypeSegment"),
             Sequence(
@@ -3096,15 +3139,15 @@
     type = "scripting_let_statement"
     match_grammar = OneOf(
         # Initial declaration and assignment
         Sequence(
             "LET",
             Ref("LocalVariableNameSegment"),
             OneOf(
-                # Variable assigment
+                # Variable assignment
                 OneOf(
                     Sequence(
                         Ref("DatatypeSegment"),
                         OneOf("DEFAULT", Ref("WalrusOperatorSegment")),
                         Ref("ExpressionSegment"),
                     ),
                     Sequence(
@@ -3843,14 +3886,15 @@
 
 
 class CreateTableStatementSegment(ansi.CreateTableStatementSegment):
     """A `CREATE TABLE` statement.
 
     A lot more options than ANSI
     https://docs.snowflake.com/en/sql-reference/sql/create-table.html
+    https://docs.snowflake.com/en/sql-reference/sql/create-dynamic-table
     """
 
     match_grammar = Sequence(
         "CREATE",
         Ref("OrReplaceGrammar", optional=True),
         Ref("TemporaryTransientGrammar", optional=True),
         Ref.keyword("DYNAMIC", optional=True),
@@ -3860,14 +3904,26 @@
         Sequence(
             "TARGET_LAG",
             Ref("EqualsSegment"),
             Ref("QuotedLiteralSegment"),
             optional=True,
         ),
         Sequence(
+            "REFRESH_MODE",
+            Ref("EqualsSegment"),
+            Ref("RefreshModeType"),
+            optional=True,
+        ),
+        Sequence(
+            "INITIALIZE",
+            Ref("EqualsSegment"),
+            Ref("InitializeType"),
+            optional=True,
+        ),
+        Sequence(
             "WAREHOUSE",
             Ref("EqualsSegment"),
             Ref("ObjectReferenceSegment"),
             optional=True,
         ),
         # Columns and comment syntax:
         AnySetOf(
@@ -4500,14 +4556,15 @@
                                         )
                                     ),
                                 ),
                                 optional=True,
                             ),
                             optional=True,
                         ),
+                        Ref("TagBracketedEqualsSegment", optional=True),
                         Ref("CommentClauseSegment", optional=True),
                     ),
                 ),
             ),
             Sequence(
                 Ref.keyword("WITH", optional=True),
                 "ROW",
@@ -4518,15 +4575,14 @@
                 Bracketed(
                     Delimited(Ref("ColumnReferenceSegment")),
                 ),
             ),
             Ref("TagBracketedEqualsSegment"),
             Sequence("COPY", "GRANTS"),
             Ref("CommentEqualsClauseSegment"),
-            # @TODO: Support column-level masking policy & tagging.
         ),
         "AS",
         OptionallyBracketed(Ref("SelectableGrammar")),
     )
 
 
 class AlterViewStatementSegment(BaseSegment):
@@ -5488,14 +5544,50 @@
             Ref("EqualsSegment"),
             Ref("ValidationModeOptionSegment"),
             optional=True,
         ),
     )
 
 
+class CopyFilesIntoLocationStatementSegment(BaseSegment):
+    """A Snowflake `COPY FILE INTO <location> FROM <location>` statement.
+
+    # https://docs.snowflake.com/en/sql-reference/sql/copy-files.html
+    """
+
+    type = "copy_files_into_location_statement"
+
+    match_grammar = Sequence(
+        "COPY",
+        "FILES",
+        "INTO",
+        Ref("StorageLocation"),
+        "FROM",
+        Ref("StorageLocation"),
+        AnySetOf(
+            Sequence(
+                "FILES",
+                Ref("EqualsSegment"),
+                Bracketed(Delimited(Ref("QuotedLiteralSegment"))),
+            ),
+            Sequence(
+                "PATTERN",
+                Ref("EqualsSegment"),
+                Ref("QuotedLiteralSegment"),
+            ),
+            Sequence(
+                "DETAILED_OUTPUT",
+                Ref("EqualsSegment"),
+                Ref("BooleanLiteralGrammar"),
+            ),
+            optional=True,
+        ),
+    )
+
+
 class StorageLocation(BaseSegment):
     """A Snowflake storage location.
 
     https://docs.snowflake.com/en/sql-reference/sql/copy-into-table.html#syntax
     """
 
     type = "storage_location"
@@ -5668,23 +5760,28 @@
     type = "stage_parameters"
 
     match_grammar = Sequence(
         OneOf(
             Sequence(
                 "STORAGE_INTEGRATION",
                 Ref("EqualsSegment"),
-                Ref("ObjectReferenceSegment"),
+                OneOf(
+                    Ref("ObjectReferenceSegment"), Ref("ReferencedVariableNameSegment")
+                ),
             ),
             Sequence(
                 "CREDENTIALS",
                 Ref("EqualsSegment"),
                 Bracketed(
                     Sequence("AZURE_SAS_TOKEN"),
                     Ref("EqualsSegment"),
-                    Ref("QuotedLiteralSegment"),
+                    OneOf(
+                        Ref("QuotedLiteralSegment"),
+                        Ref("ReferencedVariableNameSegment"),
+                    ),
                 ),
             ),
             optional=True,
         ),
         Sequence(
             "ENCRYPTION",
             Ref("EqualsSegment"),
@@ -5801,15 +5898,18 @@
                                 ),
                             ),
                             optional=True,
                         ),
                     ),
                     # External Azure Blob Storage stage
                     Sequence(
-                        Ref("AzureBlobStoragePath"),
+                        OneOf(
+                            Ref("AzureBlobStoragePath"),
+                            Ref("ReferencedVariableNameSegment"),
+                        ),
                         Ref("AzureBlobStorageExternalStageParameters", optional=True),
                         Sequence(
                             "DIRECTORY",
                             Ref("EqualsSegment"),
                             Bracketed(
                                 Sequence(
                                     "ENABLE",
@@ -6004,14 +6104,51 @@
                 Ref("ObjectReferenceSegment"),
             ),
         ),
         Ref("CommentEqualsClauseSegment", optional=True),
     )
 
 
+class CreateStreamlitStatementSegment(BaseSegment):
+    """A Snowflake `CREATE STREAMLIT` statement.
+
+    https://docs.snowflake.com/en/sql-reference/sql/create-streamlit.html
+    """
+
+    type = "create_streamlit_statement"
+
+    match_grammar = Sequence(
+        "CREATE",
+        Ref("OrReplaceGrammar", optional=True),
+        "STREAMLIT",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("ObjectReferenceSegment"),
+        Sequence(
+            "ROOT_LOCATION",
+            Ref("EqualsSegment"),
+            Ref("StagePath"),
+        ),
+        Sequence(
+            "MAIN_FILE",
+            Ref("EqualsSegment"),
+            Ref("QuotedLiteralSegment"),
+        ),
+        Sequence(
+            "QUERY_WAREHOUSE",
+            Ref("EqualsSegment"),
+            OneOf(
+                Ref("ObjectReferenceSegment"),
+                Ref("QuotedLiteralSegment"),
+            ),
+            optional=True,
+        ),
+        Ref("CommentEqualsClauseSegment", optional=True),
+    )
+
+
 class AlterStreamStatementSegment(BaseSegment):
     """A Snowflake `ALTER STREAM` statement.
 
     https://docs.snowflake.com/en/sql-reference/sql/alter-stream.html
     """
 
     type = "alter_stream_statement"
@@ -6046,14 +6183,56 @@
                     "COMMENT",
                 ),
             ),
         ),
     )
 
 
+class AlterStreamlitStatementSegment(BaseSegment):
+    """A Snowflake `ALTER STREAMLIT` statement.
+
+    https://docs.snowflake.com/en/sql-reference/sql/alter-streamlit.html
+    """
+
+    type = "alter_streamlit_statement"
+
+    match_grammar = Sequence(
+        "ALTER",
+        "STREAMLIT",
+        Ref("IfExistsGrammar", optional=True),
+        Ref("ObjectReferenceSegment"),
+        OneOf(
+            Sequence(
+                "SET",
+                Sequence(
+                    "ROOT_LOCATION",
+                    Ref("EqualsSegment"),
+                    Ref("StagePath"),
+                ),
+                Sequence(
+                    "MAIN_FILE",
+                    Ref("EqualsSegment"),
+                    Ref("QuotedLiteralSegment"),
+                ),
+                Sequence(
+                    "QUERY_WAREHOUSE",
+                    Ref("EqualsSegment"),
+                    OneOf(
+                        Ref("ObjectReferenceSegment"),
+                        Ref("QuotedLiteralSegment"),
+                    ),
+                    optional=True,
+                ),
+                Ref("CommentEqualsClauseSegment", optional=True),
+            ),
+            Sequence("RENAME", "TO", Ref("ObjectReferenceSegment")),
+        ),
+    )
+
+
 class ShowStatementSegment(BaseSegment):
     """A snowflake `SHOW` statement.
 
     https://docs.snowflake.com/en/sql-reference/sql/show.html
     """
 
     _object_types_plural = OneOf(
@@ -6088,14 +6267,15 @@
         Sequence("MASKING", "POLICIES"),
         "COLUMNS",
         Sequence("FILE", "FORMATS"),
         "SEQUENCES",
         "STAGES",
         "PIPES",
         "STREAMS",
+        "STREAMLITS",
         "TASKS",
         Sequence("USER", "FUNCTIONS"),
         Sequence("EXTERNAL", "FUNCTIONS"),
         "PROCEDURES",
         Sequence("FUTURE", "GRANTS"),
         Sequence("EXTERNAL", "VOLUMES"),
     )
@@ -6904,14 +7084,18 @@
                 Ref("ObjectReferenceSegment"),
             ),
             # https://docs.snowflake.com/en/sql-reference/sql/desc-stream.html
             Sequence(
                 "STREAM",
                 Ref("ObjectReferenceSegment"),
             ),
+            Sequence(
+                "STREAMLIT",
+                Ref("ObjectReferenceSegment"),
+            ),
             # https://docs.snowflake.com/en/sql-reference/sql/desc-task.html
             Sequence(
                 "TASK",
                 Ref("ObjectReferenceSegment"),
             ),
             # https://docs.snowflake.com/en/sql-reference/sql/desc-function.html
             Sequence(
@@ -7061,14 +7245,15 @@
             "STAGE",
             "FUNCTION",
             "PROCEDURE",
             "SEQUENCE",
             "SHARE",
             "PIPE",
             "STREAM",
+            "STREAMLIT",
             "TASK",
             Sequence(
                 "NETWORK",
                 "POLICY",
             ),
             Sequence(
                 OneOf(
@@ -7363,14 +7548,15 @@
                         ),
                         "INTEGRATION",
                     ),
                     "PIPE",
                     Sequence("ROW", "ACCESS", "POLICY"),
                     "STAGE",
                     "STREAM",
+                    "STREAMLIT",
                     "TAG",
                     "TASK",
                 ),
                 Ref("IfExistsGrammar", optional=True),
                 Ref("ObjectReferenceSegment"),
             ),
             Sequence(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 snowflake_reserved_keywords = """ALL
 ALTER
 AND
 ANY
 AS
+ASOF
 BETWEEN
 BY
 CAST
 CHECK
 CONNECT
 CONNECTION
 CONSTRAINT
@@ -45,14 +46,15 @@
 IS
 JOIN
 LATERAL
 LEFT
 LIKE
 LOCALTIME
 LOCALTIMESTAMP
+MATCH_CONDITION
 MATCH_RECOGNIZE
 MINUS
 NATURAL
 NOT
 NULL
 NULL_IF
 OF
@@ -308,14 +310,15 @@
 IMPORT
 IMPORTS
 IMPORTED
 INCLUDE_QUERY_ID
 INDEX
 INFORMATION
 INITIALLY
+INITIALIZE
 INITIALLY_SUSPENDED
 INPUT
 INTEGRATION
 INTEGRATIONS
 INTERVAL
 ISSUE
 JAVA
@@ -336,14 +339,15 @@
 LOCAL
 LOCATION
 LOCKS
 LOGIN_NAME
 LS
 LZO
 M
+MAIN_FILE
 MANAGE
 MANAGED
 MASKING
 MASTER_KEY
 MATCH
 MATCHED
 MATCHES
@@ -437,24 +441,26 @@
 PROCEDURE
 PROCEDURES
 PUBLIC
 PURGE
 PUT
 PYTHON
 QUERIES
+QUERY_WAREHOUSE
 QUEUE
 RANGE
 RAW_DEFLATE
 READ
 RECLUSTER
 RECORD_DELIMITER
 RECURSIVE
 REFERENCES
 REFERENCE_USAGE
 REFRESH
+REFRESH_MODE
 REFRESH_ON_CREATE
 REGIONS
 REMOVE
 RENAME
 REPEATABLE
 REPLACE
 REPLACE_INVALID_CHARACTERS
@@ -476,14 +482,15 @@
 RETURN_ERRORS
 RETURN_FAILED_ONLY
 RM
 ROLE
 ROLES
 ROLLBACK
 ROLLUP
+ROOT_LOCATION
 ROUTINE
 ROUTINES
 ROW
 RSA_PUBLIC_KEY
 RSA_PUBLIC_KEY_2
 RUNNING
 RUNTIME_VERSION
@@ -542,14 +549,16 @@
 STORAGE_BLOCKED_LOCATIONS
 STORAGE_INTEGRATION
 STORAGE_LOCATION
 STORAGE_LOCATIONS
 STORAGE_PROVIDER
 STREAM
 STREAMS
+STREAMLIT
+STREAMLITS
 STRIP_NULL_VALUES
 STRIP_OUTER_ARRAY
 STRIP_OUTER_ELEMENT
 SUBPATH
 SUPPORT
 SUSPEND
 SUSPEND_IMMEDIATE
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,22 @@
     ),
     JoinLikeClauseGrammar=Sequence(
         OneOf(
             Ref("PivotClauseSegment"),
             Ref("UnpivotClauseSegment"),
             Ref("LateralViewClauseSegment"),
         ),
-        Ref("AliasExpressionSegment", optional=True),
+        Ref(
+            "AliasExpressionSegment",
+            exclude=OneOf(
+                Ref("FromClauseTerminatorGrammar"),
+                Ref("JoinLikeClauseGrammar"),
+            ),
+            optional=True,
+        ),
     ),
     LikeGrammar=OneOf(
         # https://spark.apache.org/docs/latest/sql-ref-syntax-qry-select-like.html
         # ilike: https://github.com/apache/spark/pull/33966/files
         Sequence(
             OneOf("LIKE", "ILIKE"),
             OneOf(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,14 @@
                 WhitespaceSegment,
             ),
         ),
     ]
 )
 
 sqlite_dialect.replace(
-    BooleanBinaryOperatorGrammar=OneOf(
-        Ref("AndOperatorGrammar"), Ref("OrOperatorGrammar"), "REGEXP"
-    ),
     PrimaryKeyGrammar=Sequence(
         "PRIMARY", "KEY", Sequence("AUTOINCREMENT", optional=True)
     ),
     TemporaryTransientGrammar=Ref("TemporaryGrammar"),
     DateTimeLiteralGrammar=Sequence(
         OneOf("DATE", "DATETIME"),
         TypedParser("single_quote", LiteralSegment, type="date_constructor_literal"),
@@ -190,14 +187,18 @@
     ),
     IsDistinctFromGrammar=Sequence(
         "IS",
         Ref.keyword("NOT", optional=True),
         Sequence("DISTINCT", "FROM", optional=True),
     ),
     NanLiteralSegment=Nothing(),
+    PatternMatchingGrammar=Sequence(
+        Ref.keyword("NOT", optional=True),
+        OneOf("GLOB", "REGEXP", "MATCH"),
+    ),
 )
 
 
 class SetOperatorSegment(BaseSegment):
     """A set operator such as Union, Minus, Except or Intersect."""
 
     type = "set_operator"
@@ -283,14 +284,34 @@
             Ref("SingleIdentifierGrammar"),  # Column name
             Ref("ExpressionSegment"),  # Expression for simple functions
         ),
         OneOf("ASC", "DESC", optional=True),
     )
 
 
+class ReturningClauseSegment(BaseSegment):
+    """A returning clause.
+
+    Per docs https://www.sqlite.org/lang_returning.html
+    """
+
+    type = "returning_clause"
+
+    match_grammar = Sequence(
+        "RETURNING",
+        Delimited(
+            Ref("WildcardExpressionSegment"),
+            Sequence(
+                Ref("ExpressionSegment"),
+                Ref("AliasExpressionSegment", optional=True),
+            ),
+        ),
+    )
+
+
 class InsertStatementSegment(BaseSegment):
     """An`INSERT` statement.
 
     https://www.sqlite.org/lang_insert.html
     """
 
     type = "insert_statement"
@@ -317,14 +338,15 @@
         Ref("TableReferenceSegment"),
         Ref("BracketedColumnReferenceListGrammar", optional=True),
         OneOf(
             Ref("ValuesClauseSegment"),
             OptionallyBracketed(Ref("SelectableGrammar")),
             Ref("DefaultValuesGrammar"),
         ),
+        Ref("ReturningClauseSegment", optional=True),
     )
 
 
 class ColumnConstraintSegment(ansi.ColumnConstraintSegment):
     """Overriding ColumnConstraintSegment to allow for additional segment parsing."""
 
     match_grammar = ansi.ColumnConstraintSegment.match_grammar.copy(
@@ -505,14 +527,51 @@
         Ref("GroupByClauseSegment", optional=True),
         Ref("HavingClauseSegment", optional=True),
         Ref("OverlapsClauseSegment", optional=True),
         Ref("NamedWindowSegment", optional=True),
     )
 
 
+class DeleteStatementSegment(ansi.DeleteStatementSegment):
+    """A `DELETE` statement.
+
+    DELETE FROM <table name> [ WHERE <search condition> ]
+    """
+
+    type = "delete_statement"
+    # match grammar. This one makes sense in the context of knowing that it's
+    # definitely a statement, we just don't know what type yet.
+    match_grammar: Matchable = Sequence(
+        "DELETE",
+        Ref("FromClauseSegment"),
+        Ref("WhereClauseSegment", optional=True),
+        Ref("ReturningClauseSegment", optional=True),
+    )
+
+
+class UpdateStatementSegment(ansi.UpdateStatementSegment):
+    """An `Update` statement.
+
+    UPDATE <table name> SET <set clause list> [ WHERE <search condition> ]
+    """
+
+    type = "update_statement"
+    match_grammar: Matchable = Sequence(
+        "UPDATE",
+        Ref("TableReferenceSegment"),
+        # SET is not a reserved word in all dialects (e.g. RedShift)
+        # So specifically exclude as an allowed implicit alias to avoid parsing errors
+        Ref("AliasExpressionSegment", exclude=Ref.keyword("SET"), optional=True),
+        Ref("SetClauseListSegment"),
+        Ref("FromClauseSegment", optional=True),
+        Ref("WhereClauseSegment", optional=True),
+        Ref("ReturningClauseSegment", optional=True),
+    )
+
+
 class SelectStatementSegment(BaseSegment):
     """A `SELECT` statement.
 
     Replaces (without overriding) ANSI to remove Eager Matcher
     """
 
     type = "select_statement"
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_trino.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino.py`

 * *Files 7% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         ),
         "VARBINARY",
         "JSON",
         # Date and time
         "DATE",
         Sequence(
             OneOf("TIME", "TIMESTAMP"),
-            Bracketed(Ref("NumericLiteralSegment"), optional=True),
+            Ref("BracketedArguments", optional=True),
             Sequence(OneOf("WITH", "WITHOUT"), "TIME", "ZONE", optional=True),
         ),
         # Structural
         "ARRAY",
         "MAP",
         "ROW",
         # Others
@@ -397,7 +397,17 @@
                 "TRUNCATE",
                 Ref("SingleQuotedIdentifierSegment", optional=True),
                 OneOf("WITH", "WITHOUT", optional=True),
                 Ref.keyword("COUNT", optional=True),
             ),
         ),
     )
+
+
+class ArrayTypeSegment(ansi.ArrayTypeSegment):
+    """Prefix for array literals.
+
+    Trino supports "ARRAY"
+    """
+
+    type = "array_type"
+    match_grammar = Ref.keyword("ARRAY")
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_trino_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -2235,15 +2235,15 @@
             allow_gaps=False,
             optional=True,
         ),
         OneOf(
             Ref("DatatypeIdentifierSegment"),
             Bracketed(Ref("DatatypeIdentifierSegment"), bracket_type="square"),
         ),
-        # Stop Gap until explicit Data Types as only relevent for character
+        # Stop Gap until explicit Data Types as only relevant for character
         Ref.keyword("VARYING", optional=True),
         Ref("BracketedArguments", optional=True),
         Ref("CharCharacterSetGrammar", optional=True),
     )
 
 
 class CreateSequenceOptionsSegment(BaseSegment):
@@ -5046,15 +5046,15 @@
             Ref("TableReferenceSegment"),
             Sequence("ALL", "SERVER"),
             "DATABASE",
         ),
         Sequence(
             "WITH",
             AnySetOf(
-                # NOTE: Techincally, ENCRYPTION can't be combined with the other two,
+                # NOTE: Technically, ENCRYPTION can't be combined with the other two,
                 # but this slightly more generous parsing is ok for SQLFluff.
                 Ref.keyword("ENCRYPTION"),
                 Ref.keyword("NATIVE_COMPILATION"),
                 Ref.keyword("SCHEMABINDING"),
             ),
             Ref("ExecuteAsClause", optional=True),
             optional=True,
@@ -5594,15 +5594,15 @@
 
 
 class SqlcmdCommandSegment(BaseSegment):
     """A `sqlcmd` command.
 
     Microsoft allows professional CI/CD deployment through so called 'SQL Database
     Projects'.
-    There are propietary `sqlcmd Commands` that can be part of an SQL file.
+    There are proprietary `sqlcmd Commands` that can be part of an SQL file.
     https://learn.microsoft.com/en-us/sql/tools/sqlcmd/sqlcmd-utility?view=sql-server-ver16#sqlcmd-commands
     """
 
     type = "sqlcmd_command_segment"
 
     match_grammar: Matchable = OneOf(
         Sequence(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     "PERCENT",
     "PIVOT",
     "PLAN",
     "PRIMARY",
     "PRINT",
     "PROC",
     "PROCEDURE",
-    "PROPERTY",
     "PUBLIC",
     "RAISERROR",
     "READ",
     "READ_ONLY",
     "READTEXT",
     "RECONFIGURE",
     "REFERENCES",
@@ -489,14 +488,15 @@
     "PERIOD",
     "PERSISTED",
     "POPULATION",
     "PRECEDING",
     "PRECISION",  # listed as reserved but functionally unreserved
     "PRIOR",
     "PROFILE",
+    "PROPERTY",
     "PUSHDOWN",
     "QUERY_GOVERNOR_COST_LIMIT",
     "QUERYTRACEON",
     "QUOTED_IDENTIFIER",
     "R",  # sqlcmd command
     "RANDOMIZED",
     "RANGE",
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_vertica.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/dialects/dialect_vertica_keywords.py` & `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-3.0.4/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL08.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/AL09.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,25 +141,26 @@
                 first_letter_is_lowercase = character != character.upper()
                 break
             # If none of the characters are letters there will be a parsing
             # error, so not sure we need this statement
             first_letter_is_lowercase = False
 
         if first_letter_is_lowercase:
-            refuted_cases.update(["upper", "capitalise", "pascal"])
+            # snake added here as it cannot be inferred (presents as lower)
+            refuted_cases.update(["upper", "capitalise", "pascal", "snake"])
             if segment.raw != segment.raw.lower():
                 refuted_cases.update(["lower"])
         else:
             refuted_cases.update(["lower"])
             if segment.raw != segment.raw.upper():
                 refuted_cases.update(["upper"])
             if segment.raw != segment.raw.capitalize():
                 refuted_cases.update(["capitalise"])
             if not segment.raw.isalnum():
-                refuted_cases.update(["pascal"])
+                refuted_cases.update(["pascal", "snake"])
 
         # Update the memory
         memory["refuted_cases"] = refuted_cases
 
         self.logger.debug(
             f"Refuted cases after segment '{segment.raw}': {refuted_cases}"
         )
@@ -214,14 +215,23 @@
             # correct Pascalcase to PascalCase, but there's only so much we can
             # do. We do correct underscore_words to Underscore_Words.
             fixed_raw = regex.sub(
                 "([^a-zA-Z0-9]+|^)([a-zA-Z0-9])([a-zA-Z0-9]*)",
                 lambda match: match.group(1) + match.group(2).upper() + match.group(3),
                 segment.raw,
             )
+        elif concrete_policy == "snake":
+            if segment.raw.isupper():
+                fixed_raw = segment.raw.lower()
+            else:
+                fixed_raw = regex.sub(
+                    r"(?<=[a-z0-9])([A-Z])|(?<=[A-Za-z])([0-9])|(?<=[0-9])([A-Za-z])",
+                    lambda match: "_" + match.group(),
+                    segment.raw,
+                ).lower()
 
         if fixed_raw == segment.raw:
             # No need to fix
             self.logger.debug(
                 f"Capitalisation of segment '{segment.raw}' already OK with "
                 f"policy '{concrete_policy}', returning with memory {memory}"
             )
@@ -232,14 +242,16 @@
 
             if concrete_policy in ["upper", "lower"]:
                 policy = f"{concrete_policy} case."
             elif concrete_policy == "capitalise":
                 policy = "capitalised."
             elif concrete_policy == "pascal":
                 policy = "pascal case."
+            elif concrete_policy == "snake":
+                policy = "snake case."
 
             # Return the fixed segment
             self.logger.debug(
                 f"INCONSISTENT Capitalisation of segment '{segment.raw}', "
                 f"fixing to '{fixed_raw}' and returning with memory {memory}"
             )
             return LintResult(
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/capitalisation/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV01.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         # Only check ``<>`` or ``!=`` operators
         raw_operator_list = [r.raw for r in raw_comparison_operators]
         if raw_operator_list not in [["<", ">"], ["!", "="]]:
             return None
 
         memory = context.memory
-        # If style is consistent, add the style of the first occurence to memory
+        # If style is consistent, add the style of the first occurrence to memory
         if self.preferred_not_equal_style == "consistent":
             preferred_not_equal_style = context.memory.get("preferred_not_equal_style")
             if not preferred_not_equal_style:
                 preferred_not_equal_style = (
                     "ansi" if raw_operator_list == ["<", ">"] else "c_style"
                 )
                 memory["preferred_not_equal_style"] = preferred_not_equal_style
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/ST09.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/rules/tsql/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/rules/tsql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/analysis/query.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/analysis/query.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/analysis/select.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/context.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/identifers.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-3.0.4/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-3.0.4/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.3
+Version: 3.0.4
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -117,14 +117,15 @@
 - [Redshift](https://docs.aws.amazon.com/redshift/index.html)
 - [Snowflake](https://www.snowflake.com/)
 - [SOQL](https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm)
 - [SparkSQL](https://spark.apache.org/docs/latest/)
 - [SQLite](https://www.sqlite.org/)
 - [Teradata](https://www.teradata.com/)
 - [Transact-SQL](https://docs.microsoft.com/en-us/sql/t-sql/language-reference) (aka T-SQL)
+- [Trino](https://trino.io/)
 - [Vertica](https://www.vertica.com/)
 
 We aim to make it easy to expand on the support of these dialects and also
 add other, currently unsupported, dialects. Please [raise issues](https://github.com/sqlfluff/sqlfluff/issues)
 (or upvote any existing issues) to let us know of demand for missing support.
 
 Pull requests from those that know the missing syntax or dialects are especially
```

### Comparing `sqlfluff-3.0.3/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-3.0.4/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-3.0.4/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.3/test/testing_test.py` & `sqlfluff-3.0.4/test/testing_test.py`

 * *Files identical despite different names*

