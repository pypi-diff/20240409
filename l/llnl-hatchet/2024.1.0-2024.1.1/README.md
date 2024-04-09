# Comparing `tmp/llnl-hatchet-2024.1.0.tar.gz` & `tmp/llnl-hatchet-2024.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llnl-hatchet-2024.1.0.tar", last modified: Mon Mar 11 22:44:21 2024, max compression
+gzip compressed data, was "llnl-hatchet-2024.1.1.tar", last modified: Tue Apr  9 17:41:06 2024, max compression
```

## Comparing `llnl-hatchet-2024.1.0.tar` & `llnl-hatchet-2024.1.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.681796 llnl-hatchet-2024.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-11 22:44:21.681796 llnl-hatchet-2024.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/cython_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/cython_modules/graphframe_modules.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/cython_modules/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/cython_modules/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/cython_modules/reader_modules.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/external/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18750 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.665797 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/roundtrip.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.669797 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.669797 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/data/test.html
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/data/test.js
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/rt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/external/roundtrip/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    66477 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/graphframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.669797 llnl-hatchet-2024.1.0/hatchet/query/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/object_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    57905 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/query/string_dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.669797 llnl-hatchet-2024.1.0/hatchet/readers/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/caliper_native_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17034 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/caliper_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/cprofile_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/dataframe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/gprof_dot_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/hdf5_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16325 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/hpctoolkit_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/literal_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/pyinstrument_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/spotdb_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/tau_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    25695 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/readers/timemory_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.673797 llnl-hatchet-2024.1.0/hatchet/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28344 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/caliper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/callgrind.py
--rw-r--r--   0 runner    (1001) docker     (127)    46526 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/cprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/dataframe_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/graph_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/graph_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    38671 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/graphframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/hpctoolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/pyinstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    49299 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/query_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/spotdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/tau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/timemory_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/tests/timemory_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.673797 llnl-hatchet-2024.1.0/hatchet/util/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/util/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/boxplot.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/
--rw-r--r--   0 runner    (1001) docker     (127)    46419 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_chart_view.js
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_color_manager.js
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_controller.js
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_globals.js
--rw-r--r--   0 runner    (1001) docker     (127)    22694 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_menu_view.js
--rw-r--r--   0 runner    (1001) docker     (127)    23701 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_model.js
--rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_repr.js
--rw-r--r--   0 runner    (1001) docker     (127)    26303 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_scented_slider_popup.js
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_stats.js
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_tooltip_view.js
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/scripts/utils/view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/static/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/static/boxplot_bundle.html
--rw-r--r--   0 runner    (1001) docker     (127)   181961 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/static/boxplot_bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/static/cct_bundle.html
--rw-r--r--   0 runner    (1001) docker     (127)   750167 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/static/cct_bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/static_fixer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/styles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/styles/boxplot.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/styles/cct.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/vis/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/templates/boxplot.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/templates/cct.html
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/vis/webpack.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.677797 llnl-hatchet-2024.1.0/hatchet/writers/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/writers/dataframe_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/hatchet/writers/hdf5_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 22:44:21.681796 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-11 22:44:21.000000 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-11 22:44:21.000000 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 22:44:21.000000 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-11 22:44:21.000000 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 22:44:21.000000 llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 22:44:21.681796 llnl-hatchet-2024.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-11 22:44:13.000000 llnl-hatchet-2024.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.095201 llnl-hatchet-2024.1.1/hatchet/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.095201 llnl-hatchet-2024.1.1/hatchet/cython_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/cython_modules/graphframe_modules.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.095201 llnl-hatchet-2024.1.1/hatchet/cython_modules/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/cython_modules/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/cython_modules/reader_modules.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.095201 llnl-hatchet-2024.1.1/hatchet/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.099201 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.099201 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/roundtrip.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.099201 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.099201 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/data/test.html
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/data/test.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/rt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/external/roundtrip/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66477 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/graphframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.099201 llnl-hatchet-2024.1.1/hatchet/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13050 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/object_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57905 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/query/string_dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.103201 llnl-hatchet-2024.1.1/hatchet/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/caliper_native_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17034 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/caliper_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/cprofile_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/gprof_dot_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/hdf5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16325 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/hpctoolkit_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/literal_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/pyinstrument_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/spotdb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23415 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/tau_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25695 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/readers/timemory_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.103201 llnl-hatchet-2024.1.1/hatchet/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28309 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/caliper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/callgrind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46526 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/cprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/dataframe_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/graph_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/graph_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38671 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/graphframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/hpctoolkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/pyinstrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49299 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/query_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/spotdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/tau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/timemory_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/tests/timemory_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.107201 llnl-hatchet-2024.1.1/hatchet/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/util/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.107201 llnl-hatchet-2024.1.1/hatchet/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.107201 llnl-hatchet-2024.1.1/hatchet/vis/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/boxplot.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.107201 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/
+-rw-r--r--   0 runner    (1001) docker     (127)    46419 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_chart_view.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_color_manager.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_controller.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_globals.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22694 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_menu_view.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23701 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_model.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_repr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26303 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_scented_slider_popup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_stats.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_tooltip_view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.107201 llnl-hatchet-2024.1.1/hatchet/vis/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/scripts/utils/view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/hatchet/vis/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/static/boxplot_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (127)   181961 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/static/boxplot_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/static/cct_bundle.html
+-rw-r--r--   0 runner    (1001) docker     (127)   750167 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/static/cct_bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/static_fixer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/hatchet/vis/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/styles/boxplot.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/styles/cct.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/hatchet/vis/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/templates/boxplot.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/templates/cct.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/vis/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/hatchet/writers/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/writers/dataframe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/hatchet/writers/hdf5_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-09 17:41:06.000000 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-09 17:41:06.000000 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:41:06.000000 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-09 17:41:06.000000 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 17:41:06.000000 llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:41:06.111201 llnl-hatchet-2024.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-09 17:40:58.000000 llnl-hatchet-2024.1.1/setup.py
```

### Comparing `llnl-hatchet-2024.1.0/LICENSE` & `llnl-hatchet-2024.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/NOTICE` & `llnl-hatchet-2024.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/PKG-INFO` & `llnl-hatchet-2024.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llnl-hatchet
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: A Python library for analyzing hierarchical performance data
 Home-page: https://github.com/llnl/hatchet
 Author: Stephanie Brink
 Author-email: brink2@llnl.gov
 License: MIT
 Project-URL: Source Code, https://github.com/llnl/hatchet
 Project-URL: Documentation, https://llnl-hatchet.readthedocs.io/en/latest/
```

### Comparing `llnl-hatchet-2024.1.0/README.md` & `llnl-hatchet-2024.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/cython_modules/graphframe_modules.pyx` & `llnl-hatchet-2024.1.1/hatchet/cython_modules/graphframe_modules.pyx`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/cython_modules/reader_modules.pyx` & `llnl-hatchet-2024.1.1/hatchet/cython_modules/reader_modules.pyx`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/__init__.py` & `llnl-hatchet-2024.1.1/hatchet/external/__init__.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/console.py` & `llnl-hatchet-2024.1.1/hatchet/external/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,18 @@
                         ]
                     metric_str += " [{}".format(color_annotation)
                     metric_str += "{}".format(annotation_content)
                     metric_str += "{}]".format(self.colors_annotations.end)
                 else:
                     metric_str += " [{}]".format(annotation_content)
 
-            node_name = dataframe.loc[df_index, self.name]
+            if isinstance(dataframe.columns, pd.MultiIndex):
+                node_name = dataframe.loc[df_index, (self.name, "")]
+            else:
+                node_name = dataframe.loc[df_index, self.name]
             if self.expand is False:
                 if len(node_name) > 39:
                     node_name = (
                         node_name[:18] + "..." + node_name[(len(node_name) - 18) :]
                     )
             name_str = (
                 self._ansi_color_for_name(node_name) + node_name + self.colors.end
```

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/LICENSE` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/LICENSE`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/README.md` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/README.md`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/package.json` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/package.json`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/pyproject.toml` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/manager.py` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/manager.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/roundtrip.js` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/roundtrip.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/roundtrip/tests/rt_test.py` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/roundtrip/tests/rt_test.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/external/roundtrip/setup.py` & `llnl-hatchet-2024.1.1/hatchet/external/roundtrip/setup.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/frame.py` & `llnl-hatchet-2024.1.1/hatchet/frame.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/graph.py` & `llnl-hatchet-2024.1.1/hatchet/graph.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/graphframe.py` & `llnl-hatchet-2024.1.1/hatchet/graphframe.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/node.py` & `llnl-hatchet-2024.1.1/hatchet/node.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/__init__.py` & `llnl-hatchet-2024.1.1/hatchet/query/__init__.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/compat.py` & `llnl-hatchet-2024.1.1/hatchet/query/compat.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/compound.py` & `llnl-hatchet-2024.1.1/hatchet/query/compound.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/engine.py` & `llnl-hatchet-2024.1.1/hatchet/query/engine.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/errors.py` & `llnl-hatchet-2024.1.1/hatchet/query/errors.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/object_dialect.py` & `llnl-hatchet-2024.1.1/hatchet/query/object_dialect.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/query.py` & `llnl-hatchet-2024.1.1/hatchet/query/query.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/query/string_dialect.py` & `llnl-hatchet-2024.1.1/hatchet/query/string_dialect.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/caliper_native_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/caliper_native_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,17 @@
                     if column in old_to_new:
                         column = old_to_new[column]
                     exc_metrics.append(column)
 
             with self.timer.phase("data frame"):
                 # merge the metrics and node dataframes on the nid column
                 dataframe = pd.merge(df_metrics, self.df_nodes, on="nid")
-                dataframe["nid"] = dataframe["nid"].astype(pd.Int64Dtype())
+                dataframe["nid"] = dataframe["nid"].astype(
+                    self.__cali_type_dict["double"]
+                )
 
                 # set the index to be a MultiIndex
                 indices = ["node"]
                 if "rank" in dataframe.columns:
                     indices.append("rank")
                 dataframe.set_index(indices, inplace=True)
                 dataframe.sort_index(inplace=True)
```

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/caliper_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/caliper_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/cprofile_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/cprofile_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/dataframe_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/gprof_dot_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/gprof_dot_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/hdf5_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/hdf5_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/hpctoolkit_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/hpctoolkit_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/json_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/json_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/literal_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/literal_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/pyinstrument_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/pyinstrument_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/spotdb_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/spotdb_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/tau_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/tau_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/readers/timemory_reader.py` & `llnl-hatchet-2024.1.1/hatchet/readers/timemory_reader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/caliper.py` & `llnl-hatchet-2024.1.1/hatchet/tests/caliper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2017-2023 Lawrence Livermore National Security, LLC and other
 # Hatchet Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: MIT
 
 import subprocess
 import numpy as np
-import pandas as pd
 
 import pytest
 import sys
 
 from hatchet import GraphFrame
 from hatchet.readers.caliper_reader import CaliperReader
 from hatchet.util.executable import which
@@ -192,15 +191,15 @@
     assert len(gf.dataframe.groupby("name")) == 19
     assert "cali.caliper.version" in gf.metadata.keys()
 
     for col in gf.dataframe.columns:
         if col in ("time (inc)", "time"):
             assert gf.dataframe[col].dtype == np.float64
         elif col in ("nid", "rank"):
-            assert gf.dataframe[col].dtype == pd.Int64Dtype()
+            assert gf.dataframe[col].dtype == np.float64
         elif col in ("name", "node"):
             assert gf.dataframe[col].dtype == object
 
     assert type(gf.metadata["cali.channel"]) == str
     assert type(gf.metadata["cali.caliper.version"]) == str
 
 
@@ -218,15 +217,15 @@
     assert "cali.caliper.version" in gf.metadata.keys()
     assert type(gf.metadata["cali.caliper.version"]) == str
 
     for col in gf.dataframe.columns:
         if col in ("time (inc)", "time"):
             assert gf.dataframe[col].dtype == np.float64
         elif col in ("nid", "rank"):
-            assert gf.dataframe[col].dtype == pd.Int64Dtype()
+            assert gf.dataframe[col].dtype == np.float64
         elif col in ("name", "node"):
             assert gf.dataframe[col].dtype == object
 
 
 def test_graphframe_native_lulesh_from_file_node_order(caliper_ordered_cali):
     """Check the order of output from the native Caliper reader by examining a known input with node order column."""
 
@@ -878,15 +877,15 @@
     assert len(gf.dataframe.groupby("name")) == 19
     assert "cali.caliper.version" in gf.metadata.keys()
 
     for col in gf.dataframe.columns:
         if col in ("time (inc)", "time"):
             assert gf.dataframe[col].dtype == np.float64
         elif col in ("nid", "rank"):
-            assert gf.dataframe[col].dtype == pd.Int64Dtype()
+            assert gf.dataframe[col].dtype == np.float64
         elif col in ("name", "node"):
             assert gf.dataframe[col].dtype == object
 
     assert type(gf.metadata["cali.channel"]) == str
     assert type(gf.metadata["cali.caliper.version"]) == str
 
     # check for the expected timeseries and memory allocation columns
```

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/callgrind.py` & `llnl-hatchet-2024.1.1/hatchet/tests/callgrind.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/conftest.py` & `llnl-hatchet-2024.1.1/hatchet/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/cprofile.py` & `llnl-hatchet-2024.1.1/hatchet/tests/cprofile.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/dataframe_ops.py` & `llnl-hatchet-2024.1.1/hatchet/tests/dataframe_ops.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/executable.py` & `llnl-hatchet-2024.1.1/hatchet/tests/executable.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/frame.py` & `llnl-hatchet-2024.1.1/hatchet/tests/frame.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/graph.py` & `llnl-hatchet-2024.1.1/hatchet/tests/graph.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/graph_literal.py` & `llnl-hatchet-2024.1.1/hatchet/tests/graph_literal.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/graph_ops.py` & `llnl-hatchet-2024.1.1/hatchet/tests/graph_ops.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/graphframe.py` & `llnl-hatchet-2024.1.1/hatchet/tests/graphframe.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/hpctoolkit.py` & `llnl-hatchet-2024.1.1/hatchet/tests/hpctoolkit.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/json_test.py` & `llnl-hatchet-2024.1.1/hatchet/tests/json_test.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/node.py` & `llnl-hatchet-2024.1.1/hatchet/tests/node.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/profiler.py` & `llnl-hatchet-2024.1.1/hatchet/tests/profiler.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/pyinstrument.py` & `llnl-hatchet-2024.1.1/hatchet/tests/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/query.py` & `llnl-hatchet-2024.1.1/hatchet/tests/query.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/query_compat.py` & `llnl-hatchet-2024.1.1/hatchet/tests/query_compat.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/spotdb_test.py` & `llnl-hatchet-2024.1.1/hatchet/tests/spotdb_test.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/tau.py` & `llnl-hatchet-2024.1.1/hatchet/tests/tau.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/timemory_func.py` & `llnl-hatchet-2024.1.1/hatchet/tests/timemory_func.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/tests/timemory_test.py` & `llnl-hatchet-2024.1.1/hatchet/tests/timemory_test.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/colormaps.py` & `llnl-hatchet-2024.1.1/hatchet/util/colormaps.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/deprecated.py` & `llnl-hatchet-2024.1.1/hatchet/util/deprecated.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/dot.py` & `llnl-hatchet-2024.1.1/hatchet/util/dot.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/executable.py` & `llnl-hatchet-2024.1.1/hatchet/util/executable.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/profiler.py` & `llnl-hatchet-2024.1.1/hatchet/util/profiler.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/util/timer.py` & `llnl-hatchet-2024.1.1/hatchet/util/timer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/__init__.py` & `llnl-hatchet-2024.1.1/hatchet/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/loader.py` & `llnl-hatchet-2024.1.1/hatchet/vis/loader.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/package.json` & `llnl-hatchet-2024.1.1/hatchet/vis/package.json`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_chart_view.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_chart_view.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_color_manager.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_color_manager.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_controller.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_controller.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_globals.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_globals.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_menu_view.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_menu_view.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_model.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_model.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_repr.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_repr.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_scented_slider_popup.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_scented_slider_popup.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_stats.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_stats.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct/cct_tooltip_view.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct/cct_tooltip_view.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/scripts/cct.js` & `llnl-hatchet-2024.1.1/hatchet/vis/scripts/cct.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/static/boxplot_bundle.js` & `llnl-hatchet-2024.1.1/hatchet/vis/static/boxplot_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/static/cct_bundle.js` & `llnl-hatchet-2024.1.1/hatchet/vis/static/cct_bundle.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/static_fixer.py` & `llnl-hatchet-2024.1.1/hatchet/vis/static_fixer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/vis/webpack.config.js` & `llnl-hatchet-2024.1.1/hatchet/vis/webpack.config.js`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/writers/dataframe_writer.py` & `llnl-hatchet-2024.1.1/hatchet/writers/dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/hatchet/writers/hdf5_writer.py` & `llnl-hatchet-2024.1.1/hatchet/writers/hdf5_writer.py`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/PKG-INFO` & `llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llnl-hatchet
-Version: 2024.1.0
+Version: 2024.1.1
 Summary: A Python library for analyzing hierarchical performance data
 Home-page: https://github.com/llnl/hatchet
 Author: Stephanie Brink
 Author-email: brink2@llnl.gov
 License: MIT
 Project-URL: Source Code, https://github.com/llnl/hatchet
 Project-URL: Documentation, https://llnl-hatchet.readthedocs.io/en/latest/
```

### Comparing `llnl-hatchet-2024.1.0/llnl_hatchet.egg-info/SOURCES.txt` & `llnl-hatchet-2024.1.1/llnl_hatchet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llnl-hatchet-2024.1.0/pyproject.toml` & `llnl-hatchet-2024.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Cython",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "llnl-hatchet"
-version = "2024.1.0"
+version = "2024.1.1"
 description = "A Python library for analyzing hierarchical performance data."
 authors = [
     "Abhinav Bhatele <bhatele@cs.umd.edu>",
     "Stephanie Brink <brink2@llnl.gov>",
     "Todd Gamblin <tgamblin@llnl.gov>",
 ]
 license = "MIT"
```

### Comparing `llnl-hatchet-2024.1.0/setup.py` & `llnl-hatchet-2024.1.1/setup.py`

 * *Files identical despite different names*

