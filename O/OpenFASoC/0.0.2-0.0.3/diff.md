# Comparing `tmp/OpenFASoC-0.0.2.tar.gz` & `tmp/OpenFASoC-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFASoC-0.0.2.tar", last modified: Tue Apr  9 01:48:29 2024, max compression
+gzip compressed data, was "OpenFASoC-0.0.3.tar", last modified: Tue Apr  9 01:53:14 2024, max compression
```

## Comparing `OpenFASoC-0.0.2.tar` & `OpenFASoC-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,82 @@
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/
--rw-r--r--   0 labtob    (1000) labtob    (1000)    11357 2024-04-06 16:10:50.000000 OpenFASoC-0.0.2/LICENSE
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/OpenFASoC.egg-info/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)      741 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/SOURCES.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/dependency_links.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)      130 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/requires.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)       10 2024-04-09 01:48:29.000000 OpenFASoC-0.0.2/OpenFASoC.egg-info/top_level.txt
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/PKG-INFO
--rw-r--r--   0 labtob    (1000) labtob    (1000)     8013 2024-04-06 16:10:50.000000 OpenFASoC-0.0.2/README.rst
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/openfasoc/
--rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:39:12.000000 OpenFASoC-0.0.2/openfasoc/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)      467 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/config.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.425215 OpenFASoC-0.0.2/openfasoc/generators/
--rw-r--r--   0 labtob    (1000) labtob    (1000)      202 2024-04-09 01:47:29.000000 OpenFASoC-0.0.2/openfasoc/generators/__init__.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/openfasoc/generators/common/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1323 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     3369 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/check_gen_files.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)      583 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/get_ngspice_version.py
-drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4203 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/__init__.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1809 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/classify_sim_error.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     6779 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_config.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4289 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_run.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/simulation/utils.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)     4298 2024-04-06 16:10:51.000000 OpenFASoC-0.0.2/openfasoc/generators/common/verilog_generation.py
--rw-r--r--   0 labtob    (1000) labtob    (1000)      399 2024-04-09 01:48:29.426215 OpenFASoC-0.0.2/setup.cfg
--rw-r--r--   0 labtob    (1000) labtob    (1000)     1023 2024-04-09 01:45:32.000000 OpenFASoC-0.0.2/setup.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.250887 OpenFASoC-0.0.3/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11357 2024-04-06 16:10:50.000000 OpenFASoC-0.0.3/LICENSE
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.236888 OpenFASoC-0.0.3/OpenFASoC.egg-info/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:53:14.000000 OpenFASoC-0.0.3/OpenFASoC.egg-info/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3713 2024-04-09 01:53:14.000000 OpenFASoC-0.0.3/OpenFASoC.egg-info/SOURCES.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        1 2024-04-09 01:53:14.000000 OpenFASoC-0.0.3/OpenFASoC.egg-info/dependency_links.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      130 2024-04-09 01:53:14.000000 OpenFASoC-0.0.3/OpenFASoC.egg-info/requires.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       10 2024-04-09 01:53:14.000000 OpenFASoC-0.0.3/OpenFASoC.egg-info/top_level.txt
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8571 2024-04-09 01:53:14.250887 OpenFASoC-0.0.3/PKG-INFO
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8013 2024-04-06 16:10:50.000000 OpenFASoC-0.0.3/README.rst
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.236888 OpenFASoC-0.0.3/openfasoc/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:39:12.000000 OpenFASoC-0.0.3/openfasoc/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      467 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/config.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.236888 OpenFASoC-0.0.3/openfasoc/generators/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      202 2024-04-09 01:47:29.000000 OpenFASoC-0.0.3/openfasoc/generators/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.236888 OpenFASoC-0.0.3/openfasoc/generators/common/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1323 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3369 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/check_gen_files.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      583 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/get_ngspice_version.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.237887 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4203 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1809 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/classify_sim_error.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     6779 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/simulation_config.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4289 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/simulation_run.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/simulation/utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4298 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/common/verilog_generation.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.237887 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:52:23.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.237887 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       18 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.245888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10577 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/diff_pair.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     7074 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/diff_pair_cmirrorbias.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10713 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/diff_pair_stackedcmirror.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    12982 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/differential_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    10212 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/opamp.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15844 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/opamp_twostage.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4912 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/row_csamplifier_diff_to_single_ended_converter.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     3129 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/components/stacked_current_mirror.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.245888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/__init__.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.245888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/gf180_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      150 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/gf180_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1316 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/gf180_mapped/gf180_mapped.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13625 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/gf180_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14510 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/mappedpdk.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.246888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      155 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    13642 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/grules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2781 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/sky130_add_npc.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1303 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/sky130_mapped/sky130_mapped.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.247887 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    12926 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/comp_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2350 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/component_array_create.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    15988 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/port_utils.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5190 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/print_rules.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      480 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/pdk/util/snap_to_grid.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.247887 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/placement/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/placement/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     8520 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/placement/two_transistor_interdigitized.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     2241 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/placement/two_transistor_place.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.248888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    28362 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/fet.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5503 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/guardring.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     5182 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/mimcap.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    14335 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/primitives/via_gen.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.249888 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/routing/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4469 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/routing/L_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)        0 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/routing/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     9611 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/routing/c_route.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     4488 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/routing/straight_route.py
+drwxr-xr-x   0 labtob    (1000) labtob    (1000)        0 2024-04-09 01:53:14.250887 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/spice/
+-rw-r--r--   0 labtob    (1000) labtob    (1000)       28 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/spice/__init__.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    11224 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/glayout/spice/netlist.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     9380 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/process_input.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)    37211 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/relational.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1630 2024-04-06 16:10:51.000000 OpenFASoC-0.0.3/openfasoc/generators/gdsfactory-gen/run.py
+-rw-r--r--   0 labtob    (1000) labtob    (1000)      399 2024-04-09 01:53:14.250887 OpenFASoC-0.0.3/setup.cfg
+-rw-r--r--   0 labtob    (1000) labtob    (1000)     1023 2024-04-09 01:52:57.000000 OpenFASoC-0.0.3/setup.py
```

### Comparing `OpenFASoC-0.0.2/LICENSE` & `OpenFASoC-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/OpenFASoC.egg-info/PKG-INFO` & `OpenFASoC-0.0.3/OpenFASoC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFASoC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenFASoC-0.0.2/PKG-INFO` & `OpenFASoC-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFASoC
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits
 Home-page: https://github.com/idea-fasoc/OpenFASOC
 Author:  msaligane
 Author-email: mehdi@umich.edu
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OpenFASoC-0.0.2/README.rst` & `OpenFASoC-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/__init__.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/check_gen_files.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/check_gen_files.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/get_ngspice_version.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/get_ngspice_version.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/simulation/__init__.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/simulation/classify_sim_error.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/simulation/classify_sim_error.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_config.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/simulation/simulation_config.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/simulation/simulation_run.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/simulation/simulation_run.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/simulation/utils.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/openfasoc/generators/common/verilog_generation.py` & `OpenFASoC-0.0.3/openfasoc/generators/common/verilog_generation.py`

 * *Files identical despite different names*

### Comparing `OpenFASoC-0.0.2/setup.py` & `OpenFASoC-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def get_install_requires():
     with open("requirements.txt", "r") as f:
         return [line.strip() for line in f.readlines() if not line.startswith("-")]
 
 
 setup(
     name="OpenFASoC",
-    version="0.0.2",
+    version="0.0.3",
     url="https://github.com/idea-fasoc/OpenFASOC",
     license="MIT",
     author=" msaligane",
     author_email="mehdi@umich.edu",
     description="Fully Open-Source Autonomous SoC Synthesis using Customizable Cell-Based Synthesizable Analog Circuits",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
```

