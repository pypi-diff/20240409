# Comparing `tmp/roger-3.0.4.tar.gz` & `tmp/roger-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roger-3.0.4.tar", last modified: Wed Jan 10 15:53:46 2024, max compression
+gzip compressed data, was "roger-3.0.5.tar", last modified: Tue Apr  9 09:01:54 2024, max compression
```

## Comparing `roger-3.0.4.tar` & `roger-3.0.5.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.095896 roger-3.0.4/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-3.0.4/LICENSE
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      540 2023-06-22 13:44:17.000000 roger-3.0.4/MANIFEST.in
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7822 2024-01-10 15:53:46.095743 roger-3.0.4/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5956 2023-11-30 13:54:43.000000 roger-3.0.4/README.md
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.058184 roger-3.0.4/bmiroger/
--rw-rw-r--   0 robinschwemmle   (501) staff       (20)      105 2023-09-29 08:56:50.000000 roger-3.0.4/bmiroger/__init__.py
--rw-rw-r--   0 robinschwemmle   (501) staff       (20)       22 2023-09-29 08:56:06.000000 roger-3.0.4/bmiroger/_version.py
--rw-rw-r--   0 robinschwemmle   (501) staff       (20)    23846 2023-10-09 14:16:33.000000 roger-3.0.4/bmiroger/bmi_roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-3.0.4/cuda_ext.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.061160 roger-3.0.4/look_up_tables/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    10992 2023-12-13 15:21:18.000000 roger-3.0.4/look_up_tables/crop_parameters.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-3.0.4/look_up_tables/intercept_land_use.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-3.0.4/look_up_tables/intercept_sealing.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-3.0.4/look_up_tables/mp_drain_area.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-3.0.4/look_up_tables/mp_layer_manning_strickler.csv
--rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-10-18 12:57:13.000000 roger-3.0.4/look_up_tables/root_depth_land_use.csv
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      231 2023-06-21 07:35:40.000000 roger-3.0.4/pyproject.toml
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      206 2023-12-07 10:09:31.000000 roger-3.0.4/requirements.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       27 2023-12-07 09:51:27.000000 roger-3.0.4/requirements_jax.txt
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.096284 roger-3.0.4/roger/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-3.0.4/roger/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      497 2024-01-10 15:53:46.096327 roger-3.0.4/roger/_version.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-3.0.4/roger/backend.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.068323 roger-3.0.4/roger/bmimodels/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/bmimodels/__init__.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.068770 roger-3.0.4/roger/bmimodels/oneD/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-10-09 13:42:22.000000 roger-3.0.4/roger/bmimodels/oneD/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    16662 2023-10-09 14:16:33.000000 roger-3.0.4/roger/bmimodels/oneD/oneD.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.069459 roger-3.0.4/roger/bmimodels/svat/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-10-05 07:40:57.000000 roger-3.0.4/roger/bmimodels/svat/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    15706 2023-10-09 14:16:33.000000 roger-3.0.4/roger/bmimodels/svat/svat.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.071047 roger-3.0.4/roger/cli/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/roger_copy_model.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/roger_create_mask.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/roger_resubmit.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-3.0.4/roger/cli/roger_run.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-10-04 13:24:05.000000 roger-3.0.4/roger/cli/roger_run_base.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.079701 roger-3.0.4/roger/core/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-3.0.4/roger/core/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13905 2023-12-01 09:08:23.000000 roger-3.0.4/roger/core/adaptive_time_stepping.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    21125 2023-10-18 16:48:58.000000 roger-3.0.4/roger/core/capillary_rise.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    77799 2023-12-20 14:05:15.000000 roger-3.0.4/roger/core/crop.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    28992 2023-11-24 18:19:10.000000 roger-3.0.4/roger/core/evapotranspiration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-3.0.4/roger/core/film_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-3.0.4/roger/core/groundwater.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5411 2023-08-12 10:39:26.000000 roger-3.0.4/roger/core/groundwater_flow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    79194 2023-11-27 17:15:14.000000 roger-3.0.4/roger/core/infiltration.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-3.0.4/roger/core/interception.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13213 2023-10-17 18:55:53.000000 roger-3.0.4/roger/core/nitrate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    63695 2023-11-24 22:11:31.000000 roger-3.0.4/roger/core/numerics.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4191 2023-12-07 14:35:53.000000 roger-3.0.4/roger/core/operators.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7662 2023-06-14 14:01:14.000000 roger-3.0.4/roger/core/root_zone.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-06-21 20:07:16.000000 roger-3.0.4/roger/core/sas.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11056 2023-01-28 18:10:43.000000 roger-3.0.4/roger/core/snow.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    49580 2023-11-15 11:12:47.000000 roger-3.0.4/roger/core/soil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7686 2023-06-13 16:12:33.000000 roger-3.0.4/roger/core/subsoil.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    73597 2023-12-20 11:25:20.000000 roger-3.0.4/roger/core/subsurface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14096 2023-10-18 16:34:32.000000 roger-3.0.4/roger/core/surface.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7125 2023-09-25 10:14:13.000000 roger-3.0.4/roger/core/surface_runoff.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   179560 2023-12-07 15:22:58.000000 roger-3.0.4/roger/core/transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4914 2023-06-22 08:08:08.000000 roger-3.0.4/roger/core/utilities.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.083320 roger-3.0.4/roger/diagnostics/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      112 2023-10-05 14:17:57.000000 roger-3.0.4/roger/diagnostics/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2286 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/api.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3396 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/average.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4230 2023-10-09 10:38:57.000000 roger-3.0.4/roger/diagnostics/base.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2791 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/collect.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2825 2023-10-05 14:16:24.000000 roger-3.0.4/roger/diagnostics/constant.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3948 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/maximum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3949 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/minimum.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2945 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/rate.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1615 2023-10-05 14:16:45.000000 roger-3.0.4/roger/diagnostics/snapshot.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1351 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/tracer_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1369 2023-10-09 12:20:29.000000 roger-3.0.4/roger/diagnostics/water_monitor.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-3.0.4/roger/distributed.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.084607 roger-3.0.4/roger/io_tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/io_tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6511 2023-12-13 14:17:53.000000 roger-3.0.4/roger/io_tools/csv.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-3.0.4/roger/io_tools/hdf5.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-3.0.4/roger/io_tools/netcdf.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-3.0.4/roger/io_tools/yml.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-3.0.4/roger/logs.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3425 2023-12-20 13:53:49.000000 roger-3.0.4/roger/lookuptables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.084804 roger-3.0.4/roger/models/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/__init__.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.085213 roger-3.0.4/roger/models/dummy/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/dummy/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/dummy/dummy.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.085786 roger-3.0.4/roger/models/oneD/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/oneD/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    13837 2023-10-09 13:14:56.000000 roger-3.0.4/roger/models/oneD/oneD.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.086345 roger-3.0.4/roger/models/oneD_event/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/oneD_event/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11539 2023-10-05 13:53:26.000000 roger-3.0.4/roger/models/oneD_event/oneD_event.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.086837 roger-3.0.4/roger/models/svat/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    11654 2023-10-05 13:53:38.000000 roger-3.0.4/roger/models/svat/svat.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.087376 roger-3.0.4/roger/models/svat_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14560 2023-10-05 13:53:51.000000 roger-3.0.4/roger/models/svat_bromide/svat_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.087918 roger-3.0.4/roger/models/svat_crop/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_crop/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    16464 2023-10-05 13:54:01.000000 roger-3.0.4/roger/models/svat_crop/svat_crop.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.088533 roger-3.0.4/roger/models/svat_crop_bromide/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_crop_bromide/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_crop_bromide/svat_crop_bromide.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.088887 roger-3.0.4/roger/models/svat_crop_nitrate/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_crop_nitrate/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.089174 roger-3.0.4/roger/models/svat_oxygen18/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-3.0.4/roger/models/svat_oxygen18/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    21109 2023-10-09 12:20:30.000000 roger-3.0.4/roger/models/svat_oxygen18/svat_oxygen18.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-3.0.4/roger/plugins.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6612 2023-10-05 12:04:10.000000 roger-3.0.4/roger/progress.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-3.0.4/roger/restart.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    26718 2023-11-24 18:24:23.000000 roger-3.0.4/roger/roger.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-3.0.4/roger/routines.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5982 2023-06-22 08:08:08.000000 roger-3.0.4/roger/runtime.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     9633 2023-11-14 16:36:26.000000 roger-3.0.4/roger/settings.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-3.0.4/roger/signals.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    17865 2023-10-09 12:20:29.000000 roger-3.0.4/roger/state.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      828 2023-05-16 09:12:42.000000 roger-3.0.4/roger/time.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-3.0.4/roger/timer.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.091919 roger-3.0.4/roger/tools/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.4/roger/tools/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    31715 2023-07-13 16:06:52.000000 roger-3.0.4/roger/tools/evaluation.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-3.0.4/roger/tools/event_classification.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-3.0.4/roger/tools/filelock.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    12297 2023-10-17 07:35:29.000000 roger-3.0.4/roger/tools/labels.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    24733 2023-06-22 08:08:08.000000 roger-3.0.4/roger/tools/make_toy_data.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-3.0.4/roger/tools/plotting.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    24172 2023-08-08 14:47:20.000000 roger-3.0.4/roger/tools/setup.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)   192309 2023-12-20 14:00:37.000000 roger-3.0.4/roger/variables.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.095060 roger-3.0.4/roger.egg-info/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     7822 2024-01-10 15:53:45.000000 roger-3.0.4/roger.egg-info/PKG-INFO
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3386 2024-01-10 15:53:46.000000 roger-3.0.4/roger.egg-info/SOURCES.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2024-01-10 15:53:45.000000 roger-3.0.4/roger.egg-info/dependency_links.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2024-01-10 15:53:45.000000 roger-3.0.4/roger.egg-info/entry_points.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2024-01-10 15:53:44.000000 roger-3.0.4/roger.egg-info/not-zip-safe
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      311 2024-01-10 15:53:45.000000 roger-3.0.4/roger.egg-info/requires.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)       20 2024-01-10 15:53:45.000000 roger-3.0.4/roger.egg-info/top_level.txt
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      333 2024-01-10 15:53:46.096159 roger-3.0.4/setup.cfg
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     4706 2023-06-22 13:49:47.000000 roger-3.0.4/setup.py
-drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-01-10 15:53:46.094697 roger-3.0.4/test/
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-3.0.4/test/__init__.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-3.0.4/test/cli_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-3.0.4/test/conftest.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-3.0.4/test/make_data_for_svat_transport.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     1065 2023-04-20 09:13:19.000000 roger-3.0.4/test/progress_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-3.0.4/test/restart_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-3.0.4/test/setup_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-06-22 11:49:33.000000 roger-3.0.4/test/state_test.py
--rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-3.0.4/versioneer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.791918 roger-3.0.5/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1072 2023-01-28 18:10:37.000000 roger-3.0.5/LICENSE
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      540 2023-06-22 13:44:17.000000 roger-3.0.5/MANIFEST.in
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7822 2024-04-09 09:01:54.791817 roger-3.0.5/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5956 2023-11-30 13:54:43.000000 roger-3.0.5/README.md
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.758316 roger-3.0.5/bmiroger/
+-rw-rw-r--   0 robinschwemmle   (501) staff       (20)      105 2023-09-29 08:56:50.000000 roger-3.0.5/bmiroger/__init__.py
+-rw-rw-r--   0 robinschwemmle   (501) staff       (20)       22 2023-09-29 08:56:06.000000 roger-3.0.5/bmiroger/_version.py
+-rw-rw-r--   0 robinschwemmle   (501) staff       (20)    23846 2023-10-09 14:16:33.000000 roger-3.0.5/bmiroger/bmi_roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4083 2023-01-28 18:10:37.000000 roger-3.0.5/cuda_ext.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.762114 roger-3.0.5/look_up_tables/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    10992 2023-12-13 15:21:18.000000 roger-3.0.5/look_up_tables/crop_parameters.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     1174 2023-01-28 18:10:43.000000 roger-3.0.5/look_up_tables/intercept_land_use.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      818 2023-01-28 18:10:43.000000 roger-3.0.5/look_up_tables/intercept_sealing.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)     3122 2023-01-28 18:10:43.000000 roger-3.0.5/look_up_tables/mp_drain_area.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)   587663 2023-01-28 18:10:43.000000 roger-3.0.5/look_up_tables/mp_layer_manning_strickler.csv
+-rwxr-xr-x   0 robinschwemmle   (501) staff       (20)      672 2023-10-18 12:57:13.000000 roger-3.0.5/look_up_tables/root_depth_land_use.csv
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      231 2023-06-21 07:35:40.000000 roger-3.0.5/pyproject.toml
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      206 2023-12-07 10:09:31.000000 roger-3.0.5/requirements.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       27 2024-03-03 21:33:22.000000 roger-3.0.5/requirements_jax.txt
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.792271 roger-3.0.5/roger/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2354 2023-01-28 18:10:43.000000 roger-3.0.5/roger/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      497 2024-04-09 09:01:54.792302 roger-3.0.5/roger/_version.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2410 2023-01-28 18:10:43.000000 roger-3.0.5/roger/backend.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.768106 roger-3.0.5/roger/bmimodels/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/bmimodels/__init__.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.768616 roger-3.0.5/roger/bmimodels/oneD/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-10-09 13:42:22.000000 roger-3.0.5/roger/bmimodels/oneD/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    16662 2023-10-09 14:16:33.000000 roger-3.0.5/roger/bmimodels/oneD/oneD.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.769245 roger-3.0.5/roger/bmimodels/svat/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-10-05 07:40:57.000000 roger-3.0.5/roger/bmimodels/svat/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    15706 2023-10-09 14:16:33.000000 roger-3.0.5/roger/bmimodels/svat/svat.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.770760 roger-3.0.5/roger/cli/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      584 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      116 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3143 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/roger_copy_model.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1045 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/roger_create_mask.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3066 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/roger_resubmit.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4344 2023-01-28 18:10:43.000000 roger-3.0.5/roger/cli/roger_run.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1410 2023-10-04 13:24:05.000000 roger-3.0.5/roger/cli/roger_run_base.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.778842 roger-3.0.5/roger/core/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1364 2023-01-28 18:10:43.000000 roger-3.0.5/roger/core/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13905 2023-12-01 09:08:23.000000 roger-3.0.5/roger/core/adaptive_time_stepping.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    21574 2024-03-20 13:41:03.000000 roger-3.0.5/roger/core/capillary_rise.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    83006 2024-03-27 14:50:54.000000 roger-3.0.5/roger/core/crop.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    29290 2024-02-28 14:27:11.000000 roger-3.0.5/roger/core/evapotranspiration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23142 2023-01-28 18:10:43.000000 roger-3.0.5/roger/core/film_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4075 2023-01-28 18:10:43.000000 roger-3.0.5/roger/core/groundwater.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5411 2023-08-12 10:39:26.000000 roger-3.0.5/roger/core/groundwater_flow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    79118 2024-03-05 14:01:04.000000 roger-3.0.5/roger/core/infiltration.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13502 2023-01-28 18:10:43.000000 roger-3.0.5/roger/core/interception.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    22172 2024-03-01 14:07:26.000000 roger-3.0.5/roger/core/nitrate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    63924 2024-02-01 11:34:51.000000 roger-3.0.5/roger/core/numerics.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4191 2023-12-07 14:35:53.000000 roger-3.0.5/roger/core/operators.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7662 2023-06-14 14:01:14.000000 roger-3.0.5/roger/core/root_zone.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11373 2023-06-21 20:07:16.000000 roger-3.0.5/roger/core/sas.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11393 2024-01-24 11:18:41.000000 roger-3.0.5/roger/core/snow.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    51064 2024-03-21 16:08:28.000000 roger-3.0.5/roger/core/soil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7686 2023-06-13 16:12:33.000000 roger-3.0.5/roger/core/subsoil.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    75775 2024-03-27 11:27:00.000000 roger-3.0.5/roger/core/subsurface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14096 2024-02-28 14:21:34.000000 roger-3.0.5/roger/core/surface.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7125 2023-09-25 10:14:13.000000 roger-3.0.5/roger/core/surface_runoff.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   179560 2024-02-22 18:13:47.000000 roger-3.0.5/roger/core/transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4914 2023-06-22 08:08:08.000000 roger-3.0.5/roger/core/utilities.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.781353 roger-3.0.5/roger/diagnostics/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      112 2023-10-05 14:17:57.000000 roger-3.0.5/roger/diagnostics/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2286 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/api.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3396 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/average.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4230 2023-10-09 10:38:57.000000 roger-3.0.5/roger/diagnostics/base.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2791 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/collect.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2825 2023-10-05 14:16:24.000000 roger-3.0.5/roger/diagnostics/constant.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3948 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/maximum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3949 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/minimum.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2945 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/rate.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1615 2023-10-05 14:16:45.000000 roger-3.0.5/roger/diagnostics/snapshot.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1351 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/tracer_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1369 2023-10-09 12:20:29.000000 roger-3.0.5/roger/diagnostics/water_monitor.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    18158 2023-01-28 18:10:43.000000 roger-3.0.5/roger/distributed.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.782394 roger-3.0.5/roger/io_tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/io_tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6994 2024-03-01 19:44:22.000000 roger-3.0.5/roger/io_tools/csv.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1660 2023-01-28 18:10:43.000000 roger-3.0.5/roger/io_tools/hdf5.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6257 2023-01-28 18:10:43.000000 roger-3.0.5/roger/io_tools/netcdf.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      522 2023-01-28 18:10:43.000000 roger-3.0.5/roger/io_tools/yml.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1907 2023-01-28 18:10:43.000000 roger-3.0.5/roger/logs.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3836 2024-03-27 14:33:13.000000 roger-3.0.5/roger/lookuptables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.782626 roger-3.0.5/roger/models/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/__init__.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.782964 roger-3.0.5/roger/models/dummy/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       62 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/dummy/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1251 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/dummy/dummy.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.783608 roger-3.0.5/roger/models/oneD/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/oneD/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    13837 2023-10-09 13:14:56.000000 roger-3.0.5/roger/models/oneD/oneD.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.784160 roger-3.0.5/roger/models/oneD_event/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       76 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/oneD_event/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11539 2023-10-05 13:53:26.000000 roger-3.0.5/roger/models/oneD_event/oneD_event.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.784596 roger-3.0.5/roger/models/svat/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       59 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    11654 2023-10-05 13:53:38.000000 roger-3.0.5/roger/models/svat/svat.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.785172 roger-3.0.5/roger/models/svat_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       84 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14560 2023-10-05 13:53:51.000000 roger-3.0.5/roger/models/svat_bromide/svat_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.785688 roger-3.0.5/roger/models/svat_crop/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       73 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_crop/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    16464 2023-10-05 13:54:01.000000 roger-3.0.5/roger/models/svat_crop/svat_crop.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.786308 roger-3.0.5/roger/models/svat_crop_bromide/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_crop_bromide/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_crop_bromide/svat_crop_bromide.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.786705 roger-3.0.5/roger/models/svat_crop_nitrate/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       98 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_crop_nitrate/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_crop_nitrate/svat_crop_nitrate.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.786996 roger-3.0.5/roger/models/svat_oxygen18/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       86 2023-01-28 18:10:43.000000 roger-3.0.5/roger/models/svat_oxygen18/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    21109 2023-10-09 12:20:30.000000 roger-3.0.5/roger/models/svat_oxygen18/svat_oxygen18.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1936 2023-01-28 18:10:43.000000 roger-3.0.5/roger/plugins.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6612 2023-10-05 12:04:10.000000 roger-3.0.5/roger/progress.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     6221 2023-01-28 18:10:43.000000 roger-3.0.5/roger/restart.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    26718 2024-03-21 16:15:21.000000 roger-3.0.5/roger/roger.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    14190 2023-01-28 18:10:43.000000 roger-3.0.5/roger/routines.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5982 2023-06-22 08:08:08.000000 roger-3.0.5/roger/runtime.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     9740 2024-01-22 15:13:41.000000 roger-3.0.5/roger/settings.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2330 2023-01-28 18:10:43.000000 roger-3.0.5/roger/signals.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    17865 2023-10-09 12:20:29.000000 roger-3.0.5/roger/state.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      828 2023-05-16 09:12:42.000000 roger-3.0.5/roger/time.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      451 2023-01-28 18:10:43.000000 roger-3.0.5/roger/timer.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.789189 roger-3.0.5/roger/tools/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        0 2023-01-28 18:10:43.000000 roger-3.0.5/roger/tools/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    31715 2023-07-13 16:06:52.000000 roger-3.0.5/roger/tools/evaluation.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    20672 2023-01-28 18:10:43.000000 roger-3.0.5/roger/tools/event_classification.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    12678 2023-01-28 18:10:43.000000 roger-3.0.5/roger/tools/filelock.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    12442 2024-01-16 14:15:49.000000 roger-3.0.5/roger/tools/labels.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    24733 2023-06-22 08:08:08.000000 roger-3.0.5/roger/tools/make_toy_data.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      134 2023-01-28 18:10:43.000000 roger-3.0.5/roger/tools/plotting.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    24172 2023-08-08 14:47:20.000000 roger-3.0.5/roger/tools/setup.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)   199436 2024-03-27 11:55:33.000000 roger-3.0.5/roger/variables.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.791139 roger-3.0.5/roger.egg-info/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     7822 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/PKG-INFO
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3386 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/SOURCES.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/dependency_links.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      270 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/entry_points.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)        1 2024-04-09 09:01:52.000000 roger-3.0.5/roger.egg-info/not-zip-safe
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      311 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/requires.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)       20 2024-04-09 09:01:54.000000 roger-3.0.5/roger.egg-info/top_level.txt
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      333 2024-04-09 09:01:54.792153 roger-3.0.5/setup.cfg
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     4706 2023-06-22 13:49:47.000000 roger-3.0.5/setup.py
+drwxr-xr-x   0 robinschwemmle   (501) staff       (20)        0 2024-04-09 09:01:54.790887 roger-3.0.5/test/
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      103 2023-02-08 16:07:16.000000 roger-3.0.5/test/__init__.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1075 2023-01-28 18:10:43.000000 roger-3.0.5/test/cli_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)      391 2023-02-08 13:33:29.000000 roger-3.0.5/test/conftest.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    23321 2023-02-08 17:11:16.000000 roger-3.0.5/test/make_data_for_svat_transport.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     1065 2023-04-20 09:13:19.000000 roger-3.0.5/test/progress_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     2684 2023-01-28 18:10:43.000000 roger-3.0.5/test/restart_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     5047 2023-02-08 17:11:11.000000 roger-3.0.5/test/setup_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)     3320 2023-06-22 11:49:33.000000 roger-3.0.5/test/state_test.py
+-rw-r--r--   0 robinschwemmle   (501) staff       (20)    68611 2023-01-28 18:10:43.000000 roger-3.0.5/versioneer.py
```

### Comparing `roger-3.0.4/LICENSE` & `roger-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/MANIFEST.in` & `roger-3.0.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/PKG-INFO` & `roger-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roger
-Version: 3.0.4
+Version: 3.0.5
 Summary: Runoff Generation Research - a process-based hydrological toolbox model in Python
 Home-page: https://roger.readthedocs.io
 Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de
 License: MIT
 Keywords: hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roger Version: 3.0.4 Summary: Runoff Generation
+Metadata-Version: 2.1 Name: roger Version: 3.0.5 Summary: Runoff Generation
 Research - a process-based hydrological toolbox model in Python Home-page:
 https://roger.readthedocs.io Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de License: MIT Keywords:
 hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `roger-3.0.4/README.md` & `roger-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/bmiroger/bmi_roger.py` & `roger-3.0.5/bmiroger/bmi_roger.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/cuda_ext.py` & `roger-3.0.5/cuda_ext.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/crop_parameters.csv` & `roger-3.0.5/look_up_tables/crop_parameters.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/intercept_land_use.csv` & `roger-3.0.5/look_up_tables/intercept_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/intercept_sealing.csv` & `roger-3.0.5/look_up_tables/intercept_sealing.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/mp_drain_area.csv` & `roger-3.0.5/look_up_tables/mp_drain_area.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/mp_layer_manning_strickler.csv` & `roger-3.0.5/look_up_tables/mp_layer_manning_strickler.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/look_up_tables/root_depth_land_use.csv` & `roger-3.0.5/look_up_tables/root_depth_land_use.csv`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/__init__.py` & `roger-3.0.5/roger/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/backend.py` & `roger-3.0.5/roger/backend.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/bmimodels/oneD/oneD.py` & `roger-3.0.5/roger/bmimodels/oneD/oneD.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/bmimodels/svat/svat.py` & `roger-3.0.5/roger/bmimodels/svat/svat.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/__init__.py` & `roger-3.0.5/roger/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/roger_copy_model.py` & `roger-3.0.5/roger/cli/roger_copy_model.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/roger_create_mask.py` & `roger-3.0.5/roger/cli/roger_create_mask.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/roger_resubmit.py` & `roger-3.0.5/roger/cli/roger_resubmit.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/roger_run.py` & `roger-3.0.5/roger/cli/roger_run.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/cli/roger_run_base.py` & `roger-3.0.5/roger/cli/roger_run_base.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/__init__.py` & `roger-3.0.5/roger/core/__init__.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/adaptive_time_stepping.py` & `roger-3.0.5/roger/core/adaptive_time_stepping.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/capillary_rise.py` & `roger-3.0.5/roger/core/capillary_rise.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         )
         / (
             1
             + npx.power(-vs.h_rz[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
             + (vs.n_salv[2:-2, 2:-2] - 1)
             * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
         )
-        * vs.dt
+        * vs.dt * vs.ks[2:-2, 2:-2]
         * vs.maskCatch[2:-2, 2:-2],
     )
     vs.cpr_rz = update(
         vs.cpr_rz,
         at[2:-2, 2:-2],
         npx.where(vs.cpr_rz[2:-2, 2:-2] < 0, 0, vs.cpr_rz[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
@@ -180,38 +180,38 @@
     """
     vs = state.variables
     settings = state.settings
 
     z = allocate(state.dimensions, ("x", "y"))
 
     # subsoil is saturated
-    mask1 = vs.z_sat[:, :, vs.tau] > 0
+    mask1 = (vs.z_sat[:, :, vs.tau] > 0) & (vs.z_gw[:, :, vs.tau] * 1000 < vs.z_soil[:, :])
     mask2 = vs.z_gw[:, :, vs.tau] * 1000 < vs.z_soil[:, :]
     # capillary rise from groundwater table towards subsoil
     if settings.enable_groundwater_boundary | settings.enable_groundwater:
         z = allocate(state.dimensions, ("x", "y"))
         z = update(
             z,
             at[2:-2, 2:-2],
-            (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_root[2:-2, 2:-2, vs.tau]) * vs.maskCatch[2:-2, 2:-2],
+            (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_soil[2:-2, 2:-2]) + ((vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.tau])/2) * vs.maskCatch[2:-2, 2:-2],
         )
         vs.cpr_ss = update(
             vs.cpr_ss,
             at[2:-2, 2:-2],
             (
                 npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
                 - npx.power(-vs.h_ss[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
             )
             / (
                 1
                 + npx.power(-vs.h_ss[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
                 + (vs.n_salv[2:-2, 2:-2] - 1)
                 * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
             )
-            * vs.dt
+            * vs.dt * vs.ks[2:-2, 2:-2]
             * vs.maskCatch[2:-2, 2:-2],
         )
         vs.cpr_ss = update(
             vs.cpr_ss,
             at[2:-2, 2:-2],
             npx.where(vs.cpr_ss[2:-2, 2:-2] < 0, 0, vs.cpr_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
         )
@@ -230,19 +230,28 @@
         vs.cpr_ss = update(
             vs.cpr_ss,
             at[2:-2, 2:-2],
             npx.where(mask1[2:-2, 2:-2], 0, vs.cpr_ss[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
         )
 
         # reducing capillary rise if large pores of subsoil contain water
-        mask2 = (vs.z_sat[:, :, vs.tau] > 0) & (vs.cpr_ss > vs.S_lp_ss)
+        mask3 = (vs.cpr_ss > vs.S_lp_ss)
         vs.cpr_ss = update(
             vs.cpr_ss,
             at[2:-2, 2:-2],
-            npx.where(mask2[2:-2, 2:-2], vs.cpr_ss[2:-2, 2:-2] - vs.S_lp_ss[2:-2, 2:-2], vs.cpr_ss[2:-2, 2:-2])
+            npx.where(mask3[2:-2, 2:-2], vs.cpr_ss[2:-2, 2:-2] - vs.S_lp_ss[2:-2, 2:-2], vs.cpr_ss[2:-2, 2:-2])
+            * vs.maskCatch[2:-2, 2:-2],
+        )
+
+        # no capillary rise if groundwater table is below 10 m
+        mask4 = (vs.z_gw[:, :, vs.tau] * 1000 - vs.z_soil[:, :] > 10000)
+        vs.cpr_ss = update(
+            vs.cpr_ss,
+            at[2:-2, 2:-2],
+            npx.where(mask4[2:-2, 2:-2], 0, vs.cpr_ss[2:-2, 2:-2])
             * vs.maskCatch[2:-2, 2:-2],
         )
 
         # groundwater table rises into subsoil
         zgw_soil = allocate(state.dimensions, ("x", "y"))
         gw_rise = allocate(state.dimensions, ("x", "y"))
         zgw_soil = update(
```

### Comparing `roger-3.0.4/roger/core/crop.py` & `roger-3.0.5/roger/core/crop.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     """
     vs = state.variables
 
     arr0 = allocate(state.dimensions, ("x", "y", "crops"))
     mask_summer = npx.isin(vs.crop_type, lut.SUMMER_CROPS)
     mask_winter = npx.isin(vs.crop_type, lut.WINTER_CROPS)
     mask_winter_catch = npx.isin(vs.crop_type, lut.WINTER_CATCH_CROPS)
-    mask_my_init = npx.isin(vs.crop_type, lut.WINTER_MULTI_YEAR_CROPS_INIT)
-    mask_my_cont = npx.isin(vs.crop_type, lut.SUMMER_MULTI_YEAR_CROPS_CONT)
+    mask_my_init_winter = npx.isin(vs.crop_type, lut.WINTER_MULTI_YEAR_CROPS_INIT)
+    mask_my_cont_summer = npx.isin(vs.crop_type, lut.SUMMER_MULTI_YEAR_CROPS_CONT)
 
     mask1 = mask_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask2 = mask_summer & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_end)
     mask3 = mask_summer & (vs.doy[vs.tau] > vs.doy_end)
     vs.t_grow_cc = update(
         vs.t_grow_cc,
         at[2:-2, 2:-2, vs.tau, :],
@@ -96,32 +96,15 @@
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_transp_crop[2:-2, 2:-2, :] * mask2[2:-2, 2:-2, :],
     )
     vs.t_grow_cc = update(
         vs.t_grow_cc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask3[2:-2, 2:-2, :], 0, vs.t_grow_cc[2:-2, 2:-2, vs.tau, :]),
     )
-    mask4 = mask_my_cont & (vs.doy[vs.tau] < vs.doy_start)
-    mask5 = mask_my_cont & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_end)
-    mask6 = mask_my_cont & (vs.doy[vs.tau] > vs.doy_end)
-    vs.t_grow_cc = update(
-        vs.t_grow_cc,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask4[2:-2, 2:-2, :], 0, vs.t_grow_cc[2:-2, 2:-2, vs.tau, :]),
-    )
-    vs.t_grow_cc = update_add(
-        vs.t_grow_cc,
-        at[2:-2, 2:-2, vs.tau, :],
-        vs.gdd[2:-2, 2:-2, :] * vs.k_stress_transp_crop[2:-2, 2:-2, :] * mask5[2:-2, 2:-2, :],
-    )
-    vs.t_grow_cc = update(
-        vs.t_grow_cc,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask6[2:-2, 2:-2, :], 0, vs.t_grow_cc[2:-2, 2:-2, vs.tau, :]),
-    )
+
     mask7 = mask_winter & (
         (vs.doy[vs.tau] >= vs.doy_start)
         | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.ccc[:, :, vs.tau, :] > 0))
     )
     mask8 = mask_winter & (vs.doy[vs.tau] > vs.doy_end) & (vs.doy[vs.tau] < vs.doy_start)
     vs.t_grow_cc = update_add(
         vs.t_grow_cc,
@@ -144,27 +127,35 @@
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_transp_crop[2:-2, 2:-2, :] * mask9[2:-2, 2:-2, :],
     )
     vs.t_grow_cc = update(
         vs.t_grow_cc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask10[2:-2, 2:-2, :], 0, vs.t_grow_cc[2:-2, 2:-2, vs.tau, :]),
     )
-    mask11 = mask_my_init & (
-        (vs.doy[vs.tau] >= vs.doy_start) | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0))
+    mask11 = mask_my_init_winter & (
+        (vs.doy[vs.tau] >= vs.doy_start) | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.ccc[:, :, vs.tau, :] > 0))
     )
-    mask12 = mask_my_init & (vs.doy[vs.tau] > vs.doy_end) & (vs.doy[vs.tau] < vs.doy_start)
     vs.t_grow_cc = update_add(
         vs.t_grow_cc,
         at[2:-2, 2:-2, vs.tau, :],
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_transp_crop[2:-2, 2:-2, :] * mask11[2:-2, 2:-2, :],
     )
+
+    mask121 = mask_my_init_winter[:, :, 0] & mask_my_cont_summer[:, :, 1] & (vs.doy[vs.tau] == vs.doy_end[:, :, 0])
     vs.t_grow_cc = update(
         vs.t_grow_cc,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask12[2:-2, 2:-2, :], 0, vs.t_grow_cc[2:-2, 2:-2, vs.tau, :]),
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(mask121[2:-2, 2:-2], vs.t_grow_cc[2:-2, 2:-2, vs.tau, 0], vs.t_grow_cc[2:-2, 2:-2, vs.tau, 1]),
+    )
+
+    mask12 = mask_my_init_winter[:, :, 0] & mask_my_cont_summer[:, :, 1] & (vs.doy[vs.tau] >= vs.doy_start[:, :, 1]) & (vs.doy[vs.tau] <= vs.doy_end[:, :, 1]) & (vs.ccc[:, :, vs.tau, 1] > 0)
+    vs.t_grow_cc = update_add(
+        vs.t_grow_cc,
+        at[2:-2, 2:-2, vs.tau, 1],
+        vs.gdd[2:-2, 2:-2, 1] * vs.k_stress_transp_crop[2:-2, 2:-2, 1] * mask12[2:-2, 2:-2],
     )
 
     mask1 = mask_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask2 = mask_summer & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_end)
     mask3 = mask_summer & (vs.doy[vs.tau] > vs.doy_end)
     vs.t_grow_root = update(
         vs.t_grow_root,
@@ -177,32 +168,15 @@
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_root_growth[2:-2, 2:-2, :] * mask2[2:-2, 2:-2, :],
     )
     vs.t_grow_root = update(
         vs.t_grow_root,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask3[2:-2, 2:-2, :], 0, vs.t_grow_root[2:-2, 2:-2, vs.tau, :]),
     )
-    mask4 = mask_my_cont & (vs.doy[vs.tau] < vs.doy_start)
-    mask5 = mask_my_cont & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_end)
-    mask6 = mask_my_cont & (vs.doy[vs.tau] > vs.doy_end)
-    vs.t_grow_root = update(
-        vs.t_grow_root,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask4[2:-2, 2:-2, :], 0, vs.t_grow_root[2:-2, 2:-2, vs.tau, :]),
-    )
-    vs.t_grow_root = update_add(
-        vs.t_grow_root,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask5[2:-2, 2:-2, :], vs.gdd[2:-2, 2:-2, :] * vs.k_stress_root_growth[2:-2, 2:-2, :], 0),
-    )
-    vs.t_grow_root = update(
-        vs.t_grow_root,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask6[2:-2, 2:-2, :], 0, vs.t_grow_root[2:-2, 2:-2, vs.tau, :]),
-    )
+
     mask7 = mask_winter & (
         (vs.doy[vs.tau] >= vs.doy_start)
         | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.ccc[:, :, vs.tau, :] > 0))
     )
     mask8 = mask_winter & (vs.doy[vs.tau] > vs.doy_end) & (vs.doy[vs.tau] < vs.doy_start)
     vs.t_grow_root = update_add(
         vs.t_grow_root,
@@ -225,27 +199,36 @@
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_root_growth[2:-2, 2:-2, :] * mask9[2:-2, 2:-2, :],
     )
     vs.t_grow_root = update(
         vs.t_grow_root,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask10[2:-2, 2:-2, :], 0, vs.t_grow_root[2:-2, 2:-2, vs.tau, :]),
     )
-    mask11 = mask_my_init & (
-        (vs.doy[vs.tau] >= vs.doy_start) | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0))
+
+    mask11 = mask_my_init_winter & (
+        (vs.doy[vs.tau] >= vs.doy_start) | ((vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.ccc[:, :, vs.tau, :] > 0))
     )
-    mask12 = mask_my_init & (vs.doy[vs.tau] > vs.doy_end) & (vs.doy[vs.tau] < vs.doy_start)
     vs.t_grow_root = update_add(
         vs.t_grow_root,
         at[2:-2, 2:-2, vs.tau, :],
         vs.gdd[2:-2, 2:-2, :] * vs.k_stress_root_growth[2:-2, 2:-2, :] * mask11[2:-2, 2:-2, :],
     )
+
+    mask121 = mask_my_init_winter[:, :, 0] & mask_my_cont_summer[:, :, 1] & (vs.doy[vs.tau] == vs.doy_end[:, :, 0])
     vs.t_grow_root = update(
         vs.t_grow_root,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask12[2:-2, 2:-2, :], 0, vs.t_grow_root[2:-2, 2:-2, vs.tau, :]),
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(mask121[2:-2, 2:-2], vs.t_grow_root[2:-2, 2:-2, vs.tau, 0], vs.t_grow_root[2:-2, 2:-2, vs.tau, 1]),
+    )
+
+    mask12 = mask_my_init_winter[:, :, 0] & mask_my_cont_summer[:, :, 1] & (vs.doy[vs.tau] >= vs.doy_start[:, :, 1]) & (vs.doy[vs.tau] <= vs.doy_end[:, :, 1]) & (vs.ccc[:, :, vs.tau, 1] > 0)
+    vs.t_grow_root = update_add(
+        vs.t_grow_root,
+        at[2:-2, 2:-2, vs.tau, 1],
+        vs.gdd[2:-2, 2:-2, 1] * vs.k_stress_root_growth[2:-2, 2:-2, 1] * mask12[2:-2, 2:-2],
     )
 
     return KernelOutput(t_grow_cc=vs.t_grow_cc, t_grow_root=vs.t_grow_root)
 
 
 @roger_kernel
 def calc_t_decay(state):
@@ -291,14 +274,16 @@
 
     arr0 = allocate(state.dimensions, ("x", "y", "crops"))
     mask_summer = npx.isin(vs.crop_type, lut.SUMMER_CROPS)
     mask_winter = npx.isin(vs.crop_type, lut.WINTER_CROPS)
     mask_winter_catch = npx.isin(vs.crop_type, lut.WINTER_CATCH_CROPS)
     mask_growing_summer = npx.isin(vs.crop_type, npx.array([571, 580], dtype=int))
     mask_growing_winter = npx.isin(vs.crop_type, npx.array([572, 583], dtype=int))
+    mask_cont_summer = npx.isin(vs.crop_type, lut.SUMMER_MULTI_YEAR_CROPS_CONT)
+    mask_cont_winter = npx.isin(vs.crop_type, lut.WINTER_MULTI_YEAR_CROPS_CONT)
     mask_bare = vs.crop_type == 599
 
     mask1 = mask_summer & (vs.doy[vs.tau] > vs.doy_mid) & (vs.doy[vs.tau] < vs.doy_dec)
     mask2 = mask_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask3 = (
         mask_summer
         & (vs.doy[vs.tau] >= vs.doy_start)
@@ -446,14 +431,15 @@
     # harvesting
     vs.ccc = update(
         vs.ccc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask10[2:-2, 2:-2, :], 0, vs.ccc[2:-2, 2:-2, vs.tau, :]),
     )
 
+    # winter catch crops
     mask11 = mask_winter_catch & (
         (vs.doy[vs.tau] > vs.doy_mid) | ((vs.doy[vs.tau] < vs.doy_dec) & (vs.doy[vs.tau] > arr0))
     )
     mask12 = mask_winter_catch & (vs.t_grow_cc[:, :, vs.tau, :] <= 0)
     mask13 = (
         mask_winter_catch
         & (vs.ccc[:, :, vs.tau, :] < vs.ccc_max)
@@ -531,14 +517,15 @@
     # harvesting
     vs.ccc = update(
         vs.ccc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask15[2:-2, 2:-2, :], 0, vs.ccc[2:-2, 2:-2, vs.tau, :]),
     )
 
+    # multi-year crop starting in summer
     mask16 = mask_growing_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask17 = (
         mask_growing_summer
         & (vs.doy[vs.tau] >= vs.doy_start)
         & (vs.ccc[:, :, vs.tau, :] < vs.ccc_max)
         & (vs.doy[vs.tau] <= vs.doy_end)
     )
@@ -567,28 +554,30 @@
                     * (vs.t_grow_cc[2:-2, 2:-2, vs.tau, :] - vs.t_half_mid[2:-2, 2:-2, :])
                 ),
             ),
             vs.ccc[2:-2, 2:-2, vs.tau, :],
         ),
     )
 
-    mask18 = mask_growing_winter & (vs.t_grow_cc[:, :, vs.tau, :] <= 0)
+    # multi-year crop starting in winter
+    mask18 = mask_growing_winter & (
+        (vs.doy[vs.tau] > vs.doy_mid) | ((vs.doy[vs.tau] < vs.doy_dec) & (vs.doy[vs.tau] > arr0))
+    )
     mask19 = (
         mask_growing_winter
-        & (vs.ccc[:, :, vs.tau, :] < vs.ccc_mid)
         & (
             (vs.doy[vs.tau] >= vs.doy_start)
-            | (vs.doy[vs.tau] <= vs.doy_dec) & (vs.doy[vs.tau] > arr0) & (vs.t_grow_cc[:, :, vs.tau, :] > 0)
+            | (vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.t_grow_cc[:, :, vs.tau, :] > 0)
         )
     )
-    # before growing period
-    vs.ccc = update(
-        vs.ccc,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask18[2:-2, 2:-2, :], 0, vs.ccc[2:-2, 2:-2, vs.tau, :]),
+    # mature crop
+    vs.ccc_mid = update(
+        vs.ccc_mid,
+        at[2:-2, 2:-2, :],
+        npx.where(mask18[2:-2, 2:-2, :], vs.ccc[2:-2, 2:-2, vs.tau, :], vs.ccc_mid[2:-2, 2:-2, :]),
     )
     # growth of canopy cover
     vs.ccc = update(
         vs.ccc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(
             mask19[2:-2, 2:-2, :],
@@ -605,14 +594,105 @@
                     * (vs.t_grow_cc[2:-2, 2:-2, vs.tau, :] - vs.t_half_mid[2:-2, 2:-2, :])
                 ),
             ),
             vs.ccc[2:-2, 2:-2, vs.tau, :],
         ),
     )
 
+    # multi-year crop continued in summer
+    mask20 = mask_cont_summer & (
+        (vs.doy[vs.tau] > vs.doy_mid) & (vs.doy[vs.tau] < vs.doy_end)
+    )
+    mask21 = (
+        mask_cont_summer[:, :, 1] & mask_growing_winter[:, :, 0]
+        & (vs.doy[vs.tau] >= vs.doy_start[:, :, 1])
+        & (vs.doy[vs.tau] <= vs.doy_end[:, :, 1])
+    )
+    # mature crop
+    vs.ccc_mid = update(
+        vs.ccc_mid,
+        at[2:-2, 2:-2, :],
+        npx.where(mask20[2:-2, 2:-2, :], vs.ccc[2:-2, 2:-2, vs.tau, :], vs.ccc_mid[2:-2, 2:-2, :]),
+    )
+    # growth of canopy cover
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            mask21[2:-2, 2:-2],
+            npx.where(
+                vs.ccc_min[2:-2, 2:-2, 1]
+                * npx.exp(vs.ccc_growth_rate[2:-2, 2:-2, 1] * vs.t_grow_cc[2:-2, 2:-2, vs.tau, 1])
+                <= vs.ccc_max[2:-2, 2:-2, 1] / 2,
+                vs.ccc_min[2:-2, 2:-2, 1]
+                * npx.exp(vs.ccc_growth_rate[2:-2, 2:-2, 1] * vs.t_grow_cc[2:-2, 2:-2, vs.tau, 1]),
+                vs.ccc_max[2:-2, 2:-2, 1]
+                - (vs.ccc_max[2:-2, 2:-2, 1] / 2 - vs.ccc_min[2:-2, 2:-2, 1])
+                * npx.exp(
+                    -vs.ccc_growth_rate[2:-2, 2:-2, 1]
+                    * (vs.t_grow_cc[2:-2, 2:-2, vs.tau, 1] - vs.t_half_mid[2:-2, 2:-2, 1])
+                ),
+            ),
+            vs.ccc[2:-2, 2:-2, vs.tau, 1],
+        ),
+    )
+
+    # multi-year crop continued in winter
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, -1],
+        npx.where(
+            mask_cont_winter[2:-2, 2:-2, -1] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 1]),
+            vs.ccc[2:-2, 2:-2, vs.tau, 1],
+            vs.ccc[2:-2, 2:-2, vs.tau, -1]
+        ),
+    )
+
+    # multi-year crop continued in summer
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            mask_cont_winter[2:-2, 2:-2, 0] & mask_cont_summer[2:-2, 2:-2, 1] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 0]),
+            vs.ccc[2:-2, 2:-2, vs.tau, 0],
+            vs.ccc[2:-2, 2:-2, vs.tau, 1]
+        ),
+    )
+
+    # multi-year crop stops in winter
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, 0],
+        npx.where(
+            (mask_cont_winter[2:-2, 2:-2, 0]) & (mask_cont_summer[2:-2, 2:-2, 1] == False) & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 0]),
+            0,
+            vs.ccc[2:-2, 2:-2, vs.tau, 0]
+        ),
+    )
+
+    # multi-year crop stops in summer
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            (mask_cont_winter[2:-2, 2:-2, -1] == False) & mask_cont_summer[2:-2, 2:-2, 0] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 1]),
+            0,
+            vs.ccc[2:-2, 2:-2, vs.tau, 1]
+        ),
+    )
+
+    # harvesting of miscanthus
+    mask_miscanthus = vs.crop_type == 590
+    mask21 = mask_summer & (vs.doy[vs.tau] > vs.doy_end)
+    vs.ccc = update(
+        vs.ccc,
+        at[2:-2, 2:-2, vs.tau, :],
+        npx.where(mask21[2:-2, 2:-2, :], 0, vs.ccc[2:-2, 2:-2, vs.tau, :]),
+    )
+
     # bare
     vs.ccc = update(
         vs.ccc,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask_bare[2:-2, 2:-2, :], 0, vs.ccc[2:-2, 2:-2, vs.tau, :]),
     )
 
@@ -764,16 +844,19 @@
 
     arr0 = allocate(state.dimensions, ("x", "y", "crops"))
     mask_summer = npx.isin(vs.crop_type, lut.SUMMER_CROPS)
     mask_winter = npx.isin(vs.crop_type, lut.WINTER_CROPS)
     mask_winter_catch = npx.isin(vs.crop_type, lut.WINTER_CATCH_CROPS)
     mask_growing_summer = npx.isin(vs.crop_type, npx.array([571, 580], dtype=int))
     mask_growing_winter = npx.isin(vs.crop_type, npx.array([572, 583], dtype=int))
+    mask_cont_summer = npx.isin(vs.crop_type, lut.SUMMER_MULTI_YEAR_CROPS_CONT)
+    mask_cont_winter = npx.isin(vs.crop_type, lut.WINTER_MULTI_YEAR_CROPS_CONT)
     mask_bare = vs.crop_type == 599
 
+    # summer crops
     mask1 = mask_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask2 = mask_summer & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_mid)
     mask3 = mask_summer & (vs.doy[vs.tau] > vs.doy_end)
 
     # before growing period
     vs.z_root_crop = update(
         vs.z_root_crop,
@@ -798,14 +881,15 @@
     # harvesting
     vs.z_root_crop = update(
         vs.z_root_crop,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask3[2:-2, 2:-2, :], vs.z_evap[2:-2, 2:-2, npx.newaxis], vs.z_root_crop[2:-2, 2:-2, vs.tau, :]),
     )
 
+    # winter crops
     mask4 = mask_winter & (vs.t_grow_root[:, :, vs.tau, :] <= 0)
     mask5 = mask_winter & (
         (vs.doy[vs.tau] >= vs.doy_start)
         | (vs.doy[vs.tau] <= vs.doy_mid) & (vs.doy[vs.tau] > arr0) & (vs.t_grow_root[:, :, vs.tau, :] > 0)
     )
     mask6 = mask_winter & (vs.doy[vs.tau] > vs.doy_end) & (vs.doy[vs.tau] < vs.doy_start)
     # before growing period
@@ -863,14 +947,15 @@
     # harvesting
     vs.z_root_crop = update(
         vs.z_root_crop,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask9[2:-2, 2:-2, :], vs.z_evap[2:-2, 2:-2, npx.newaxis], vs.z_root_crop[2:-2, 2:-2, vs.tau, :]),
     )
 
+    # multi-year crop starting in summer
     mask10 = mask_growing_summer & (vs.doy[vs.tau] < vs.doy_start)
     mask11 = mask_growing_summer & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_mid)
     # before growing period
     vs.z_root_crop = update(
         vs.z_root_crop,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(mask10[2:-2, 2:-2, :], vs.z_evap[2:-2, 2:-2, npx.newaxis], vs.z_root_crop[2:-2, 2:-2, vs.tau, :]),
@@ -887,22 +972,22 @@
                 * npx.exp(vs.root_growth_rate[2:-2, 2:-2, :] * vs.t_grow_root[2:-2, 2:-2, vs.tau, :])
             )
             * 1000,
             vs.z_root_crop[2:-2, 2:-2, vs.tau, :],
         ),
     )
 
-    mask12 = mask_growing_winter & (vs.t_grow_root[:, :, vs.tau, :] <= 0)
-    mask13 = mask_growing_winter & (vs.doy[vs.tau] >= vs.doy_start) & (vs.doy[vs.tau] <= vs.doy_mid)
-    # before growing period
-    vs.z_root_crop = update(
-        vs.z_root_crop,
-        at[2:-2, 2:-2, vs.tau, :],
-        npx.where(mask12[2:-2, 2:-2, :], vs.z_evap[2:-2, 2:-2, npx.newaxis], vs.z_root_crop[2:-2, 2:-2, vs.tau, :]),
+    mask13 = (
+        mask_growing_winter
+        & (
+            (vs.doy[vs.tau] >= vs.doy_start)
+            | (vs.doy[vs.tau] <= vs.doy_end) & (vs.doy[vs.tau] > arr0) & (vs.t_grow_cc[:, :, vs.tau, :] > 0)
+        )
     )
+
     # crop root growth
     vs.z_root_crop = update(
         vs.z_root_crop,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(
             mask13[2:-2, 2:-2, :],
             (
@@ -911,14 +996,81 @@
                 * npx.exp(vs.root_growth_rate[2:-2, 2:-2, :] * vs.t_grow_root[2:-2, 2:-2, vs.tau, :])
             )
             * 1000,
             vs.z_root_crop[2:-2, 2:-2, vs.tau, :],
         ),
     )
 
+    # multi-year crop continued in summer
+    mask14 = (
+        mask_cont_summer[:, :, 1] & mask_growing_winter[:, :, 0]
+        & (vs.doy[vs.tau] >= vs.doy_start[:, :, 1])
+        & (vs.doy[vs.tau] <= vs.doy_end[:, :, 1])
+    )
+
+    # crop root growth
+    vs.z_root_crop = update(
+        vs.z_root_crop,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            mask14[2:-2, 2:-2],
+            (
+                (vs.z_root_crop_max[2:-2, 2:-2, 1] / 1000)
+                - ((vs.z_root_crop_max[2:-2, 2:-2, 1] - vs.z_evap[2:-2, 2:-2]) / 1000)
+                * npx.exp(vs.root_growth_rate[2:-2, 2:-2, 1] * vs.t_grow_root[2:-2, 2:-2, vs.tau, 1])
+            )
+            * 1000,
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 1],
+        ),
+    )
+
+    # multi-year crop continued in winter
+    vs.z_root_crop = update(
+        vs.z_root_crop,
+        at[2:-2, 2:-2, vs.tau, -1],
+        npx.where(
+            mask_cont_winter[2:-2, 2:-2, -1] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 1]),
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 1],
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, -1]
+        ),
+    )
+
+    # multi-year crop continued in summer
+    vs.z_root_crop = update(
+        vs.z_root_crop,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            mask_cont_winter[2:-2, 2:-2, 0] & mask_cont_summer[2:-2, 2:-2, 1] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 0]),
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 0],
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 1]
+        ),
+    )
+
+    # multi-year crop stops in winter
+    vs.z_root_crop = update(
+        vs.z_root_crop,
+        at[2:-2, 2:-2, vs.tau, 0],
+        npx.where(
+            (mask_cont_winter[2:-2, 2:-2, 0]) & (mask_cont_summer[2:-2, 2:-2, 1] == False) & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 0]),
+            vs.z_evap[2:-2, 2:-2],
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 0]
+        ),
+    )
+
+    # multi-year crop stops in summer
+    vs.z_root_crop = update(
+        vs.z_root_crop,
+        at[2:-2, 2:-2, vs.tau, 1],
+        npx.where(
+            (mask_cont_winter[2:-2, 2:-2, -1] == False) & mask_cont_summer[2:-2, 2:-2, 0] & (vs.doy[vs.tau] == vs.doy_end[2:-2, 2:-2, 1]),
+            vs.z_evap[2:-2, 2:-2],
+            vs.z_root_crop[2:-2, 2:-2, vs.tau, 1]
+        ),
+    )
+
     # crop root growth stops if 70 % of total soil depth is reached
     mask_stop_growth = vs.z_root_crop[:, :, vs.tau, :] >= vs.zroot_to_zsoil_max[:, :, npx.newaxis] * vs.z_soil[:, :, npx.newaxis]
     vs.z_root_crop = update(
         vs.z_root_crop,
         at[2:-2, 2:-2, vs.tau, :],
         npx.where(
             mask_stop_growth[2:-2, 2:-2, :],
```

### Comparing `roger-3.0.4/roger/core/evapotranspiration.py` & `roger-3.0.5/roger/core/evapotranspiration.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,14 +283,15 @@
     )
     # residual ET
     vs.pet_res = update_add(
         vs.pet_res,
         at[2:-2, 2:-2],
         -pevap_soil[2:-2, 2:-2] * mask1[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
+
     vs.pet_res = update(
         vs.pet_res,
         at[2:-2, 2:-2],
         npx.where(vs.pet_res[2:-2, 2:-2] < 0, 0, vs.pet_res[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
 
     # water evaporates from fine pores in root zone
@@ -302,14 +303,15 @@
     )
     # residual ET
     vs.pet_res = update_add(
         vs.pet_res,
         at[2:-2, 2:-2],
         -vs.S_fp_rz[2:-2, 2:-2] * mask2[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
+
     vs.pet_res = update(
         vs.pet_res,
         at[2:-2, 2:-2],
         npx.where(vs.pet_res[2:-2, 2:-2] < 0, 0, vs.pet_res[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
     )
 
     vs.evap_soil = update(
@@ -382,14 +384,21 @@
     # potential transpiration
     vs.ptransp = update(
         vs.ptransp,
         at[2:-2, 2:-2],
         vs.pet_res[2:-2, 2:-2] * vs.transp_coeff[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
 
+    # potential transpiration of trees
+    vs.ptransp = update(
+        vs.ptransp,
+        at[2:-2, 2:-2],
+        npx.where(npx.isin(vs.lu_id[2:-2, 2:-2], npx.array([10, 11, 12, 15, 16, 17])), vs.pet[2:-2, 2:-2] * vs.transp_coeff[2:-2, 2:-2], vs.ptransp[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
+
     # residual transpiration
     vs.ptransp_res = update(
         vs.ptransp_res,
         at[2:-2, 2:-2],
         vs.ptransp[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
 
@@ -855,15 +864,15 @@
         C_iso_transp=vs.C_iso_transp,
     )
 
 
 @roger_kernel
 def calc_transpiration_transport_anion_kernel(state):
     """
-    Calculates chloride/bromide/nitrate transport of transpiration
+    Calculates chloride/bromide transport of transpiration
     """
     vs = state.variables
 
     vs.SA_rz = update(
         vs.SA_rz,
         at[2:-2, 2:-2, :, :],
         transport.calc_SA(state, vs.SA_rz, vs.sa_rz)[2:-2, 2:-2, :, :]
```

### Comparing `roger-3.0.4/roger/core/film_flow.py` & `roger-3.0.5/roger/core/film_flow.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/groundwater.py` & `roger-3.0.5/roger/core/groundwater.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/groundwater_flow.py` & `roger-3.0.5/roger/core/groundwater_flow.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/infiltration.py` & `roger-3.0.5/roger/core/infiltration.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     )
 
     # first wetting front
     # potential matrix infiltration rate after saturation is reached
     vs.inf_mat_pot = update(
         vs.inf_mat_pot,
         at[2:-2, 2:-2],
-        0,
+        vs.ks[2:-2, 2:-2] * vs.dt,
     )
     vs.inf_mat_pot = update(
         vs.inf_mat_pot,
         at[2:-2, 2:-2],
         npx.where(
             mask1[2:-2, 2:-2],
             (vs.ks[2:-2, 2:-2] * vs.dt / 2)
@@ -1429,19 +1429,15 @@
         at[2:-2, 2:-2],
         0,
     )
 
     vs.q_hof = update(
         vs.q_hof,
         at[2:-2, 2:-2],
-        npx.where(
-            (vs.S_rz[2:-2, 2:-2, vs.tau] <= vs.S_sat_rz[2:-2, 2:-2]),
-            vs.z0[2:-2, 2:-2, vs.tau],
-            0,
-        )
+        vs.z0[2:-2, 2:-2, vs.tau]
         * vs.maskCatch[2:-2, 2:-2],
     )
 
     vs.q_hof = update(
         vs.q_hof,
         at[2:-2, 2:-2],
         npx.where(vs.q_hof[2:-2, 2:-2] < 0, 0, vs.q_hof[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
@@ -1456,15 +1452,15 @@
     vs.q_sof = update(
         vs.q_sof,
         at[2:-2, 2:-2],
         npx.where(
             ((vs.S_lp_rz[2:-2, 2:-2] + vs.S_fp_rz[2:-2, 2:-2]) > (vs.S_ac_rz[2:-2, 2:-2] + vs.S_ufc_rz[2:-2, 2:-2]))
             & ((vs.S_lp_ss[2:-2, 2:-2] + vs.S_fp_ss[2:-2, 2:-2]) >= (vs.S_ac_ss[2:-2, 2:-2] + vs.S_ufc_ss[2:-2, 2:-2])),
             (vs.S_lp_rz[2:-2, 2:-2] + vs.S_fp_rz[2:-2, 2:-2]) - (vs.S_ac_rz[2:-2, 2:-2] + vs.S_ufc_rz[2:-2, 2:-2]),
-            0,
+            vs.q_sof[2:-2, 2:-2],
         )
         * vs.maskCatch[2:-2, 2:-2],
     )
 
     mask = (vs.q_sof > 0)
     vs.S_fp_rz = update(
         vs.S_fp_rz,
```

### Comparing `roger-3.0.4/roger/core/interception.py` & `roger-3.0.5/roger/core/interception.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/nitrate.py` & `roger-3.0.5/roger/models/svat_crop/svat_crop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,457 +1,507 @@
-from roger import roger_kernel, roger_routine, KernelOutput
+from pathlib import Path
+import h5netcdf
+from roger import RogerSetup, roger_routine, roger_kernel, KernelOutput
 from roger.variables import allocate
-from roger.core.operators import numpy as npx, update, update_add, at
+from roger.core.operators import numpy as npx, update, at
+from roger.core.surface import calc_parameters_surface_kernel
+import roger.lookuptables as lut
+import numpy as onp
 
 
-@roger_kernel
-def calc_soil_temperature_kernel(state):
-    """Calculates soil temperature."""
-    vs = state.variables
-    settings = state.settings
-
-    ta_year = allocate(state.dimensions, ("x", "y"))
-    a_year = allocate(state.dimensions, ("x", "y"))
-
-    # calculate annual average air temperature and annual average amplitude of air temperature
-    if vs.itt + 364 < settings.nitt:
-        ta_year = update(
-            ta_year,
-            at[2:-2, 2:-2],
-            npx.mean(vs.TA[vs.itt:vs.itt+364]),
-        )
-        a_year = update(
-            a_year,
-            at[2:-2, 2:-2],
-            2 * npx.mean(npx.abs(vs.TA[npx.newaxis, npx.newaxis, vs.itt:vs.itt+364] - ta_year[2:-2, 2:-2, npx.newaxis]), axis=-1),
-        )
-    else:
-        ta_year = update(
-            ta_year,
-            at[2:-2, 2:-2],
-            npx.mean(vs.TA[settings.nitt-364:]),
-        )
-        a_year = update(
-            a_year,
-            at[2:-2, 2:-2],
-            2 * npx.mean(npx.abs(vs.TA[npx.newaxis, npx.newaxis, settings.nitt-364:] - ta_year[2:-2, 2:-2, npx.newaxis]), axis=-1),
-        )
-
-    vs.temp_soil = update(
-        vs.temp_soil,
-        at[2:-2, 2:-2, vs.tau],
-        ta_year[2:-2, 2:-2]
-        + a_year[2:-2, 2:-2]
-        * npx.sin(
-            (2 * settings.pi) * (vs.doy[1]/365)
-            - (2 * settings.pi) * (vs.phi_soil_temp[2:-2, 2:-2]/365)/2
-            - ((0.5 * (vs.z_soil[2:-2, 2:-2]/1000)) / (vs.damp_soil_temp[2:-2, 2:-2] * (vs.S_s[2:-2, 2:-2, vs.tau]/(vs.S_sat_rz[2:-2, 2:-2] + vs.S_sat_ss[2:-2, 2:-2])))))
-        * npx.exp((-0.5 * (vs.z_soil[2:-2, 2:-2]/1000)) / (vs.damp_soil_temp[2:-2, 2:-2] * (vs.S_s[2:-2, 2:-2, vs.tau]/(vs.S_sat_rz[2:-2, 2:-2] + vs.S_sat_ss[2:-2, 2:-2]))))
-        * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    return KernelOutput(
-        temp_soil=vs.temp_soil,
-        )
-
-
-@roger_kernel
-def calc_denit_soil(state, msa, km, Dmax, sa, S_sat):
-    """Calculates soil dentirification rate."""
-    vs = state.variables
-    settings = state.settings
-
-    S = allocate(state.dimensions, ("x", "y"))
-    S = update(
-        S,
-        at[2:-2, 2:-2],
-        npx.sum(sa[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    # soil temperature coefficient
-    soil_temp_coeff = allocate(state.dimensions, ("x", "y"))
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            ((vs.temp_soil[2:-2, 2:-2, vs.tau] >= 5) & (vs.temp_soil[2:-2, 2:-2, vs.tau] <= 30)),
-            vs.temp_soil[2:-2, 2:-2, vs.tau] / (30 - 5),
-            0,
-        )
-        * vs.maskCatch[2:-2, 2:-2],
-    )
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            (vs.temp_soil[2:-2, 2:-2, vs.tau] > 30),
-            1,
-            soil_temp_coeff[2:-2, 2:-2],
-        )
-        * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    # calculate denitrification rate
-    mr = allocate(state.dimensions, ("x", "y", "ages"))
-    mr = update(
-        mr,
-        at[2:-2, 2:-2, :],
-        (Dmax[2:-2, 2:-2, npx.newaxis] * (vs.dt / (365 * 24)) * settings.dx * settings.dy * 100
-        * (msa[2:-2, 2:-2, vs.tau, :] / (km[2:-2, 2:-2, npx.newaxis] * (vs.dt / (365 * 24)) * settings.dx * settings.dy * 100 + msa[2:-2, 2:-2, vs.tau, :])))
-        * soil_temp_coeff[2:-2, 2:-2, npx.newaxis]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    # no denitrification if storage is lower than 70 % of pore volume
-    mr = update(
-        mr,
-        at[2:-2, 2:-2, :],
-        npx.where(
-            S[2:-2, 2:-2, npx.newaxis] >= 0.7 * S_sat[2:-2, 2:-2, npx.newaxis],
-            mr[2:-2, 2:-2, :],
-            0,
-        )
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    # limit denitrification to available solute mass
-    mr = update(
-        mr,
-        at[2:-2, 2:-2, :],
-        npx.where(mr[2:-2, 2:-2, :] > msa[2:-2, 2:-2, vs.tau, :], msa[2:-2, 2:-2, vs.tau, :], mr[2:-2, 2:-2, :])
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-
-    return mr
-
-
-@roger_kernel
-def calc_nit_soil(state, Nmin, knit, Dnit, sa, S_sat):
-    """Calculates soil nitrification rate."""
-    vs = state.variables
-    settings = state.settings
-
-    S = allocate(state.dimensions, ("x", "y"))
-    S = update(
-        S,
-        at[2:-2, 2:-2],
-        npx.sum(sa[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    # soil temperature coefficient
-    soil_temp_coeff = allocate(state.dimensions, ("x", "y"))
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            ((vs.temp_soil[2:-2, 2:-2, vs.tau] >= 1) & (vs.temp_soil[2:-2, 2:-2, vs.tau] <= 30)),
-            vs.temp_soil[2:-2, 2:-2, vs.tau] / (30 - 1),
-            0,
-        )
-        * vs.maskCatch[2:-2, 2:-2],
-    )
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            (vs.temp_soil[2:-2, 2:-2, vs.tau] > 30),
-            1,
-            soil_temp_coeff[2:-2, 2:-2],
-        )
-        * vs.maskCatch[2:-2, 2:-2],
-    )
+class SVATCROPSetup(RogerSetup):
+    """A SVAT model including crop phenology/crop rotation.
+    """
+    _base_path = Path(__file__).parent
+    _input_dir = _base_path / "input"
 
-    # calculate nitrification rate
-    ma = allocate(state.dimensions, ("x", "y", "ages"))
-    ma = update(
-        ma,
-        at[2:-2, 2:-2, :],
-        (Dnit[2:-2, 2:-2, npx.newaxis] * (vs.dt / (365 * 24)) * settings.dx * settings.dy * 100
-        * (Nmin[2:-2, 2:-2, vs.tau, :] / (knit[2:-2, 2:-2, npx.newaxis] * (vs.dt / (365 * 24)) * settings.dx * settings.dy * 100 + Nmin[2:-2, 2:-2, vs.tau, :])))
-        * soil_temp_coeff[2:-2, 2:-2, npx.newaxis]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    # no nitrification if storage is greater than 70 % of pore volume
-    ma = update(
-        ma,
-        at[2:-2, 2:-2, :],
-        npx.where(
-            S[2:-2, 2:-2, npx.newaxis] < 0.7 * S_sat[2:-2, 2:-2, npx.newaxis],
-            ma[2:-2, 2:-2, :],
-            0,
-        )
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    # limit denitrification to available solute mass
-    ma = update(
-        ma,
-        at[2:-2, 2:-2, :],
-        npx.where(ma[2:-2, 2:-2, :] > Nmin[2:-2, 2:-2, vs.tau, :], Nmin[2:-2, 2:-2, vs.tau, :], ma[2:-2, 2:-2, :])
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
+    # custom helper functions
+    def _read_var_from_nc(self, var, path_dir, file, group=None):
+        nc_file = path_dir / file
+        if group:
+            with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+                var_obj = infile.groups[group].variables[var]
+                return npx.array(var_obj)
+        else:
+            with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+                var_obj = infile.variables[var]
+                return npx.array(var_obj)
+
+    def _get_nitt(self, path_dir, file):
+        nc_file = path_dir / file
+        with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+            var_obj = infile.variables['Time']
+            return len(onp.array(var_obj))
+
+    def _get_runlen(self, path_dir, file):
+        nc_file = path_dir / file
+        with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+            var_obj = infile.variables['dt']
+            return onp.sum(onp.array(var_obj))
+
+    def _get_time_origin(self, path_dir, file):
+        nc_file = path_dir / file
+        with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+            date = infile.variables['Time'].attrs['time_origin'].split(" ")[0]
+            return f"{date} 00:00:00"
+
+    def _get_ncr(self, path_dir, file):
+        nc_file = path_dir / file
+        with h5netcdf.File(nc_file, "r", decode_vlen_strings=False) as infile:
+            var_obj = infile.variables['year_season']
+            return len(onp.array(var_obj))
+
+    @roger_routine
+    def set_settings(self, state):
+        settings = state.settings
+        settings.identifier = "SVATCROP"
+
+        # output frequency (in seconds)
+        settings.output_frequency = 86400
+        # total grid numbers in x- and y-direction
+        settings.nx, settings.ny = 1, 1
+        # length of simulation (in seconds)
+        settings.runlen = self._get_runlen(self._input_dir, 'forcing.nc')
+
+        # spatial discretization (in meters)
+        settings.dx = 1
+        settings.dy = 1
+
+        # origin of spatial grid
+        settings.x_origin = 0.0
+        settings.y_origin = 0.0
+        # origin of time steps (e.g. 01-01-2023)
+        settings.time_origin = self._get_time_origin(self._input_dir, 'forcing.nc')
+
+        # enable specific processes
+        settings.enable_groundwater_boundary = False
+        settings.enable_crop_water_stress = True
+        settings.enable_crop_phenology = True
+        settings.enable_crop_rotation = True
+        settings.enable_macropore_lower_boundary_condition = False
+        settings.enable_adaptive_time_stepping = True
+
+        if settings.enable_crop_rotation:
+            settings.ncrops = 3
+            settings.ncr = 3
+
+    @roger_routine(
+        dist_safe=False,
+        local_variables=[
+            "x",
+            "y",
+        ],
+    )
+    def set_grid(self, state):
+        vs = state.variables
+        settings = state.settings
+
+        # spatial grid
+        dx = allocate(state.dimensions, ("x"))
+        dx = update(dx, at[:], settings.dx)
+        dy = allocate(state.dimensions, ("y"))
+        dy = update(dy, at[:], settings.dy)
+        # distance from origin
+        vs.x = update(vs.x, at[3:-2], settings.x_origin + npx.cumsum(dx[3:-2]))
+        vs.y = update(vs.y, at[3:-2], settings.y_origin + npx.cumsum(dy[3:-2]))
+
+    @roger_routine(
+        dist_safe=False,
+        local_variables=[
+            "lut_ilu",
+            "lut_gc",
+            "lut_gcm",
+            "lut_is",
+            "lut_rdlu",
+            "lut_crops",
+        ],
+    )
+    def set_look_up_tables(self, state):
+        vs = state.variables
+
+        vs.lut_ilu = update(vs.lut_ilu, at[:, :], lut.ARR_ILU)
+        vs.lut_gc = update(vs.lut_gc, at[:, :], lut.ARR_GC)
+        vs.lut_gcm = update(vs.lut_gcm, at[:, :], lut.ARR_GCM)
+        vs.lut_is = update(vs.lut_is, at[:, :], lut.ARR_IS)
+        vs.lut_rdlu = update(vs.lut_rdlu, at[:, :], lut.ARR_RDLU)
+        vs.lut_crops = update(vs.lut_crops, at[:, :], lut.ARR_CP)
+
+    @roger_routine
+    def set_topography(self, state):
+        pass
+
+    @roger_routine(
+        dist_safe=False,
+        local_variables=[
+            "lu_id",
+            "z_soil",
+            "dmpv",
+            "lmpv",
+            "theta_ac",
+            "theta_ufc",
+            "theta_pwp",
+            "ks",
+            "kf",
+            "crop_type",
+            "z_root",
+            "z_root_crop",
+        ],
+    )
+    def set_parameters_setup(self, state):
+        vs = state.variables
+
+        vs.lu_id = update(vs.lu_id, at[2:-2, 2:-2], 8)
+        vs.z_soil = update(vs.z_soil, at[2:-2, 2:-2], 1350)
+        vs.dmpv = update(vs.dmpv, at[2:-2, 2:-2], 50)
+        vs.lmpv = update(vs.lmpv, at[2:-2, 2:-2], 1000)
+        vs.theta_ac = update(vs.theta_ac, at[2:-2, 2:-2], 0.1)
+        vs.theta_ufc = update(vs.theta_ufc, at[2:-2, 2:-2], 0.1)
+        vs.theta_pwp = update(vs.theta_pwp, at[2:-2, 2:-2], 0.2)
+        vs.ks = update(vs.ks, at[2:-2, 2:-2], 5)
+        vs.kf = update(vs.kf, at[2:-2, 2:-2], 2500)
+
+        vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 0], 564)
+        vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 1], 539)
+        vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 2], 564)
+
+        vs.z_root = update(vs.z_root, at[2:-2, 2:-2, :2], 200)
+        vs.z_root_crop = update(
+            vs.z_root_crop,
+            at[2:-2, 2:-2, :2, 0], 200
+        )
+
+    @roger_routine
+    def set_parameters(self, state):
+        vs = state.variables
+
+        if (vs.month[vs.tau] != vs.month[vs.taum1]) & (vs.itt > 1):
+            vs.update(calc_parameters_surface_kernel(state))
+
+    @roger_routine
+    def set_initial_conditions_setup(self, state):
+        pass
+
+    @roger_routine
+    def set_initial_conditions(self, state):
+        vs = state.variables
+
+        vs.theta_rz = update(vs.theta_rz, at[2:-2, 2:-2, :vs.taup1], 0.3)
+        vs.theta_ss = update(vs.theta_ss, at[2:-2, 2:-2, :vs.taup1], 0.3)
+
+        vs.update(set_initial_conditions_crops_kernel(state))
+
+    @roger_routine
+    def set_boundary_conditions_setup(self, state):
+        pass
+
+    @roger_routine
+    def set_boundary_conditions(self, state):
+        pass
+
+    @roger_routine
+    def set_forcing_setup(self, state):
+        pass
+
+    @roger_routine(
+        dist_safe=False,
+        local_variables=[
+            "time",
+            "itt_day",
+            "itt_forc",
+            "prec_day",
+            "ta_day",
+            "pet_day",
+            "year",
+            "month",
+            "doy",
+            "itt",
+            "itt_cr",
+            "crop_type",
+        ],
+    )
+    def set_forcing(self, state):
+        vs = state.variables
+
+        condt = (vs.time % (24 * 60 * 60) == 0)
+        if condt:
+            vs.itt_day = 0
+            vs.year = update(vs.year, at[1], self._read_var_from_nc("YEAR", self._input_dir, 'forcing.nc')[vs.itt_forc])
+            vs.month = update(vs.month, at[1], self._read_var_from_nc("MONTH", self._input_dir, 'forcing.nc')[vs.itt_forc])
+            vs.doy = update(vs.doy, at[1], self._read_var_from_nc("DOY", self._input_dir, 'forcing.nc')[vs.itt_forc])
+            vs.prec_day = update(vs.prec_day, at[2:-2, 2:-2, :], self._read_var_from_nc("PREC", self._input_dir, 'forcing.nc')[:, :, vs.itt_forc:vs.itt_forc+6*24])
+            vs.ta_day = update(vs.ta_day, at[2:-2, 2:-2, :], self._read_var_from_nc("TA", self._input_dir, 'forcing.nc')[:, :, vs.itt_forc:vs.itt_forc+6*24])
+            vs.pet_day = update(vs.pet_day, at[2:-2, 2:-2, :], self._read_var_from_nc("PET", self._input_dir, 'forcing.nc')[:, :, vs.itt_forc:vs.itt_forc+6*24])
+            vs.itt_forc = vs.itt_forc + 6 * 24
+
+        if (vs.year[1] != vs.year[0]) & (vs.itt > 1):
+            vs.itt_cr = vs.itt_cr + 2
+            vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 0], 564)
+            vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 1], 539)
+            vs.crop_type = update(vs.crop_type, at[2:-2, 2:-2, 2], 564)
+
+    @roger_routine
+    def set_diagnostics(self, state):
+        pass
+
+    @roger_routine
+    def after_timestep(self, state):
+        vs = state.variables
 
-    return ma
+        vs.update(after_timestep_kernel(state))
+        vs.update(after_timestep_crops_kernel(state))
 
 
 @roger_kernel
-def calc_min_soil(state, kmin):
-    """Calculates soil nitrogen mineralization rate."""
+def set_initial_conditions_crops_kernel(state):
     vs = state.variables
-    settings = state.settings
 
-    # soil temperature coefficient
-    soil_temp_coeff = allocate(state.dimensions, ("x", "y"))
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            ((vs.temp_soil[2:-2, 2:-2, vs.tau] >= 0) & (vs.temp_soil[2:-2, 2:-2, vs.tau] <= 30)),
-            vs.temp_soil[2:-2, 2:-2, vs.tau] / (30 - 0),
-            0,
-        )
-        * vs.maskCatch[2:-2, 2:-2],
-    )
-    soil_temp_coeff = update(
-        soil_temp_coeff,
-        at[2:-2, 2:-2],
-        npx.where(
-            (vs.temp_soil[2:-2, 2:-2, vs.tau] > 30),
-            1,
-            soil_temp_coeff[2:-2, 2:-2],
-        )
-        * vs.maskCatch[2:-2, 2:-2],
+    # calculate time since growing
+    t_grow = allocate(state.dimensions, ("x", "y", "crops"))
+    t_grow = update(
+        t_grow,
+        at[2:-2, 2:-2, :], npx.where(vs.z_root_crop[2:-2, 2:-2, vs.taum1, :] > 0, (-1 / vs.root_growth_rate[2:-2, 2:-2, :]) * npx.log(1 / ((vs.z_root_crop[2:-2, 2:-2, vs.taum1, :] / 1000 - vs.z_root_crop_max[2:-2, 2:-2, :] / 1000) * (-1 / (vs.z_root_crop_max[2:-2, 2:-2, :] / 1000 - vs.z_evap[2:-2, 2:-2, npx.newaxis] / 1000)))), 0)
     )
 
-    ma = allocate(state.dimensions, ("x", "y"))
-    ma = update(
-        ma,
-        at[2:-2, 2:-2],
-        kmin[2:-2, 2:-2]
-        * (vs.dt / (365 * 24))
-        * settings.dx
-        * settings.dy
-        * 100
-        * soil_temp_coeff[2:-2, 2:-2]
-        * vs.maskCatch[2:-2, 2:-2],
+    vs.t_grow_cc = update(
+        vs.t_grow_cc,
+        at[2:-2, 2:-2, :2, :], t_grow[2:-2, 2:-2, npx.newaxis, :]
     )
 
-    return ma
-
-
-@roger_kernel
-def calc_n_fixation(state, kfix):
-    """Calculates nitrogen fixation."""
-    vs = state.variables
-    settings = state.settings
-
-    nfix = allocate(state.dimensions, ("x", "y"))
-    nfix = update(
-        nfix,
-        at[2:-2, 2:-2],
-        kfix[2:-2, 2:-2] * (vs.dt / (365 * 24)) * settings.dx * settings.dy * 100 * (vs.z_root[2:-2, 2:-2, vs.tau]/(0.7 * vs.z_soil[2:-2, 2:-2])) * vs.maskCatch[2:-2, 2:-2],
+    vs.t_grow_root = update(
+        vs.t_grow_root,
+        at[2:-2, 2:-2, :2, :], t_grow[2:-2, 2:-2, npx.newaxis, :]
     )
 
-    return nfix
-
-
-@roger_kernel
-def calc_denit_gw(state, msa, k):
-    """Calculates groundwater dentrification rate."""
-    vs = state.variables
-
-    # calculate denitrification rate
-    age = allocate(state.dimensions, ("x", "y", "ages"))
-    mr = allocate(state.dimensions, ("x", "y", "ages"))
-    age = update(
-        age,
-        at[2:-2, 2:-2, :],
-        vs.ages[npx.newaxis, npx.newaxis, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    mr = update(
-        mr,
-        at[2:-2, 2:-2, :],
-        msa[2:-2, 2:-2, :]
-        * k[2:-2, 2:-2, npx.newaxis]
-        * npx.exp(-k[2:-2, 2:-2, npx.newaxis] * age[2:-2, 2:-2, :])
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-    # limit denitrification to available solute mass
-    mr = update(
-        mr,
-        at[2:-2, 2:-2, :],
-        npx.where(mr[2:-2, 2:-2, :] > msa[2:-2, 2:-2, vs.tau, :], msa[2:-2, 2:-2, vs.tau, :], mr[2:-2, 2:-2, :])
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
+    return KernelOutput(
+        t_grow_cc=vs.t_grow_cc,
+        t_grow_root=vs.t_grow_root,
     )
 
-    return mr
-
 
 @roger_kernel
-def calc_nitrogen_cycle_kernel(state):
+def after_timestep_kernel(state):
     vs = state.variables
 
-    vs.Nmin_rz = update_add(
-        vs.Nmin_rz,
-        at[2:-2, 2:-2, vs.tau, 0],
-        calc_n_fixation(state, vs.kfix_rz)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    vs.Nmin_rz = update_add(
-        vs.Nmin_rz,
-        at[2:-2, 2:-2, vs.tau, 0],
-        calc_min_soil(state, vs.kmin_rz)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    vs.Nmin_ss = update_add(
-        vs.Nmin_ss,
-        at[2:-2, 2:-2, vs.tau, 0],
-        calc_min_soil(state, vs.kmin_ss)[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
-    )
-
-    vs.ma_rz = update(
-        vs.ma_rz,
-        at[2:-2, 2:-2, :],
-        calc_nit_soil(state, vs.Nmin_rz, vs.km_nit_rz, vs.dmax_nit_rz, vs.sa_rz, vs.S_sat_rz)[
-            2:-2, 2:-2, :
-        ]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-
-    vs.Nmin_rz = update_add(
-        vs.Nmin_rz,
-        at[2:-2, 2:-2, vs.tau, :],
-        -vs.ma_rz[2:-2, 2:-2, :],
-    )
-
-    vs.msa_rz = update_add(
-        vs.msa_rz,
-        at[2:-2, 2:-2, vs.tau, 0],
-        npx.sum(vs.ma_rz[2:-2, 2:-2, :], axis=-1),
-    )
-
-    vs.ma_ss = update(
-        vs.ma_ss,
-        at[2:-2, 2:-2, :],
-        calc_nit_soil(state, vs.Nmin_ss, vs.km_nit_ss, vs.dmax_nit_ss, vs.sa_ss, vs.S_sat_ss)[
-            2:-2, 2:-2, :
-        ]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-
-    vs.Nmin_ss = update_add(
-        vs.Nmin_ss,
-        at[2:-2, 2:-2, vs.tau, :],
-        -vs.ma_ss[2:-2, 2:-2, :],
-    )
-
-    vs.msa_ss = update_add(
-        vs.msa_ss,
-        at[2:-2, 2:-2, vs.tau, 0],
-        npx.sum(vs.ma_ss[2:-2, 2:-2, :], axis=-1),
-    )
-
-    vs.mr_rz = update(
-        vs.mr_rz,
-        at[2:-2, 2:-2, :],
-        calc_denit_soil(state, vs.msa_rz, vs.km_denit_rz, vs.dmax_denit_rz, vs.sa_rz, vs.S_sat_rz)[
-            2:-2, 2:-2, :
-        ]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-
-    vs.msa_rz = update_add(
-        vs.msa_rz,
-        at[2:-2, 2:-2, vs.tau, :],
-        -vs.mr_rz[2:-2, 2:-2, :],
-    )
-
-    vs.mr_ss = update(
-        vs.mr_ss,
-        at[2:-2, 2:-2, :],
-        calc_denit_soil(state, vs.msa_ss, vs.km_denit_ss, vs.dmax_denit_ss, vs.sa_ss, vs.S_sat_ss)[
-            2:-2, 2:-2, :
-        ]
-        * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
-
-    vs.msa_ss = update_add(
-        vs.msa_ss,
-        at[2:-2, 2:-2, vs.tau, :],
-        -vs.mr_ss[2:-2, 2:-2, :],
-    )
-
-    vs.ma_s = update(
-        vs.ma_s,
-        at[2:-2, 2:-2, :],
-        vs.ma_rz[2:-2, 2:-2, :] + vs.ma_ss[2:-2, 2:-2, :],
-    )
-
-    vs.nit_s = update(
-        vs.nit_s,
-        at[2:-2, 2:-2],
-        npx.sum(vs.ma_s[2:-2, 2:-2, :], axis=-1),
-    )    
-
-    vs.mr_s = update(
-        vs.mr_s,
-        at[2:-2, 2:-2, :],
-        vs.mr_rz[2:-2, 2:-2, :] + vs.mr_ss[2:-2, 2:-2, :],
-    )
-
-    vs.denit_s = update(
-        vs.denit_s,
-        at[2:-2, 2:-2],
-        npx.sum(vs.mr_s[2:-2, 2:-2, :], axis=-1),
-    )   
-
-    vs.Nmin_s = update(
-        vs.Nmin_s,
-        at[2:-2, 2:-2, vs.tau],
-        npx.sum(vs.Nmin_rz[2:-2, 2:-2, vs.tau, :], axis=-1) + npx.sum(vs.Nmin_ss[2:-2, 2:-2, vs.tau, :], axis=-1) * vs.maskCatch[2:-2, 2:-2],
+    vs.ta = update(
+        vs.ta,
+        at[2:-2, 2:-2, vs.taum1], vs.ta[2:-2, 2:-2, vs.tau],
+    )
+    vs.z_root = update(
+        vs.z_root,
+        at[2:-2, 2:-2, vs.taum1], vs.z_root[2:-2, 2:-2, vs.tau],
+    )
+    vs.ground_cover = update(
+        vs.ground_cover,
+        at[2:-2, 2:-2, vs.taum1], vs.ground_cover[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_sur = update(
+        vs.S_sur,
+        at[2:-2, 2:-2, vs.taum1], vs.S_sur[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_int_top = update(
+        vs.S_int_top,
+        at[2:-2, 2:-2, vs.taum1], vs.S_int_top[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_int_ground = update(
+        vs.S_int_ground,
+        at[2:-2, 2:-2, vs.taum1], vs.S_int_ground[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_dep = update(
+        vs.S_dep,
+        at[2:-2, 2:-2, vs.taum1], vs.S_dep[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_snow = update(
+        vs.S_snow,
+        at[2:-2, 2:-2, vs.taum1], vs.S_snow[2:-2, 2:-2, vs.tau],
+    )
+    vs.swe = update(
+        vs.swe,
+        at[2:-2, 2:-2, vs.taum1], vs.swe[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_rz = update(
+        vs.S_rz,
+        at[2:-2, 2:-2, vs.taum1], vs.S_rz[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_ss = update(
+        vs.S_ss,
+        at[2:-2, 2:-2, vs.taum1], vs.S_ss[2:-2, 2:-2, vs.tau],
+    )
+    vs.S_s = update(
+        vs.S_s,
+        at[2:-2, 2:-2, vs.taum1], vs.S_s[2:-2, 2:-2, vs.tau],
+    )
+    vs.S = update(
+        vs.S,
+        at[2:-2, 2:-2, vs.taum1], vs.S[2:-2, 2:-2, vs.tau],
+    )
+    vs.z_sat = update(
+        vs.z_sat,
+        at[2:-2, 2:-2, vs.taum1], vs.z_sat[2:-2, 2:-2, vs.tau],
+    )
+    vs.z_wf = update(
+        vs.z_wf,
+        at[2:-2, 2:-2, vs.taum1], vs.z_wf[2:-2, 2:-2, vs.tau],
+    )
+    vs.z_wf_t0 = update(
+        vs.z_wf_t0,
+        at[2:-2, 2:-2, vs.taum1], vs.z_wf_t0[2:-2, 2:-2, vs.tau],
+    )
+    vs.z_wf_t1 = update(
+        vs.z_wf_t1,
+        at[2:-2, 2:-2, vs.taum1], vs.z_wf_t1[2:-2, 2:-2, vs.tau],
+    )
+    vs.y_mp = update(
+        vs.y_mp,
+        at[2:-2, 2:-2, vs.taum1], vs.y_mp[2:-2, 2:-2, vs.tau],
+    )
+    vs.y_sc = update(
+        vs.y_sc,
+        at[2:-2, 2:-2, vs.taum1], vs.y_sc[2:-2, 2:-2, vs.tau],
+    )
+    vs.theta_rz = update(
+        vs.theta_rz,
+        at[2:-2, 2:-2, vs.taum1], vs.theta_rz[2:-2, 2:-2, vs.tau],
+    )
+    vs.theta_ss = update(
+        vs.theta_ss,
+        at[2:-2, 2:-2, vs.taum1], vs.theta_ss[2:-2, 2:-2, vs.tau],
+    )
+    vs.theta = update(
+        vs.theta,
+        at[2:-2, 2:-2, vs.taum1], vs.theta[2:-2, 2:-2, vs.tau],
+    )
+    vs.k_rz = update(
+        vs.k_rz,
+        at[2:-2, 2:-2, vs.taum1], vs.k_rz[2:-2, 2:-2, vs.tau],
+    )
+    vs.k_ss = update(
+        vs.k_ss,
+        at[2:-2, 2:-2, vs.taum1], vs.k_ss[2:-2, 2:-2, vs.tau],
+    )
+    vs.k = update(
+        vs.k,
+        at[2:-2, 2:-2, vs.taum1], vs.k[2:-2, 2:-2, vs.tau],
+    )
+    vs.h_rz = update(
+        vs.h_rz,
+        at[2:-2, 2:-2, vs.taum1], vs.h_rz[2:-2, 2:-2, vs.tau],
+    )
+    vs.h_ss = update(
+        vs.h_ss,
+        at[2:-2, 2:-2, vs.taum1], vs.h_ss[2:-2, 2:-2, vs.tau],
+    )
+    vs.h = update(
+        vs.h,
+        at[2:-2, 2:-2, vs.taum1], vs.h[2:-2, 2:-2, vs.tau],
+    )
+    vs.z0 = update(
+        vs.z0,
+        at[2:-2, 2:-2, vs.taum1], vs.z0[2:-2, 2:-2, vs.tau],
+    )
+    # set to 0 for numerical errors
+    vs.S_fp_rz = update(
+        vs.S_fp_rz,
+        at[2:-2, 2:-2], npx.where((vs.S_fp_rz[2:-2, 2:-2] > -1e-6) & (vs.S_fp_rz[2:-2, 2:-2] < 0), 0, vs.S_fp_rz[2:-2, 2:-2]),
+    )
+    vs.S_lp_rz = update(
+        vs.S_lp_rz,
+        at[2:-2, 2:-2], npx.where((vs.S_lp_rz[2:-2, 2:-2] > -1e-6) & (vs.S_lp_rz[2:-2, 2:-2] < 0), 0, vs.S_lp_rz[2:-2, 2:-2]),
+    )
+    vs.S_fp_ss = update(
+        vs.S_fp_ss,
+        at[2:-2, 2:-2], npx.where((vs.S_fp_ss[2:-2, 2:-2] > -1e-6) & (vs.S_fp_ss[2:-2, 2:-2] < 0), 0, vs.S_fp_ss[2:-2, 2:-2]),
+    )
+    vs.S_lp_ss = update(
+        vs.S_lp_ss,
+        at[2:-2, 2:-2], npx.where((vs.S_lp_ss[2:-2, 2:-2] > -1e-6) & (vs.S_lp_ss[2:-2, 2:-2] < 0), 0, vs.S_lp_ss[2:-2, 2:-2]),
+    )
+    vs.prec = update(
+        vs.prec,
+        at[2:-2, 2:-2, vs.taum1], vs.prec[2:-2, 2:-2, vs.tau],
+    )
+    vs.event_id = update(
+        vs.event_id,
+        at[vs.taum1], vs.event_id[vs.tau],
+    )
+    vs.year = update(
+        vs.year,
+        at[vs.taum1], vs.year[vs.tau],
+    )
+    vs.month = update(
+        vs.month,
+        at[vs.taum1], vs.month[vs.tau],
+    )
+    vs.doy = update(
+        vs.doy,
+        at[vs.taum1], vs.doy[vs.tau],
     )
 
     return KernelOutput(
-        msa_rz=vs.msa_rz,
-        msa_ss=vs.msa_ss,
-        ma_rz=vs.ma_rz,
-        ma_ss=vs.ma_ss,
-        ma_s=vs.ma_s,
-        mr_rz=vs.mr_rz,
-        mr_ss=vs.mr_ss,
-        mr_s=vs.mr_s,
-        Nmin_rz=vs.Nmin_rz,
-        Nmin_ss=vs.Nmin_ss,
-        Nmin_s=vs.Nmin_s,
-        nit_s=vs.nit_s,
-        denit_s=vs.denit_s,
+        ta=vs.ta,
+        z_root=vs.z_root,
+        ground_cover=vs.ground_cover,
+        S_sur=vs.S_sur,
+        S_int_top=vs.S_int_top,
+        S_int_ground=vs.S_int_ground,
+        S_dep=vs.S_dep,
+        S_snow=vs.S_snow,
+        swe=vs.swe,
+        S_rz=vs.S_rz,
+        S_ss=vs.S_ss,
+        S_s=vs.S_s,
+        S=vs.S,
+        z_sat=vs.z_sat,
+        z_wf=vs.z_wf,
+        z_wf_t0=vs.z_wf_t0,
+        z_wf_t1=vs.z_wf_t1,
+        y_mp=vs.y_mp,
+        y_sc=vs.y_sc,
+        theta_rz=vs.theta_rz,
+        theta_ss=vs.theta_ss,
+        theta=vs.theta,
+        h_rz=vs.h_rz,
+        h_ss=vs.h_ss,
+        h=vs.h,
+        k_rz=vs.k_rz,
+        k_ss=vs.k_ss,
+        k=vs.k,
+        z0=vs.z0,
+        prec=vs.prec,
+        event_id=vs.event_id,
+        year=vs.year,
+        month=vs.month,
+        doy=vs.doy,
+        S_fp_rz=vs.S_fp_rz,
+        S_lp_rz=vs.S_lp_rz,
+        S_fp_ss=vs.S_fp_ss,
+        S_lp_ss=vs.S_lp_ss,
     )
 
-
 @roger_kernel
-def calc_nitrogen_cycle_gw_kernel(state):
+def after_timestep_crops_kernel(state):
     vs = state.variables
 
-    vs.mr_gw = update(
-        vs.mr_gw,
-        at[2:-2, 2:-2, :],
-        calc_denit_gw(state, vs.msa_gw, vs.k_calc_denit_gw)[2:-2, 2:-2, :] * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
-    )
+    vs.ta_min = update(vs.ta_min, at[2:-2, 2:-2, vs.taum1], vs.ta_min[2:-2, 2:-2, vs.tau])
+    vs.ta_max = update(vs.ta_max, at[2:-2, 2:-2, vs.taum1], vs.ta_max[2:-2, 2:-2, vs.tau])
+    vs.gdd_sum = update(vs.gdd_sum, at[2:-2, 2:-2, vs.taum1, :], vs.gdd_sum[2:-2, 2:-2, vs.tau, :])
+    vs.t_grow_cc = update(vs.t_grow_cc, at[2:-2, 2:-2, vs.taum1, :], vs.t_grow_cc[2:-2, 2:-2, vs.tau, :])
+    vs.t_grow_root = update(vs.t_grow_root, at[2:-2, 2:-2, vs.taum1, :], vs.t_grow_root[2:-2, 2:-2, vs.tau, :])
+    vs.ccc = update(vs.ccc, at[2:-2, 2:-2, vs.taum1, :], vs.ccc[2:-2, 2:-2, vs.tau, :])
+    vs.z_root_crop = update(vs.z_root_crop, at[2:-2, 2:-2, vs.taum1, :], vs.z_root_crop[2:-2, 2:-2, vs.tau, :])
+    vs.re_rg_pwp = update(vs.re_rg_pwp, at[2:-2, 2:-2], 0)
+    vs.re_rg = update(vs.re_rg, at[2:-2, 2:-2], 0)
+    vs.re_rl_pwp = update(vs.re_rl_pwp, at[2:-2, 2:-2], 0)
+    vs.re_rl = update(vs.re_rl, at[2:-2, 2:-2], 0)
 
-    vs.msa_gw = update_add(
-        vs.msa_gw,
-        at[2:-2, 2:-2, vs.tau, :],
-        -vs.mr_gw[2:-2, 2:-2, :],
+    return KernelOutput(
+        ta_min=vs.ta_min,
+        ta_max=vs.ta_max,
+        gdd_sum=vs.gdd_sum,
+        t_grow_cc=vs.t_grow_cc,
+        t_grow_root=vs.t_grow_root,
+        ccc=vs.ccc,
+        z_root_crop=vs.z_root_crop,
+        re_rg_pwp=vs.re_rg_pwp,
+        re_rg=vs.re_rg,
+        re_rl_pwp=vs.re_rl_pwp,
+        re_rl=vs.re_rl,
     )
-
-    return KernelOutput(msa_rz=vs.msa_rz, msa_ss=vs.msa_ss)
-
-
-@roger_routine
-def calculate_nitrogen_cycle(state):
-    """
-    Calculates nitrogen cycle
-    """
-    vs = state.variables
-    settings = state.settings
-
-    vs.update(calc_soil_temperature_kernel(state))
-    vs.update(calc_nitrogen_cycle_kernel(state))
-    if settings.enable_groundwater:
-        vs.update(calc_nitrogen_cycle_gw_kernel(state))
```

### Comparing `roger-3.0.4/roger/core/numerics.py` & `roger-3.0.5/roger/core/numerics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roger.core.operators import numpy as npx, update, at
 from roger import runtime_settings as rs, logger
 
 
 def validate_parameters_surface(state):
     vs = state.variables
 
-    mask1 = ((vs.slope > 1) | (vs.slope < 0)) & vs.maskCatch
+    mask1 = (vs.slope < 0) & vs.maskCatch
     if global_and(npx.any(mask1[2:-2, 2:-2])):
         raise ValueError("slope-parameter is out of range.")
 
     mask2 = ((vs.sealing > 1) | (vs.sealing < 0)) & vs.maskCatch
     if global_and(npx.any(mask2[2:-2, 2:-2])):
         raise ValueError("sealing-parameter is out of range.")
 
@@ -715,25 +715,25 @@
         and not settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_groundwater_boundary
         and not settings.enable_groundwater
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_ss[2:-2, 2:-2]
                     - vs.q_sub[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
@@ -758,27 +758,27 @@
         and settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_groundwater_boundary
         and not settings.enable_groundwater
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur_out[2:-2, 2:-2]
                     + vs.q_sur_in[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_ss[2:-2, 2:-2]
                     - vs.q_sub_out[2:-2, 2:-2]
                     + vs.q_sub_in[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
@@ -802,34 +802,34 @@
         settings.enable_lateral_flow
         and settings.enable_groundwater_boundary
         and not settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_ss[2:-2, 2:-2]
                     - vs.q_sub[2:-2, 2:-2]
                     + vs.cpr_ss[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
-                (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
-                & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
-                & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
-                & (npx.where(npx.isnan(vs.S_lp_ss[2:-2, 2:-2]) , 0,  vs.S_lp_ss[2:-2, 2:-2]) > -settings.atol)
+                (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]), 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
+                & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]), 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
+                & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]), 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
+                & (npx.where(npx.isnan(vs.S_lp_ss[2:-2, 2:-2]), 0,  vs.S_lp_ss[2:-2, 2:-2]) > -settings.atol)
             )
         )
         check3 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]), 0,  vs.S_fp_rz[2:-2, 2:-2]) - settings.atol <= npx.where(npx.isnan(vs.S_ufc_rz[2:-2, 2:-2]), 0,  vs.S_ufc_rz[2:-2, 2:-2]))
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]), 0,  vs.S_lp_rz[2:-2, 2:-2]) - settings.atol <= npx.where(npx.isnan(vs.S_ac_rz[2:-2, 2:-2]), 0,  vs.S_ac_rz[2:-2, 2:-2]))
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]), 0,  vs.S_fp_ss[2:-2, 2:-2]) - settings.atol <= npx.where(npx.isnan(vs.S_ufc_ss[2:-2, 2:-2]), 0,  vs.S_ufc_ss[2:-2, 2:-2]))
@@ -842,26 +842,26 @@
         settings.enable_lateral_flow
         and settings.enable_groundwater
         and not settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_sub[2:-2, 2:-2]
                     - vs.q_gw[2:-2, 2:-2]
                     - vs.q_leak[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
@@ -882,25 +882,25 @@
         settings.enable_groundwater_boundary
         and not settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_lateral_flow
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_ss[2:-2, 2:-2]
                     + vs.cpr_ss[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
@@ -920,25 +920,25 @@
     elif (
         settings.enable_film_flow
         and not settings.enable_routing_1D
         and not settings.enable_routing_2D
         and not settings.enable_offline_transport
     ):
         check1 = global_and(
-            npx.all(
+            npx.all(npx.where(vs.maskCatch[2:-2, 2:-2],
                 npx.isclose(
                     vs.S[2:-2, 2:-2, vs.tau] - vs.S[2:-2, 2:-2, vs.taum1],
                     vs.prec[2:-2, 2:-2, vs.tau]
                     - vs.q_sur[2:-2, 2:-2]
                     - vs.aet[2:-2, 2:-2]
                     - vs.q_ss[2:-2, 2:-2]
                     - vs.ff_drain[2:-2, 2:-2],
                     atol=settings.atol,
                     rtol=settings.rtol,
-                )
+                ), True)
             )
         )
         check2 = global_and(
             npx.all(
                 (npx.where(npx.isnan(vs.S_fp_rz[2:-2, 2:-2]) , 0,  vs.S_fp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_lp_rz[2:-2, 2:-2]) , 0,  vs.S_lp_rz[2:-2, 2:-2]) > -settings.atol)
                 & (npx.where(npx.isnan(vs.S_fp_ss[2:-2, 2:-2]) , 0,  vs.S_fp_ss[2:-2, 2:-2]) > -settings.atol)
```

### Comparing `roger-3.0.4/roger/core/operators.py` & `roger-3.0.5/roger/core/operators.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/root_zone.py` & `roger-3.0.5/roger/core/root_zone.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/sas.py` & `roger-3.0.5/roger/core/sas.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/snow.py` & `roger-3.0.5/roger/core/snow.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,19 @@
         at[2:-2, 2:-2], -vs.swe_top[2:-2, 2:-2, vs.tau] * mask5[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
     vs.swe_top = update_add(
         vs.swe_top,
         at[2:-2, 2:-2, vs.tau], npx.where(mask5[2:-2, 2:-2], 0, -vs.swe_top[2:-2, 2:-2, vs.tau]) * vs.maskCatch[2:-2, 2:-2],
     )
 
+    vs.pet_res = update(
+        vs.pet_res,
+        at[2:-2, 2:-2], npx.where(vs.pet_res[2:-2, 2:-2] < 0, 0, vs.pet_res[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
+
     # snow layer retention storage
     wtmx = allocate(state.dimensions, ("x", "y"))
     wtmx = (10000. / (100 - settings.rmax) / 100.) * vs.swe_top[:, :, vs.tau]
     # retained water
     q_ret = allocate(state.dimensions, ("x", "y"))
     q_ret = update(
         q_ret,
@@ -240,14 +245,18 @@
         vs.pet_res,
         at[2:-2, 2:-2], -vs.swe[2:-2, 2:-2, vs.tau] * mask6[2:-2, 2:-2] * vs.maskCatch[2:-2, 2:-2],
     )
     vs.swe = update(
         vs.swe,
         at[2:-2, 2:-2, vs.tau], npx.where(mask6[2:-2, 2:-2], 0, vs.swe[2:-2, 2:-2, vs.tau]) * vs.maskCatch[2:-2, 2:-2],
     )
+    vs.pet_res = update(
+        vs.pet_res,
+        at[2:-2, 2:-2], npx.where(vs.pet_res[2:-2, 2:-2] < 0, 0, vs.pet_res[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
 
     # snow layer retention storage
     wtmx = allocate(state.dimensions, ("x", "y"))
     wtmx = (10000. / (100 - settings.rmax) / 100.) * vs.swe[:, :, vs.tau]
     # retained water
     q_ret = allocate(state.dimensions, ("x", "y"))
     q_ret = update(
```

### Comparing `roger-3.0.4/roger/core/soil.py` & `roger-3.0.5/roger/core/soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -809,20 +809,38 @@
             vs.S_pwp_rz[2:-2, 2:-2, npx.newaxis]
             + vs.S_fp_rz[2:-2, 2:-2, npx.newaxis]
             + vs.S_lp_rz[2:-2, 2:-2, npx.newaxis]
         )
         * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
+    vs.theta_rz = update(
+        vs.theta_rz,
+        at[2:-2, 2:-2, vs.tau], ((vs.S_fp_rz[2:-2, 2:-2] + vs.S_lp_rz[2:-2, 2:-2])/vs.z_root[2:-2, 2:-2, vs.tau] + vs.theta_pwp[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.k_rz = update(
+        vs.k_rz,
+        at[2:-2, 2:-2, vs.tau], (vs.ks[2:-2, 2:-2]/(1 + (vs.theta_rz[2:-2, 2:-2, vs.tau]/vs.theta_sat[2:-2, 2:-2])**(-vs.m_bc[2:-2, 2:-2]))) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.h_rz = update(
+        vs.h_rz,
+        at[2:-2, 2:-2, vs.tau], (vs.ha[2:-2, 2:-2]/((vs.theta_rz[2:-2, 2:-2, vs.tau]/vs.theta_sat[2:-2, 2:-2])**(1/vs.lambda_bc[2:-2, 2:-2]))) * vs.maskCatch[2:-2, 2:-2],
+    )
+
     return KernelOutput(
         theta_fp_rz=vs.theta_fp_rz,
         theta_lp_rz=vs.theta_lp_rz,
         S_fp_rz=vs.S_fp_rz,
         S_lp_rz=vs.S_lp_rz,
         S_rz=vs.S_rz,
+        theta_rz=vs.theta_rz,
+        k_rz=vs.k_rz,
+        h_rz=vs.h_rz,
     )
 
 
 @roger_kernel
 def calc_initial_conditions_subsoil_kernel(state):
     vs = state.variables
 
@@ -885,20 +903,38 @@
             vs.S_pwp_ss[2:-2, 2:-2, npx.newaxis]
             + vs.S_fp_ss[2:-2, 2:-2, npx.newaxis]
             + vs.S_lp_ss[2:-2, 2:-2, npx.newaxis]
         )
         * vs.maskCatch[2:-2, 2:-2, npx.newaxis],
     )
 
+    vs.theta_ss = update(
+        vs.theta_ss,
+        at[2:-2, 2:-2, vs.tau], ((vs.S_fp_ss[2:-2, 2:-2] + vs.S_lp_ss[2:-2, 2:-2])/(vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.tau]) + vs.theta_pwp[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.k_ss = update(
+        vs.k_ss,
+        at[2:-2, 2:-2, vs.tau], (vs.ks[2:-2, 2:-2]/(1 + (vs.theta_ss[2:-2, 2:-2, vs.tau]/vs.theta_sat[2:-2, 2:-2])**(-vs.m_bc[2:-2, 2:-2]))) * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    vs.h_ss = update(
+        vs.h_ss,
+        at[2:-2, 2:-2, vs.tau], (vs.ha[2:-2, 2:-2]/((vs.theta_ss[2:-2, 2:-2, vs.tau]/vs.theta_sat[2:-2, 2:-2])**(1/vs.lambda_bc[2:-2, 2:-2]))) * vs.maskCatch[2:-2, 2:-2],
+    )
+
     return KernelOutput(
         theta_fp_ss=vs.theta_fp_ss,
         theta_lp_ss=vs.theta_lp_ss,
         S_fp_ss=vs.S_fp_ss,
         S_lp_ss=vs.S_lp_ss,
         S_ss=vs.S_ss,
+        theta_ss=vs.theta_ss,
+        k_ss=vs.k_ss,
+        h_ss=vs.h_ss,
     )
 
 
 @roger_kernel
 def calc_initial_conditions_kernel(state):
     vs = state.variables
```

### Comparing `roger-3.0.4/roger/core/subsoil.py` & `roger-3.0.5/roger/core/subsoil.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/subsurface_runoff.py` & `roger-3.0.5/roger/core/subsurface_runoff.py`

 * *Files 8% similar despite different names*

```diff
@@ -250,43 +250,39 @@
     """
     Calculates potential lateral subsurface runoff
     """
     vs = state.variables
     settings = state.settings
 
     # calculate potential matrix subsurface runoff with darcy (in mm/dt)
-    # convert mm3 to mm (1e-6)
+    # convert mm3 to liter (1e-6)
     vs.q_sub_mat_pot = update(
         vs.q_sub_mat_pot,
         at[2:-2, 2:-2],
-        ((vs.ks[2:-2, 2:-2] * vs.slope[2:-2, 2:-2] * vs.z_sat[2:-2, 2:-2, vs.tau] * vs.dt) * 1e-6)
+        ((vs.ks[2:-2, 2:-2] * vs.slope[2:-2, 2:-2] * vs.z_sat[2:-2, 2:-2, vs.tau] * settings.dx * 1000 * vs.dt) * 1e-6 * (1 / (settings.dx * settings.dy)))
         * vs.maskCatch[2:-2, 2:-2],
     )
 
     # total potential macropore subsurface runoff (in mm/dt)
-    # convert mm3 to mm (1e-9)
+    # convert mm3 to liter (1e-6)
     vs.q_sub_mp_pot = update(
         vs.q_sub_mp_pot,
         at[2:-2, 2:-2],
         (
             (
-                vs.z_sat_layer_1[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_1[2:-2, 2:-2]
-                + vs.z_sat_layer_2[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_2[2:-2, 2:-2]
-                + vs.z_sat_layer_3[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_3[2:-2, 2:-2]
-                + vs.z_sat_layer_4[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_4[2:-2, 2:-2]
-                + vs.z_sat_layer_5[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_5[2:-2, 2:-2]
-                + vs.z_sat_layer_6[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_6[2:-2, 2:-2]
-                + vs.z_sat_layer_7[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_7[2:-2, 2:-2]
-                + vs.z_sat_layer_8[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_8[2:-2, 2:-2]
+                  vs.z_sat_layer_1[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_1[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_2[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_2[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_3[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_3[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_4[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_4[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_5[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_5[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_6[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_6[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_7[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_7[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
+                + vs.z_sat_layer_8[2:-2, 2:-2, vs.tau] * vs.v_mp_layer_8[2:-2, 2:-2] * vs.dt * settings.dx * 1000 * vs.dmph[2:-2, 2:-2] * 1e-6 * settings.r_mp**2 * settings.pi * 1e-6 
             )
-            * vs.dt
-            * vs.dmph[2:-2, 2:-2]
-            * settings.r_mp**2
-            * settings.pi
-            * 1e-9
+            * (1 / (settings.dx * settings.dy))
         )
         * vs.maskCatch[2:-2, 2:-2],
     )
     vs.q_sub_mp_pot = update(
         vs.q_sub_mp_pot,
         at[2:-2, 2:-2],
         npx.where(vs.q_sub_mp_pot[2:-2, 2:-2] < 0, 0, vs.q_sub_mp_pot[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
@@ -799,15 +795,15 @@
                 / (
                     1
                     + npx.power(-vs.h_rz[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
                     + (vs.n_salv[2:-2, 2:-2] - 1)
                     * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
                 )
             )
-            * vs.dt,
+            * vs.dt * vs.ks[2:-2, 2:-2] * (-1),
             perc_pot[2:-2, 2:-2],
         )
         * vs.maskCatch[2:-2, 2:-2],
     )
     perc_pot = update(
         perc_pot,
         at[2:-2, 2:-2],
@@ -970,38 +966,57 @@
     # potential drainage rate
     # calculate potential percolation rate
     perc_pot = allocate(state.dimensions, ("x", "y"))
     z = allocate(state.dimensions, ("x", "y"))
     z = update(
         z,
         at[2:-2, 2:-2],
-        vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_soil[2:-2, 2:-2],
+        (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_soil[2:-2, 2:-2]) + ((vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.tau])/2) * vs.maskCatch[2:-2, 2:-2],
     )
     perc_pot = update(
         perc_pot,
         at[2:-2, 2:-2],
         npx.where(
-            (vs.z_gw[2:-2, 2:-2, vs.tau] > 10) & (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 > vs.z_soil[2:-2, 2:-2]),
+            (vs.z_gw[2:-2, 2:-2, vs.tau] > 10) & (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 > vs.z_soil[2:-2, 2:-2]) & (vs.z_sat[2:-2, 2:-2, vs.tau] > 0),
             npx.fmin(npx.fmin(vs.kf[2:-2, 2:-2] * vs.dt, vs.ks[2:-2, 2:-2] * vs.dt), vs.k_ss[2:-2, 2:-2, vs.tau] * vs.dt),
-            npx.where(
-                vs.z_sat[2:-2, 2:-2, vs.tau] > 0,
-                npx.fmin(vs.kf[2:-2, 2:-2] * vs.dt, vs.ks[2:-2, 2:-2] * vs.dt),
                 npx.fmin(
                     vs.kf[2:-2, 2:-2] * vs.dt,
                     (
                         npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
                         / (
                             (1 + (vs.n_salv[2:-2, 2:-2] - 1))
                             * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
                         )
                     )
-                    * vs.dt,
-                ),
-            ),
-        )
+                    * vs.dt * vs.ks[2:-2, 2:-2],
+                )
+            )
+        * vs.maskCatch[2:-2, 2:-2],
+    )
+
+    perc_pot = update(
+        perc_pot,
+        at[2:-2, 2:-2],
+        npx.where(
+            (vs.z_gw[2:-2, 2:-2, vs.tau] <= 10) & (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 > vs.z_soil[2:-2, 2:-2]) & (vs.z_sat[2:-2, 2:-2, vs.tau] > 0),
+            npx.fmin(npx.fmin(vs.kf[2:-2, 2:-2] * vs.dt, vs.ks[2:-2, 2:-2] * vs.dt), vs.k_ss[2:-2, 2:-2, vs.tau] * vs.dt),
+                npx.fmin(
+                    vs.kf[2:-2, 2:-2] * vs.dt,
+                    (
+                        npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
+                        - npx.power(-vs.h_ss[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
+                    )
+                    / (
+                        1
+                        + npx.power(-vs.h_ss[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
+                        + (vs.n_salv[2:-2, 2:-2] - 1)
+                        * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
+                    ) * vs.dt * vs.ks[2:-2, 2:-2] * (-1),
+                )
+            )
         * vs.maskCatch[2:-2, 2:-2],
     )
 
     # where drainage occurs
     mask1 = (perc_pot > 0) & (vs.z_soil < vs.z_gw[:, :, vs.tau] * 1000) & (perc_pot <= vs.S_fp_ss + vs.S_lp_ss)
     mask2 = (perc_pot > 0) & (vs.z_soil < vs.z_gw[:, :, vs.tau] * 1000) & (perc_pot > vs.S_fp_ss + vs.S_lp_ss)
 
@@ -1026,20 +1041,15 @@
     # percolation stops while shallow groundwater table or groundwater table
     # rises into soil
     z = allocate(state.dimensions, ("x", "y"))
     cpr_pot = allocate(state.dimensions, ("x", "y"))
     z = update(
         z,
         at[2:-2, 2:-2],
-        npx.where(
-            vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 < vs.z_soil[2:-2, 2:-2],
-            0,
-            vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_soil[2:-2, 2:-2],
-        )
-        * vs.maskCatch[2:-2, 2:-2],
+        (vs.z_gw[2:-2, 2:-2, vs.tau] * 1000 - vs.z_soil[2:-2, 2:-2]) + ((vs.z_soil[2:-2, 2:-2] - vs.z_root[2:-2, 2:-2, vs.tau])/2) * vs.maskCatch[2:-2, 2:-2],
     )
     cpr_pot = update(
         cpr_pot,
         at[2:-2, 2:-2],
         (
             (
                 npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
@@ -1047,26 +1057,34 @@
             )
             / (
                 1
                 + npx.power(-vs.h_ss[2:-2, 2:-2, vs.tau] / -vs.ha[2:-2, 2:-2], -vs.n_salv[2:-2, 2:-2])
                 + (vs.n_salv[2:-2, 2:-2] - 1)
                 * npx.power((z[2:-2, 2:-2]) / (-vs.ha[2:-2, 2:-2] * 10.2), -vs.n_salv[2:-2, 2:-2])
             )
-        )
+        ) * vs.dt * vs.ks[2:-2, 2:-2]
         * vs.maskCatch[2:-2, 2:-2],
     )
     cpr_pot = update(
         cpr_pot,
         at[2:-2, 2:-2],
-        npx.where(z[2:-2, 2:-2] > 0, 0, cpr_pot[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+        npx.where((perc_pot[2:-2, 2:-2] > 0) & (vs.z_soil[2:-2, 2:-2] < vs.z_gw[2:-2, 2:-2, vs.tau] * 1000), 0, cpr_pot[2:-2, 2:-2]) * vs.maskCatch[2:-2, 2:-2],
+    )
+    mask3 = (vs.z_gw[:, :, vs.tau] * 1000 - vs.z_soil[:, :] > 10000)
+    cpr_pot = update(
+        cpr_pot,
+        at[2:-2, 2:-2],
+        npx.where(mask3[2:-2, 2:-2], 0, cpr_pot[2:-2, 2:-2])
+        * vs.maskCatch[2:-2, 2:-2],
     )
+
     vs.q_pot_ss = update(
         vs.q_pot_ss,
         at[2:-2, 2:-2],
-        npx.where((cpr_pot[2:-2, 2:-2] > 0) & (z[2:-2, 2:-2] > 0), 0, vs.q_pot_ss[2:-2, 2:-2])
+        npx.where((cpr_pot[2:-2, 2:-2] > 0), 0, vs.q_pot_ss[2:-2, 2:-2])
         * vs.maskCatch[2:-2, 2:-2],
     )
 
     return KernelOutput(q_pot_ss=vs.q_pot_ss)
 
 
 @roger_kernel
```

### Comparing `roger-3.0.4/roger/core/surface.py` & `roger-3.0.5/roger/core/surface.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/surface_runoff.py` & `roger-3.0.5/roger/core/surface_runoff.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/transport.py` & `roger-3.0.5/roger/core/transport.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/core/utilities.py` & `roger-3.0.5/roger/core/utilities.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/api.py` & `roger-3.0.5/roger/diagnostics/api.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/average.py` & `roger-3.0.5/roger/diagnostics/average.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/base.py` & `roger-3.0.5/roger/diagnostics/base.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/collect.py` & `roger-3.0.5/roger/diagnostics/collect.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/constant.py` & `roger-3.0.5/roger/diagnostics/constant.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/maximum.py` & `roger-3.0.5/roger/diagnostics/maximum.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/minimum.py` & `roger-3.0.5/roger/diagnostics/minimum.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/rate.py` & `roger-3.0.5/roger/diagnostics/rate.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/snapshot.py` & `roger-3.0.5/roger/diagnostics/snapshot.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/tracer_monitor.py` & `roger-3.0.5/roger/diagnostics/tracer_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/diagnostics/water_monitor.py` & `roger-3.0.5/roger/diagnostics/water_monitor.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/distributed.py` & `roger-3.0.5/roger/distributed.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/io_tools/csv.py` & `roger-3.0.5/roger/io_tools/csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
 import os
 import glob
 import pandas as pd
 from datetime import datetime
+import warnings
+warnings.filterwarnings("ignore", category=UserWarning)
 
 
 def read_meteo(path_to_dir: Path):
     """Reads the meteorological data
 
     Data is imported from .txt files and stored in dataframes. Format of NA/NaN
     values is -9999.
@@ -36,74 +38,71 @@
     RS_path = path_to_dir / "RS.txt"
 
     df_PREC = pd.read_csv(
         PREC_path,
         sep=r"\s+",
         skiprows=0,
         header=0,
-        parse_dates=[[0, 1, 2, 3, 4]],
-        index_col=0,
         na_values=-9999,
     )
-    df_PREC.index = pd.to_datetime(df_PREC.index, format="%Y %m %d %H %M")
+    df_PREC.index = [pd.to_datetime(f"{df_PREC.iloc[i, 0]} {df_PREC.iloc[i, 1]} {df_PREC.iloc[i, 2]} {df_PREC.iloc[i, 3]} {df_PREC.iloc[i, 4]}", format="%Y %m %d %H %M") for i in range(len(df_PREC.index))]
+    df_PREC = df_PREC.loc[:, ["PREC"]]
     df_PREC.index = df_PREC.index.rename("Index")
 
     if os.path.exists(PET_path):
         df_pet = pd.read_csv(
             PET_path,
             sep=r"\s+",
             skiprows=0,
             header=0,
-            parse_dates=[[0, 1, 2, 3, 4]],
-            index_col=0,
             na_values=-9999,
         )
-        df_pet.index = pd.to_datetime(df_pet.index, format="%Y %m %d %H %M")
+        df_pet.index = [pd.to_datetime(f"{df_pet.iloc[i, 0]} {df_pet.iloc[i, 1]} {df_pet.iloc[i, 2]} {df_pet.iloc[i, 3]} {df_pet.iloc[i, 4]}", format="%Y %m %d %H %M") for i in range(len(df_pet.index))]
+        df_pet = df_pet.loc[:, ["PET"]]
         df_pet.index = df_pet.index.rename("Index")
+
     else:
         df_pet = None
 
     if os.path.exists(RS_path):
         df_rs = pd.read_csv(
             RS_path,
             sep=r"\s+",
             skiprows=0,
             header=0,
-            parse_dates=[[0, 1, 2, 3, 4]],
-            index_col=0,
             na_values=-9999,
         )
-        df_rs.index = pd.to_datetime(df_rs.index, format="%Y %m %d %H %M")
+        df_rs.index = [pd.to_datetime(f"{df_rs.iloc[i, 0]} {df_rs.iloc[i, 1]} {df_rs.iloc[i, 2]} {df_rs.iloc[i, 3]} {df_rs.iloc[i, 4]}", format="%Y %m %d %H %M") for i in range(len(df_rs.index))]
+        df_rs = df_rs.loc[:, ["RS"]]
         df_rs.index = df_rs.index.rename("Index")
     else:
         df_rs = None
 
     df_ta = pd.read_csv(
         Ta_path,
         sep=r"\s+",
         skiprows=0,
         header=0,
-        parse_dates=[[0, 1, 2, 3, 4]],
-        index_col=0,
         na_values=-9999,
     )
-    df_ta.index = pd.to_datetime(df_ta.index, format="%Y %m %d %H %M")
+    df_ta.index = [pd.to_datetime(f"{df_ta.iloc[i, 0]} {df_ta.iloc[i, 1]} {df_ta.iloc[i, 2]} {df_ta.iloc[i, 3]} {df_ta.iloc[i, 4]}", format="%Y %m %d %H %M") for i in range(len(df_ta.index))]
+    df_ta = df_ta.loc[:, "TA":]
     df_ta.index = df_ta.index.rename("Index")
 
     # reset index of precipitation time series
     # time series starts on first day at 00:00 and ends on last day at 23:50
     prec_ind = df_PREC.index
     new_prec_ind = pd.date_range(
         start=datetime(prec_ind[0].year, prec_ind[0].month, prec_ind[0].day, 0, 0),
         end=datetime(prec_ind[-1].year, prec_ind[-1].month, prec_ind[-1].day, 23, 50),
-        freq="10T",
+        freq="10min",
     )
     prec_10mins = pd.DataFrame(index=new_prec_ind)
-    prec_10mins["PREC"] = 0
-    prec_10mins.loc[df_PREC.index, "PREC"] = df_PREC["PREC"].values
+    prec_10mins["PREC"] = 0.
+    prec_10mins.loc[df_PREC.index, "PREC"] = df_PREC["PREC"].values.astype(float)
 
     return prec_10mins, df_pet, df_ta, df_rs
 
 
 def write_meteo_csv_from_dwd(path_to_dir: Path):
     """Writes the meteorological data downloaded from WeatherDB
     (https://weather.hydro.intra.uni-freiburg.de/)
@@ -161,15 +160,15 @@
 
     # reset index of precipitation time series
     # time series starts on first day at 00:00 and ends on last day at 23:50
     prec_ind = df_prec.index
     new_prec_ind = pd.date_range(
         start=datetime(prec_ind[0].year, prec_ind[0].month, prec_ind[0].day, 0, 0),
         end=datetime(prec_ind[-1].year, prec_ind[-1].month, prec_ind[-1].day, 23, 50),
-        freq="10T",
+        freq="10min",
     )
     prec_10mins = pd.DataFrame(index=new_prec_ind)
     prec_10mins["PREC"] = 0
     prec_10mins.loc[df_prec.index, "PREC"] = df_prec["N"].values.astype(float)
 
     Ta_path = path_to_dir / "TA.txt"
     PREC_path = path_to_dir / "PREC.txt"
```

### Comparing `roger-3.0.4/roger/io_tools/hdf5.py` & `roger-3.0.5/roger/io_tools/hdf5.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/io_tools/netcdf.py` & `roger-3.0.5/roger/io_tools/netcdf.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/io_tools/yml.py` & `roger-3.0.5/roger/io_tools/yml.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/logs.py` & `roger-3.0.5/roger/logs.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/lookuptables.py` & `roger-3.0.5/roger/lookuptables.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,36 +22,43 @@
 
 path_cp = CSV_DIR / "crop_parameters.csv"
 df_cp = pd.read_csv(path_cp, sep=";", na_values=-9999, skiprows=1)
 ARR_CP = onp.asarray(df_cp.values)
 
 path_fert1 = CSV_DIR / "fertilization1.csv"
 df_fert1 = pd.read_csv(path_fert1, sep=";", na_values=-9999, skiprows=1)
+df_fert1.fillna(0, inplace=True)
 ARR_FERT1 = onp.asarray(df_fert1.values)
 
 path_fert2 = CSV_DIR / "fertilization2.csv"
 df_fert2 = pd.read_csv(path_fert2, sep=";", na_values=-9999, skiprows=1)
+df_fert2.fillna(0, inplace=True)
 ARR_FERT2 = onp.asarray(df_fert2.values)
 
 path_fert3 = CSV_DIR / "fertilization3.csv"
 df_fert3 = pd.read_csv(path_fert3, sep=";", na_values=-9999, skiprows=1)
+df_fert3.fillna(0, inplace=True)
 ARR_FERT3 = onp.asarray(df_fert3.values)
 
+path_nup = CSV_DIR / "nitrogen_uptake.csv"
+df_nup = pd.read_csv(path_nup, sep=";", na_values=-9999, skiprows=1)
+df_nup.fillna(0, inplace=True)
+ARR_NUP = onp.asarray(df_nup.iloc[:, :-1].values)
+
 ARR_GC = onp.zeros((25, 13))
 ARR_GC[:, 0] = ARR_ILU[:, 0]
 ARR_GC[:, 1:] = 1 - 0.7 ** (ARR_ILU[:, 1:] / 0.2)
 
 ARR_GCM = onp.zeros((25, 2))
 ARR_GCM[:, 0] = ARR_ILU[:, 0]
 
 ARR_GCM[:, 1] = onp.max(ARR_GC[:, 1:], axis=1)
 
 SUMMER_CROPS = onp.array(
-    [
-        501,
+    [   501,
         502,
         503,
         504,
         505,
         506,
         507,
         508,
@@ -106,22 +113,23 @@
         562,
         563,
         565,
         567,
     ],
     dtype=onp.int32,
 )
-WINTER_CROPS = onp.array([556, 557, 558, 559, 560, 564], dtype=onp.int32)
-WINTER_CATCH_CROPS = onp.array([566, 568, 569, 570], dtype=onp.int32)
+WINTER_CROPS = onp.array([556, 557, 558, 559, 560, 564, 579], dtype=onp.int32)
+WINTER_CATCH_CROPS = onp.array([566, 568, 569, 570, 586, 587], dtype=onp.int32)
 MULTI_YEAR_CROPS_INIT = onp.array([571, 572, 580, 583], dtype=onp.int32)
 MULTI_YEAR_CROPS_CONT = onp.array([573, 574, 581, 582, 584, 585], dtype=onp.int32)
 WINTER_MULTI_YEAR_CROPS_INIT = onp.array([572, 583], dtype=onp.int32)
-WINTER_MULTI_YEAR_CROPS_CONT = onp.array([574, 581, 585], dtype=onp.int32)
-SUMMER_MULTI_YEAR_CROPS_INIT = onp.array([571, 580], dtype=onp.int32)
+WINTER_MULTI_YEAR_CROPS_CONT = onp.array([574, 581, 585, 590], dtype=onp.int32)
+SUMMER_MULTI_YEAR_CROPS_INIT = onp.array([571, 580, 589], dtype=onp.int32)
 SUMMER_MULTI_YEAR_CROPS_CONT = onp.array([573, 582, 584], dtype=onp.int32)
+WINTER_CROPS_FERT = onp.array([556, 557, 558, 559, 560, 564, 579, 580, 582, 584], dtype=onp.int32)
 
 dict_crops = {
     536: "beetroot",
     539: "silage_corn",
     543: "summer wheat",
     556: "winter barley",
     557: "winter wheat",
```

### Comparing `roger-3.0.4/roger/models/dummy/dummy.py` & `roger-3.0.5/roger/models/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/models/oneD/oneD.py` & `roger-3.0.5/roger/models/oneD/oneD.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/models/oneD_event/oneD_event.py` & `roger-3.0.5/roger/models/oneD_event/oneD_event.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/models/svat/svat.py` & `roger-3.0.5/roger/models/svat/svat.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/models/svat_bromide/svat_bromide.py` & `roger-3.0.5/roger/models/svat_bromide/svat_bromide.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/models/svat_oxygen18/svat_oxygen18.py` & `roger-3.0.5/roger/models/svat_oxygen18/svat_oxygen18.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/plugins.py` & `roger-3.0.5/roger/plugins.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/progress.py` & `roger-3.0.5/roger/progress.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/restart.py` & `roger-3.0.5/roger/restart.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/roger.py` & `roger-3.0.5/roger/roger.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/routines.py` & `roger-3.0.5/roger/routines.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/runtime.py` & `roger-3.0.5/roger/runtime.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/settings.py` & `roger-3.0.5/roger/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "ff_tc": Setting(0.15, float, "film flow termination criterium in -"),
     "VSMOW_conc18O": Setting(2005.2e-6, float, "oxygen-18 abundancy ratios according to VSMOW in -"),
     "d18O_min": Setting(-20, float, "potentially lowest oxygen-18 value in per mille"),
     "d18O_max": Setting(0, float, "potentially greatest oxygen-18 value in per mille"),
     "VSMOW_conc2H": Setting(155.76e-6, float, "deuterium abundancy ratios according to VSMOW in -"),
     "d2H_min": Setting(-160, float, "potentially lowest deuterium value in per mille"),
     "d2H_max": Setting(0, float, "potentially greatest deuterium value in per mille"),
+    "cum_inf_for_N_input": Setting(20, float, "cumulated infiltration required for nitrogen input in mm"),
     # Logical switches for general model setup
     "coord_degree": Setting(False, bool, "either spherical (True) or cartesian (False) coordinates"),
     "enable_distributed_input": Setting(False, bool, "enable distributed input"),
     "enable_film_flow": Setting(False, bool, "enable film flow process"),
     "enable_lateral_flow": Setting(False, bool, "enable lateral flow"),
     "enable_crop_phenology": Setting(False, bool, "enable crop phenology"),
     "enable_crop_rotation": Setting(False, bool, "enable crop rotation"),
```

### Comparing `roger-3.0.4/roger/signals.py` & `roger-3.0.5/roger/signals.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/state.py` & `roger-3.0.5/roger/state.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/time.py` & `roger-3.0.5/roger/time.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/tools/evaluation.py` & `roger-3.0.5/roger/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/tools/event_classification.py` & `roger-3.0.5/roger/tools/event_classification.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/tools/filelock.py` & `roger-3.0.5/roger/tools/filelock.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/tools/labels.py` & `roger-3.0.5/roger/tools/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     "theta_ss": r"$\theta_{subsoil}$ [-]",
     "S_snow": r"$S_{snow}$ [mm]",
     "S_s": r"$S_s$ [mm]",
     "S_vad": r"$S_{vad}$ [mm]",
     "ta": r"$TA$ [degC]",
     "z_root": r"$z_{root}$ [mm]",
     "ground_cover": r"GC [-]",
+    "transp_coeff": r"c_{TRANSP} [-]",
+    "basal_transp_coeff": r"bc_{TRANSP} [-]",
+    "k_stress_transp": r"k_{TS} [-]",
+    "z0": r"z0 [mm]",
 }
 
 _Y_LABS_HOURLY = {
     "prec": r"$PREC$ [mm $hour^{-1}$]",
     "prec_corr": r"$PREC_{corr}$ [mm $hour^{-1}$]",
     "q_hof": r"$q_{hof}$ [mm $hour^{-1}$]",
     "q_sof": r"$q_{sof}$ [mm $hour^{-1}$]",
```

### Comparing `roger-3.0.4/roger/tools/make_toy_data.py` & `roger-3.0.5/roger/tools/make_toy_data.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/tools/setup.py` & `roger-3.0.5/roger/tools/setup.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/roger/variables.py` & `roger-3.0.5/roger/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 BOUNDGW_GRID = ("x", "y")
 LUT_ILU_GRID = ("n_lu", "n_params13")
 LUT_GC_GRID = ("n_lu", "n_params13")
 LUT_IS_GRID = ("n_sealing", "n_params2")
 LUT_MLMS_GRID = ("n_slope", "n_params9")
 LUT_RDLU_GRID = ("n_lu", "n_params7")
 LUT_CROPS_GRID = ("n_crop_types", "n_crop_params")
-LUT_FERT_GRID = ("n_crop_types", "n_params9")
+LUT_FERT_GRID = ("n_crop_types", "n_params13")
+LUT_NUP_GRID = ("n_crop_types", "n_params3")
 LUT_GCM_GRID = ("n_lu", "n_params2")
 TIMESTEPS = ("timesteps",)
 TIMESTEPS_DAY = ("timesteps_day",)
 TIMESTEPS_EVENT_FF = ("timesteps_event_ff",)
 TIMESTEPS_EVENT_FF_P1 = ("timesteps_event_ff_p1",)
 TIME = ("t",)
 TIME_FORCING = ("t_forc",)
@@ -105,20 +106,21 @@
     "timesteps_event_ff_p1": "nittevent_ff_p1",
     "ages": "ages",
     "nages": "nages",
     "crops": "ncrops",
     "cr": "ncr",
     "events_ff": "nevent_ff",
     "n_sas_params": "nsas",
-    "n_crop_types": 88,
+    "n_crop_types": 91,
     "n_crop_params": 24,
     "n_lu": 25,
     "n_sealing": 101,
     "n_slope": 10000,
     "n_params2": 2,
+    "n_params3": 3,
     "n_params7": 7,
     "n_params9": 9,
     "n_params13": 13,
     "n_flowdir": "nflowdirs",
 }
 
 DEFAULT_MASKS = {
@@ -337,14 +339,68 @@
         CATCH_GRID,
         "",
         "Day of year at Current iteration",
         dtype="int32",
         initial=1,
         active=lambda settings: settings.enable_nitrate,
     ),
+    "doy_fert1": Variable(
+        "Day of year of first mineral fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of first mineral fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "doy_fert2": Variable(
+        "Day of year of second mineral fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of second mineral fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "doy_fert3": Variable(
+        "Day of year of third mineral fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of third mineral fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "doy_fert1_org": Variable(
+        "Day of year of first organic fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of first organic fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "doy_fert2_org": Variable(
+        "Day of year of second organic fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of second organic fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "doy_fert3_org": Variable(
+        "Day of year of third organic fertilizer application",
+        CATCH_GRID,
+        "",
+        "Day of year of third organic fertilizer application",
+        dtype="int32",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
     "DOY": Variable(
         "Day of year",
         TIME_FORCING,
         "",
         "Day of year",
         dtype="int32",
         write_to_restart=True,
@@ -2024,27 +2080,59 @@
         "denitrification of soil nitrate",
         CATCH_GRID,
         "mg/dt",
         "denitrification of soil nitrate",
         time_dependent=True,
         active=lambda settings: settings.enable_nitrate,
     ),
+    "ngas_s": Variable(
+        "gaseous loss of ammonium",
+        CATCH_GRID,
+        "mg/dt",
+        "gaseous loss of ammonium",
+        time_dependent=True,
+        active=lambda settings: settings.enable_nitrate,
+    ),
     "ma_s": Variable(
         "mass input to solute mass StorAge of soil",
         CATCH_GRID + AGES,
         "mg",
         "mass input to solute mass StorAge of soil",
         time_dependent=True,
         active=lambda settings: settings.enable_nitrate,
     ),
     "nit_s": Variable(
-        "nitrification of soil nitrogen",
+        "nitrification of mineral soil nitrogen",
+        CATCH_GRID,
+        "mg/dt",
+        "nitrification of mineral soil nitrogen",
+        time_dependent=True,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "min_s": Variable(
+        "mineralization of soil nitrogen",
+        CATCH_GRID,
+        "mg/dt",
+        "mineralization of soil nitrogen",
+        time_dependent=True,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "ndep_s": Variable(
+        "nitrogen deposition",
         CATCH_GRID,
         "mg/dt",
-        "nitrification of soil nitrogen",
+        "nitrogen deposition",
+        time_dependent=True,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "nfix_s": Variable(
+        "nitrogen fixation",
+        CATCH_GRID,
+        "mg/dt",
+        "nitrogen fixation",
         time_dependent=True,
         active=lambda settings: settings.enable_nitrate,
     ),
     "rt10_s": Variable(
         "10th percentile of soil residence time",
         CATCH_GRID,
         "days",
@@ -2491,24 +2579,73 @@
         CATCH_GRID,
         "kg N ha-1 year-1",
         "constant soil nitrogen mineralization rate",
         write_to_restart=True,
         time_dependent=False,
         active=lambda settings: settings.enable_nitrate,
     ),
+    "kngl_rz": Variable(
+        "constant gaseous loss rate of ammonium",
+        CATCH_GRID,
+        "kg N ha-1 year-1",
+        "constant gaseous loss rate of ammonium",
+        write_to_restart=True,
+        time_dependent=False,
+        active=lambda settings: settings.enable_nitrate,
+    ),
     "kfix_rz": Variable(
         "constant nitrogen fixation rate",
         CATCH_GRID,
         "kg N ha-1 year-1",
         "constant nitrogen fixation rate",
         write_to_restart=True,
         time_dependent=False,
         initial=0,
         active=lambda settings: settings.enable_nitrate,
     ),
+    "kdep": Variable(
+        "constant nitrogen deposition rate",
+        CATCH_GRID,
+        "kg N ha-1 year-1",
+        "constant nitrogen deposition rate",
+        write_to_restart=True,
+        time_dependent=False,
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "nup": Variable(
+        "potential nitrogen uptake rate by plants",
+        CATCH_GRID,
+        "kg N ha-1 day-1",
+        "potential nitrogen uptake rate by plants",
+        write_to_restart=True,
+        time_dependent=False,
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "nh4_up": Variable(
+        "nitrogen uptake rate by plants",
+        CATCH_GRID,
+        "mg N day-1",
+        "nitrogen uptake rate by plants",
+        write_to_restart=True,
+        time_dependent=False,
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "c_fert": Variable(
+        "ratio to dissolve mineral nitrogen fertilizer",
+        CATCH_GRID,
+        "-",
+        "ratio to dissolve mineral nitrogen fertilizer",
+        write_to_restart=True,
+        time_dependent=False,
+        initial=0.3,
+        active=lambda settings: settings.enable_nitrate,
+    ),
     "mr_rz": Variable(
         "mass removal from solute mass StorAge of root zone",
         CATCH_GRID + AGES,
         "mg",
         "mass removal from solute mass StorAge of root zone",
         time_dependent=True,
         active=lambda settings: settings.enable_nitrate,
@@ -2865,14 +3002,62 @@
         CATCH_GRID + TIMESTEPS + AGES,
         "mg",
         "inorganic nitrogen in subsoil",
         write_to_restart=True,
         time_dependent=True,
         active=lambda settings: settings.enable_nitrate,
     ),
+    "N_fert1": Variable(
+        "Nitrogen of first mineral fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of first mineral fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "N_fert2": Variable(
+        "Nitrogen of second mineral fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of second mineral fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "N_fert3": Variable(
+        "Nitrogen of third mineral fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of third mineral fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "N_fert1_org": Variable(
+        "Nitrogen of first organic fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of first organic fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "N_fert2_org": Variable(
+        "Nitrogen of second organic fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of second organic fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
+    "N_fert3_org": Variable(
+        "Nitrogen of third organic fertilizer application",
+        CATCH_GRID,
+        "kg N ha-1",
+        "Nitrogen of third organic fertilizer application",
+        initial=0,
+        active=lambda settings: settings.enable_nitrate,
+    ),
     # groundwater parameters
     "S_gw_tot": Variable(
         "total groundwater storage",
         CATCH_GRID,
         "mm",
         "total groundwater storage",
         time_dependent=False,
@@ -5202,14 +5387,23 @@
         "mg",
         "mineral nitrogen fertilizer",
         write_to_restart=True,
         time_dependent=False,
         active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
     ),
     "Nmin_in": Variable(
+        "undissolved mineral nitrogen fertilizer",
+        CATCH_GRID,
+        "mg",
+        "undissolved mineral nitrogen fertilizer",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
+    ),
+    "Nfert_min": Variable(
         "mineral nitrogen fertilizer",
         CATCH_GRID,
         "mg",
         "mineral nitrogen fertilizer",
         write_to_restart=False,
         time_dependent=False,
         active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
@@ -5228,14 +5422,32 @@
         CATCH_GRID,
         "mg",
         "organic nitrogen fertilizer",
         write_to_restart=False,
         time_dependent=False,
         active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
     ),
+    "Nfert_org": Variable(
+        "organic nitrogen fertilizer",
+        CATCH_GRID,
+        "mg",
+        "organic nitrogen fertilizer",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
+    ),
+    "Nfert": Variable(
+        "nitrogen fertilizer",
+        CATCH_GRID,
+        "mg",
+        "nitrogen fertilizer",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_offline_transport & settings.enable_nitrate,
+    ),
     # transport variables
     # film flow parameters
     # film flow variables
     # routing parameters
     "z_stream_tot": Variable(
         "total depth of river",
         RIVER_GRID,
@@ -5825,14 +6037,23 @@
         LUT_FERT_GRID,
         "",
         "Look-up-table of nitrogen fertilization",
         write_to_restart=False,
         time_dependent=False,
         active=lambda settings: settings.enable_crop_phenology & settings.enable_nitrate,
     ),
+    "lut_nup": Variable(
+        "Look-up-table of nitrogen uptake by crops",
+        LUT_NUP_GRID,
+        "",
+        "Look-up-table of nitrogen uptake by crops",
+        write_to_restart=False,
+        time_dependent=False,
+        active=lambda settings: settings.enable_crop_phenology & settings.enable_nitrate,
+    ),
     "dS_num_error": Variable(
         "numerical error of water balance",
         CATCH_GRID,
         "mm",
         "numerical error of water balance",
         write_to_restart=False,
         time_dependent=False,
```

### Comparing `roger-3.0.4/roger.egg-info/PKG-INFO` & `roger-3.0.5/roger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roger
-Version: 3.0.4
+Version: 3.0.5
 Summary: Runoff Generation Research - a process-based hydrological toolbox model in Python
 Home-page: https://roger.readthedocs.io
 Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de
 License: MIT
 Keywords: hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roger Version: 3.0.4 Summary: Runoff Generation
+Metadata-Version: 2.1 Name: roger Version: 3.0.5 Summary: Runoff Generation
 Research - a process-based hydrological toolbox model in Python Home-page:
 https://roger.readthedocs.io Author: Robin Schwemmle (University of Freiburg)
 Author-email: robin.schwemmle@hydrology.uni-freiburg.de License: MIT Keywords:
 hydrology python parallel numpy multi-core geophysics hydrologic-model gpu jax
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

### Comparing `roger-3.0.4/roger.egg-info/SOURCES.txt` & `roger-3.0.5/roger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/setup.py` & `roger-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/cli_test.py` & `roger-3.0.5/test/cli_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/make_data_for_svat_transport.py` & `roger-3.0.5/test/make_data_for_svat_transport.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/progress_test.py` & `roger-3.0.5/test/progress_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/restart_test.py` & `roger-3.0.5/test/restart_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/setup_test.py` & `roger-3.0.5/test/setup_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/test/state_test.py` & `roger-3.0.5/test/state_test.py`

 * *Files identical despite different names*

### Comparing `roger-3.0.4/versioneer.py` & `roger-3.0.5/versioneer.py`

 * *Files identical despite different names*

