# Comparing `tmp/fused-1.5.2.tar.gz` & `tmp/fused-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fused-1.5.2.tar", max compression
+gzip compressed data, was "fused-1.5.3.tar", max compression
```

## Comparing `fused-1.5.2.tar` & `fused-1.5.3.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.2/README.md
--rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.2/fused/MIGRATION_VERSION
--rw-r--r--   0        0        0     1111 2024-04-01 22:41:30.718989 fused-1.5.2/fused/__init__.py
--rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.2/fused/__main__.py
--rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.2/fused/_auth.py
--rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.2/fused/_cache/__init__.py
--rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.2/fused/_cache/memory.py
--rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.2/fused/_constants.py
--rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.2/fused/_deserialize.py
--rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.2/fused/_deserialize_parquet.py
--rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.2/fused/_environment.py
--rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.2/fused/_experimental.py
--rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.2/fused/_formatter/common.py
--rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.2/fused/_formatter/formatter_dataset.py
--rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.2/fused/_formatter/formatter_eval_result.py
--rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.2/fused/_formatter/formatter_job_config.py
--rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.2/fused/_formatter/formatter_jobs.py
--rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.2/fused/_formatter/formatter_options.py
--rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.2/fused/_formatter/formatter_project.py
--rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.2/fused/_formatter/formatter_templates.py
--rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.2/fused/_formatter/formatter_udf_access_token.py
--rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.2/fused/_formatter/noraise.py
--rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.2/fused/_formatter/template.py
--rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.2/fused/_formatter/udf.py
--rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.2/fused/_global_api.py
--rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.2/fused/_load_udf.py
--rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.2/fused/_magic/__init__.py
--rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.2/fused/_magic/magics.py
--rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.2/fused/_magic/output.py
--rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.2/fused/_options.py
--rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.2/fused/_project.py
--rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.2/fused/_public_api.py
--rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.2/fused/_quick/__init__.py
--rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.2/fused/_quick/udf.py
--rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.2/fused/_raster/__init__.py
--rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.2/fused/_raster/signer.py
--rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.2/fused/_raster/stac.py
--rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.2/fused/_registry.py
--rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.2/fused/_request.py
--rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.2/fused/_run.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.2/fused/_static/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.2/fused/_static/css/__init__.py
--rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.2/fused/_static/css/style.css
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.2/fused/_static/html/__init__.py
--rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.2/fused/_static/html/icons-svg-inline.html
--rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.2/fused/_static/templates/__init__.py
--rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.2/fused/_str_utils.py
--rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.2/fused/_templates/__init__.py
--rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.2/fused/_templates/loaders.py
--rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.2/fused/_templates/templates.py
--rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.2/fused/_udf/__init__.py
--rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.2/fused/_udf/coerce.py
--rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.2/fused/_udf/context.py
--rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.2/fused/_udf/decorators.py
--rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.2/fused/_udf/execute_v2.py
--rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.2/fused/_udf/load.py
--rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.2/fused/_udf/noop_decorators.py
--rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.2/fused/_udf/state.py
--rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.2/fused/_utils.py
--rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.2/fused/api/__init__.py
--rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.2/fused/api/_open_dataset.py
--rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.2/fused/api/_public_api.py
--rw-r--r--   0        0        0    48807 2024-04-01 21:12:17.248568 fused-1.5.2/fused/api/api.py
--rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.2/fused/api/credentials.py
--rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.2/fused/api/docker_api.py
--rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.2/fused/api/docker_http_api.py
--rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.2/fused/cli.py
--rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.2/fused/core/__init__.py
--rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.2/fused/core/_cache.py
--rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.2/fused/core/_download.py
--rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.2/fused/core/_impl/_context_impl.py
--rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.2/fused/core/_impl/_download_impl.py
--rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.2/fused/core/_impl/_realtime_ops_impl.py
--rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.2/fused/core/_impl/_reimports.py
--rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.2/fused/core/_impl/_table_ops_impl.py
--rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.2/fused/core/_impl/_udf_ops_impl.py
--rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.2/fused/core/_realtime_ops.py
--rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.2/fused/core/_table_ops.py
--rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.2/fused/core/_udf_ops.py
--rw-r--r--   0        0        0      795 2024-02-16 20:07:37.390060 fused-1.5.2/fused/models/__init__.py
--rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.2/fused/models/_codegen/__init__.py
--rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.2/fused/models/_codegen/job.py
--rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.2/fused/models/_codegen/udf.py
--rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.2/fused/models/_inplace.py
--rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.2/fused/models/_project_aware.py
--rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.2/fused/models/api/__init__.py
--rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.2/fused/models/api/_folder.py
--rw-r--r--   0        0        0    34461 2024-03-25 21:04:06.818813 fused-1.5.2/fused/models/api/dataset.py
--rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.2/fused/models/api/enums.py
--rw-r--r--   0        0        0    77407 2024-03-04 17:12:17.771506 fused-1.5.2/fused/models/api/job.py
--rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.2/fused/models/api/udf_access_token.py
--rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.2/fused/models/base.py
--rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.2/fused/models/coerce_dataset.py
--rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.2/fused/models/input.py
--rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.2/fused/models/internal/__init__.py
--rw-r--r--   0        0        0     8519 2023-10-13 17:39:24.951254 fused-1.5.2/fused/models/internal/dataset.py
--rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.2/fused/models/internal/job.py
--rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.2/fused/models/migrations.py
--rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.2/fused/models/request.py
--rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.2/fused/models/schema.py
--rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.2/fused/models/udf/__init__.py
--rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.2/fused/models/udf/_eval_result.py
--rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.2/fused/models/udf/_specialized_udfs.py
--rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.2/fused/models/udf/_udf_registry.py
--rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.2/fused/models/udf/base_udf.py
--rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.2/fused/models/udf/common.py
--rw-r--r--   0        0        0     6026 2024-04-01 22:41:07.810512 fused-1.5.2/fused/models/udf/header.py
--rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.2/fused/models/udf/output.py
--rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.2/fused/models/udf/udf.py
--rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.2/fused/models/urls.py
--rw-r--r--   0        0        0     7940 2023-10-13 17:39:24.956442 fused-1.5.2/fused/models/viz.py
--rw-r--r--   0        0        0      671 2023-10-13 17:39:24.956576 fused-1.5.2/fused/models/viz_colors.py
--rw-r--r--   0        0        0     1126 2023-10-13 17:39:24.956677 fused-1.5.2/fused/models/viz_presets.py
--rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.2/fused/types.py
--rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.2/fused/warnings.py
--rw-r--r--   0        0        0     3111 2024-04-01 22:41:30.708448 fused-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1144 2024-03-14 18:20:20.452694 fused-1.5.3/README.md
+-rw-r--r--   0        0        0        6 2023-10-13 17:39:24.936083 fused-1.5.3/fused/MIGRATION_VERSION
+-rw-r--r--   0        0        0     1111 2024-04-09 19:05:19.867615 fused-1.5.3/fused/__init__.py
+-rw-r--r--   0        0        0       66 2023-08-29 21:43:53.192271 fused-1.5.3/fused/__main__.py
+-rw-r--r--   0        0        0    10367 2024-03-01 23:09:39.488200 fused-1.5.3/fused/_auth.py
+-rw-r--r--   0        0        0       66 2023-10-13 17:39:24.936596 fused-1.5.3/fused/_cache/__init__.py
+-rw-r--r--   0        0        0     1401 2023-10-13 17:39:24.936653 fused-1.5.3/fused/_cache/memory.py
+-rw-r--r--   0        0        0       77 2023-10-13 17:39:24.936726 fused-1.5.3/fused/_constants.py
+-rw-r--r--   0        0        0     4181 2023-10-13 17:39:24.936791 fused-1.5.3/fused/_deserialize.py
+-rw-r--r--   0        0        0      287 2023-10-13 17:39:24.937361 fused-1.5.3/fused/_deserialize_parquet.py
+-rw-r--r--   0        0        0     2504 2023-10-13 17:39:24.937551 fused-1.5.3/fused/_environment.py
+-rw-r--r--   0        0        0      357 2024-02-29 19:31:09.757442 fused-1.5.3/fused/_experimental.py
+-rw-r--r--   0        0        0     2364 2024-02-29 19:31:09.757801 fused-1.5.3/fused/_formatter/common.py
+-rw-r--r--   0        0        0    14878 2024-02-27 23:12:15.998414 fused-1.5.3/fused/_formatter/formatter_dataset.py
+-rw-r--r--   0        0        0    11761 2024-01-03 19:21:18.331904 fused-1.5.3/fused/_formatter/formatter_eval_result.py
+-rw-r--r--   0        0        0    16550 2023-10-13 20:24:00.322327 fused-1.5.3/fused/_formatter/formatter_job_config.py
+-rw-r--r--   0        0        0     6962 2024-02-27 23:12:15.998885 fused-1.5.3/fused/_formatter/formatter_jobs.py
+-rw-r--r--   0        0        0     2020 2023-10-13 17:39:24.939257 fused-1.5.3/fused/_formatter/formatter_options.py
+-rw-r--r--   0        0        0     7031 2023-10-13 17:39:24.939757 fused-1.5.3/fused/_formatter/formatter_project.py
+-rw-r--r--   0        0        0     1939 2024-02-29 19:31:09.758102 fused-1.5.3/fused/_formatter/formatter_templates.py
+-rw-r--r--   0        0        0     5370 2024-02-16 20:07:37.387760 fused-1.5.3/fused/_formatter/formatter_udf_access_token.py
+-rw-r--r--   0        0        0     1013 2023-10-13 17:39:24.940039 fused-1.5.3/fused/_formatter/noraise.py
+-rw-r--r--   0        0        0     5379 2024-02-29 19:31:09.758573 fused-1.5.3/fused/_formatter/template.py
+-rw-r--r--   0        0        0    11611 2024-02-07 21:35:13.328473 fused-1.5.3/fused/_formatter/udf.py
+-rw-r--r--   0        0        0      905 2023-10-13 17:39:24.940709 fused-1.5.3/fused/_global_api.py
+-rw-r--r--   0        0        0     2752 2024-04-01 21:12:17.245535 fused-1.5.3/fused/_load_udf.py
+-rw-r--r--   0        0        0      721 2023-10-13 17:39:24.940878 fused-1.5.3/fused/_magic/__init__.py
+-rw-r--r--   0        0        0     2853 2024-02-27 23:12:15.999392 fused-1.5.3/fused/_magic/magics.py
+-rw-r--r--   0        0        0      608 2023-10-13 17:39:24.941393 fused-1.5.3/fused/_magic/output.py
+-rw-r--r--   0        0        0     7783 2024-04-01 21:12:17.246431 fused-1.5.3/fused/_options.py
+-rw-r--r--   0        0        0    39426 2024-04-01 21:12:17.247134 fused-1.5.3/fused/_project.py
+-rw-r--r--   0        0        0    32913 2024-04-01 21:12:17.247928 fused-1.5.3/fused/_public_api.py
+-rw-r--r--   0        0        0       40 2024-02-29 19:31:09.759028 fused-1.5.3/fused/_quick/__init__.py
+-rw-r--r--   0        0        0    16830 2024-03-04 22:08:50.310839 fused-1.5.3/fused/_quick/udf.py
+-rw-r--r--   0        0        0      118 2024-02-29 19:31:09.759558 fused-1.5.3/fused/_raster/__init__.py
+-rw-r--r--   0        0        0     1431 2024-02-29 19:31:09.759769 fused-1.5.3/fused/_raster/signer.py
+-rw-r--r--   0        0        0     4213 2024-02-29 19:31:09.759965 fused-1.5.3/fused/_raster/stac.py
+-rw-r--r--   0        0        0     1015 2023-10-13 17:39:24.943010 fused-1.5.3/fused/_registry.py
+-rw-r--r--   0        0        0      995 2023-10-13 17:39:24.943187 fused-1.5.3/fused/_request.py
+-rw-r--r--   0        0        0    13798 2024-04-01 21:12:17.248121 fused-1.5.3/fused/_run.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.759996 fused-1.5.3/fused/_static/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.760075 fused-1.5.3/fused/_static/css/__init__.py
+-rw-r--r--   0        0        0     7272 2024-02-29 19:31:09.762187 fused-1.5.3/fused/_static/css/style.css
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762251 fused-1.5.3/fused/_static/html/__init__.py
+-rw-r--r--   0        0        0     3891 2024-02-29 19:31:09.762366 fused-1.5.3/fused/_static/html/icons-svg-inline.html
+-rw-r--r--   0        0        0        0 2024-02-29 19:31:09.762441 fused-1.5.3/fused/_static/templates/__init__.py
+-rw-r--r--   0        0        0     1495 2023-10-18 19:12:32.880479 fused-1.5.3/fused/_str_utils.py
+-rw-r--r--   0        0        0      176 2024-02-29 19:31:09.762566 fused-1.5.3/fused/_templates/__init__.py
+-rw-r--r--   0        0        0      396 2024-02-29 19:31:09.762690 fused-1.5.3/fused/_templates/loaders.py
+-rw-r--r--   0        0        0    15844 2024-02-29 19:31:09.763050 fused-1.5.3/fused/_templates/templates.py
+-rw-r--r--   0        0        0      126 2023-10-13 17:39:24.943664 fused-1.5.3/fused/_udf/__init__.py
+-rw-r--r--   0        0        0     1522 2023-10-13 17:39:24.943754 fused-1.5.3/fused/_udf/coerce.py
+-rw-r--r--   0        0        0      790 2023-10-13 17:39:24.943812 fused-1.5.3/fused/_udf/context.py
+-rw-r--r--   0        0        0     9116 2024-03-04 19:13:44.145677 fused-1.5.3/fused/_udf/decorators.py
+-rw-r--r--   0        0        0     9049 2024-03-04 17:12:17.771016 fused-1.5.3/fused/_udf/execute_v2.py
+-rw-r--r--   0        0        0    14851 2024-02-08 00:33:54.700810 fused-1.5.3/fused/_udf/load.py
+-rw-r--r--   0        0        0      225 2023-10-13 17:39:24.944631 fused-1.5.3/fused/_udf/noop_decorators.py
+-rw-r--r--   0        0        0      659 2023-10-13 17:39:24.944746 fused-1.5.3/fused/_udf/state.py
+-rw-r--r--   0        0        0     3202 2024-04-01 21:12:17.248259 fused-1.5.3/fused/_utils.py
+-rw-r--r--   0        0        0      404 2024-02-27 23:12:16.001476 fused-1.5.3/fused/api/__init__.py
+-rw-r--r--   0        0        0      975 2023-10-13 17:39:24.945994 fused-1.5.3/fused/api/_open_dataset.py
+-rw-r--r--   0        0        0     3586 2023-10-13 17:39:24.946052 fused-1.5.3/fused/api/_public_api.py
+-rw-r--r--   0        0        0    48807 2024-04-01 21:12:17.248568 fused-1.5.3/fused/api/api.py
+-rw-r--r--   0        0        0     3363 2024-03-11 21:21:34.935322 fused-1.5.3/fused/api/credentials.py
+-rw-r--r--   0        0        0    25931 2024-04-01 21:12:17.249314 fused-1.5.3/fused/api/docker_api.py
+-rw-r--r--   0        0        0    16529 2024-04-01 21:12:17.249955 fused-1.5.3/fused/api/docker_http_api.py
+-rw-r--r--   0        0        0      290 2024-02-27 23:12:16.002737 fused-1.5.3/fused/cli.py
+-rw-r--r--   0        0        0      492 2024-03-04 16:53:04.882953 fused-1.5.3/fused/core/__init__.py
+-rw-r--r--   0        0        0    10279 2024-04-01 21:12:17.250418 fused-1.5.3/fused/core/_cache.py
+-rw-r--r--   0        0        0     6513 2024-04-01 21:12:17.250608 fused-1.5.3/fused/core/_download.py
+-rw-r--r--   0        0        0      509 2024-03-01 23:09:39.489541 fused-1.5.3/fused/core/_impl/_context_impl.py
+-rw-r--r--   0        0        0     2995 2024-02-27 23:12:16.003344 fused-1.5.3/fused/core/_impl/_download_impl.py
+-rw-r--r--   0        0        0     1022 2024-03-02 00:21:59.447576 fused-1.5.3/fused/core/_impl/_realtime_ops_impl.py
+-rw-r--r--   0        0        0      254 2024-03-04 16:53:04.883231 fused-1.5.3/fused/core/_impl/_reimports.py
+-rw-r--r--   0        0        0     2427 2024-03-14 21:19:20.148282 fused-1.5.3/fused/core/_impl/_table_ops_impl.py
+-rw-r--r--   0        0        0     1369 2024-03-04 16:53:04.883573 fused-1.5.3/fused/core/_impl/_udf_ops_impl.py
+-rw-r--r--   0        0        0    23387 2024-03-01 23:09:39.489874 fused-1.5.3/fused/core/_realtime_ops.py
+-rw-r--r--   0        0        0     1067 2024-04-01 21:12:17.251472 fused-1.5.3/fused/core/_table_ops.py
+-rw-r--r--   0        0        0     1767 2024-03-04 16:53:04.883828 fused-1.5.3/fused/core/_udf_ops.py
+-rw-r--r--   0        0        0      795 2024-02-16 20:07:37.390060 fused-1.5.3/fused/models/__init__.py
+-rw-r--r--   0        0        0      298 2023-10-13 17:39:24.948177 fused-1.5.3/fused/models/_codegen/__init__.py
+-rw-r--r--   0        0        0     4861 2024-03-04 02:10:26.519019 fused-1.5.3/fused/models/_codegen/job.py
+-rw-r--r--   0        0        0     4280 2024-02-08 00:33:54.701166 fused-1.5.3/fused/models/_codegen/udf.py
+-rw-r--r--   0        0        0      224 2023-10-13 17:39:24.948705 fused-1.5.3/fused/models/_inplace.py
+-rw-r--r--   0        0        0      250 2023-10-13 17:39:24.948775 fused-1.5.3/fused/models/_project_aware.py
+-rw-r--r--   0        0        0      506 2024-02-16 20:07:37.390698 fused-1.5.3/fused/models/api/__init__.py
+-rw-r--r--   0        0        0      221 2023-10-13 17:39:24.949226 fused-1.5.3/fused/models/api/_folder.py
+-rw-r--r--   0        0        0    34461 2024-03-25 21:04:06.818813 fused-1.5.3/fused/models/api/dataset.py
+-rw-r--r--   0        0        0       89 2023-05-12 15:11:04.143892 fused-1.5.3/fused/models/api/enums.py
+-rw-r--r--   0        0        0    77407 2024-03-04 17:12:17.771506 fused-1.5.3/fused/models/api/job.py
+-rw-r--r--   0        0        0     3235 2024-02-16 20:07:37.391066 fused-1.5.3/fused/models/api/udf_access_token.py
+-rw-r--r--   0        0        0     3135 2023-10-13 17:39:24.950268 fused-1.5.3/fused/models/base.py
+-rw-r--r--   0        0        0     1616 2024-03-04 16:53:04.884210 fused-1.5.3/fused/models/coerce_dataset.py
+-rw-r--r--   0        0        0     3223 2024-02-08 20:07:13.852325 fused-1.5.3/fused/models/input.py
+-rw-r--r--   0        0        0      330 2023-10-13 17:39:24.950681 fused-1.5.3/fused/models/internal/__init__.py
+-rw-r--r--   0        0        0     8519 2023-10-13 17:39:24.951254 fused-1.5.3/fused/models/internal/dataset.py
+-rw-r--r--   0        0        0    12158 2023-11-01 00:31:41.970766 fused-1.5.3/fused/models/internal/job.py
+-rw-r--r--   0        0        0     1434 2023-10-13 17:39:24.952019 fused-1.5.3/fused/models/migrations.py
+-rw-r--r--   0        0        0     5221 2024-02-16 20:07:37.391813 fused-1.5.3/fused/models/request.py
+-rw-r--r--   0        0        0    29988 2024-03-25 21:04:06.819025 fused-1.5.3/fused/models/schema.py
+-rw-r--r--   0        0        0      241 2023-10-13 17:39:24.953204 fused-1.5.3/fused/models/udf/__init__.py
+-rw-r--r--   0        0        0     1432 2024-01-03 19:21:18.332999 fused-1.5.3/fused/models/udf/_eval_result.py
+-rw-r--r--   0        0        0     8835 2024-03-04 16:53:21.723025 fused-1.5.3/fused/models/udf/_specialized_udfs.py
+-rw-r--r--   0        0        0      781 2023-10-13 17:39:24.953888 fused-1.5.3/fused/models/udf/_udf_registry.py
+-rw-r--r--   0        0        0    13495 2024-04-01 21:12:35.530426 fused-1.5.3/fused/models/udf/base_udf.py
+-rw-r--r--   0        0        0     5358 2023-10-27 22:44:48.239852 fused-1.5.3/fused/models/udf/common.py
+-rw-r--r--   0        0        0     5927 2024-04-09 19:05:13.177073 fused-1.5.3/fused/models/udf/header.py
+-rw-r--r--   0        0        0     5564 2023-12-11 22:59:41.284263 fused-1.5.3/fused/models/udf/output.py
+-rw-r--r--   0        0        0     3580 2024-03-04 17:12:17.771844 fused-1.5.3/fused/models/udf/udf.py
+-rw-r--r--   0        0        0     1575 2023-10-13 17:39:24.955946 fused-1.5.3/fused/models/urls.py
+-rw-r--r--   0        0        0     7940 2023-10-13 17:39:24.956442 fused-1.5.3/fused/models/viz.py
+-rw-r--r--   0        0        0      671 2023-10-13 17:39:24.956576 fused-1.5.3/fused/models/viz_colors.py
+-rw-r--r--   0        0        0     1126 2023-10-13 17:39:24.956677 fused-1.5.3/fused/models/viz_presets.py
+-rw-r--r--   0        0        0      254 2024-03-11 20:54:28.030281 fused-1.5.3/fused/types.py
+-rw-r--r--   0        0        0      675 2023-10-13 17:39:24.961379 fused-1.5.3/fused/warnings.py
+-rw-r--r--   0        0        0     3111 2024-04-09 19:05:19.861421 fused-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3162 1970-01-01 00:00:00.000000 fused-1.5.3/PKG-INFO
```

### Comparing `fused-1.5.2/README.md` & `fused-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/__init__.py` & `fused-1.5.3/fused/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 from .core import cache, download, get_chunk_from_table, get_chunks_metadata
 
 # Must be later so that models get imported first
 from . import _experimental as experimental  # isort:skip
 
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-__version__ = "1.5.2"
+__version__ = "1.5.3"
```

### Comparing `fused-1.5.2/fused/_auth.py` & `fused-1.5.3/fused/_auth.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_cache/memory.py` & `fused-1.5.3/fused/_cache/memory.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_deserialize.py` & `fused-1.5.3/fused/_deserialize.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_environment.py` & `fused-1.5.3/fused/_environment.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/common.py` & `fused-1.5.3/fused/_formatter/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_dataset.py` & `fused-1.5.3/fused/_formatter/formatter_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_eval_result.py` & `fused-1.5.3/fused/_formatter/formatter_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_job_config.py` & `fused-1.5.3/fused/_formatter/formatter_job_config.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_jobs.py` & `fused-1.5.3/fused/_formatter/formatter_jobs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_options.py` & `fused-1.5.3/fused/_formatter/formatter_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_project.py` & `fused-1.5.3/fused/_formatter/formatter_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_templates.py` & `fused-1.5.3/fused/_formatter/formatter_templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/formatter_udf_access_token.py` & `fused-1.5.3/fused/_formatter/formatter_udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/noraise.py` & `fused-1.5.3/fused/_formatter/noraise.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/template.py` & `fused-1.5.3/fused/_formatter/template.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_formatter/udf.py` & `fused-1.5.3/fused/_formatter/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_global_api.py` & `fused-1.5.3/fused/_global_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_load_udf.py` & `fused-1.5.3/fused/_load_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_magic/__init__.py` & `fused-1.5.3/fused/_magic/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_magic/magics.py` & `fused-1.5.3/fused/_magic/magics.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_magic/output.py` & `fused-1.5.3/fused/_magic/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_options.py` & `fused-1.5.3/fused/_options.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_project.py` & `fused-1.5.3/fused/_project.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_public_api.py` & `fused-1.5.3/fused/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_quick/udf.py` & `fused-1.5.3/fused/_quick/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_raster/signer.py` & `fused-1.5.3/fused/_raster/signer.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_raster/stac.py` & `fused-1.5.3/fused/_raster/stac.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_registry.py` & `fused-1.5.3/fused/_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_request.py` & `fused-1.5.3/fused/_request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_run.py` & `fused-1.5.3/fused/_run.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_static/css/style.css` & `fused-1.5.3/fused/_static/css/style.css`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_static/html/icons-svg-inline.html` & `fused-1.5.3/fused/_static/html/icons-svg-inline.html`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_str_utils.py` & `fused-1.5.3/fused/_str_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_templates/templates.py` & `fused-1.5.3/fused/_templates/templates.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/coerce.py` & `fused-1.5.3/fused/_udf/coerce.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/context.py` & `fused-1.5.3/fused/_udf/context.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/decorators.py` & `fused-1.5.3/fused/_udf/decorators.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/execute_v2.py` & `fused-1.5.3/fused/_udf/execute_v2.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/load.py` & `fused-1.5.3/fused/_udf/load.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_udf/state.py` & `fused-1.5.3/fused/_udf/state.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/_utils.py` & `fused-1.5.3/fused/_utils.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/_open_dataset.py` & `fused-1.5.3/fused/api/_open_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/_public_api.py` & `fused-1.5.3/fused/api/_public_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/api.py` & `fused-1.5.3/fused/api/api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/credentials.py` & `fused-1.5.3/fused/api/credentials.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/docker_api.py` & `fused-1.5.3/fused/api/docker_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/api/docker_http_api.py` & `fused-1.5.3/fused/api/docker_http_api.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_cache.py` & `fused-1.5.3/fused/core/_cache.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_download.py` & `fused-1.5.3/fused/core/_download.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_impl/_download_impl.py` & `fused-1.5.3/fused/core/_impl/_download_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_impl/_realtime_ops_impl.py` & `fused-1.5.3/fused/core/_impl/_realtime_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_impl/_table_ops_impl.py` & `fused-1.5.3/fused/core/_impl/_table_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_impl/_udf_ops_impl.py` & `fused-1.5.3/fused/core/_impl/_udf_ops_impl.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_realtime_ops.py` & `fused-1.5.3/fused/core/_realtime_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_table_ops.py` & `fused-1.5.3/fused/core/_table_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/core/_udf_ops.py` & `fused-1.5.3/fused/core/_udf_ops.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/__init__.py` & `fused-1.5.3/fused/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/_codegen/job.py` & `fused-1.5.3/fused/models/_codegen/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/_codegen/udf.py` & `fused-1.5.3/fused/models/_codegen/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/api/dataset.py` & `fused-1.5.3/fused/models/api/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/api/job.py` & `fused-1.5.3/fused/models/api/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/api/udf_access_token.py` & `fused-1.5.3/fused/models/api/udf_access_token.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/base.py` & `fused-1.5.3/fused/models/base.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/coerce_dataset.py` & `fused-1.5.3/fused/models/coerce_dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/input.py` & `fused-1.5.3/fused/models/input.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/internal/dataset.py` & `fused-1.5.3/fused/models/internal/dataset.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/internal/job.py` & `fused-1.5.3/fused/models/internal/job.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/migrations.py` & `fused-1.5.3/fused/models/migrations.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/request.py` & `fused-1.5.3/fused/models/request.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/schema.py` & `fused-1.5.3/fused/models/schema.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/_eval_result.py` & `fused-1.5.3/fused/models/udf/_eval_result.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/_specialized_udfs.py` & `fused-1.5.3/fused/models/udf/_specialized_udfs.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/_udf_registry.py` & `fused-1.5.3/fused/models/udf/_udf_registry.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/base_udf.py` & `fused-1.5.3/fused/models/udf/base_udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/common.py` & `fused-1.5.3/fused/models/udf/common.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/header.py` & `fused-1.5.3/fused/models/udf/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,18 +81,17 @@
     def write_to_gist(self):
         raise NotImplementedError
 
     def _exec(self) -> Dict[str, Any]:
         """
         Execute the header and return it's locals. This is comparable to importing the header.
         """
-        # TODO: Inject fused here
-        # import fused
-        # exec_globals = {"fused": fused}
-        ret = {}
+        import fused
+
+        ret = {"fused": fused}
         # TODO: Does not raise HeaderSyntaxError here
         exec(self.source_code, ret)
         return ret
 
     def _register_custom_finder(self, preceding_sys_modules):
         module_name = self.module_name
         source_code = self.source_code
@@ -160,12 +159,12 @@
         self.module_name = module_name
         self.source_code = source_code
 
     def create_module(self, spec):
         return None
 
     def exec_module(self, module):
-        # TODO: Inject fused here
-        # import fused
-        # exec_globals = {"fused": fused}
+        import fused
+
+        module.__dict__["fused"] = fused
         # TODO: Does not raise HeaderSyntaxError here
         exec(self.source_code, module.__dict__)
```

### Comparing `fused-1.5.2/fused/models/udf/output.py` & `fused-1.5.3/fused/models/udf/output.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/udf/udf.py` & `fused-1.5.3/fused/models/udf/udf.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/urls.py` & `fused-1.5.3/fused/models/urls.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/viz.py` & `fused-1.5.3/fused/models/viz.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/viz_colors.py` & `fused-1.5.3/fused/models/viz_colors.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/models/viz_presets.py` & `fused-1.5.3/fused/models/viz_presets.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/fused/warnings.py` & `fused-1.5.3/fused/warnings.py`

 * *Files identical despite different names*

### Comparing `fused-1.5.2/pyproject.toml` & `fused-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fused"
 # Version is set to 0.0.0 as the version string is automatically generated by
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "1.5.2"
+version = "1.5.3"
 description = ""
 authors = []
 readme = "README.md"
 packages = [{ include = "fused" }]
 
 [project.urls]
 Homepage = "https://www.fused.io"
```

### Comparing `fused-1.5.2/PKG-INFO` & `fused-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fused
-Version: 1.5.2
+Version: 1.5.3
 Summary: 
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

