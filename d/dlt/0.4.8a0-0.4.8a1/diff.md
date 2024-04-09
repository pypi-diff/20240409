# Comparing `tmp/dlt-0.4.8a0.tar.gz` & `tmp/dlt-0.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.4.8a0.tar", max compression
+gzip compressed data, was "dlt-0.4.8a1.tar", max compression
```

## Comparing `dlt-0.4.8a0.tar` & `dlt-0.4.8a1.tar`

### file list

```diff
@@ -1,341 +1,341 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.8a0/LICENSE.txt
--rw-r--r--   0        0        0     5296 2024-03-22 07:07:43.963916 dlt-0.4.8a0/README.md
--rw-r--r--   0        0        0     2229 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/__init__.py
--rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.8a0/dlt/__main__.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    21507 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     4178 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    16912 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.8a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.8a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    21105 2024-01-25 20:07:33.363195 dlt-0.4.8a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    14152 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0    10152 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/requirements.py
--rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      292 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      808 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.8a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     7410 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0    11848 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.8a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.8a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     5161 2024-02-27 21:03:24.127544 dlt-0.4.8a0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    13407 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    20983 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1836 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     5263 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0     2643 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/specs/azure_credentials.py
--rw-r--r--   0        0        0    18147 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     6498 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3456 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     2339 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    13313 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      874 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2856 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6680 2024-02-29 18:05:14.217554 dlt-0.4.8a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6859 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.8a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      537 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     9917 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     4936 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0     1021 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0    12252 2024-03-25 19:46:02.160297 dlt-0.4.8a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      423 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     3967 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0     5108 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/destination/exceptions.py
--rw-r--r--   0        0        0    24950 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6274 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/git.py
--rw-r--r--   0        0        0     7195 2024-02-27 21:03:24.127544 dlt-0.4.8a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.8a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.8a0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a0/dlt/common/libs/__init__.py
--rw-r--r--   0        0        0      181 2024-03-08 19:36:32.669855 dlt-0.4.8a0/dlt/common/libs/numpy.py
--rw-r--r--   0        0        0      436 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/libs/pandas.py
--rw-r--r--   0        0        0      217 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/libs/pandas_sql.py
--rw-r--r--   0        0        0    14420 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/libs/pyarrow.py
--rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/common/libs/pydantic.py
--rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.8a0/dlt/common/libs/sql_alchemy.py
--rw-r--r--   0        0        0     3652 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/logger.py
--rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.8a0/dlt/common/managed_thread_pool.py
--rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1408 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    14418 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.8a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     3426 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    31088 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.8a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     6119 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      665 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     3640 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.8a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.8a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    14599 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.8a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0     1067 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runtime/json_logging.py
--rw-r--r--   0        0        0     2074 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     6753 2024-03-25 13:59:17.909819 dlt-0.4.8a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     1938 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      582 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/runtime/typing.py
--rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     2419 2024-01-24 17:23:08.496518 dlt-0.4.8a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     5245 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/common/schema/migrations.py
--rw-r--r--   0        0        0    42525 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     5209 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    28381 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.8a0/dlt/common/source.py
--rw-r--r--   0        0        0     1182 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     4869 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     4833 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     4289 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0    11056 2024-02-26 22:08:47.270507 dlt-0.4.8a0/dlt/common/storages/fsspec_filesystem.py
--rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.8a0/dlt/common/storages/fsspecs/__init__.py
--rw-r--r--   0        0        0    20474 2024-02-26 22:08:47.270507 dlt-0.4.8a0/dlt/common/storages/fsspecs/google_drive.py
--rw-r--r--   0        0        0     3513 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    25742 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/common/storages/load_package.py
--rw-r--r--   0        0        0     9624 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     3197 2024-03-22 07:07:43.963916 dlt-0.4.8a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     9524 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     7578 2024-03-08 19:36:32.669855 dlt-0.4.8a0/dlt/common/time.py
--rw-r--r--   0        0        0     8854 2024-03-08 19:36:32.669855 dlt-0.4.8a0/dlt/common/typing.py
--rw-r--r--   0        0        0    19563 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/common/utils.py
--rw-r--r--   0        0        0     7978 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/common/validation.py
--rw-r--r--   0        0        0     1658 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/common/versioned_state.py
--rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/warnings.py
--rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/common/wei.py
--rw-r--r--   0        0        0     1147 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/destinations/adapters.py
--rw-r--r--   0        0        0     4855 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/decorators.py
--rw-r--r--   0        0        0     4918 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/destinations/impl/__init__.py
--rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/destinations/impl/athena/__init__.py
--rw-r--r--   0        0        0    18448 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/impl/athena/athena.py
--rw-r--r--   0        0        0     1054 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/athena/configuration.py
--rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.8a0/dlt/destinations/impl/athena/factory.py
--rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/destinations/impl/bigquery/README.md
--rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.8a0/dlt/destinations/impl/bigquery/__init__.py
--rw-r--r--   0        0        0    18083 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/bigquery/bigquery.py
--rw-r--r--   0        0        0     7453 2024-03-08 19:36:32.669855 dlt-0.4.8a0/dlt/destinations/impl/bigquery/bigquery_adapter.py
--rw-r--r--   0        0        0     1714 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/bigquery/configuration.py
--rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/impl/bigquery/factory.py
--rw-r--r--   0        0        0    10708 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/bigquery/sql_client.py
--rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/databricks/__init__.py
--rw-r--r--   0        0        0     2043 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/databricks/configuration.py
--rw-r--r--   0        0        0    13411 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/databricks/databricks.py
--rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/impl/databricks/factory.py
--rw-r--r--   0        0        0     6136 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/databricks/sql_client.py
--rw-r--r--   0        0        0      706 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/impl/destination/__init__.py
--rw-r--r--   0        0        0     1046 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/destination/configuration.py
--rw-r--r--   0        0        0     7654 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/impl/destination/destination.py
--rw-r--r--   0        0        0     5631 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/impl/destination/factory.py
--rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/duckdb/__init__.py
--rw-r--r--   0        0        0     9013 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/duckdb/configuration.py
--rw-r--r--   0        0        0     6803 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/duckdb/duck.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/duckdb/factory.py
--rw-r--r--   0        0        0     6828 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/duckdb/sql_client.py
--rw-r--r--   0        0        0     1459 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/dummy/__init__.py
--rw-r--r--   0        0        0     1027 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/dummy/configuration.py
--rw-r--r--   0        0        0     6704 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/impl/dummy/dummy.py
--rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.8a0/dlt/destinations/impl/dummy/factory.py
--rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/filesystem/__init__.py
--rw-r--r--   0        0        0      889 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/filesystem/configuration.py
--rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.8a0/dlt/destinations/impl/filesystem/factory.py
--rw-r--r--   0        0        0     9542 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/destinations/impl/filesystem/filesystem.py
--rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/motherduck/__init__.py
--rw-r--r--   0        0        0     3243 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/motherduck/configuration.py
--rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/motherduck/factory.py
--rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/motherduck/motherduck.py
--rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/motherduck/sql_client.py
--rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/mssql/README.md
--rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/mssql/__init__.py
--rw-r--r--   0        0        0     3971 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/mssql/configuration.py
--rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/mssql/factory.py
--rw-r--r--   0        0        0     7267 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/mssql/mssql.py
--rw-r--r--   0        0        0     6282 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/mssql/sql_client.py
--rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/postgres/README.md
--rw-r--r--   0        0        0     1349 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/postgres/__init__.py
--rw-r--r--   0        0        0     1794 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/postgres/configuration.py
--rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/postgres/factory.py
--rw-r--r--   0        0        0     5320 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/postgres/postgres.py
--rw-r--r--   0        0        0     5678 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/postgres/sql_client.py
--rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/qdrant/__init__.py
--rw-r--r--   0        0        0     3044 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/qdrant/configuration.py
--rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/qdrant/factory.py
--rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/impl/qdrant/qdrant_adapter.py
--rw-r--r--   0        0        0    17902 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/impl/qdrant/qdrant_client.py
--rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/redshift/README.md
--rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/redshift/__init__.py
--rw-r--r--   0        0        0     1005 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/redshift/configuration.py
--rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/redshift/factory.py
--rw-r--r--   0        0        0    10603 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/redshift/redshift.py
--rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/snowflake/__init__.py
--rw-r--r--   0        0        0     5449 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/snowflake/configuration.py
--rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/snowflake/factory.py
--rw-r--r--   0        0        0    11443 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/snowflake/snowflake.py
--rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/snowflake/sql_client.py
--rw-r--r--   0        0        0     2355 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/synapse/__init__.py
--rw-r--r--   0        0        0     2746 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/synapse/configuration.py
--rw-r--r--   0        0        0     2640 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/synapse/factory.py
--rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/impl/synapse/sql_client.py
--rw-r--r--   0        0        0    13083 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/destinations/impl/synapse/synapse.py
--rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/destinations/impl/synapse/synapse_adapter.py
--rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/weaviate/README.md
--rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/impl/weaviate/__init__.py
--rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/weaviate/ci_naming.py
--rw-r--r--   0        0        0     2009 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/impl/weaviate/configuration.py
--rw-r--r--   0        0        0      666 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/impl/weaviate/exceptions.py
--rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/weaviate/factory.py
--rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/impl/weaviate/naming.py
--rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/impl/weaviate/weaviate_adapter.py
--rw-r--r--   0        0        0    26322 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/impl/weaviate/weaviate_client.py
--rw-r--r--   0        0        0     6532 2024-02-07 18:59:43.276965 dlt-0.4.8a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    23883 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0     3049 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/path_utils.py
--rw-r--r--   0        0        0     9310 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    21311 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/destinations/sql_jobs.py
--rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.8a0/dlt/destinations/type_mapping.py
--rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.8a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0      506 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/destinations/utils.py
--rw-r--r--   0        0        0      639 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/extract/concurrency.py
--rw-r--r--   0        0        0    35614 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0    17152 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14914 2024-03-24 08:57:37.871597 dlt-0.4.8a0/dlt/extract/extractors.py
--rw-r--r--   0        0        0    18640 2024-03-24 08:57:37.871597 dlt-0.4.8a0/dlt/extract/hints.py
--rw-r--r--   0        0        0    29556 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/extract/incremental/__init__.py
--rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/extract/incremental/exceptions.py
--rw-r--r--   0        0        0    14942 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/extract/incremental/transform.py
--rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/extract/incremental/typing.py
--rw-r--r--   0        0        0     6786 2024-03-24 08:57:37.871597 dlt-0.4.8a0/dlt/extract/items.py
--rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0    16344 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/extract/pipe_iterator.py
--rw-r--r--   0        0        0    26683 2024-03-24 08:57:37.871597 dlt-0.4.8a0/dlt/extract/resource.py
--rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.8a0/dlt/extract/source.py
--rw-r--r--   0        0        0     5293 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/extract/storage.py
--rw-r--r--   0        0        0     9254 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/extract/utils.py
--rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/extract/validation.py
--rw-r--r--   0        0        0      832 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/extract/wrappers.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.8a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    23495 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1241 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6821 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.8a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    15742 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.8a0/dlt/helpers/dbt_cloud/__init__.py
--rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/helpers/dbt_cloud/client.py
--rw-r--r--   0        0        0      623 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/helpers/dbt_cloud/configuration.py
--rw-r--r--   0        0        0      349 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/__init__.py
--rw-r--r--   0        0        0     1230 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/load_info.py
--rw-r--r--   0        0        0      483 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/menu.py
--rw-r--r--   0        0        0     2451 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/query.py
--rw-r--r--   0        0        0      928 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/resource_state.py
--rw-r--r--   0        0        0      618 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/show_data.py
--rw-r--r--   0        0        0     2842 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/table_hints.py
--rw-r--r--   0        0        0      150 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/index.py
--rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/pages/__init__.py
--rw-r--r--   0        0        0     1668 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/pages/dashboard.py
--rw-r--r--   0        0        0     4446 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/pages/load_info.py
--rw-r--r--   0        0        0      757 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/theme.py
--rw-r--r--   0        0        0     2361 2024-03-24 08:57:37.871597 dlt-0.4.8a0/dlt/helpers/streamlit_app/utils.py
--rw-r--r--   0        0        0      386 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/__init__.py
--rw-r--r--   0        0        0      901 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
--rw-r--r--   0        0        0     1004 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/logo.py
--rw-r--r--   0        0        0      613 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/schema.py
--rw-r--r--   0        0        0     1542 2024-03-22 07:07:43.983916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/stats.py
--rw-r--r--   0        0        0      805 2024-03-22 07:07:43.993916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/summary.py
--rw-r--r--   0        0        0     1189 2024-03-22 07:07:43.993916 dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/tags.py
--rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.8a0/dlt/load/__init__.py
--rw-r--r--   0        0        0      807 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     2061 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    24626 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/load/load.py
--rw-r--r--   0        0        0     8096 2024-03-20 22:31:16.351558 dlt-0.4.8a0/dlt/load/utils.py
--rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1525 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0      529 2024-01-24 17:23:08.526518 dlt-0.4.8a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    15226 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/normalize/items_normalizers.py
--rw-r--r--   0        0        0    20321 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    14454 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     2098 2024-03-25 16:17:38.059826 dlt-0.4.8a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      709 2024-03-22 07:07:43.993916 dlt-0.4.8a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     4599 2024-03-22 07:07:43.993916 dlt-0.4.8a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     9792 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      212 2024-03-22 07:07:43.993916 dlt-0.4.8a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    73879 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     3858 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/pipeline/platform.py
--rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     5539 2024-03-25 13:59:13.899819 dlt-0.4.8a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0    13256 2024-03-25 13:59:17.919819 dlt-0.4.8a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     5579 2024-02-27 21:03:24.147544 dlt-0.4.8a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/pipeline/warnings.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.8a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5818 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/config.py
--rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/credentials.py
--rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/filesystem.py
--rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0     1368 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.8a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.8a0/dlt/sources/helpers/requests/typing.py
--rw-r--r--   0        0        0     1210 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/__init__.py
--rw-r--r--   0        0        0     7202 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/auth.py
--rw-r--r--   0        0        0     9317 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/client.py
--rw-r--r--   0        0        0     4502 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/detector.py
--rw-r--r--   0        0        0      103 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/exceptions.py
--rw-r--r--   0        0        0     5510 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/paginators.py
--rw-r--r--   0        0        0      446 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/typing.py
--rw-r--r--   0        0        0      406 2024-03-25 19:48:22.140297 dlt-0.4.8a0/dlt/sources/helpers/rest_client/utils.py
--rw-r--r--   0        0        0      682 2024-03-08 19:36:32.679855 dlt-0.4.8a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-11-28 14:04:28.308006 dlt-0.4.8a0/dlt/version.py
--rw-r--r--   0        0        0     6929 2024-03-26 13:05:09.999253 dlt-0.4.8a0/pyproject.toml
--rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 dlt-0.4.8a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.4.8a1/LICENSE.txt
+-rw-r--r--   0        0        0     5296 2024-03-22 07:07:43.963916 dlt-0.4.8a1/README.md
+-rw-r--r--   0        0        0     2229 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/__init__.py
+-rw-r--r--   0        0        0       69 2024-03-08 19:36:32.659855 dlt-0.4.8a1/dlt/__main__.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    21507 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     4178 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    18229 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    16912 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1944 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    21105 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    14152 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0    10152 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     2524 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/requirements.py
+-rw-r--r--   0        0        0     4895 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1912 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/cli/utils.py
+-rw-r--r--   0        0        0      292 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      808 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5144 2024-01-24 17:23:08.476518 dlt-0.4.8a1/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     7410 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     8457 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0    11848 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1777 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      682 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      805 2024-03-05 18:21:35.930419 dlt-0.4.8a1/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1129 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1346 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1995 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     5161 2024-02-27 21:03:24.127544 dlt-0.4.8a1/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1319 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    13407 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    20983 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0     1742 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1836 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     5263 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0     2643 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/azure_credentials.py
+-rw-r--r--   0        0        0    18147 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     6498 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3456 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     2339 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2667 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    13313 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      874 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2856 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6680 2024-02-29 18:05:14.217554 dlt-0.4.8a1/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      220 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6859 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      269 2024-01-24 17:23:08.486518 dlt-0.4.8a1/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      537 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     9917 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     4936 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0     1021 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0    12252 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      423 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     3967 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0     5108 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/destination/exceptions.py
+-rw-r--r--   0        0        0    24950 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6274 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     5149 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/git.py
+-rw-r--r--   0        0        0     7195 2024-02-27 21:03:24.127544 dlt-0.4.8a1/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1814 2024-02-16 18:38:47.332466 dlt-0.4.8a1/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2948 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1562 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.257189 dlt-0.4.8a1/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0      181 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/libs/numpy.py
+-rw-r--r--   0        0        0      436 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pandas.py
+-rw-r--r--   0        0        0      217 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pandas_sql.py
+-rw-r--r--   0        0        0    14420 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0    15624 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/libs/pydantic.py
+-rw-r--r--   0        0        0    15486 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/libs/sql_alchemy.py
+-rw-r--r--   0        0        0     3652 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/logger.py
+-rw-r--r--   0        0        0      854 2024-03-01 09:52:05.856761 dlt-0.4.8a1/dlt/common/managed_thread_pool.py
+-rw-r--r--   0        0        0      384 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1408 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      510 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1905 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    14418 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0      123 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      810 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0      798 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      830 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     4570 2024-03-18 14:01:48.098768 dlt-0.4.8a1/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     2967 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      359 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     3426 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      461 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    31088 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      375 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     6119 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5103 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      329 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      665 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     3640 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4132 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3162 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5583 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       71 2023-11-18 17:38:04.267189 dlt-0.4.8a1/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    14599 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     5461 2024-01-25 20:07:33.363195 dlt-0.4.8a1/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     1067 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     6616 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/json_logging.py
+-rw-r--r--   0        0        0     2074 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     6753 2024-03-25 13:59:17.909819 dlt-0.4.8a1/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2784 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1938 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      582 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0     2960 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      579 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/runtime/typing.py
+-rw-r--r--   0        0        0      805 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     2419 2024-01-24 17:23:08.496518 dlt-0.4.8a1/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     5245 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0     5269 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/schema/migrations.py
+-rw-r--r--   0        0        0    42525 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     5209 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    28381 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1672 2024-02-10 23:59:00.181729 dlt-0.4.8a1/dlt/common/source.py
+-rw-r--r--   0        0        0     1182 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     4869 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     4833 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     4289 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    14242 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0    11056 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspec_filesystem.py
+-rw-r--r--   0        0        0        0 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspecs/__init__.py
+-rw-r--r--   0        0        0    20474 2024-02-26 22:08:47.270507 dlt-0.4.8a1/dlt/common/storages/fsspecs/google_drive.py
+-rw-r--r--   0        0        0     3513 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    25742 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/load_package.py
+-rw-r--r--   0        0        0     9624 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     3197 2024-03-22 07:07:43.963916 dlt-0.4.8a1/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     9524 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9065 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2867 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     7578 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/time.py
+-rw-r--r--   0        0        0     8854 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/common/typing.py
+-rw-r--r--   0        0        0    19563 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/common/utils.py
+-rw-r--r--   0        0        0     7978 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/common/validation.py
+-rw-r--r--   0        0        0     1658 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/common/versioned_state.py
+-rw-r--r--   0        0        0     5528 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/warnings.py
+-rw-r--r--   0        0        0     1219 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/common/wei.py
+-rw-r--r--   0        0        0     1147 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      404 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/adapters.py
+-rw-r--r--   0        0        0     4855 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/decorators.py
+-rw-r--r--   0        0        0     4918 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/destinations/impl/__init__.py
+-rw-r--r--   0        0        0     1311 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/destinations/impl/athena/__init__.py
+-rw-r--r--   0        0        0    18448 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/athena/athena.py
+-rw-r--r--   0        0        0     1054 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/athena/configuration.py
+-rw-r--r--   0        0        0     2169 2024-01-24 17:23:08.506518 dlt-0.4.8a1/dlt/destinations/impl/athena/factory.py
+-rw-r--r--   0        0        0      439 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/bigquery/README.md
+-rw-r--r--   0        0        0     1118 2024-03-18 14:01:48.108768 dlt-0.4.8a1/dlt/destinations/impl/bigquery/__init__.py
+-rw-r--r--   0        0        0    18083 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery.py
+-rw-r--r--   0        0        0     7453 2024-03-08 19:36:32.669855 dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery_adapter.py
+-rw-r--r--   0        0        0     1714 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/bigquery/configuration.py
+-rw-r--r--   0        0        0     1309 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/bigquery/factory.py
+-rw-r--r--   0        0        0    10708 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1430 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/__init__.py
+-rw-r--r--   0        0        0     2043 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/databricks/configuration.py
+-rw-r--r--   0        0        0    13411 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/databricks.py
+-rw-r--r--   0        0        0     1741 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/databricks/factory.py
+-rw-r--r--   0        0        0     6136 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/databricks/sql_client.py
+-rw-r--r--   0        0        0      706 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/__init__.py
+-rw-r--r--   0        0        0     1046 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/destination/configuration.py
+-rw-r--r--   0        0        0     7654 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/destination.py
+-rw-r--r--   0        0        0     5631 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/impl/destination/factory.py
+-rw-r--r--   0        0        0     1236 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/__init__.py
+-rw-r--r--   0        0        0     9013 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/duckdb/configuration.py
+-rw-r--r--   0        0        0     6803 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/duck.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/duckdb/factory.py
+-rw-r--r--   0        0        0     6828 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1459 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/dummy/__init__.py
+-rw-r--r--   0        0        0     1027 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/dummy/configuration.py
+-rw-r--r--   0        0        0     6704 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/dummy/dummy.py
+-rw-r--r--   0        0        0     1111 2024-02-23 11:16:27.641941 dlt-0.4.8a1/dlt/destinations/impl/dummy/factory.py
+-rw-r--r--   0        0        0      194 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/filesystem/__init__.py
+-rw-r--r--   0        0        0      889 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/filesystem/configuration.py
+-rw-r--r--   0        0        0     2411 2024-03-24 19:55:58.511453 dlt-0.4.8a1/dlt/destinations/impl/filesystem/factory.py
+-rw-r--r--   0        0        0     9542 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1134 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/motherduck/__init__.py
+-rw-r--r--   0        0        0     3243 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/motherduck/configuration.py
+-rw-r--r--   0        0        0     1966 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/motherduck/factory.py
+-rw-r--r--   0        0        0      911 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/motherduck/motherduck.py
+-rw-r--r--   0        0        0     1515 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/motherduck/sql_client.py
+-rw-r--r--   0        0        0      253 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/README.md
+-rw-r--r--   0        0        0     1385 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/__init__.py
+-rw-r--r--   0        0        0     3971 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/mssql/configuration.py
+-rw-r--r--   0        0        0     1764 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/mssql/factory.py
+-rw-r--r--   0        0        0     7267 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/mssql/mssql.py
+-rw-r--r--   0        0        0     6282 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/mssql/sql_client.py
+-rw-r--r--   0        0        0      251 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/postgres/README.md
+-rw-r--r--   0        0        0     1349 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/__init__.py
+-rw-r--r--   0        0        0     1794 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/postgres/configuration.py
+-rw-r--r--   0        0        0     1840 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/postgres/factory.py
+-rw-r--r--   0        0        0     5320 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/postgres.py
+-rw-r--r--   0        0        0     5678 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/postgres/sql_client.py
+-rw-r--r--   0        0        0      677 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/qdrant/__init__.py
+-rw-r--r--   0        0        0     3044 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/qdrant/configuration.py
+-rw-r--r--   0        0        0     1146 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/qdrant/factory.py
+-rw-r--r--   0        0        0     1831 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_adapter.py
+-rw-r--r--   0        0        0    17902 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_client.py
+-rw-r--r--   0        0        0     1159 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/redshift/README.md
+-rw-r--r--   0        0        0     1181 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/redshift/__init__.py
+-rw-r--r--   0        0        0     1005 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/redshift/configuration.py
+-rw-r--r--   0        0        0     2006 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/redshift/factory.py
+-rw-r--r--   0        0        0    10603 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/redshift/redshift.py
+-rw-r--r--   0        0        0     1218 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/__init__.py
+-rw-r--r--   0        0        0     5449 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/snowflake/configuration.py
+-rw-r--r--   0        0        0     2008 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/snowflake/factory.py
+-rw-r--r--   0        0        0    11443 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/snowflake.py
+-rw-r--r--   0        0        0     6885 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/snowflake/sql_client.py
+-rw-r--r--   0        0        0     2355 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/synapse/__init__.py
+-rw-r--r--   0        0        0     2746 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/synapse/configuration.py
+-rw-r--r--   0        0        0     2640 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/synapse/factory.py
+-rw-r--r--   0        0        0     1179 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/synapse/sql_client.py
+-rw-r--r--   0        0        0    13083 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse.py
+-rw-r--r--   0        0        0     2231 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse_adapter.py
+-rw-r--r--   0        0        0      526 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/README.md
+-rw-r--r--   0        0        0      752 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/impl/weaviate/__init__.py
+-rw-r--r--   0        0        0      280 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/ci_naming.py
+-rw-r--r--   0        0        0     2009 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/configuration.py
+-rw-r--r--   0        0        0      666 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/exceptions.py
+-rw-r--r--   0        0        0     1935 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/factory.py
+-rw-r--r--   0        0        0     3259 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/impl/weaviate/naming.py
+-rw-r--r--   0        0        0     3914 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_adapter.py
+-rw-r--r--   0        0        0    26322 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_client.py
+-rw-r--r--   0        0        0     6532 2024-02-07 18:59:43.276965 dlt-0.4.8a1/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    23883 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     2086 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0     3049 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/path_utils.py
+-rw-r--r--   0        0        0     9310 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    21311 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/destinations/sql_jobs.py
+-rw-r--r--   0        0        0     4895 2024-02-27 21:03:24.137544 dlt-0.4.8a1/dlt/destinations/type_mapping.py
+-rw-r--r--   0        0        0     1877 2024-01-24 17:23:08.516518 dlt-0.4.8a1/dlt/destinations/typing.py
+-rw-r--r--   0        0        0      506 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/destinations/utils.py
+-rw-r--r--   0        0        0      639 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/__init__.py
+-rw-r--r--   0        0        0     8539 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/concurrency.py
+-rw-r--r--   0        0        0    35614 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    16480 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0    17152 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14914 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/extractors.py
+-rw-r--r--   0        0        0    18640 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/hints.py
+-rw-r--r--   0        0        0    29556 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/incremental/__init__.py
+-rw-r--r--   0        0        0     1142 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/extract/incremental/exceptions.py
+-rw-r--r--   0        0        0    14942 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/incremental/transform.py
+-rw-r--r--   0        0        0      322 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/extract/incremental/typing.py
+-rw-r--r--   0        0        0     6786 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/items.py
+-rw-r--r--   0        0        0    16368 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/pipe.py
+-rw-r--r--   0        0        0    16344 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/extract/pipe_iterator.py
+-rw-r--r--   0        0        0    26683 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/extract/resource.py
+-rw-r--r--   0        0        0    19990 2024-03-18 14:01:48.118769 dlt-0.4.8a1/dlt/extract/source.py
+-rw-r--r--   0        0        0     5293 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/storage.py
+-rw-r--r--   0        0        0     9254 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/extract/utils.py
+-rw-r--r--   0        0        0     3500 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/extract/validation.py
+-rw-r--r--   0        0        0      832 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/extract/wrappers.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.4.8a1/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    23495 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3701 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1241 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6821 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      772 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     7163 2024-02-07 18:59:43.286965 dlt-0.4.8a1/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    15742 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     4881 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/helpers/dbt_cloud/__init__.py
+-rw-r--r--   0        0        0     4926 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/helpers/dbt_cloud/client.py
+-rw-r--r--   0        0        0      623 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/helpers/dbt_cloud/configuration.py
+-rw-r--r--   0        0        0      349 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/__init__.py
+-rw-r--r--   0        0        0     1230 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/load_info.py
+-rw-r--r--   0        0        0      483 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/menu.py
+-rw-r--r--   0        0        0     2451 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/query.py
+-rw-r--r--   0        0        0      928 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/resource_state.py
+-rw-r--r--   0        0        0      618 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/show_data.py
+-rw-r--r--   0        0        0     2842 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/table_hints.py
+-rw-r--r--   0        0        0      150 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/index.py
+-rw-r--r--   0        0        0        0 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/__init__.py
+-rw-r--r--   0        0        0     1668 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/dashboard.py
+-rw-r--r--   0        0        0     4446 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/load_info.py
+-rw-r--r--   0        0        0      757 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/theme.py
+-rw-r--r--   0        0        0     2361 2024-03-24 08:57:37.871597 dlt-0.4.8a1/dlt/helpers/streamlit_app/utils.py
+-rw-r--r--   0        0        0      386 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/__init__.py
+-rw-r--r--   0        0        0      901 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py
+-rw-r--r--   0        0        0     1004 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/logo.py
+-rw-r--r--   0        0        0      613 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/schema.py
+-rw-r--r--   0        0        0     1542 2024-03-22 07:07:43.983916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/stats.py
+-rw-r--r--   0        0        0      805 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/summary.py
+-rw-r--r--   0        0        0     1189 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/tags.py
+-rw-r--r--   0        0        0       51 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/load/__init__.py
+-rw-r--r--   0        0        0      807 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/load/configuration.py
+-rw-r--r--   0        0        0     2061 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    24626 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/load/load.py
+-rw-r--r--   0        0        0     8096 2024-03-20 22:31:16.351558 dlt-0.4.8a1/dlt/load/utils.py
+-rw-r--r--   0        0        0       58 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1525 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0      529 2024-01-24 17:23:08.526518 dlt-0.4.8a1/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    15226 2024-03-26 22:09:23.640890 dlt-0.4.8a1/dlt/normalize/items_normalizers.py
+-rw-r--r--   0        0        0    20321 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    14454 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     2098 2024-03-25 16:17:38.059826 dlt-0.4.8a1/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      709 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4950 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     4599 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     9792 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      212 2024-03-22 07:07:43.993916 dlt-0.4.8a1/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    73879 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3858 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/platform.py
+-rw-r--r--   0        0        0     1007 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     5539 2024-03-25 13:59:13.899819 dlt-0.4.8a1/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0    13256 2024-03-25 13:59:17.919819 dlt-0.4.8a1/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     5579 2024-02-27 21:03:24.147544 dlt-0.4.8a1/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       92 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0      796 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/pipeline/warnings.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.4.8a1/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      565 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5818 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6278 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      417 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      110 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/config.py
+-rw-r--r--   0        0        0      790 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/credentials.py
+-rw-r--r--   0        0        0      200 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/filesystem.py
+-rw-r--r--   0        0        0        0 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0     1291 2024-03-27 11:19:53.626208 dlt-0.4.8a1/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0    10965 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1969 2024-01-24 17:23:08.536518 dlt-0.4.8a1/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      234 2023-11-18 17:38:04.277189 dlt-0.4.8a1/dlt/sources/helpers/requests/typing.py
+-rw-r--r--   0        0        0     1210 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/__init__.py
+-rw-r--r--   0        0        0     7202 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/auth.py
+-rw-r--r--   0        0        0     9317 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/client.py
+-rw-r--r--   0        0        0     4502 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/detector.py
+-rw-r--r--   0        0        0      103 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/exceptions.py
+-rw-r--r--   0        0        0     5510 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/paginators.py
+-rw-r--r--   0        0        0      446 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/typing.py
+-rw-r--r--   0        0        0      406 2024-03-25 19:48:22.140297 dlt-0.4.8a1/dlt/sources/helpers/rest_client/utils.py
+-rw-r--r--   0        0        0      682 2024-03-08 19:36:32.679855 dlt-0.4.8a1/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-11-28 14:04:28.308006 dlt-0.4.8a1/dlt/version.py
+-rw-r--r--   0        0        0     6929 2024-03-27 12:18:58.750863 dlt-0.4.8a1/pyproject.toml
+-rw-r--r--   0        0        0     9890 1970-01-01 00:00:00.000000 dlt-0.4.8a1/PKG-INFO
```

### Comparing `dlt-0.4.8a0/LICENSE.txt` & `dlt-0.4.8a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/README.md` & `dlt-0.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/__init__.py` & `dlt-0.4.8a1/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/_dlt.py` & `dlt-0.4.8a1/dlt/cli/_dlt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/config_toml_writer.py` & `dlt-0.4.8a1/dlt/cli/config_toml_writer.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/deploy_command.py` & `dlt-0.4.8a1/dlt/cli/deploy_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/deploy_command_helpers.py` & `dlt-0.4.8a1/dlt/cli/deploy_command_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/echo.py` & `dlt-0.4.8a1/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/init_command.py` & `dlt-0.4.8a1/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/pipeline_command.py` & `dlt-0.4.8a1/dlt/cli/pipeline_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/pipeline_files.py` & `dlt-0.4.8a1/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/requirements.py` & `dlt-0.4.8a1/dlt/cli/requirements.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/source_detection.py` & `dlt-0.4.8a1/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/telemetry_command.py` & `dlt-0.4.8a1/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/cli/utils.py` & `dlt-0.4.8a1/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/arithmetics.py` & `dlt-0.4.8a1/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/__init__.py` & `dlt-0.4.8a1/dlt/common/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/accessors.py` & `dlt-0.4.8a1/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/container.py` & `dlt-0.4.8a1/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/exceptions.py` & `dlt-0.4.8a1/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/inject.py` & `dlt-0.4.8a1/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/paths.py` & `dlt-0.4.8a1/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/__init__.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/context.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/environ.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/provider.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/providers/toml.py` & `dlt-0.4.8a1/dlt/common/configuration/providers/toml.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/resolve.py` & `dlt-0.4.8a1/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/azure_credentials.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/azure_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.4.8a1/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/configuration/utils.py` & `dlt-0.4.8a1/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_types/type_helpers.py` & `dlt-0.4.8a1/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_writers/__init__.py` & `dlt-0.4.8a1/dlt/common/data_writers/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_writers/buffered.py` & `dlt-0.4.8a1/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_writers/escape.py` & `dlt-0.4.8a1/dlt/common/data_writers/escape.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_writers/exceptions.py` & `dlt-0.4.8a1/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/data_writers/writers.py` & `dlt-0.4.8a1/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/destination/capabilities.py` & `dlt-0.4.8a1/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/destination/exceptions.py` & `dlt-0.4.8a1/dlt/common/destination/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/destination/reference.py` & `dlt-0.4.8a1/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/exceptions.py` & `dlt-0.4.8a1/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/git.py` & `dlt-0.4.8a1/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/json/__init__.py` & `dlt-0.4.8a1/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/json/_orjson.py` & `dlt-0.4.8a1/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/json/_simplejson.py` & `dlt-0.4.8a1/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/jsonpath.py` & `dlt-0.4.8a1/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/libs/pyarrow.py` & `dlt-0.4.8a1/dlt/common/libs/pyarrow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/libs/pydantic.py` & `dlt-0.4.8a1/dlt/common/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/libs/sql_alchemy.py` & `dlt-0.4.8a1/dlt/common/libs/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/logger.py` & `dlt-0.4.8a1/dlt/common/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/managed_thread_pool.py` & `dlt-0.4.8a1/dlt/common/managed_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/configuration.py` & `dlt-0.4.8a1/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.4.8a1/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/json/relational.py` & `dlt-0.4.8a1/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.4.8a1/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.4.8a1/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.4.8a1/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.4.8a1/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.4.8a1/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/normalizers/utils.py` & `dlt-0.4.8a1/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/pipeline.py` & `dlt-0.4.8a1/dlt/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/reflection/spec.py` & `dlt-0.4.8a1/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/reflection/utils.py` & `dlt-0.4.8a1/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/configuration.py` & `dlt-0.4.8a1/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/pool_runner.py` & `dlt-0.4.8a1/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/runnable.py` & `dlt-0.4.8a1/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/stdout.py` & `dlt-0.4.8a1/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/synth_pickle.py` & `dlt-0.4.8a1/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runners/venv.py` & `dlt-0.4.8a1/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/collector.py` & `dlt-0.4.8a1/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/exec_info.py` & `dlt-0.4.8a1/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/init.py` & `dlt-0.4.8a1/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/json_logging.py` & `dlt-0.4.8a1/dlt/common/runtime/json_logging.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/prometheus.py` & `dlt-0.4.8a1/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/segment.py` & `dlt-0.4.8a1/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/sentry.py` & `dlt-0.4.8a1/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/signals.py` & `dlt-0.4.8a1/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/slack.py` & `dlt-0.4.8a1/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/telemetry.py` & `dlt-0.4.8a1/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/runtime/typing.py` & `dlt-0.4.8a1/dlt/common/runtime/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/__init__.py` & `dlt-0.4.8a1/dlt/common/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/detections.py` & `dlt-0.4.8a1/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/exceptions.py` & `dlt-0.4.8a1/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/migrations.py` & `dlt-0.4.8a1/dlt/common/schema/migrations.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/schema.py` & `dlt-0.4.8a1/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/typing.py` & `dlt-0.4.8a1/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/schema/utils.py` & `dlt-0.4.8a1/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/source.py` & `dlt-0.4.8a1/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/__init__.py` & `dlt-0.4.8a1/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/configuration.py` & `dlt-0.4.8a1/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/data_item_storage.py` & `dlt-0.4.8a1/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/exceptions.py` & `dlt-0.4.8a1/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/file_storage.py` & `dlt-0.4.8a1/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/fsspec_filesystem.py` & `dlt-0.4.8a1/dlt/common/storages/fsspec_filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/fsspecs/google_drive.py` & `dlt-0.4.8a1/dlt/common/storages/fsspecs/google_drive.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.4.8a1/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/load_package.py` & `dlt-0.4.8a1/dlt/common/storages/load_package.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/load_storage.py` & `dlt-0.4.8a1/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/normalize_storage.py` & `dlt-0.4.8a1/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/schema_storage.py` & `dlt-0.4.8a1/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/transactional_file.py` & `dlt-0.4.8a1/dlt/common/storages/transactional_file.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/storages/versioned_storage.py` & `dlt-0.4.8a1/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/time.py` & `dlt-0.4.8a1/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/typing.py` & `dlt-0.4.8a1/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/utils.py` & `dlt-0.4.8a1/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/validation.py` & `dlt-0.4.8a1/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/versioned_state.py` & `dlt-0.4.8a1/dlt/common/versioned_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/warnings.py` & `dlt-0.4.8a1/dlt/common/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/common/wei.py` & `dlt-0.4.8a1/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/__init__.py` & `dlt-0.4.8a1/dlt/destinations/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/decorators.py` & `dlt-0.4.8a1/dlt/destinations/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/exceptions.py` & `dlt-0.4.8a1/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/athena/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/athena/athena.py` & `dlt-0.4.8a1/dlt/destinations/impl/athena/athena.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/athena/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/athena/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/athena/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/athena/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/bigquery.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/bigquery_adapter.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/bigquery_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/bigquery/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/databricks/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/databricks/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/databricks/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/databricks/databricks.py` & `dlt-0.4.8a1/dlt/destinations/impl/databricks/databricks.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/databricks/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/databricks/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/databricks/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/databricks/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/destination/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/destination/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/destination/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/destination/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/destination/destination.py` & `dlt-0.4.8a1/dlt/destinations/impl/destination/destination.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/destination/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/destination/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/duckdb/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/duckdb/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/duckdb/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/duckdb/duck.py` & `dlt-0.4.8a1/dlt/destinations/impl/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/duckdb/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/duckdb/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/duckdb/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/dummy/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/dummy/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/dummy/dummy.py` & `dlt-0.4.8a1/dlt/destinations/impl/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/dummy/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/dummy/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/filesystem/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/filesystem/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/filesystem/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/filesystem/filesystem.py` & `dlt-0.4.8a1/dlt/destinations/impl/filesystem/filesystem.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/motherduck/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/motherduck/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/motherduck/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/motherduck/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/motherduck/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/motherduck/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/motherduck/motherduck.py` & `dlt-0.4.8a1/dlt/destinations/impl/motherduck/motherduck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/motherduck/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/motherduck/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/mssql/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/mssql/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/mssql/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/mssql/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/mssql/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/mssql/mssql.py` & `dlt-0.4.8a1/dlt/destinations/impl/mssql/mssql.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/mssql/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/mssql/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/postgres/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/postgres/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/postgres/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/postgres/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/postgres/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/postgres/postgres.py` & `dlt-0.4.8a1/dlt/destinations/impl/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/postgres/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/qdrant/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/qdrant/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/qdrant/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/qdrant/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/qdrant/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/qdrant/qdrant_adapter.py` & `dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/qdrant/qdrant_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/qdrant/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/redshift/README.md` & `dlt-0.4.8a1/dlt/destinations/impl/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/redshift/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/redshift/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/redshift/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/redshift/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/redshift/redshift.py` & `dlt-0.4.8a1/dlt/destinations/impl/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/snowflake/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/snowflake/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/snowflake/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/snowflake/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/snowflake/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/snowflake/snowflake.py` & `dlt-0.4.8a1/dlt/destinations/impl/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/snowflake/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/snowflake/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/synapse.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/synapse/synapse_adapter.py` & `dlt-0.4.8a1/dlt/destinations/impl/synapse/synapse_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/README.md` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/__init__.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/configuration.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/exceptions.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/factory.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/factory.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/naming.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/weaviate_adapter.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_adapter.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/impl/weaviate/weaviate_client.py` & `dlt-0.4.8a1/dlt/destinations/impl/weaviate/weaviate_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/insert_job_client.py` & `dlt-0.4.8a1/dlt/destinations/insert_job_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/job_client_impl.py` & `dlt-0.4.8a1/dlt/destinations/job_client_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/job_impl.py` & `dlt-0.4.8a1/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/path_utils.py` & `dlt-0.4.8a1/dlt/destinations/path_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/sql_client.py` & `dlt-0.4.8a1/dlt/destinations/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/sql_jobs.py` & `dlt-0.4.8a1/dlt/destinations/sql_jobs.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/type_mapping.py` & `dlt-0.4.8a1/dlt/destinations/type_mapping.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/destinations/typing.py` & `dlt-0.4.8a1/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/__init__.py` & `dlt-0.4.8a1/dlt/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/concurrency.py` & `dlt-0.4.8a1/dlt/extract/concurrency.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/decorators.py` & `dlt-0.4.8a1/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/exceptions.py` & `dlt-0.4.8a1/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/extract.py` & `dlt-0.4.8a1/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/extractors.py` & `dlt-0.4.8a1/dlt/extract/extractors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/hints.py` & `dlt-0.4.8a1/dlt/extract/hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/incremental/__init__.py` & `dlt-0.4.8a1/dlt/extract/incremental/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/incremental/exceptions.py` & `dlt-0.4.8a1/dlt/extract/incremental/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/incremental/transform.py` & `dlt-0.4.8a1/dlt/extract/incremental/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/items.py` & `dlt-0.4.8a1/dlt/extract/items.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/pipe.py` & `dlt-0.4.8a1/dlt/extract/pipe.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/pipe_iterator.py` & `dlt-0.4.8a1/dlt/extract/pipe_iterator.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/resource.py` & `dlt-0.4.8a1/dlt/extract/resource.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/source.py` & `dlt-0.4.8a1/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/storage.py` & `dlt-0.4.8a1/dlt/extract/storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/utils.py` & `dlt-0.4.8a1/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/validation.py` & `dlt-0.4.8a1/dlt/extract/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/extract/wrappers.py` & `dlt-0.4.8a1/dlt/extract/wrappers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/airflow_helper.py` & `dlt-0.4.8a1/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/__init__.py` & `dlt-0.4.8a1/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/configuration.py` & `dlt-0.4.8a1/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.4.8a1/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.4.8a1/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.4.8a1/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt/runner.py` & `dlt-0.4.8a1/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt_cloud/__init__.py` & `dlt-0.4.8a1/dlt/helpers/dbt_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt_cloud/client.py` & `dlt-0.4.8a1/dlt/helpers/dbt_cloud/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/dbt_cloud/configuration.py` & `dlt-0.4.8a1/dlt/helpers/dbt_cloud/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/load_info.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/query.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/query.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/resource_state.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/resource_state.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/show_data.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/show_data.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/blocks/table_hints.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/blocks/table_hints.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/pages/dashboard.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/pages/load_info.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/pages/load_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/theme.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/theme.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/utils.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/color_mode_selector.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/color_mode_selector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/logo.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/logo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/schema.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/stats.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/stats.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/summary.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/summary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/helpers/streamlit_app/widgets/tags.py` & `dlt-0.4.8a1/dlt/helpers/streamlit_app/widgets/tags.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/load/configuration.py` & `dlt-0.4.8a1/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/load/exceptions.py` & `dlt-0.4.8a1/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/load/load.py` & `dlt-0.4.8a1/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/load/utils.py` & `dlt-0.4.8a1/dlt/load/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/normalize/configuration.py` & `dlt-0.4.8a1/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/normalize/exceptions.py` & `dlt-0.4.8a1/dlt/normalize/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/normalize/items_normalizers.py` & `dlt-0.4.8a1/dlt/normalize/items_normalizers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/normalize/normalize.py` & `dlt-0.4.8a1/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/__init__.py` & `dlt-0.4.8a1/dlt/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/configuration.py` & `dlt-0.4.8a1/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/current.py` & `dlt-0.4.8a1/dlt/pipeline/current.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/dbt.py` & `dlt-0.4.8a1/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/exceptions.py` & `dlt-0.4.8a1/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/helpers.py` & `dlt-0.4.8a1/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/pipeline.py` & `dlt-0.4.8a1/dlt/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/platform.py` & `dlt-0.4.8a1/dlt/pipeline/platform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/progress.py` & `dlt-0.4.8a1/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/state_sync.py` & `dlt-0.4.8a1/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/trace.py` & `dlt-0.4.8a1/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/track.py` & `dlt-0.4.8a1/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/pipeline/warnings.py` & `dlt-0.4.8a1/dlt/pipeline/warnings.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/reflection/names.py` & `dlt-0.4.8a1/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/reflection/script_inspector.py` & `dlt-0.4.8a1/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/reflection/script_visitor.py` & `dlt-0.4.8a1/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/credentials.py` & `dlt-0.4.8a1/dlt/sources/credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.4.8a1/dlt/sources/helpers/requests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,27 @@
     Timeout,
     TooManyRedirects,
     URLRequired,
 )
 from requests.exceptions import ChunkedEncodingError
 from dlt.sources.helpers.requests.retry import Client
 from dlt.sources.helpers.requests.session import Session
-from dlt.sources.helpers.rest_client import paginate
 from dlt.common.configuration.specs import RunConfiguration
 
 client = Client()
 
-get, post, put, patch, delete, options, head, request, paginate = (
+get, post, put, patch, delete, options, head, request = (
     client.get,
     client.post,
     client.put,
     client.patch,
     client.delete,
     client.options,
     client.head,
     client.request,
-    paginate,
 )
 
 
 def init(config: RunConfiguration) -> None:
     """Initialize the default requests client from config"""
     client.update_from_config(config)
```

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.4.8a1/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/requests/session.py` & `dlt-0.4.8a1/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/rest_client/__init__.py` & `dlt-0.4.8a1/dlt/sources/helpers/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/rest_client/auth.py` & `dlt-0.4.8a1/dlt/sources/helpers/rest_client/auth.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/rest_client/client.py` & `dlt-0.4.8a1/dlt/sources/helpers/rest_client/client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/rest_client/detector.py` & `dlt-0.4.8a1/dlt/sources/helpers/rest_client/detector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/rest_client/paginators.py` & `dlt-0.4.8a1/dlt/sources/helpers/rest_client/paginators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/sources/helpers/transform.py` & `dlt-0.4.8a1/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/dlt/version.py` & `dlt-0.4.8a1/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.4.8a0/pyproject.toml` & `dlt-0.4.8a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.4.8a0"
+version = "0.4.8a1"
 description = "dlt is an open-source python-first scalable data loading library that does not require any backend to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
```

### Comparing `dlt-0.4.8a0/PKG-INFO` & `dlt-0.4.8a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.4.8a0
+Version: 0.4.8a1
 Summary: dlt is an open-source python-first scalable data loading library that does not require any backend to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
```

