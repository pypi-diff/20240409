# Comparing `tmp/pixeltable-0.2.2.tar.gz` & `tmp/pixeltable-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.2.tar", max compression
+gzip compressed data, was "pixeltable-0.2.3.tar", max compression
```

## Comparing `pixeltable-0.2.2.tar` & `pixeltable-0.2.3.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      746 2024-01-15 22:21:10.025602 pixeltable-0.2.2/LICENSE
--rw-r--r--   0        0        0     4193 2024-04-05 01:34:32.679704 pixeltable-0.2.2/README.md
--rw-r--r--   0        0        0      959 2024-04-04 15:03:13.491688 pixeltable-0.2.2/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-29 02:10:24.349472 pixeltable-0.2.2/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-02 22:13:56.668343 pixeltable-0.2.2/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     8661 2024-04-04 15:03:13.492105 pixeltable-0.2.2/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-29 02:10:24.350840 pixeltable-0.2.2/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-29 02:10:24.351032 pixeltable-0.2.2/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8280 2024-04-04 15:03:13.492541 pixeltable-0.2.2/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-29 02:10:24.351974 pixeltable-0.2.2/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-04 15:03:13.492968 pixeltable-0.2.2/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-04 15:03:13.493364 pixeltable-0.2.2/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-29 02:10:24.352764 pixeltable-0.2.2/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    25499 2024-04-04 15:03:13.493856 pixeltable-0.2.2/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    35680 2024-04-04 15:03:13.494406 pixeltable-0.2.2/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5461 2024-04-04 15:03:13.495287 pixeltable-0.2.2/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-02 22:13:56.672469 pixeltable-0.2.2/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    20548 2024-04-04 15:03:13.495950 pixeltable-0.2.2/pixeltable/client.py
--rw-r--r--   0        0        0    28339 2024-04-05 01:34:32.701874 pixeltable-0.2.2/pixeltable/dataframe.py
--rw-r--r--   0        0        0    16398 2024-04-05 01:34:32.702438 pixeltable-0.2.2/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-01-15 22:21:10.095679 pixeltable-0.2.2/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-01-15 22:21:10.095882 pixeltable-0.2.2/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-02 22:13:56.674688 pixeltable-0.2.2/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5104 2024-03-29 02:10:24.358353 pixeltable-0.2.2/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-29 02:10:24.358711 pixeltable-0.2.2/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-29 02:10:24.359053 pixeltable-0.2.2/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-29 02:10:24.359224 pixeltable-0.2.2/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-01-15 22:21:10.096673 pixeltable-0.2.2/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-02 22:13:56.675099 pixeltable-0.2.2/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     2949 2024-03-29 02:10:24.359831 pixeltable-0.2.2/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-01-15 22:21:10.097303 pixeltable-0.2.2/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-29 02:10:24.360143 pixeltable-0.2.2/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-04 15:03:13.497550 pixeltable-0.2.2/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-29 02:10:24.360769 pixeltable-0.2.2/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-29 02:10:24.361026 pixeltable-0.2.2/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-29 02:10:24.361259 pixeltable-0.2.2/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-29 02:10:24.361503 pixeltable-0.2.2/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     3000 2024-03-29 02:10:24.361847 pixeltable-0.2.2/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-29 02:10:24.362201 pixeltable-0.2.2/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     7535 2024-01-15 22:21:10.098798 pixeltable-0.2.2/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-02 22:13:56.676458 pixeltable-0.2.2/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-01-15 22:21:10.099182 pixeltable-0.2.2/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-04 15:03:13.526393 pixeltable-0.2.2/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-01-15 22:21:10.099445 pixeltable-0.2.2/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-29 02:10:24.364993 pixeltable-0.2.2/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-29 02:10:24.365419 pixeltable-0.2.2/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-29 02:10:24.366065 pixeltable-0.2.2/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-29 02:10:24.366678 pixeltable-0.2.2/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-29 02:10:24.367023 pixeltable-0.2.2/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-29 02:10:24.368455 pixeltable-0.2.2/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-29 02:10:24.368997 pixeltable-0.2.2/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     1885 2024-03-29 02:10:24.369311 pixeltable-0.2.2/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-01-15 22:21:10.100425 pixeltable-0.2.2/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-29 02:10:24.374640 pixeltable-0.2.2/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    16992 2024-04-02 22:13:56.677709 pixeltable-0.2.2/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-29 02:10:24.376127 pixeltable-0.2.2/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-29 02:10:24.376650 pixeltable-0.2.2/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-04 15:03:13.527090 pixeltable-0.2.2/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      457 2024-04-04 15:03:13.584303 pixeltable-0.2.2/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-04 15:03:13.601913 pixeltable-0.2.2/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-04 15:03:13.602549 pixeltable-0.2.2/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-04 15:03:13.602985 pixeltable-0.2.2/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3392 2024-04-04 15:03:13.603326 pixeltable-0.2.2/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-04 15:03:13.603679 pixeltable-0.2.2/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-04 15:03:13.604235 pixeltable-0.2.2/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1220 2024-04-04 15:03:13.604579 pixeltable-0.2.2/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-04 15:03:13.604966 pixeltable-0.2.2/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7107 2024-04-04 15:03:13.605389 pixeltable-0.2.2/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6457 2024-04-04 15:03:13.605802 pixeltable-0.2.2/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3419 2024-04-04 15:03:13.606222 pixeltable-0.2.2/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-02 22:13:56.685253 pixeltable-0.2.2/pixeltable/functions/eval.py
--rw-r--r--   0        0        0     1596 2024-04-04 15:03:13.606866 pixeltable-0.2.2/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     4804 2024-04-04 15:03:13.607357 pixeltable-0.2.2/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-04 15:03:13.607789 pixeltable-0.2.2/pixeltable/functions/image.py
--rw-r--r--   0        0        0     2863 2024-04-04 20:32:17.201830 pixeltable-0.2.2/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-04 15:03:13.608251 pixeltable-0.2.2/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-02 22:13:56.687559 pixeltable-0.2.2/pixeltable/functions/string.py
--rw-r--r--   0        0        0      650 2024-04-04 15:03:13.608761 pixeltable-0.2.2/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1596 2024-04-02 22:13:56.688834 pixeltable-0.2.2/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-02 22:13:56.689676 pixeltable-0.2.2/pixeltable/functions/video.py
--rw-r--r--   0        0        0       70 2024-01-15 22:21:10.104617 pixeltable-0.2.2/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-29 02:10:24.389524 pixeltable-0.2.2/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13088 2024-03-29 02:10:24.390315 pixeltable-0.2.2/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-29 02:10:24.390700 pixeltable-0.2.2/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-04 15:03:13.609220 pixeltable-0.2.2/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-29 02:10:24.391424 pixeltable-0.2.2/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     7761 2024-04-02 22:13:56.690669 pixeltable-0.2.2/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    34710 2024-04-04 15:03:13.609842 pixeltable-0.2.2/pixeltable/plan.py
--rw-r--r--   0        0        0    19230 2024-04-02 22:13:56.691931 pixeltable-0.2.2/pixeltable/store.py
--rw-r--r--   0        0        0     6677 2024-04-04 21:05:30.616015 pixeltable-0.2.2/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     3186 2024-04-04 15:03:13.610924 pixeltable-0.2.2/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-01-15 22:21:10.632434 pixeltable-0.2.2/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-04 15:03:13.611478 pixeltable-0.2.2/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    17732 2024-04-04 21:05:30.639792 pixeltable-0.2.2/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    17686 2024-04-04 15:03:13.612660 pixeltable-0.2.2/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-04 15:03:13.613238 pixeltable-0.2.2/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5657 2024-04-04 15:03:13.613735 pixeltable-0.2.2/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32695 2024-04-04 15:03:13.614257 pixeltable-0.2.2/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12817 2024-04-04 15:03:13.614623 pixeltable-0.2.2/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0    14394 2024-04-05 01:34:32.702868 pixeltable-0.2.2/pixeltable/tests/test_functions.py
--rw-r--r--   0        0        0     1535 2024-04-04 15:03:13.615516 pixeltable-0.2.2/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-04 15:03:13.615912 pixeltable-0.2.2/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0     9297 2024-04-04 15:03:13.616356 pixeltable-0.2.2/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    48202 2024-04-04 15:03:13.617029 pixeltable-0.2.2/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-04 15:03:13.617428 pixeltable-0.2.2/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0      970 2024-04-04 15:03:13.617805 pixeltable-0.2.2/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7676 2024-04-04 15:03:13.618199 pixeltable-0.2.2/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    21859 2024-04-04 15:03:13.618642 pixeltable-0.2.2/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0    10213 2024-04-04 21:05:30.640283 pixeltable-0.2.2/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5148 2024-04-04 15:03:13.619429 pixeltable-0.2.2/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0     2899 2024-04-04 21:05:30.640709 pixeltable-0.2.2/pixeltable/tool/create_test_video.py
--rw-r--r--   0        0        0    31781 2024-04-04 20:32:17.202919 pixeltable-0.2.2/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-01-15 22:21:10.635863 pixeltable-0.2.2/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0      720 2024-01-15 22:21:10.635981 pixeltable-0.2.2/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-29 02:10:24.462374 pixeltable-0.2.2/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-29 02:10:24.462842 pixeltable-0.2.2/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-29 02:10:24.463396 pixeltable-0.2.2/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-01-15 22:21:10.636442 pixeltable-0.2.2/pixeltable/utils/help.py
--rw-r--r--   0        0        0     3116 2024-03-29 02:10:24.463930 pixeltable-0.2.2/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     5775 2024-01-15 22:21:10.636686 pixeltable-0.2.2/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     6515 2024-04-04 15:03:13.619950 pixeltable-0.2.2/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-01-15 22:21:10.636985 pixeltable-0.2.2/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-01-15 22:21:10.637081 pixeltable-0.2.2/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-04 15:03:13.620278 pixeltable-0.2.2/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3284 2024-04-05 01:34:32.726498 pixeltable-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 pixeltable-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-03-22 03:20:30.854989 pixeltable-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4193 2024-04-06 17:38:28.064844 pixeltable-0.2.3/README.md
+-rw-r--r--   0        0        0      959 2024-04-04 00:11:47.491970 pixeltable-0.2.3/pixeltable/__init__.py
+-rw-r--r--   0        0        0      453 2024-03-22 03:20:30.929081 pixeltable-0.2.3/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.492457 pixeltable-0.2.3/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     8661 2024-04-04 00:11:47.492730 pixeltable-0.2.3/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-22 03:20:30.929659 pixeltable-0.2.3/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-22 03:20:30.929786 pixeltable-0.2.3/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8280 2024-04-04 00:11:47.492972 pixeltable-0.2.3/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.930368 pixeltable-0.2.3/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.493163 pixeltable-0.2.3/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.493341 pixeltable-0.2.3/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.931044 pixeltable-0.2.3/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    25499 2024-04-04 00:11:47.493604 pixeltable-0.2.3/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    35680 2024-04-04 00:11:47.493943 pixeltable-0.2.3/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5461 2024-04-04 00:11:47.494156 pixeltable-0.2.3/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.494389 pixeltable-0.2.3/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    20548 2024-04-04 00:11:47.494657 pixeltable-0.2.3/pixeltable/client.py
+-rw-r--r--   0        0        0    28339 2024-04-06 17:38:28.087008 pixeltable-0.2.3/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    16398 2024-04-06 17:38:28.087581 pixeltable-0.2.3/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-03-22 03:20:30.937922 pixeltable-0.2.3/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      412 2024-03-22 03:20:30.938153 pixeltable-0.2.3/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.495476 pixeltable-0.2.3/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5212 2024-04-08 22:50:04.684752 pixeltable-0.2.3/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.939348 pixeltable-0.2.3/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.939513 pixeltable-0.2.3/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-22 03:20:30.939633 pixeltable-0.2.3/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.939748 pixeltable-0.2.3/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.495696 pixeltable-0.2.3/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     2949 2024-03-22 03:20:30.941553 pixeltable-0.2.3/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.945244 pixeltable-0.2.3/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.945695 pixeltable-0.2.3/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      935 2024-04-04 00:11:47.495925 pixeltable-0.2.3/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.948503 pixeltable-0.2.3/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.948806 pixeltable-0.2.3/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.949036 pixeltable-0.2.3/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.949236 pixeltable-0.2.3/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     3000 2024-03-22 03:20:30.949375 pixeltable-0.2.3/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.949509 pixeltable-0.2.3/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     8046 2024-04-08 22:50:04.685112 pixeltable-0.2.3/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.496409 pixeltable-0.2.3/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.954653 pixeltable-0.2.3/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.496718 pixeltable-0.2.3/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.958471 pixeltable-0.2.3/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.958665 pixeltable-0.2.3/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.958803 pixeltable-0.2.3/pixeltable/exprs/image_similarity_predicate.py
+-rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.958978 pixeltable-0.2.3/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.959427 pixeltable-0.2.3/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.959589 pixeltable-0.2.3/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.959717 pixeltable-0.2.3/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.959875 pixeltable-0.2.3/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     1885 2024-03-22 03:20:30.960091 pixeltable-0.2.3/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.960205 pixeltable-0.2.3/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.960322 pixeltable-0.2.3/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    16992 2024-04-04 00:11:47.497017 pixeltable-0.2.3/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.962221 pixeltable-0.2.3/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.962353 pixeltable-0.2.3/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.497543 pixeltable-0.2.3/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      457 2024-04-04 00:11:47.497746 pixeltable-0.2.3/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-04 00:11:47.497895 pixeltable-0.2.3/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.498062 pixeltable-0.2.3/pixeltable/func/batched_function.py
+-rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.498480 pixeltable-0.2.3/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     3392 2024-04-04 00:11:47.498601 pixeltable-0.2.3/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.498783 pixeltable-0.2.3/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.498985 pixeltable-0.2.3/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1220 2024-04-04 00:11:47.499364 pixeltable-0.2.3/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.499601 pixeltable-0.2.3/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     7107 2024-04-04 00:11:47.499798 pixeltable-0.2.3/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6457 2024-04-04 00:11:47.499973 pixeltable-0.2.3/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3419 2024-04-04 00:11:47.500386 pixeltable-0.2.3/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8453 2024-04-04 00:11:47.500621 pixeltable-0.2.3/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0     1596 2024-04-06 17:37:50.512896 pixeltable-0.2.3/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     4804 2024-04-04 00:11:47.500918 pixeltable-0.2.3/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-04 00:11:47.501186 pixeltable-0.2.3/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     2863 2024-04-04 00:11:47.501300 pixeltable-0.2.3/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.501525 pixeltable-0.2.3/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-04 00:11:47.501661 pixeltable-0.2.3/pixeltable/functions/string.py
+-rw-r--r--   0        0        0      650 2024-04-04 00:11:47.501927 pixeltable-0.2.3/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1596 2024-04-04 00:11:47.502099 pixeltable-0.2.3/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.502279 pixeltable-0.2.3/pixeltable/functions/video.py
+-rw-r--r--   0        0        0       70 2024-03-22 03:20:30.970568 pixeltable-0.2.3/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.970760 pixeltable-0.2.3/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.685460 pixeltable-0.2.3/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.991846 pixeltable-0.2.3/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.502483 pixeltable-0.2.3/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-22 03:20:30.992614 pixeltable-0.2.3/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0     7761 2024-04-04 00:11:47.502834 pixeltable-0.2.3/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    34710 2024-04-04 00:11:47.503153 pixeltable-0.2.3/pixeltable/plan.py
+-rw-r--r--   0        0        0    19511 2024-04-08 22:50:04.685849 pixeltable-0.2.3/pixeltable/store.py
+-rw-r--r--   0        0        0     6677 2024-04-06 17:38:28.088257 pixeltable-0.2.3/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.504570 pixeltable-0.2.3/pixeltable/tests/test_audio.py
+-rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.514506 pixeltable-0.2.3/pixeltable/tests/test_catalog.py
+-rw-r--r--   0        0        0      531 2024-04-04 00:11:47.504789 pixeltable-0.2.3/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0    17732 2024-04-06 17:38:28.114456 pixeltable-0.2.3/pixeltable/tests/test_component_view.py
+-rw-r--r--   0        0        0    18007 2024-04-08 22:50:04.686513 pixeltable-0.2.3/pixeltable/tests/test_dataframe.py
+-rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.505572 pixeltable-0.2.3/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.384273 pixeltable-0.2.3/pixeltable/tests/test_document.py
+-rw-r--r--   0        0        0    32743 2024-04-08 22:50:04.687225 pixeltable-0.2.3/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0    12817 2024-04-04 00:11:47.506385 pixeltable-0.2.3/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0    14394 2024-04-06 17:38:28.115085 pixeltable-0.2.3/pixeltable/tests/test_functions.py
+-rw-r--r--   0        0        0     1535 2024-04-04 00:11:47.506868 pixeltable-0.2.3/pixeltable/tests/test_migration.py
+-rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.507072 pixeltable-0.2.3/pixeltable/tests/test_nos.py
+-rw-r--r--   0        0        0     9297 2024-04-04 00:11:47.507288 pixeltable-0.2.3/pixeltable/tests/test_snapshot.py
+-rw-r--r--   0        0        0    48484 2024-04-06 17:38:32.384895 pixeltable-0.2.3/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.507879 pixeltable-0.2.3/pixeltable/tests/test_transactional_directory.py
+-rw-r--r--   0        0        0      970 2024-04-04 00:11:47.508085 pixeltable-0.2.3/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     7782 2024-04-06 17:38:32.385556 pixeltable-0.2.3/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0    21859 2024-04-04 00:11:47.508548 pixeltable-0.2.3/pixeltable/tests/test_view.py
+-rw-r--r--   0        0        0    10378 2024-04-08 22:50:04.687903 pixeltable-0.2.3/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     5148 2024-04-04 00:11:47.508980 pixeltable-0.2.3/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.116159 pixeltable-0.2.3/pixeltable/tool/create_test_video.py
+-rw-r--r--   0        0        0    31798 2024-04-08 22:50:04.688715 pixeltable-0.2.3/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-03-22 03:20:31.517814 pixeltable-0.2.3/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0      720 2024-03-22 03:20:31.517938 pixeltable-0.2.3/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.518069 pixeltable-0.2.3/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.518173 pixeltable-0.2.3/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.518306 pixeltable-0.2.3/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-03-22 03:20:31.518421 pixeltable-0.2.3/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.518536 pixeltable-0.2.3/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     5775 2024-03-22 03:20:31.518658 pixeltable-0.2.3/pixeltable/utils/parquet.py
+-rw-r--r--   0        0        0     6515 2024-04-04 00:11:47.509542 pixeltable-0.2.3/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-03-22 03:20:31.518890 pixeltable-0.2.3/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-03-22 03:20:31.519000 pixeltable-0.2.3/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.509715 pixeltable-0.2.3/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     3267 2024-04-08 22:50:04.692841 pixeltable-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 pixeltable-0.2.3/PKG-INFO
```

### Comparing `pixeltable-0.2.2/LICENSE` & `pixeltable-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/README.md` & `pixeltable-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/__init__.py` & `pixeltable-0.2.3/pixeltable/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/catalog.py` & `pixeltable-0.2.3/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/column.py` & `pixeltable-0.2.3/pixeltable/catalog/column.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/dir.py` & `pixeltable-0.2.3/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/globals.py` & `pixeltable-0.2.3/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.3/pixeltable/catalog/insertable_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/named_function.py` & `pixeltable-0.2.3/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/path.py` & `pixeltable-0.2.3/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.3/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.3/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/table.py` & `pixeltable-0.2.3/pixeltable/catalog/table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/table_version.py` & `pixeltable-0.2.3/pixeltable/catalog/table_version.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.3/pixeltable/catalog/table_version_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/catalog/view.py` & `pixeltable-0.2.3/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/client.py` & `pixeltable-0.2.3/pixeltable/client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/dataframe.py` & `pixeltable-0.2.3/pixeltable/dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/env.py` & `pixeltable-0.2.3/pixeltable/env.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.3/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.3/pixeltable/exec/cache_prefetch_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
-from typing import List, Optional, Any, Tuple, Dict
+
+import concurrent.futures
+import logging
 import threading
+import urllib.parse
+import urllib.request
 from collections import defaultdict
-from uuid import UUID
-import concurrent
-import logging
-import urllib
 from pathlib import Path
+from typing import List, Optional, Any, Tuple, Dict
+from uuid import UUID
 
-from .data_row_batch import DataRowBatch
-from .exec_node import ExecNode
-import pixeltable.exprs as exprs
-from pixeltable.utils.filecache import FileCache
 import pixeltable.env as env
 import pixeltable.exceptions as excs
+import pixeltable.exprs as exprs
+from pixeltable.utils.filecache import FileCache
+from .data_row_batch import DataRowBatch
+from .exec_node import ExecNode
 
 _logger = logging.getLogger('pixeltable')
 
 class CachePrefetchNode(ExecNode):
     """Brings files with external URLs into the cache
 
     TODO:
@@ -77,29 +79,30 @@
 
         return input_batch
 
     def _fetch_url(self, row: exprs.DataRow, slot_idx: int) -> Optional[str]:
         """Fetches a remote URL into Env.tmp_dir and returns its path"""
         url = row.file_urls[slot_idx]
         parsed = urllib.parse.urlparse(url)
-        assert parsed.scheme != '' and parsed.scheme != 'file'
+        # Use len(parsed.scheme) > 1 here to ensure we're not being passed
+        # a Windows filename
+        assert len(parsed.scheme) > 1 and parsed.scheme != 'file'
         # preserve the file extension, if there is one
         extension = ''
         if parsed.path != '':
             p = Path(urllib.parse.unquote(parsed.path))
             extension = p.suffix
         tmp_path = env.Env.get().create_tmp_path(extension=extension)
         try:
             if parsed.scheme == 's3':
                 from pixeltable.utils.s3 import get_client
                 with self.boto_client_lock:
                     if self.boto_client is None:
                         self.boto_client = get_client()
                     self.boto_client.download_file(parsed.netloc, parsed.path.lstrip('/'), str(tmp_path))
-                    return tmp_path
             elif parsed.scheme == 'http' or parsed.scheme == 'https':
                 with urllib.request.urlopen(url) as resp, open(tmp_path, 'wb') as f:
                     data = resp.read()
                     f.write(data)
             else:
                 assert False, f'Unsupported URL scheme: {parsed.scheme}'
             return tmp_path
```

### Comparing `pixeltable-0.2.2/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.3/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.3/pixeltable/exec/data_row_batch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/exec_context.py` & `pixeltable-0.2.3/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/exec_node.py` & `pixeltable-0.2.3/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.3/pixeltable/exec/expr_eval_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.3/pixeltable/exec/in_memory_data_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.3/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.3/pixeltable/exec/sql_scan_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/__init__.py` & `pixeltable-0.2.3/pixeltable/exprs/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.3/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.3/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.3/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.3/pixeltable/exprs/column_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/comparison.py` & `pixeltable-0.2.3/pixeltable/exprs/comparison.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.3/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/data_row.py` & `pixeltable-0.2.3/pixeltable/exprs/data_row.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
-from typing import Optional, List, Any, Tuple
+
 import io
-import urllib
+import urllib.parse
+import urllib.request
+from typing import Optional, List, Any, Tuple
 
 import PIL
 import numpy as np
 
 
 class DataRow:
     """
@@ -100,14 +102,15 @@
         assert self.has_val[index], index
 
         if self.file_urls[index] is not None and index in self.img_slot_idxs:
             # if we need to load this from a file, it should have been materialized locally
             assert self.file_paths[index] is not None
             if self.vals[index] is None:
                 self.vals[index] = PIL.Image.open(self.file_paths[index])
+                self.vals[index].load()
 
         return self.vals[index]
 
     def get_stored_val(self, index: object) -> Any:
         """Return the value that gets stored in the db"""
         assert self.excs[index] is None
         if not self.has_val[index]:
@@ -133,22 +136,27 @@
         This allows overwriting
         """
         assert self.excs[idx] is None
 
         if (idx in self.img_slot_idxs or idx in self.media_slot_idxs) and isinstance(val, str):
             # this is either a local file path or a URL
             parsed = urllib.parse.urlparse(val)
-            if parsed.scheme == '' or parsed.scheme == 'file':
+            # Determine if this is a local file or a remote URL. If the scheme length is <= 1,
+            # we assume it's a local file. (This is because a Windows path will be interpreted
+            # by urllib as a URL with scheme equal to the drive letter.)
+            if len(parsed.scheme) <= 1 or parsed.scheme == 'file':
                 # local file path
                 assert self.file_urls[idx] is None and self.file_paths[idx] is None
-                if parsed.scheme == '':
-                    self.file_urls[idx] = urllib.parse.urljoin('file:', urllib.request.pathname2url(parsed.path))
+                if len(parsed.scheme) <= 1:
+                    self.file_urls[idx] = urllib.parse.urljoin('file:', urllib.request.pathname2url(val))
+                    self.file_paths[idx] = val
                 else:
                     self.file_urls[idx] = val
-                self.file_paths[idx] = urllib.parse.unquote(parsed.path)
+                    # Wrap the path in a url2pathname() call to ensure proper handling on Windows.
+                    self.file_paths[idx] = urllib.parse.unquote(urllib.request.url2pathname(parsed.path))
             else:
                 # URL
                 assert self.file_urls[idx] is None
                 self.file_urls[idx] = val
 
             if idx in self.media_slot_idxs:
                 self.vals[idx] = self.file_paths[idx] if self.file_paths[idx] is not None else self.file_urls[idx]
```

### Comparing `pixeltable-0.2.2/pixeltable/exprs/expr.py` & `pixeltable-0.2.3/pixeltable/exprs/expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.3/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/function_call.py` & `pixeltable-0.2.3/pixeltable/exprs/function_call.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/globals.py` & `pixeltable-0.2.3/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.3/pixeltable/exprs/image_member_access.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/image_similarity_predicate.py` & `pixeltable-0.2.3/pixeltable/exprs/image_similarity_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.3/pixeltable/exprs/inline_array.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.3/pixeltable/exprs/inline_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/is_null.py` & `pixeltable-0.2.3/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.3/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/json_path.py` & `pixeltable-0.2.3/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/literal.py` & `pixeltable-0.2.3/pixeltable/exprs/literal.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.3/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/predicate.py` & `pixeltable-0.2.3/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.3/pixeltable/exprs/row_builder.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.3/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.3/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/exprs/variable.py` & `pixeltable-0.2.3/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.3/pixeltable/func/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/batched_function.py` & `pixeltable-0.2.3/pixeltable/func/batched_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/callable_function.py` & `pixeltable-0.2.3/pixeltable/func/callable_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.3/pixeltable/func/expr_template_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/function.py` & `pixeltable-0.2.3/pixeltable/func/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/function_registry.py` & `pixeltable-0.2.3/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/globals.py` & `pixeltable-0.2.3/pixeltable/func/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/nos_function.py` & `pixeltable-0.2.3/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/signature.py` & `pixeltable-0.2.3/pixeltable/func/signature.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/func/udf.py` & `pixeltable-0.2.3/pixeltable/func/udf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/__init__.py` & `pixeltable-0.2.3/pixeltable/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/eval.py` & `pixeltable-0.2.3/pixeltable/functions/eval.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/fireworks.py` & `pixeltable-0.2.3/pixeltable/functions/fireworks.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/huggingface.py` & `pixeltable-0.2.3/pixeltable/functions/huggingface.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/openai.py` & `pixeltable-0.2.3/pixeltable/functions/openai.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/pil/image.py` & `pixeltable-0.2.3/pixeltable/functions/pil/image.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/string.py` & `pixeltable-0.2.3/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/together.py` & `pixeltable-0.2.3/pixeltable/functions/together.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/util.py` & `pixeltable-0.2.3/pixeltable/functions/util.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/functions/video.py` & `pixeltable-0.2.3/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/iterators/base.py` & `pixeltable-0.2.3/pixeltable/iterators/base.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/iterators/document.py` & `pixeltable-0.2.3/pixeltable/iterators/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self, document: str, *, separators: str, limit: int = 0, overlap: int = 0, metadata: str = '',
             html_skip_tags: List[str] = None, tiktoken_encoding: Optional[str] = 'cl100k_base',
             tiktoken_target_model: Optional[str] = None
     ):
         import bs4
         if html_skip_tags is None:
             html_skip_tags = ['nav']
-        with open(document, 'r') as fh:
+        with open(document, 'r', encoding='utf8') as fh:
             s = fh.read()
             self._doc_handle = get_document_handle(s)
             assert self._doc_handle is not None
         self._separators = [Separator[s.upper()] for s in separators.split(',')]
         self._md_fields = [ChunkMetadata[m.upper()] for m in metadata.split(',')] if len(metadata) > 0 else []
         self._doc_title = \
             self._doc_handle.bs_doc.title.get_text().strip() if self._doc_handle.bs_doc is not None else ''
```

### Comparing `pixeltable-0.2.2/pixeltable/iterators/video.py` & `pixeltable-0.2.3/pixeltable/iterators/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/metadata/__init__.py` & `pixeltable-0.2.3/pixeltable/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.3/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/metadata/schema.py` & `pixeltable-0.2.3/pixeltable/metadata/schema.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/plan.py` & `pixeltable-0.2.3/pixeltable/plan.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/store.py` & `pixeltable-0.2.3/pixeltable/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
+import abc
+import logging
 import os
 import sys
+import urllib.parse
+import urllib.request
 import warnings
 from typing import Optional, Dict, Any, List, Tuple, Set
-import logging
-import urllib
+
 import sqlalchemy as sql
 from tqdm import tqdm, TqdmWarning
-import abc
 
 import pixeltable.catalog as catalog
+import pixeltable.env as env
+from pixeltable import exprs
+import pixeltable.exceptions as excs
+from pixeltable.exec import ExecNode
 from pixeltable.metadata import schema
 from pixeltable.type_system import StringType
-from pixeltable.exec import ExecNode
-from pixeltable import exprs
-from pixeltable.utils.sql import log_stmt, log_explain
-import pixeltable.env as env
 from pixeltable.utils.media_store import MediaStore
-
+from pixeltable.utils.sql import log_stmt, log_explain
 
 _logger = logging.getLogger('pixeltable')
 
 
 class StoreBase:
     """Base class for stored tables
 
@@ -117,18 +119,21 @@
 
     def _move_tmp_media_file(self, file_url: Optional[str], col: catalog.Column, v_min: int) -> str:
         """Move tmp media file with given url to Env.media_dir and return new url, or given url if not a tmp_dir file"""
         pxt_tmp_dir = str(env.Env.get().tmp_dir)
         if file_url is None:
             return None
         parsed = urllib.parse.urlparse(file_url)
-        if parsed.scheme != '' and parsed.scheme != 'file':
+        # We should never be passed a local file path here. The "len > 1" ensures that Windows
+        # file paths aren't mistaken for URLs with a single-character scheme.
+        assert len(parsed.scheme) > 1
+        if parsed.scheme != 'file':
             # remote url
             return file_url
-        file_path = urllib.parse.unquote(parsed.path)
+        file_path = urllib.parse.unquote(urllib.request.url2pathname(parsed.path))
         if not file_path.startswith(pxt_tmp_dir):
             # not a tmp file
             return file_url
         _, ext = os.path.splitext(file_path)
         new_path = str(MediaStore.prepare_media_path(self.tbl_version.id, col.id, v_min, ext=ext))
         os.rename(file_path, new_path)
         new_file_url = urllib.parse.urljoin('file:', urllib.request.pathname2url(new_path))
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/conftest.py` & `pixeltable-0.2.3/pixeltable/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_audio.py` & `pixeltable-0.2.3/pixeltable/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_catalog.py` & `pixeltable-0.2.3/pixeltable/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_client.py` & `pixeltable-0.2.3/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_component_view.py` & `pixeltable-0.2.3/pixeltable/tests/test_component_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_dataframe.py` & `pixeltable-0.2.3/pixeltable/tests/test_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pathlib import Path
 from typing import Any, Dict
 
 import bs4
 import numpy as np
 import pytest
 import requests
-from pycocotools.coco import COCO
 
 import pixeltable as pxt
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import get_video_files, get_audio_files, skip_test_if_not_installed
 
@@ -180,14 +179,16 @@
             _ = t.where(t.img.width > 100).count()
 
     def test_select_literal(self, test_tbl: catalog.Table) -> None:
         t = test_tbl
         res = t.select(1.0).where(t.c2 < 10).collect()
         assert res[res.column_names()[0]] == [1.0] * 10
 
+    # TODO This test doesn't work on Windows due to reliance on the structure of file URLs
+    @pytest.mark.skip('Test is not portable')
     def test_html_media_url(self, test_client: pxt.Client) -> None:
         tab = test_client.create_table('test_html_repr', {'video': pxt.VideoType(), 'audio': pxt.AudioType()})
         status = tab.insert(video=get_video_files()[0], audio=get_audio_files()[0])
         assert status.num_rows == 1
         assert status.num_excs == 0
 
         res = tab.select(tab.video, tab.audio).collect()
@@ -204,14 +205,15 @@
             for src in sources:
                 response = requests.get(src['src'])
                 assert response.status_code == 200
 
     def test_to_pytorch_dataset(self, all_datatypes_tbl: catalog.Table):
         """ tests all types are handled correctly in this conversion
         """
+        skip_test_if_not_installed('torch')
         import torch
 
         t = all_datatypes_tbl
         df = t.where(t.row_id < 1)
         assert df.count() > 0
         ds = df.to_pytorch_dataset()
         type_dict = dict(zip(df.get_column_names(),df.get_column_types()))
@@ -234,14 +236,15 @@
             assert torch.is_tensor(tup['c_image'])
             assert isinstance(tup['c_video'], str)
             assert isinstance(tup['c_json'], dict)
 
     def test_to_pytorch_image_format(self, all_datatypes_tbl: catalog.Table) -> None:
         """ tests the image_format parameter is honored
         """
+        skip_test_if_not_installed('torch')
         import torch
         import torchvision.transforms as T
 
         W, H = 220, 224 # make different from each other
         t = all_datatypes_tbl
         df = t.select(
             t.row_id,
@@ -291,14 +294,15 @@
 
     @pytest.mark.skip('Flaky test (fails intermittently)')
     def test_to_pytorch_dataloader(self, all_datatypes_tbl: catalog.Table) -> None:
         """ Tests the dataset works well with pytorch dataloader:
             1. compatibility with multiprocessing
             2. compatibility of all types with default collate_fn
         """
+        skip_test_if_not_installed('torch')
         import torch.utils.data
         @pxt.udf(param_types=[pxt.JsonType()], return_type=pxt.JsonType())
         def restrict_json_for_default_collate(obj):
             keys = ['id', 'label', 'iscrowd', 'bounding_box']
             return {k: obj[k] for k in keys}
         
         t = all_datatypes_tbl
@@ -348,14 +352,15 @@
 
     def test_pytorch_dataset_caching(self, all_datatypes_tbl: catalog.Table) -> None:
         """ Tests that dataset caching works
             1. using the same dataset twice in a row uses the cache
             2. adding a row to the table invalidates the cached version
             3. changing the select list invalidates the cached version
         """
+        skip_test_if_not_installed('torch')
         t = all_datatypes_tbl
 
         t.drop_column('c_video') # null value video column triggers internal assertions in DataRow
         # see https://github.com/pixeltable/pixeltable/issues/38
 
         t.drop_column('c_array') # no support yet for null array values in the pytorch dataset
 
@@ -379,14 +384,15 @@
 
         # check select list invalidation
         ds4 = t.select(t.row_id).to_pytorch_dataset(image_format='pt')
         assert ds4.path != ds3.path, 'different select list, hence different path should be used'
 
     def test_to_coco(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('nos')
+        from pycocotools.coco import COCO
         cl = test_client
         base_t = cl.create_table('videos', {'video': pxt.VideoType()})
         args = {'video': base_t.video, 'fps': 1}
         view_t = cl.create_view('frames', base_t, iterator_class=FrameIterator, iterator_args=args)
         from pixeltable.functions.nos.object_detection_2d import yolox_medium
         view_t.add_column(detections=yolox_medium(view_t.frame))
         base_t.insert(video=get_video_files()[0])
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_dirs.py` & `pixeltable-0.2.3/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_document.py` & `pixeltable-0.2.3/pixeltable/tests/test_document.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional, Set, List
 
 import pytest
 
 import pixeltable as pxt
 from pixeltable.iterators.document import DocumentSplitter
 from pixeltable.tests.utils import get_documents, get_video_files, get_audio_files, get_image_files
+from pixeltable.tests.utils import skip_test_if_not_installed
 from pixeltable.type_system import DocumentType
 
 
 class TestDocument:
     def valid_doc_paths(self) -> List[str]:
         return get_documents()
 
@@ -30,14 +31,15 @@
 
         file_paths = self.invalid_doc_paths()
         status = doc_t.insert(({'doc': p} for p in file_paths), fail_on_exception=False)
         assert status.num_rows == len(file_paths)
         assert status.num_excs == len(file_paths)
 
     def test_doc_splitter(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('tiktoken')
         file_paths = self.valid_doc_paths()
         cl = test_client
         doc_t = cl.create_table('docs', {'doc': DocumentType()})
         status = doc_t.insert({'doc': p} for p in file_paths)
         assert status.num_excs == 0
 
         def normalize(s: str) -> str:
@@ -84,14 +86,15 @@
 
                         assert all_text == all_text_reference, f'{sep1}, {sep2}, {limit}'
                         assert headings == headings_reference, f'{sep1}, {sep2}, {limit}'
                         # TODO: verify chunk limit
                     cl.drop_table('chunks')
 
     def test_doc_splitter_headings(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('spacy')
         file_paths = self.valid_doc_paths()
         cl = test_client
         doc_t = cl.create_table('docs', {'doc': DocumentType()})
         status = doc_t.insert({'doc': p} for p in file_paths)
         assert status.num_excs == 0
 
         # verify that only the requested metadata is present in the view
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_exprs.py` & `pixeltable-0.2.3/pixeltable/tests/test_exprs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import urllib.parse
+import urllib.request
 from typing import List, Dict
 
 import pytest
 import sqlalchemy as sql
 
 import pixeltable as pxt
 import pixeltable.func as func
@@ -170,15 +171,15 @@
         assert res.to_pandas()['error'].isna().all()
 
         img_t = img_tbl
         # fileurl
         res = img_t.select(img_t.img.fileurl).show(0).to_pandas()
         stored_urls = set(res.iloc[:, 0])
         assert len(stored_urls) == len(res)
-        all_urls  = set([urllib.parse.urljoin('file:', path) for path in get_image_files()])
+        all_urls = set(urllib.parse.urljoin('file:', urllib.request.pathname2url(path)) for path in get_image_files())
         assert stored_urls <= all_urls
 
         # localpath
         res = img_t.select(img_t.img.localpath).show(0).to_pandas()
         stored_paths = set(res.iloc[:, 0])
         assert len(stored_paths) == len(res)
         all_paths  = set(get_image_files())
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_function.py` & `pixeltable-0.2.3/pixeltable/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_functions.py` & `pixeltable-0.2.3/pixeltable/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_migration.py` & `pixeltable-0.2.3/pixeltable/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_nos.py` & `pixeltable-0.2.3/pixeltable/tests/test_nos.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_snapshot.py` & `pixeltable-0.2.3/pixeltable/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_table.py` & `pixeltable-0.2.3/pixeltable/tests/test_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import pixeltable.functions as ptf
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import \
     make_tbl, create_table_data, read_data_file, get_video_files, get_audio_files, get_image_files, get_documents, \
     assert_resultset_eq
+from pixeltable.tests.utils import skip_test_if_not_installed
 from pixeltable.type_system import \
     StringType, IntType, FloatType, TimestampType, ImageType, VideoType, JsonType, BoolType, ArrayType, AudioType, \
     DocumentType
 from pixeltable.utils.filecache import FileCache
 from pixeltable.utils.media_store import MediaStore
 
 
@@ -292,14 +293,15 @@
         invalid_doc_paths = [get_video_files()[0], get_audio_files()[0], get_image_files()[0]]
         doc_paths = valid_doc_paths + invalid_doc_paths
         is_valid = [True] * len(valid_doc_paths) + [False] * len(invalid_doc_paths)
         rows = [{'media': f, 'is_bad_media': not is_valid} for f, is_valid in zip(doc_paths, is_valid)]
         self.check_bad_media(test_client, rows, DocumentType(nullable=True))
 
     def test_validate_external_url(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('boto3')
         rows = [
             {'media': 's3://open-images-dataset/validation/doesnotexist.jpg', 'is_bad_media': True},
             {'media': 'https://archive.random.org/download?file=2024-01-28.bin', 'is_bad_media': True},  # 403 error
             {'media': 's3://open-images-dataset/validation/3c02ca9ec9b2b77b.jpg', 'is_bad_media': True},  # wrong media
             # test s3 url
             {
                 'media': 's3://multimedia-commons/data/videos/mp4/ffe/ff3/ffeff3c6bf57504e7a6cecaff6aefbc9.mp4',
@@ -311,14 +313,15 @@
                 'is_bad_media': False
             },
 
         ]
         self.check_bad_media(test_client, rows, VideoType(nullable=True))
 
     def test_create_s3_image_table(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('boto3')
         cl = test_client
         tbl = cl.create_table('test', {'img': ImageType(nullable=False)})
         # this is needed because Client.reset_catalog() doesn't call TableVersion.drop(), which would
         # clear the file cache
         # TODO: change reset_catalog() to drop tables
         FileCache.get().clear()
         cache_stats = FileCache.get().stats()
@@ -367,14 +370,15 @@
 
         # dropping the table also clears the file cache
         cl.drop_table('test')
         cache_stats = FileCache.get().stats()
         assert cache_stats.total_size == 0
 
     def test_video_url(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('boto3')
         cl = test_client
         schema = {
             'payload': IntType(nullable=False),
             'video': VideoType(nullable=False),
         }
         tbl = cl.create_table('test', schema)
         url = 's3://multimedia-commons/data/videos/mp4/ffe/ff3/ffeff3c6bf57504e7a6cecaff6aefbc9.mp4'
@@ -386,14 +390,15 @@
         assert os.path.exists(local_path) and os.path.isfile(local_path)
         cap = cv2.VideoCapture(local_path)
         # TODO: this isn't sufficient to determine that this is actually a video, rather than an image
         assert cap.isOpened()
         cap.release()
 
     def test_create_video_table(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('boto3')
         cl = test_client
         tbl = cl.create_table(
             'test_tbl',
             {'payload': IntType(nullable=False), 'video': VideoType(nullable=True)})
         args = {'video': tbl.video, 'fps': 0}
         view = cl.create_view('test_view', tbl, iterator_class=FrameIterator, iterator_args=args)
         view.add_column(c1=view.frame.rotate(30), stored=True)
@@ -525,14 +530,15 @@
         cl.drop_table('test1', ignore_errors=True)
         t = cl.create_table('test1', {'c5': ArrayType((2, 3), dtype=IntType(), nullable=False)})
         with pytest.raises(excs.Error) as exc_info:
             t.insert(c5=np.ndarray((3, 2)))
         assert 'expected ndarray((2, 3)' in str(exc_info.value)
 
     def test_query(self, test_client: pxt.Client) -> None:
+        skip_test_if_not_installed('boto3')
         cl = test_client
         col_names = ['c1', 'c2', 'c3', 'c4', 'c5']
         t = make_tbl(cl, 'test', col_names)
         rows = create_table_data(t)
         t.insert(rows)
         _ = t.show(n=0)
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_transactional_directory.py` & `pixeltable-0.2.3/pixeltable/tests/test_transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_types.py` & `pixeltable-0.2.3/pixeltable/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_video.py` & `pixeltable-0.2.3/pixeltable/tests/test_video.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 import pixeltable as pxt
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import get_video_files
+from pixeltable.tests.utils import skip_test_if_not_installed
 from pixeltable.type_system import VideoType, ImageType
 from pixeltable.utils.media_store import MediaStore
 
 
 class TestVideo:
     def create_tbls(
             self, cl: pxt.Client, base_name: str = 'video_tbl', view_name: str = 'frame_view'
@@ -57,14 +58,15 @@
 
         # revert() also removes computed images
         tbl.insert({'video': p} for p in video_filepaths)
         tbl.revert()
         assert MediaStore.count(view.get_id()) == view.count()
 
     def test_query(self, test_client: pxt.client) -> None:
+        skip_test_if_not_installed('boto3')
         video_filepaths = get_video_files()
         cl = test_client
         base_t, view_t = self.create_tbls(cl)
         # also include an external file, to make sure that prefetching works
         url = 's3://multimedia-commons/data/videos/mp4/ffe/ff3/ffeff3c6bf57504e7a6cecaff6aefbc9.mp4'
         video_filepaths.append(url)
         status = base_t.insert({'video': p} for p in video_filepaths)
```

### Comparing `pixeltable-0.2.2/pixeltable/tests/test_view.py` & `pixeltable-0.2.3/pixeltable/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tests/utils.py` & `pixeltable-0.2.3/pixeltable/tests/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -221,49 +221,51 @@
     assert data_file_path.is_file(), f'Not a file: {str(data_file_path)}'
     df = pd.read_csv(str(data_file_path))
     for col_name in path_col_names:
         assert col_name in df.columns
         df[col_name] = df.apply(lambda r: str(abs_path / r[col_name]), axis=1)
     return df.to_dict(orient='records')
 
-def get_video_files(include_bad_video=False) -> List[str]:
+def get_video_files(include_bad_video: bool = False) -> List[str]:
     tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/videos/*', recursive=True)
     if not include_bad_video:
         glob_result = [f for f in glob_result if 'bad_video' not in f]
 
     half_res = [f for f in glob_result if 'half_res' in f or 'bad_video' in f]
     return half_res
 
 def get_test_video_files() -> List[str]:
     tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/test_videos/*', recursive=True)
     return glob_result
 
-def get_image_files() -> List[str]:
+def get_image_files(include_bad_image: bool = False) -> List[str]:
     tests_dir = os.path.dirname(__file__) # search with respect to tests/ dir
     glob_result = glob.glob(f'{tests_dir}/**/imagenette2-160/*', recursive=True)
+    if not include_bad_image:
+        glob_result = [f for f in glob_result if 'bad_image' not in f]
     return glob_result
 
-def get_audio_files(include_bad_audio=False) -> List[str]:
+def get_audio_files(include_bad_audio: bool = False) -> List[str]:
     tests_dir = os.path.dirname(__file__)
     glob_result = glob.glob(f'{tests_dir}/**/audio/*', recursive=True)
     if not include_bad_audio:
         glob_result = [f for f in glob_result if 'bad_audio' not in f]
     return glob_result
 
 def get_documents() -> List[str]:
     tests_dir = os.path.dirname(__file__)
     # for now, we can only handle .html and .md
     return [p for p in glob.glob(f'{tests_dir}/**/documents/*', recursive=True) if not p.endswith('.pdf')]
 
 def get_sentences(n: int = 100) -> List[str]:
     tests_dir = os.path.dirname(__file__)
     path = glob.glob(f'{tests_dir}/**/jeopardy.json', recursive=True)[0]
-    with open(path, 'r') as f:
+    with open(path, 'r', encoding='utf8') as f:
         questions_list = json.load(f)
     # this dataset contains \' around the questions
     return [q['question'].replace("'", '') for q in questions_list[:n]]
 
 def assert_resultset_eq(r1: DataFrameResultSet, r2: DataFrameResultSet) -> None:
     assert len(r1) == len(r2)
     assert len(r1.column_names()) == len(r2.column_names())  # we don't care about the actual column names
```

### Comparing `pixeltable-0.2.2/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.3/pixeltable/tool/create_test_db_dump.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/tool/create_test_video.py` & `pixeltable-0.2.3/pixeltable/tool/create_test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/type_system.py` & `pixeltable-0.2.3/pixeltable/type_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -907,15 +907,15 @@
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         from pixeltable.utils.documents import get_document_handle
-        with open(val, 'r') as fh:
+        with open(val, 'r', encoding='utf8') as fh:
             try:
                 s = fh.read()
                 dh = get_document_handle(s)
                 if dh is None:
                     raise excs.Error(f'Not a recognized document format: {val}')
             except Exception as e:
                 raise excs.Error(f'Not a recognized document format: {val}') from None
```

### Comparing `pixeltable-0.2.2/pixeltable/utils/clip.py` & `pixeltable-0.2.3/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/coco.py` & `pixeltable-0.2.3/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/documents.py` & `pixeltable-0.2.3/pixeltable/utils/documents.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/filecache.py` & `pixeltable-0.2.3/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/media_store.py` & `pixeltable-0.2.3/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/parquet.py` & `pixeltable-0.2.3/pixeltable/utils/parquet.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/pytorch.py` & `pixeltable-0.2.3/pixeltable/utils/pytorch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/sql.py` & `pixeltable-0.2.3/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.3/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.2/pyproject.toml` & `pixeltable-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.2"
+version = "0.2.3"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
     "pixeltable/tests/data"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-numpy = "^1.24.1"
+numpy = "^1.26"
 pandas = ">=2.0,<3.0"
 pillow = "^9.4.0"
 opencv-python-headless = "^4.7.0.68"
 tqdm = "^4.64.1"
 jmespath = "^1.0.1"
 regex = "^2022.10.31"
 cloudpickle = "^2.2.1"
 psycopg2-binary = "^2.9.5"
 psutil = "^5.9.5"
 sqlalchemy = {extras = ["mypy"], version = "^2.0.23"}
 sqlalchemy-utils = "^0.41.1"
 pgvector = "^0.2.1"
 av = ">=10.0.0"
+beautifulsoup4 = "^4.0.0"
+requests = "^2.31.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
-pgserver = "0.0.7"
+pgserver = "0.0.9"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
 pytest = "^7.2.1"
@@ -57,28 +59,25 @@
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 mkdocs-material = "^9.5.3"
 mkdocs-jupyter = "^0.24"
 # other
 pycocotools = "^2.0.7"
 ipykernel = "^6.27.1"
 nbmake = "^1.4.6"
-bs4 = "^0.0.2"
-requests = "^2.31.0"
 # packages required by various optional pieces of the codebase
 torch = "^2.2"
 torchvision = "^0.17"
 pyarrow = ">=13.0.0"
 openai = "^1.0.0"
 together = "^0.2.11"
 fireworks-ai = "^0.13.0"
 boto3 = "^1.17"
 spacy = "^3.0"
 en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1-py3-none-any.whl"}
 tiktoken = ">=0.3"
-beautifulsoup4 = "^4.0.0"
 sentence-transformers = "^2.0.0"
 transformers = "^4.20"
 
 [tool.mypy]
 plugins = "sqlalchemy.ext.mypy.plugin"
 disallow_untyped_defs = true
 disallow_any_unimported = true
```

### Comparing `pixeltable-0.2.2/PKG-INFO` & `pixeltable-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.2
+Version: 0.2.3
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: av (>=10.0.0)
+Requires-Dist: beautifulsoup4 (>=4.0.0,<5.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: numpy (>=1.26,<2.0)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
-Requires-Dist: pgserver (==0.0.7)
+Requires-Dist: pgserver (==0.0.9)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.23,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img src="docs/pixeltable-banner.png" width="45%"/>
```

