# Comparing `tmp/deltacat-1.1.0.tar.gz` & `tmp/deltacat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deltacat-1.1.0.tar", last modified: Wed Mar 27 21:18:00 2024, max compression
+gzip compressed data, was "dist/deltacat-1.1.1.tar", last modified: Tue Apr  9 00:21:18 2024, max compression
```

## Comparing `deltacat-1.1.0.tar` & `deltacat-1.1.1.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 21:05:19.000000 deltacat-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-27 21:18:00.000000 deltacat-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-27 21:05:19.000000 deltacat-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/aws/redshift/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/aws/s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/benchmarking/benchmark_parquet_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/benchmarking/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/catalog/default_catalog_impl/
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/default_catalog_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/catalog/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/model/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14344 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    30174 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/compaction_session_audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/compactor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/dedupe_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/repartition_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/model/table_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/repartition_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/steps/repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23668 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/hash_bucket_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/merge_file_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/merge_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/model/merge_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    20731 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/steps/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/content_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/compactor_v2/utils/task_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/daft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/model/merge_on_read_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/merge_on_read/utils/delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/metastats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/metastats/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/metastats/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/stats/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/compute/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/io/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/io/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/io/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/storage/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/delete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/table_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/storage/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/aws/test_clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/catalog/test_default_catalog_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compact_partition_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/steps/test_repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor/utils/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/test_compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/test_hashlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     8322 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_util_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/compute/test_util_create_table_deltas_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_cloudpickle_bug_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/io/test_s3_object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/local_deltacat_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/local_deltacat_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/stats/test_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/test_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/test_utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/test_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/tests/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/test_cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/test_daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/test_record_batch_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/tests/utils/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/types/partial_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/types/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/daft.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat/utils/ray_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/ray_utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-03-27 21:05:19.000000 deltacat-1.1.0/deltacat/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:18:00.000000 deltacat-1.1.0/deltacat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-27 21:17:59.000000 deltacat-1.1.0/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-03-27 21:17:59.000000 deltacat-1.1.0/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:17:59.000000 deltacat-1.1.0/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-27 21:17:59.000000 deltacat-1.1.0/deltacat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 21:17:59.000000 deltacat-1.1.0/deltacat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 21:18:00.000000 deltacat-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-27 21:05:19.000000 deltacat-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-09 00:09:04.000000 deltacat-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-09 00:21:18.000000 deltacat-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-09 00:09:04.000000 deltacat-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/benchmarking/benchmark_parquet_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/benchmarking/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/catalog/default_catalog_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/default_catalog_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/compaction_session_audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/compactor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/dedupe_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/repartition_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/model/table_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/repartition_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/steps/repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/hash_bucket_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/merge_file_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/merge_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/model/merge_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21394 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/steps/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/content_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/compactor_v2/utils/task_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/daft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/model/merge_on_read_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/merge_on_read/utils/delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/io/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/delete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/aws/test_clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/catalog/test_default_catalog_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compact_partition_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/steps/test_repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor/utils/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/test_compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/test_hashlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_util_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/compute/test_util_create_table_deltas_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_cloudpickle_bug_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/io/test_s3_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/local_deltacat_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/local_deltacat_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/stats/test_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/test_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/test_utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/tests/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/test_cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/test_daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/test_record_batch_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/tests/utils/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/types/partial_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/ray_utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-09 00:09:04.000000 deltacat-1.1.1/deltacat/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:21:18.000000 deltacat-1.1.1/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-09 00:21:17.000000 deltacat-1.1.1/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-09 00:21:17.000000 deltacat-1.1.1/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:21:17.000000 deltacat-1.1.1/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 00:21:17.000000 deltacat-1.1.1/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 00:21:17.000000 deltacat-1.1.1/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:21:18.000000 deltacat-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-09 00:09:04.000000 deltacat-1.1.1/setup.py
```

### Comparing `deltacat-1.1.0/PKG-INFO` & `deltacat-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.0
+Version: 1.1.1
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.0/README.md` & `deltacat-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/__init__.py` & `deltacat-1.1.1/deltacat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     SortOrder,
 )
 from deltacat.types.media import ContentEncoding, ContentType, TableType
 from deltacat.types.tables import TableWriteMode
 
 deltacat.logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-1.1.0/deltacat/aws/clients.py` & `deltacat-1.1.1/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/aws/redshift/model/manifest.py` & `deltacat-1.1.1/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/aws/s3u.py` & `deltacat-1.1.1/deltacat/aws/s3u.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/benchmarking/benchmark_parquet_reads.py` & `deltacat-1.1.1/deltacat/benchmarking/benchmark_parquet_reads.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/benchmarking/conftest.py` & `deltacat-1.1.1/deltacat/benchmarking/conftest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/catalog/default_catalog_impl/__init__.py` & `deltacat-1.1.1/deltacat/catalog/default_catalog_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/catalog/delegate.py` & `deltacat-1.1.1/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/catalog/interface.py` & `deltacat-1.1.1/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/catalog/model/catalog.py` & `deltacat-1.1.1/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/catalog/model/table_definition.py` & `deltacat-1.1.1/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/__init__.py` & `deltacat-1.1.1/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/compaction_session.py` & `deltacat-1.1.1/deltacat/compute/compactor/compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/compact_partition_params.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/compact_partition_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from deltacat.compute.compactor_v2.constants import (
     MAX_RECORDS_PER_COMPACTED_FILE,
     MIN_DELTA_BYTES_IN_BATCH,
     MIN_FILES_IN_BATCH,
     AVERAGE_RECORD_SIZE_BYTES,
     TASK_MAX_PARALLELISM,
     DROP_DUPLICATES,
+    TOTAL_MEMORY_BUFFER_PERCENTAGE,
 )
 from deltacat.constants import PYARROW_INFLATION_MULTIPLIER
 from deltacat.compute.compactor.utils.sort_key import validate_sort_keys
 from deltacat.utils.metrics import MetricsConfig
 
 
 class CompactPartitionParams(dict):
@@ -81,20 +82,25 @@
         )
         result.previous_inflation = params.get(
             "previous_inflation", PYARROW_INFLATION_MULTIPLIER
         )
         result.average_record_size_bytes = params.get(
             "average_record_size_bytes", AVERAGE_RECORD_SIZE_BYTES
         )
+        result.total_memory_buffer_percentage = params.get(
+            "total_memory_buffer_percentage", TOTAL_MEMORY_BUFFER_PERCENTAGE
+        )
         result.hash_group_count = params.get(
             "hash_group_count", result.hash_bucket_count
         )
         result.drop_duplicates = params.get("drop_duplicates", DROP_DUPLICATES)
         result.ray_custom_resources = params.get("ray_custom_resources")
 
+        result.memory_logs_enabled = params.get("memory_logs_enabled", False)
+
         result.metrics_config = params.get("metrics_config")
 
         if not importlib.util.find_spec("memray"):
             result.enable_profiler = False
 
         if result.primary_keys:
             result.primary_keys = sorted(result.primary_keys)
@@ -187,14 +193,24 @@
         return self["average_record_size_bytes"]
 
     @average_record_size_bytes.setter
     def average_record_size_bytes(self, average_record_size_bytes: float) -> None:
         self["average_record_size_bytes"] = average_record_size_bytes
 
     @property
+    def total_memory_buffer_percentage(self) -> int:
+        return self["total_memory_buffer_percentage"]
+
+    @total_memory_buffer_percentage.setter
+    def total_memory_buffer_percentage(
+        self, total_memory_buffer_percentage: int
+    ) -> None:
+        self["total_memory_buffer_percentage"] = total_memory_buffer_percentage
+
+    @property
     def min_files_in_batch(self) -> float:
         return self["min_files_in_batch"]
 
     @min_files_in_batch.setter
     def min_files_in_batch(self, min_files_in_batch: float) -> None:
         self["min_files_in_batch"] = min_files_in_batch
 
@@ -352,14 +368,22 @@
         return self.get("sort_keys")
 
     @sort_keys.setter
     def sort_keys(self, keys: List[SortKey]) -> None:
         self["sort_keys"] = keys
 
     @property
+    def memory_logs_enabled(self) -> bool:
+        return self.get("memory_logs_enabled")
+
+    @memory_logs_enabled.setter
+    def memory_logs_enabled(self, value: bool) -> None:
+        self["memory_logs_enabled"] = value
+
+    @property
     def metrics_config(self) -> Optional[MetricsConfig]:
         return self.get("metrics_config")
 
     @metrics_config.setter
     def metrics_config(self, config: MetricsConfig) -> None:
         self["metrics_config"] = config
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/compaction_session_audit_info.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/compaction_session_audit_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,21 @@
         The total number of records that were deduplicated. For example,
         if there are 100 records with a particular primary key, 99 records
         will be deduplicated.
         """
         return self.get("recordsDeduped")
 
     @property
+    def records_deleted(self) -> int:
+        """
+        The total count of deleted records in a compaction session if delete deltas are present.
+        """
+        return self.get("recordsDeleted")
+
+    @property
     def input_size_bytes(self) -> float:
         """
         The on-disk size in bytes of the input. Analogous to bytes scanned
         """
         return self.get("inputSizeBytes")
 
     @property
@@ -457,14 +464,18 @@
         self["uniformDeltasCreated"] = uniform_deltas_created
         return self
 
     def set_records_deduped(self, records_deduped: int) -> CompactionSessionAuditInfo:
         self["recordsDeduped"] = records_deduped
         return self
 
+    def set_records_deleted(self, records_deleted: int) -> CompactionSessionAuditInfo:
+        self["recordsDeleted"] = records_deleted
+        return self
+
     def set_input_size_bytes(
         self, input_size_bytes: float
     ) -> CompactionSessionAuditInfo:
         self["inputSizeBytes"] = input_size_bytes
         return self
 
     def set_hash_bucket_count(
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/model/table_object_store.py` & `deltacat-1.1.1/deltacat/compute/compactor/model/table_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/repartition_session.py` & `deltacat-1.1.1/deltacat/compute/compactor/repartition_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/steps/dedupe.py` & `deltacat-1.1.1/deltacat/compute/compactor/steps/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-1.1.1/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/steps/materialize.py` & `deltacat-1.1.1/deltacat/compute/compactor/steps/materialize.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/steps/repartition.py` & `deltacat-1.1.1/deltacat/compute/compactor/steps/repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/utils/io.py` & `deltacat-1.1.1/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-1.1.1/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-1.1.1/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/utils/sort_key.py` & `deltacat-1.1.1/deltacat/compute/compactor/utils/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-1.1.1/deltacat/compute/compactor/utils/system_columns.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/compaction_session.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/compaction_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 )
 from deltacat.utils.resources import (
     get_current_process_peak_memory_usage_in_bytes,
 )
 from deltacat.compute.compactor_v2.utils.task_options import (
     hash_bucket_resource_options_provider,
     merge_resource_options_provider,
+    local_merge_resource_options_provider,
 )
 from deltacat.compute.compactor.model.compactor_version import CompactorVersion
 
 if importlib.util.find_spec("memray"):
     import memray
 
 
@@ -254,16 +255,18 @@
 
     hb_options_provider = functools.partial(
         task_resource_options_provider,
         pg_config=params.pg_config,
         resource_amount_provider=hash_bucket_resource_options_provider,
         previous_inflation=params.previous_inflation,
         average_record_size_bytes=params.average_record_size_bytes,
+        total_memory_buffer_percentage=params.total_memory_buffer_percentage,
         primary_keys=params.primary_keys,
         ray_custom_resources=params.ray_custom_resources,
+        memory_logs_enabled=params.memory_logs_enabled,
     )
 
     total_input_records_count = np.int64(0)
     total_hb_record_count = np.int64(0)
     telemetry_time_hb = 0
     if params.hash_bucket_count == 1:
         merge_start = time.monotonic()
@@ -271,15 +274,37 @@
             params,
             uniform_deltas,
             compacted_partition,
             round_completion_info,
             delete_strategy,
             delete_file_envelopes,
         )
-        local_merge_result = ray.get(mg.merge.remote(local_merge_input))
+        estimated_da_bytes = (
+            compaction_audit.estimated_in_memory_size_bytes_during_discovery
+        )
+        estimated_num_records = sum(
+            [
+                entry.meta.record_count
+                for delta in uniform_deltas
+                for entry in delta.manifest.entries
+            ]
+        )
+        local_merge_options = local_merge_resource_options_provider(
+            estimated_da_size=estimated_da_bytes,
+            estimated_num_rows=estimated_num_records,
+            total_memory_buffer_percentage=params.total_memory_buffer_percentage,
+            round_completion_info=round_completion_info,
+            compacted_delta_manifest=previous_compacted_delta_manifest,
+            ray_custom_resources=params.ray_custom_resources,
+            primary_keys=params.primary_keys,
+            memory_logs_enabled=params.memory_logs_enabled,
+        )
+        local_merge_result = ray.get(
+            mg.merge.options(**local_merge_options).remote(local_merge_input)
+        )
         total_input_records_count += local_merge_result.input_record_count
         merge_results = [local_merge_result]
         merge_invoke_end = time.monotonic()
     else:
         hb_start = time.monotonic()
 
         def hash_bucket_input_provider(index, item):
@@ -292,14 +317,15 @@
                     num_hash_groups=params.hash_group_count,
                     enable_profiler=params.enable_profiler,
                     metrics_config=params.metrics_config,
                     read_kwargs_provider=params.read_kwargs_provider,
                     object_store=params.object_store,
                     deltacat_storage=params.deltacat_storage,
                     deltacat_storage_kwargs=params.deltacat_storage_kwargs,
+                    memory_logs_enabled=params.memory_logs_enabled,
                 )
             }
 
         all_hash_group_idx_to_obj_id = defaultdict(list)
         all_hash_group_idx_to_size_bytes = defaultdict(int)
         all_hash_group_idx_to_num_rows = defaultdict(int)
         hb_tasks_pending = invoke_parallel(
@@ -378,20 +404,22 @@
         merge_options_provider = functools.partial(
             task_resource_options_provider,
             pg_config=params.pg_config,
             resource_amount_provider=merge_resource_options_provider,
             num_hash_groups=params.hash_group_count,
             hash_group_size_bytes=all_hash_group_idx_to_size_bytes,
             hash_group_num_rows=all_hash_group_idx_to_num_rows,
+            total_memory_buffer_percentage=params.total_memory_buffer_percentage,
             round_completion_info=round_completion_info,
             compacted_delta_manifest=previous_compacted_delta_manifest,
             primary_keys=params.primary_keys,
             deltacat_storage=params.deltacat_storage,
             deltacat_storage_kwargs=params.deltacat_storage_kwargs,
             ray_custom_resources=params.ray_custom_resources,
+            memory_logs_enabled=params.memory_logs_enabled,
         )
 
         def merge_input_provider(index, item):
             return {
                 "input": MergeInput.of(
                     merge_file_groups_provider=RemoteMergeFileGroupsProvider(
                         hash_group_index=item[0],
@@ -413,14 +441,15 @@
                     read_kwargs_provider=params.read_kwargs_provider,
                     round_completion_info=round_completion_info,
                     object_store=params.object_store,
                     deltacat_storage=params.deltacat_storage,
                     deltacat_storage_kwargs=params.deltacat_storage_kwargs,
                     delete_strategy=delete_strategy,
                     delete_file_envelopes=delete_file_envelopes,
+                    memory_logs_enabled=params.memory_logs_enabled,
                 )
             }
 
         merge_start = time.monotonic()
         merge_tasks_pending = invoke_parallel(
             items=all_hash_group_idx_to_obj_id.items(),
             ray_task=mg.merge,
@@ -434,33 +463,33 @@
 
     logger.info(f"Got {len(merge_results)} merge results.")
 
     merge_results_retrieved_at = time.time()
     merge_end = time.monotonic()
 
     total_dd_record_count = sum([ddr.deduped_record_count for ddr in merge_results])
-    total_dropped_record_count = sum(
+    total_deleted_record_count = sum(
         [ddr.deleted_record_count for ddr in merge_results]
     )
     logger.info(
-        f"Deduped {total_dd_record_count} records and dropped {total_dropped_record_count} records..."
+        f"Deduped {total_dd_record_count} records and deleted {total_deleted_record_count} records..."
     )
 
     compaction_audit.set_input_records(total_input_records_count.item())
 
     telemetry_time_merge = compaction_audit.save_step_stats(
         CompactionSessionAuditInfo.MERGE_STEP_NAME,
         merge_results,
         merge_results_retrieved_at,
         merge_invoke_end - merge_start,
         merge_end - merge_start,
     )
 
     compaction_audit.set_records_deduped(total_dd_record_count.item())
-
+    compaction_audit.set_records_deleted(total_deleted_record_count.item())
     mat_results = []
     for merge_result in merge_results:
         mat_results.extend(merge_result.materialize_results)
 
     mat_results: List[MaterializeResult] = sorted(
         mat_results, key=lambda m: m.task_index
     )
@@ -499,15 +528,15 @@
         deltas,
         stream_position=params.last_stream_position_to_compact,
     )
 
     record_info_msg = (
         f"Hash bucket records: {total_hb_record_count},"
         f" Deduped records: {total_dd_record_count}, "
-        f" Dropped records: {total_dropped_record_count}, "
+        f" Deleted records: {total_deleted_record_count}, "
         f" Materialized records: {merged_delta.meta.record_count}"
     )
     logger.info(record_info_msg)
 
     compacted_delta = params.deltacat_storage.commit_delta(
         merged_delta,
         properties=kwargs.get("properties", {}),
@@ -599,13 +628,12 @@
         input_average_record_size_bytes=input_average_record_size_bytes,
     )
 
     logger.info(
         f"partition-{params.source_partition_locator.partition_values},"
         f"compacted at: {params.last_stream_position_to_compact},"
     )
-
     return (
         compacted_partition,
         new_round_completion_info,
         rcf_source_partition_locator,
     )
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/constants.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_strategy.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_strategy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/model.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/model.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/deletes/utils.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/deletes/utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/model/hash_bucket_input.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/model/hash_bucket_input.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,30 @@
         hb_task_index: Optional[int] = 0,
         enable_profiler: Optional[bool] = False,
         metrics_config: Optional[MetricsConfig] = None,
         read_kwargs_provider: Optional[ReadKwargsProvider] = None,
         object_store: Optional[IObjectStore] = None,
         deltacat_storage=unimplemented_deltacat_storage,
         deltacat_storage_kwargs: Optional[Dict[str, Any]] = None,
+        memory_logs_enabled: Optional[bool] = None,
     ) -> HashBucketInput:
 
         result = HashBucketInput()
         result["annotated_delta"] = annotated_delta
         result["primary_keys"] = primary_keys
         result["hb_task_index"] = hb_task_index
         result["num_hash_buckets"] = num_hash_buckets
         result["num_hash_groups"] = num_hash_groups
         result["enable_profiler"] = enable_profiler
         result["metrics_config"] = metrics_config
         result["read_kwargs_provider"] = read_kwargs_provider
         result["object_store"] = object_store
         result["deltacat_storage"] = deltacat_storage
         result["deltacat_storage_kwargs"] = deltacat_storage_kwargs or {}
+        result["memory_logs_enabled"] = memory_logs_enabled
 
         return result
 
     @property
     def annotated_delta(self) -> DeltaAnnotated:
         return self["annotated_delta"]
 
@@ -78,7 +80,11 @@
     @property
     def deltacat_storage(self) -> unimplemented_deltacat_storage:
         return self.get("deltacat_storage")
 
     @property
     def deltacat_storage_kwargs(self) -> Optional[Dict[str, Any]]:
         return self.get("deltacat_storage_kwargs")
+
+    @property
+    def memory_logs_enabled(self) -> Optional[bool]:
+        return self.get("memory_logs_enabled")
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/model/merge_file_group.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/model/merge_file_group.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/model/merge_input.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/model/merge_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         read_kwargs_provider: Optional[ReadKwargsProvider] = None,
         round_completion_info: Optional[RoundCompletionInfo] = None,
         object_store: Optional[IObjectStore] = None,
         delete_strategy: Optional[DeleteStrategy] = None,
         delete_file_envelopes: Optional[List] = None,
         deltacat_storage=unimplemented_deltacat_storage,
         deltacat_storage_kwargs: Optional[Dict[str, Any]] = None,
+        memory_logs_enabled: Optional[bool] = None,
     ) -> MergeInput:
 
         result = MergeInput()
         result["merge_file_groups_provider"] = merge_file_groups_provider
         result["write_to_partition"] = write_to_partition
         result["compacted_file_content_type"] = compacted_file_content_type
         result["primary_keys"] = primary_keys
@@ -63,14 +64,15 @@
         result["read_kwargs_provider"] = read_kwargs_provider
         result["round_completion_info"] = round_completion_info
         result["object_store"] = object_store
         result["delete_file_envelopes"] = delete_file_envelopes
         result["delete_strategy"] = delete_strategy
         result["deltacat_storage"] = deltacat_storage
         result["deltacat_storage_kwargs"] = deltacat_storage_kwargs or {}
+        result["memory_logs_enabled"] = memory_logs_enabled
         return result
 
     @property
     def merge_file_groups_provider(self) -> MergeFileGroupsProvider:
         return self["merge_file_groups_provider"]
 
     @property
@@ -130,14 +132,18 @@
         return self["deltacat_storage"]
 
     @property
     def deltacat_storage_kwargs(self) -> Optional[Dict[str, Any]]:
         return self.get("deltacat_storage_kwargs")
 
     @property
+    def memory_logs_enabled(self) -> Optional[bool]:
+        return self.get("memory_logs_enabled")
+
+    @property
     def delete_file_envelopes(
         self,
     ) -> Optional[List[DeleteFileEnvelope]]:
         return self.get("delete_file_envelopes")
 
     @property
     def delete_strategy(self) -> Optional[DeleteStrategy]:
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/steps/hash_bucket.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/steps/hash_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,16 @@
         # Log node peak memory utilization every 10 seconds
         def log_peak_memory():
             logger.debug(
                 f"Process peak memory utilization so far: {process_util.max_memory} bytes "
                 f"({process_util.max_memory/BYTES_PER_GIBIBYTE} GB)"
             )
 
-        process_util.schedule_callback(log_peak_memory, 10)
+        if input.memory_logs_enabled:
+            process_util.schedule_callback(log_peak_memory, 10)
 
         hash_bucket_result, duration = timed_invocation(
             func=_timed_hash_bucket, input=input
         )
 
         emit_metrics_time = 0.0
         if input.metrics_config:
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/steps/merge.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/steps/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import time
 import pyarrow.compute as pc
 import deltacat.compute.compactor_v2.utils.merge as merge_utils
 from uuid import uuid4
 from deltacat import logs
 from typing import Callable, Iterator, List, Optional, Tuple
 from deltacat.compute.compactor_v2.model.merge_result import MergeResult
+from deltacat.compute.compactor_v2.model.merge_file_group import MergeFileGroup
 from deltacat.compute.compactor.model.materialize_result import MaterializeResult
 from deltacat.compute.compactor.model.pyarrow_write_result import PyArrowWriteResult
 from deltacat.compute.compactor import RoundCompletionInfo, DeltaFileEnvelope
 from deltacat.utils.common import ReadKwargsProvider
 from contextlib import nullcontext
 from deltacat.utils.ray_utils.runtime import (
     get_current_ray_task_id,
@@ -265,14 +266,32 @@
         input.round_completion_info
         and input.round_completion_info.hb_index_to_entry_range
         and input.round_completion_info.hb_index_to_entry_range.get(str(hb_idx))
         is not None
     )
 
 
+def _can_copy_by_reference(
+    has_delete: bool, merge_file_group: MergeFileGroup, input: MergeInput
+) -> bool:
+    """
+    Can copy by reference only if there are no deletes to merge in
+    and previous compacted stream id matches that of new stream
+    """
+    return (
+        not has_delete
+        and not merge_file_group.dfe_groups
+        and input.round_completion_info is not None
+        and (
+            input.write_to_partition.stream_id
+            == input.round_completion_info.compacted_delta_locator.stream_id
+        )
+    )
+
+
 def _flatten_dfe_list(
     df_envelopes_list: List[List[DeltaFileEnvelope]],
 ) -> List[DeltaFileEnvelope]:
     """
     Flattens a list of lists of DeltaFileEnvelope objects into a single list of DeltaFileEnvelope objects.
 
     Args:
@@ -345,15 +364,15 @@
         hb_idx (int): The hash bucket index for the compaction.
 
     Returns:
         Tuple[pa.Table, int, int, int]: A tuple containing:
             1. The compacted PyArrow table.
             2. The total number of records in the incremental data.
             3. The total number of deduplicated records.
-            4. The total number of dropped records due to DELETE operations.
+            4. The total number of deleted records due to DELETE operations.
     """
     df_envelopes: List[DeltaFileEnvelope] = _flatten_dfe_list(dfe_list)
     delete_file_envelopes = input.delete_file_envelopes or []
     reordered_all_dfes: List[DeltaFileEnvelope] = _sort_df_envelopes(
         delete_file_envelopes + df_envelopes
     )
     assert all(
@@ -475,18 +494,20 @@
         for merge_file_group in merge_file_groups:
             compacted_table = None
             has_delete = input.delete_file_envelopes is not None
             if has_delete:
                 assert (
                     input.delete_strategy is not None
                 ), "Merge input missing delete_strategy"
-            if not has_delete and not merge_file_group.dfe_groups:
-                # Can copy by reference only if there are no deletes to merge in
+            if _can_copy_by_reference(
+                has_delete=has_delete, merge_file_group=merge_file_group, input=input
+            ):
                 hb_index_copy_by_ref_ids.append(merge_file_group.hb_index)
                 continue
+
             if _has_previous_compacted_table(input, merge_file_group.hb_index):
                 compacted_table = _download_compacted_table(
                     hb_index=merge_file_group.hb_index,
                     rcf=input.round_completion_info,
                     read_kwargs_provider=input.read_kwargs_provider,
                     deltacat_storage=input.deltacat_storage,
                     deltacat_storage_kwargs=input.deltacat_storage_kwargs,
@@ -544,15 +565,16 @@
         # Log node peak memory utilization every 10 seconds
         def log_peak_memory():
             logger.debug(
                 f"Process peak memory utilization so far: {process_util.max_memory} bytes "
                 f"({process_util.max_memory/BYTES_PER_GIBIBYTE} GB)"
             )
 
-        process_util.schedule_callback(log_peak_memory, 10)
+        if input.memory_logs_enabled:
+            process_util.schedule_callback(log_peak_memory, 10)
 
         merge_result, duration = timed_invocation(func=_timed_merge, input=input)
 
         emit_metrics_time = 0.0
         if input.metrics_config:
             emit_result, latency = timed_invocation(
                 func=emit_timer_metrics,
```

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/content_type_params.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/content_type_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/dedupe.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/delta.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/io.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/merge.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/compactor_v2/utils/primary_key_index.py` & `deltacat-1.1.1/deltacat/compute/compactor_v2/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/merge_on_read/daft.py` & `deltacat-1.1.1/deltacat/compute/merge_on_read/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/merge_on_read/model/merge_on_read_params.py` & `deltacat-1.1.1/deltacat/compute/merge_on_read/model/merge_on_read_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/merge_on_read/utils/delta.py` & `deltacat-1.1.1/deltacat/compute/merge_on_read/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/meta_stats.py` & `deltacat-1.1.1/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-1.1.1/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-1.1.1/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/stats.py` & `deltacat-1.1.1/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/utils/constants.py` & `deltacat-1.1.1/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/utils/io.py` & `deltacat-1.1.1/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-1.1.1/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-1.1.1/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/basic.py` & `deltacat-1.1.1/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-1.1.1/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/models/delta_stats.py` & `deltacat-1.1.1/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-1.1.1/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-1.1.1/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/models/stats_result.py` & `deltacat-1.1.1/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/utils/intervals.py` & `deltacat-1.1.1/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/utils/io.py` & `deltacat-1.1.1/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-1.1.1/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/constants.py` & `deltacat-1.1.1/deltacat/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-1.1.1/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/dataset.py` & `deltacat-1.1.1/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/file_object_store.py` & `deltacat-1.1.1/deltacat/io/file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/memcached_object_store.py` & `deltacat-1.1.1/deltacat/io/memcached_object_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,23 +177,43 @@
 
         client = self._get_client_by_ip(ip)
         serialized = bytearray()
 
         for chunk_index in range(chunk_count):
             ref = self._create_ref(uid, ip, chunk_index)
             chunk = client.get(ref)
+            if chunk is None:
+                raise ValueError(
+                    f"Expected uid: {uid}, chunk index: {chunk_index} from client ip: {ip}"
+                    f" to be non-empty."
+                )
             serialized.extend(chunk)
 
         return cloudpickle.loads(serialized)
 
+    def clear(self) -> bool:
+        flushed = all(
+            [
+                self._get_client_by_ip(ip).flush_all(noreply=False)
+                for ip in self.storage_node_ips
+            ]
+        )
+        self.client_cache.clear()
+
+        if flushed:
+            logger.info("Successfully cleared cache contents.")
+
+        return flushed
+
     def close(self) -> None:
         for client in self.client_cache.values():
             client.close()
 
         self.client_cache.clear()
+        logger.info("Successfully closed object store clients.")
 
     def _create_ref(self, uid, ip, chunk_index) -> str:
         return f"{uid}{self.SEPARATOR}{ip}{self.SEPARATOR}{chunk_index}"
 
     def _get_storage_node_ip(self, key: str):
         storage_node_ip = self.hasher.get_node(key)
         return storage_node_ip
```

### Comparing `deltacat-1.1.0/deltacat/io/object_store.py` & `deltacat-1.1.1/deltacat/io/object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/ray_plasma_object_store.py` & `deltacat-1.1.1/deltacat/io/ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/read_api.py` & `deltacat-1.1.1/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/redis_object_store.py` & `deltacat-1.1.1/deltacat/io/redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/io/s3_object_store.py` & `deltacat-1.1.1/deltacat/io/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/logs.py` & `deltacat-1.1.1/deltacat/logs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 import pathlib
 from logging import FileHandler, Handler, Logger, LoggerAdapter, handlers
-from typing import Union
+from typing import Any, Dict, Optional, Union
 
 import ray
 from ray.runtime_context import RuntimeContext
 
 from deltacat.constants import (
     DELTACAT_APP_LOG_LEVEL,
     DELTACAT_SYS_LOG_LEVEL,
@@ -22,15 +22,40 @@
 DEFAULT_LOG_FORMAT = (
     "%(asctime)s\t%(levelname)s pid=%(process)d %(filename)s:%(lineno)s -- %(message)s"
 )
 DEFAULT_MAX_BYTES_PER_LOG = 2 ^ 20 * 256  # 256 MiB
 DEFAULT_BACKUP_COUNT = 0
 
 
-class RayRuntimeContextLoggerAdapter(logging.LoggerAdapter):
+class DeltaCATLoggerAdapter(logging.LoggerAdapter):
+    """
+    Logger Adapter class with additional functionality
+    """
+
+    def __init__(self, logger: Logger, extra: Optional[Dict[str, Any]] = {}):
+        super().__init__(logger, extra)
+
+    def debug_conditional(self, msg, do_print: bool, *args, **kwargs):
+        if do_print:
+            self.debug(msg, *args, **kwargs)
+
+    def info_conditional(self, msg, do_print: bool, *args, **kwargs):
+        if do_print:
+            self.info(msg, *args, **kwargs)
+
+    def warning_conditional(self, msg, do_print: bool, *args, **kwargs):
+        if do_print:
+            self.warning(msg, *args, **kwargs)
+
+    def error_conditional(self, msg, do_print: bool, *args, **kwargs):
+        if do_print:
+            self.error(msg, *args, **kwargs)
+
+
+class RayRuntimeContextLoggerAdapter(DeltaCATLoggerAdapter):
     """
     Logger Adapter for injecting Ray Runtime Context into logging messages.
     """
 
     def __init__(self, logger: Logger, runtime_context: RuntimeContext):
         super().__init__(logger, {})
         self.runtime_context = runtime_context
@@ -143,14 +168,16 @@
             log_dir, log_base_file_name, primary_log_level
         )
         _add_logger_handler(logger, handler)
     if ray.is_initialized():
         ray_runtime_ctx = ray.get_runtime_context()
         if ray_runtime_ctx.worker.connected:
             logger = RayRuntimeContextLoggerAdapter(logger, ray_runtime_ctx)
+    else:
+        logger = DeltaCATLoggerAdapter(logger)
 
     return logger
 
 
 def configure_deltacat_logger(logger: Logger) -> Union[Logger, LoggerAdapter]:
     return _configure_logger(
         logger,
```

### Comparing `deltacat-1.1.0/deltacat/storage/__init__.py` & `deltacat-1.1.1/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/interface.py` & `deltacat-1.1.1/deltacat/storage/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/delete_parameters.py` & `deltacat-1.1.1/deltacat/storage/model/delete_parameters.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/delta.py` & `deltacat-1.1.1/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/list_result.py` & `deltacat-1.1.1/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/locator.py` & `deltacat-1.1.1/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/namespace.py` & `deltacat-1.1.1/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/partition.py` & `deltacat-1.1.1/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/sort_key.py` & `deltacat-1.1.1/deltacat/storage/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/stream.py` & `deltacat-1.1.1/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/table.py` & `deltacat-1.1.1/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/table_version.py` & `deltacat-1.1.1/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/storage/model/types.py` & `deltacat-1.1.1/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/aws/test_clients.py` & `deltacat-1.1.1/deltacat/tests/aws/test_clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/catalog/test_default_catalog_impl.py` & `deltacat-1.1.1/deltacat/tests/catalog/test_default_catalog_impl.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py` & `deltacat-1.1.1/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compact_partition_test_cases.py` & `deltacat-1.1.1/deltacat/tests/compute/compact_partition_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compactor/steps/test_repartition.py` & `deltacat-1.1.1/deltacat/tests/compute/compactor/steps/test_repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compactor/utils/test_io.py` & `deltacat-1.1.1/deltacat/tests/compute/compactor/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compactor_v2/test_compaction_session.py` & `deltacat-1.1.1/deltacat/tests/compute/compactor_v2/test_compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/compactor_v2/utils/test_task_options.py` & `deltacat-1.1.1/deltacat/tests/compute/compactor_v2/utils/test_task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_incremental.py` & `deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_params.py` & `deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                     },
                     "streamId": "foobar",
                     "storageType": "fooType",
                 },
                 "partitionValues": [],
                 "partitionId": "79612ea39ac5493eae925abe60767d42",
             },
+            "memory_logs_enabled": True,
             "metrics_config": MetricsConfig("us-east-1", MetricsTarget.CLOUDWATCH_EMF),
         }
 
         super().setUpClass()
 
     def test_serialize_returns_json_string(self):
         from deltacat.compute.compactor.model.compact_partition_params import (
@@ -132,14 +133,18 @@
             == params.source_partition_locator
         )
         assert (
             json.loads(serialized_params)["destination_partition_locator"]
             == params.destination_partition_locator
         )
         assert (
+            json.loads(serialized_params)["memory_logs_enabled"]
+            == params.memory_logs_enabled
+        )
+        assert (
             json.loads(serialized_params)["metrics_config"]["metrics_target"]
             == params.metrics_config.metrics_target
         )
 
     def test_serialize_handles_sets(self):
         from deltacat.compute.compactor.model.compact_partition_params import (
             CompactPartitionParams,
```

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py` & `deltacat-1.1.1/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_util_common.py` & `deltacat-1.1.1/deltacat/tests/compute/test_util_common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_util_constant.py` & `deltacat-1.1.1/deltacat/tests/compute/test_util_constant.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/compute/test_util_create_table_deltas_repo.py` & `deltacat-1.1.1/deltacat/tests/compute/test_util_create_table_deltas_repo.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_cloudpickle_bug_fix.py` & `deltacat-1.1.1/deltacat/tests/io/test_cloudpickle_bug_fix.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_file_object_store.py` & `deltacat-1.1.1/deltacat/tests/io/test_file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_memcached_object_store.py` & `deltacat-1.1.1/deltacat/tests/io/test_memcached_object_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     def set(self, key, value, *args, **kwargs):
         self.store[key] = value
         return True
 
     def get(self, key, *args, **kwargs):
         return self.store.get(key)
 
+    def flush_all(self, *args, **kwargs):
+        for key, value in self.store.items():
+            self.store[key] = None
+
 
 class TestMemcachedObjectStore(unittest.TestCase):
 
     TEST_VALUE_LARGE = "test-value-greater-than-10-bytes"
 
     def setUp(self):
         from deltacat.io.memcached_object_store import MemcachedObjectStore
@@ -188,7 +192,22 @@
 
         # action
         ref = object_store.put(self.TEST_VALUE_LARGE)
 
         # assert
         result = self.object_store.get(ref)
         self.assertEqual(result, self.TEST_VALUE_LARGE)
+
+    @mock.patch("deltacat.io.memcached_object_store.Client")
+    @mock.patch("deltacat.io.memcached_object_store.RetryingClient")
+    def test_clear_sanity(self, mock_retrying_client, mock_client):
+        # setup
+        mock_client.return_value = MockPyMemcacheClient()
+        mock_retrying_client.return_value = mock_client.return_value
+
+        # action
+        ref = self.object_store.put(self.TEST_VALUE_LARGE)
+        self.object_store.clear()
+
+        # assert
+        with self.assertRaises(ValueError):
+            self.object_store.get(ref)
```

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_ray_plasma_object_store.py` & `deltacat-1.1.1/deltacat/tests/io/test_ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_redis_object_store.py` & `deltacat-1.1.1/deltacat/tests/io/test_redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/io/test_s3_object_store.py` & `deltacat-1.1.1/deltacat/tests/io/test_s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/local_deltacat_storage/__init__.py` & `deltacat-1.1.1/deltacat/tests/local_deltacat_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/stats/test_intervals.py` & `deltacat-1.1.1/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/test_utils/pyarrow.py` & `deltacat-1.1.1/deltacat/tests/test_utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/test_utils/storage.py` & `deltacat-1.1.1/deltacat/tests/test_utils/storage.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/utils/test_cloudpickle.py` & `deltacat-1.1.1/deltacat/tests/utils/test_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/utils/test_daft.py` & `deltacat-1.1.1/deltacat/tests/utils/test_daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/utils/test_pyarrow.py` & `deltacat-1.1.1/deltacat/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/utils/test_record_batch_tables.py` & `deltacat-1.1.1/deltacat/tests/utils/test_record_batch_tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/tests/utils/test_resources.py` & `deltacat-1.1.1/deltacat/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/types/media.py` & `deltacat-1.1.1/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/types/partial_download.py` & `deltacat-1.1.1/deltacat/types/partial_download.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/types/tables.py` & `deltacat-1.1.1/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/arguments.py` & `deltacat-1.1.1/deltacat/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/cloudpickle.py` & `deltacat-1.1.1/deltacat/utils/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/common.py` & `deltacat-1.1.1/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/daft.py` & `deltacat-1.1.1/deltacat/utils/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/metrics.py` & `deltacat-1.1.1/deltacat/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/numpy.py` & `deltacat-1.1.1/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/pandas.py` & `deltacat-1.1.1/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/performance.py` & `deltacat-1.1.1/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/placement.py` & `deltacat-1.1.1/deltacat/utils/placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/pyarrow.py` & `deltacat-1.1.1/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/ray_utils/collections.py` & `deltacat-1.1.1/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/ray_utils/concurrency.py` & `deltacat-1.1.1/deltacat/utils/ray_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/ray_utils/dataset.py` & `deltacat-1.1.1/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/ray_utils/runtime.py` & `deltacat-1.1.1/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/resources.py` & `deltacat-1.1.1/deltacat/utils/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,21 +32,23 @@
             if (
                 isinstance(cluster_resources[key], float)
                 or isinstance(cluster_resources[key], int)
             ) and key in available_resources:
                 used_resources[key] = cluster_resources[key] - available_resources[key]
 
         self.total_memory_bytes = cluster_resources.get("memory")
-        self.used_memory_bytes = used_resources.get("memory")
+        self.used_memory_bytes = used_resources.get("memory", 0.0)
         self.total_cpu = cluster_resources.get("CPU")
-        self.used_cpu = used_resources.get("CPU")
+        self.used_cpu = used_resources.get("CPU", 0)
         self.total_object_store_memory_bytes = cluster_resources.get(
             "object_store_memory"
         )
-        self.used_object_store_memory_bytes = used_resources.get("object_store_memory")
+        self.used_object_store_memory_bytes = used_resources.get(
+            "object_store_memory", 0.0
+        )
         self.used_memory_percent = (
             self.used_memory_bytes / self.total_memory_bytes
         ) * 100
         self.used_object_store_memory_percent = (
             self.used_object_store_memory_bytes / self.total_object_store_memory_bytes
         ) * 100
         self.used_cpu_percent = (self.used_cpu / self.total_cpu) * 100
```

### Comparing `deltacat-1.1.0/deltacat/utils/s3fs.py` & `deltacat-1.1.1/deltacat/utils/s3fs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat/utils/schema.py` & `deltacat-1.1.1/deltacat/utils/schema.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/deltacat.egg-info/PKG-INFO` & `deltacat-1.1.1/deltacat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.0
+Version: 1.1.1
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.0/deltacat.egg-info/SOURCES.txt` & `deltacat-1.1.1/deltacat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.0/setup.py` & `deltacat-1.1.1/setup.py`

 * *Files identical despite different names*

