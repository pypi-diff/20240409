# Comparing `tmp/FLORIS-3.6.tar.gz` & `tmp/FLORIS-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLORIS-3.6.tar", last modified: Fri Apr  5 20:18:15 2024, max compression
+gzip compressed data, was "FLORIS-4.tar", last modified: Tue Apr  9 20:24:44 2024, max compression
```

## Comparing `FLORIS-3.6.tar` & `FLORIS-4.tar`

### file list

```diff
@@ -1,121 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/FLORIS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 20:18:15.000000 FLORIS-3.6/FLORIS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-05 20:18:03.000000 FLORIS-3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-05 20:18:15.529142 FLORIS-3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6831 2024-04-05 20:18:03.000000 FLORIS-3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.501142 FLORIS-3.6/floris/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21042 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/farm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17324 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/floris.py
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/flow_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    37599 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    66932 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    27618 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)    20506 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/turbine_multi_dim.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_combination/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/fls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_combination/sosfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_deflection/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)    17510 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/jimenez.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_deflection/none.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.505142 FLORIS-3.6/floris/simulation/wake_turbulence/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_turbulence/wake_induced_mixing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.509142 FLORIS-3.6/floris/simulation/wake_velocity/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/cumulative_gauss_curl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/empirical_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/jensen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/turbopark.py
--rw-r--r--   0 runner    (1001) docker     (127)  9163212 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/simulation/wake_velocity/turbopark_lookup_table.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/cut_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)    48328 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/floris_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/floris_interface_legacy_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/interface_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/layout_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/layout_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.521142 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13345 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/pyoptsparse/yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.525142 FLORIS-3.6/floris/tools/optimization/legacy/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/base_COE.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/cluster_turbines.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16134 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/layout_height.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    18216 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/power_density_1D.py
--rw-r--r--   0 runner    (1001) docker     (127)    30497 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw.py
--rw-r--r--   0 runner    (1001) docker     (127)    14451 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_clustered.py
--rw-r--r--   0 runner    (1001) docker     (127)    46052 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
--rw-r--r--   0 runner    (1001) docker     (127)    22003 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
--rw-r--r--   0 runner    (1001) docker     (127)    26829 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    30232 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.525142 FLORIS-3.6/floris/tools/optimization/other/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/other/boundary_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/floris/tools/optimization/yaw_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34644 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13707 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
--rw-r--r--   0 runner    (1001) docker     (127)    24167 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/parallel_computing_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18526 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/power_rose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/rews.py
--rw-r--r--   0 runner    (1001) docker     (127)    30208 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/uncertainty_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    61719 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/tools/wind_rose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 20:18:15.529142 FLORIS-3.6/floris/turbine_library/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_10MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/nrel_5MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34777 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/turbine_previewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/turbine_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/turbine_library/x_20MW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/type_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-05 20:18:03.000000 FLORIS-3.6/floris/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-05 20:18:03.000000 FLORIS-3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 20:18:15.533142 FLORIS-3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-05 20:18:03.000000 FLORIS-3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.785059 FLORIS-4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/FLORIS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:24:44.000000 FLORIS-4/FLORIS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-09 20:24:34.000000 FLORIS-4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 20:24:44.785059 FLORIS-4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-09 20:24:34.000000 FLORIS-4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.761059 FLORIS-4/floris/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-09 20:24:34.000000 FLORIS-4/floris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-09 20:24:34.000000 FLORIS-4/floris/convert_floris_input_v3_to_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-09 20:24:34.000000 FLORIS-4/floris/convert_turbine_v3_to_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/farm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/flow_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35084 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/rotor_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62372 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/turbine/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/operation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28768 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/turbine/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_combination/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/fls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_combination/sosfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_deflection/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/jimenez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_deflection/none.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.765059 FLORIS-4/floris/core/wake_turbulence/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_turbulence/wake_induced_mixing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.769059 FLORIS-4/floris/core/wake_velocity/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/cumulative_gauss_curl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/turbopark.py
+-rw-r--r--   0 runner    (1001) docker     (127)  9163212 2024-04-09 20:24:34.000000 FLORIS-4/floris/core/wake_velocity/turbopark_lookup_table.mat
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-09 20:24:34.000000 FLORIS-4/floris/cut_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71608 2024-04-09 20:24:34.000000 FLORIS-4/floris/floris_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29230 2024-04-09 20:24:34.000000 FLORIS-4/floris/flow_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21418 2024-04-09 20:24:34.000000 FLORIS-4/floris/layout_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-09 20:24:34.000000 FLORIS-4/floris/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.777059 FLORIS-4/floris/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/layout_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/layout_optimization/layout_optimization_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/other/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/other/boundary_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/optimization/yaw_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28535 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-09 20:24:34.000000 FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22700 2024-04-09 20:24:34.000000 FLORIS-4/floris/parallel_floris_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:24:44.781059 FLORIS-4/floris/turbine_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_10MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW_floating_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/iea_15MW_multi_dim_cp_ct.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/nrel_5MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34909 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/turbine_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-09 20:24:34.000000 FLORIS-4/floris/turbine_library/turbine_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-09 20:24:34.000000 FLORIS-4/floris/type_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36981 2024-04-09 20:24:34.000000 FLORIS-4/floris/uncertain_floris_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-04-09 20:24:34.000000 FLORIS-4/floris/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-09 20:24:34.000000 FLORIS-4/floris/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104097 2024-04-09 20:24:34.000000 FLORIS-4/floris/wind_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-09 20:24:34.000000 FLORIS-4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:24:44.785059 FLORIS-4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-09 20:24:34.000000 FLORIS-4/setup.py
```

### Comparing `FLORIS-3.6/FLORIS.egg-info/PKG-INFO` & `FLORIS-4/FLORIS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.6
+Version: 4
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -22,21 +21,20 @@
 Requires-Dist: numexpr~=2.0
 Requires-Dist: numpy~=1.20
 Requires-Dist: scipy~=1.1
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: pandas~=2.0
 Requires-Dist: shapely~=2.0
 Requires-Dist: coloredlogs~=10.0
-Requires-Dist: flatten_dict~=0.0
 Provides-Extra: docs
-Requires-Dist: jupyter-book; extra == "docs"
-Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Provides-Extra: develop
+Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
-Requires-Dist: pre-commit; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-3.6/PKG-INFO` & `FLORIS-4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.6
+Version: 4
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -22,21 +21,20 @@
 Requires-Dist: numexpr~=2.0
 Requires-Dist: numpy~=1.20
 Requires-Dist: scipy~=1.1
 Requires-Dist: matplotlib~=3.0
 Requires-Dist: pandas~=2.0
 Requires-Dist: shapely~=2.0
 Requires-Dist: coloredlogs~=10.0
-Requires-Dist: flatten_dict~=0.0
 Provides-Extra: docs
-Requires-Dist: jupyter-book; extra == "docs"
-Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinxcontrib-autoyaml; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: jupyter-book; extra == "docs"
 Requires-Dist: sphinxcontrib.mermaid; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Provides-Extra: develop
+Requires-Dist: pre-commit; extra == "develop"
 Requires-Dist: pytest; extra == "develop"
 Requires-Dist: isort; extra == "develop"
 Requires-Dist: ruff; extra == "develop"
-Requires-Dist: pre-commit; extra == "develop"
 
 A controls-oriented engineering wake model.
```

### Comparing `FLORIS-3.6/floris/logging_manager.py` & `FLORIS-4/floris/logging_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 import logging
 from datetime import datetime
 
 import coloredlogs
```

### Comparing `FLORIS-3.6/floris/simulation/farm.py` & `FLORIS-4/floris/core/farm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,49 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from __future__ import annotations
 
 import copy
+from collections.abc import Callable
 from pathlib import Path
 from typing import (
     Any,
     Dict,
     List,
 )
 
 import attrs
 import numpy as np
 from attrs import define, field
 from scipy.interpolate import interp1d
 
-from floris.simulation import (
+from floris.core import (
     BaseClass,
     State,
     Turbine,
-    TurbineMultiDimensional,
 )
-from floris.simulation.turbine import compute_tilt_angles_for_floating_turbines
+from floris.core.rotor_velocity import compute_tilt_angles_for_floating_turbines_map
+from floris.core.turbine.operation_models import POWER_SETPOINT_DEFAULT
 from floris.type_dec import (
     convert_to_path,
     floris_array_converter,
     iter_validator,
     NDArrayFloat,
     NDArrayObject,
+    NDArrayStr,
 )
 from floris.utilities import load_yaml
 
 
 default_turbine_library_path = Path(__file__).parents[1] / "turbine_library"
 
 
 @define
 class Farm(BaseClass):
     """Farm is where wind power plants should be instantiated from a YAML configuration
-    file. The Farm will create a heterogenous set of turbines that compose a wind farm,
+    file. The Farm will create a heterogeneous set of turbines that compose a wind farm,
     validate the inputs, and then create a vectorized representation of the the turbine
     data.
 
     Farm is the container class of the FLORIS package. It brings
     together all of the component objects after input (i.e., Turbine,
     Wake, FlowField) and packages everything into the appropriate data
     type. Farm should also be used as an entry point to probe objects
@@ -77,53 +68,56 @@
     turbine_type: List = field(validator=iter_validator(list, (dict, str)))
     turbine_library_path: Path = field(
         default=default_turbine_library_path, converter=convert_to_path
     )
 
     turbine_definitions: list = field(init=False, validator=iter_validator(list, dict))
 
-    turbine_fCts: Dict[str, interp1d] | List[interp1d] = field(init=False, factory=list)
-    turbine_fCts_sorted: NDArrayFloat = field(init=False, factory=list)
+    turbine_thrust_coefficient_functions: Dict[str, Callable] = field(init=False, factory=list)
+    turbine_axial_induction_functions: Dict[str, Callable] = field(init=False, factory=list)
 
     turbine_tilt_interps: dict[str, interp1d] = field(init=False, factory=dict)
 
     yaw_angles: NDArrayFloat = field(init=False)
     yaw_angles_sorted: NDArrayFloat = field(init=False)
 
     tilt_angles: NDArrayFloat = field(init=False)
     tilt_angles_sorted: NDArrayFloat = field(init=False)
 
+    power_setpoints: NDArrayFloat = field(init=False)
+    power_setpoints_sorted: NDArrayFloat = field(init=False)
+
+    awc_modes: NDArrayStr = field(init=False)
+    awc_modes_sorted: NDArrayStr = field(init=False)
+
+    awc_amplitudes: NDArrayFloat = field(init=False)
+    awc_amplitudes_sorted: NDArrayFloat = field(init=False)
+
+    awc_frequencies: NDArrayFloat = field(init=False)
+    awc_frequencies_sorted: NDArrayFloat = field(init=False)
+
     hub_heights: NDArrayFloat = field(init=False)
     hub_heights_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    turbine_map: List[Turbine | TurbineMultiDimensional] = field(init=False, factory=list)
+    turbine_map: List[Turbine] = field(init=False, factory=list)
 
     turbine_type_map: NDArrayObject = field(init=False, factory=list)
     turbine_type_map_sorted: NDArrayObject = field(init=False, factory=list)
 
-    turbine_power_interps: Dict[str, interp1d] | List[interp1d] = field(init=False, factory=list)
-    turbine_power_interps_sorted: NDArrayFloat = field(init=False, factory=list)
+    turbine_power_functions: Dict[str, Callable] = field(init=False, factory=list)
+    turbine_power_thrust_tables: Dict[str, dict] = field(init=False, factory=list)
 
     rotor_diameters: NDArrayFloat = field(init=False, factory=list)
     rotor_diameters_sorted: NDArrayFloat = field(init=False, factory=list)
 
     TSRs: NDArrayFloat = field(init=False, factory=list)
     TSRs_sorted: NDArrayFloat = field(init=False, factory=list)
 
-    pPs: NDArrayFloat = field(init=False, factory=list)
-    pPs_sorted: NDArrayFloat = field(init=False, factory=list)
-
-    pTs: NDArrayFloat = field(init=False, factory=list)
-    pTs_sorted: NDArrayFloat = field(init=False, factory=list)
-
-    ref_density_cp_cts: NDArrayFloat = field(init=False, factory=list)
-    ref_density_cp_cts_sorted: NDArrayFloat = field(init=False, factory=list)
-
-    ref_tilt_cp_cts: NDArrayFloat = field(init=False, factory=list)
-    ref_tilt_cp_cts_sorted: NDArrayFloat = field(init=False, factory=list)
+    ref_tilts: NDArrayFloat = field(init=False, factory=list)
+    ref_tilts_sorted: NDArrayFloat = field(init=False, factory=list)
 
     correct_cp_ct_for_tilt: NDArrayFloat = field(init=False, factory=list)
     correct_cp_ct_for_tilt_sorted: NDArrayFloat = field(init=False, factory=list)
 
     internal_turbine_library: Path = field(init=False, default=default_turbine_library_path)
 
     def __attrs_post_init__(self) -> None:
@@ -196,14 +190,18 @@
         ]
 
         # If 1 turbine definition is given, expand to N turbines; this covers a 1-turbine
         # farm and 1 definition for multiple turbines
         if len(_turbine_types) == 1:
             _turbine_types *= self.n_turbines
 
+        # Check that turbine definitions contain any v3 keys
+        for t in _turbine_types:
+            check_turbine_definition_for_v3_keys(turbine_definition_cache[t])
+
         # Map each turbine definition to its index in this list
         self.turbine_definitions = [
             copy.deepcopy(turbine_definition_cache[t]) for t in _turbine_types
         ]
 
     @layout_x.validator
     def check_x(self, attribute: attrs.Attribute, value: Any) -> None:
@@ -217,290 +215,251 @@
 
     @turbine_type.validator
     def check_turbine_type(self, attribute: attrs.Attribute, value: Any) -> None:
         # Check that the list of turbines is either of length 1 or N turbines
         if len(value) != 1 and len(value) != self.n_turbines:
             raise ValueError(
                 "turbine_type must have the same number of entries as layout_x/layout_y or have "
-                "a single turbine_type value."
+                "a single turbine_type value. This error can arise if you set the turbine_type or "
+                "alter the operation model before setting the layout."
             )
 
     @turbine_library_path.validator
     def check_library_path(self, attribute: attrs.Attribute, value: Path) -> None:
         """Ensures that the input to `library_path` exists and is a directory."""
         if not value.is_dir():
             raise FileExistsError(f"The input file path: {str(value)} is not a valid directory.")
 
     def initialize(self, sorted_indices):
         # Sort yaw angles from most upstream to most downstream wind turbine
         self.yaw_angles_sorted = np.take_along_axis(
             self.yaw_angles,
-            sorted_indices[:, :, :, 0, 0],
-            axis=2,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
         )
         self.tilt_angles_sorted = np.take_along_axis(
             self.tilt_angles,
-            sorted_indices[:, :, :, 0, 0],
-            axis=2,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
+        )
+        self.power_setpoints_sorted = np.take_along_axis(
+            self.power_setpoints,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
+        )
+        self.awc_modes_sorted = np.take_along_axis(
+            self.awc_modes,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
+        )
+        self.awc_amplitudes_sorted = np.take_along_axis(
+            self.awc_amplitudes,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
+        )
+        self.awc_frequencies_sorted = np.take_along_axis(
+            self.awc_frequencies,
+            sorted_indices[:, :, 0, 0],
+            axis=1,
         )
         self.state = State.INITIALIZED
 
     def construct_hub_heights(self):
         self.hub_heights = np.array([turb['hub_height'] for turb in self.turbine_definitions])
 
     def construct_rotor_diameters(self):
         self.rotor_diameters = np.array([
             turb['rotor_diameter'] for turb in self.turbine_definitions
         ])
 
     def construct_turbine_TSRs(self):
         self.TSRs = np.array([turb['TSR'] for turb in self.turbine_definitions])
 
-    def construct_turbine_pPs(self):
-        self.pPs = np.array([turb['pP'] for turb in self.turbine_definitions])
-
-    def construct_turbine_pTs(self):
-        self.pTs = np.array([turb['pT'] for turb in self.turbine_definitions])
-
-    def construct_turbine_ref_density_cp_cts(self):
-        self.ref_density_cp_cts = np.array([
-            turb['ref_density_cp_ct'] for turb in self.turbine_definitions
-        ])
-
-    def construct_turbine_ref_tilt_cp_cts(self):
-        self.ref_tilt_cp_cts = np.array(
-            [turb['ref_tilt_cp_ct'] for turb in self.turbine_definitions]
+    def construct_turbine_ref_tilts(self):
+        self.ref_tilts = np.array(
+            [turb['power_thrust_table']['ref_tilt'] for turb in self.turbine_definitions]
         )
 
     def construct_turbine_correct_cp_ct_for_tilt(self):
         self.correct_cp_ct_for_tilt = np.array(
             [turb.correct_cp_ct_for_tilt for turb in self.turbine_map]
         )
 
     def construct_turbine_map(self):
-        multi_key = "multi_dimensional_cp_ct"
-        if multi_key in self.turbine_definitions[0] and self.turbine_definitions[0][multi_key]:
-            self.turbine_map = []
-            for turb in self.turbine_definitions:
-                _turb = {**turb, **{"turbine_library_path": self.internal_turbine_library}}
-                try:
-                    self.turbine_map.append(TurbineMultiDimensional.from_dict(_turb))
-                except FileNotFoundError:
-                    _turb["turbine_library_path"] = self.turbine_library_path
-                    self.turbine_map.append(TurbineMultiDimensional.from_dict(_turb))
-        else:
-            self.turbine_map = [Turbine.from_dict(turb) for turb in self.turbine_definitions]
-
-    def construct_turbine_fCts(self):
-        self.turbine_fCts = {
-            turb.turbine_type: turb.fCt_interp for turb in self.turbine_map
+        self.turbine_map = [Turbine.from_dict(turb) for turb in self.turbine_definitions]
+
+    def construct_turbine_thrust_coefficient_functions(self):
+        self.turbine_thrust_coefficient_functions = {
+            turb.turbine_type: turb.thrust_coefficient_function for turb in self.turbine_map
         }
 
-    def construct_multidim_turbine_fCts(self):
-        self.turbine_fCts = [turb.fCt_interp for turb in self.turbine_map]
+    def construct_turbine_axial_induction_functions(self):
+        self.turbine_axial_induction_functions = {
+            turb.turbine_type: turb.axial_induction_function for turb in self.turbine_map
+        }
 
     def construct_turbine_tilt_interps(self):
         self.turbine_tilt_interps = {
             turb.turbine_type: turb.tilt_interp for turb in self.turbine_map
         }
 
-    def construct_turbine_power_interps(self):
-        self.turbine_power_interps = {
-            turb.turbine_type: turb.power_interp for turb in self.turbine_map
+    def construct_turbine_power_functions(self):
+        self.turbine_power_functions = {
+            turb.turbine_type: turb.power_function for turb in self.turbine_map
         }
 
-    def construct_multidim_turbine_power_interps(self):
-        self.turbine_power_interps = [turb.power_interp for turb in self.turbine_map]
+    def construct_turbine_power_thrust_tables(self):
+        self.turbine_power_thrust_tables = {
+            turb.turbine_type: turb.power_thrust_table for turb in self.turbine_map
+        }
 
-    def expand_farm_properties(
-        self,
-        n_wind_directions: int,
-        n_wind_speeds: int,
-        sorted_coord_indices
-    ):
+    def expand_farm_properties(self, n_findex: int, sorted_coord_indices):
         template_shape = np.ones_like(sorted_coord_indices)
         self.hub_heights_sorted = np.take_along_axis(
             self.hub_heights * template_shape,
             sorted_coord_indices,
-            axis=2
+            axis=1
         )
-        if 'multi_dimensional_cp_ct' in self.turbine_definitions[0].keys() \
-            and self.turbine_definitions[0]['multi_dimensional_cp_ct'] is True:
-            wd_dim = np.shape(template_shape)[0]
-            ws_dim = np.shape(template_shape)[1]
-            if wd_dim != 1 | ws_dim != 0:
-                self.turbine_fCts_sorted = np.take_along_axis(
-                    np.reshape(
-                        np.repeat(self.turbine_fCts, wd_dim * ws_dim),
-                        np.shape(template_shape)
-                    ),
-                    sorted_coord_indices,
-                    axis=2
-                )
-                self.turbine_power_interps_sorted = np.take_along_axis(
-                    np.reshape(
-                        np.repeat(self.turbine_power_interps, wd_dim * ws_dim),
-                        np.shape(template_shape)
-                    ),
-                    sorted_coord_indices,
-                    axis=2
-                )
-            else:
-                self.turbine_fCts_sorted = np.take_along_axis(
-                    np.reshape(self.turbine_fCts, np.shape(template_shape)),
-                    sorted_coord_indices,
-                    axis=2
-                )
-                self.turbine_power_interps_sorted = np.take_along_axis(
-                    np.reshape(self.turbine_power_interps, np.shape(template_shape)),
-                    sorted_coord_indices,
-                    axis=2
-                )
         self.rotor_diameters_sorted = np.take_along_axis(
             self.rotor_diameters * template_shape,
             sorted_coord_indices,
-            axis=2
+            axis=1
         )
         self.TSRs_sorted = np.take_along_axis(
             self.TSRs * template_shape,
             sorted_coord_indices,
-            axis=2
-        )
-        self.ref_density_cp_cts_sorted = np.take_along_axis(
-            self.ref_density_cp_cts * template_shape,
-            sorted_coord_indices,
-            axis=2
+            axis=1
         )
-        self.ref_tilt_cp_cts_sorted = np.take_along_axis(
-            self.ref_tilt_cp_cts * template_shape,
+        self.ref_tilts_sorted = np.take_along_axis(
+            self.ref_tilts * template_shape,
             sorted_coord_indices,
-            axis=2
+            axis=1
         )
         self.correct_cp_ct_for_tilt_sorted = np.take_along_axis(
             self.correct_cp_ct_for_tilt * template_shape,
             sorted_coord_indices,
-            axis=2
-        )
-        self.pPs_sorted = np.take_along_axis(
-            self.pPs * template_shape,
-            sorted_coord_indices,
-            axis=2
-        )
-        self.pTs_sorted = np.take_along_axis(
-            self.pTs * template_shape,
-            sorted_coord_indices,
-            axis=2
+            axis=1
         )
 
         # NOTE: Tilt angles are sorted twice - here and in initialize()
         self.tilt_angles_sorted = np.take_along_axis(
             self.tilt_angles * template_shape,
             sorted_coord_indices,
-            axis=2
+            axis=1
         )
         self.turbine_type_map_sorted = np.take_along_axis(
             np.reshape(
-                [turb["turbine_type"] for turb in self.turbine_definitions] * n_wind_directions,
+                [turb["turbine_type"] for turb in self.turbine_definitions] * n_findex,
                 np.shape(sorted_coord_indices)
             ),
             sorted_coord_indices,
-            axis=2
+            axis=1
         )
 
-    def set_yaw_angles(self, n_wind_directions: int, n_wind_speeds: int):
-        # TODO Is this just for initializing yaw angles to zero?
-        self.yaw_angles = np.zeros((n_wind_directions, n_wind_speeds, self.n_turbines))
-        self.yaw_angles_sorted = np.zeros((n_wind_directions, n_wind_speeds, self.n_turbines))
+    def set_yaw_angles(self, yaw_angles: NDArrayFloat | list[float]):
+        self.yaw_angles = np.array(yaw_angles)
+
+    def set_yaw_angles_to_ref_yaw(self, n_findex: int):
+        yaw_angles = np.zeros((n_findex, self.n_turbines))
+        self.set_yaw_angles(yaw_angles)
+        self.yaw_angles_sorted = np.zeros((n_findex, self.n_turbines))
 
-    def set_tilt_to_ref_tilt(self, n_wind_directions: int, n_wind_speeds: int):
+    def set_tilt_to_ref_tilt(self, n_findex: int):
         self.tilt_angles = (
-            np.ones((n_wind_directions, n_wind_speeds, self.n_turbines))
-            * self.ref_tilt_cp_cts
+            np.ones((n_findex, self.n_turbines))
+            * self.ref_tilts
         )
         self.tilt_angles_sorted = (
-            np.ones((n_wind_directions, n_wind_speeds, self.n_turbines))
-            * self.ref_tilt_cp_cts
+            np.ones((n_findex, self.n_turbines))
+            * self.ref_tilts
         )
 
+    def set_power_setpoints(self, power_setpoints: NDArrayFloat):
+        self.power_setpoints = np.array(power_setpoints)
+
+    def set_power_setpoints_to_ref_power(self, n_findex: int):
+        power_setpoints = POWER_SETPOINT_DEFAULT * np.ones((n_findex, self.n_turbines))
+        self.set_power_setpoints(power_setpoints)
+        self.power_setpoints_sorted = POWER_SETPOINT_DEFAULT * np.ones((n_findex, self.n_turbines))
+
+    def set_awc_modes(self, awc_modes: NDArrayStr):
+        self.awc_modes = np.array(awc_modes)
+
+    def set_awc_modes_to_ref_mode(self, n_findex: int):
+        # awc_modes = np.empty((n_findex, self.n_turbines))\
+        awc_modes = np.array([["baseline"]*self.n_turbines]*n_findex)
+        self.set_awc_modes(awc_modes)
+        # self.awc_modes_sorted = np.empty((n_findex, self.n_turbines))
+        self.awc_modes_sorted = np.array([["baseline"]*self.n_turbines]*n_findex)
+
+    def set_awc_amplitudes(self, awc_amplitudes: NDArrayFloat):
+        self.awc_amplitudes = np.array(awc_amplitudes)
+
+    def set_awc_amplitudes_to_ref_amp(self, n_findex: int):
+        awc_amplitudes = np.zeros((n_findex, self.n_turbines))
+        self.set_awc_amplitudes(awc_amplitudes)
+        self.awc_amplitudes_sorted = np.zeros((n_findex, self.n_turbines))
+
+    def set_awc_frequencies(self, awc_frequencies: NDArrayFloat):
+        self.awc_frequencies = np.array(awc_frequencies)
+
+    def set_awc_frequencies_to_ref_freq(self, n_findex: int):
+        awc_frequencies = np.zeros((n_findex, self.n_turbines))
+        self.set_awc_frequencies(awc_frequencies)
+        self.awc_frequencies_sorted = np.zeros((n_findex, self.n_turbines))
+
     def calculate_tilt_for_eff_velocities(self, rotor_effective_velocities):
-        tilt_angles = compute_tilt_angles_for_floating_turbines(
+        tilt_angles = compute_tilt_angles_for_floating_turbines_map(
             self.turbine_type_map_sorted,
             self.tilt_angles_sorted,
             self.turbine_tilt_interps,
             rotor_effective_velocities,
         )
         return tilt_angles
 
     def finalize(self, unsorted_indices):
-        if 'multi_dimensional_cp_ct' in self.turbine_definitions[0].keys() \
-            and self.turbine_definitions[0]['multi_dimensional_cp_ct'] is True:
-            self.turbine_fCts = np.take_along_axis(
-                self.turbine_fCts_sorted,
-                unsorted_indices[:,:,:,0,0],
-                axis=2
-            )
-            self.turbine_power_interps = np.take_along_axis(
-                self.turbine_power_interps_sorted,
-                unsorted_indices[:,:,:,0,0],
-                axis=2
-            )
         self.yaw_angles = np.take_along_axis(
             self.yaw_angles_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.tilt_angles = np.take_along_axis(
             self.tilt_angles_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.hub_heights = np.take_along_axis(
             self.hub_heights_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.rotor_diameters = np.take_along_axis(
             self.rotor_diameters_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.TSRs = np.take_along_axis(
             self.TSRs_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
-        self.ref_density_cp_cts = np.take_along_axis(
-            self.ref_density_cp_cts_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
-        )
-        self.ref_tilt_cp_cts = np.take_along_axis(
-            self.ref_tilt_cp_cts_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+        self.ref_tilts = np.take_along_axis(
+            self.ref_tilts_sorted,
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.correct_cp_ct_for_tilt = np.take_along_axis(
             self.correct_cp_ct_for_tilt_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
-        )
-        self.pPs = np.take_along_axis(
-            self.pPs_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
-        )
-        self.pTs = np.take_along_axis(
-            self.pTs_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.turbine_type_map = np.take_along_axis(
             self.turbine_type_map_sorted,
-            unsorted_indices[:,:,:,0,0],
-            axis=2
+            unsorted_indices[:,:,0,0],
+            axis=1
         )
         self.state.USED
 
     @property
     def coordinates(self):
         return np.array([
             np.array([x, y, z]) for x, y, z in zip(
@@ -509,7 +468,42 @@
                 self.hub_heights if len(self.hub_heights.shape) == 1 else self.hub_heights[0,0]
             )
         ])
 
     @property
     def n_turbines(self):
         return len(self.layout_x)
+
+def check_turbine_definition_for_v3_keys(turbine_definition: dict):
+    """Check that the turbine definition does not contain any v3 keys."""
+    v3_deprecation_msg = (
+        "Consider using the convert_turbine_v3_to_v4.py utility in floris/tools "
+        + "to convert from a FLORIS v3 turbine definition to FLORIS v4. "
+        + "See https://nrel.github.io/floris/v3_to_v4.html for more information."
+    )
+    if "generator_efficiency" in turbine_definition:
+        raise ValueError(
+            "generator_efficiency is no longer supported as power is specified in absolute terms "
+            + "in FLORIS v4. "
+            + v3_deprecation_msg
+        )
+
+    v3_renamed_keys = ["pP", "pT", "ref_density_cp_ct", "ref_tilt_cp_ct"]
+    if any(k in turbine_definition for k in v3_renamed_keys):
+        v3_list_keys = ", ".join(map(str,v3_renamed_keys[:-1]))+", and "+v3_renamed_keys[-1]
+        v4_versions = (
+            "cosine_loss_exponent_yaw, cosine_loss_exponent_tilt, ref_air_density, and ref_tilt"
+        )
+        raise ValueError(
+            v3_list_keys
+            + " have been renamed to "
+            + v4_versions
+            + ", respectively, and placed under the power_thrust_table field in FLORIS v4. "
+            + v3_deprecation_msg
+        )
+
+    if "thrust" in turbine_definition["power_thrust_table"]:
+        raise ValueError(
+            "thrust has been renamed thrust_coefficient in FLORIS v4 (and power is now specified "
+            "in absolute terms with units kW, rather than as a coefficient). "
+            + v3_deprecation_msg
+        )
```

### Comparing `FLORIS-3.6/floris/simulation/floris.py` & `FLORIS-4/floris/core/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import yaml
 from attrs import define, field
 
 from floris import logging_manager
-from floris.simulation import (
+from floris.core import (
     BaseClass,
     cc_solver,
     empirical_gauss_solver,
     Farm,
     FlowField,
     FlowFieldGrid,
     FlowFieldPlanarGrid,
     full_flow_cc_solver,
     full_flow_empirical_gauss_solver,
     full_flow_sequential_solver,
     full_flow_turbopark_solver,
     Grid,
     PointsGrid,
-    sequential_multidim_solver,
     sequential_solver,
     State,
     TurbineCubatureGrid,
     TurbineGrid,
     turbopark_solver,
     WakeModelManager,
 )
@@ -48,15 +34,15 @@
 from floris.utilities import (
     load_yaml,
     reverse_rotate_coordinates_rel_west,
 )
 
 
 @define
-class Floris(BaseClass):
+class Core(BaseClass):
     """
     Top-level class that describes a Floris model and initializes the
     simulation. Use the :py:class:`~.simulation.farm.Farm` attribute to
     access other objects within the model.
     """
 
     logging: dict = field(converter=dict)
@@ -81,130 +67,78 @@
             self.logging["console"]["level"],
         )
         logging_manager.configure_file_log(
             self.logging["file"]["enable"],
             self.logging["file"]["level"],
         )
 
-        self.check_deprecated_inputs()
-
         # Initialize farm quantities that depend on other objects
         self.farm.construct_turbine_map()
-        if self.wake.model_strings['velocity_model'] == 'multidim_cp_ct':
-            self.farm.construct_multidim_turbine_fCts()
-            self.farm.construct_multidim_turbine_power_interps()
-        else:
-            self.farm.construct_turbine_fCts()
-            self.farm.construct_turbine_power_interps()
+        self.farm.construct_turbine_thrust_coefficient_functions()
+        self.farm.construct_turbine_axial_induction_functions()
+        self.farm.construct_turbine_power_functions()
+        self.farm.construct_turbine_power_thrust_tables()
         self.farm.construct_hub_heights()
         self.farm.construct_rotor_diameters()
         self.farm.construct_turbine_TSRs()
-        self.farm.construct_turbine_pPs()
-        self.farm.construct_turbine_pTs()
-        self.farm.construct_turbine_ref_density_cp_cts()
-        self.farm.construct_turbine_ref_tilt_cp_cts()
+        self.farm.construct_turbine_ref_tilts()
         self.farm.construct_turbine_tilt_interps()
         self.farm.construct_turbine_correct_cp_ct_for_tilt()
-        self.farm.set_yaw_angles(self.flow_field.n_wind_directions, self.flow_field.n_wind_speeds)
-        self.farm.set_tilt_to_ref_tilt(
-            self.flow_field.n_wind_directions,
-            self.flow_field.n_wind_speeds,
-        )
+        self.farm.set_yaw_angles_to_ref_yaw(self.flow_field.n_findex)
+        self.farm.set_tilt_to_ref_tilt(self.flow_field.n_findex)
+        self.farm.set_power_setpoints_to_ref_power(self.flow_field.n_findex)
+        self.farm.set_awc_modes_to_ref_mode(self.flow_field.n_findex)
+        self.farm.set_awc_amplitudes_to_ref_amp(self.flow_field.n_findex)
+        self.farm.set_awc_frequencies_to_ref_freq(self.flow_field.n_findex)
 
         if self.solver["type"] == "turbine_grid":
             self.grid = TurbineGrid(
                 turbine_coordinates=self.farm.coordinates,
                 turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
-                wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["turbine_grid_points"],
-                time_series=self.flow_field.time_series,
             )
         elif self.solver["type"] == "turbine_cubature_grid":
             self.grid = TurbineCubatureGrid(
                 turbine_coordinates=self.farm.coordinates,
                 turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
-                wind_speeds=self.flow_field.wind_speeds,
-                time_series=self.flow_field.time_series,
                 grid_resolution=self.solver["turbine_grid_points"],
             )
         elif self.solver["type"] == "flow_field_grid":
             self.grid = FlowFieldGrid(
                 turbine_coordinates=self.farm.coordinates,
                 turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
-                wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["flow_field_grid_points"],
-                time_series=self.flow_field.time_series,
             )
         elif self.solver["type"] == "flow_field_planar_grid":
             self.grid = FlowFieldPlanarGrid(
                 turbine_coordinates=self.farm.coordinates,
                 turbine_diameters=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
-                wind_speeds=self.flow_field.wind_speeds,
                 normal_vector=self.solver["normal_vector"],
                 planar_coordinate=self.solver["planar_coordinate"],
                 grid_resolution=self.solver["flow_field_grid_points"],
-                time_series=self.flow_field.time_series,
                 x1_bounds=self.solver["flow_field_bounds"][0],
                 x2_bounds=self.solver["flow_field_bounds"][1],
             )
         else:
             raise ValueError(
                 "Supported solver types are "
                 "[turbine_grid, turbine_cubature_grid, flow_field_grid, flow_field_planar_grid], "
                 f"but type given was {self.solver['type']}"
             )
 
         if isinstance(self.grid, (TurbineGrid, TurbineCubatureGrid)):
             self.farm.expand_farm_properties(
-                self.flow_field.n_wind_directions,
-                self.flow_field.n_wind_speeds,
+                self.flow_field.n_findex,
                 self.grid.sorted_coord_indices
             )
 
-    def check_deprecated_inputs(self):
-        """
-        This function should used when the FLORIS input file changes in order to provide
-        an informative error and suggest a fix.
-        """
-
-        error_messages = []
-        # Check for missing values add in version 3.2 and 3.4
-        for turbine in self.farm.turbine_definitions:
-
-            if "ref_density_cp_ct" not in turbine.keys():
-                error_messages.append(
-                    "From FLORIS v3.2, the turbine definition must include 'ref_density_cp_ct'. "
-                    "This value represents the air density at which the provided Cp and Ct "
-                    "curves are defined. Previously, this was assumed to be 1.225 kg/m^3, "
-                    "and other air density values applied were assumed to be a deviation "
-                    "from the defined level. FLORIS now requires the user to explicitly "
-                    "define the reference density. Add 'ref_density_cp_ct' to your "
-                    "turbine definition and try again. For a description of the turbine inputs, "
-                    "see https://nrel.github.io/floris/input_reference_turbine.html."
-                )
-
-            if "ref_tilt_cp_ct" not in turbine.keys():
-                error_messages.append(
-                    "From FLORIS v3.4, the turbine definition must include 'ref_tilt_cp_ct'. "
-                    "This value represents the tilt angle at which the provided Cp and Ct "
-                    "curves are defined. Add 'ref_tilt_cp_ct' to your turbine definition and "
-                    "try again. For a description of the turbine inputs, "
-                    "see https://nrel.github.io/floris/input_reference_turbine.html."
-                )
-
-            if len(error_messages) > 0:
-                raise ValueError(
-                    f"{turbine['turbine_type']} turbine model\n" +
-                    "\n\n".join(error_messages)
-                )
-
     def initialize_domain(self):
         """Initialize solution space prior to wake calculations"""
 
         # Initialize field quantities; doing this immediately prior to doing
         # the calculation step allows for manipulating inputs in a script
         # without changing the data structures
         self.flow_field.initialize_velocity_field(self.grid)
@@ -220,16 +154,27 @@
 
         vel_model = self.wake.model_strings["velocity_model"]
 
         if vel_model in ["gauss", "cc", "turbopark", "jensen"] and \
             self.farm.correct_cp_ct_for_tilt.any():
             self.logger.warning(
                 "The current model does not account for vertical wake deflection due to " +
-                "tilt. Corrections to Cp and Ct can be included, but no vertical wake " +
-                "deflection will occur."
+                "tilt. Corrections to power and thrust coefficient can be included, but no " +
+                "vertical wake deflection will occur."
+            )
+
+        operation_model_awc = False
+        for td in self.farm.turbine_definitions:
+            if "operation_model" in td and td["operation_model"] == "awc":
+                operation_model_awc = True
+        if vel_model != "empirical_gauss" and operation_model_awc:
+            self.logger.warning(
+                f"The current model `{vel_model}` does not account for additional wake mixing " +
+                "due to active wake control. Corrections to power and thrust coefficient can " +
+                "be included, but no enhanced wake recovery will occur."
             )
 
         if vel_model=="cc":
             cc_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
@@ -245,21 +190,14 @@
         elif vel_model=="empirical_gauss":
             empirical_gauss_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
-        elif vel_model=="multidim_cp_ct":
-            sequential_multidim_solver(
-                self.farm,
-                self.flow_field,
-                self.grid,
-                self.wake
-            )
         else:
             sequential_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
@@ -297,17 +235,15 @@
         field_grid = PointsGrid(
             points_x=x,
             points_y=y,
             points_z=z,
             turbine_coordinates=self.farm.coordinates,
             turbine_diameters=self.farm.rotor_diameters,
             wind_directions=self.flow_field.wind_directions,
-            wind_speeds=self.flow_field.wind_speeds,
             grid_resolution=1,
-            time_series=self.flow_field.time_series,
             x_center_of_rotation=self.grid.x_center_of_rotation,
             y_center_of_rotation=self.grid.y_center_of_rotation
         )
 
         self.flow_field.initialize_velocity_field(field_grid)
 
         vel_model = self.wake.model_strings["velocity_model"]
@@ -318,15 +254,15 @@
                 "gauss, jensen, and empirical_guass models."
             )
         elif vel_model == "empirical_gauss":
             full_flow_empirical_gauss_solver(self.farm, self.flow_field, field_grid, self.wake)
         else:
             full_flow_sequential_solver(self.farm, self.flow_field, field_grid, self.wake)
 
-        return self.flow_field.u_sorted[:,:,:,0,0] # Remove turbine grid dimensions
+        return self.flow_field.u_sorted[:,:,0,0] # Remove turbine grid dimensions
 
     def solve_for_velocity_deficit_profiles(
         self,
         direction: str,
         downstream_dists: NDArrayFloat | list,
         profile_range: NDArrayFloat | list,
         resolution: int,
@@ -334,15 +270,15 @@
         ref_rotor_diameter: float,
         x_start: float,
         y_start: float,
         reference_height: float,
     ) -> list[pd.DataFrame]:
         """
         Extract velocity deficit profiles. See
-        :py:meth:`~floris.tools.floris_interface.FlorisInterface.sample_velocity_deficit_profiles`
+        :py:meth:`~floris.floris_model.FlorisModel.sample_velocity_deficit_profiles`
         for more details.
         """
 
         # Create a grid that contains coordinates for all the sample points in all profiles.
         # Effectively, this is a grid of parallel lines.
         n_lines = len(downstream_dists)
 
@@ -374,15 +310,15 @@
             y_center_of_rotation=0.0,
         )
         x = np.squeeze(x, axis=0) + x_start
         y = np.squeeze(y, axis=0) + y_start
         z = np.squeeze(z, axis=0) + reference_height
 
         u = self.solve_for_points(x.flatten(), y.flatten(), z.flatten())
-        u = np.reshape(u[0, 0, :], (n_lines, resolution))
+        u = np.reshape(u[0, :], (n_lines, resolution))
         velocity_deficit = (homogeneous_wind_speed - u) / homogeneous_wind_speed
 
         velocity_deficit_profiles = []
 
         for i in range(n_lines):
             df = pd.DataFrame(
                 {
@@ -405,33 +341,67 @@
         self.flow_field.finalize(self.grid.unsorted_indices)
         self.farm.finalize(self.grid.unsorted_indices)
         self.state = State.USED
 
     ## I/O
 
     @classmethod
-    def from_file(cls, input_file_path: str | Path) -> Floris:
+    def from_file(cls, input_file_path: str | Path) -> Core:
         """Creates a `Floris` instance from an input file. Must be filetype YAML.
 
         Args:
             input_file_path (str): The relative or absolute file path and name to the
                 input file.
 
         Returns:
             Floris: The class object instance.
         """
         input_dict = load_yaml(Path(input_file_path).resolve())
-        return Floris.from_dict(input_dict)
+        check_input_file_for_v3_keys(input_dict)
+        return Core.from_dict(input_dict)
 
     def to_file(self, output_file_path: str) -> None:
         """Converts the `Floris` object to an input-ready YAML file at `output_file_path`.
 
         Args:
             output_file_path (str): The full path and filename for where to save the file.
         """
         with open(output_file_path, "w+") as f:
             yaml.dump(
                 self.as_dict(),
                 f,
                 sort_keys=False,
                 default_flow_style=False
             )
+
+def check_input_file_for_v3_keys(input_dict) -> None:
+    """
+    Checks if any FLORIS v3 keys are present in the input file and raises special errors if
+    the extra keys belong to a v3 definition of the input_dct.
+    and raises special errors if the extra arguments belong to a v3 definition of the class.
+
+    Args:
+        input_dict (dict): The input dictionary to be checked for v3 keys.
+    """
+    v3_deprecation_msg = (
+        "Consider using the convert_floris_input_v3_to_v4.py utility in floris/tools "
+        + "to convert from a FLORIS v3 input file to FLORIS v4. "
+        "See https://nrel.github.io/floris/upgrade_guides/v3_to_v4.html for more information."
+    )
+    if "turbulence_intensity" in input_dict["flow_field"]:
+        raise AttributeError(
+            "turbulence_intensity has been updated to turbulence_intensities in FLORIS v4. "
+            + v3_deprecation_msg
+        )
+    elif not hasattr(input_dict["flow_field"]["turbulence_intensities"], "__len__"):
+        raise AttributeError(
+            "turbulence_intensities must be a list of floats in FLORIS v4. "
+            + v3_deprecation_msg
+        )
+
+    if input_dict["wake"]["model_strings"]["velocity_model"] == "multidim_cp_ct":
+        raise AttributeError(
+            "Dedicated 'multidim_cp_ct' velocity model has been removed in FLORIS v4 in favor of "
+            + "supporting all available wake models. To recover previous operation, set "
+            + "velocity_model to gauss. "
+            + v3_deprecation_msg
+        )
```

### Comparing `FLORIS-3.6/floris/simulation/flow_field.py` & `FLORIS-4/floris/core/flow_field.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,19 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import attrs
 import matplotlib.path as mpltPath
 import numpy as np
 from attrs import define, field
 from scipy.interpolate import LinearNDInterpolator
 from scipy.spatial import ConvexHull
 from shapely.geometry import Polygon
 
-from floris.simulation import (
+from floris.core import (
     BaseClass,
     Grid,
 )
 from floris.type_dec import (
     floris_array_converter,
     NDArrayFloat,
 )
@@ -35,23 +22,20 @@
 @define
 class FlowField(BaseClass):
     wind_speeds: NDArrayFloat = field(converter=floris_array_converter)
     wind_directions: NDArrayFloat = field(converter=floris_array_converter)
     wind_veer: float = field(converter=float)
     wind_shear: float = field(converter=float)
     air_density: float = field(converter=float)
-    turbulence_intensity: float = field(converter=float)
+    turbulence_intensities: NDArrayFloat = field(converter=floris_array_converter)
     reference_wind_height: float = field(converter=float)
-    time_series: bool = field(default=False)
-    heterogenous_inflow_config: dict = field(default=None)
+    heterogeneous_inflow_config: dict = field(default=None)
     multidim_conditions: dict = field(default=None)
 
-    n_wind_speeds: int = field(init=False)
-    n_wind_directions: int = field(init=False)
-
+    n_findex: int = field(init=False)
     u_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     v_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     w_initial_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     u_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     v_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     w_sorted: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
     u: NDArrayFloat = field(init=False, factory=lambda: np.array([]))
@@ -64,62 +48,93 @@
     turbulence_intensity_field_sorted: NDArrayFloat = field(
         init=False, factory=lambda: np.array([])
     )
     turbulence_intensity_field_sorted_avg: NDArrayFloat = field(
         init=False, factory=lambda: np.array([])
     )
 
-    @wind_speeds.validator
-    def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_speeds` attribute up to date."""
-        if self.time_series:
-            self.n_wind_speeds = 1
-        else:
-            self.n_wind_speeds = value.size
+    @turbulence_intensities.validator
+    def turbulence_intensities_validator(
+        self, instance: attrs.Attribute, value: NDArrayFloat
+    ) -> None:
+
+        # Check that the array is 1-dimensional
+        if value.ndim != 1:
+            raise ValueError(
+                "turbulence_intensities must have 1-dimension"
+            )
+
+        # Check the turbulence intensity is length n_findex
+        if len(value) != self.n_findex:
+            raise ValueError("turbulence_intensities must be length n_findex")
+
+
 
     @wind_directions.validator
     def wind_directions_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_directions` attribute up to date."""
-        self.n_wind_directions = value.size
+        # Check that the array is 1-dimensional
+        if self.wind_directions.ndim != 1:
+            raise ValueError(
+                "wind_directions must have 1-dimension"
+            )
+
+        """Using the validator method to keep the `n_findex` attribute up to date."""
+        self.n_findex = value.size
+
+    @wind_speeds.validator
+    def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
+
+        # Check that the array is 1-dimensional
+        if self.wind_speeds.ndim != 1:
+            raise ValueError(
+                "wind_speeds must have 1-dimension"
+            )
+
+        """Confirm wind speeds and wind directions have the same length"""
+        if len(self.wind_directions) != len(self.wind_speeds):
+            raise ValueError(
+                f"wind_directions (length = {len(self.wind_directions)}) and "
+                f"wind_speeds (length = {len(self.wind_speeds)}) must have the same length"
+            )
 
-    @heterogenous_inflow_config.validator
-    def heterogenous_config_validator(self, instance: attrs.Attribute, value: dict | None) -> None:
-        """Using the validator method to check that the heterogenous_inflow_config dictionary has
+    @heterogeneous_inflow_config.validator
+    def heterogeneous_config_validator(self, instance: attrs.Attribute, value: dict | None) -> None:
+        """Using the validator method to check that the heterogeneous_inflow_config dictionary has
         the correct key-value pairs.
         """
         if value is None:
             return
 
-        # Check that the correct keys are supplied for the heterogenous_inflow_config dict
+        # Check that the correct keys are supplied for the heterogeneous_inflow_config dict
         for k in ["speed_multipliers", "x", "y"]:
             if k not in value.keys():
                 raise ValueError(
-                    "heterogenous_inflow_config must contain entries for 'speed_multipliers',"
+                    "heterogeneous_inflow_config must contain entries for 'speed_multipliers',"
                     f"'x', and 'y', with 'z' optional. Missing '{k}'."
                 )
         if "z" not in value:
             # If only a 2D case, add "None" for the z locations
             value["z"] = None
 
     @het_map.validator
     def het_map_validator(self, instance: attrs.Attribute, value: list | None) -> None:
         """Using this validator to make sure that the het_map has an interpolant defined for
-        each wind direction.
+        each findex.
         """
         if value is None:
             return
 
-        if self.n_wind_directions!= np.array(value).shape[0]:
+        if self.n_findex != np.array(value).shape[0]:
             raise ValueError(
-                "The het_map's wind direction dimension not equal to number of wind directions."
+                "The het_map's first dimension not equal to the FLORIS first dimension."
             )
 
 
     def __attrs_post_init__(self) -> None:
-        if self.heterogenous_inflow_config is not None:
+        if self.heterogeneous_inflow_config is not None:
             self.generate_heterogeneous_wind_map()
 
 
     def initialize_velocity_field(self, grid: Grid) -> None:
 
         # Create an initial wind profile as a function of height. The values here will
         # be multiplied with the wind speeds to give the initial wind field.
@@ -145,16 +160,16 @@
         if self.het_map is None:
             speed_ups = 1.0
 
         # If heterogeneous flow data is given, the speed ups at the defined
         # grid locations are determined in either 2 or 3 dimensions.
         else:
             bounds = np.array(list(zip(
-                self.heterogenous_inflow_config['x'],
-                self.heterogenous_inflow_config['y']
+                self.heterogeneous_inflow_config['x'],
+                self.heterogeneous_inflow_config['y']
             )))
             hull = ConvexHull(bounds)
             polygon = Polygon(bounds[hull.vertices])
             path = mpltPath.Path(polygon.boundary.coords)
             points = np.column_stack(
                 (
                     grid.x_sorted_inertial_frame.flatten(),
@@ -187,68 +202,51 @@
 
         # Create the sheer-law wind profile
         # This array is of shape (# wind directions, # wind speeds, grid.template_array)
         # Since generally grid.template_array may be many different shapes, we use transposes
         # here to do broadcasting from left to right (transposed), and then transpose back.
         # The result is an array the wind speed and wind direction dimensions on the left side
         # of the shape and the grid.template array on the right
-        if self.time_series:
-            self.u_initial_sorted = (
-                (self.wind_speeds[:].T * wind_profile_plane.T).T
-                * speed_ups
-            )
-            self.dudz_initial_sorted = (
-                (self.wind_speeds[:].T * dwind_profile_plane.T).T
-                * speed_ups
-            )
-        else:
-            self.u_initial_sorted = (
-                (self.wind_speeds[None, :].T * wind_profile_plane.T).T
-                * speed_ups
-            )
-            self.dudz_initial_sorted = (
-                (self.wind_speeds[None, :].T * dwind_profile_plane.T).T
-                * speed_ups
-            )
+        self.u_initial_sorted = (self.wind_speeds.T * wind_profile_plane.T).T * speed_ups
+        self.dudz_initial_sorted = (self.wind_speeds.T * dwind_profile_plane.T).T * speed_ups
+
         self.v_initial_sorted = np.zeros(
             np.shape(self.u_initial_sorted),
             dtype=self.u_initial_sorted.dtype
         )
         self.w_initial_sorted = np.zeros(
             np.shape(self.u_initial_sorted),
             dtype=self.u_initial_sorted.dtype
         )
 
         self.u_sorted = self.u_initial_sorted.copy()
         self.v_sorted = self.v_initial_sorted.copy()
         self.w_sorted = self.w_initial_sorted.copy()
 
-        self.turbulence_intensity_field = self.turbulence_intensity * np.ones(
-            (
-                self.n_wind_directions,
-                self.n_wind_speeds,
-                grid.n_turbines,
-                1,
-                1,
-            )
+        self.turbulence_intensity_field = self.turbulence_intensities[:, None, None, None]
+        self.turbulence_intensity_field = np.repeat(
+            self.turbulence_intensity_field,
+            grid.n_turbines,
+            axis=1
         )
+
         self.turbulence_intensity_field_sorted = self.turbulence_intensity_field.copy()
 
     def finalize(self, unsorted_indices):
-        self.u = np.take_along_axis(self.u_sorted, unsorted_indices, axis=2)
-        self.v = np.take_along_axis(self.v_sorted, unsorted_indices, axis=2)
-        self.w = np.take_along_axis(self.w_sorted, unsorted_indices, axis=2)
+        self.u = np.take_along_axis(self.u_sorted, unsorted_indices, axis=1)
+        self.v = np.take_along_axis(self.v_sorted, unsorted_indices, axis=1)
+        self.w = np.take_along_axis(self.w_sorted, unsorted_indices, axis=1)
 
         self.turbulence_intensity_field = np.mean(
             np.take_along_axis(
                 self.turbulence_intensity_field_sorted,
                 unsorted_indices,
-                axis=2
+                axis=1
             ),
-            axis=(3,4)
+            axis=(2,3)
         )
 
     def calculate_speed_ups(self, het_map, x, y, z=None):
         if z is not None:
             # Calculate the 3-dimensional speed ups; squeeze is needed as the generator
             # adds an extra dimension
             speed_ups = np.squeeze(
@@ -270,27 +268,27 @@
         """This function creates the heterogeneous interpolant used to calculate heterogeneous
         inflows. The interpolant is for computing wind speed based on an x and y location in the
         flow field. This is computed using SciPy's LinearNDInterpolator and uses a fill value
         equal to the freestream for interpolated values outside of the user-defined heterogeneous
         map bounds.
 
         Args:
-            heterogenous_inflow_config (dict): The heterogeneous inflow configuration dictionary.
+            heterogeneous_inflow_config (dict): The heterogeneous inflow configuration dictionary.
             The configuration should have the following inputs specified.
                 - **speed_multipliers** (list): A list of speed up factors that will multiply
                     the specified freestream wind speed. This 2-dimensional array should have an
                     array of multiplicative factors defined for each wind direction.
                 - **x** (list): A list of x locations at which the speed up factors are defined.
                 - **y**: A list of y locations at which the speed up factors are defined.
                 - **z** (optional): A list of z locations at which the speed up factors are defined.
         """
-        speed_multipliers = self.heterogenous_inflow_config['speed_multipliers']
-        x = self.heterogenous_inflow_config['x']
-        y = self.heterogenous_inflow_config['y']
-        z = self.heterogenous_inflow_config['z']
+        speed_multipliers = self.heterogeneous_inflow_config['speed_multipliers']
+        x = self.heterogeneous_inflow_config['x']
+        y = self.heterogeneous_inflow_config['y']
+        z = self.heterogeneous_inflow_config['z']
 
         if z is not None:
             # Compute the 3-dimensional interpolants for each wind direction
             # Linear interpolation is used for points within the user-defined area of values,
             # while the freestream wind speed is used for points outside that region
             in_region = [
                 LinearNDInterpolator(list(zip(x, y, z)), multiplier, fill_value=1.0)
```

### Comparing `FLORIS-3.6/floris/simulation/grid.py` & `FLORIS-4/floris/core/grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,18 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Iterable
 
 import attrs
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import BaseClass
+from floris.core import BaseClass
 from floris.type_dec import (
     floris_array_converter,
     floris_float_type,
     NDArrayFloat,
     NDArrayInt,
 )
 from floris.utilities import (
@@ -55,30 +41,24 @@
     all of these arrays are the same size
 
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
             arrays with shape (N coordinates, 3).
         turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
         grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Grid resolution with values
             specific to each grid type.
     """
     turbine_coordinates: NDArrayFloat = field(converter=floris_array_converter)
     turbine_diameters: NDArrayFloat = field(converter=floris_array_converter)
     wind_directions: NDArrayFloat = field(converter=floris_array_converter)
-    wind_speeds: NDArrayFloat = field(converter=floris_array_converter)
-    time_series: bool = field()
     grid_resolution: int | Iterable = field()
 
     n_turbines: int = field(init=False)
-    n_wind_speeds: int = field(init=False)
-    n_wind_directions: int = field(init=False)
+    n_findex: int = field(init=False)
     x_sorted: NDArrayFloat = field(init=False)
     y_sorted: NDArrayFloat = field(init=False)
     z_sorted: NDArrayFloat = field(init=False)
     x_sorted_inertial_frame: NDArrayFloat = field(init=False)
     y_sorted_inertial_frame: NDArrayFloat = field(init=False)
     z_sorted_inertial_frame: NDArrayFloat = field(init=False)
     cubature_weights: NDArrayFloat = field(init=False, default=None)
@@ -94,26 +74,18 @@
             raise TypeError(
                 "'turbine_coordinates' must be `np.array` objects "
                 "with three components of type `float`."
             )
 
         self.n_turbines = len(value)
 
-    @wind_speeds.validator
-    def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_speeds` attribute up to date."""
-        if self.time_series:
-            self.n_wind_speeds = 1
-        else:
-            self.n_wind_speeds = value.size
-
     @wind_directions.validator
     def wind_directions_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_directions` attribute up to date."""
-        self.n_wind_directions = value.size
+        """Using the validator method to keep the `n_findex` attribute up to date."""
+        self.n_findex = value.size
 
     @grid_resolution.validator
     def grid_resolution_validator(self, instance: attrs.Attribute, value: int | Iterable) -> None:
         # TODO move this to the grid types and off of the base class
         """Check that grid resolution is given as appropriate for the chosen Grid-type."""
         if isinstance(value, int) and \
             isinstance(self, (TurbineGrid, TurbineCubatureGrid, PointsGrid)):
@@ -137,17 +109,14 @@
     """See `Grid` for more details.
 
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
             arrays with shape (N coordinates, 3).
         turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
         grid_resolution (:py:obj:`int`): The number of points in each
             direction of the square grid on the rotor plane. For example, grid_resolution=3
             creates a 3x3 grid within the rotor swept area.
     """
     # TODO: describe these and the differences between `sorted_indices` and `sorted_coord_indices`
     sorted_indices: NDArrayInt = field(init=False)
     sorted_coord_indices: NDArrayInt = field(init=False)
@@ -224,16 +193,15 @@
         #         Defaults to 0.5.
 
         # Create the data for the turbine grids
         radius_ratio = 0.5
         disc_area_radius = radius_ratio * self.turbine_diameters / 2
         template_grid = np.ones(
             (
-                self.n_wind_directions,
-                self.n_wind_speeds,
+                self.n_findex,
                 self.n_turbines,
                 self.grid_resolution,
                 self.grid_resolution,
             ),
             dtype=floris_float_type
         )
         # Calculate the radial distance from the center of the turbine rotor.
@@ -248,38 +216,38 @@
                 disc_area_radius,
                 self.grid_resolution,
                 dtype=floris_float_type,
                 axis=1
             )
         # Construct the turbine grids
         # Here, they are already rotated to the correct orientation for each wind direction
-        _x = x[:, :, :, None, None] * template_grid
+        _x = x[:, :, None, None] * template_grid
 
         ones_grid = np.ones(
             (self.n_turbines, self.grid_resolution, self.grid_resolution),
             dtype=floris_float_type
         )
-        _y = y[:, :, :, None, None] + template_grid * ( disc_grid[None, None, :, :, None])
-        _z = z[:, :, :, None, None] + template_grid * ( disc_grid[:, None, :] * ones_grid )
+        _y = y[:, :, None, None] + template_grid * ( disc_grid[None, :, :, None])
+        _z = z[:, :, None, None] + template_grid * ( disc_grid[:, None, :] * ones_grid )
 
         # Sort the turbines at each wind direction
 
         # Get the sorted indices for the x coordinates. These are the indices
         # to sort the turbines from upstream to downstream for all wind directions.
         # Also, store the indices to sort them back for when the calculation finishes.
-        self.sorted_indices = _x.argsort(axis=2)
-        self.sorted_coord_indices = x.argsort(axis=2)
-        self.unsorted_indices = self.sorted_indices.argsort(axis=2)
+        self.sorted_indices = _x.argsort(axis=1)
+        self.sorted_coord_indices = x.argsort(axis=1)
+        self.unsorted_indices = self.sorted_indices.argsort(axis=1)
 
         # Put the turbine coordinates into the final arrays in their sorted order
         # These are the coordinates that should be used within the internal calculations
         # such as the wake models and the solvers.
-        self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=2)
-        self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=2)
-        self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=2)
+        self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=1)
+        self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=1)
+        self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=1)
 
         # Now calculate grid coordinates in original frame (from 270 deg perspective)
         self.x_sorted_inertial_frame, self.y_sorted_inertial_frame, self.z_sorted_inertial_frame = \
             reverse_rotate_coordinates_rel_west(
                 wind_directions=self.wind_directions,
                 grid_x=self.x_sorted,
                 grid_y=self.y_sorted,
@@ -298,17 +266,14 @@
     a more accurate average velocity, thrust coefficient, and axial induction.
 
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
             arrays with shape (N coordinates, 3).
         turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
         grid_resolution (:py:obj:`int`): The number of points to
             include in the cubature method. This value must be in the range [1, 10], and the
             corresponding cubature weights are set automatically.
     """
     sorted_indices: NDArrayInt = field(init=False)
     sorted_coord_indices: NDArrayInt = field(init=False)
     unsorted_indices: NDArrayInt = field(init=False)
@@ -341,16 +306,15 @@
             * cubature_coefficients["B"] / np.pi
         )
 
         # Here, the coordinates are already rotated to the correct orientation for each
         # wind direction
         template_grid = np.ones(
             (
-                self.n_wind_directions,
-                self.n_wind_speeds,
+                self.n_findex,
                 self.n_turbines,
                 len(yv),  # Number of coordinates
                 1,
             ),
             dtype=floris_float_type
         )
         _x = x[:, :, :, None, None] * template_grid
@@ -368,21 +332,21 @@
         self.sorted_indices = _x.argsort(axis=2)
         self.sorted_coord_indices = x.argsort(axis=2)
         self.unsorted_indices = self.sorted_indices.argsort(axis=2)
 
         # Put the turbine coordinates into the final arrays in their sorted order
         # These are the coordinates that should be used within the internal calculations
         # such as the wake models and the solvers.
-        self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=2)
-        self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=2)
-        self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=2)
-
-        self.x = np.take_along_axis(self.x_sorted, self.unsorted_indices, axis=2)
-        self.y = np.take_along_axis(self.y_sorted, self.unsorted_indices, axis=2)
-        self.z = np.take_along_axis(self.z_sorted, self.unsorted_indices, axis=2)
+        self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=1)
+        self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=1)
+        self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=1)
+
+        self.x = np.take_along_axis(self.x_sorted, self.unsorted_indices, axis=1)
+        self.y = np.take_along_axis(self.y_sorted, self.unsorted_indices, axis=1)
+        self.z = np.take_along_axis(self.z_sorted, self.unsorted_indices, axis=1)
 
     @classmethod
     def get_cubature_coefficients(cls, N: int):
         """
         Retrieve cubature integration coefficients. This is a class-method, and therefore
         the coefficients can be accessed without creating an instance of the class.
 
@@ -463,17 +427,14 @@
 class FlowFieldGrid(Grid):
     """
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
             arrays with shape (N coordinates, 3).
         turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
         grid_resolution (:py:obj:`Iterable(int,)`): The number of grid points to create in each
             planar direction. Must be 3 components for resolution in the x, y, and z directions.
     """
     x_center_of_rotation: NDArrayFloat = field(init=False)
     y_center_of_rotation: NDArrayFloat = field(init=False)
 
     def __attrs_post_init__(self) -> None:
@@ -535,17 +496,14 @@
 class FlowFieldPlanarGrid(Grid):
     """
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): The arrays of turbine coordinates as Numpy
             arrays with shape (N coordinates, 3).
         turbine_diameters (:py:obj:`NDArrayFloat`): The rotor diameters of each turbine.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): Flag to indicate whether the supplied wind data is a time
-            series.
         grid_resolution (:py:obj:`Iterable(int,)`): The number of grid points to create in each
             planar direction. Must be 2 components for resolution in the x and y directions.
             The z direction is set to 3 planes at -10.0, 0.0, and +10.0 relative to the
             `planar_coordinate`.
     """
     normal_vector: str = field()
     planar_coordinate: float = field()
@@ -593,17 +551,17 @@
                     float(self.planar_coordinate) - 10.0,
                     float(self.planar_coordinate),
                     float(self.planar_coordinate) + 10.0
                 ]),
                 indexing="ij"
             )
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
+            self.x_sorted = x_points[None, :, :, :]
+            self.y_sorted = y_points[None, :, :, :]
+            self.z_sorted = z_points[None, :, :, :]
 
         elif self.normal_vector == "x":  # Rules of thumb for cross plane
             if self.x1_bounds is None:
                 self.x1_bounds = (np.min(y) - 2 * max_diameter, np.max(y) + 2 * max_diameter)
 
             if self.x2_bounds is None:
                 self.x2_bounds = (0.001, 6 * np.max(z))
@@ -611,17 +569,17 @@
             x_points, y_points, z_points = np.meshgrid(
                 np.array([float(self.planar_coordinate)]),
                 np.linspace(self.x1_bounds[0], self.x1_bounds[1], int(self.grid_resolution[0])),
                 np.linspace(self.x2_bounds[0], self.x2_bounds[1], int(self.grid_resolution[1])),
                 indexing="ij"
             )
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
+            self.x_sorted = x_points[None, :, :, :]
+            self.y_sorted = y_points[None, :, :, :]
+            self.z_sorted = z_points[None, :, :, :]
 
         elif self.normal_vector == "y":  # Rules of thumb for y plane
             if self.x1_bounds is None:
                 self.x1_bounds = (np.min(x) - 2 * max_diameter, np.max(x) + 10 * max_diameter)
 
             if self.x2_bounds is None:
                 self.x2_bounds = (0.001, 6 * np.max(z))
@@ -629,17 +587,17 @@
             x_points, y_points, z_points = np.meshgrid(
                 np.linspace(self.x1_bounds[0], self.x1_bounds[1], int(self.grid_resolution[0])),
                 np.array([float(self.planar_coordinate)]),
                 np.linspace(self.x2_bounds[0], self.x2_bounds[1], int(self.grid_resolution[1])),
                 indexing="ij"
             )
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
+            self.x_sorted = x_points[None, :, :, :]
+            self.y_sorted = y_points[None, :, :, :]
+            self.z_sorted = z_points[None, :, :, :]
 
         # Now calculate grid coordinates in original frame (from 270 deg perspective)
         self.x_sorted_inertial_frame, self.y_sorted_inertial_frame, self.z_sorted_inertial_frame = \
             reverse_rotate_coordinates_rel_west(
                 wind_directions=self.wind_directions,
                 grid_x=self.x_sorted,
                 grid_y=self.y_sorted,
@@ -653,18 +611,14 @@
     """
     Args:
         turbine_coordinates (:py:obj:`NDArrayFloat`): Not used for PointsGrid, but
             required for the `Grid` super-class.
         turbine_diameters (:py:obj:`NDArrayFloat`):  Not used for PointsGrid, but
             required for the `Grid` super-class.
         wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`):  Not used for PointsGrid, but
-            required for the `Grid` super-class.
-        time_series (:py:obj:`bool`):  Not used for PointsGrid, but
-            required for the `Grid` super-class.
         grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Not used for PointsGrid, but
             required for the `Grid` super-class.
 
         points_x (:py:obj:`NDArrayFloat`): Array of x-components for the points in the grid.
         points_y (:py:obj:`NDArrayFloat`): Array of y-components for the points in the grid.
         points_z (:py:obj:`NDArrayFloat`): Array of z-components for the points in the grid.
         x_center_of_rotation (:py:obj:`float`, optional): Component of the centroid of the
@@ -694,10 +648,10 @@
         # These are the rotated coordinates of the wind turbines based on the wind direction
         x, y, z, _, _ = rotate_coordinates_rel_west(
             self.wind_directions,
             point_coordinates,
             x_center_of_rotation=self.x_center_of_rotation,
             y_center_of_rotation=self.y_center_of_rotation
         )
-        self.x_sorted = x[:,:,:,None,None]
-        self.y_sorted = y[:,:,:,None,None]
-        self.z_sorted = z[:,:,:,None,None]
+        self.x_sorted = x[:,:,None,None]
+        self.y_sorted = y[:,:,None,None]
+        self.z_sorted = z[:,:,None,None]
```

### Comparing `FLORIS-3.6/floris/simulation/solver.py` & `FLORIS-4/floris/core/solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from __future__ import annotations
 
 import copy
 
 import numpy as np
 
-from floris.simulation import (
+from floris.core import (
     axial_induction,
-    Ct,
     Farm,
     FlowField,
     FlowFieldGrid,
     FlowFieldPlanarGrid,
     PointsGrid,
+    thrust_coefficient,
     TurbineGrid,
 )
-from floris.simulation.turbine import average_velocity
-from floris.simulation.turbine_multi_dim import (
-    axial_induction_multidim,
-    Ct_multidim,
-    multidim_Ct_down_select,
-)
-from floris.simulation.wake import WakeModelManager
-from floris.simulation.wake_deflection.empirical_gauss import yaw_added_wake_mixing
-from floris.simulation.wake_deflection.gauss import (
+from floris.core.rotor_velocity import average_velocity
+from floris.core.wake import WakeModelManager
+from floris.core.wake_deflection.empirical_gauss import yaw_added_wake_mixing
+from floris.core.wake_deflection.gauss import (
     calculate_transverse_velocity,
     wake_added_yaw,
     yaw_added_turbulence_mixing,
 )
+from floris.core.wake_velocity.empirical_gauss import awc_added_wake_mixing
 from floris.type_dec import NDArrayFloat
 from floris.utilities import cosd
 
 
 def calculate_area_overlap(wake_velocities, freestream_velocities, y_ngrid, z_ngrid):
     """
     compute wake overlap based on the number of points that are not freestream
@@ -77,82 +62,95 @@
     deficit_model_args = model_manager.velocity_model.prepare_function(grid, flow_field)
 
     # This is u_wake
     wake_field = np.zeros_like(flow_field.u_initial_sorted)
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
 
-    turbine_turbulence_intensity = (
-        flow_field.turbulence_intensity
-        * np.ones((flow_field.n_wind_directions, flow_field.n_wind_speeds, farm.n_turbines, 1, 1))
-    )
-    ambient_turbulence_intensity = flow_field.turbulence_intensity
+    # Expand input turbulence intensity to 4d for (n_turbines, grid, grid)
+    turbine_turbulence_intensity = flow_field.turbulence_intensities[:, None, None, None]
+    turbine_turbulence_intensity = np.repeat(turbine_turbulence_intensity, farm.n_turbines, axis=1)
+
+    # Ambient turbulent intensity should be a copy of n_findex-long turbulence_intensity
+    # with dimensions expanded for (n_turbines, grid, grid)
+    ambient_turbulence_intensities = flow_field.turbulence_intensities.copy()
+    ambient_turbulence_intensities = ambient_turbulence_intensities[:, None, None, None]
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
+        x_i = np.mean(grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        u_i = flow_field.u_sorted[:, :, i:i+1]
-        v_i = flow_field.v_sorted[:, :, i:i+1]
+        u_i = flow_field.u_sorted[:, i:i+1]
+        v_i = flow_field.v_sorted[:, i:i+1]
 
-        ct_i = Ct(
+        ct_i = thrust_coefficient(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes_sorted,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=farm.turbine_thrust_coefficient_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions
         )
-        # Since we are filtering for the i'th turbine in the Ct function,
+        # Since we are filtering for the i'th turbine in the thrust coefficient function,
         # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
+        ct_i = ct_i[:, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes_sorted,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            axial_induction_functions=farm.turbine_axial_induction_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
-        turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
-        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        rotor_diameter_i = farm.rotor_diameters_sorted[:, :, i:i+1, None, None]
-        TSR_i = farm.TSRs_sorted[:, :, i:i+1, None, None]
+        axial_induction_i = axial_induction_i[:, 0:1, None, None]
+        turbulence_intensity_i = turbine_turbulence_intensity[:, i:i+1]
+        yaw_angle_i = farm.yaw_angles_sorted[:, i:i+1, None, None]
+        hub_height_i = farm.hub_heights_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = farm.rotor_diameters_sorted[:, i:i+1, None, None]
+        TSR_i = farm.TSRs_sorted[:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         if model_manager.enable_secondary_steering:
             added_yaw = wake_added_yaw(
                 u_i,
                 v_i,
                 flow_field.u_initial_sorted,
-                grid.y_sorted[:, :, i:i+1] - y_i,
-                grid.z_sorted[:, :, i:i+1],
+                grid.y_sorted[:, i:i+1] - y_i,
+                grid.z_sorted[:, i:i+1],
                 rotor_diameter_i,
                 hub_height_i,
                 ct_i,
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
             )
@@ -188,20 +186,20 @@
             )
 
         if model_manager.enable_yaw_added_recovery:
             I_mixing = yaw_added_turbulence_mixing(
                 u_i,
                 turbulence_intensity_i,
                 v_i,
-                flow_field.w_sorted[:, :, i:i+1],
-                v_wake[:, :, i:i+1],
-                w_wake[:, :, i:i+1],
+                flow_field.w_sorted[:, i:i+1],
+                v_wake[:, i:i+1],
+                w_wake[:, i:i+1],
             )
             gch_gain = 2
-            turbine_turbulence_intensity[:, :, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
+            turbine_turbulence_intensity[:, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
 
         # NOTE: exponential
         velocity_deficit = model_manager.velocity_model.function(
             x_i,
             y_i,
             z_i,
             axial_induction_i,
@@ -216,91 +214,85 @@
 
         wake_field = model_manager.combination_model.function(
             wake_field,
             velocity_deficit * flow_field.u_initial_sorted
         )
 
         wake_added_turbulence_intensity = model_manager.turbulence_model.function(
-            ambient_turbulence_intensity,
+            ambient_turbulence_intensities,
             grid.x_sorted,
             x_i,
             rotor_diameter_i,
             axial_induction_i,
         )
 
         # Calculate wake overlap for wake-added turbulence (WAT)
         area_overlap = (
-            np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(3, 4))
+            np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(2, 3))
             / (grid.grid_resolution * grid.grid_resolution)
         )
-        area_overlap = area_overlap[:, :, :, None, None]
+        area_overlap = area_overlap[:, :, None, None]
 
         # Modify wake added turbulence by wake area overlap
         downstream_influence_length = 15 * rotor_diameter_i
         ti_added = (
             area_overlap
             * np.nan_to_num(wake_added_turbulence_intensity, posinf=0.0)
             * (grid.x_sorted > x_i)
             * (np.abs(y_i - grid.y_sorted) < 2 * rotor_diameter_i)
             * (grid.x_sorted <= downstream_influence_length + x_i)
         )
 
         # Combine turbine TIs with WAT
         turbine_turbulence_intensity = np.maximum(
-            np.sqrt( ti_added ** 2 + ambient_turbulence_intensity ** 2 ),
-            turbine_turbulence_intensity
+            np.sqrt(ti_added**2 + ambient_turbulence_intensities**2), turbine_turbulence_intensity
         )
 
         flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
 
     flow_field.turbulence_intensity_field_sorted = turbine_turbulence_intensity
     flow_field.turbulence_intensity_field_sorted_avg = np.mean(
         turbine_turbulence_intensity,
-        axis=(3,4)
-    )[:, :, :, None, None]
+        axis=(2,3)
+    )[:, :, None, None]
 
 
 def full_flow_sequential_solver(
     farm: Farm,
     flow_field: FlowField,
     flow_field_grid: FlowFieldGrid | FlowFieldPlanarGrid | PointsGrid,
     model_manager: WakeModelManager
 ) -> None:
 
     # Get the flow quantities and turbine performance
     turbine_grid_farm = copy.deepcopy(farm)
     turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     turbine_grid_farm.construct_turbine_map()
-    turbine_grid_farm.construct_turbine_fCts()
-    turbine_grid_farm.construct_turbine_power_interps()
+    turbine_grid_farm.construct_turbine_thrust_coefficient_functions()
+    turbine_grid_farm.construct_turbine_axial_induction_functions()
+    turbine_grid_farm.construct_turbine_power_functions()
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
-    turbine_grid_farm.construct_turbine_pPs()
-    turbine_grid_farm.construct_turbine_pTs()
-    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
-    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilts()
     turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_findex)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
         turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
-        wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
-        time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
-        turbine_grid_flow_field.n_wind_directions,
-        turbine_grid_flow_field.n_wind_speeds,
+        turbine_grid_flow_field.n_findex,
         turbine_grid.sorted_coord_indices,
     )
     turbine_grid_flow_field.initialize_velocity_field(turbine_grid)
     turbine_grid_farm.initialize(turbine_grid.sorted_indices)
     sequential_solver(turbine_grid_farm, turbine_grid_flow_field, turbine_grid, model_manager)
 
     ### Referring to the quantities from above, calculate the wake in the full grid
@@ -319,69 +311,83 @@
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(flow_field_grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(turbine_grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(turbine_grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(turbine_grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
+        x_i = np.mean(turbine_grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(turbine_grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(turbine_grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        u_i = turbine_grid_flow_field.u_sorted[:, :, i:i+1]
-        v_i = turbine_grid_flow_field.v_sorted[:, :, i:i+1]
+        u_i = turbine_grid_flow_field.u_sorted[:, i:i+1]
+        v_i = turbine_grid_flow_field.v_sorted[:, i:i+1]
 
-        ct_i = Ct(
+        ct_i = thrust_coefficient(
             velocities=turbine_grid_flow_field.u_sorted,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes_sorted,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=turbine_grid_farm.turbine_thrust_coefficient_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             ix_filter=[i],
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
-        # Since we are filtering for the i'th turbine in the Ct function,
+        # Since we are filtering for the i'th turbine in the thrust_coefficient function,
         # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
+        ct_i = ct_i[:, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes_sorted,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            axial_induction_functions=turbine_grid_farm.turbine_axial_induction_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             ix_filter=[i],
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
+        axial_induction_i = axial_induction_i[:, 0:1, None, None]
         turbulence_intensity_i = \
-            turbine_grid_flow_field.turbulence_intensity_field_sorted_avg[:, :, i:i+1]
-        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = turbine_grid_farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[:, :, i:i+1, None, None]
-        TSR_i = turbine_grid_farm.TSRs_sorted[:, :, i:i+1, None, None]
+            turbine_grid_flow_field.turbulence_intensity_field_sorted_avg[:, i:i+1]
+        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, i:i+1, None, None]
+        hub_height_i = turbine_grid_farm.hub_heights_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[:, i:i+1, None, None]
+        TSR_i = turbine_grid_farm.TSRs_sorted[:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         if model_manager.enable_secondary_steering:
             added_yaw = wake_added_yaw(
                 u_i,
                 v_i,
                 turbine_grid_flow_field.u_initial_sorted,
-                turbine_grid.y_sorted[:, :, i:i+1] - y_i,
-                turbine_grid.z_sorted[:, :, i:i+1],
+                turbine_grid.y_sorted[:, i:i+1] - y_i,
+                turbine_grid.z_sorted[:, i:i+1],
                 rotor_diameter_i,
                 hub_height_i,
                 ct_i,
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
             )
@@ -453,132 +459,150 @@
 
     # This is u_wake
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
     turb_u_wake = np.zeros_like(flow_field.u_initial_sorted)
     turb_inflow_field = copy.deepcopy(flow_field.u_initial_sorted)
 
-    turbine_turbulence_intensity = (
-        flow_field.turbulence_intensity
-        * np.ones((flow_field.n_wind_directions, flow_field.n_wind_speeds, farm.n_turbines, 1, 1))
-    )
-    ambient_turbulence_intensity = flow_field.turbulence_intensity
+    # Set up turbulence arrays
+    turbine_turbulence_intensity = flow_field.turbulence_intensities[:, None, None, None]
+    turbine_turbulence_intensity = np.repeat(turbine_turbulence_intensity, farm.n_turbines, axis=1)
+
+    # Ambient turbulent intensity should be a copy of n_findex-long turbulence_intensities
+    # with extra dimension to reach 4d
+    ambient_turbulence_intensities = flow_field.turbulence_intensities.copy()
+    ambient_turbulence_intensities = ambient_turbulence_intensities[:, None, None, None]
 
     shape = (farm.n_turbines,) + np.shape(flow_field.u_initial_sorted)
     Ctmp = np.zeros((shape))
     # Ctmp = np.zeros((len(x_coord), len(wd), len(ws), len(x_coord), y_ngrid, z_ngrid))
 
     # sigma_i = np.zeros((shape))
     # sigma_i = np.zeros((len(x_coord), len(wd), len(ws), len(x_coord), y_ngrid, z_ngrid))
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
+        x_i = np.mean(grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        rotor_diameter_i = farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
+        rotor_diameter_i = farm.rotor_diameters_sorted[:, i:i+1, None, None]
 
         mask2 = (
             (grid.x_sorted < x_i + 0.01)
             * (grid.x_sorted > x_i - 0.01)
             * (grid.y_sorted < y_i + 0.51 * rotor_diameter_i)
             * (grid.y_sorted > y_i - 0.51 * rotor_diameter_i)
         )
         turb_inflow_field = (
             turb_inflow_field * ~mask2
             + (flow_field.u_initial_sorted - turb_u_wake) * mask2
         )
 
         turb_avg_vels = average_velocity(turb_inflow_field)
-        turb_Cts = Ct(
+        turb_Cts = thrust_coefficient(
             turb_avg_vels,
+            flow_field.air_density,
             farm.yaw_angles_sorted,
             farm.tilt_angles_sorted,
-            farm.ref_tilt_cp_cts_sorted,
-            farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            farm.power_setpoints_sorted,
+            farm.awc_modes_sorted,
+            farm.awc_amplitudes_sorted,
+            farm.turbine_thrust_coefficient_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
-        turb_Cts = turb_Cts[:, :, :, None, None]
+        turb_Cts = turb_Cts[:, :, None, None]
         turb_aIs = axial_induction(
             turb_avg_vels,
+            flow_field.air_density,
             farm.yaw_angles_sorted,
             farm.tilt_angles_sorted,
-            farm.ref_tilt_cp_cts_sorted,
-            farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            farm.power_setpoints_sorted,
+            farm.awc_modes_sorted,
+            farm.awc_amplitudes_sorted,
+            farm.turbine_axial_induction_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
-        turb_aIs = turb_aIs[:, :, :, None, None]
+        turb_aIs = turb_aIs[:, :, None, None]
 
-        u_i = turb_inflow_field[:, :, i:i+1]
-        v_i = flow_field.v_sorted[:, :, i:i+1]
+        u_i = turb_inflow_field[:, i:i+1]
+        v_i = flow_field.v_sorted[:, i:i+1]
 
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes_sorted,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            axial_induction_functions=farm.turbine_axial_induction_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
 
-        axial_induction_i = axial_induction_i[:, :, :, None, None]
+        axial_induction_i = axial_induction_i[:, :, None, None]
 
-        turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
-        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        TSR_i = farm.TSRs_sorted[:, :, i:i+1, None, None]
+        turbulence_intensity_i = turbine_turbulence_intensity[:, i:i+1]
+        yaw_angle_i = farm.yaw_angles_sorted[:, i:i+1, None, None]
+        hub_height_i = farm.hub_heights_sorted[:, i:i+1, None, None]
+        TSR_i = farm.TSRs_sorted[:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         if model_manager.enable_secondary_steering:
             added_yaw = wake_added_yaw(
                 u_i,
                 v_i,
                 flow_field.u_initial_sorted,
-                grid.y_sorted[:, :, i:i+1] - y_i,
-                grid.z_sorted[:, :, i:i+1],
+                grid.y_sorted[:, i:i+1] - y_i,
+                grid.z_sorted[:, i:i+1],
                 rotor_diameter_i,
                 hub_height_i,
-                turb_Cts[:, :, i:i+1],
+                turb_Cts[:, i:i+1],
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
                 scale=2.0,
             )
             effective_yaw_i += added_yaw
 
         # Model calculations
         # NOTE: exponential
         deflection_field = model_manager.deflection_model.function(
             x_i,
             y_i,
             effective_yaw_i,
             turbulence_intensity_i,
-            turb_Cts[:, :, i:i+1],
+            turb_Cts[:, i:i+1],
             rotor_diameter_i,
             **deflection_model_args,
         )
 
         if model_manager.enable_transverse_velocities:
             v_wake, w_wake = calculate_transverse_velocity(
                 u_i,
@@ -586,126 +610,120 @@
                 flow_field.dudz_initial_sorted,
                 grid.x_sorted - x_i,
                 grid.y_sorted - y_i,
                 grid.z_sorted,
                 rotor_diameter_i,
                 hub_height_i,
                 yaw_angle_i,
-                turb_Cts[:, :, i:i+1],
+                turb_Cts[:, i:i+1],
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
                 scale=2.0,
             )
 
         if model_manager.enable_yaw_added_recovery:
             I_mixing = yaw_added_turbulence_mixing(
                 u_i,
                 turbulence_intensity_i,
                 v_i,
-                flow_field.w_sorted[:, :, i:i+1],
-                v_wake[:, :, i:i+1],
-                w_wake[:, :, i:i+1],
+                flow_field.w_sorted[:, i:i+1],
+                v_wake[:, i:i+1],
+                w_wake[:, i:i+1],
             )
             gch_gain = 1.0
-            turbine_turbulence_intensity[:, :, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
+            turbine_turbulence_intensity[:, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
 
         turb_u_wake, Ctmp = model_manager.velocity_model.function(
             i,
             x_i,
             y_i,
             z_i,
             u_i,
             deflection_field,
             yaw_angle_i,
             turbine_turbulence_intensity,
             turb_Cts,
-            farm.rotor_diameters_sorted[:, :, :, None, None],
+            farm.rotor_diameters_sorted[:, :, None, None],
             turb_u_wake,
             Ctmp,
             **deficit_model_args,
         )
 
         wake_added_turbulence_intensity = model_manager.turbulence_model.function(
-            ambient_turbulence_intensity,
+            ambient_turbulence_intensities,
             grid.x_sorted,
             x_i,
             rotor_diameter_i,
             turb_aIs
         )
 
         # Calculate wake overlap for wake-added turbulence (WAT)
         area_overlap = 1 - (
-            np.sum(turb_u_wake <= 0.05, axis=(3, 4))
+            np.sum(turb_u_wake <= 0.05, axis=(2, 3))
             / (grid.grid_resolution * grid.grid_resolution)
         )
-        area_overlap = area_overlap[:, :, :, None, None]
+        area_overlap = area_overlap[:, :, None, None]
 
         # Modify wake added turbulence by wake area overlap
         downstream_influence_length = 15 * rotor_diameter_i
         ti_added = (
             area_overlap
             * np.nan_to_num(wake_added_turbulence_intensity, posinf=0.0)
             * (grid.x_sorted > x_i)
             * (np.abs(y_i - grid.y_sorted) < 2 * rotor_diameter_i)
             * (grid.x_sorted <= downstream_influence_length + x_i)
         )
 
         # Combine turbine TIs with WAT
         turbine_turbulence_intensity = np.maximum(
-            np.sqrt(ti_added ** 2 + ambient_turbulence_intensity ** 2),
-            turbine_turbulence_intensity
+            np.sqrt(ti_added**2 + ambient_turbulence_intensities**2), turbine_turbulence_intensity
         )
 
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
     flow_field.u_sorted = turb_inflow_field
 
     flow_field.turbulence_intensity_field_sorted = turbine_turbulence_intensity
     flow_field.turbulence_intensity_field_sorted_avg = np.mean(
         turbine_turbulence_intensity,
-        axis=(3,4)
+        axis=(2,3)
     )
 
 
 def full_flow_cc_solver(
     farm: Farm,
     flow_field: FlowField,
-    flow_field_grid: FlowFieldGrid,
+    flow_field_grid: FlowFieldGrid | FlowFieldPlanarGrid | PointsGrid,
     model_manager: WakeModelManager,
 ) -> None:
     # Get the flow quantities and turbine performance
     turbine_grid_farm = copy.deepcopy(farm)
     turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     turbine_grid_farm.construct_turbine_map()
-    turbine_grid_farm.construct_turbine_fCts()
-    turbine_grid_farm.construct_turbine_power_interps()
+    turbine_grid_farm.construct_turbine_thrust_coefficient_functions()
+    turbine_grid_farm.construct_turbine_axial_induction_functions()
+    turbine_grid_farm.construct_turbine_power_functions()
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
-    turbine_grid_farm.construct_turbine_pPs()
-    turbine_grid_farm.construct_turbine_pTs()
-    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
-    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilts()
     turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_findex)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
         turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
-        wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
-        time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
-        turbine_grid_flow_field.n_wind_directions,
-        turbine_grid_flow_field.n_wind_speeds,
+        turbine_grid_flow_field.n_findex,
         turbine_grid.sorted_coord_indices,
     )
     turbine_grid_flow_field.initialize_velocity_field(turbine_grid)
     turbine_grid_farm.initialize(turbine_grid.sorted_indices)
     cc_solver(turbine_grid_farm, turbine_grid_flow_field, turbine_grid, model_manager)
 
     ### Referring to the quantities from above, calculate the wake in the full grid
@@ -727,89 +745,99 @@
     shape = (farm.n_turbines,) + np.shape(flow_field.u_initial_sorted)
     Ctmp = np.zeros((shape))
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(flow_field_grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(turbine_grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(turbine_grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(turbine_grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
+        x_i = np.mean(turbine_grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(turbine_grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(turbine_grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        u_i = turbine_grid_flow_field.u_sorted[:, :, i:i+1]
-        v_i = turbine_grid_flow_field.v_sorted[:, :, i:i+1]
+        u_i = turbine_grid_flow_field.u_sorted[:, i:i+1]
+        v_i = turbine_grid_flow_field.v_sorted[:, i:i+1]
 
         turb_avg_vels = average_velocity(turbine_grid_flow_field.u_sorted)
-        turb_Cts = Ct(
+        turb_Cts = thrust_coefficient(
             velocities=turb_avg_vels,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=turbine_grid_farm.turbine_thrust_coefficient_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             average_method=turbine_grid.average_method,
-            cubature_weights=turbine_grid.cubature_weights
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
-        turb_Cts = turb_Cts[:, :, :, None, None]
+        turb_Cts = turb_Cts[:, :, None, None]
 
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            axial_induction_functions=turbine_grid_farm.turbine_axial_induction_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=turbine_grid.average_method,
-            cubature_weights=turbine_grid.cubature_weights
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
-        axial_induction_i = axial_induction_i[:, :, :, None, None]
+        axial_induction_i = axial_induction_i[:, :, None, None]
 
         turbulence_intensity_i = \
-            turbine_grid_flow_field.turbulence_intensity_field_sorted_avg[:, :, i:i+1]
-        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = turbine_grid_farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[:, :, i:i+1, None, None]
-        TSR_i = turbine_grid_farm.TSRs_sorted[:, :, i:i+1, None, None]
+            turbine_grid_flow_field.turbulence_intensity_field_sorted_avg[:, i:i+1]
+        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, i:i+1, None, None]
+        hub_height_i = turbine_grid_farm.hub_heights_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[:, i:i+1, None, None]
+        TSR_i = turbine_grid_farm.TSRs_sorted[:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         if model_manager.enable_secondary_steering:
             added_yaw = wake_added_yaw(
                 u_i,
                 v_i,
                 turbine_grid_flow_field.u_initial_sorted,
-                turbine_grid.y_sorted[:, :, i:i+1] - y_i,
-                turbine_grid.z_sorted[:, :, i:i+1],
+                turbine_grid.y_sorted[:, i:i+1] - y_i,
+                turbine_grid.z_sorted[:, i:i+1],
                 rotor_diameter_i,
                 hub_height_i,
-                turb_Cts[:, :, i:i+1],
+                turb_Cts[:, i:i+1],
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
                 scale=2.0,
             )
             effective_yaw_i += added_yaw
 
         # Model calculations
         # NOTE: exponential
         deflection_field = model_manager.deflection_model.function(
             x_i,
             y_i,
             effective_yaw_i,
             turbulence_intensity_i,
-            turb_Cts[:, :, i:i+1],
+            turb_Cts[:, i:i+1],
             rotor_diameter_i,
             **deflection_model_args,
         )
 
         if model_manager.enable_transverse_velocities:
             v_wake, w_wake = calculate_transverse_velocity(
                 u_i,
@@ -817,15 +845,15 @@
                 flow_field.dudz_initial_sorted,
                 flow_field_grid.x_sorted - x_i,
                 flow_field_grid.y_sorted - y_i,
                 flow_field_grid.z_sorted,
                 rotor_diameter_i,
                 hub_height_i,
                 yaw_angle_i,
-                turb_Cts[:, :, i:i+1],
+                turb_Cts[:, i:i+1],
                 TSR_i,
                 axial_induction_i,
                 flow_field.wind_shear,
                 scale=2.0,
             )
 
         # NOTE: exponential
@@ -835,15 +863,15 @@
             y_i,
             z_i,
             u_i,
             deflection_field,
             yaw_angle_i,
             turbine_grid_flow_field.turbulence_intensity_field_sorted_avg,
             turb_Cts,
-            turbine_grid_farm.rotor_diameters_sorted[:, :, :, None, None],
+            turbine_grid_farm.rotor_diameters_sorted[:, :, None, None],
             turb_u_wake,
             Ctmp,
             **deficit_model_args,
         )
 
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
@@ -870,290 +898,232 @@
     wake_field = np.zeros_like(flow_field.u_initial_sorted)
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
     shape = (farm.n_turbines,) + np.shape(flow_field.u_initial_sorted)
     velocity_deficit = np.zeros(shape)
     deflection_field = np.zeros_like(flow_field.u_initial_sorted)
 
-    turbine_turbulence_intensity = (
-        flow_field.turbulence_intensity
-        * np.ones((flow_field.n_wind_directions, flow_field.n_wind_speeds, farm.n_turbines, 1, 1))
-    )
-    ambient_turbulence_intensity = flow_field.turbulence_intensity
+    # Set up turbulence arrays
+    turbine_turbulence_intensity = flow_field.turbulence_intensities[:, None, None, None]
+    turbine_turbulence_intensity = np.repeat(turbine_turbulence_intensity, farm.n_turbines, axis=1)
+
+    # Ambient turbulent intensity should be a copy of n_findex-long turbulence_intensities
+    # with extra dimension to reach 4d
+    ambient_turbulence_intensities = flow_field.turbulence_intensities.copy()
+    ambient_turbulence_intensities = ambient_turbulence_intensities[:, None, None, None]
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(grid.n_turbines):
         # Get the current turbine quantities
-        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
-
-        u_i = flow_field.u_sorted[:, :, i:i+1]
-        v_i = flow_field.v_sorted[:, :, i:i+1]
+        x_i = np.mean(grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        Cts = Ct(
+        Cts = thrust_coefficient(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=farm.turbine_thrust_coefficient_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
 
-        ct_i = Ct(
+        ct_i = thrust_coefficient(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=farm.turbine_thrust_coefficient_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
-        # Since we are filtering for the i'th turbine in the Ct function,
+        # Since we are filtering for the i'th turbine in the thrust coefficient function,
         # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
+        ct_i = ct_i[:, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            axial_induction_functions=farm.turbine_axial_induction_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
-        turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
-        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        rotor_diameter_i = farm.rotor_diameters_sorted[:, :, i:i+1, None, None]
-        TSR_i = farm.TSRs_sorted[:, :, i:i+1, None, None]
+        axial_induction_i = axial_induction_i[:, 0:1, None, None]
+        yaw_angle_i = farm.yaw_angles_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = farm.rotor_diameters_sorted[:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
+
         if model_manager.enable_secondary_steering:
-            added_yaw = wake_added_yaw(
-                u_i,
-                v_i,
-                flow_field.u_initial_sorted,
-                grid.y_sorted[:, :, i:i+1] - y_i,
-                grid.z_sorted[:, :, i:i+1],
-                rotor_diameter_i,
-                hub_height_i,
-                ct_i,
-                TSR_i,
-                axial_induction_i,
-                flow_field.wind_shear,
-            )
-            effective_yaw_i += added_yaw
+            raise NotImplementedError(
+                "Secondary steering not available for this model.")
 
         # Model calculations
         # NOTE: exponential
         if np.any(farm.yaw_angles_sorted):
             model_manager.deflection_model.logger.warning(
-                "WARNING: Deflection with the TurbOPark model has not been fully validated."
-                "This is an initial implementation, and we advise you use at your own risk"
+                "WARNING: Deflection with the TurbOPark model has not been fully validated. "
+                "This is an initial implementation, and we advise you use at your own risk "
                 "and perform a thorough examination of the results."
             )
             for ii in range(i):
-                x_ii = np.mean(grid.x_sorted[:, :, ii:ii+1], axis=(3, 4))
-                x_ii = x_ii[:, :, :, None, None]
-                y_ii = np.mean(grid.y_sorted[:, :, ii:ii+1], axis=(3, 4))
-                y_ii = y_ii[:, :, :, None, None]
-
-                yaw_ii = farm.yaw_angles_sorted[:, :, ii:ii+1, None, None]
-                turbulence_intensity_ii = turbine_turbulence_intensity[:, :, ii:ii+1]
-                ct_ii = Ct(
+                x_ii = np.mean(grid.x_sorted[:, ii:ii+1], axis=(2, 3))
+                x_ii = x_ii[:, :, None, None]
+                y_ii = np.mean(grid.y_sorted[:, ii:ii+1], axis=(2, 3))
+                y_ii = y_ii[:, :, None, None]
+
+                yaw_ii = farm.yaw_angles_sorted[:, ii:ii+1, None, None]
+                turbulence_intensity_ii = turbine_turbulence_intensity[:, ii:ii+1]
+                ct_ii = thrust_coefficient(
                     velocities=flow_field.u_sorted,
-                    yaw_angle=farm.yaw_angles_sorted,
-                    tilt_angle=farm.tilt_angles_sorted,
-                    ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-                    fCt=farm.turbine_fCts,
-                    tilt_interp=farm.turbine_tilt_interps,
+                    air_density=flow_field.air_density,
+                    yaw_angles=farm.yaw_angles_sorted,
+                    tilt_angles=farm.tilt_angles_sorted,
+                    power_setpoints=farm.power_setpoints_sorted,
+                    awc_modes=farm.awc_modes,
+                    awc_amplitudes=farm.awc_amplitudes_sorted,
+                    thrust_coefficient_functions=farm.turbine_thrust_coefficient_functions,
+                    tilt_interps=farm.turbine_tilt_interps,
                     correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
                     turbine_type_map=farm.turbine_type_map_sorted,
+                    turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
                     ix_filter=[ii],
                     average_method=grid.average_method,
-                    cubature_weights=grid.cubature_weights
+                    cubature_weights=grid.cubature_weights,
+                    multidim_condition=flow_field.multidim_conditions,
                 )
-                ct_ii = ct_ii[:, :, 0:1, None, None]
-                rotor_diameter_ii = farm.rotor_diameters_sorted[:, :, ii:ii+1, None, None]
+                ct_ii = ct_ii[:, 0:1, None, None]
+                rotor_diameter_ii = farm.rotor_diameters_sorted[:, ii:ii+1, None, None]
 
                 deflection_field_ii = model_manager.deflection_model.function(
                     x_ii,
                     y_ii,
                     yaw_ii,
                     turbulence_intensity_ii,
                     ct_ii,
                     rotor_diameter_ii,
                     **deflection_model_args,
                 )
 
-                deflection_field[:, :, ii:ii+1, :, :] = deflection_field_ii[:, :, i:i+1, :, :]
+                deflection_field[:, ii:ii+1, :, :] = deflection_field_ii[:, i:i+1, :, :]
 
         if model_manager.enable_transverse_velocities:
-            v_wake, w_wake = calculate_transverse_velocity(
-                u_i,
-                flow_field.u_initial_sorted,
-                flow_field.dudz_initial_sorted,
-                grid.x_sorted - x_i,
-                grid.y_sorted - y_i,
-                grid.z_sorted,
-                rotor_diameter_i,
-                hub_height_i,
-                yaw_angle_i,
-                ct_i,
-                TSR_i,
-                axial_induction_i,
-                flow_field.wind_shear,
-            )
+            raise NotImplementedError(
+                "Transverse velocities not used in this model.")
 
         if model_manager.enable_yaw_added_recovery:
-            I_mixing = yaw_added_turbulence_mixing(
-                u_i,
-                turbulence_intensity_i,
-                v_i,
-                flow_field.w_sorted[:, :, i:i+1],
-                v_wake[:, :, i:i+1],
-                w_wake[:, :, i:i+1],
-            )
-            gch_gain = 2
-            turbine_turbulence_intensity[:, :, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
+            raise NotImplementedError(
+                "Yaw added recovery not used in this model.")
 
         # NOTE: exponential
         velocity_deficit = model_manager.velocity_model.function(
             x_i,
             y_i,
             z_i,
             turbine_turbulence_intensity,
-            Cts[:, :, :, None, None],
+            Cts[:, :, None, None],
             rotor_diameter_i,
-            farm.rotor_diameters_sorted[:, :, :, None, None],
+            farm.rotor_diameters_sorted[:, :, None, None],
             i,
             deflection_field,
             **deficit_model_args,
         )
 
         wake_field = model_manager.combination_model.function(
             wake_field,
             velocity_deficit * flow_field.u_initial_sorted
         )
 
         wake_added_turbulence_intensity = model_manager.turbulence_model.function(
-            ambient_turbulence_intensity,
+            ambient_turbulence_intensities,
             grid.x_sorted,
             x_i,
             rotor_diameter_i,
             axial_induction_i
         )
 
         # TODO: leaving this in for GCH quantities; will need to find another way to
         # compute area_overlap as the current wake deficit is solved for only upstream
         # turbines; could use WAT_upstream
         # Calculate wake overlap for wake-added turbulence (WAT)
         area_overlap = (
-            np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(3, 4))
+            np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(2, 3))
             / (grid.grid_resolution * grid.grid_resolution)
         )
-        area_overlap = area_overlap[:, :, :, None, None]
+        area_overlap = area_overlap[:, :, None, None]
 
         # Modify wake added turbulence by wake area overlap
         downstream_influence_length = 15 * rotor_diameter_i
         ti_added = (
             area_overlap
             * np.nan_to_num(wake_added_turbulence_intensity, posinf=0.0)
             * (grid.x_sorted > x_i)
             * (np.abs(y_i - grid.y_sorted) < 2 * rotor_diameter_i)
             * (grid.x_sorted <= downstream_influence_length + x_i)
         )
 
         # Combine turbine TIs with WAT
         turbine_turbulence_intensity = np.maximum(
-            np.sqrt( ti_added ** 2 + ambient_turbulence_intensity ** 2 ),
-            turbine_turbulence_intensity
+            np.sqrt(ti_added**2 + ambient_turbulence_intensities**2), turbine_turbulence_intensity
         )
 
         flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
 
     flow_field.turbulence_intensity_field_sorted = turbine_turbulence_intensity
     flow_field.turbulence_intensity_field_sorted_avg = np.mean(
         turbine_turbulence_intensity,
-        axis=(3,4)
+        axis=(2, 3)
     )
 
 
 def full_flow_turbopark_solver(
     farm: Farm,
     flow_field: FlowField,
     flow_field_grid: FlowFieldGrid,
     model_manager: WakeModelManager
 ) -> None:
     raise NotImplementedError("Plotting for the TurbOPark model is not currently implemented.")
 
-    # TODO: Below is a first attempt at plotting, and uses just the values on the rotor.
-    # The current TurbOPark model requires that points to be calculated are only at turbine
-    # locations. Modification will be required to allow for full flow field calculations.
-
-    # # Get the flow quantities and turbine performance
-    # turbine_grid_farm = copy.deepcopy(farm)
-    # turbine_grid_flow_field = copy.deepcopy(flow_field)
-
-    # turbine_grid_farm.construct_turbine_map()
-    # turbine_grid_farm.construct_turbine_fCts()
-    # turbine_grid_farm.construct_turbine_power_interps()
-    # turbine_grid_farm.construct_hub_heights()
-    # turbine_grid_farm.construct_rotor_diameters()
-    # turbine_grid_farm.construct_turbine_TSRs()
-    # turbine_grid_farm.construc_turbine_pPs()
-
-    # turbine_grid = TurbineGrid(
-    #     turbine_coordinates=turbine_grid_farm.coordinates,
-    #     turbine_diameters=turbine_grid_farm.rotor_diameters,
-    #     wind_directions=turbine_grid_flow_field.wind_directions,
-    #     wind_speeds=turbine_grid_flow_field.wind_speeds,
-    #     grid_resolution=11,
-    # )
-    # turbine_grid_farm.expand_farm_properties(
-    #     turbine_grid_flow_field.n_wind_directions,
-    #     turbine_grid_flow_field.n_wind_speeds,
-    #     turbine_grid.sorted_coord_indices
-    # )
-    # turbine_grid_flow_field.initialize_velocity_field(turbine_grid)
-    # turbine_grid_farm.initialize(turbine_grid.sorted_indices)
-    # turbopark_solver(turbine_grid_farm, turbine_grid_flow_field, turbine_grid, model_manager)
-
-
-
-    # flow_field.u = copy.deepcopy(turbine_grid_flow_field.u)
-    # flow_field.v = copy.deepcopy(turbine_grid_flow_field.v)
-    # flow_field.w = copy.deepcopy(turbine_grid_flow_field.w)
-
-    # flow_field_grid.x = copy.deepcopy(turbine_grid.x)
-    # flow_field_grid.y = copy.deepcopy(turbine_grid.y)
-    # flow_field_grid.z = copy.deepcopy(turbine_grid.z)
-
 
 def empirical_gauss_solver(
     farm: Farm,
     flow_field: FlowField,
     grid: TurbineGrid,
     model_manager: WakeModelManager
 ) -> NDArrayFloat:
@@ -1184,114 +1154,143 @@
     deficit_model_args = model_manager.velocity_model.prepare_function(grid, flow_field)
 
     # This is u_wake
     wake_field = np.zeros_like(flow_field.u_initial_sorted)
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
 
-    x_locs = np.mean(grid.x_sorted, axis=(3, 4))[:,:,:,None]
-    downstream_distance_D = x_locs - np.transpose(x_locs, axes=(0,1,3,2))
+    x_locs = np.mean(grid.x_sorted, axis=(2, 3))[:,:,None]
+    downstream_distance_D = x_locs - np.transpose(x_locs, axes=(0,2,1))
     downstream_distance_D = downstream_distance_D / \
-        np.repeat(farm.rotor_diameters_sorted[:,:,:,None], grid.n_turbines, axis=-1)
+        np.repeat(farm.rotor_diameters_sorted[:,:,None], grid.n_turbines, axis=-1)
     downstream_distance_D = np.maximum(downstream_distance_D, 0.1) # For ease
-    mixing_factor = np.zeros_like(downstream_distance_D)
-    mixing_factor[:,:,:,:] = model_manager.turbulence_model.atmospheric_ti_gain*\
-        flow_field.turbulence_intensity*np.eye(grid.n_turbines)
+    # Initialize the mixing factor model using TI if specified
+    initial_mixing_factor = model_manager.turbulence_model.atmospheric_ti_gain * np.eye(
+        grid.n_turbines
+    )
+    mixing_factor = np.repeat(
+        initial_mixing_factor[None, :, :],
+        flow_field.n_findex,
+        axis=0
+    )
+    mixing_factor = mixing_factor * flow_field.turbulence_intensities[:, None, None]
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
+        x_i = np.mean(grid.x_sorted[:, i:i+1], axis=(2, 3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(grid.y_sorted[:, i:i+1], axis=(2, 3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(grid.z_sorted[:, i:i+1], axis=(2, 3))
+        z_i = z_i[:, :, None, None]
 
-        flow_field.u_sorted[:, :, i:i+1]
-        flow_field.v_sorted[:, :, i:i+1]
-
-        ct_i = Ct(
+        ct_i = thrust_coefficient(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes_sorted,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=farm.turbine_thrust_coefficient_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
-        # Since we are filtering for the i'th turbine in the Ct function,
+        # Since we are filtering for the i'th turbine in the thrust coefficient function,
         # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
+        ct_i = ct_i[:, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=farm.turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
+            air_density=flow_field.air_density,
+            yaw_angles=farm.yaw_angles_sorted,
+            tilt_angles=farm.tilt_angles_sorted,
+            power_setpoints=farm.power_setpoints_sorted,
+            awc_modes=farm.awc_modes_sorted,
+            awc_amplitudes=farm.awc_amplitudes_sorted,
+            axial_induction_functions=farm.turbine_axial_induction_functions,
+            tilt_interps=farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=farm.turbine_power_thrust_tables,
             ix_filter=[i],
             average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
+            cubature_weights=grid.cubature_weights,
+            multidim_condition=flow_field.multidim_conditions,
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
-        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = farm.hub_heights_sorted[: ,:, i:i+1, None, None]
-        rotor_diameter_i = farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
-
-        effective_yaw_i = np.zeros_like(yaw_angle_i)
-        effective_yaw_i += yaw_angle_i
+        axial_induction_i = axial_induction_i[:, 0:1, None, None]
+        yaw_angle_i = farm.yaw_angles_sorted[:, i:i+1, None, None]
+        awc_mode_i = farm.awc_modes_sorted[:, i:i+1, None, None]
+        awc_amplitude_i = farm.awc_amplitudes_sorted[:, i:i+1, None, None]
+        awc_frequency_i = farm.awc_frequencies_sorted[:, i:i+1, None, None]
+        hub_height_i = farm.hub_heights_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = farm.rotor_diameters_sorted[:, i:i+1, None, None]
+
+        # Secondary steering not currently implemented in EmGauss model
+        # effective_yaw_i = np.zeros_like(yaw_angle_i)
+        # effective_yaw_i += yaw_angle_i
 
         average_velocities = average_velocity(
             flow_field.u_sorted,
             method=grid.average_method,
             cubature_weights=grid.cubature_weights
         )
         tilt_angle_i = farm.calculate_tilt_for_eff_velocities(average_velocities)
-        tilt_angle_i = tilt_angle_i[:, :, i:i+1, None, None]
+        tilt_angle_i = tilt_angle_i[:, i:i+1, None, None]
 
         if model_manager.enable_secondary_steering:
             raise NotImplementedError(
                 "Secondary steering not available for this model.")
 
         if model_manager.enable_transverse_velocities:
             raise NotImplementedError(
                 "Transverse velocities not used in this model.")
 
         if model_manager.enable_yaw_added_recovery:
             # Influence of yawing on turbine's own wake
-            mixing_factor[:, :, i:i+1, i] += \
+            mixing_factor[:, i:i+1, i] += \
                 yaw_added_wake_mixing(
                     axial_induction_i,
                     yaw_angle_i,
                     1,
                     model_manager.deflection_model.yaw_added_mixing_gain
                 )
 
+        if model_manager.enable_active_wake_mixing:
+            # Influence of awc on turbine's own wake
+            mixing_factor[:, i:i+1, i] += \
+                awc_added_wake_mixing(
+                    awc_mode_i,
+                    awc_amplitude_i,
+                    awc_frequency_i,
+                    model_manager.velocity_model.awc_wake_exp,
+                    model_manager.velocity_model.awc_wake_denominator
+                )
+
         # Extract total wake induced mixing for turbine i
         mixing_i = np.linalg.norm(
-            mixing_factor[:, :, i:i+1, :, None],
-            ord=2, axis=3, keepdims=True
+            mixing_factor[:, i:i+1, :, None],
+            ord=2, axis=2, keepdims=True
         )
 
         # Model calculations
         # NOTE: exponential
         deflection_field_y, deflection_field_z = model_manager.deflection_model.function(
             x_i,
             y_i,
-            effective_yaw_i,
+            yaw_angle_i,
             tilt_angle_i,
             mixing_i,
             ct_i,
             rotor_diameter_i,
             **deflection_model_args
         )
 
@@ -1314,28 +1313,28 @@
 
         wake_field = model_manager.combination_model.function(
             wake_field,
             velocity_deficit * flow_field.u_initial_sorted
         )
 
         # Calculate wake overlap for wake-added turbulence (WAT)
-        area_overlap = np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(3, 4))\
+        area_overlap = np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(2, 3))\
             / (grid.grid_resolution * grid.grid_resolution)
 
         # Compute wake induced mixing factor
-        mixing_factor[:,:,:,i] += \
+        mixing_factor[:,:,i] += \
             area_overlap * model_manager.turbulence_model.function(
-                axial_induction_i, downstream_distance_D[:,:,:,i]
+                axial_induction_i, downstream_distance_D[:,:,i]
             )
         if model_manager.enable_yaw_added_recovery:
-            mixing_factor[:,:,:,i] += \
+            mixing_factor[:,:,i] += \
                 area_overlap * yaw_added_wake_mixing(
                 axial_induction_i,
                 yaw_angle_i,
-                downstream_distance_D[:,:,:,i],
+                downstream_distance_D[:,:,i],
                 model_manager.deflection_model.yaw_added_mixing_gain
             )
 
         flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
 
@@ -1350,38 +1349,33 @@
 ) -> None:
 
     # Get the flow quantities and turbine performance
     turbine_grid_farm = copy.deepcopy(farm)
     turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     turbine_grid_farm.construct_turbine_map()
-    turbine_grid_farm.construct_turbine_fCts()
-    turbine_grid_farm.construct_turbine_power_interps()
+    turbine_grid_farm.construct_turbine_thrust_coefficient_functions()
+    turbine_grid_farm.construct_turbine_axial_induction_functions()
+    turbine_grid_farm.construct_turbine_power_functions()
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
-    turbine_grid_farm.construct_turbine_pPs()
-    turbine_grid_farm.construct_turbine_pTs()
-    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
-    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilts()
     turbine_grid_farm.construct_turbine_tilt_interps()
     turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
-    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_findex)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
         turbine_diameters=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
-        wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
-        time_series=turbine_grid_flow_field.time_series,
     )
     turbine_grid_farm.expand_farm_properties(
-        turbine_grid_flow_field.n_wind_directions,
-        turbine_grid_flow_field.n_wind_speeds,
+        turbine_grid_flow_field.n_findex,
         turbine_grid.sorted_coord_indices
     )
     turbine_grid_flow_field.initialize_velocity_field(turbine_grid)
     turbine_grid_farm.initialize(turbine_grid.sorted_indices)
     wim_field = empirical_gauss_solver(
         turbine_grid_farm,
         turbine_grid_flow_field,
@@ -1401,67 +1395,77 @@
     v_wake = np.zeros_like(flow_field.v_initial_sorted)
     w_wake = np.zeros_like(flow_field.w_initial_sorted)
 
     # Calculate the velocity deficit sequentially from upstream to downstream turbines
     for i in range(flow_field_grid.n_turbines):
 
         # Get the current turbine quantities
-        x_i = np.mean(turbine_grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(turbine_grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(turbine_grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
-
-        turbine_grid_flow_field.u_sorted[:, :, i:i+1]
-        turbine_grid_flow_field.v_sorted[:, :, i:i+1]
+        x_i = np.mean(turbine_grid.x_sorted[:, i:i+1], axis=(2,3))
+        x_i = x_i[:, :, None, None]
+        y_i = np.mean(turbine_grid.y_sorted[:, i:i+1], axis=(2,3))
+        y_i = y_i[:, :, None, None]
+        z_i = np.mean(turbine_grid.z_sorted[:, i:i+1], axis=(2,3))
+        z_i = z_i[:, :, None, None]
 
-        ct_i = Ct(
+        ct_i = thrust_coefficient(
             velocities=turbine_grid_flow_field.u_sorted,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes_sorted,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            thrust_coefficient_functions=turbine_grid_farm.turbine_thrust_coefficient_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             ix_filter=[i],
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
-        # Since we are filtering for the i'th turbine in the Ct function,
+        # Since we are filtering for the i'th turbine in the thrust coefficient function,
         # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
+        ct_i = ct_i[:, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
-            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
-            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
-            fCt=turbine_grid_farm.turbine_fCts,
-            tilt_interp=turbine_grid_farm.turbine_tilt_interps,
+            air_density=turbine_grid_flow_field.air_density,
+            yaw_angles=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angles=turbine_grid_farm.tilt_angles_sorted,
+            power_setpoints=turbine_grid_farm.power_setpoints_sorted,
+            awc_modes=turbine_grid_farm.awc_modes_sorted,
+            awc_amplitudes=turbine_grid_farm.awc_amplitudes_sorted,
+            axial_induction_functions=turbine_grid_farm.turbine_axial_induction_functions,
+            tilt_interps=turbine_grid_farm.turbine_tilt_interps,
             correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            turbine_power_thrust_tables=turbine_grid_farm.turbine_power_thrust_tables,
             ix_filter=[i],
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights,
+            multidim_condition=turbine_grid_flow_field.multidim_conditions,
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
-        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = turbine_grid_farm.hub_heights_sorted[: ,:, i:i+1, None, None]
-        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
-        wake_induced_mixing_i = wim_field[:, :, i:i+1, :, None].sum(axis=3, keepdims=1)
-
+        axial_induction_i = axial_induction_i[:, 0:1, None, None]
+        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, i:i+1, None, None]
+        hub_height_i = turbine_grid_farm.hub_heights_sorted[:, i:i+1, None, None]
+        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[:, i:i+1, None, None]
+        wake_induced_mixing_i = wim_field[:, i:i+1, :, None].sum(axis=2, keepdims=1)
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         average_velocities = average_velocity(
             turbine_grid_flow_field.u_sorted,
             method=turbine_grid.average_method,
             cubature_weights=turbine_grid.cubature_weights
         )
         tilt_angle_i = turbine_grid_farm.calculate_tilt_for_eff_velocities(average_velocities)
-        tilt_angle_i = tilt_angle_i[:, :, i:i+1, None, None]
+        tilt_angle_i = tilt_angle_i[:, i:i+1, None, None]
 
         if model_manager.enable_secondary_steering:
             raise NotImplementedError(
                 "Secondary steering not available for this model.")
 
         if model_manager.enable_transverse_velocities:
             raise NotImplementedError(
@@ -1501,212 +1505,7 @@
             wake_field,
             velocity_deficit * flow_field.u_initial_sorted
         )
 
         flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
-
-
-def sequential_multidim_solver(
-    farm: Farm,
-    flow_field: FlowField,
-    grid: TurbineGrid,
-    model_manager: WakeModelManager
-) -> None:
-    # Algorithm
-    # For each turbine, calculate its effect on every downstream turbine.
-    # For the current turbine, we are calculating the deficit that it adds to downstream turbines.
-    # Integrate this into the main data structure.
-    # Move on to the next turbine.
-
-    # <<interface>>
-    deflection_model_args = model_manager.deflection_model.prepare_function(grid, flow_field)
-    deficit_model_args = model_manager.velocity_model.prepare_function(grid, flow_field)
-    downselect_turbine_fCts = multidim_Ct_down_select(
-        farm.turbine_fCts_sorted,
-        flow_field.multidim_conditions,
-    )
-
-    # This is u_wake
-    wake_field = np.zeros_like(flow_field.u_initial_sorted)
-    v_wake = np.zeros_like(flow_field.v_initial_sorted)
-    w_wake = np.zeros_like(flow_field.w_initial_sorted)
-
-    turbine_turbulence_intensity = (
-        flow_field.turbulence_intensity
-        * np.ones((flow_field.n_wind_directions, flow_field.n_wind_speeds, farm.n_turbines, 1, 1))
-    )
-    ambient_turbulence_intensity = flow_field.turbulence_intensity
-
-    # Calculate the velocity deficit sequentially from upstream to downstream turbines
-    for i in range(grid.n_turbines):
-
-        # Get the current turbine quantities
-        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
-        x_i = x_i[:, :, :, None, None]
-        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
-        y_i = y_i[:, :, :, None, None]
-        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
-        z_i = z_i[:, :, :, None, None]
-
-        u_i = flow_field.u_sorted[:, :, i:i+1]
-        v_i = flow_field.v_sorted[:, :, i:i+1]
-
-        ct_i = Ct_multidim(
-            velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=downselect_turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
-            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
-            turbine_type_map=farm.turbine_type_map_sorted,
-            ix_filter=[i],
-            average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
-        )
-        # Since we are filtering for the i'th turbine in the Ct function,
-        # get the first index here (0:1)
-        ct_i = ct_i[:, :, 0:1, None, None]
-        axial_induction_i = axial_induction_multidim(
-            velocities=flow_field.u_sorted,
-            yaw_angle=farm.yaw_angles_sorted,
-            tilt_angle=farm.tilt_angles_sorted,
-            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
-            fCt=downselect_turbine_fCts,
-            tilt_interp=farm.turbine_tilt_interps,
-            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
-            turbine_type_map=farm.turbine_type_map_sorted,
-            ix_filter=[i],
-            average_method=grid.average_method,
-            cubature_weights=grid.cubature_weights
-        )
-        # Since we are filtering for the i'th turbine in the axial induction function,
-        # get the first index here (0:1)
-        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
-        turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
-        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
-        hub_height_i = farm.hub_heights_sorted[:, :, i:i+1, None, None]
-        rotor_diameter_i = farm.rotor_diameters_sorted[:, :, i:i+1, None, None]
-        TSR_i = farm.TSRs_sorted[:, :, i:i+1, None, None]
-
-        effective_yaw_i = np.zeros_like(yaw_angle_i)
-        effective_yaw_i += yaw_angle_i
-
-        if model_manager.enable_secondary_steering:
-            added_yaw = wake_added_yaw(
-                u_i,
-                v_i,
-                flow_field.u_initial_sorted,
-                grid.y_sorted[:, :, i:i+1] - y_i,
-                grid.z_sorted[:, :, i:i+1],
-                rotor_diameter_i,
-                hub_height_i,
-                ct_i,
-                TSR_i,
-                axial_induction_i,
-                flow_field.wind_shear,
-            )
-            effective_yaw_i += added_yaw
-
-        # Model calculations
-        # NOTE: exponential
-        deflection_field = model_manager.deflection_model.function(
-            x_i,
-            y_i,
-            effective_yaw_i,
-            turbulence_intensity_i,
-            ct_i,
-            rotor_diameter_i,
-            **deflection_model_args,
-        )
-
-        if model_manager.enable_transverse_velocities:
-            v_wake, w_wake = calculate_transverse_velocity(
-                u_i,
-                flow_field.u_initial_sorted,
-                flow_field.dudz_initial_sorted,
-                grid.x_sorted - x_i,
-                grid.y_sorted - y_i,
-                grid.z_sorted,
-                rotor_diameter_i,
-                hub_height_i,
-                yaw_angle_i,
-                ct_i,
-                TSR_i,
-                axial_induction_i,
-                flow_field.wind_shear,
-            )
-
-        if model_manager.enable_yaw_added_recovery:
-            I_mixing = yaw_added_turbulence_mixing(
-                u_i,
-                turbulence_intensity_i,
-                v_i,
-                flow_field.w_sorted[:, :, i:i+1],
-                v_wake[:, :, i:i+1],
-                w_wake[:, :, i:i+1],
-            )
-            gch_gain = 2
-            turbine_turbulence_intensity[:, :, i:i+1] = turbulence_intensity_i + gch_gain * I_mixing
-
-        # NOTE: exponential
-        velocity_deficit = model_manager.velocity_model.function(
-            x_i,
-            y_i,
-            z_i,
-            axial_induction_i,
-            deflection_field,
-            yaw_angle_i,
-            turbulence_intensity_i,
-            ct_i,
-            hub_height_i,
-            rotor_diameter_i,
-            **deficit_model_args,
-        )
-
-        wake_field = model_manager.combination_model.function(
-            wake_field,
-            velocity_deficit * flow_field.u_initial_sorted
-        )
-
-        wake_added_turbulence_intensity = model_manager.turbulence_model.function(
-            ambient_turbulence_intensity,
-            grid.x_sorted,
-            x_i,
-            rotor_diameter_i,
-            axial_induction_i,
-        )
-
-        # Calculate wake overlap for wake-added turbulence (WAT)
-        area_overlap = (
-            np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(3, 4))
-            / (grid.grid_resolution * grid.grid_resolution)
-        )
-        area_overlap = area_overlap[:, :, :, None, None]
-
-        # Modify wake added turbulence by wake area overlap
-        downstream_influence_length = 15 * rotor_diameter_i
-        ti_added = (
-            area_overlap
-            * np.nan_to_num(wake_added_turbulence_intensity, posinf=0.0)
-            * (grid.x_sorted > x_i)
-            * (np.abs(y_i - grid.y_sorted) < 2 * rotor_diameter_i)
-            * (grid.x_sorted <= downstream_influence_length + x_i)
-        )
-
-        # Combine turbine TIs with WAT
-        turbine_turbulence_intensity = np.maximum(
-            np.sqrt( ti_added ** 2 + ambient_turbulence_intensity ** 2 ),
-            turbine_turbulence_intensity
-        )
-
-        flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
-        flow_field.v_sorted += v_wake
-        flow_field.w_sorted += w_wake
-
-    flow_field.turbulence_intensity_field_sorted = turbine_turbulence_intensity
-    flow_field.turbulence_intensity_field_sorted_avg = np.mean(
-        turbine_turbulence_intensity,
-        axis=(3,4)
-    )[:, :, :, None, None]
```

### Comparing `FLORIS-3.6/floris/simulation/turbine.py` & `FLORIS-4/floris/core/turbine/turbine.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,576 +1,507 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import copy
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
+from pathlib import Path
 
 import attrs
 import numpy as np
+import pandas as pd
 from attrs import define, field
 from scipy.interpolate import interp1d
 
-from floris.simulation import BaseClass
+from floris.core import BaseClass
+from floris.core.turbine import (
+    AWCTurbine,
+    CosineLossTurbine,
+    MixedOperationTurbine,
+    SimpleDeratingTurbine,
+    SimpleTurbine,
+)
 from floris.type_dec import (
+    convert_to_path,
     floris_numeric_dict_converter,
     NDArrayBool,
     NDArrayFilter,
     NDArrayFloat,
     NDArrayInt,
     NDArrayObject,
+    NDArrayStr,
 )
 from floris.utilities import cosd
 
 
-def _rotor_velocity_yaw_correction(
-    pP: float,
-    yaw_angle: NDArrayFloat,
-    rotor_effective_velocities: NDArrayFloat,
-) -> NDArrayFloat:
-    # Compute the rotor effective velocity adjusting for yaw settings
-    pW = pP / 3.0  # Convert from pP to w
-    rotor_effective_velocities = rotor_effective_velocities * cosd(yaw_angle) ** pW
-
-    return rotor_effective_velocities
-
+TURBINE_MODEL_MAP = {
+    "operation_model": {
+        "simple": SimpleTurbine,
+        "cosine-loss": CosineLossTurbine,
+        "simple-derating": SimpleDeratingTurbine,
+        "mixed": MixedOperationTurbine,
+        "awc": AWCTurbine,
+    },
+}
 
-def _rotor_velocity_tilt_correction(
-    turbine_type_map: NDArrayObject,
-    tilt_angle: NDArrayFloat,
-    ref_tilt_cp_ct: NDArrayFloat,
-    pT: float,
-    tilt_interp: NDArrayObject,
-    correct_cp_ct_for_tilt: NDArrayBool,
-    rotor_effective_velocities: NDArrayFloat,
-) -> NDArrayFloat:
-    # Compute the tilt, if using floating turbines
-    old_tilt_angle = copy.deepcopy(tilt_angle)
-    tilt_angle = compute_tilt_angles_for_floating_turbines(
-        turbine_type_map,
-        tilt_angle,
-        tilt_interp,
-        rotor_effective_velocities,
-    )
-    # Only update tilt angle if requested (if the tilt isn't accounted for in the Cp curve)
-    tilt_angle = np.where(correct_cp_ct_for_tilt, tilt_angle, old_tilt_angle)
 
-    # Compute the rotor effective velocity adjusting for tilt
-    relative_tilt = tilt_angle - ref_tilt_cp_ct
-    rotor_effective_velocities = rotor_effective_velocities * cosd(relative_tilt) ** (pT / 3.0)
-    return rotor_effective_velocities
+def select_multidim_condition(
+    condition: dict | tuple,
+    specified_conditions: Iterable[tuple]
+) -> tuple:
+    """
+    Convert condition to the type expected by power_thrust_table and select
+    nearest specified condition
+    """
+    if type(condition) is tuple:
+        pass
+    elif type(condition) is dict:
+        condition = tuple(condition.values())
+    else:
+        raise TypeError("condition should be of type dict or tuple.")
 
+    # Find the nearest key to the specified conditions.
+    specified_conditions = np.array(specified_conditions)
 
-def compute_tilt_angles_for_floating_turbines(
-    turbine_type_map: NDArrayObject,
-    tilt_angle: NDArrayFloat,
-    tilt_interp: dict[str, interp1d],
-    rotor_effective_velocities: NDArrayFloat,
-) -> NDArrayFloat:
-    # Loop over each turbine type given to get tilt angles for all turbines
-    tilt_angles = np.zeros(np.shape(rotor_effective_velocities))
-    turb_types = np.unique(turbine_type_map)
-    for turb_type in turb_types:
-        # If no tilt interpolation is specified, assume no modification to tilt
-        if tilt_interp[turb_type] is None:
-            # TODO should this be break? Should it be continue? Do we want to support mixed
-            # fixed-bottom and floating? Or non-tilting floating?
-            pass
-        # Using a masked array, apply the tilt angle for all turbines of the current
-        # type to the main tilt angle array
-        else:
-            tilt_angles += (
-                tilt_interp[turb_type](rotor_effective_velocities)
-                * (turbine_type_map == turb_type)
-            )
-
-    # TODO: Not sure if this is the best way to do this? Basically replaces the initialized
-    # tilt_angles if there are non-zero tilt angles calculated above (meaning that the turbine
-    # definition contained  a wind_speed/tilt table definition)
-    if not tilt_angles.all() == 0.0:
-        tilt_angle = tilt_angles
+    # Find the nearest key to the specified conditions.
+    nearest_condition = np.zeros_like(condition)
+    for i, c in enumerate(condition):
+        nearest_condition[i] = (
+            specified_conditions[:, i][np.absolute(specified_conditions[:, i] - c).argmin()]
+        )
 
-    return tilt_angle
+    return tuple(nearest_condition)
 
 
-def rotor_effective_velocity(
-    air_density: float,
-    ref_density_cp_ct: float,
+def power(
     velocities: NDArrayFloat,
-    yaw_angle: NDArrayFloat,
-    tilt_angle: NDArrayFloat,
-    ref_tilt_cp_ct: NDArrayFloat,
-    pP: float,
-    pT: float,
-    tilt_interp: NDArrayObject,
-    correct_cp_ct_for_tilt: NDArrayBool,
+    air_density: float,
+    power_functions: dict[str, Callable],
+    yaw_angles: NDArrayFloat,
+    tilt_angles: NDArrayFloat,
+    power_setpoints: NDArrayFloat,
+    awc_modes: NDArrayStr,
+    awc_amplitudes: NDArrayFloat,
+    tilt_interps: dict[str, interp1d],
     turbine_type_map: NDArrayObject,
+    turbine_power_thrust_tables: dict,
     ix_filter: NDArrayInt | Iterable[int] | None = None,
     average_method: str = "cubic-mean",
-    cubature_weights: NDArrayFloat | None = None
-) -> NDArrayFloat:
-
-    if isinstance(yaw_angle, list):
-        yaw_angle = np.array(yaw_angle)
-    if isinstance(tilt_angle, list):
-        tilt_angle = np.array(tilt_angle)
-
-    # Down-select inputs if ix_filter is given
-    if ix_filter is not None:
-        velocities = velocities[:, :, ix_filter]
-        yaw_angle = yaw_angle[:, :, ix_filter]
-        tilt_angle = tilt_angle[:, :, ix_filter]
-        ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
-        pP = pP[:, :, ix_filter]
-        pT = pT[:, :, ix_filter]
-        turbine_type_map = turbine_type_map[:, :, ix_filter]
-
-    # Compute the rotor effective velocity adjusting for air density
-    # TODO: This correction is currently split across two functions: this one and `power`, where in
-    # `power` the returned power is multiplied by the reference air density
-    average_velocities = average_velocity(
-        velocities,
-        method=average_method,
-        cubature_weights=cubature_weights
-    )
-    rotor_effective_velocities = (air_density/ref_density_cp_ct)**(1/3) * average_velocities
-
-    # Compute the rotor effective velocity adjusting for yaw settings
-    rotor_effective_velocities = _rotor_velocity_yaw_correction(
-        pP, yaw_angle, rotor_effective_velocities
-    )
-
-    # Compute the tilt, if using floating turbines
-    rotor_effective_velocities = _rotor_velocity_tilt_correction(
-        turbine_type_map,
-        tilt_angle,
-        ref_tilt_cp_ct,
-        pT,
-        tilt_interp,
-        correct_cp_ct_for_tilt,
-        rotor_effective_velocities,
-    )
-
-    return rotor_effective_velocities
-
-
-def power(
-    ref_density_cp_ct: float,
-    rotor_effective_velocities: NDArrayFloat,
-    power_interp: dict[str, interp1d],
-    turbine_type_map: NDArrayObject,
-    ix_filter: NDArrayInt | Iterable[int] | None = None,
+    cubature_weights: NDArrayFloat | None = None,
+    correct_cp_ct_for_tilt: bool = False,
+    multidim_condition: tuple | None = None, # Assuming only one condition at a time?
 ) -> NDArrayFloat:
     """Power produced by a turbine adjusted for yaw and tilt. Value
     given in Watts.
 
     Args:
-        ref_density_cp_cts (NDArrayFloat[wd, ws, turbines]): The reference density for each turbine
-        rotor_effective_velocities (NDArrayFloat[wd, ws, turbines]): The rotor
-            effective velocities at a turbine.
-        power_interp (dict[str, interp1d]): A dictionary of power interpolation functions for
-            each turbine type.
+        velocities (NDArrayFloat[n_findex, n_turbines, n_grid, n_grid]): The velocities at a
+            turbine.
+        air_density (float): air density for simulation [kg/m^3]
+        power_functions (dict[str, Callable]): A dictionary of power functions for
+            each turbine type. Keys are the turbine type and values are the callable functions.
+        yaw_angles (NDArrayFloat[findex, turbines]): The yaw angle for each turbine.
+        tilt_angles (NDArrayFloat[findex, turbines]): The tilt angle for each turbine.
+        power_setpoints: (NDArrayFloat[findex, turbines]): Maximum power setpoint for each
+            turbine [W].
+        awc_modes: (NDArrayStr[findex, turbines]): awc excitation mode (currently, only "baseline"
+            and "helix" are implemented).
+        awc_modes: (NDArrayStr[findex, turbines]): awc excitation mode (currently, only "baseline"
+            and "helix" are implemented).
+        awc_amplitudes: (NDArrayFloat[findex, turbines]): awc excitation amplitude for each
+            turbine [deg].
+        tilt_interps (Iterable[tuple]): The tilt interpolation functions for each
+            turbine.
         turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition for
             each turbine.
+        turbine_power_thrust_tables: Reference data for the power and thrust representation
         ix_filter (NDArrayInt, optional): The boolean array, or
             integer indices to filter out before calculation. Defaults to None.
+        average_method (str, optional): The method for averaging over turbine rotor points
+            to determine a rotor-average wind speed. Defaults to "cubic-mean".
+        cubature_weights (NDArrayFloat | None): Weights for cubature averaging methods. Defaults to
+            None.
+        multidim_condition (tuple | None): The condition tuple used to select the appropriate
+            thrust coefficient relationship for multidimensional power/thrust tables. Defaults to
+            None.
 
     Returns:
         NDArrayFloat: The power, in Watts, for each turbine after adjusting for yaw and tilt.
     """
-    # TODO: Change the order of input arguments to be consistent with the other
-    # utility functions - velocities first...
-    # Update to power calculation which replaces the fixed pP exponent with
-    # an exponent pW, that changes the effective wind speed input to the power
-    # calculation, rather than scaling the power.  This better handles power
-    # loss to yaw in above rated conditions
-    #
-    # based on the paper "Optimising yaw control at wind farm level" by
-    # Ervin Bossanyi
-
-    # TODO: check this - where is it?
-    # P = 1/2 rho A V^3 Cp
 
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        rotor_effective_velocities = rotor_effective_velocities[:, :, ix_filter]
-        turbine_type_map = turbine_type_map[:, :, ix_filter]
+        velocities = velocities[:, ix_filter]
+        yaw_angles = yaw_angles[:, ix_filter]
+        tilt_angles = tilt_angles[:, ix_filter]
+        power_setpoints = power_setpoints[:, ix_filter]
+        awc_modes = awc_modes[:, ix_filter]
+        awc_amplitudes = awc_amplitudes[:, ix_filter]
+        turbine_type_map = turbine_type_map[:, ix_filter]
+        if type(correct_cp_ct_for_tilt) is bool:
+            pass
+        else:
+            correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, ix_filter]
 
     # Loop over each turbine type given to get power for all turbines
-    p = np.zeros(np.shape(rotor_effective_velocities))
+    p = np.zeros(np.shape(velocities)[0:2])
     turb_types = np.unique(turbine_type_map)
     for turb_type in turb_types:
-        # Using a masked array, apply the thrust coefficient for all turbines of the current
-        # type to the main thrust coefficient array
-        p += power_interp[turb_type](rotor_effective_velocities) * (turbine_type_map == turb_type)
+        # Handle possible multidimensional power thrust tables
+        if "power" in turbine_power_thrust_tables[turb_type]: # normal
+            power_thrust_table = turbine_power_thrust_tables[turb_type]
+        else: # assumed multidimensional, use multidim lookup
+            # Currently, only works for single mutlidim condition. May need to
+            # loop in the case where there are multiple conditions.
+            multidim_condition = select_multidim_condition(
+                multidim_condition,
+                list(turbine_power_thrust_tables[turb_type].keys())
+            )
+            power_thrust_table = turbine_power_thrust_tables[turb_type][multidim_condition]
+
+        # Construct full set of possible keyword arguments for power()
+        power_model_kwargs = {
+            "power_thrust_table": power_thrust_table,
+            "velocities": velocities,
+            "air_density": air_density,
+            "yaw_angles": yaw_angles,
+            "tilt_angles": tilt_angles,
+            "power_setpoints": power_setpoints,
+            "awc_modes": awc_modes,
+            "awc_amplitudes": awc_amplitudes,
+            "tilt_interp": tilt_interps[turb_type],
+            "average_method": average_method,
+            "cubature_weights": cubature_weights,
+            "correct_cp_ct_for_tilt": correct_cp_ct_for_tilt,
+        }
+
+        # Using a masked array, apply the power for all turbines of the current
+        # type to the main power
+        p += power_functions[turb_type](**power_model_kwargs) * (turbine_type_map == turb_type)
 
-    return p * ref_density_cp_ct
+    return p
 
 
-def Ct(
+def thrust_coefficient(
     velocities: NDArrayFloat,
-    yaw_angle: NDArrayFloat,
-    tilt_angle: NDArrayFloat,
-    ref_tilt_cp_ct: NDArrayFloat,
-    fCt: dict,
-    tilt_interp: NDArrayObject,
+    air_density: float,
+    yaw_angles: NDArrayFloat,
+    tilt_angles: NDArrayFloat,
+    power_setpoints: NDArrayFloat,
+    awc_modes: NDArrayStr,
+    awc_amplitudes: NDArrayFloat,
+    thrust_coefficient_functions: dict[str, Callable],
+    tilt_interps: dict[str, interp1d],
     correct_cp_ct_for_tilt: NDArrayBool,
     turbine_type_map: NDArrayObject,
+    turbine_power_thrust_tables: dict,
     ix_filter: NDArrayFilter | Iterable[int] | None = None,
     average_method: str = "cubic-mean",
-    cubature_weights: NDArrayFloat | None = None
+    cubature_weights: NDArrayFloat | None = None,
+    multidim_condition: tuple | None = None, # Assuming only one condition at a time?
 ) -> NDArrayFloat:
 
-    """Thrust coefficient of a turbine incorporating the yaw angle.
-    The value is interpolated from the coefficient of thrust vs
-    wind speed table using the rotor swept area average velocity.
+    """Thrust coefficient of a turbine.
+    The value is obtained from the coefficient of thrust specified by the callables specified
+    in the thrust_coefficient_functions.
 
     Args:
-        velocities (NDArrayFloat[wd, ws, turbines, grid1, grid2]): The velocity field at
+        velocities (NDArrayFloat[findex, turbines, grid1, grid2]): The velocity field at
             a turbine.
-        yaw_angle (NDArrayFloat[wd, ws, turbines]): The yaw angle for each turbine.
-        tilt_angle (NDArrayFloat[wd, ws, turbines]): The tilt angle for each turbine.
-        ref_tilt_cp_ct (NDArrayFloat[wd, ws, turbines]): The reference tilt angle for each turbine
-            that the Cp/Ct tables are defined at.
-        fCt (dict): The thrust coefficient interpolation functions for each turbine. Keys are
-            the turbine type string and values are the interpolation functions.
-        tilt_interp (Iterable[tuple]): The tilt interpolation functions for each
+        air_density (float): air density for simulation [kg/m^3]
+        yaw_angles (NDArrayFloat[findex, turbines]): The yaw angle for each turbine.
+        tilt_angles (NDArrayFloat[findex, turbines]): The tilt angle for each turbine.
+        power_setpoints: (NDArrayFloat[findex, turbines]): Maximum power setpoint for each
+            turbine [W].
+        awc_modes: (NDArrayStr[findex, turbines]): awc excitation mode (currently, only "baseline"
+            and "helix" are implemented).
+        awc_amplitudes: (NDArrayFloat[findex, turbines]): awc excitation amplitude for each
+            turbine [deg].
+        thrust_coefficient_functions (dict): The thrust coefficient functions for each turbine. Keys
+            are the turbine type string and values are the callable functions.
+        tilt_interps (Iterable[tuple]): The tilt interpolation functions for each
             turbine.
-        correct_cp_ct_for_tilt (NDArrayBool[wd, ws, turbines]): Boolean for determining if the
+        correct_cp_ct_for_tilt (NDArrayBool[findex, turbines]): Boolean for determining if the
             turbines Cp and Ct should be corrected for tilt.
-        turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition
+        turbine_type_map: (NDArrayObject[findex, turbines]): The Turbine type definition
             for each turbine.
         ix_filter (NDArrayFilter | Iterable[int] | None, optional): The boolean array, or
             integer indices as an iterable of array to filter out before calculation.
             Defaults to None.
+        average_method (str, optional): The method for averaging over turbine rotor points
+            to determine a rotor-average wind speed. Defaults to "cubic-mean".
+        cubature_weights (NDArrayFloat | None): Weights for cubature averaging methods. Defaults to
+            None.
+        multidim_condition (tuple | None): The condition tuple used to select the appropriate
+            thrust coefficient relationship for multidimensional power/thrust tables. Defaults to
+            None.
 
     Returns:
         NDArrayFloat: Coefficient of thrust for each requested turbine.
     """
 
-    if isinstance(yaw_angle, list):
-        yaw_angle = np.array(yaw_angle)
-
-    if isinstance(tilt_angle, list):
-        tilt_angle = np.array(tilt_angle)
-
     # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        velocities = velocities[:, :, ix_filter]
-        yaw_angle = yaw_angle[:, :, ix_filter]
-        tilt_angle = tilt_angle[:, :, ix_filter]
-        ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
-        turbine_type_map = turbine_type_map[:, :, ix_filter]
-        correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, :, ix_filter]
-
-    average_velocities = average_velocity(
-        velocities,
-        method=average_method,
-        cubature_weights=cubature_weights
-    )
-
-    # Compute the tilt, if using floating turbines
-    old_tilt_angle = copy.deepcopy(tilt_angle)
-    tilt_angle = compute_tilt_angles_for_floating_turbines(
-        turbine_type_map,
-        tilt_angle,
-        tilt_interp,
-        average_velocities,
-    )
-    # Only update tilt angle if requested (if the tilt isn't accounted for in the Ct curve)
-    tilt_angle = np.where(correct_cp_ct_for_tilt, tilt_angle, old_tilt_angle)
+        velocities = velocities[:, ix_filter]
+        yaw_angles = yaw_angles[:, ix_filter]
+        tilt_angles = tilt_angles[:, ix_filter]
+        power_setpoints = power_setpoints[:, ix_filter]
+        awc_modes = awc_modes[:, ix_filter]
+        awc_amplitudes = awc_amplitudes[:, ix_filter]
+        turbine_type_map = turbine_type_map[:, ix_filter]
+        if type(correct_cp_ct_for_tilt) is bool:
+            pass
+        else:
+            correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, ix_filter]
 
     # Loop over each turbine type given to get thrust coefficient for all turbines
-    thrust_coefficient = np.zeros(np.shape(average_velocities))
+    thrust_coefficient = np.zeros(np.shape(velocities)[0:2])
     turb_types = np.unique(turbine_type_map)
     for turb_type in turb_types:
+        # Handle possible multidimensional power thrust tables
+        if "thrust_coefficient" in turbine_power_thrust_tables[turb_type]: # normal
+            power_thrust_table = turbine_power_thrust_tables[turb_type]
+        else: # assumed multidimensional, use multidim lookup
+            # Currently, only works for single mutlidim condition. May need to
+            # loop in the case where there are multiple conditions.
+            multidim_condition = select_multidim_condition(
+                multidim_condition,
+                list(turbine_power_thrust_tables[turb_type].keys())
+            )
+            power_thrust_table = turbine_power_thrust_tables[turb_type][multidim_condition]
+
+        # Construct full set of possible keyword arguments for thrust_coefficient()
+        thrust_model_kwargs = {
+            "power_thrust_table": power_thrust_table,
+            "velocities": velocities,
+            "air_density": air_density,
+            "yaw_angles": yaw_angles,
+            "tilt_angles": tilt_angles,
+            "power_setpoints": power_setpoints,
+            "awc_modes": awc_modes,
+            "awc_amplitudes": awc_amplitudes,
+            "tilt_interp": tilt_interps[turb_type],
+            "average_method": average_method,
+            "cubature_weights": cubature_weights,
+            "correct_cp_ct_for_tilt": correct_cp_ct_for_tilt,
+        }
+
         # Using a masked array, apply the thrust coefficient for all turbines of the current
         # type to the main thrust coefficient array
         thrust_coefficient += (
-            fCt[turb_type](average_velocities)
+            thrust_coefficient_functions[turb_type](**thrust_model_kwargs)
             * (turbine_type_map == turb_type)
         )
-    thrust_coefficient = np.clip(thrust_coefficient, 0.0001, 0.9999)
-    effective_thrust = thrust_coefficient * cosd(yaw_angle) * cosd(tilt_angle - ref_tilt_cp_ct)
-    return effective_thrust
+
+    return thrust_coefficient
 
 
 def axial_induction(
-    velocities: NDArrayFloat,  # (wind directions, wind speeds, turbines, grid, grid)
-    yaw_angle: NDArrayFloat,  # (wind directions, wind speeds, turbines)
-    tilt_angle: NDArrayFloat,  # (wind directions, wind speeds, turbines)
-    ref_tilt_cp_ct: NDArrayFloat,
-    fCt: dict,  # (turbines)
-    tilt_interp: NDArrayObject,  # (turbines)
-    correct_cp_ct_for_tilt: NDArrayBool, # (wind directions, wind speeds, turbines)
-    turbine_type_map: NDArrayObject, # (wind directions, 1, turbines)
+    velocities: NDArrayFloat,
+    air_density: float,
+    yaw_angles: NDArrayFloat,
+    tilt_angles: NDArrayFloat,
+    power_setpoints: NDArrayFloat,
+    awc_modes: NDArrayStr,
+    awc_amplitudes: NDArrayFloat,
+    axial_induction_functions: dict,
+    tilt_interps: NDArrayObject,
+    correct_cp_ct_for_tilt: NDArrayBool,
+    turbine_type_map: NDArrayObject,
+    turbine_power_thrust_tables: dict,
     ix_filter: NDArrayFilter | Iterable[int] | None = None,
     average_method: str = "cubic-mean",
-    cubature_weights: NDArrayFloat | None = None
+    cubature_weights: NDArrayFloat | None = None,
+    multidim_condition: tuple | None = None, # Assuming only one condition at a time?
 ) -> NDArrayFloat:
     """Axial induction factor of the turbine incorporating
     the thrust coefficient and yaw angle.
 
     Args:
         velocities (NDArrayFloat): The velocity field at each turbine; should be shape:
             (number of turbines, ngrid, ngrid), or (ngrid, ngrid) for a single turbine.
-        yaw_angle (NDArrayFloat[wd, ws, turbines]): The yaw angle for each turbine.
-        tilt_angle (NDArrayFloat[wd, ws, turbines]): The tilt angle for each turbine.
-        ref_tilt_cp_ct (NDArrayFloat[wd, ws, turbines]): The reference tilt angle for each turbine
-            that the Cp/Ct tables are defined at.
-        fCt (dict): The thrust coefficient interpolation functions for each turbine. Keys are
-            the turbine type string and values are the interpolation functions.
-        tilt_interp (Iterable[tuple]): The tilt interpolation functions for each
+        yaw_angles (NDArrayFloat[findex, turbines]): The yaw angle for each turbine.
+        tilt_angles (NDArrayFloat[findex, turbines]): The tilt angle for each turbine.
+        power_setpoints: (NDArrayFloat[findex, turbines]): Maximum power setpoint for each
+            turbine [W].
+        awc_amplitudes: (NDArrayFloat[findex, turbines]): awc excitation amplitude for each
+            turbine [deg].
+        axial_induction_functions (dict): The axial induction functions for each turbine. Keys are
+            the turbine type string and values are the callable functions.
+        tilt_interps (Iterable[tuple]): The tilt interpolation functions for each
             turbine.
-        correct_cp_ct_for_tilt (NDArrayBool[wd, ws, turbines]): Boolean for determining if the
+        correct_cp_ct_for_tilt (NDArrayBool[findex, turbines]): Boolean for determining if the
             turbines Cp and Ct should be corrected for tilt.
-        turbine_type_map: (NDArrayObject[wd, ws, turbines]): The Turbine type definition
+        turbine_type_map: (NDArrayObject[findex, turbines]): The Turbine type definition
             for each turbine.
         ix_filter (NDArrayFilter | Iterable[int] | None, optional): The boolean array, or
             integer indices (as an array or iterable) to filter out before calculation.
             Defaults to None.
+        average_method (str, optional): The method for averaging over turbine rotor points
+            to determine a rotor-average wind speed. Defaults to "cubic-mean".
+        cubature_weights (NDArrayFloat | None): Weights for cubature averaging methods. Defaults to
+            None.
+        multidim_condition (tuple | None): The condition tuple used to select the appropriate
+            thrust coefficient relationship for multidimensional power/thrust tables. Defaults to
+            None.
 
     Returns:
         Union[float, NDArrayFloat]: [description]
     """
 
-    if isinstance(yaw_angle, list):
-        yaw_angle = np.array(yaw_angle)
-
-    # TODO: Should the tilt_angle used for the return calculation be modified the same as the
-    # tilt_angle in Ct, if the user has supplied a tilt/wind_speed table?
-    if isinstance(tilt_angle, list):
-        tilt_angle = np.array(tilt_angle)
-
-    # Get Ct first before modifying any data
-    thrust_coefficient = Ct(
-        velocities,
-        yaw_angle,
-        tilt_angle,
-        ref_tilt_cp_ct,
-        fCt,
-        tilt_interp,
-        correct_cp_ct_for_tilt,
-        turbine_type_map,
-        ix_filter,
-        average_method,
-        cubature_weights
-    )
-
-    # Then, process the input arguments as needed for this function
+    # Down-select inputs if ix_filter is given
     if ix_filter is not None:
-        yaw_angle = yaw_angle[:, :, ix_filter]
-        tilt_angle = tilt_angle[:, :, ix_filter]
-        ref_tilt_cp_ct = ref_tilt_cp_ct[:, :, ix_filter]
-
-    return (
-        0.5
-        / (cosd(yaw_angle)
-        * cosd(tilt_angle - ref_tilt_cp_ct))
-        * (
-            1 - np.sqrt(
-                1 - thrust_coefficient * cosd(yaw_angle) * cosd(tilt_angle - ref_tilt_cp_ct)
-            )
-        )
-    )
-
-
-def simple_mean(array, axis=0):
-    return np.mean(array, axis=axis)
-
-def cubic_mean(array, axis=0):
-    return np.cbrt(np.mean(array ** 3.0, axis=axis))
-
-def simple_cubature(array, cubature_weights, axis=0):
-    weights = cubature_weights.flatten()
-    weights = weights * len(weights) / np.sum(weights)
-    product = (array * weights[None, None, None, :, None])
-    return simple_mean(product, axis)
-
-def cubic_cubature(array, cubature_weights, axis=0):
-    weights = cubature_weights.flatten()
-    weights = weights * len(weights) / np.sum(weights)
-    return np.cbrt(np.mean((array**3.0 * weights[None, None, None, :, None]), axis=axis))
-
-def average_velocity(
-    velocities: NDArrayFloat,
-    ix_filter: NDArrayFilter | Iterable[int] | None = None,
-    method: str = "cubic-mean",
-    cubature_weights: NDArrayFloat | None = None
-) -> NDArrayFloat:
-    """This property calculates and returns the cube root of the
-    mean cubed velocity in the turbine's rotor swept area (m/s).
-
-    **Note:** The velocity is scaled to an effective velocity by the yaw.
-
-    Args:
-        velocities (NDArrayFloat): The velocity field at each turbine; should be shape:
-            (number of turbines, ngrid, ngrid), or (ngrid, ngrid) for a single turbine.
-        ix_filter (NDArrayFilter | Iterable[int] | None], optional): The boolean array, or
-            integer indices (as an iterable or array) to filter out before calculation.
-            Defaults to None.
+        velocities = velocities[:, ix_filter]
+        yaw_angles = yaw_angles[:, ix_filter]
+        tilt_angles = tilt_angles[:, ix_filter]
+        power_setpoints = power_setpoints[:, ix_filter]
+        awc_modes = awc_modes[:, ix_filter]
+        awc_amplitudes = awc_amplitudes[:, ix_filter]
+        turbine_type_map = turbine_type_map[:, ix_filter]
+        if type(correct_cp_ct_for_tilt) is bool:
+            pass
+        else:
+            correct_cp_ct_for_tilt = correct_cp_ct_for_tilt[:, ix_filter]
 
-    Returns:
-        NDArrayFloat: The average velocity across the rotor(s).
-    """
+    # Loop over each turbine type given to get axial induction for all turbines
+    axial_induction = np.zeros(np.shape(velocities)[0:2])
+    turb_types = np.unique(turbine_type_map)
+    for turb_type in turb_types:
+        # Handle possible multidimensional power thrust tables
+        if "thrust_coefficient" in turbine_power_thrust_tables[turb_type]: # normal
+            power_thrust_table = turbine_power_thrust_tables[turb_type]
+        else: # assumed multidimensional, use multidim lookup
+            # Currently, only works for single mutlidim condition. May need to
+            # loop in the case where there are multiple conditions.
+            multidim_condition = select_multidim_condition(
+                multidim_condition,
+                list(turbine_power_thrust_tables[turb_type].keys())
+            )
+            power_thrust_table = turbine_power_thrust_tables[turb_type][multidim_condition]
 
-    # The input velocities are expected to be a 5 dimensional array with shape:
-    # (# wind directions, # wind speeds, # turbines, grid resolution, grid resolution)
+        # Construct full set of possible keyword arguments for thrust_coefficient()
+        axial_induction_model_kwargs = {
+            "power_thrust_table": power_thrust_table,
+            "velocities": velocities,
+            "air_density": air_density,
+            "yaw_angles": yaw_angles,
+            "tilt_angles": tilt_angles,
+            "power_setpoints": power_setpoints,
+            "awc_modes": awc_modes,
+            "awc_amplitudes": awc_amplitudes,
+            "tilt_interp": tilt_interps[turb_type],
+            "average_method": average_method,
+            "cubature_weights": cubature_weights,
+            "correct_cp_ct_for_tilt": correct_cp_ct_for_tilt,
+        }
 
-    if ix_filter is not None:
-        velocities = velocities[:, :, ix_filter]
+        # Using a masked array, apply the thrust coefficient for all turbines of the current
+        # type to the main thrust coefficient array
+        axial_induction += (
+            axial_induction_functions[turb_type](**axial_induction_model_kwargs)
+            * (turbine_type_map == turb_type)
+        )
 
-    axis = tuple([3 + i for i in range(velocities.ndim - 3)])
-    if method == "simple-mean":
-        return simple_mean(velocities, axis)
-
-    elif method == "cubic-mean":
-        return cubic_mean(velocities, axis)
-
-    elif method == "simple-cubature":
-        if cubature_weights is None:
-            raise ValueError("cubature_weights is required for 'simple-cubature' method.")
-        return simple_cubature(velocities, cubature_weights, axis)
-
-    elif method == "cubic-cubature":
-        if cubature_weights is None:
-            raise ValueError("cubature_weights is required for 'cubic-cubature' method.")
-        return cubic_cubature(velocities, cubature_weights, axis)
+    return axial_induction
 
-    else:
-        raise ValueError("Incorrect method given.")
 
 @define
 class Turbine(BaseClass):
     """
     A class containing the parameters and infrastructure to model a wind turbine's performance
     for a particular atmospheric condition.
 
     Args:
         turbine_type (str): An identifier for this type of turbine such as "NREL_5MW".
         rotor_diameter (float): The rotor diameter in meters.
         hub_height (float): The hub height in meters.
-        pP (float): The cosine exponent relating the yaw misalignment angle to turbine power.
-        pT (float): The cosine exponent relating the rotor tilt angle to turbine power.
         TSR (float): The Tip Speed Ratio of the turbine.
-        generator_efficiency (float): The efficiency of the generator used to scale
-            power production.
-        ref_density_cp_ct (float): The density at which the provided Cp and Ct curves are defined.
-        ref_tilt_cp_ct (float): The implicit tilt of the turbine for which the Cp and Ct
-            curves are defined. This is typically the nacelle tilt.
         power_thrust_table (dict[str, float]): Contains power coefficient and thrust coefficient
             values at a series of wind speeds to define the turbine performance.
             The dictionary must have the following three keys with equal length values:
                 {
                     "wind_speeds": List[float],
                     "power": List[float],
                     "thrust": List[float],
                 }
+            or, contain a key "power_thrust_data_file" pointing to the power/thrust data.
+            Optionally, power_thrust_table may include parameters for use in the turbine submodel,
+            for example:
+                cosine_loss_exponent_yaw (float): The cosine exponent relating the yaw misalignment
+                    angle to turbine power.
+                cosine_loss_exponent_tilt (float): The cosine exponent relating the rotor tilt angle
+                    to turbine power.
+                ref_air_density (float): The density at which the provided Cp and Ct curves are
+                    defined.
+                ref_tilt (float): The implicit tilt of the turbine for which the Cp and Ct
+                    curves are defined. This is typically the nacelle tilt.
         correct_cp_ct_for_tilt (bool): A flag to indicate whether to correct Cp and Ct for tilt
             usually for a floating turbine.
             Optional, defaults to False.
         floating_tilt_table (dict[str, float]): Look up table of tilt angles at a series of
             wind speeds. The dictionary must have the following keys with equal length values:
                 {
                     "wind_speeds": List[float],
                     "tilt": List[float],
                 }
             Required if `correct_cp_ct_for_tilt = True`. Defaults to None.
+        multi_dimensional_cp_ct (bool): Use a multidimensional power_thrust_table. Defaults to
+            False.
     """
     turbine_type: str = field()
     rotor_diameter: float = field()
     hub_height: float = field()
-    pP: float = field()
-    pT: float = field()
     TSR: float = field()
-    generator_efficiency: float = field()
-    ref_density_cp_ct: float = field()
-    ref_tilt_cp_ct: float = field()
-    power_thrust_table: dict[str, NDArrayFloat] = field(converter=floris_numeric_dict_converter)
+    power_thrust_table: dict = field(default={}) # conversion to numpy in __post_init__
+    operation_model: str = field(default="cosine-loss")
 
     correct_cp_ct_for_tilt: bool = field(default=False)
     floating_tilt_table: dict[str, NDArrayFloat] | None = field(default=None)
 
     # Even though this Turbine class does not support the multidimensional features as they
     # are implemented in TurbineMultiDim, providing the following two attributes here allows
     # the turbine data inputs to keep the multidimensional Cp and Ct curve but switch them off
     # with multi_dimensional_cp_ct = False
     multi_dimensional_cp_ct: bool = field(default=False)
-    power_thrust_data_file: str = field(default=None)
 
     # Initialized in the post_init function
     rotor_radius: float = field(init=False)
     rotor_area: float = field(init=False)
-    fCt_interp: interp1d = field(init=False)
-    power_interp: interp1d = field(init=False)
+    thrust_coefficient_function: Callable = field(init=False)
+    axial_induction_function: Callable = field(init=False)
+    power_function: Callable = field(init=False)
     tilt_interp: interp1d = field(init=False, default=None)
+    power_thrust_data_file: str = field(default=None)
+
+    # Only used by mutlidimensional turbines
+    turbine_library_path: Path = field(
+        default=Path(__file__).parents[2] / "turbine_library",
+        converter=convert_to_path,
+        validator=attrs.validators.instance_of(Path)
+    )
+
+    # Not to be provided by the user
+    condition_keys: list[str] = field(init=False, factory=list)
 
     def __attrs_post_init__(self) -> None:
-        self._initialize_power_thrust_interpolation()
+        self._initialize_power_thrust_functions()
         self.__post_init__()
 
     def __post_init__(self) -> None:
         self._initialize_tilt_interpolation()
+        if self.multi_dimensional_cp_ct:
+            self._initialize_multidim_power_thrust_table()
+        else:
+            self.power_thrust_table = floris_numeric_dict_converter(self.power_thrust_table)
 
-    def _initialize_power_thrust_interpolation(self) -> None:
-        # TODO This validation for the power thrust tables should go in the turbine library
-        # since it's preprocessing
-        # Remove any duplicate wind speed entries
-        # _, duplicate_filter = np.unique(self.wind_speed, return_index=True)
-        # self.power = self.power[duplicate_filter]
-        # self.thrust = self.thrust[duplicate_filter]
-        # self.wind_speed = self.wind_speed[duplicate_filter]
-
-        wind_speeds = self.power_thrust_table["wind_speed"]
-        cp_interp = interp1d(
-            wind_speeds,
-            self.power_thrust_table["power"],
-            fill_value=(0.0, 1.0),
-            bounds_error=False,
-        )
-        self.power_interp = interp1d(
-            wind_speeds,
-            (
-                0.5 * self.rotor_area
-                * cp_interp(wind_speeds)
-                * self.generator_efficiency
-                * wind_speeds ** 3
-            ),
-            bounds_error=False,
-            fill_value=0
-        )
-
-        """
-        Given an array of wind speeds, this function returns an array of the
-        interpolated thrust coefficients from the power / thrust table used
-        to define the Turbine. The values are bound by the range of the input
-        values. Any requested wind speeds outside of the range of input wind
-        speeds are assigned Ct of 0.0001 or 0.9999.
+    def _initialize_power_thrust_functions(self) -> None:
+        turbine_function_model = TURBINE_MODEL_MAP["operation_model"][self.operation_model]
+        self.thrust_coefficient_function = turbine_function_model.thrust_coefficient
+        self.axial_induction_function = turbine_function_model.axial_induction
+        self.power_function = turbine_function_model.power
 
-        The fill_value arguments sets (upper, lower) bounds for any values
-        outside of the input range.
-        """
-        self.fCt_interp = interp1d(
-            wind_speeds,
-            self.power_thrust_table["thrust"],
-            fill_value=(0.0001, 0.9999),
-            bounds_error=False,
-        )
 
     def _initialize_tilt_interpolation(self) -> None:
         # TODO:
         # Remove any duplicate wind speed entries
         # _, duplicate_filter = np.unique(self.wind_speeds, return_index=True)
         # self.tilt = self.tilt[duplicate_filter]
         # self.wind_speeds = self.wind_speeds[duplicate_filter]
@@ -585,38 +516,82 @@
             self.tilt_interp = interp1d(
                 self.floating_tilt_table["wind_speed"],
                 self.floating_tilt_table["tilt"],
                 fill_value=(0.0, self.floating_tilt_table["tilt"][-1]),
                 bounds_error=False,
             )
 
+    def _initialize_multidim_power_thrust_table(self):
+        # Collect reference information
+        power_thrust_table_ref = copy.deepcopy(self.power_thrust_table)
+        self.power_thrust_data_file = power_thrust_table_ref.pop("power_thrust_data_file")
+
+        # Solidify the data file path and name
+        self.power_thrust_data_file = self.turbine_library_path / self.power_thrust_data_file
+
+        # Read in the multi-dimensional data supplied by the user.
+        df = pd.read_csv(self.power_thrust_data_file)
+
+        # Down-select the DataFrame to have just the ws, Cp, and Ct values
+        index_col = df.columns.values[:-3]
+        self.condition_keys = index_col.tolist()
+        df2 = df.set_index(index_col.tolist())
+
+        # Loop over the multi-dimensional keys to get the correct ws/Cp/Ct data to make
+        # the thrust_coefficient and power interpolants.
+        power_thrust_table_ = {} # Reset
+        for key in df2.index.unique():
+            # Select the correct ws/Cp/Ct data
+            data = df2.loc[key]
+
+            # Build the interpolants
+            power_thrust_table_.update(
+                {
+                    key: {
+                        "wind_speed": data['ws'].values,
+                        "power": data['power'].values,
+                        "thrust_coefficient": data['thrust_coefficient'].values,
+                        **power_thrust_table_ref
+                    },
+                }
+            )
+            # Add reference information at the lower level
+
+        # Set on-object version
+        self.power_thrust_table = power_thrust_table_
+
     @power_thrust_table.validator
     def check_power_thrust_table(self, instance: attrs.Attribute, value: dict) -> None:
         """
         Verify that the power and thrust tables are given with arrays of equal length
         to the wind speed array.
         """
-        if len(value.keys()) != 3 or set(value.keys()) != {"wind_speed", "power", "thrust"}:
+
+        if self.multi_dimensional_cp_ct:
+            if isinstance(list(value.keys())[0], tuple):
+                value = list(value.values())[0] # Check the first entry of multidim
+            elif "power_thrust_data_file" in value.keys():
+                return None
+            else:
+                raise ValueError(
+                    "power_thrust_data_file must be defined if multi_dimensional_cp_ct is True."
+                )
+
+        if not {"wind_speed", "power", "thrust_coefficient"} <= set(value.keys()):
             raise ValueError(
                 """
-                power_thrust_table dictionary must have the form:
+                power_thrust_table dictionary must contain:
                     {
                         "wind_speed": List[float],
                         "power": List[float],
-                        "thrust": List[float],
+                        "thrust_coefficient": List[float],
                     }
                 """
             )
 
-        if any(e.ndim > 1 for e in (value["power"], value["thrust"], value["wind_speed"])):
-            raise ValueError("power, thrust, and wind_speed inputs must be 1-D.")
-
-        if len( {value["power"].size, value["thrust"].size, value["wind_speed"].size} ) > 1:
-            raise ValueError("power, thrust, and wind_speed tables must be the same size.")
-
     @rotor_diameter.validator
     def reset_rotor_diameter_dependencies(self, instance: attrs.Attribute, value: float) -> None:
         """Resets the `rotor_radius` and `rotor_area` attributes."""
         # Temporarily turn off validators to avoid infinite recursion
         with attrs.validators.disabled():
             # Reset the values
             self.rotor_radius = value / 2.0
```

### Comparing `FLORIS-3.6/floris/simulation/wake.py` & `FLORIS-4/floris/core/wake.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 import attrs
 from attrs import define, field
 
-from floris.simulation import BaseClass, BaseModel
-from floris.simulation.wake_combination import (
+from floris.core import BaseClass, BaseModel
+from floris.core.wake_combination import (
     FLS,
     MAX,
     SOSFS,
 )
-from floris.simulation.wake_deflection import (
+from floris.core.wake_deflection import (
     EmpiricalGaussVelocityDeflection,
     GaussVelocityDeflection,
     JimenezVelocityDeflection,
     NoneVelocityDeflection,
 )
-from floris.simulation.wake_turbulence import (
+from floris.core.wake_turbulence import (
     CrespoHernandez,
     NoneWakeTurbulence,
     WakeInducedMixing,
 )
-from floris.simulation.wake_velocity import (
+from floris.core.wake_velocity import (
     CumulativeGaussCurlVelocityDeficit,
     EmpiricalGaussVelocityDeficit,
     GaussVelocityDeficit,
     JensenVelocityDeficit,
     NoneVelocityDeficit,
     TurbOParkVelocityDeficit,
 )
@@ -62,15 +49,14 @@
     "velocity_model": {
         "none": NoneVelocityDeficit,
         "cc": CumulativeGaussCurlVelocityDeficit,
         "gauss": GaussVelocityDeficit,
         "jensen": JensenVelocityDeficit,
         "turbopark": TurbOParkVelocityDeficit,
         "empirical_gauss": EmpiricalGaussVelocityDeficit,
-        "multidim_cp_ct": GaussVelocityDeficit
     },
 }
 
 
 @define
 class WakeModelManager(BaseClass):
     """
@@ -83,14 +69,15 @@
             - turbulence_model (str): The name of the turbulence model to be instantiated.
             - deflection_model (str): The name of the deflection model to be instantiated.
             - combination_model (str): The name of the combination model to be instantiated.
     """
     model_strings: dict = field(converter=dict)
     enable_secondary_steering: bool = field(converter=bool)
     enable_yaw_added_recovery: bool = field(converter=bool)
+    enable_active_wake_mixing: bool = field(converter=bool)
     enable_transverse_velocities: bool = field(converter=bool)
 
     wake_deflection_parameters: dict = field(converter=dict)
     wake_turbulence_parameters: dict = field(converter=dict)
     wake_velocity_parameters: dict = field(converter=dict, factory=dict)
 
     combination_model: BaseModel = field(init=False)
```

### Comparing `FLORIS-3.6/floris/simulation/wake_combination/sosfs.py` & `FLORIS-4/floris/core/wake_combination/max.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 import numpy as np
 from attrs import define
 
-from floris.simulation import BaseModel
+from floris.core import BaseModel
 
 
 @define
-class SOSFS(BaseModel):
+class MAX(BaseModel):
     """
-    SOSFS uses sum of squares freestream superposition to combine the
-    wake velocity deficits to the base flow field.
+    MAX uses the maximum wake velocity deficit to add to the
+    base flow field. For more information, refer to
+    :cite:`max-gunn2016limitations`.
+
+    References:
+        .. bibliography:: /references.bib
+            :style: unsrt
+            :filter: docname in docnames
+            :keyprefix: max-
     """
 
     def prepare_function(self) -> dict:
         pass
 
     def function(self, wake_field: np.ndarray, velocity_field: np.ndarray):
         """
-        Combines the base flow field with the velocity deficits
-        using sum of squares.
+        Incorporates the velocity deficits into the base flow field by
+        selecting the maximum of the two for each point.
 
         Args:
             u_field (np.array): The base flow field.
             u_wake (np.array): The wake to apply to the base flow field.
 
         Returns:
             np.array: The resulting flow field after applying the wake to the
                 base.
         """
-        return np.hypot(wake_field, velocity_field)
+        return np.maximum(wake_field, velocity_field)
```

### Comparing `FLORIS-3.6/floris/simulation/wake_deflection/empirical_gauss.py` & `FLORIS-4/floris/core/wake_deflection/empirical_gauss.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import cosd, sind
@@ -56,15 +45,15 @@
     References:
         .. bibliography:: /references.bib
             :style: unsrt
             :filter: docname in docnames
     """
     horizontal_deflection_gain_D: float = field(default=3.0)
     vertical_deflection_gain_D: float = field(default=-1)
-    deflection_rate: float = field(default=30)
+    deflection_rate: float = field(default=22)
     mixing_gain_deflection: float = field(default=0.0)
     yaw_added_mixing_gain: float = field(default=0.0)
 
     def prepare_function(
         self,
         grid: Grid,
         flow_field: FlowField,
@@ -141,12 +130,12 @@
 def yaw_added_wake_mixing(
     axial_induction_i,
     yaw_angle_i,
     downstream_distance_D_i,
     yaw_added_mixing_gain
 ):
     return (
-        axial_induction_i[:,:,:,0,0]
+        axial_induction_i[:,:,0,0]
         * yaw_added_mixing_gain
-        * (1 - cosd(yaw_angle_i[:,:,:,0,0]))
+        * (1 - cosd(yaw_angle_i[:,:,0,0]))
         / downstream_distance_D_i**2
     )
```

### Comparing `FLORIS-3.6/floris/simulation/wake_deflection/gauss.py` & `FLORIS-4/floris/core/wake_deflection/gauss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from __future__ import annotations
 
 from typing import Any
 
 import numexpr as ne
 import numpy as np
 from attrs import (
     define,
     field,
     fields,
 )
 from numpy import pi
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import cosd, sind
@@ -126,15 +115,20 @@
     ):
         """
         Calculates the deflection field of the wake. See
         :cite:`gdm-bastankhah2016experimental` and :cite:`gdm-King2019Controls`
         for details on the methods used.
 
         Args:
-            # TODO
+            x_i (np.array): x-coordinates of turbine i.
+            y_i (np.array): y-coordinates of turbine i.
+            yaw_i (np.array): Yaw angle of turbine i.
+            turbulence_intensity_i (np.array): Turbulence intensity at turbine i.
+            ct_i (np.array): Thrust coefficient of turbine i.
+            rotor_diameter_i (float): Rotor diameter of turbine i.
 
         Returns:
             np.array: Deflection field for the wake.
         """
         # ==============================================================
 
         # Opposite sign convention in this model
@@ -260,46 +254,46 @@
     similar equations it is left. However, the turbine dimension should
     always have length 1.
     """
 
     # turbine parameters
     D = rotor_diameter              # scalar
     HH = hub_height                 # scalar
-    Ct = ct_i                       # (wd, ws, 1, 1, 1) for the current turbine
+    Ct = ct_i                       # (findex, 1, 1, 1) for the current turbine
     TSR = tip_speed_ratio           # scalar
-    aI = axial_induction_i          # (wd, ws, 1, 1, 1) for the current turbine
-    avg_v = np.mean(v_i, axis=(3, 4))  # (wd, ws, 1, grid, grid)
+    aI = axial_induction_i          # (findex, 1, 1, 1) for the current turbine
+    avg_v = np.mean(v_i, axis=(2,3))  # (findex, 1, grid, grid)
 
     # flow parameters
-    Uinf = np.mean(u_initial, axis=(2, 3, 4))
-    Uinf = Uinf[:, :, None, None, None]
+    Uinf = np.mean(u_initial, axis=(1, 2, 3))
+    Uinf = Uinf[:, None, None, None]
 
     # TODO: Allow user input for eps gain
     eps_gain = 0.2
     eps = eps_gain * D  # Use set value
 
-    vel_top = ((HH + D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1, 1))
+    vel_top = ((HH + D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1))
     Gamma_top = gamma(
         D,
         vel_top,
         Uinf,
         Ct,
         scale,
     )
 
-    vel_bottom = ((HH - D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1, 1))
+    vel_bottom = ((HH - D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1))
     Gamma_bottom = -1 * gamma(
         D,
         vel_bottom,
         Uinf,
         Ct,
         scale,
     )
 
-    turbine_average_velocity = np.cbrt(np.mean(u_i ** 3, axis=(3, 4)))[:, :, :, None, None]
+    turbine_average_velocity = np.cbrt(np.mean(u_i ** 3, axis=(2, 3)))[:, :, None, None]
     Gamma_wake_rotation = 0.25 * 2 * pi * D * (aI - aI ** 2) * turbine_average_velocity / TSR
 
     ### compute the spanwise and vertical velocities induced by yaw
 
     # decay = eps ** 2 / (4 * nu * delta_x / Uinf + eps ** 2)   # This is the decay downstream
     yLocs = delta_y + NUM_EPS
 
@@ -307,41 +301,40 @@
     # NOTE: this is the top of the grid, not the top of the rotor
     zT = z_i - (HH + D / 2) + NUM_EPS  # distance from the top of the grid
     rT = ne.evaluate("yLocs ** 2 + zT ** 2")  # TODO: This is (-) in the paper
     # This looks like spanwise decay;
     # it defines the vortex profile in the spanwise directions
     core_shape = ne.evaluate("1 - exp(-rT / (eps ** 2))")
     v_top = ne.evaluate("(Gamma_top * zT) / (2 * pi * rT) * core_shape")
-    v_top = np.mean( v_top, axis=(3,4) )
+    v_top = np.mean( v_top, axis=(2,3) )
     # w_top = (-1 * Gamma_top * yLocs) / (2 * pi * rT) * core_shape * decay
 
     # bottom vortex
     zB = z_i - (HH - D / 2) + NUM_EPS
     rB = ne.evaluate("yLocs ** 2 + zB ** 2")
     core_shape = ne.evaluate("1 - exp(-rB / (eps ** 2))")
     v_bottom = ne.evaluate("(Gamma_bottom * zB) / (2 * pi * rB) * core_shape")
-    v_bottom = np.mean( v_bottom, axis=(3,4) )
+    v_bottom = np.mean( v_bottom, axis=(2,3) )
     # w_bottom = (-1 * Gamma_bottom * yLocs) / (2 * pi * rB) * core_shape * decay
 
     # wake rotation vortex
     zC = z_i - HH + NUM_EPS
     rC = ne.evaluate("yLocs ** 2 + zC ** 2")
     core_shape = ne.evaluate("1 - exp(-rC / (eps ** 2))")
     v_core = ne.evaluate("(Gamma_wake_rotation * zC) / (2 * pi * rC) * core_shape")
-    v_core = np.mean( v_core, axis=(3,4) )
+    v_core = np.mean( v_core, axis=(2,3) )
     # w_core = (-1 * Gamma_wake_rotation * yLocs) / (2 * pi * rC) * core_shape * decay
 
     # Cap the effective yaw values between -45 and 45 degrees
     val = 2 * (avg_v - v_core) / (v_top + v_bottom)
     val = np.where(val < -1.0, -1.0, val)
     val = np.where(val > 1.0, 1.0, val)
     y = np.degrees(0.5 * np.arcsin(val))
 
-    return y[:, :, :, None, None]
-
+    return y[:, :, None, None]
 
 def calculate_transverse_velocity(
     u_i,
     u_initial,
     dudz_initial,
     delta_x,
     delta_y,
@@ -364,37 +357,38 @@
     D = rotor_diameter
     HH = hub_height
     Ct = ct_i
     TSR = tsr_i
     aI = axial_induction_i
 
     # flow parameters
-    Uinf = np.mean(u_initial, axis=(2, 3, 4))[:, :, None, None, None]
+    Uinf = np.mean(u_initial, axis=(1, 2, 3))
+    Uinf = Uinf[:, None, None, None]
 
     eps_gain = 0.2
     eps = eps_gain * D  # Use set value
 
-    vel_top = ((HH + D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1, 1))
+    vel_top = ((HH + D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1))
     Gamma_top = sind(yaw) * cosd(yaw) * gamma(
         D,
         vel_top,
         Uinf,
         Ct,
         scale,
     )
 
-    vel_bottom = ((HH - D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1, 1))
+    vel_bottom = ((HH - D / 2) / HH) ** wind_shear * np.ones((1, 1, 1, 1))
     Gamma_bottom = -1 * sind(yaw) * cosd(yaw) * gamma(
         D,
         vel_bottom,
         Uinf,
         Ct,
         scale,
     )
-    turbine_average_velocity = np.cbrt(np.mean(u_i ** 3, axis=(3, 4)))[:, :, :, None, None]
+    turbine_average_velocity = np.cbrt(np.mean(u_i ** 3, axis=(2,3)))[:, :, None, None]
     Gamma_wake_rotation = 0.25 * 2 * pi * D * (aI - aI ** 2) * turbine_average_velocity / TSR
 
     ### compute the spanwise and vertical velocities induced by yaw
 
     # decay the vortices as they move downstream - using mixing length
     lmda = D / 8
     kappa = 0.41
@@ -482,28 +476,28 @@
     turb_v_i,
     turb_w_i
 ):
     # Since turbulence mixing is constant for the turbine,
     # use the left two dimensions only here and expand
     # before returning. Dimensions are (wd, ws).
 
-    I_i = I_i[:, :, 0, 0, 0]
+    I_i = I_i[:, 0, 0, 0]
 
-    average_u_i = np.cbrt(np.mean(u_i ** 3, axis=(2, 3, 4)))
+    average_u_i = np.cbrt(np.mean(u_i ** 3, axis=(1, 2, 3)))
 
     # Convert ambient turbulence intensity to TKE (eq 24)
     k = (average_u_i * I_i) ** 2 / (2 / 3)
 
     u_term = np.sqrt(2 * k)
-    v_term = np.mean(v_i + turb_v_i, axis=(2, 3, 4))
-    w_term = np.mean(w_i + turb_w_i, axis=(2, 3, 4))
+    v_term = np.mean(v_i + turb_v_i, axis=(1, 2, 3))
+    w_term = np.mean(w_i + turb_w_i, axis=(1, 2, 3))
 
     # Compute the new TKE (eq 23)
     k_total = 0.5 * (u_term ** 2 + v_term ** 2 + w_term ** 2)
 
     # Convert TKE back to TI
     I_total = np.sqrt((2 / 3) * k_total) / average_u_i
 
     # Remove ambient from total TI leaving only the TI due to mixing
     I_mixing = I_total - I_i
 
-    return I_mixing[:, :, None, None, None]
+    return I_mixing[:, None, None, None]
```

### Comparing `FLORIS-3.6/floris/simulation/wake_turbulence/crespo_hernandez.py` & `FLORIS-4/floris/core/wake_turbulence/crespo_hernandez.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numexpr as ne
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import cosd, sind
```

### Comparing `FLORIS-3.6/floris/simulation/wake_turbulence/wake_induced_mixing.py` & `FLORIS-4/floris/core/wake_turbulence/wake_induced_mixing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import cosd, sind
@@ -78,10 +67,10 @@
                 of multiples of turbine i's rotor diameter) (D).
 
         Returns:
             np.array: Components of the wake-induced mixing term due to
                 the ith turbine.
         """
 
-        wake_induced_mixing = axial_induction_i[:,:,:,0,0] / downstream_distance_D_i**2
+        wake_induced_mixing = axial_induction_i[:,:,0,0] / downstream_distance_D_i**2
 
         return wake_induced_mixing
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/cumulative_gauss_curl.py` & `FLORIS-4/floris/core/wake_velocity/cumulative_gauss_curl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numpy as np
 from attrs import define, field
 from scipy.special import gamma
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import (
@@ -91,66 +80,66 @@
     ) -> None:
 
         turbine_Ct = ct
         turbine_ti = turbulence_intensity
         turbine_yaw = yaw_i
 
         # TODO Should this be cbrt? This is done to match v2
-        turb_avg_vels = np.cbrt(np.mean(u_i ** 3, axis=(3, 4)))
-        turb_avg_vels = turb_avg_vels[:, :, :, None, None]
+        turb_avg_vels = np.cbrt(np.mean(u_i ** 3, axis=(2, 3)))
+        turb_avg_vels = turb_avg_vels[:, :, None, None]
 
         delta_x = x - x_i
 
         sigma_n = wake_expansion(
             delta_x,
-            turbine_Ct[:, :, ii:ii+1],
-            turbine_ti[:, :, ii:ii+1],
-            turbine_diameter[:, :, ii:ii+1],
+            turbine_Ct[:, ii:ii+1],
+            turbine_ti[:, ii:ii+1],
+            turbine_diameter[:, ii:ii+1],
             self.a_s,
             self.b_s,
             self.c_s1,
             self.c_s2,
         )
 
-        x_i_loc = np.mean(x_i, axis=(3, 4))
-        x_i_loc = x_i_loc[:, :, :, None, None]
+        x_i_loc = np.mean(x_i, axis=(2, 3))
+        x_i_loc = x_i_loc[:, :, None, None]
 
-        y_i_loc = np.mean(y_i, axis=(3, 4))
-        y_i_loc = y_i_loc[:, :, :, None, None]
+        y_i_loc = np.mean(y_i, axis=(2, 3))
+        y_i_loc = y_i_loc[:, :, None, None]
 
-        z_i_loc = np.mean(z_i, axis=(3, 4))
-        z_i_loc = z_i_loc[:, :, :, None, None]
+        z_i_loc = np.mean(z_i, axis=(2, 3))
+        z_i_loc = z_i_loc[:, :, None, None]
 
-        x_coord = np.mean(x, axis=(3, 4))[:, :, :, None, None]
+        x_coord = np.mean(x, axis=(2, 3))[:, :, None, None]
 
         y_loc = y
-        y_coord = np.mean(y, axis=(3, 4))[:, :, :, None, None]
+        y_coord = np.mean(y, axis=(2, 3))[:, :, None, None]
 
         z_loc = z  # np.mean(z, axis=(3,4))
-        z_coord = np.mean(z, axis=(3, 4))[:, :, :, None, None]
+        z_coord = np.mean(z, axis=(2, 3))[:, :, None, None]
 
         sum_lbda = np.zeros_like(u_initial)
 
         for m in range(0, ii - 1):
-            x_coord_m = x_coord[:, :, m:m+1]
-            y_coord_m = y_coord[:, :, m:m+1]
-            z_coord_m = z_coord[:, :, m:m+1]
+            x_coord_m = x_coord[:, m:m+1]
+            y_coord_m = y_coord[:, m:m+1]
+            z_coord_m = z_coord[:, m:m+1]
 
             # For computing cross planes, we don't need to compute downstream
             # turbines from out cross plane position.
-            if x_coord[:, :, m:m+1].size == 0:
+            if x_coord[:, m:m+1].size == 0:
                 break
 
             delta_x_m = x - x_coord_m
 
             sigma_i = wake_expansion(
                 delta_x_m,
-                turbine_Ct[:, :, m:m+1],
-                turbine_ti[:, :, m:m+1],
-                turbine_diameter[:, :, m:m+1],
+                turbine_Ct[:, m:m+1],
+                turbine_ti[:, m:m+1],
+                turbine_diameter[:, m:m+1],
                 self.a_s,
                 self.b_s,
                 self.c_s1,
                 self.c_s2,
             )
 
             S_i = sigma_n ** 2 + sigma_i ** 2
@@ -177,25 +166,25 @@
         #     sum_lbda = 0.0
 
         # sigma_i[ii] = sigma_n
 
         # blondel
         # super gaussian
         # b_f = self.b_f1 * np.exp(self.b_f2 * TI) + self.b_f3
-        x_tilde = np.abs(delta_x) / turbine_diameter[:,:,ii:ii+1]
+        x_tilde = np.abs(delta_x) / turbine_diameter[:,ii:ii+1]
         r_tilde = np.sqrt( (y_loc - y_i_loc - deflection_field) ** 2 + (z_loc - z_i_loc) ** 2 )
-        r_tilde /= turbine_diameter[:,:,ii:ii+1]
+        r_tilde /= turbine_diameter[:,ii:ii+1]
 
         n = self.a_f * np.exp(self.b_f * x_tilde) + self.c_f
         a1 = 2 ** (2 / n - 1)
         a2 = 2 ** (4 / n - 2)
 
         # based on Blondel model, modified to include cumulative effects
         tmp = a2 - (
-            (n * turbine_Ct[:, :, ii:ii+1])
+            (n * turbine_Ct[:, ii:ii+1])
             * cosd(turbine_yaw)
             / (
                 16.0
                 * gamma(2 / n)
                 * np.sign(sigma_n)
                 * (np.abs(sigma_n) ** (4 / n))
                 * (1 - sum_lbda) ** 2
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/empirical_gauss.py` & `FLORIS-4/floris/core/wake_velocity/empirical_gauss.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numexpr as ne
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
-from floris.simulation.wake_velocity.gauss import gaussian_function
+from floris.core.wake_velocity.gauss import gaussian_function
 from floris.utilities import (
     cosd,
     sind,
     tand,
 )
 
 
@@ -66,14 +55,17 @@
             :filter: docname in docnames
     """
     wake_expansion_rates: list = field(factory=lambda: [0.023, 0.008])
     breakpoints_D: list = field(factory=lambda: [10])
     sigma_0_D: float = field(default=0.28)
     smoothing_length_D: float = field(default=2.0)
     mixing_gain_velocity: float = field(default=2.0)
+    awc_mode: str = field(default="baseline")
+    awc_wake_exp: float = field(default=1.2)
+    awc_wake_denominator: float = field(default=400)
 
     def prepare_function(
         self,
         grid: Grid,
         flow_field: FlowField,
     ) -> Dict[str, Any]:
 
@@ -166,26 +158,26 @@
             self.wake_expansion_rates,
             [b * rotor_diameter_i for b in self.breakpoints_D], # .flatten()[0]
             sigma_y0,
             self.smoothing_length_D * rotor_diameter_i,
             self.mixing_gain_velocity * mixing_i,
         )
         sigma_y[upstream_mask] = \
-            np.tile(sigma_y0, np.shape(sigma_y)[2:])[upstream_mask]
+            np.tile(sigma_y0, np.shape(sigma_y)[1:])[upstream_mask]
 
         sigma_z = empirical_gauss_model_wake_width(
             x - x_i,
             self.wake_expansion_rates,
             [b * rotor_diameter_i for b in self.breakpoints_D], # .flatten()[0]
             sigma_z0,
             self.smoothing_length_D * rotor_diameter_i,
             self.mixing_gain_velocity * mixing_i,
         )
         sigma_z[upstream_mask] = \
-            np.tile(sigma_z0, np.shape(sigma_z)[2:])[upstream_mask]
+            np.tile(sigma_z0, np.shape(sigma_z)[1:])[upstream_mask]
 
         # 'Standard' wake component
         r, C = rCalt(
             wind_veer,
             sigma_y,
             sigma_z,
             y,
@@ -261,15 +253,15 @@
     )
     d = 1 - Ct * (sigma_y0 * sigma_z0)/(sigma_y * sigma_z) * cosd(yaw) * cosd(tilt)
     C = ne.evaluate("1 - sqrt(d)")
     return r, C
 
 def sigmoid_integral(x, center=0, width=1):
     y = np.zeros_like(x)
-    #TODO: Can this be made faster?
+    # TODO: Can this be made faster?
     above_smoothing_zone = (x-center) > width/2
     y[above_smoothing_zone] = (x-center)[above_smoothing_zone]
     in_smoothing_zone = ((x-center) >= -width/2) & ((x-center) <= width/2)
     z = ((x-center)/width + 0.5)[in_smoothing_zone]
     if width.shape[0] > 1: # multiple turbine sizes
         width = np.broadcast_to(width, x.shape)[in_smoothing_zone]
     y[in_smoothing_zone] = (width*(z**6 - 3*z**5 + 5/2*z**4)).flatten()
@@ -288,7 +280,26 @@
 
     sigma = (wake_expansion_rates[0] + mixing_final) * x + sigma_0
     for ib, b in enumerate(breakpoints):
         sigma += (wake_expansion_rates[ib+1] - wake_expansion_rates[ib]) * \
             sigmoid_integral(x, center=b, width=smoothing_length)
 
     return sigma
+
+def awc_added_wake_mixing(
+    awc_mode_i,
+    awc_amplitude_i,
+    awc_frequency_i,
+    awc_wake_exp,
+    awc_wake_denominator
+):
+
+    # TODO: Add TI in the mix, finetune amplitude/freq effect
+    if (awc_mode_i == "helix").any():
+        return awc_amplitude_i[:,:,0,0]**awc_wake_exp/awc_wake_denominator
+    elif (awc_mode_i == "baseline").any():
+        return 0
+    else:
+        raise NotImplementedError(
+            'Active wake mixing strategies other than the `helix` mode '
+            'have not yet been implemented in FLORIS.'
+        )
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/gauss.py` & `FLORIS-4/floris/core/wake_velocity/gauss.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numexpr as ne
 import numpy as np
 from attrs import define, field
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import (
@@ -127,15 +116,15 @@
 
             # This is a linear ramp from 0 to 1 from the start of the near wake to the start
             # of the far wake.
             near_wake_ramp_up = (x - xR) / (x0 - xR)
             # Another linear ramp, but positive upstream of the far wake and negative in the
             # far wake; 0 at the start of the far wake
             near_wake_ramp_down = (x0 - x) / (x0 - xR)
-            # near_wake_ramp_down = -1 * (near_wake_ramp_up - 1)  # TODO: this is equivalent, right?
+            # near_wake_ramp_down = -1 * (near_wake_ramp_up - 1)  # : this is equivalent, right?
 
             sigma_y = near_wake_ramp_down * 0.501 * rotor_diameter_i * np.sqrt(ct_i / 2.0)
             sigma_y += near_wake_ramp_up * sigma_y0
             sigma_y *= (x >= xR)
             sigma_y += np.ones_like(sigma_y) * (x < xR) * 0.5 * rotor_diameter_i
 
             sigma_z = near_wake_ramp_down * 0.501 * rotor_diameter_i * np.sqrt(ct_i / 2.0)
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/jensen.py` & `FLORIS-4/floris/core/wake_velocity/jensen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,19 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from typing import Any, Dict
 
 import numexpr as ne
 import numpy as np
 from attrs import (
     define,
     field,
     fields,
 )
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/turbopark.py` & `FLORIS-4/floris/core/wake_velocity/turbopark.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,19 @@
-# Copyright 2022 NREL
 
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
 
 from pathlib import Path
 from typing import Any, Dict
 
 import numpy as np
 import scipy.io
 from attrs import define, field
 from scipy import integrate
 from scipy.interpolate import RegularGridInterpolator
 
-from floris.simulation import (
+from floris.core import (
     BaseModel,
     Farm,
     FlowField,
     Grid,
     Turbine,
 )
 from floris.utilities import (
@@ -76,15 +66,15 @@
 
     # @profile
     def function(
         self,
         x_i: np.ndarray,
         y_i: np.ndarray,
         z_i: np.ndarray,
-        ambient_turbulence_intensity: np.ndarray,
+        ambient_turbulence_intensities: np.ndarray,
         Cts: np.ndarray,
         rotor_diameter_i: np.ndarray,
         rotor_diameters: np.ndarray,
         i: int,
         deflection_field: np.ndarray,
         # enforces the use of the below as keyword arguments and adherence to the
         # unpacking of the results from prepare_function()
@@ -105,18 +95,18 @@
         x_dist = (x_i - x) * downstream_mask / rotor_diameters
 
         # Radial distance between turbine i and the center lines of wakes from all
         # real/image turbines
         r_dist = np.sqrt((y_i - (y + deflection_field)) ** 2 + (z_i - z) ** 2)
         r_dist_image = np.sqrt((y_i - (y + deflection_field)) ** 2 + (z_i - (-z)) ** 2)
 
-        Cts[:, :, i:, :, :] = 0.00001
+        Cts[:, i:, :, :] = 0.00001
 
         # Characteristic wake widths from all turbines relative to turbine i
-        dw = characteristic_wake_width(x_dist, ambient_turbulence_intensity, Cts, self.A)
+        dw = characteristic_wake_width(x_dist, ambient_turbulence_intensities, Cts, self.A)
         epsilon = 0.25 * np.sqrt(
             np.min( 0.5 * (1 + np.sqrt(1 - Cts)) / np.sqrt(1 - Cts), 3, keepdims=True )
         )
         sigma = rotor_diameters * (epsilon + dw)
 
         # Peak wake deficits
         val = 1 - Cts / (8 * (sigma / rotor_diameters) ** 2)
@@ -133,17 +123,17 @@
         # Compute deficits for real turbines and for mirrored (image) turbines
         delta_real = C * wtg_overlapping * self.overlap_gauss_interp(
             (r_dist / sigma, rotor_diameter_i / 2 / sigma)
         )
         delta_image = C * wtg_overlapping * self.overlap_gauss_interp(
             (r_dist_image / sigma, rotor_diameter_i / 2 / sigma)
         )
-        delta = np.concatenate((delta_real, delta_image), axis=2)
+        delta = np.concatenate((delta_real, delta_image), axis=1)
 
-        delta_total[:, :, i, :, :] = np.sqrt(np.sum(np.nan_to_num(delta) ** 2, axis=2))
+        delta_total[:, i, :, :] = np.sqrt(np.sum(np.nan_to_num(delta) ** 2, axis=1))
 
         return delta_total
 
 
 def precalculate_overlap():
     # TODO: first implementation to generate wake overlap lookup table
     # (currently supplied by turbopark_lookup_table.mat.)
```

### Comparing `FLORIS-3.6/floris/simulation/wake_velocity/turbopark_lookup_table.mat` & `FLORIS-4/floris/core/wake_velocity/turbopark_lookup_table.mat`

 * *Files identical despite different names*

### Comparing `FLORIS-3.6/floris/tools/cut_plane.py` & `FLORIS-4/floris/cut_plane.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import copy
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy.interpolate import griddata
@@ -348,15 +334,15 @@
 
 
 def calculate_wind_speed(cross_plane, x1_loc, x2_loc, R):
     """
     Calculate effective wind speed within specified range of a point.
 
     Args:
-        cross_plane (:py:class:`floris.tools.cut_plane.CrossPlane`):
+        cross_plane (:py:class:`floris.cut_plane.CrossPlane`):
             plane of data.
         x1_loc (float): x1-coordinate of point of interest.
         x2_loc (float): x2-coordinate of point of interest.
         R (float): radius from point of interest to consider
 
     Returns:
         (float): effective wind speed
@@ -387,15 +373,15 @@
 def calculate_power(
     cross_plane, x1_loc, x2_loc, R, ws_array, cp_array, air_density=1.225
 ):
     """
     Calculate maximum power available in a given cross plane.
 
     Args:
-        cross_plane (:py:class:`floris.tools.cut_plane.CrossPlane`):
+        cross_plane (:py:class:`floris.cut_plane.CrossPlane`):
             plane of data.
         x1_loc (float): x1-coordinate of point of interest.
         x2_loc (float): x2-coordinate of point of interest.
         R (float): Radius of wind turbine rotor.
         ws_array (np.array): reference wind speed for cp curve.
         cp_array (np.array): cp curve at reference wind speeds.
         air_density (float, optional): air density. Defaults to 1.225.
```

### Comparing `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_base.py` & `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_scipy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,143 +1,142 @@
-# Copyright 2022 NREL
 
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
-import matplotlib.pyplot as plt
 import numpy as np
-from shapely.geometry import LineString, Polygon
-
-from floris.tools.optimization.yaw_optimization.yaw_optimizer_geometric import (
-    YawOptimizationGeometric,
-)
-
-from ....logging_manager import LoggingManager
-
-
-class LayoutOptimization(LoggingManager):
-    def __init__(self, fi, boundaries, min_dist=None, freq=None, enable_geometric_yaw=False):
-        self.fi = fi.copy()
-        self.boundaries = boundaries
-        self.enable_geometric_yaw = enable_geometric_yaw
-
-        self._boundary_polygon = Polygon(self.boundaries)
-        self._boundary_line = LineString(self.boundaries)
-
-        self.xmin = np.min([tup[0] for tup in boundaries])
-        self.xmax = np.max([tup[0] for tup in boundaries])
-        self.ymin = np.min([tup[1] for tup in boundaries])
-        self.ymax = np.max([tup[1] for tup in boundaries])
-
-        # If no minimum distance is provided, assume a value of 2 rotor diamters
-        if min_dist is None:
-            self.min_dist = 2 * self.rotor_diameter
-        else:
-            self.min_dist = min_dist
-
-        # If freq is not provided, give equal weight to all wind conditions
-        if freq is None:
-            self.freq = np.ones((
-                self.fi.floris.flow_field.n_wind_directions,
-                self.fi.floris.flow_field.n_wind_speeds
-            ))
-            self.freq = self.freq / self.freq.sum()
-        else:
-            self.freq = freq
-
-        # Establish geometric yaw class
-        if self.enable_geometric_yaw:
-            self.yaw_opt = YawOptimizationGeometric(
-                fi,
-                minimum_yaw_angle=-30.0,
-                maximum_yaw_angle=30.0,
-                exploit_layout_symmetry=False
-            )
-
-        self.initial_AEP = fi.get_farm_AEP(self.freq)
+from scipy.optimize import minimize
 
-    def __str__(self):
-        return "layout"
+from .yaw_optimization_base import YawOptimization
 
-    def _norm(self, val, x1, x2):
-            return (val - x1) / (x2 - x1)
 
-    def _unnorm(self, val, x1, x2):
-        return np.array(val) * (x2 - x1) + x1
-
-    def _get_geoyaw_angles(self):
-        # NOTE: requires that child class saves x and y locations
-        # as self.x and self.y and updates them during optimization.
-        if self.enable_geometric_yaw:
-            self.yaw_opt.fi_subset.reinitialize(layout_x=self.x, layout_y=self.y)
-            df_opt = self.yaw_opt.optimize()
-            self.yaw_angles = np.vstack(df_opt['yaw_angles_opt'])[:, None, :]
-        else:
-            self.yaw_angles = None
-
-        return self.yaw_angles
+class YawOptimizationScipy(YawOptimization):
+    """
+    YawOptimizationScipy is a subclass of
+    :py:class:`floris.optimization.general_library.YawOptimization` that is
+    used to optimize the yaw angles of all turbines in a Floris Farm for a single
+    set of inflow conditions using the SciPy optimize package.
+    """
+
+    def __init__(
+        self,
+        fmodel,
+        minimum_yaw_angle=0.0,
+        maximum_yaw_angle=25.0,
+        yaw_angles_baseline=None,
+        x0=None,
+        opt_method="SLSQP",
+        opt_options=None,
+        turbine_weights=None,
+        exclude_downstream_turbines=True,
+        verify_convergence=False,
+    ):
+        """
+        Instantiate YawOptimizationScipy object with a FlorisModel object
+        and assign parameter values.
+        """
+        if opt_options is None:
+            # Default SciPy parameters
+            opt_options = {
+                "maxiter": 100,
+                "disp": True,
+                "iprint": 2,
+                "ftol": 1e-12,
+                "eps": 0.1,
+            }
+
+        super().__init__(
+            fmodel=fmodel,
+            minimum_yaw_angle=minimum_yaw_angle,
+            maximum_yaw_angle=maximum_yaw_angle,
+            yaw_angles_baseline=yaw_angles_baseline,
+            x0=x0,
+            turbine_weights=turbine_weights,
+            normalize_control_variables=True,
+            calc_baseline_power=True,
+            exclude_downstream_turbines=exclude_downstream_turbines,
+            verify_convergence=verify_convergence,
+        )
 
-    # Public methods
+        self.opt_method = opt_method
+        self.opt_options = opt_options
 
     def optimize(self):
-        sol = self._optimize()
-        return sol
+        """
+        Find optimum setting of turbine yaw angles for a single turbine
+        cluster that maximizes the weighted wind farm power production
+        given fixed atmospheric conditions (wind speed, direction, etc.)
+        using the scipy.optimize.minimize function.
 
-    def plot_layout_opt_results(self):
-        x_initial, y_initial, x_opt, y_opt = self._get_initial_and_final_locs()
+        Returns:
+            opt_yaw_angles (np.array): Optimal yaw angles in degrees. This
+            array is equal in length to the number of turbines in the farm.
+        """
+        # Loop through every wind condition individually
+        wd_array = self.fmodel_subset.core.flow_field.wind_directions
+        ws_array = self.fmodel_subset.core.flow_field.wind_speeds
+        ti_array = self.fmodel_subset.core.flow_field.turbulence_intensities
+        for i, (wd, ws, ti) in enumerate(zip(wd_array, ws_array, ti_array)):
+
+            self.fmodel_subset.set(
+                wind_directions=[wd],
+                wind_speeds=[ws],
+                turbulence_intensities=[ti]
+            )
 
-        plt.figure(figsize=(9, 6))
-        fontsize = 16
-        plt.plot(x_initial, y_initial, "ob")
-        plt.plot(x_opt, y_opt, "or")
-        # plt.title('Layout Optimization Results', fontsize=fontsize)
-        plt.xlabel("x (m)", fontsize=fontsize)
-        plt.ylabel("y (m)", fontsize=fontsize)
-        plt.axis("equal")
-        plt.grid()
-        plt.tick_params(which="both", labelsize=fontsize)
-        plt.legend(
-            ["Old locations", "New locations"],
-            loc="lower center",
-            bbox_to_anchor=(0.5, 1.01),
-            ncol=2,
-            fontsize=fontsize,
-        )
 
-        verts = self.boundaries
-        for i in range(len(verts)):
-            if i == len(verts) - 1:
-                plt.plot([verts[i][0], verts[0][0]], [verts[i][1], verts[0][1]], "b")
-            else:
-                plt.plot(
-                    [verts[i][0], verts[i + 1][0]], [verts[i][1], verts[i + 1][1]], "b"
+            # Find turbines to optimize
+            turbs_to_opt = self._turbs_to_opt_subset[i, :]
+            if not any(turbs_to_opt):
+                continue  # Nothing to do here: no turbines to optimize
+
+            # Extract current optimization problem variables (normalized)
+            yaw_lb = self._minimum_yaw_angle_subset_norm[i, turbs_to_opt]
+            yaw_ub = self._maximum_yaw_angle_subset_norm[i, turbs_to_opt]
+            bnds = [(a, b) for a, b in zip(yaw_lb, yaw_ub)]
+            x0 = self._x0_subset_norm[i, turbs_to_opt]
+
+            J0 = self._farm_power_baseline_subset[i]
+            yaw_template = self._yaw_angles_template_subset[i, :]
+            turbine_weights = self._turbine_weights_subset[i, :]
+            yaw_template = np.tile(yaw_template, (1, 1))
+            turbine_weights = np.tile(turbine_weights, (1, 1))
+
+            # Handle heterogeneous inflow, if there is one
+            if (hasattr(self.fmodel.core.flow_field, 'heterogeneous_inflow_config') and
+                self.fmodel.core.flow_field.heterogeneous_inflow_config is not None):
+                het_sm_orig = np.array(
+                    self.fmodel.core.flow_field.heterogeneous_inflow_config['speed_multipliers']
                 )
+                het_sm = het_sm_orig[i, :].reshape(1, -1)
+            else:
+                het_sm = None
 
+            # Define cost function
+            def cost(x):
+                x_full = np.array(yaw_template, copy=True)
+                x_full[0, turbs_to_opt] = x * self._normalization_length
+                return (
+                    - 1.0 * self._calculate_farm_power(
+                        yaw_angles=x_full,
+                        wd_array=[wd],
+                        ws_array=[ws],
+                        ti_array=[ti],
+                        turbine_weights=turbine_weights,
+                        heterogeneous_speed_multipliers=het_sm
+                    )[0] / J0
+                )
 
-    ###########################################################################
-    # Properties
-    ###########################################################################
-
-    @property
-    def nturbs(self):
-        """
-        This property returns the number of turbines in the FLORIS
-        object.
+            # Perform optimization
+            residual_plant = minimize(
+                fun=cost,
+                x0=x0,
+                bounds=bnds,
+                method=self.opt_method,
+                options=self.opt_options,
+            )
 
-        Returns:
-            nturbs (int): The number of turbines in the FLORIS object.
-        """
-        self._nturbs = self.fi.floris.farm.n_turbines
-        return self._nturbs
+            # Undo normalization/masks and save results to self
+            self._farm_power_opt_subset[i] = -residual_plant.fun * J0
+            self._yaw_angles_opt_subset[i, turbs_to_opt] = (
+                residual_plant.x * self._normalization_length
+            )
 
-    @property
-    def rotor_diameter(self):
-        return self.fi.floris.farm.rotor_diameters_sorted[0][0][0]
+        # Finalize optimization, i.e., retrieve full solutions
+        df_opt = self._finalize()
+        return df_opt
```

### Comparing `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py` & `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_boundary_grid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2022 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.spatial.distance import cdist
 from shapely.geometry import (
     LineString,
     Point,
@@ -24,28 +10,28 @@
 
 from .layout_optimization_base import LayoutOptimization
 
 
 class LayoutOptimizationBoundaryGrid(LayoutOptimization):
     def __init__(
         self,
-        fi,
+        fmodel,
         boundaries,
         start,
         x_spacing,
         y_spacing,
         shear,
         rotation,
         center_x,
         center_y,
         boundary_setback,
         n_boundary_turbines=None,
         boundary_spacing=None,
     ):
-        self.fi = fi
+        self.fmodel = fmodel
 
         self.boundary_x = np.array([val[0] for val in boundaries])
         self.boundary_y = np.array([val[1] for val in boundaries])
         boundary = np.zeros((len(self.boundary_x), 2))
         boundary[:, 0] = self.boundary_x[:]
         boundary[:, 1] = self.boundary_y[:]
         self._boundary_polygon = Polygon(boundary)
@@ -622,21 +608,21 @@
             self.center_x,
             self.center_y,
             self.boundary_setback,
             self.n_boundary_turbines,
             self.boundary_spacing,
         )
 
-        self.fi.reinitialize(layout=(layout_x, layout_y))
+        self.fmodel.set(layout=(layout_x, layout_y))
 
     def plot_layout(self):
         plt.figure(figsize=(9, 6))
         fontsize = 16
 
-        plt.plot(self.fi.layout_x, self.fi.layout_y, "ob")
+        plt.plot(self.fmodel.layout_x, self.fmodel.layout_y, "ob")
         # plt.plot(locsx, locsy, "or")
 
         plt.xlabel("x (m)", fontsize=fontsize)
         plt.ylabel("y (m)", fontsize=fontsize)
         plt.axis("equal")
         plt.grid()
         plt.tick_params(which="both", labelsize=fontsize)
```

### Comparing `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py` & `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,36 @@
-# Copyright 2022 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.spatial.distance import cdist
 from shapely.geometry import Point
 
 from .layout_optimization_base import LayoutOptimization
 
 
 class LayoutOptimizationPyOptSparse(LayoutOptimization):
     def __init__(
         self,
-        fi,
+        fmodel,
         boundaries,
         min_dist=None,
-        freq=None,
         solver=None,
         optOptions=None,
         timeLimit=None,
         storeHistory='hist.hist',
-        hotStart=None,
-        enable_geometric_yaw=False,
+        hotStart=None
     ):
-        super().__init__(fi, boundaries, min_dist=min_dist, freq=freq,
-                         enable_geometric_yaw=enable_geometric_yaw)
-
-        self.x0 = self._norm(self.fi.layout_x, self.xmin, self.xmax)
-        self.y0 = self._norm(self.fi.layout_y, self.ymin, self.ymax)
+        super().__init__(fmodel, boundaries, min_dist=min_dist)
+        self._reinitialize(solver=solver, optOptions=optOptions)
 
         self.storeHistory = storeHistory
         self.timeLimit = timeLimit
         self.hotStart = hotStart
-        self.enable_geometric_yaw = enable_geometric_yaw
 
+    def _reinitialize(self, solver=None, optOptions=None):
         try:
             import pyoptsparse
         except ImportError:
             err_msg = (
                 "It appears you do not have pyOptSparse installed. "
                 + "Please refer to https://pyoptsparse.readthedocs.io/ for "
                 + "guidance on how to properly install the module."
@@ -102,23 +83,21 @@
         return self.sol
 
     def _obj_func(self, varDict):
         # Parse the variable dictionary
         self.parse_opt_vars(varDict)
 
         # Update turbine map with turbince locations
-        self.fi.reinitialize(layout_x = self.x, layout_y = self.y)
-
-        # Compute turbine yaw angles using PJ's geometric code (if enabled)
-        yaw_angles = self._get_geoyaw_angles()
+        # self.fmodel.reinitialize(layout=[self.x, self.y])
+        # self.fmodel.calculate_wake()
 
         # Compute the objective function
         funcs = {}
         funcs["obj"] = (
-            -1 * self.fi.get_farm_AEP(self.freq, yaw_angles=yaw_angles) / self.initial_AEP
+            -1 * self.mean_distance(self.x, self.y)
         )
 
         # Compute constraints, if any are defined for the optimization
         funcs = self.compute_cons(funcs, self.x, self.y)
 
         fail = False
         return funcs, fail
@@ -135,18 +114,18 @@
 
     def parse_sol_vars(self, sol):
         self.x = list(self._unnorm(sol.getDVs()["x"], self.xmin, self.xmax))[0]
         self.y = list(self._unnorm(sol.getDVs()["y"], self.ymin, self.ymax))[1]
 
     def add_var_group(self, optProb):
         optProb.addVarGroup(
-            "x", self.nturbs, varType="c", lower=0.0, upper=1.0, value=self.x0
+            "x", self.nturbs, type="c", lower=0.0, upper=1.0, value=self.x0
         )
         optProb.addVarGroup(
-            "y", self.nturbs, varType="c", lower=0.0, upper=1.0, value=self.y0
+            "y", self.nturbs, type="c", lower=0.0, upper=1.0, value=self.y0
         )
 
         return optProb
 
     def add_con_group(self, optProb):
         optProb.addConGroup("boundary_con", self.nturbs, upper=0.0)
         optProb.addConGroup("spacing_con", 1, upper=0.0)
@@ -155,14 +134,21 @@
 
     def compute_cons(self, funcs, x, y):
         funcs["boundary_con"] = self.distance_from_boundaries(x, y)
         funcs["spacing_con"] = self.space_constraint(x, y)
 
         return funcs
 
+    def mean_distance(self, x, y):
+
+        locs = np.vstack((x, y)).T
+        distances = cdist(locs, locs)
+        return np.mean(distances)
+
+
     def space_constraint(self, x, y, rho=500):
         # Calculate distances between turbines
         locs = np.vstack((x, y)).T
         distances = cdist(locs, locs)
         arange = np.arange(distances.shape[0])
         distances[arange, arange] = 1e10
         dist = np.min(distances, axis=0)
@@ -179,23 +165,48 @@
 
         return KS_constraint[0][0]
 
     def distance_from_boundaries(self, x, y):
         boundary_con = np.zeros(self.nturbs)
         for i in range(self.nturbs):
             loc = Point(x[i], y[i])
-            boundary_con[i] = loc.distance(self._boundary_line)
-            if self._boundary_polygon.contains(loc) is True:
+            boundary_con[i] = loc.distance(self.boundary_line)
+            if self.boundary_polygon.contains(loc) is True:
                 boundary_con[i] *= -1.0
 
         return boundary_con
 
-    def _get_initial_and_final_locs(self):
-        x_initial = self._unnorm(self.x0, self.xmin, self.xmax)
-        y_initial = self._unnorm(self.y0, self.ymin, self.ymax)
-        x_opt, y_opt = self.get_optimized_locs()
-        return x_initial, y_initial, x_opt, y_opt
-
-    def get_optimized_locs(self):
-        x_opt = self._unnorm(self.sol.getDVs()["x"], self.xmin, self.xmax)
-        y_opt = self._unnorm(self.sol.getDVs()["y"], self.ymin, self.ymax)
-        return x_opt, y_opt
+    def plot_layout_opt_results(self):
+        """
+        Method to plot the old and new locations of the layout opitimization.
+        """
+        locsx = self._unnorm(self.sol.getDVs()["x"], self.xmin, self.xmax)
+        locsy = self._unnorm(self.sol.getDVs()["y"], self.ymin, self.ymax)
+        x0 = self._unnorm(self.x0, self.xmin, self.xmax)
+        y0 = self._unnorm(self.y0, self.ymin, self.ymax)
+
+        plt.figure(figsize=(9, 6))
+        fontsize = 16
+        plt.plot(x0, y0, "ob")
+        plt.plot(locsx, locsy, "or")
+        # plt.title('Layout Optimization Results', fontsize=fontsize)
+        plt.xlabel("x (m)", fontsize=fontsize)
+        plt.ylabel("y (m)", fontsize=fontsize)
+        plt.axis("equal")
+        plt.grid()
+        plt.tick_params(which="both", labelsize=fontsize)
+        plt.legend(
+            ["Old locations", "New locations"],
+            loc="lower center",
+            bbox_to_anchor=(0.5, 1.01),
+            ncol=2,
+            fontsize=fontsize,
+        )
+
+        verts = self.boundaries
+        for i in range(len(verts)):
+            if i == len(verts) - 1:
+                plt.plot([verts[i][0], verts[0][0]], [verts[i][1], verts[0][1]], "b")
+            else:
+                plt.plot(
+                    [verts[i][0], verts[i + 1][0]], [verts[i][1], verts[i + 1][1]], "b"
+                )
```

### Comparing `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py` & `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_pyoptsparse.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,92 @@
-# Copyright 2022 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.spatial.distance import cdist
 from shapely.geometry import Point
 
 from .layout_optimization_base import LayoutOptimization
 
 
 class LayoutOptimizationPyOptSparse(LayoutOptimization):
+    """
+    This class provides an interface for optimizing the layout of wind turbines
+    using the pyOptSparse optimization library.  The optimization objective is to
+    maximize annual energy production (AEP) or annual value production (AVP).
+
+    Args:
+        fmodel (FlorisModel): A FlorisModel object.
+        boundaries (iterable(float, float)): Pairs of x- and y-coordinates
+            that represent the boundary's vertices (m).
+        min_dist (float, optional): The minimum distance to be maintained
+            between turbines during the optimization (m). If not specified,
+            initializes to 2 rotor diameters. Defaults to None.
+        solver (str, optional): Sets the solver used by pyOptSparse. Defaults
+            to 'SLSQP'.
+        optOptions (dict, optional): Dictionary for setting the
+            optimization options. Defaults to None.
+        timeLimit (float, optional): Variable passed to pyOptSparse optimizer.
+            The maximum amount of time for optimizer to run (seconds). If None,
+            no time limit is imposed. Defaults to None.
+        storeHistory (str, optional): Variable passed to pyOptSparse optimizer.
+            File name of the history file into which the history of the
+            pyOptSparse optimization will be stored. Defaults to "hist.hist".
+        hotStart (str, optional): Variable passed to pyOptSparse optimizer.
+            File name of the history file to “replay” for the optimization.
+            If None, pyOptSparse initializes the optimization from scratch.
+            Defaults to None.
+        enable_geometric_yaw (bool, optional): If True, enables geometric yaw
+            optimization. Defaults to False.
+        use_value (bool, optional): If True, the layout optimization objective
+            is to maximize annual value production using the value array in the
+            FLORIS model's WindData object. If False, the optimization
+            objective is to maximize AEP. Defaults to False.
+    """
     def __init__(
         self,
-        fi,
+        fmodel,
         boundaries,
         min_dist=None,
-        freq=None,
         solver=None,
         optOptions=None,
         timeLimit=None,
         storeHistory='hist.hist',
-        hotStart=None
+        hotStart=None,
+        enable_geometric_yaw=False,
+        use_value=False,
     ):
-        super().__init__(fi, boundaries, min_dist=min_dist, freq=freq)
-        self._reinitialize(solver=solver, optOptions=optOptions)
+
+        super().__init__(
+            fmodel,
+            boundaries,
+            min_dist=min_dist,
+            enable_geometric_yaw=enable_geometric_yaw,
+            use_value=use_value
+        )
+
+        self.x0 = self._norm(self.fmodel.layout_x, self.xmin, self.xmax)
+        self.y0 = self._norm(self.fmodel.layout_y, self.ymin, self.ymax)
 
         self.storeHistory = storeHistory
         self.timeLimit = timeLimit
         self.hotStart = hotStart
+        self.enable_geometric_yaw = enable_geometric_yaw
 
-    def _reinitialize(self, solver=None, optOptions=None):
         try:
             import pyoptsparse
         except ImportError:
             err_msg = (
                 "It appears you do not have pyOptSparse installed. "
                 + "Please refer to https://pyoptsparse.readthedocs.io/ for "
                 + "guidance on how to properly install the module."
             )
             self.logger.error(err_msg, stack_info=True)
             raise ImportError(err_msg)
 
-        # Insantiate ptOptSparse optimization object with name and objective function
+        # Instantiate pyOptSparse optimization object with name and objective function
         self.optProb = pyoptsparse.Optimization('layout', self._obj_func)
 
         self.optProb = self.add_var_group(self.optProb)
         self.optProb = self.add_con_group(self.optProb)
         self.optProb.addObj("obj")
 
         if solver is not None:
@@ -97,24 +126,26 @@
                 )
         return self.sol
 
     def _obj_func(self, varDict):
         # Parse the variable dictionary
         self.parse_opt_vars(varDict)
 
-        # Update turbine map with turbince locations
-        # self.fi.reinitialize(layout=[self.x, self.y])
-        # self.fi.calculate_wake()
+        # Compute turbine yaw angles using PJ's geometric code (if enabled)
+        yaw_angles = self._get_geoyaw_angles()
+        # Update turbine map with turbine locations and yaw angles
+        self.fmodel.set(layout_x=self.x, layout_y=self.y, yaw_angles=yaw_angles)
+        self.fmodel.run()
 
         # Compute the objective function
         funcs = {}
-        funcs["obj"] = (
-            -1 * self.mean_distance(self.x, self.y)
-           #  -1 * np.sum(self.fi.get_farm_power() * self.freq * 8760) / self.initial_AEP
-        )
+        if self.use_value:
+            funcs["obj"] = -1 * self.fmodel.get_farm_AVP() / self.initial_AEP_or_AVP
+        else:
+            funcs["obj"] = -1 * self.fmodel.get_farm_AEP() / self.initial_AEP_or_AVP
 
         # Compute constraints, if any are defined for the optimization
         funcs = self.compute_cons(funcs, self.x, self.y)
 
         fail = False
         return funcs, fail
 
@@ -130,18 +161,18 @@
 
     def parse_sol_vars(self, sol):
         self.x = list(self._unnorm(sol.getDVs()["x"], self.xmin, self.xmax))[0]
         self.y = list(self._unnorm(sol.getDVs()["y"], self.ymin, self.ymax))[1]
 
     def add_var_group(self, optProb):
         optProb.addVarGroup(
-            "x", self.nturbs, type="c", lower=0.0, upper=1.0, value=self.x0
+            "x", self.nturbs, varType="c", lower=0.0, upper=1.0, value=self.x0
         )
         optProb.addVarGroup(
-            "y", self.nturbs, type="c", lower=0.0, upper=1.0, value=self.y0
+            "y", self.nturbs, varType="c", lower=0.0, upper=1.0, value=self.y0
         )
 
         return optProb
 
     def add_con_group(self, optProb):
         optProb.addConGroup("boundary_con", self.nturbs, upper=0.0)
         optProb.addConGroup("spacing_con", 1, upper=0.0)
@@ -150,21 +181,14 @@
 
     def compute_cons(self, funcs, x, y):
         funcs["boundary_con"] = self.distance_from_boundaries(x, y)
         funcs["spacing_con"] = self.space_constraint(x, y)
 
         return funcs
 
-    def mean_distance(self, x, y):
-
-        locs = np.vstack((x, y)).T
-        distances = cdist(locs, locs)
-        return np.mean(distances)
-
-
     def space_constraint(self, x, y, rho=500):
         # Calculate distances between turbines
         locs = np.vstack((x, y)).T
         distances = cdist(locs, locs)
         arange = np.arange(distances.shape[0])
         distances[arange, arange] = 1e10
         dist = np.min(distances, axis=0)
@@ -181,48 +205,23 @@
 
         return KS_constraint[0][0]
 
     def distance_from_boundaries(self, x, y):
         boundary_con = np.zeros(self.nturbs)
         for i in range(self.nturbs):
             loc = Point(x[i], y[i])
-            boundary_con[i] = loc.distance(self.boundary_line)
-            if self.boundary_polygon.contains(loc) is True:
+            boundary_con[i] = loc.distance(self._boundary_line)
+            if self._boundary_polygon.contains(loc) is True:
                 boundary_con[i] *= -1.0
 
         return boundary_con
 
-    def plot_layout_opt_results(self):
-        """
-        Method to plot the old and new locations of the layout opitimization.
-        """
-        locsx = self._unnorm(self.sol.getDVs()["x"], self.xmin, self.xmax)
-        locsy = self._unnorm(self.sol.getDVs()["y"], self.ymin, self.ymax)
-        x0 = self._unnorm(self.x0, self.xmin, self.xmax)
-        y0 = self._unnorm(self.y0, self.ymin, self.ymax)
-
-        plt.figure(figsize=(9, 6))
-        fontsize = 16
-        plt.plot(x0, y0, "ob")
-        plt.plot(locsx, locsy, "or")
-        # plt.title('Layout Optimization Results', fontsize=fontsize)
-        plt.xlabel("x (m)", fontsize=fontsize)
-        plt.ylabel("y (m)", fontsize=fontsize)
-        plt.axis("equal")
-        plt.grid()
-        plt.tick_params(which="both", labelsize=fontsize)
-        plt.legend(
-            ["Old locations", "New locations"],
-            loc="lower center",
-            bbox_to_anchor=(0.5, 1.01),
-            ncol=2,
-            fontsize=fontsize,
-        )
-
-        verts = self.boundaries
-        for i in range(len(verts)):
-            if i == len(verts) - 1:
-                plt.plot([verts[i][0], verts[0][0]], [verts[i][1], verts[0][1]], "b")
-            else:
-                plt.plot(
-                    [verts[i][0], verts[i + 1][0]], [verts[i][1], verts[i + 1][1]], "b"
-                )
+    def _get_initial_and_final_locs(self):
+        x_initial = self._unnorm(self.x0, self.xmin, self.xmax)
+        y_initial = self._unnorm(self.y0, self.ymin, self.ymax)
+        x_opt, y_opt = self.get_optimized_locs()
+        return x_initial, y_initial, x_opt, y_opt
+
+    def get_optimized_locs(self):
+        x_opt = self._unnorm(self.sol.getDVs()["x"], self.xmin, self.xmax)
+        y_opt = self._unnorm(self.sol.getDVs()["y"], self.ymin, self.ymax)
+        return x_opt, y_opt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `FLORIS-3.6/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py` & `FLORIS-4/floris/optimization/layout_optimization/layout_optimization_scipy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,79 +1,77 @@
-# Copyright 2022 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.optimize import minimize
 from scipy.spatial.distance import cdist
 from shapely.geometry import Point
 
 from .layout_optimization_base import LayoutOptimization
 
 
 class LayoutOptimizationScipy(LayoutOptimization):
+    """
+    This class provides an interface for optimizing the layout of wind turbines
+    using the Scipy optimization library.  The optimization objective is to
+    maximize annual energy production (AEP) or annual value production (AVP).
+
+
+    Args:
+        fmodel (FlorisModel): A FlorisModel object.
+        boundaries (iterable(float, float)): Pairs of x- and y-coordinates
+            that represent the boundary's vertices (m).
+        bnds (iterable, optional): Bounds for the optimization
+            variables (pairs of min/max values for each variable (m)). If
+            none are specified, they are set to 0 and 1. Defaults to None.
+        min_dist (float, optional): The minimum distance to be maintained
+            between turbines during the optimization (m). If not specified,
+            initializes to 2 rotor diameters. Defaults to None.
+        solver (str, optional): Sets the solver used by Scipy. Defaults to 'SLSQP'.
+        optOptions (dict, optional): Dictionary for setting the
+            optimization options. Defaults to None.
+        enable_geometric_yaw (bool, optional): If True, enables geometric yaw
+            optimization. Defaults to False.
+        use_value (bool, optional): If True, the layout optimization objective
+            is to maximize annual value production using the value array in the
+            FLORIS model's WindData object. If False, the optimization
+            objective is to maximize AEP. Defaults to False.
+    """
     def __init__(
         self,
-        fi,
+        fmodel,
         boundaries,
-        freq=None,
         bnds=None,
         min_dist=None,
         solver='SLSQP',
         optOptions=None,
         enable_geometric_yaw=False,
+        use_value=False,
     ):
-        """
-        _summary_
 
-        Args:
-            fi (_type_): _description_
-            boundaries (iterable(float, float)): Pairs of x- and y-coordinates
-                that represent the boundary's vertices (m).
-            freq (np.array): An array of the frequencies of occurance
-                correponding to each pair of wind direction and wind speed
-                values. If None, equal weight is given to each pair of wind conditions
-                Defaults to None.
-            bnds (iterable, optional): Bounds for the optimization
-                variables (pairs of min/max values for each variable (m)). If
-                none are specified, they are set to 0 and 1. Defaults to None.
-            min_dist (float, optional): The minimum distance to be maintained
-                between turbines during the optimization (m). If not specified,
-                initializes to 2 rotor diameters. Defaults to None.
-            solver (str, optional): Sets the solver used by Scipy. Defaults to 'SLSQP'.
-            optOptions (dict, optional): Dicitonary for setting the
-                optimization options. Defaults to None.
-        """
-        super().__init__(fi, boundaries, min_dist=min_dist, freq=freq,
-                    enable_geometric_yaw=enable_geometric_yaw)
+        super().__init__(
+            fmodel,
+            boundaries,
+            min_dist=min_dist,
+            enable_geometric_yaw=enable_geometric_yaw,
+            use_value=use_value
+        )
 
         self.boundaries_norm = [
             [
                 self._norm(val[0], self.xmin, self.xmax),
                 self._norm(val[1], self.ymin, self.ymax),
             ]
             for val in self.boundaries
         ]
         self.x0 = [
             self._norm(x, self.xmin, self.xmax)
-            for x in self.fi.layout_x
+            for x in self.fmodel.layout_x
         ] + [
             self._norm(y, self.ymin, self.ymax)
-            for y in self.fi.layout_y
+            for y in self.fmodel.layout_y
         ]
         if bnds is not None:
             self.bnds = bnds
         else:
             self._set_opt_bounds()
         if solver is not None:
             self.solver = solver
@@ -108,28 +106,34 @@
         ] + [
             self._unnorm(valy, self.ymin, self.ymax)
             for valy in locs[self.nturbs : 2 * self.nturbs]
         ]
         self._change_coordinates(locs_unnorm)
         # Compute turbine yaw angles using PJ's geometric code (if enabled)
         yaw_angles = self._get_geoyaw_angles()
-        return (-1 * self.fi.get_farm_AEP(self.freq, yaw_angles=yaw_angles) /
-                self.initial_AEP)
+        self.fmodel.set_operation(yaw_angles=yaw_angles)
+        self.fmodel.run()
+
+        if self.use_value:
+            return -1 * self.fmodel.get_farm_AVP() / self.initial_AEP_or_AVP
+        else:
+            return -1 * self.fmodel.get_farm_AEP() / self.initial_AEP_or_AVP
+
 
     def _change_coordinates(self, locs):
         # Parse the layout coordinates
         layout_x = locs[0 : self.nturbs]
         layout_y = locs[self.nturbs : 2 * self.nturbs]
 
         # Store on object for use in geoyaw code
         self.x = layout_x
         self.y = layout_y
 
         # Update the turbine map in floris
-        self.fi.reinitialize(layout_x=layout_x, layout_y=layout_y)
+        self.fmodel.set(layout_x=layout_x, layout_y=layout_y)
 
     def _generate_constraints(self):
         tmp1 = {
             "type": "ineq",
             "fun": lambda x, *args: self._space_constraint(x),
         }
         tmp2 = {
@@ -212,15 +216,15 @@
 
 
     # Public methods
 
     def optimize(self):
         """
         This method finds the optimized layout of wind turbines for power
-        production given the provided frequencies of occurance of wind
+        production given the provided frequencies of occurrence of wind
         conditions (wind speed, direction).
 
         Returns:
             opt_locs (iterable): A list of the optimized locations of each
             turbine (m).
         """
         print("=====================================================")
```

### Comparing `FLORIS-3.6/floris/tools/optimization/legacy/scipy/cluster_turbines.py` & `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,49 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 
 
-def cluster_turbines(fi, wind_direction=None, wake_slope=0.30, plot_lines=False):
-    """Separate a wind farm into separate clusters in which the turbines in
-    each subcluster only affects the turbines in its cluster and has zero
-    interaction with turbines from other clusters, both ways (being waked,
-    generating wake), This allows the user to separate the control setpoint
-    optimization in several lower-dimensional optimization problems, for
-    example. This function assumes a very simplified wake function where the
-    wakes are assumed to have a linearly diverging profile. In comparisons
-    with the FLORIS GCH model, the wake_slope matches well with the FLORIS'
-    wake profiles for a value of wake_slope = 0.5 * turbulence_intensity, where
+def derive_downstream_turbines(fmodel, wind_direction, wake_slope=0.30, plot_lines=False):
+    """Determine which turbines have no effect on other turbines in the
+    farm, i.e., which turbines have wakes that do not impact the other
+    turbines in the farm. This allows the user to exclude these turbines
+    from a control setpoint optimization, for example. This function
+    assumes a very simplified wake function where the wakes are assumed
+    to have a linearly diverging profile. In comparisons with the FLORIS
+    GCH model, the wake_slope matches well with the FLORIS' wake profiles
+    for a value of wake_slope = 0.5 * turbulence_intensity, where
     turbulence_intensity is an input to the FLORIS model at the default
     GCH parameterization. Note that does not include wind direction variability.
     To be conservative, the user is recommended to use the rule of thumb:
     `wake_slope = turbulence_intensity`. Hence, the default value for
     `wake_slope=0.30` should be conservative for turbulence intensities up to
     0.30 and is likely to provide valid estimates of which turbines are
     downstream until a turbulence intensity of 0.50. This simple model saves
     time compared to FLORIS.
 
     Args:
-        fi ([floris object]): FLORIS object of the farm of interest.
+        fmodel (FlorisModel): A FlorisModel object.
         wind_direction (float): The wind direction in the FLORIS frame
         of reference for which the downstream turbines are to be determined.
         wake_slope (float, optional): linear slope of the wake (dy/dx)
         plot_lines (bool, optional): Enable plotting wakes/turbines.
         Defaults to False.
 
     Returns:
-        clusters (iterable): A list in which each entry contains a list
-        of turbine numbers that together form a cluster which
-        exclusively interact with one another and have zero
-        interaction with turbines outside of this cluster.
+        turbs_downstream (iterable): A list containing the turbine
+        numbers that have a wake that does not affect any other
+        turbine inside the farm.
     """
 
-    if wind_direction is None:
-        wind_direction = np.mean(fi.floris.farm.wind_direction)
-
     # Get farm layout
-    x = fi.layout_x
-    y = fi.layout_y
-    D = np.array([t.rotor_diameter for t in fi.floris.farm.turbines])
+    x = fmodel.layout_x
+    y = fmodel.layout_y
+    D = np.ones_like(x) * fmodel.core.farm.rotor_diameters_sorted[0][0]
     n_turbs = len(x)
 
     # Rotate farm and determine freestream/waked turbines
     is_downstream = [False for _ in range(n_turbs)]
     x_rot = (
         np.cos((wind_direction - 270.0) * np.pi / 180.0) * x
         - np.sin((wind_direction - 270.0) * np.pi / 180.0) * y
@@ -80,18 +62,16 @@
                 "k",
             )
         for ii in range(n_turbs):
             ax.text(x_rot[ii], y_rot[ii], "T%03d" % ii)
         ax.axis("equal")
 
     srt = np.argsort(x_rot)
-    usrt = np.argsort(srt)
     x_rot_srt = x_rot[srt]
     y_rot_srt = y_rot[srt]
-    affected_by_turbs = np.tile(False, (n_turbs, n_turbs))
     for ii in range(n_turbs):
         x0 = x_rot_srt[ii]
         y0 = y_rot_srt[ii]
 
         def wake_profile_ub_turbii(x):
             y = (y0 + D[ii]) + (x - x0) * wake_slope
             if isinstance(y, (float, np.float64, np.float32)):
@@ -109,27 +89,17 @@
             else:
                 y[x < x0 + 0.01] = -np.Inf
             return y
 
         def determine_if_in_wake(xt, yt):
             return (yt < wake_profile_ub_turbii(xt)) & (yt > wake_profile_lb_turbii(xt))
 
-        # Get most downstream turbine
         is_downstream[ii] = not any(
             determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii]) for iii in range(n_turbs)
         )
-        # Determine which turbines are affected by this turbine ('ii')
-        affecting_following_turbs = [
-                determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii])
-                for iii in range(n_turbs)
-        ]
-
-        # Determine by which turbines this turbine ('ii') is affected
-        for aft in np.where(affecting_following_turbs)[0]:
-            affected_by_turbs[aft, ii] = True
 
         if plot_lines:
             x1 = np.max(x_rot_srt) + 500.0
             ax.fill_between(
                 [x0, x1, x1, x0],
                 [
                     wake_profile_ub_turbii(x0 + 0.02),
@@ -138,47 +108,23 @@
                     wake_profile_lb_turbii(x0 + 0.02),
                 ],
                 alpha=0.1,
                 color="k",
                 edgecolor=None,
             )
 
-    # Rearrange into initial frame of reference
-    affected_by_turbs = affected_by_turbs[:, usrt][usrt, :]
-    for ii in range(n_turbs):
-        affected_by_turbs[ii, ii] = True  # Add self to turb_list_affected
-    affected_by_turbs = [np.where(c)[0] for c in affected_by_turbs]
-
-    # List of downstream turbines
-    turbs_downstream = [is_downstream[i] for i in usrt]
-    turbs_downstream = list(np.where(turbs_downstream)[0])
-
-    # Initialize one cluster for each turbine and all the turbines its affected by
-    clusters = affected_by_turbs
-
-    # Iteratively merge clusters if any overlap between turbines
-    ci = 0
-    while ci < len(clusters):
-        # Compare current row to the ones to the right of it
-        cj = ci + 1
-        merged_column = False
-        while cj < len(clusters):
-            if any(y in clusters[ci] for y in clusters[cj]):
-                # Merge
-                clusters[ci] = np.hstack([clusters[ci], clusters[cj]])
-                clusters[ci] = np.array(np.unique(clusters[ci]), dtype=int)
-                clusters.pop(cj)
-                merged_column = True
-            else:
-                cj = cj + 1
-        if not merged_column:
-            ci = ci + 1
+    usrt = np.argsort(srt)
+    is_downstream = [is_downstream[i] for i in usrt]
+    turbs_downstream = list(np.where(is_downstream)[0])
 
     if plot_lines:
-        ax.set_title("wind_direction = %.1f deg" % wind_direction)
+        ax.set_title("wind_direction = %03d" % wind_direction)
         ax.set_xlim([np.min(x_rot) - 500.0, x1])
         ax.set_ylim([np.min(y_rot) - 500.0, np.max(y_rot) + 500.0])
-        for ci, cl in enumerate(clusters):
-            ax.plot(x_rot[cl], y_rot[cl], 'o', label='cluster %d' % ci)
-        ax.legend()
+        ax.plot(
+            x_rot[turbs_downstream],
+            y_rot[turbs_downstream],
+            "o",
+            color="green",
+        )
 
-    return clusters
+    return turbs_downstream
```

### Comparing `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw.py` & `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimization_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,59 @@
-# Copyright 2021 NREL
 
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
+import copy
+from time import perf_counter as timerpc
 
 import numpy as np
-from scipy.optimize import minimize
-from scipy.stats import norm
+import pandas as pd
+
+from floris.logging_manager import LoggingManager
 
-from .derive_downstream_turbines import derive_downstream_turbines
-from .optimization import Optimization
+from .yaw_optimization_tools import derive_downstream_turbines
 
 
-class YawOptimization(Optimization):
+class YawOptimization(LoggingManager):
     """
-    YawOptimization is a subclass of :py:class:`floris.tools.optimization.scipy.
+    YawOptimization is a subclass of :py:class:`floris.optimization.scipy.
     Optimization` that is used to optimize the yaw angles of all turbines in a Floris
     Farm for a single set of inflow conditions using the SciPy optimize package.
     """
 
     def __init__(
         self,
-        fi,
+        fmodel,
         minimum_yaw_angle=0.0,
         maximum_yaw_angle=25.0,
         yaw_angles_baseline=None,
         x0=None,
-        bnds=None,
-        opt_method="SLSQP",
-        opt_options=None,
-        include_unc=False,
-        unc_pmfs=None,
-        unc_options=None,
         turbine_weights=None,
-        calc_init_power=True,
-        exclude_downstream_turbines=False,
+        normalize_control_variables=False,
+        calc_baseline_power=True,
+        exclude_downstream_turbines=True,
+        verify_convergence=False,
     ):
         """
-        Instantiate YawOptimization object with a FlorisInterface object
+        Instantiate YawOptimization object with a FlorisModel object
         and assign parameter values.
 
         Args:
-            fi (:py:class:`~.tools.floris_interface.FlorisInterface`):
-                Interface used to interact with the Floris object.
-            minimum_yaw_angle (float, optional): Minimum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 0.0.
-            maximum_yaw_angle (float, optional): Maximum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 25.0.
+            fmodel (:py:class:`~.floris_model.FlorisModel`): A FlorisModel object.
+            minimum_yaw_angle (float or ndarray): Minimum constraint on yaw
+                angle (deg). If a single value specified, assumes this value
+                for all turbines. If a 1D array is specified, assumes these
+                limits for each turbine specifically, but uniformly across
+                all atmospheric conditions. If a 2D array, limits are specific
+                both to the turbine and to the atmospheric condition.
+                Defaults to 0.0.
+            maximum_yaw_angle (float or ndarray): Maximum constraint on yaw
+                angle (deg). If a single value specified, assumes this value
+                for all turbines. If a 1D array is specified, assumes these
+                limits for each turbine specifically, but uniformly across
+                all atmospheric conditions. If a 2D array, limits are specific
+                both to the turbine and to the atmospheric condition.
+                Defaults to 25.0.
             yaw_angles_baseline (iterable, optional): The baseline yaw
                 angles used to calculate the initial and baseline power
                 production in the wind farm and used to normalize the cost
                 function. If none are specified, this variable is set equal
                 to the current yaw angles in floris. Note that this variable
                 need not meet the yaw constraints specified in self.bnds,
                 yet a warning is raised if it does to inform the user.
@@ -72,78 +65,14 @@
                 since they are not part of the optimization. Instead, the yaw
                 angles for those turbines are 0.0 if that meets the lower and
                 upper bound, or otherwise as close to 0.0 as feasible. If no
                 values for x0 are specified, x0 is set to be equal to zeros
                 wherever feasible (w.r.t. the bounds), and equal to the
                 average of its lower and upper bound for all non-downstream
                 turbines otherwise. Defaults to None.
-            bnds (iterable, optional): Bounds for the yaw angles, as tuples of
-                min, max values for each turbine (deg). One can fix the yaw
-                angle of certain turbines to a predefined value by setting that
-                turbine's lower bound equal to its upper bound (i.e., an
-                equality constraint), as: bnds[ti] = (x, x), where x is the
-                fixed yaw angle assigned to the turbine. This works for both
-                zero and nonzero yaw angles. Moreover, if
-                exclude_downstream_turbines=True, the yaw angles for all
-                downstream turbines will be 0.0 or a feasible value closest to
-                0.0. If none are specified, the bounds are set to
-                (minimum_yaw_angle, maximum_yaw_angle) for each turbine. Note
-                that, if bnds is not none, its values overwrite any value given
-                in minimum_yaw_angle and maximum_yaw_angle. Defaults to None.
-            opt_method (str, optional): The optimization method used by
-                scipy.optimize.minize. Defaults to 'SLSQP'.
-            opt_options (dictionary, optional): Optimization options used by
-                scipy.optimize.minize. If none are specified, they are set to
-                {'maxiter': 100, 'disp': False, 'iprint': 1, 'ftol': 1e-7,
-                'eps': 0.01}. Defaults to None.
-            include_unc (bool, optional): Determines whether wind direction or
-                yaw uncertainty are included. If True, uncertainty in wind
-                direction and/or yaw position is included when determining
-                wind farm power. Uncertainty is included by computing the
-                mean wind farm power for a distribution of wind direction
-                and yaw position deviations from the intended wind direction
-                and yaw angles. Defaults to False.
-            unc_pmfs (dictionary, optional): A dictionary containing
-                probability mass functions describing the distribution of
-                wind direction and yaw position deviations when wind direction
-                and/or yaw position uncertainty is included in the power
-                calculations. Contains the following key-value pairs:
-
-                -   **wd_unc** (*np.array*): The wind direction
-                    deviations from the intended wind direction (deg).
-                -   **wd_unc_pmf** (*np.array*): The probability
-                    of each wind direction deviation in **wd_unc** occuring.
-                -   **yaw_unc** (*np.array*): The yaw angle deviations
-                    from the intended yaw angles (deg).
-                -   **yaw_unc_pmf** (*np.array*): The probability
-                    of each yaw angle deviation in **yaw_unc** occuring.
-
-                If none are specified, default PMFs are calculated using
-                values provided in **unc_options**. Defaults to None.
-            unc_options (dictionary, optional): A dictionary containing values
-                used to create normally-distributed, zero-mean probability mass
-                functions describing the distribution of wind direction and yaw
-                position deviations when wind direction and/or yaw position
-                uncertainty is included. This argument is only used when
-                **unc_pmfs** is None and contains the following key-value pairs:
-
-                -   **std_wd** (*float*): The standard deviation of
-                    the wind direction deviations from the original wind
-                    direction (deg).
-                -   **std_yaw** (*float*): The standard deviation of
-                    the yaw angle deviations from the original yaw angles (deg).
-                -   **pmf_res** (*float*): The resolution in degrees
-                    of the wind direction and yaw angle PMFs.
-                -   **pdf_cutoff** (*float*): The cumulative
-                    distribution function value at which the tails of the
-                    PMFs are truncated.
-
-                If none are specified, default values of
-                {'std_wd': 4.95, 'std_yaw': 1.75, 'pmf_res': 1.0,
-                'pdf_cutoff': 0.995} are used. Defaults to None.
             turbine_weights (iterable, optional): weighing terms that allow
                 the user to emphasize power gains at particular turbines or
                 completely ignore power gains from other turbines. The array
                 of turbine powers from floris is multiplied with this array
                 in the calculation of the objective function. If None, this
                 is an array with all values 1.0 and length equal to the
                 number of turbines. Defaults to None.
@@ -154,507 +83,537 @@
                 automatically finds and excludes turbines that are most
                 downstream from the optimization problem. This significantly
                 reduces computation time at no loss in performance. The yaw
                 angles of these downstream turbines are fixed to 0.0 deg if
                 the yaw bounds specified in self.bnds allow that, or otherwise
                 are fixed to the lower or upper yaw bound, whichever is closer
                 to 0.0. Defaults to False.
-        """
-        super().__init__(fi)
+            verify_convergence (bool, optional): specifies whether the found
+                optimal yaw angles will be checked for accurately convergence.
+                With large farms, especially when using SciPy or other global
+                optimization methods, solutions do not always converge and
+                turbines that should have a 0.0 deg actually have a 1.0 deg
+                angle, for example. By enabling this function, the final yaw
+                angles are compared to their baseline values one-by-one for
+                the turbines to make sure no such convergence issues arise.
+                Defaults to False.
+        """
+
+        # Save turbine object to self
+        self.fmodel = fmodel.copy()
+        self.nturbs = len(self.fmodel.layout_x)
+
+        # # Check floris options
+        # if self.fmodel.core.flow_field.n_wind_speeds > 1:
+        #     raise NotImplementedError(
+        #         "Optimizer currently does not support more than one wind" +
+        #         " speed. Please assign FLORIS a single wind speed."
+        #     )
 
-        if opt_options is None:
-            self.opt_options = {
-                "maxiter": 50,
-                "disp": True,
-                "iprint": 2,
-                "ftol": 1e-12,
-                "eps": 0.1,
-            }
-
-        self.unc_pmfs = unc_pmfs
-
-        if unc_options is None:
-            self.unc_options = {
-                "std_wd": 4.95,
-                "std_yaw": 1.75,
-                "pmf_res": 1.0,
-                "pdf_cutoff": 0.995,
-            }
-
-        self.reinitialize_opt(
-            minimum_yaw_angle=minimum_yaw_angle,
-            maximum_yaw_angle=maximum_yaw_angle,
-            yaw_angles_baseline=yaw_angles_baseline,
-            x0=x0,
-            bnds=bnds,
-            opt_method=opt_method,
-            opt_options=opt_options,
-            include_unc=include_unc,
-            unc_pmfs=unc_pmfs,
-            unc_options=unc_options,
-            turbine_weights=turbine_weights,
-            calc_init_power=calc_init_power,
-            exclude_downstream_turbines=exclude_downstream_turbines,
-        )
+        # Initialize optimizer
+        self.verify_convergence = verify_convergence
+        if yaw_angles_baseline is not None:
+            yaw_angles_baseline = self._unpack_variable(yaw_angles_baseline)
+            self.yaw_angles_baseline = yaw_angles_baseline
+        else:
+            b = self.fmodel.core.farm.yaw_angles
+            self.yaw_angles_baseline = self._unpack_variable(b)
+            if np.any(np.abs(b) > 0.0):
+                print(
+                    "INFO: Baseline yaw angles were not specified and "
+                    "were derived from the floris object."
+                )
+                print(
+                    "INFO: The inherent yaw angles in the floris object "
+                    "are not all 0.0 degrees."
+                )
 
-    # Private methods
+        # Set optimization bounds
+        self.minimum_yaw_angle = self._unpack_variable(minimum_yaw_angle)
+        self.maximum_yaw_angle = self._unpack_variable(maximum_yaw_angle)
 
-    def _yaw_power_opt(self, yaw_angles_subset_norm):
-        # Unnorm subset
-        yaw_angles_subset = self._unnorm(
-            np.array(yaw_angles_subset_norm),
-            self.minimum_yaw_angle,
-            self.maximum_yaw_angle,
-        )
-        # Create a full yaw angle array
-        yaw_angles = np.array(self.yaw_angles_template, copy=True)
-        yaw_angles[self.turbs_to_opt] = yaw_angles_subset
-
-        self.fi.calculate_wake(yaw_angles=yaw_angles)
-        turbine_powers = self.fi.get_turbine_power(
-            include_unc=self.include_unc,
-            unc_pmfs=self.unc_pmfs,
-            unc_options=self.unc_options,
-        )
+        # Set initial condition for optimization
+        if x0 is not None:
+            self.x0 = self._unpack_variable(x0)
+        else:
+            self.x0 = self._unpack_variable(0.0)
+            for ti in range(self.nturbs):
+                yaw_lb = self.minimum_yaw_angle[:, ti]
+                yaw_ub = self.maximum_yaw_angle[:, ti]
+                idx = (yaw_lb > 0.0) | (yaw_ub < 0.0)
+                self.x0[idx, ti] = (yaw_lb[idx] + yaw_ub[idx]) / 2.0
 
-        return (
-            -1.0
-            * np.dot(self.turbine_weights, turbine_powers)
-            / self.initial_farm_power
-        )
+        # Check inputs for consistency
+        if np.any(self.yaw_angles_baseline < self.minimum_yaw_angle):
+            print("INFO: yaw_angles_baseline exceed lower bound constraints.")
+        if np.any(self.yaw_angles_baseline > self.maximum_yaw_angle):
+            print("INFO: yaw_angles_baseline exceed upper bound constraints.")
+        if np.any(self.x0 < self.minimum_yaw_angle):
+            raise ValueError("Initial guess x0 exceeds lower bound constraints.")
+        if np.any(self.x0 > self.maximum_yaw_angle):
+            raise ValueError("Initial guess x0 exceeds upper bound constraints.")
 
-    def _optimize(self):
-        """
-        Find optimum setting of turbine yaw angles for power production
-        given fixed atmospheric conditins (wind speed, direction, etc.).
+        # Define turbine weighing terms
+        if turbine_weights is None:
+            self.turbine_weights = self._unpack_variable(1.0)
+        else:
+            self.turbine_weights = self._unpack_variable(turbine_weights)
 
-        Returns:
-            opt_yaw_angles (np.array): optimal yaw angles of each turbine.
-        """
-        opt_yaw_angles = np.array(self.yaw_angles_template, copy=True)
-        self._reduce_control_variables()
-        if len(self.turbs_to_opt) > 0:
-            self.residual_plant = minimize(
-                self._yaw_power_opt,
-                self.x0_norm,
-                method=self.opt_method,
-                bounds=self.bnds_norm,
-                options=self.opt_options,
-            )
+        # Save remaining user options to self
+        self.normalize_variables = normalize_control_variables
+        self.calc_baseline_power = calc_baseline_power
+        self.exclude_downstream_turbines = exclude_downstream_turbines
+
+
+        # Prepare for optimization and calculate baseline powers (if applic.)
+        self._initialize()
+        self._calculate_baseline_farm_power()
+
+        # Initialize optimal yaw angles and cost function as baseline values
+        self._yaw_angles_opt_subset = copy.deepcopy(self._yaw_angles_baseline_subset)
+        self._farm_power_opt_subset = copy.deepcopy(self._farm_power_baseline_subset)
+        self._yaw_lbs = copy.deepcopy(self._minimum_yaw_angle_subset)
+        self._yaw_ubs = copy.deepcopy(self._maximum_yaw_angle_subset)
 
-            opt_yaw_angles_subset = self._unnorm(
-                self.residual_plant.x, self.minimum_yaw_angle, self.maximum_yaw_angle
+    # Private methods
+
+    def _initialize(self):
+        # Reduce optimization problem as much as possible
+        self._reduce_control_problem()
+
+        # Normalize optimization variables
+        if self.normalize_variables:
+            self._normalize_control_problem()
+
+    def _unpack_variable(self, variable, subset=False):
+        """Take a variable, can be either a float, a list equal in
+        length to the number of turbines, or an ndarray. It then
+        upsamples this value so that it always matches the dimensions
+        (self.nconds, self.nturbs).
+        """
+        # Deal with full vs. subset dimensions
+        nturbs = self.nturbs
+        if subset:
+            nturbs = np.shape(self._x0_subset.shape[1])
+
+        # Then process maximum yaw angle
+        if isinstance(variable, (int, float)):
+            # If single value, copy over to all turbines
+            variable = np.tile(variable, (nturbs))
+
+        variable = np.array(variable, dtype=float)
+        if len(np.shape(variable)) == 1:
+            # If one-dimensional array, copy over to all atmos. conditions
+            variable = np.tile(
+                variable,
+                (self.fmodel.core.flow_field.n_findex, 1)
             )
-            opt_yaw_angles[self.turbs_to_opt] = opt_yaw_angles_subset
 
-        return opt_yaw_angles
 
-    def _set_opt_bounds(self, minimum_yaw_angle, maximum_yaw_angle):
-        self.bnds = [(minimum_yaw_angle, maximum_yaw_angle) for _ in range(self.nturbs)]
+        return variable
 
-    def _reduce_control_variables(self):
-        """This function reduces the control problem by eliminating turbines
+    def _reduce_control_problem(self):
+        """
+        This function reduces the control problem by eliminating turbines
         of which the yaw angles need not be optimized, either because of a
         user-specified set of bounds (where bounds[i][0] == bounds[i][1]),
         or alternatively turbines that are far downstream in the wind farm
-        and of which the wake does not impinge other turbines, if the
-        boolean exclude_downstream_turbines == True. The normalized initial
-        conditions and bounds are then calculated for the subset of turbines,
-        to be used in the optimization.
+        and of which the wake does not impinge other turbines, if
+        exclude_downstream_turbines == True.
         """
-        if self.bnds is not None:
-            self.turbs_to_opt, _ = np.where(np.abs(np.diff(self.bnds)) >= 0.001)
-        else:
-            self.turbs_to_opt = np.array(range(self.nturbs), dtype=int)
+        # Initialize which turbines to optimize for
+        self.turbs_to_opt = (self.maximum_yaw_angle - self.minimum_yaw_angle >= 0.001)
+
+        # Initialize subset variables as full set
+        self.fmodel_subset = self.fmodel.copy()
+        n_findex_subset = copy.deepcopy(self.fmodel.core.flow_field.n_findex)
+        minimum_yaw_angle_subset = copy.deepcopy(self.minimum_yaw_angle)
+        maximum_yaw_angle_subset = copy.deepcopy(self.maximum_yaw_angle)
+        x0_subset = copy.deepcopy(self.x0)
+        turbs_to_opt_subset = copy.deepcopy(self.turbs_to_opt)
+        turbine_weights_subset = copy.deepcopy(self.turbine_weights)
+        yaw_angles_template_subset = self._unpack_variable(0.0)
+        yaw_angles_baseline_subset = copy.deepcopy(self.yaw_angles_baseline)
 
+        # Define which turbines to optimize for
         if self.exclude_downstream_turbines:
-            # Remove turbines from turbs_to_opt that are downstream
-            downstream_turbines = derive_downstream_turbines(
-                fi=self.fi, wind_direction=self.fi.floris.farm.wind_direction[0]
-            )
-            downstream_turbines = np.array(downstream_turbines, dtype=int)
-            self.turbs_to_opt = [
-                i for i in self.turbs_to_opt if i not in downstream_turbines
-            ]
+            for iw, wd in enumerate(self.fmodel.core.flow_field.wind_directions):
+                # Remove turbines from turbs_to_opt that are downstream
+                downstream_turbines = derive_downstream_turbines(self.fmodel, wd)
+                downstream_turbines = np.array(downstream_turbines, dtype=int)
+                self.turbs_to_opt[iw, downstream_turbines] = False
+                turbs_to_opt_subset = copy.deepcopy(self.turbs_to_opt)  # Update
 
         # Set up a template yaw angles array with default solutions. The default
         # solutions are either 0.0 or the allowable yaw angle closest to 0.0 deg.
         # This solution addresses both downstream turbines, minimizing their abs.
         # yaw offset, and additionally fixing equality-constrained turbines to
         # their appropriate yaw angle.
-        yaw_angles_template = np.zeros(self.nturbs, dtype=float)
-        for ti in range(self.nturbs):
-            if (self.bnds[ti][0] > 0.0) | (self.bnds[ti][1] < 0.0):
-                yaw_angles_template[ti] = self.bnds[ti][
-                    np.argmin(np.abs(self.bnds[ti]))
-                ]
-        self.yaw_angles_template = yaw_angles_template
-
-        # Derive normalized initial condition and bounds
-        x0_subset = [self.x0[i] for i in self.turbs_to_opt]
-        self.x0_norm = self._norm(
-            np.array(x0_subset), self.minimum_yaw_angle, self.maximum_yaw_angle
-        )
-        self.bnds_norm = [
-            (
-                self._norm(
-                    self.bnds[i][0], self.minimum_yaw_angle, self.maximum_yaw_angle
-                ),
-                self._norm(
-                    self.bnds[i][1], self.minimum_yaw_angle, self.maximum_yaw_angle
+        idx = (minimum_yaw_angle_subset > 0.0) | (maximum_yaw_angle_subset < 0.0)
+        if np.any(idx):
+            # Find bounds closest to 0.0 deg
+            combined_bounds = np.concatenate(
+                (
+                    np.expand_dims(minimum_yaw_angle_subset, axis=3),
+                    np.expand_dims(maximum_yaw_angle_subset, axis=3)
                 ),
+                axis=3
             )
-            for i in self.turbs_to_opt
-        ]
-
-    # Public methods
+            # Overwrite all values that are not allowed to be 0.0 with bound value closest to zero
+            ids_closest = np.expand_dims(np.argmin(np.abs(combined_bounds), axis=3), axis=3)
+            yaw_mb = np.squeeze(np.take_along_axis(combined_bounds, ids_closest, axis=3))
+            yaw_angles_template_subset[idx] = yaw_mb[idx]
+
+        # Save all subset variables to self
+        self._n_findex_subset = n_findex_subset
+        self._minimum_yaw_angle_subset = minimum_yaw_angle_subset
+        self._maximum_yaw_angle_subset = maximum_yaw_angle_subset
+        self._x0_subset = x0_subset
+        self._turbs_to_opt_subset = turbs_to_opt_subset
+        self._turbine_weights_subset = turbine_weights_subset
+        self._yaw_angles_template_subset = yaw_angles_template_subset
+        self._yaw_angles_baseline_subset = yaw_angles_baseline_subset
+
+    def _normalize_control_problem(self):
+        """
+        This private function normalizes variables for the optimization
+        problem, specifically the initial condition x0 and the bounds.
+        Normalization can improve optimization performance when using common
+        optimization methods such as the SciPy Optimization Toolbox.
+        """
+        lb = np.min(self._minimum_yaw_angle_subset)
+        ub = np.max(self._maximum_yaw_angle_subset)
+        self._normalization_length = (ub - lb)
+        self._x0_subset_norm = self._x0_subset / self._normalization_length
+        self._minimum_yaw_angle_subset_norm = (
+            self._minimum_yaw_angle_subset
+            / self._normalization_length
+        )
+        self._maximum_yaw_angle_subset_norm = (
+            self._maximum_yaw_angle_subset
+            / self._normalization_length
+        )
 
-    def optimize(self, verbose=True):
+    def _calculate_farm_power(
+            self,
+            yaw_angles=None,
+            wd_array=None,
+            ws_array=None,
+            ti_array=None,
+            turbine_weights=None,
+            heterogeneous_speed_multipliers=None,
+        ):
         """
-        This method solves for the optimum turbine yaw angles for power
-        production given a fixed set of atmospheric conditions
-        (wind speed, direction, etc.).
+        Calculate the wind farm power production assuming the predefined
+        probability distribution (self.unc_options/unc_pmf), with the
+        appropriate weighing terms, and for a specific set of yaw angles.
+
+        Args:
+            yaw_angles (iterable, optional): Array or list of yaw angles in degrees.
+                Defaults to None.
+            wd_array (iterable, optional): Array or list of wind directions in degrees.
+                Defaults to None.
+            ws_array (iterable, optional): Array or list of wind speeds in m/s. Defaults to None.
+            ti_array (iterable, optional): Array or list of turbulence intensities.
+                Defaults to None.
+            turbine_weights (iterable, optional): Array or list of weights to apply to the turbine
+                powers. Defaults to None.
+            heterogeneous_speed_multipliers (iterable, optional): Array or list of speed up factors
+                for heterogeneous inflow. Defaults to None.
+
 
         Returns:
-            np.array: Optimal yaw angles for each turbine (deg).
+            farm_power (float): Weighted wind farm power.
         """
-        if verbose:
-            print("=====================================================")
-            print("Optimizing wake redirection control...")
-            print("Number of parameters to optimize = ", len(self.turbs_to_opt))
-            print("=====================================================")
-
-        opt_yaw_angles = self._optimize()
-
-        if verbose and np.sum(opt_yaw_angles) == 0:
-            print(
-                "No change in controls suggested for this inflow \
-                   condition..."
+        # Unpack all variables, whichever are defined.
+        fmodel_subset = copy.deepcopy(self.fmodel_subset)
+        if wd_array is None:
+            wd_array = fmodel_subset.core.flow_field.wind_directions
+        if ws_array is None:
+            ws_array = fmodel_subset.core.flow_field.wind_speeds
+        if ti_array is None:
+            ti_array = fmodel_subset.core.flow_field.turbulence_intensities
+        if yaw_angles is None:
+            yaw_angles = self._yaw_angles_baseline_subset
+        if turbine_weights is None:
+            turbine_weights = self._turbine_weights_subset
+        if heterogeneous_speed_multipliers is not None:
+            fmodel_subset.core.flow_field.\
+                heterogeneous_inflow_config['speed_multipliers'] = heterogeneous_speed_multipliers
+
+        # Ensure format [incompatible with _subset notation]
+        yaw_angles = self._unpack_variable(yaw_angles, subset=True)
+
+        # # Correct wind direction definition: 270 deg is from left, cw positive
+        # wd_array = wrap_360(wd_array)
+
+        # Calculate solutions
+        turbine_power = np.zeros_like(self._minimum_yaw_angle_subset[:, :])
+        fmodel_subset.set(
+            wind_directions=wd_array,
+            wind_speeds=ws_array,
+            turbulence_intensities=ti_array,
+            yaw_angles=yaw_angles,
+        )
+        fmodel_subset.run()
+        turbine_power = fmodel_subset.get_turbine_powers()
+
+        # Multiply with turbine weighing terms
+        turbine_power_weighted = np.multiply(turbine_weights, turbine_power)
+        farm_power_weighted = np.sum(turbine_power_weighted, axis=1)
+        return farm_power_weighted
+
+    def _calculate_baseline_farm_power(self):
+        """
+        Calculate the weighted wind farm power under the baseline turbine yaw
+        angles.
+        """
+        if self.calc_baseline_power:
+            P = self._calculate_farm_power(self._yaw_angles_baseline_subset)
+            self._farm_power_baseline_subset = P
+            self.farm_power_baseline = P
+        else:
+            self._farm_power_baseline_subset = None
+            self.farm_power_baseline = None
+
+    def _finalize(self, farm_power_opt_subset=None, yaw_angles_opt_subset=None):
+        # Process final solutions
+        if farm_power_opt_subset is None:
+            farm_power_opt_subset = self._farm_power_opt_subset
+        if yaw_angles_opt_subset is None:
+            yaw_angles_opt_subset = self._yaw_angles_opt_subset
+
+        # Now verify solutions for convergence, if necessary
+        if self.verify_convergence:
+            yaw_angles_opt_subset, farm_power_opt_subset = (
+                self._verify_solutions_for_convergence(
+                    farm_power_opt_subset,
+                    yaw_angles_opt_subset
+                )
             )
 
-        return opt_yaw_angles
+        # Finalization step for optimization: undo reduction step
+        self.farm_power_opt = farm_power_opt_subset
+        self.yaw_angles_opt = yaw_angles_opt_subset
+
+        # Produce output table
+        df_list = []
+        df_list.append(
+            pd.DataFrame(
+                {
+                    "wind_direction": self.fmodel.core.flow_field.wind_directions,
+                    "wind_speed": self.fmodel.core.flow_field.wind_speeds,
+                    "turbulence_intensity": self.fmodel.core.flow_field.turbulence_intensities,
+                    "yaw_angles_opt": list(self.yaw_angles_opt[:, :]),
+                    "farm_power_opt": None
+                    if self.farm_power_opt is None
+                    else self.farm_power_opt[:],
+                    "farm_power_baseline": None
+                    if self.farm_power_baseline is None
+                    else self.farm_power_baseline[:],
+                }
+            )
+        )
+        df_opt = pd.concat(df_list, axis=0)
 
-    def reinitialize_opt(
+        return df_opt
+
+    def _verify_solutions_for_convergence(
         self,
-        minimum_yaw_angle=None,
-        maximum_yaw_angle=None,
-        yaw_angles_baseline=None,
-        x0=None,
-        bnds=None,
-        opt_method=None,
-        opt_options=None,
-        include_unc=None,
-        unc_pmfs=None,
-        unc_options=None,
-        turbine_weights=None,
-        calc_init_power=True,
-        exclude_downstream_turbines=None,
+        farm_power_opt_subset,
+        yaw_angles_opt_subset,
+        min_yaw_offset=0.01,
+        min_power_gain_for_yaw=0.02,
+        verbose=True,
     ):
         """
-        This method reinitializes any optimization parameters that are
-        specified. Otherwise, the current parameter values are kept.
+        This function verifies whether the found solutions (yaw_angles_opt)
+        have any nonzero yaw angles that are actually a result of incorrect
+        convergence. By evaluating the power production by setting each turbine's
+        yaw angle to 0.0 deg, one by one, we verify that the found
+        optimal values do in fact lead to a nonzero power production gain.
 
         Args:
-            minimum_yaw_angle (float, optional): Minimum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to None.
-            maximum_yaw_angle (float, optional): Maximum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to None.
-            yaw_angles_baseline (iterable, optional): The baseline yaw
-                angles used to calculate the initial and baseline power
-                production in the wind farm and used to normalize the cost
-                function. If none are specified, this variable is set equal
-                to the current yaw angles in floris. Note that this variable
-                need not meet the yaw constraints specified in self.bnds,
-                yet a warning is raised if it does to inform the user.
-                Defaults to None.
-            x0 (iterable, optional): The initial guess for the optimization
-                problem. These values must meet the constraints specified
-                in self.bnds. Note that, if exclude_downstream_turbines=True,
-                the initial guess for any downstream turbines are ignored
-                since they are not part of the optimization. Instead, the yaw
-                angles for those turbines are 0.0 if that meets the lower and
-                upper bound, or otherwise as close to 0.0 as feasible. If no
-                values for x0 are specified, x0 is set to be equal to zeros
-                wherever feasible (w.r.t. the bounds), and equal to the
-                average of its lower and upper bound for all non-downstream
-                turbines otherwise. Defaults to None.
-            bnds (iterable, optional): Bounds for the yaw angles, as tuples of
-                min, max values for each turbine (deg). One can fix the yaw
-                angle of certain turbines to a predefined value by setting that
-                turbine's lower bound equal to its upper bound (i.e., an
-                equality constraint), as: bnds[ti] = (x, x), where x is the
-                fixed yaw angle assigned to the turbine. This works for both
-                zero and nonzero yaw angles. Moreover, if
-                exclude_downstream_turbines=True, the yaw angles for all
-                downstream turbines will be 0.0 or a feasible value closest to
-                0.0. If none are specified, the bounds are set to
-                (minimum_yaw_angle, maximum_yaw_angle) for each turbine. Note
-                that, if bnds is not none, its values overwrite any value given
-                in minimum_yaw_angle and maximum_yaw_angle. Defaults to None.
-            opt_method (str, optional): The optimization method used by
-                scipy.optimize.minize. Defaults to None.
-            opt_options (dictionary, optional): Optimization options used by
-                scipy.optimize.minize. Defaults to None.
-            include_unc (bool, optional): Determines whether wind direction or
-                yaw uncertainty are included. If True, uncertainty in wind
-                direction and/or yaw position is included when determining
-                wind farm power. Uncertainty is included by computing the
-                mean wind farm power for a distribution of wind direction
-                and yaw position deviations from the intended wind direction
-                and yaw angles. Defaults to None.
-            unc_pmfs (dictionary, optional): A dictionary containing
-                probability mass functions describing the distribution of
-                wind direction and yaw position deviations when wind direction
-                and/or yaw position uncertainty is included in the power
-                calculations. Contains the following key-value pairs:
-
-                -   **wd_unc** (*np.array*): The wind direction
-                    deviations from the intended wind direction (deg).
-                -   **wd_unc_pmf** (*np.array*): The probability
-                    of each wind direction deviation in **wd_unc** occuring.
-                -   **yaw_unc** (*np.array*): The yaw angle deviations
-                    from the intended yaw angles (deg).
-                -   **yaw_unc_pmf** (*np.array*): The probability
-                    of each yaw angle deviation in **yaw_unc** occuring.
-
-                If none are specified, default PMFs are calculated using
-                values provided in **unc_options**. Defaults to None.
-            unc_options (dictionary, optional): A dictionary containing values
-                used to create normally-distributed, zero-mean probability mass
-                functions describing the distribution of wind direction and yaw
-                position deviations when wind direction and/or yaw position
-                uncertainty is included. This argument is only used when
-                **unc_pmfs** is None and contains the following key-value pairs:
-
-                -   **std_wd** (*float*): The standard deviation of
-                    the wind direction deviations from the original wind
-                    direction (deg).
-                -   **std_yaw** (*float*): The standard deviation of
-                    the yaw angle deviations from the original yaw angles (deg).
-                -   **pmf_res** (*float*): The resolution in degrees
-                    of the wind direction and yaw angle PMFs.
-                -   **pdf_cutoff** (*float*): The cumulative
-                    distribution function value at which the tails of the
-                    PMFs are truncated.
-
-                If none are specified, default values of
-                {'std_wd': 4.95, 'std_yaw': 1.75, 'pmf_res': 1.0,
-                'pdf_cutoff': 0.995} are used. Defaults to None.
-            turbine_weights (iterable, optional): weighing terms that allow
-                the user to emphasize power gains at particular turbines or
-                completely ignore power gains from other turbines. The array
-                of turbine powers from floris is multiplied with this array
-                in the calculation of the objective function. If None, this
-                is an array with all values 1.0 and length equal to the
-                number of turbines. Defaults to None.
-            calc_init_power (bool, optional): If True, calculates initial
-                wind farm power for each set of wind conditions. Defaults to
-                None.
-            exclude_downstream_turbines (bool, optional): If True,
-                automatically finds and excludes turbines that are most
-                downstream from the optimization problem. This significantly
-                reduces computation time at no loss in performance. The yaw
-                angles of these downstream turbines are fixed to 0.0 deg if
-                the yaw bounds specified in self.bnds allow that, or otherwise
-                are fixed to the lower or upper yaw bound, whichever is closer
-                to 0.0. Defaults to None.
-        """
-        if minimum_yaw_angle is not None:
-            self.minimum_yaw_angle = minimum_yaw_angle
-        if maximum_yaw_angle is not None:
-            self.maximum_yaw_angle = maximum_yaw_angle
-        if yaw_angles_baseline is not None:
-            self.yaw_angles_baseline = yaw_angles_baseline
-        else:
-            self.yaw_angles_baseline = [
-                turbine.yaw_angle
-                for turbine in self.fi.floris.farm.turbine_map.turbines
-            ]
-            if any(np.abs(self.yaw_angles_baseline) > 0.0):
-                print(
-                    "INFO: Baseline yaw angles were not specified and were derived "
-                    "from the floris object."
-                )
-                print(
-                    "INFO: The inherent yaw angles in the floris object are not all 0.0 degrees."
-                )
+            farm_power_opt_subset (iterable): Array with the optimal wind
+            farm power values (i.e., farm powers with yaw_angles_opt_subset).
+            yaw_angles_opt_subset (iterable): Array with the optimal yaw angles
+            for all turbines in the farm (or for all the to-be-optimized
+            turbines in the farm). The yaw angles in this array will be
+            verified.
+            min_yaw_offset (float, optional): Values that differ by less than
+            this amount compared to the baseline value will be assumed to be
+            too small to make any notable difference. Therefore, for practical
+            reasons, the value is overwritten by its baseline value (which
+            typically is 0.0 deg). Defaults to 0.01.
+            min_power_gain_for_yaw (float, optional): The minimum percentage
+            uplift a turbine must create in the farm power production for its
+            yaw offset to be considered non negligible. Set to 0.0 to ignore
+            this criteria. Defaults to 0.02 (implying 0.02%).
+            verbose (bool, optional): Print to console. Defaults to True.
+        Returns:
+            x_opt (iterable): Array with the optimal yaw angles, possibly
+            with certain values being set to 0.0 deg as they were found
+            to be a result of incorrect convergence. If the optimization
+            has perfectly converged, x_opt will be identical to the user-
+            provided input yaw_angles_opt.
+        """
+
+        print("Verifying convergence of the found optimal yaw angles.")
+
+        # Start timer
+        start_time = timerpc()
+
+        # Define variables locally
+        yaw_angles_opt_subset = np.array(yaw_angles_opt_subset, copy=True)
+        yaw_angles_baseline_subset = self._yaw_angles_baseline_subset
+        farm_power_baseline_subset = self._farm_power_baseline_subset
+        turbs_to_opt_subset = self._turbs_to_opt_subset
+
+        # Round small nonzero yaw angles to zero
+        ydiff = np.abs(yaw_angles_opt_subset - yaw_angles_baseline_subset)
+        ids = np.where((ydiff < min_yaw_offset) & (ydiff > 0.0))
+        if len(ids[0]) > 0:
+            if verbose:
+                print(f"Rounding {len(ids)} insignificant yaw angles to their baseline value.")
+            yaw_angles_opt_subset[ids] = yaw_angles_baseline_subset[ids]
+            ydiff[ids] = 0.0
+
+        # Turbines to test whether their angles sufficiently improve farm power
+        ids = np.where((turbs_to_opt_subset) & (ydiff > min_yaw_offset))
+
+        # Define situations that need to be calculated and find farm power.
+        # Each situation basically contains the exact same conditions as the
+        # baseline conditions and optimal yaw angles, besides for a single
+        # turbine for which its yaw angle was set to its baseline value (
+        # typically 0.0 deg). This way, we investigate whether the yaw offset
+        # of that turbine really adds significant uplift to the farm power
+        # production.
+
+        # For each turbine in the farm, reset its values to baseline. Thus,
+        # we copy the atmospheric conditions n_turbs times and for each
+        # copy of atmospheric conditions, we reset that turbine's yaw angle
+        # to its baseline value for all conditions.
+        n_turbs = len(self.fmodel.layout_x)
+        sp = (n_turbs, 1)  # Tile shape for matrix expansion
+        wd_array_nominal = self.fmodel_subset.core.flow_field.wind_directions
+        ws_array_nominal = self.fmodel_subset.core.flow_field.wind_speeds
+        ti_array_nominal = self.fmodel_subset.core.flow_field.turbulence_intensities
+        n_wind_directions = len(wd_array_nominal)
+        yaw_angles_verify = np.tile(yaw_angles_opt_subset, sp)
+        yaw_angles_bl_verify = np.tile(yaw_angles_baseline_subset, sp)
+        turbine_id_array = np.zeros(np.shape(yaw_angles_verify)[0], dtype=int)
+        for ti in range(n_turbs):
+            ids = ti * n_wind_directions + np.arange(n_wind_directions)
+            yaw_angles_verify[ids, ti] = yaw_angles_bl_verify[ids, ti]
+            turbine_id_array[ids] = ti
+
+        # Now evaluate all situations
+        farm_power_baseline_verify = np.tile(farm_power_baseline_subset, (n_turbs))
+        farm_power = self._calculate_farm_power(
+            yaw_angles=yaw_angles_verify,
+            wd_array=np.tile(wd_array_nominal, n_turbs),
+            ws_array=np.tile(ws_array_nominal, n_turbs),
+            ti_array=np.tile(ti_array_nominal, n_turbs),
+            turbine_weights=np.tile(self._turbs_to_opt_subset, sp)
+        )
 
-        self.bnds = bnds
-        if bnds is not None:
-            self.minimum_yaw_angle = np.min([bnds[i][0] for i in range(self.nturbs)])
-            self.maximum_yaw_angle = np.max([bnds[i][1] for i in range(self.nturbs)])
-        else:
-            self._set_opt_bounds(self.minimum_yaw_angle, self.maximum_yaw_angle)
+        # Calculate power uplift for optimal solutions
+        uplift_o = 100 * (
+            np.tile(farm_power_opt_subset, (n_turbs)) /
+            farm_power_baseline_verify - 1.0
+        )
 
-        if x0 is not None:
-            self.x0 = x0
-        else:
-            self.x0 = np.zeros(self.nturbs, dtype=float)
-            for ti in range(self.nturbs):
-                if (self.bnds[ti][0] > 0.0) | (self.bnds[ti][1] < 0.0):
-                    self.x0[ti] = np.mean(self.bnds[ti])
+        # Calculate power uplift for all cases we evaluated
+        uplift_n = 100.0 * (farm_power / farm_power_baseline_verify - 1.0)
 
-        if any(
-            np.array(self.yaw_angles_baseline) < np.array([b[0] for b in self.bnds])
-        ):
-            print("INFO: yaw_angles_baseline exceed lower bound constraints.")
-        if any(
-            np.array(self.yaw_angles_baseline) > np.array([b[1] for b in self.bnds])
-        ):
-            print("INFO: yaw_angles_baseline in FLORIS exceed upper bound constraints.")
-        if any(np.array(self.x0) < np.array([b[0] for b in self.bnds])):
-            raise ValueError("Initial guess x0 exceeds lower bound constraints.")
-        if any(np.array(self.x0) > np.array([b[1] for b in self.bnds])):
-            raise ValueError("Initial guess x0 exceeds upper bound constraints.")
+        # Check difference in uplift, where each row represents a different
+        # situation (i.e., where one turbine was set to its baseline yaw angle
+        # instead of its optimal yaw angle).
+        dp = uplift_o - uplift_n
+        ids_to_simplify = np.where(dp < min_power_gain_for_yaw)
+        ids_to_simplify = (
+            np.remainder(ids_to_simplify[0], n_wind_directions),  # Wind direction identifier
+            turbine_id_array[ids_to_simplify[0]],  # Turbine identifier
+        )
 
-        if opt_method is not None:
-            self.opt_method = opt_method
-        if opt_options is not None:
-            self.opt_options = opt_options
-        if include_unc is not None:
-            self.include_unc = include_unc
-        if unc_pmfs is not None:
-            self.unc_pmfs = unc_pmfs
-        if unc_options is not None:
-            self.unc_options = unc_options
-
-        if self.include_unc & (self.unc_pmfs is None):
-            if self.unc_options is None:
-                self.unc_options = {
-                    "std_wd": 4.95,
-                    "std_yaw": 1.75,
-                    "pmf_res": 1.0,
-                    "pdf_cutoff": 0.995,
-                }
+        # Overwrite yaw angles that insufficiently increased farm power with baseline values
+        yaw_angles_opt_subset[ids_to_simplify] = (
+            yaw_angles_baseline_subset[ids_to_simplify]
+        )
 
-            # create normally distributed wd and yaw uncertainty pmfs
-            if self.unc_options["std_wd"] > 0:
-                wd_bnd = int(
-                    np.ceil(
-                        norm.ppf(
-                            self.unc_options["pdf_cutoff"],
-                            scale=self.unc_options["std_wd"],
-                        )
-                        / self.unc_options["pmf_res"]
-                    )
-                )
-                wd_unc = np.linspace(
-                    -1 * wd_bnd * self.unc_options["pmf_res"],
-                    wd_bnd * self.unc_options["pmf_res"],
-                    2 * wd_bnd + 1,
+        n = len(ids_to_simplify[0])
+        if n > 0:
+            # Yaw angles notably changed: recalculate farm powers
+            farm_power_opt_subset_new = (
+                self._calculate_farm_power(yaw_angles_opt_subset)
+            )
+
+            if verbose:
+                # Calculate old uplift for all conditions
+                dP_old = 100.0 * (
+                    farm_power_opt_subset /
+                    farm_power_baseline_subset
+                ) - 100.0
+
+                # Calculate new uplift for all conditions
+                dP_new = 100.0 * (
+                    farm_power_opt_subset_new /
+                    farm_power_baseline_subset
+                ) - 100.0
+
+                # Calculate differences in power uplift
+                diff_uplift = dP_old - dP_new
+                ids_max_loss = np.where(np.nanmax(diff_uplift) == diff_uplift)
+                jj = (ids_max_loss[0][0], ids_max_loss[1][0])
+                ws_array_nominal = self.fmodel_subset.core.flow_field.wind_speeds
+                print(
+                    "Nullified the optimal yaw offset for {:d}".format(n) +
+                    " conditions and turbines."
                 )
-                wd_unc_pmf = norm.pdf(wd_unc, scale=self.unc_options["std_wd"])
-                # normalize so sum = 1.0
-                wd_unc_pmf = wd_unc_pmf / np.sum(wd_unc_pmf)
-            else:
-                wd_unc = np.zeros(1)
-                wd_unc_pmf = np.ones(1)
-
-            if self.unc_options["std_yaw"] > 0:
-                yaw_bnd = int(
-                    np.ceil(
-                        norm.ppf(
-                            self.unc_options["pdf_cutoff"],
-                            scale=self.unc_options["std_yaw"],
-                        )
-                        / self.unc_options["pmf_res"]
+                print(
+                    "Simplifying the yaw angles for these conditions lead " +
+                    "to a maximum change in wake-steering power uplift from "
+                    + "{:.5f}% to {:.5f}% at ".format(dP_old[jj], dP_new[jj])
+                    + " WD = {:.1f} deg and WS = {:.1f} m/s.".format(
+                        wd_array_nominal[jj[0]], ws_array_nominal[jj[1]],
                     )
                 )
-                yaw_unc = np.linspace(
-                    -1 * yaw_bnd * self.unc_options["pmf_res"],
-                    yaw_bnd * self.unc_options["pmf_res"],
-                    2 * yaw_bnd + 1,
-                )
-                yaw_unc_pmf = norm.pdf(yaw_unc, scale=self.unc_options["std_yaw"])
-                # normalize so sum = 1.0
-                yaw_unc_pmf = yaw_unc_pmf / np.sum(yaw_unc_pmf)
-            else:
-                yaw_unc = np.zeros(1)
-                yaw_unc_pmf = np.ones(1)
-
-            self.unc_pmfs = {
-                "wd_unc": wd_unc,
-                "wd_unc_pmf": wd_unc_pmf,
-                "yaw_unc": yaw_unc,
-                "yaw_unc_pmf": yaw_unc_pmf,
-            }
 
-        if turbine_weights is None:
-            self.turbine_weights = np.ones(self.nturbs)
-        else:
-            self.turbine_weights = np.array(turbine_weights, dtype=float)
-
-        if calc_init_power:
-            self.fi.calculate_wake(yaw_angles=self.yaw_angles_baseline)
-            turbine_powers = self.fi.get_turbine_power(
-                include_unc=self.include_unc,
-                unc_pmfs=self.unc_pmfs,
-                unc_options=self.unc_options,
-            )
-            self.initial_farm_power = np.dot(self.turbine_weights, turbine_powers)
-
-        if exclude_downstream_turbines is not None:
-            self.exclude_downstream_turbines = exclude_downstream_turbines
-        self._reduce_control_variables()
-
-    # Properties
-
-    @property
-    def minimum_yaw_angle(self):
-        """
-        The minimum yaw angle for the optimization. The setting-method
-        updates the optimization bounds accordingly.
-
-        **Note**: This is a virtual property used to "get" or "set" a value.
-
-        Args:
-            value (float): The minimum yaw angle to set (deg).
+                t = timerpc() - start_time
+                print(
+                    "Time spent to verify the convergence of the optimal " +
+                    "yaw angles: {:.3f} s.".format(t)
+                )
 
-        Returns:
-            float: The minimum yaw angle currently set (deg).
-        """
-        return self._minimum_yaw_angle
+            # Return optimal solutions to the user
+            farm_power_opt_subset = farm_power_opt_subset_new
 
-    @minimum_yaw_angle.setter
-    def minimum_yaw_angle(self, value):
-        self._minimum_yaw_angle = value
+        return yaw_angles_opt_subset, farm_power_opt_subset
 
-    @property
-    def maximum_yaw_angle(self):
+    # Supporting functions
+    def _norm(self, val, x1, x2):
         """
-        The maximum yaw angle for the optimization. The setting-method
-        updates the optimization bounds accordingly.
-
-        **Note**: This is a virtual property used to "get" or "set" a value.
+        Normalize a variable to a value range.
 
         Args:
-            value (float): The maximum yaw angle to set (deg).
+            val ([float]): Value to normalize.
+            x1 ([float]): Normalization lower bound.
+            x2 ([float]): Normalization upper bound.
 
         Returns:
-            float: The maximum yaw angle currently set (deg).
+            val_norm: Normalized variable.
         """
-        return self._maximum_yaw_angle
-
-    @maximum_yaw_angle.setter
-    def maximum_yaw_angle(self, value):
-        self._maximum_yaw_angle = value
+        return (val - x1) / (x2 - x1)
 
-    @property
-    def x0(self):
+    def _unnorm(self, val_norm, x1, x2):
         """
-        The initial yaw angles used for the optimization.
-
-        **Note**: This is a virtual property used to "get" or "set" a value.
+        Unnormalize a variable to a value range.
 
         Args:
-            value (iterable): The yaw angle initial conditions to set (deg).
+            val_norm ([float]): Normalized value.
+            x1 ([float]): Normalization lower bound.
+            x2 ([float]): Normalization upper bound.
 
         Returns:
-            list: The yaw angle initial conditions currently set (deg).
+            val: Unnormalized variable.
         """
-        return self._x0
-
-    @x0.setter
-    def x0(self, value):
-        self._x0 = value
+        return np.array(val_norm) * (x2 - x1) + x1
```

### Comparing `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_clustered.py` & `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_sr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,289 +1,311 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 import copy
+import warnings
+from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
 from floris.logging_manager import LoggingManager
 
-from .cluster_turbines import cluster_turbines
-from .yaw import YawOptimization
-
+# from .yaw_optimizer_scipy import YawOptimizationScipy
+from .yaw_optimization_base import YawOptimization
 
-class YawOptimizationClustered(YawOptimization, LoggingManager):
-    """
-    YawOptimization is a subclass of
-    :py:class:`~.tools.optimizationscipy.YawOptimization` that is used to
-    perform optimizations of the yaw angles of all or a subset of wind turbines
-    in a Floris Farm for a single set of inflow conditions using the scipy
-    optimization package. This class facilitates the clusterization of the
-    turbines inside seperate subsets in which the turbines witin each subset
-    exclusively interact with one another and have no impact on turbines
-    in other clusters. This may significantly reduce the computational
-    burden at no loss in performance (assuming the turbine clusters are truly
-    independent).
-    """
 
+class YawOptimizationSR(YawOptimization, LoggingManager):
     def __init__(
         self,
-        fi,
+        fmodel,
         minimum_yaw_angle=0.0,
         maximum_yaw_angle=25.0,
         yaw_angles_baseline=None,
         x0=None,
-        bnds=None,
-        opt_method="SLSQP",
-        opt_options=None,
-        include_unc=False,
-        unc_pmfs=None,
-        unc_options=None,
+        Ny_passes=[5, 4],  # Optimization options
         turbine_weights=None,
-        calc_init_power=True,
-        exclude_downstream_turbines=False,
-        clustering_wake_slope=0.30,
+        exclude_downstream_turbines=True,
+        verify_convergence=False,
     ):
         """
-        Instantiate YawOptimization object with a FlorisInterface object
+        Instantiate YawOptimizationSR object with a FlorisModel object
         and assign parameter values.
-
-        Args:
-            fi (:py:class:`~.tools.floris_interface.FlorisInterface`):
-                Interface used to interact with the Floris object.
-            minimum_yaw_angle (float, optional): Minimum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 0.0.
-            maximum_yaw_angle (float, optional): Maximum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 25.0.
-            yaw_angles_baseline (iterable, optional): The baseline yaw
-                angles used to calculate the initial and baseline power
-                production in the wind farm and used to normalize the cost
-                function. If none are specified, this variable is set equal
-                to the current yaw angles in floris. Note that this variable
-                need not meet the yaw constraints specified in self.bnds,
-                yet a warning is raised if it does to inform the user.
-                Defaults to None.
-            x0 (iterable, optional): The initial guess for the optimization
-                problem. These values must meet the constraints specified
-                in self.bnds. Note that, if exclude_downstream_turbines=True,
-                the initial guess for any downstream turbines are ignored
-                since they are not part of the optimization. Instead, the yaw
-                angles for those turbines are 0.0 if that meets the lower and
-                upper bound, or otherwise as close to 0.0 as feasible. If no
-                values for x0 are specified, x0 is set to be equal to zeros
-                wherever feasible (w.r.t. the bounds), and equal to the
-                average of its lower and upper bound for all non-downstream
-                turbines otherwise. Defaults to None.
-            bnds (iterable, optional): Bounds for the yaw angles, as tuples of
-                min, max values for each turbine (deg). One can fix the yaw
-                angle of certain turbines to a predefined value by setting that
-                turbine's lower bound equal to its upper bound (i.e., an
-                equality constraint), as: bnds[ti] = (x, x), where x is the
-                fixed yaw angle assigned to the turbine. This works for both
-                zero and nonzero yaw angles. Moreover, if
-                exclude_downstream_turbines=True, the yaw angles for all
-                downstream turbines will be 0.0 or a feasible value closest to
-                0.0. If none are specified, the bounds are set to
-                (minimum_yaw_angle, maximum_yaw_angle) for each turbine. Note
-                that, if bnds is not none, its values overwrite any value given
-                in minimum_yaw_angle and maximum_yaw_angle. Defaults to None.
-            opt_method (str, optional): The optimization method used by
-                scipy.optimize.minize. Defaults to 'SLSQP'.
-            opt_options (dictionary, optional): Optimization options used by
-                scipy.optimize.minize. If none are specified, they are set to
-                {'maxiter': 100, 'disp': False, 'iprint': 1, 'ftol': 1e-7,
-                'eps': 0.01}. Defaults to None.
-            include_unc (bool, optional): Determines whether wind direction or
-                yaw uncertainty are included. If True, uncertainty in wind
-                direction and/or yaw position is included when determining
-                wind farm power. Uncertainty is included by computing the
-                mean wind farm power for a distribution of wind direction
-                and yaw position deviations from the intended wind direction
-                and yaw angles. Defaults to False.
-            unc_pmfs (dictionary, optional): A dictionary containing
-                probability mass functions describing the distribution of
-                wind direction and yaw position deviations when wind direction
-                and/or yaw position uncertainty is included in the power
-                calculations. Contains the following key-value pairs:
-
-                -   **wd_unc** (*np.array*): The wind direction
-                    deviations from the intended wind direction (deg).
-                -   **wd_unc_pmf** (*np.array*): The probability
-                    of each wind direction deviation in **wd_unc** occuring.
-                -   **yaw_unc** (*np.array*): The yaw angle deviations
-                    from the intended yaw angles (deg).
-                -   **yaw_unc_pmf** (*np.array*): The probability
-                    of each yaw angle deviation in **yaw_unc** occuring.
-
-                If none are specified, default PMFs are calculated using
-                values provided in **unc_options**. Defaults to None.
-            unc_options (dictionary, optional): A dictionary containing values
-                used to create normally-distributed, zero-mean probability mass
-                functions describing the distribution of wind direction and yaw
-                position deviations when wind direction and/or yaw position
-                uncertainty is included. This argument is only used when
-                **unc_pmfs** is None and contains the following key-value pairs:
-
-                -   **std_wd** (*float*): The standard deviation of
-                    the wind direction deviations from the original wind
-                    direction (deg).
-                -   **std_yaw** (*float*): The standard deviation of
-                    the yaw angle deviations from the original yaw angles (deg).
-                -   **pmf_res** (*float*): The resolution in degrees
-                    of the wind direction and yaw angle PMFs.
-                -   **pdf_cutoff** (*float*): The cumulative
-                    distribution function value at which the tails of the
-                    PMFs are truncated.
-
-                If none are specified, default values of
-                {'std_wd': 4.95, 'std_yaw': 1.75, 'pmf_res': 1.0,
-                'pdf_cutoff': 0.995} are used. Defaults to None.
-            turbine_weights (iterable, optional): weighing terms that allow
-                the user to emphasize power gains at particular turbines or
-                completely ignore power gains from other turbines. The array
-                of turbine powers from floris is multiplied with this array
-                in the calculation of the objective function. If None, this
-                is an array with all values 1.0 and length equal to the
-                number of turbines. Defaults to None.
-            calc_init_power (bool, optional): If True, calculates initial
-                wind farm power for each set of wind conditions. Defaults to
-                True.
-            exclude_downstream_turbines (bool, optional): If True,
-                automatically finds and excludes turbines that are most
-                downstream from the optimization problem. This significantly
-                reduces computation time at no loss in performance. The yaw
-                angles of these downstream turbines are fixed to 0.0 deg if
-                the yaw bounds specified in self.bnds allow that, or otherwise
-                are fixed to the lower or upper yaw bound, whichever is closer
-                to 0.0. Defaults to False.
-            clustering_wake_slope (float, optional): linear slope of the wake
-                in the simplified linear expansion wake model (dy/dx). This
-                model is used to derive wake interactions between turbines and
-                to identify the turbine clusters. A good value is about equal
-                to the turbulence intensity in FLORIS. Though, since yaw
-                optimizations may shift the wake laterally, a safer option
-                is twice the turbulence intensity. The default value is 0.30
-                which should be valid for yaw optimizations at wd_std = 0.0 deg
-                and turbulence intensities up to 15%. Defaults to 0.30.
         """
+
+        # Initialize base class
         super().__init__(
-            fi=fi,
+            fmodel=fmodel,
             minimum_yaw_angle=minimum_yaw_angle,
             maximum_yaw_angle=maximum_yaw_angle,
             yaw_angles_baseline=yaw_angles_baseline,
             x0=x0,
-            bnds=bnds,
-            opt_method=opt_method,
-            opt_options=opt_options,
-            include_unc=include_unc,
-            unc_pmfs=unc_pmfs,
-            unc_options=unc_options,
             turbine_weights=turbine_weights,
-            calc_init_power=calc_init_power,
+            calc_baseline_power=True,
             exclude_downstream_turbines=exclude_downstream_turbines,
+            verify_convergence=verify_convergence,
         )
-        self.clustering_wake_slope = clustering_wake_slope
 
+        # Start a timer for FLORIS computations
+        self.time_spent_in_floris = 0
 
-    def _cluster_turbines(self):
-        wind_directions = self.fi.floris.farm.wind_direction
-        if (np.std(wind_directions) > 0.001):
-            raise ValueError("Wind directions must be uniform for clustering algorithm.")
-        self.clusters = cluster_turbines(
-            fi=self.fi,
-            wind_direction=self.fi.floris.farm.wind_direction[0],
-            wake_slope=self.clustering_wake_slope
-        )
+        # Confirm that Ny_passes are integers and odd/even
+        for Nii, Ny in enumerate(Ny_passes):
+            if not isinstance(Ny, int):
+                raise ValueError("Ny_passes must contain exclusively integers")
+            if Ny < 2:
+                raise ValueError("Each entry in Ny_passes must have a value of at least 2.")
+            if (Nii > 0) & ((Ny + 1) % 2 == 0):
+                raise ValueError(
+                    "The second and further entries of Ny_passes must be even numbers. "
+                    "This is to ensure the same yaw angles are not evaluated twice between passes."
+                )
+
+        # # Set baseline and optimization settings
+        # if reduce_ngrid:
+        #     for ti in range(self.nturbs):
+        #         # Force number of grid points to 2
+        #         self.fmodel.core.farm.turbines[ti].ngrid = 2
+        #         self.fmodel.core.farm.turbines[ti].initialize_turbine()
+        #         print("Reducing ngrid. Unsure if this functionality works!")
+
+        # Save optimization choices to self
+        self.Ny_passes = Ny_passes
+
+        # For each wind direction, determine the order of turbines
+        self._get_turbine_orders()
+
+    def _get_turbine_orders(self):
+        layout_x = self.fmodel.layout_x
+        layout_y = self.fmodel.layout_y
+        turbines_ordered_array = []
+        for wd in self.fmodel_subset.core.flow_field.wind_directions:
+            layout_x_rot = (
+                np.cos((wd - 270.0) * np.pi / 180.0) * layout_x
+                - np.sin((wd - 270.0) * np.pi / 180.0) * layout_y
+            )
+            turbines_ordered = np.argsort(layout_x_rot)
+            turbines_ordered_array.append(turbines_ordered)
+        self.turbines_ordered_array_subset = np.vstack(turbines_ordered_array)
+
+
+    def _calc_powers_with_memory(self, yaw_angles_subset, use_memory=True):
+        # Define current optimal solutions and floris wind directions locally
+        yaw_angles_opt_subset = self._yaw_angles_opt_subset
+        farm_power_opt_subset = self._farm_power_opt_subset
+        wd_array_subset = self.fmodel_subset.core.flow_field.wind_directions
+        ws_array_subset = self.fmodel_subset.core.flow_field.wind_speeds
+        ti_array_subset = self.fmodel_subset.core.flow_field.turbulence_intensities
+        turbine_weights_subset = self._turbine_weights_subset
+
+        # Reformat yaw_angles_subset, if necessary
+        eval_multiple_passes = (len(np.shape(yaw_angles_subset)) == 3)
+        if eval_multiple_passes:
+            # Four-dimensional; format everything into three-dimensional
+            Ny = yaw_angles_subset.shape[0]  # Number of passes
+            yaw_angles_subset = np.vstack(
+                [yaw_angles_subset[iii, :, :] for iii in range(Ny)]
+            )
+            yaw_angles_opt_subset = np.tile(yaw_angles_opt_subset, (Ny, 1))
+            farm_power_opt_subset = np.tile(farm_power_opt_subset, (Ny))
+            wd_array_subset = np.tile(wd_array_subset, Ny)
+            ws_array_subset = np.tile(ws_array_subset, Ny)
+            ti_array_subset = np.tile(ti_array_subset, Ny)
+            turbine_weights_subset = np.tile(turbine_weights_subset, (Ny, 1))
+
+        # Initialize empty matrix for floris farm power outputs
+        farm_powers = np.zeros((yaw_angles_subset.shape[0]))
+
+        # Find indices of yaw angles that we previously already evaluated, and
+        # prevent redoing the same calculations
+        if use_memory:
+            idx = (np.abs(yaw_angles_opt_subset - yaw_angles_subset) < 0.01).all(axis=1)
+            farm_powers[idx] = farm_power_opt_subset[idx]
+            if self.print_progress:
+                self.logger.info(
+                    "Skipping {:d}/{:d} calculations: already in memory.".format(
+                        np.sum(idx), len(idx))
+                )
+        else:
+            idx = np.zeros(yaw_angles_subset.shape[0], dtype=bool)
+
+        if not np.all(idx):
+            # Now calculate farm powers for conditions we haven't yet evaluated previously
+            start_time = timerpc()
+            if (hasattr(self.fmodel.core.flow_field, 'heterogeneous_inflow_config') and
+                self.fmodel.core.flow_field.heterogeneous_inflow_config is not None):
+                het_sm_orig = np.array(
+                    self.fmodel.core.flow_field.heterogeneous_inflow_config['speed_multipliers']
+                )
+                het_sm = np.tile(het_sm_orig, (Ny, 1))[~idx, :]
+            else:
+                het_sm = None
+            farm_powers[~idx] = self._calculate_farm_power(
+                wd_array=wd_array_subset[~idx],
+                ws_array=ws_array_subset[~idx],
+                ti_array=ti_array_subset[~idx],
+                turbine_weights=turbine_weights_subset[~idx, :],
+                yaw_angles=yaw_angles_subset[~idx, :],
+                heterogeneous_speed_multipliers=het_sm
+            )
+            self.time_spent_in_floris += (timerpc() - start_time)
 
-    def plot_clusters(self):
-        cluster_turbines(
-            fi=self.fi,
-            wind_direction=self.fi.floris.farm.wind_direction[0],
-            wake_slope=self.clustering_wake_slope,
-            plot_lines=True
-        )
+        # Finally format solutions back to original format, if necessary
+        if eval_multiple_passes:
+            farm_powers = np.reshape(
+                farm_powers,
+                (
+                    Ny,
+                    self.fmodel_subset.core.flow_field.n_findex
+                )
+            )
 
-    def optimize(self, verbose=True):
-        """
-        This method solves for the optimum turbine yaw angles for power
-        production given a fixed set of atmospheric conditions
-        (wind speed, direction, etc.).
+        return farm_powers
 
-        Returns:
-            np.array: Optimal yaw angles for each turbine (deg).
+    def _generate_evaluation_grid(self, pass_depth, turbine_depth):
+        """
+        Calculate the yaw angles for every iteration in the SR algorithm, for turbine,
+        for every wind direction, for every wind speed, for every TI. Basically, this
+        should yield a grid of yaw angle sets to evaluate the wind farm AEP with 'Ny'
+        times. Then, for each ambient condition set,
         """
-        if verbose:
-            print("=====================================================")
-            print("Optimizing wake redirection control...")
-            print("Number of parameters to optimize = ", len(self.turbs_to_opt))
-            print("=====================================================")
-
-        # Cluster turbines first
-        self._cluster_turbines()
-        if verbose:
-            print("Clustered turbines into %d separate clusters." % len(self.clusters))
-
-        # Save parameters to a full list
-        yaw_angles_template_full = copy.copy(self.yaw_angles_template)
-        yaw_angles_baseline_full = copy.copy(self.yaw_angles_baseline)
-        turbine_weights_full = copy.copy(self.turbine_weights)
-        bnds_full = copy.copy(self.bnds)
-        # nturbs_full = copy.copy(self.nturbs)
-        x0_full = copy.copy(self.x0)
-        fi_full = copy.deepcopy(self.fi)
-
-        # Overwrite parameters for each cluster and optimize
-        opt_yaw_angles = np.zeros_like(x0_full)
-        for ci, cl in enumerate(self.clusters):
-            if verbose:
-                print("=====================================================")
-                print("Optimizing %d parameters in cluster %d." % (len(cl), ci))
-                print("=====================================================")
-            self.yaw_angles_template = np.array(yaw_angles_template_full)[cl]
-            self.yaw_angles_baseline = np.array(yaw_angles_baseline_full)[cl]
-            self.turbine_weights = np.array(turbine_weights_full)[cl]
-            self.bnds = np.array(bnds_full)[cl]
-            self.x0 = np.array(x0_full)[cl]
-            self.fi = copy.deepcopy(fi_full)
-            self.fi.reinitialize_flow_field(
-                layout_array=[
-                    np.array(fi_full.layout_x)[cl],
-                    np.array(fi_full.layout_y)[cl]
-                ]
+
+        # Initialize yaw angles to evaluate, 'Ny' times the wind rose
+        Ny = self.Ny_passes[pass_depth]
+        evaluation_grid = np.tile(self._yaw_angles_opt_subset, (Ny, 1, 1))
+
+        # Get a list of the turbines in order of x and sort front to back
+        for iw in range(self._n_findex_subset):
+            turbid = self.turbines_ordered_array_subset[iw, turbine_depth]  # Turbine to manipulate
+
+            # # Check if this turbine needs to be optimized. If not, continue
+            # if not self._turbs_to_opt_subset[iw, 0, turbid]:
+            #     continue
+
+            # # Remove turbines that need not be optimized
+            # turbines_ordered = [ti for ti in turbines_ordered if ti in self.turbs_to_opt]
+
+            # Grab yaw bounds from self
+            yaw_lb = self._yaw_lbs[iw, turbid]
+            yaw_ub = self._yaw_ubs[iw, turbid]
+
+            # Saturate to allowable yaw limits
+            yaw_lb = np.clip(
+                yaw_lb,
+                self.minimum_yaw_angle[iw, turbid],
+                self.maximum_yaw_angle[iw, turbid]
+            )
+            yaw_ub = np.clip(
+                yaw_ub,
+                self.minimum_yaw_angle[iw, turbid],
+                self.maximum_yaw_angle[iw, turbid]
             )
-            opt_yaw_angles[cl] = self._optimize()
 
-        # Restore parameters
-        self.yaw_angles_template = yaw_angles_template_full
-        self.yaw_angles_baseline = yaw_angles_baseline_full
-        self.turbine_weights = turbine_weights_full
-        self.bnds = bnds_full
-        self.x0 = x0_full
-        self.fi = fi_full
-        self.fi.reinitialize_flow_field(
-            layout_array=[
-                np.array(fi_full.layout_x),
-                np.array(fi_full.layout_y)
-            ]
-        )
+            if pass_depth == 0:
+                # Evaluate all possible coordinates
+                yaw_angles_subset = np.linspace(yaw_lb, yaw_ub, Ny)
+            else:
+                # Remove middle point: was evaluated in previous iteration
+                c = int(Ny / 2)  # Central point (to remove)
+                ids = [*list(range(0, c)), *list(range(c + 1, Ny + 1))]
+                yaw_angles_subset = np.linspace(yaw_lb, yaw_ub, Ny + 1)[ids]
+
+            evaluation_grid[:, iw, turbid] = yaw_angles_subset
+
+        self._yaw_evaluation_grid = evaluation_grid
+        return evaluation_grid
+
+    def _process_evaluation_grid(self):
+        # Evaluate the farm AEPs for the grid of possible yaw angles
+        evaluation_grid = self._yaw_evaluation_grid
+        farm_powers = self._calc_powers_with_memory(evaluation_grid)
+        return farm_powers
 
-        if verbose and np.sum(np.abs(opt_yaw_angles)) == 0:
-            print(
-                "No change in controls suggested for this inflow \
-                   condition..."
-            )
+    def optimize(self, print_progress=True):
+        """
+        Find the yaw angles that maximize the power production for every wind direction,
+        wind speed and turbulence intensity.
+        """
+        self.print_progress = print_progress
 
-        return opt_yaw_angles
+        # For each pass, from front to back
+        ii = 0
+        for Nii in range(len(self.Ny_passes)):
+            # Disturb yaw angles for one turbine at a time, from front to back
+            for turbine_depth in range(self.nturbs):
+                p = 100.0 * ii / (len(self.Ny_passes) * self.nturbs)
+                ii += 1
+                if self.print_progress:
+                    print(
+                        f"[Serial Refine] Processing pass={Nii}, "
+                        f"turbine_depth={turbine_depth} ({p:.1f}%)"
+                    )
+
+                # Create grid to evaluate yaw angles for one turbine == turbine_depth
+                evaluation_grid = self._generate_evaluation_grid(
+                    pass_depth=Nii,
+                    turbine_depth=turbine_depth
+                )
+
+                # Evaluate grid of yaw angles, get farm powers and find optimal solutions
+                farm_powers = self._process_evaluation_grid()
+
+                # If farm powers contains any nans, then issue a warning
+                if np.any(np.isnan(farm_powers)):
+                    err_msg = (
+                        "NaNs found in farm powers during SerialRefine "
+                        "optimization routine. Proceeding to maximize over yaw "
+                        "settings that produce valid powers."
+                    )
+                    self.logger.warning(err_msg, stack_info=True)
+
+                # Find optimal solutions in new evaluation grid
+                args_opt = np.expand_dims(np.nanargmax(farm_powers, axis=0), axis=0)
+                farm_powers_opt_new = np.squeeze(
+                    np.take_along_axis(farm_powers, args_opt, axis=0),
+                    axis=0,
+                )
+                yaw_angles_opt_new = np.squeeze(
+                    np.take_along_axis(
+                        evaluation_grid,
+                        np.expand_dims(args_opt, axis=2),
+                        axis=0
+                    ),
+                    axis=0
+                )
+
+                farm_powers_opt_prev = self._farm_power_opt_subset
+                yaw_angles_opt_prev = self._yaw_angles_opt_subset
+
+                # Now update optimal farm powers if better than previous
+                ids_better = (farm_powers_opt_new > farm_powers_opt_prev)
+                farm_power_opt = farm_powers_opt_prev
+                farm_power_opt[ids_better] = farm_powers_opt_new[ids_better]
+
+                # Now update optimal yaw angles if better than previous
+                turbs_sorted = self.turbines_ordered_array_subset
+                turbids = turbs_sorted[np.where(ids_better)[0], turbine_depth]
+                ids = (*np.where(ids_better), turbids)
+                yaw_angles_opt = yaw_angles_opt_prev
+                yaw_angles_opt[ids] = yaw_angles_opt_new[ids]
+
+                # Update bounds for next iteration to close proximity of optimal solution
+                dx = (
+                    evaluation_grid[1, :, :] -
+                    evaluation_grid[0, :, :]
+                )[ids]
+                self._yaw_lbs[ids] = np.clip(
+                    yaw_angles_opt[ids] - 0.50 * dx,
+                    self._minimum_yaw_angle_subset[ids],
+                    self._maximum_yaw_angle_subset[ids]
+                )
+                self._yaw_ubs[ids] = np.clip(
+                    yaw_angles_opt[ids] + 0.50 * dx,
+                    self._minimum_yaw_angle_subset[ids],
+                    self._maximum_yaw_angle_subset[ids]
+                )
+
+                # Save results to self
+                self._farm_power_opt_subset = farm_power_opt
+                self._yaw_angles_opt_subset = yaw_angles_opt
+
+        # Finalize optimization, i.e., retrieve full solutions
+        df_opt = self._finalize()
+        return df_opt
```

### Comparing `FLORIS-3.6/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py` & `FLORIS-4/floris/parallel_floris_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,452 +1,557 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
+# Copyright 2022 Shell
 import copy
+import warnings
+from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
+from floris.floris_model import FlorisModel
 from floris.logging_manager import LoggingManager
+from floris.optimization.yaw_optimization.yaw_optimizer_sr import YawOptimizationSR
+from floris.uncertain_floris_model import map_turbine_powers_uncertain, UncertainFlorisModel
 
-from .cluster_turbines import cluster_turbines
-from .yaw_wind_rose import YawOptimizationWindRose
 
+def _get_turbine_powers_serial(fmodel_information, yaw_angles=None):
+    fmodel = FlorisModel(fmodel_information)
+    fmodel.set(yaw_angles=yaw_angles)
+    fmodel.run()
+    return (fmodel.get_turbine_powers(), fmodel.core.flow_field)
+
+
+def _optimize_yaw_angles_serial(
+    fmodel_information,
+    minimum_yaw_angle,
+    maximum_yaw_angle,
+    yaw_angles_baseline,
+    x0,
+    Ny_passes,
+    turbine_weights,
+    exclude_downstream_turbines,
+    verify_convergence,
+    print_progress,
+):
+    fmodel_opt = FlorisModel(fmodel_information)
+    yaw_opt = YawOptimizationSR(
+        fmodel=fmodel_opt,
+        minimum_yaw_angle=minimum_yaw_angle,
+        maximum_yaw_angle=maximum_yaw_angle,
+        yaw_angles_baseline=yaw_angles_baseline,
+        x0=x0,
+        Ny_passes=Ny_passes,
+        turbine_weights=turbine_weights,
+        exclude_downstream_turbines=exclude_downstream_turbines,
+        verify_convergence=verify_convergence,
+    )
+
+    # Perform optimization but silence print statements to avoid cluttering
+    df_opt = yaw_opt.optimize(print_progress=print_progress)
+    return df_opt
 
-class YawOptimizationWindRoseClustered(YawOptimizationWindRose, LoggingManager):
-    """
-    YawOptimizationWindRose is a subclass of
-    :py:class:`~.tools.optimizationscipy.YawOptimizationWindRose` that is used
-    to perform optimizations of the yaw angles of all or a subset of wind
-    turbines in a Floris Farm for multiple sets of inflow conditions using the
-    scipy optimization package. This class facilitates the clusterization of the
-    turbines inside seperate subsets in which the turbines witin each subset
-    exclusively interact with one another and have no impact on turbines
-    in other clusters. This may significantly reduce the computational
-    burden at no loss in performance (assuming the turbine clusters are truly
-    independent).
-    """
 
+class ParallelFlorisModel(LoggingManager):
     def __init__(
         self,
-        fi,
-        wd,
-        ws,
-        ti=None,
-        minimum_yaw_angle=0.0,
-        maximum_yaw_angle=25.0,
-        minimum_ws=3.0,
-        maximum_ws=25.0,
-        yaw_angles_baseline=None,
-        x0=None,
-        bnds=None,
-        opt_method="SLSQP",
-        opt_options=None,
-        include_unc=False,
-        unc_pmfs=None,
-        unc_options=None,
-        turbine_weights=None,
-        verbose=False,
-        calc_init_power=True,
-        exclude_downstream_turbines=False,
-        clustering_wake_slope=0.30,
+        fmodel,
+        max_workers,
+        n_wind_condition_splits,
+        interface="multiprocessing",  # Options are 'multiprocessing', 'mpi4py' or 'concurrent'
+        use_mpi4py=None,
+        propagate_flowfield_from_workers=False,
+        print_timings=False
     ):
-        """
-        Instantiate YawOptimizationWindRose object with a FlorisInterface object
-        and assign parameter values.
+        """A wrapper around the nominal floris_interface class that adds
+        parallel computing to common FlorisModel properties.
 
         Args:
-            fi (:py:class:`~.tools.floris_interface.FlorisInterface`):
-                Interface used to interact with the Floris object.
-            wd (iterable) : The wind directions for which the yaw angles are
-                optimized (deg).
-            ws (iterable): The wind speeds for which the yaw angles are
-                optimized (m/s).
-            ti (iterable, optional): An optional list of turbulence intensity
-                values for which the yaw angles are optimized. If not
-                specified, the current TI value in the Floris object will be
-                used for all optimizations. Defaults to None.
-            minimum_yaw_angle (float, optional): Minimum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 0.0.
-            maximum_yaw_angle (float, optional): Maximum constraint on yaw
-                angle (deg). This value will be ignored if bnds is also
-                specified. Defaults to 25.0.
-            minimum_ws (float, optional): Minimum wind speed at which
-                optimization is performed (m/s). Assumes zero power generated
-                below this value. Defaults to 3.
-            maximum_ws (float, optional): Maximum wind speed at which
-                optimization is performed (m/s). Assumes optimal yaw offsets
-                are zero above this wind speed. Defaults to 25.
-            yaw_angles_baseline (iterable, optional): The baseline yaw
-                angles used to calculate the initial and baseline power
-                production in the wind farm and used to normalize the cost
-                function. If none are specified, this variable is set equal
-                to the current yaw angles in floris. Note that this variable
-                need not meet the yaw constraints specified in self.bnds,
-                yet a warning is raised if it does to inform the user.
-                Defaults to None.
-            x0 (iterable, optional): The initial guess for the optimization
-                problem. These values must meet the constraints specified
-                in self.bnds. Note that, if exclude_downstream_turbines=True,
-                the initial guess for any downstream turbines are ignored
-                since they are not part of the optimization. Instead, the yaw
-                angles for those turbines are 0.0 if that meets the lower and
-                upper bound, or otherwise as close to 0.0 as feasible. If no
-                values for x0 are specified, x0 is set to be equal to zeros
-                wherever feasible (w.r.t. the bounds), and equal to the
-                average of its lower and upper bound for all non-downstream
-                turbines otherwise. Defaults to None.
-            bnds (iterable, optional): Bounds for the yaw angles, as tuples of
-                min, max values for each turbine (deg). One can fix the yaw
-                angle of certain turbines to a predefined value by setting that
-                turbine's lower bound equal to its upper bound (i.e., an
-                equality constraint), as: bnds[ti] = (x, x), where x is the
-                fixed yaw angle assigned to the turbine. This works for both
-                zero and nonzero yaw angles. Moreover, if
-                exclude_downstream_turbines=True, the yaw angles for all
-                downstream turbines will be 0.0 or a feasible value closest to
-                0.0. If none are specified, the bounds are set to
-                (minimum_yaw_angle, maximum_yaw_angle) for each turbine. Note
-                that, if bnds is not none, its values overwrite any value given
-                in minimum_yaw_angle and maximum_yaw_angle. Defaults to None.
-            opt_method (str, optional): The optimization method used by
-                scipy.optimize.minize. Defaults to 'SLSQP'.
-            opt_options (dictionary, optional): Optimization options used by
-                scipy.optimize.minize. If none are specified, they are set to
-                {'maxiter': 100, 'disp': False, 'iprint': 1, 'ftol': 1e-7,
-                'eps': 0.01}. Defaults to None.
-            include_unc (bool, optional): Determines whether wind direction or
-                yaw uncertainty are included. If True, uncertainty in wind
-                direction and/or yaw position is included when determining
-                wind farm power. Uncertainty is included by computing the
-                mean wind farm power for a distribution of wind direction
-                and yaw position deviations from the intended wind direction
-                and yaw angles. Defaults to False.
-            unc_pmfs (dictionary, optional): A dictionary containing
-                probability mass functions describing the distribution of
-                wind direction and yaw position deviations when wind direction
-                and/or yaw position uncertainty is included in the power
-                calculations. Contains the following key-value pairs:
-
-                -   **wd_unc** (*np.array*): The wind direction
-                    deviations from the intended wind direction (deg).
-                -   **wd_unc_pmf** (*np.array*): The probability
-                    of each wind direction deviation in **wd_unc** occuring.
-                -   **yaw_unc** (*np.array*): The yaw angle deviations
-                    from the intended yaw angles (deg).
-                -   **yaw_unc_pmf** (*np.array*): The probability
-                    of each yaw angle deviation in **yaw_unc** occuring.
-
-                If none are specified, default PMFs are calculated using
-                values provided in **unc_options**. Defaults to None.
-            unc_options (dictionary, optional): A dictionary containing values
-                used to create normally-distributed, zero-mean probability mass
-                functions describing the distribution of wind direction and yaw
-                position deviations when wind direction and/or yaw position
-                uncertainty is included. This argument is only used when
-                **unc_pmfs** is None and contains the following key-value pairs:
-
-                -   **std_wd** (*float*): The standard deviation of
-                    the wind direction deviations from the original wind
-                    direction (deg).
-                -   **std_yaw** (*float*): The standard deviation of
-                    the yaw angle deviations from the original yaw angles (deg).
-                -   **pmf_res** (*float*): The resolution in degrees
-                    of the wind direction and yaw angle PMFs.
-                -   **pdf_cutoff** (*float*): The cumulative
-                    distribution function value at which the tails of the
-                    PMFs are truncated.
-
-                If none are specified, default values of
-                {'std_wd': 4.95, 'std_yaw': 1.75, 'pmf_res': 1.0,
-                'pdf_cutoff': 0.995} are used. Defaults to None.
-            turbine_weights (iterable, optional): weighing terms that allow
-                the user to emphasize power gains at particular turbines or
-                completely ignore power gains from other turbines. The array
-                of turbine powers from floris is multiplied with this array
-                in the calculation of the objective function. If None, this
-                is an array with all values 1.0 and length equal to the
-                number of turbines. Defaults to None.
-            calc_init_power (bool, optional): If True, calculates initial
-                wind farm power for each set of wind conditions. Defaults to
-                True.
-            exclude_downstream_turbines (bool, optional): If True,
-                automatically finds and excludes turbines that are most
-                downstream from the optimization problem. This significantly
-                reduces computation time at no loss in performance. The yaw
-                angles of these downstream turbines are fixed to 0.0 deg if
-                the yaw bounds specified in self.bnds allow that, or otherwise
-                are fixed to the lower or upper yaw bound, whichever is closer
-                to 0.0. Defaults to False.
-            clustering_wake_slope (float, optional): linear slope of the wake
-                in the simplified linear expansion wake model (dy/dx). This
-                model is used to derive wake interactions between turbines and
-                to identify the turbine clusters. A good value is about equal
-                to the turbulence intensity in FLORIS. Though, since yaw
-                optimizations may shift the wake laterally, a safer option
-                is twice the turbulence intensity. The default value is 0.30
-                which should be valid for yaw optimizations at wd_std = 0.0 deg
-                and turbulence intensities up to 15%. Defaults to 0.30.
+        fmodel (FlorisModel or UncertainFlorisModel object): Interactive FLORIS object used to
+            perform the wake and turbine calculations. Can either be a regular FlorisModel
+            object or can be an UncertainFlorisModel object.
+        max_workers (int): Number of parallel workers, typically equal to the number of cores
+            you have on your system or HPC.
+        n_wind_condition_splits (int): Number of sectors to split the wind findex array over.
+            This is typically equal to max_workers, or a multiple of it.
+        interface (str): Parallel computing interface to leverage. Recommended is 'concurrent'
+            or 'multiprocessing' for local (single-system) use, and 'mpi4py' for high performance
+            computing on multiple nodes. Defaults to 'multiprocessing'.
+        use_mpi4py (bool): Deprecated option to enable/disable the usage of 'mpi4py'. This option
+            has been superseded by 'interface'.
+        propagate_flowfield_from_workers (bool): By enabling this, the flow field from every
+            floris object (one for each worker) is exported, combined and sent back to the main
+            module. This is slow so unless it's needed, it's recommended to be disabled. Defaults
+            to False.
+        print_timings (bool): Print the computation time to the console. Defaults to False.
         """
-        super().__init__(
-            fi=fi,
-            wd=wd,
-            ws=ws,
-            ti=ti,
-            minimum_yaw_angle=minimum_yaw_angle,
-            maximum_yaw_angle=maximum_yaw_angle,
-            minimum_ws=minimum_ws,
-            maximum_ws=maximum_ws,
-            yaw_angles_baseline=yaw_angles_baseline,
-            x0=x0,
-            bnds=bnds,
-            opt_method=opt_method,
-            opt_options=opt_options,
-            include_unc=include_unc,
-            unc_pmfs=unc_pmfs,
-            unc_options=unc_options,
-            turbine_weights=turbine_weights,
-            verbose=verbose,
-            calc_init_power=calc_init_power,
-            exclude_downstream_turbines=exclude_downstream_turbines,
-        )
-        self.clustering_wake_slope = clustering_wake_slope
-
-
-    def _cluster_turbines(self):
-        wind_directions = self.fi.floris.farm.wind_direction
-        if (np.std(wind_directions) > 0.001):
-            raise ValueError("Wind directions must be uniform for clustering algorithm.")
-        self.clusters = cluster_turbines(
-            fi=self.fi,
-            wind_direction=self.fi.floris.farm.wind_direction[0],
-            wake_slope=self.clustering_wake_slope
-        )
-
-    def plot_clusters(self):
-        for wd in self.wd:
-            cluster_turbines(
-                fi=self.fi,
-                wind_direction=wd,
-                wake_slope=self.clustering_wake_slope,
-                plot_lines=True
+
+        # Set defaults for backward compatibility
+        if use_mpi4py is not None:
+            warnings.warn(
+                "The option 'mpi4py' will be removed in a future version. "
+                "Please use the option 'interface'."
             )
+            if use_mpi4py:
+                interface = "mpi4py"
+            else:
+                interface = "multiprocessing"
 
+        if interface == "mpi4py":
+            import mpi4py.futures as mp
+            self._PoolExecutor = mp.MPIPoolExecutor
+        elif interface == "multiprocessing":
+            import multiprocessing as mp
+            self._PoolExecutor = mp.Pool
+            if max_workers is None:
+                max_workers = mp.cpu_count()
+        elif interface == "concurrent":
+            from concurrent.futures import ProcessPoolExecutor
+            self._PoolExecutor = ProcessPoolExecutor
+        else:
+            raise UserWarning(
+                f"Interface '{interface}' not recognized. "
+                "Please use 'concurrent', 'multiprocessing' or 'mpi4py'."
+            )
 
-    def optimize(self):
-        """
-        This method solves for the optimum turbine yaw angles for power
-        production and the resulting power produced by the wind farm for a
-        series of wind speed, wind direction, and optionally TI combinations.
+        # Initialize floris object and copy common properties
+        if isinstance(fmodel, FlorisModel):
+            self.fmodel = fmodel.copy()
+            self._is_uncertain = False
+        elif isinstance(fmodel, UncertainFlorisModel):
+            self.fmodel = fmodel.fmodel_expanded.copy()
+            self._is_uncertain = True
+            self._weights = fmodel.weights
+            self._n_unexpanded = fmodel.n_unexpanded
+            self._n_sample_points = fmodel.n_sample_points
+            self._map_to_expanded_inputs = fmodel.map_to_expanded_inputs
+        self.core = self.fmodel.core # Static copy as a placeholder
+
+        # Save to self
+        self._n_wind_condition_splits = n_wind_condition_splits  # Save initial user input
+        self._max_workers = max_workers  # Save initial user input
 
-        Returns:
-            pandas.DataFrame: A pandas DataFrame with the same number of rows
-            as the length of the wd and ws arrays, containing the following
-            columns:
-
-                - **ws** (*float*) - The wind speed values for which the yaw
-                angles are optimized and power is computed (m/s).
-                - **wd** (*float*) - The wind direction values for which the
-                yaw angles are optimized and power is computed (deg).
-                - **ti** (*float*) - The turbulence intensity values for which
-                the yaw angles are optimized and power is computed. Only
-                included if self.ti is not None.
-                - **power_opt** (*float*) - The total power produced by the
-                wind farm with optimal yaw offsets (W).
-                - **turbine_power_opt** (*list* (*float*)) - A list
-                containing the power produced by each wind turbine with optimal
-                yaw offsets (W).
-                - **yaw_angles** (*list* (*float*)) - A list containing
-                the optimal yaw offsets for maximizing total wind farm power
-                for each wind turbine (deg).
-        """
-        print("=====================================================")
-        print("Optimizing wake redirection control...")
-        print("Number of wind conditions to optimize = ", len(self.wd))
-        print("Number of yaw angles to optimize = ", len(self.turbs_to_opt))
-        print("=====================================================")
-
-        df_opt = pd.DataFrame()
-
-        for i in range(len(self.wd)):
-            if self.verbose:
-                if self.ti is None:
-                    print(
-                        "Computing wind speed, wind direction pair "
-                        + str(i)
-                        + " out of "
-                        + str(len(self.wd))
-                        + ": wind speed = "
-                        + str(self.ws[i])
-                        + " m/s, wind direction = "
-                        + str(self.wd[i])
-                        + " deg."
-                    )
-                else:
-                    print(
-                        "Computing wind speed, wind direction, turbulence "
-                        + "intensity set "
-                        + str(i)
-                        + " out of "
-                        + str(len(self.wd))
-                        + ": wind speed = "
-                        + str(self.ws[i])
-                        + " m/s, wind direction = "
-                        + str(self.wd[i])
-                        + " deg, turbulence intensity = "
-                        + str(self.ti[i])
-                        + "."
-                    )
-
-            # Optimizing wake redirection control
-            if (self.ws[i] >= self.minimum_ws) & (self.ws[i] <= self.maximum_ws):
-                if self.ti is None:
-                    self.fi.reinitialize_flow_field(
-                        wind_direction=[self.wd[i]], wind_speed=[self.ws[i]]
-                    )
-                else:
-                    self.fi.reinitialize_flow_field(
-                        wind_direction=[self.wd[i]],
-                        wind_speed=[self.ws[i]],
-                        turbulence_intensity=self.ti[i],
-                    )
-
-                # Set initial farm power
-                self.initial_farm_power = self.initial_farm_powers[i]
-
-                # Determine clusters and then optimize by cluster
-                self._cluster_turbines()
-                if self.verbose:
-                    print("Clustered turbines into %d separate clusters." % len(self.clusters))
-
-                # Save parameters to a full list
-                yaw_angles_template_full = copy.copy(self.yaw_angles_template)
-                yaw_angles_baseline_full = copy.copy(self.yaw_angles_baseline)
-                turbine_weights_full = copy.copy(self.turbine_weights)
-                bnds_full = copy.copy(self.bnds)
-                # nturbs_full = copy.copy(self.nturbs)
-                x0_full = copy.copy(self.x0)
-                fi_full = copy.deepcopy(self.fi)
-
-                # Overwrite parameters for each cluster and optimize
-                opt_yaw_angles = np.zeros_like(x0_full)
-                for ci, cl in enumerate(self.clusters):
-                    if self.verbose:
-                        print("=====================================================")
-                        print("Optimizing %d parameters in cluster %d." % (len(cl), ci))
-                        print("=====================================================")
-                    self.yaw_angles_template = np.array(yaw_angles_template_full)[cl]
-                    self.yaw_angles_baseline = np.array(yaw_angles_baseline_full)[cl]
-                    self.turbine_weights = np.array(turbine_weights_full)[cl]
-                    self.bnds = np.array(bnds_full)[cl]
-                    self.x0 = np.array(x0_full)[cl]
-                    self.fi = copy.deepcopy(fi_full)
-                    self.fi.reinitialize_flow_field(
-                        layout_array=[
-                            np.array(fi_full.layout_x)[cl],
-                            np.array(fi_full.layout_y)[cl]
-                        ]
-                    )
-                    opt_yaw_angles[cl] = self._optimize()
-
-                # Restore parameters
-                self.yaw_angles_template = yaw_angles_template_full
-                self.yaw_angles_baseline = yaw_angles_baseline_full
-                self.turbine_weights = turbine_weights_full
-                self.bnds = bnds_full
-                self.x0 = x0_full
-                self.fi = fi_full
-                self.fi.reinitialize_flow_field(
-                    layout_array=[
-                        np.array(fi_full.layout_x),
-                        np.array(fi_full.layout_y)
-                    ]
-                )
+        self.n_wind_condition_splits = int(
+            np.min([n_wind_condition_splits, self.fmodel.core.flow_field.n_findex])
+        )
+        self.max_workers = int(
+            np.min([max_workers, self.n_wind_condition_splits])
+        )
+        self.propagate_flowfield_from_workers = propagate_flowfield_from_workers
+        self.interface = interface
+        self.print_timings = print_timings
+
+    def copy(self):
+        # Make an independent copy
+        self_copy = copy.deepcopy(self)
+        self_copy.fmodel = self.fmodel.copy()
+        return self_copy
 
-                if np.sum(np.abs(opt_yaw_angles)) == 0:
-                    print(
-                        "No change in controls suggested for this inflow \
-                        condition..."
-                    )
-
-                # optimized power
-                self.fi.calculate_wake(yaw_angles=opt_yaw_angles)
-                power_opt = self.fi.get_turbine_power(
-                    include_unc=self.include_unc,
-                    unc_pmfs=self.unc_pmfs,
-                    unc_options=self.unc_options,
-                )
-            elif self.ws[i] >= self.maximum_ws:
-                print(
-                    "No change in controls suggested for this inflow \
-                        condition..."
-                )
-                if self.ti is None:
-                    self.fi.reinitialize_flow_field(
-                        wind_direction=[self.wd[i]], wind_speed=[self.ws[i]]
-                    )
-                else:
-                    self.fi.reinitialize_flow_field(
-                        wind_direction=[self.wd[i]],
-                        wind_speed=[self.ws[i]],
-                        turbulence_intensity=self.ti[i],
-                    )
-                opt_yaw_angles = np.array(self.yaw_angles_template, copy=True)
-                self.fi.calculate_wake(yaw_angles=opt_yaw_angles)
-                power_opt = self.fi.get_turbine_power(
-                    include_unc=self.include_unc,
-                    unc_pmfs=self.unc_pmfs,
-                    unc_options=self.unc_options,
-                )
+    def set(
+        self,
+        wind_speeds=None,
+        wind_directions=None,
+        wind_shear=None,
+        wind_veer=None,
+        reference_wind_height=None,
+        turbulence_intensities=None,
+        air_density=None,
+        layout=None,
+        layout_x=None,
+        layout_y=None,
+        turbine_type=None,
+        solver_settings=None,
+    ):
+        """Pass to the FlorisModel set function. To allow users
+        to directly replace a FlorisModel object with this
+        UncertainFlorisModel object, this function is required."""
+
+        if layout is not None:
+            msg = "Use the `layout_x` and `layout_y` parameters in place of `layout` "
+            msg += "because the `layout` parameter will be deprecated in 3.3."
+            self.logger.warning(msg)
+            layout_x = layout[0]
+            layout_y = layout[1]
+
+        # Just passes arguments to the floris object
+        fmodel = self.fmodel.copy()
+        fmodel.set(
+            wind_speeds=wind_speeds,
+            wind_directions=wind_directions,
+            wind_shear=wind_shear,
+            wind_veer=wind_veer,
+            reference_wind_height=reference_wind_height,
+            turbulence_intensities=turbulence_intensities,
+            air_density=air_density,
+            layout_x=layout_x,
+            layout_y=layout_y,
+            turbine_type=turbine_type,
+            solver_settings=solver_settings,
+        )
+
+        # Reinitialize settings
+        self.__init__(
+            fmodel=fmodel,
+            max_workers=self._max_workers,
+            n_wind_condition_splits=self._n_wind_condition_splits,
+            interface=self.interface,
+            propagate_flowfield_from_workers=self.propagate_flowfield_from_workers,
+            print_timings=self.print_timings,
+        )
+
+    def _preprocessing(self, yaw_angles=None):
+        # Format yaw angles
+        if yaw_angles is None:
+            yaw_angles = np.zeros((
+                self.fmodel.core.flow_field.n_findex,
+                self.fmodel.core.farm.n_turbines
+            ))
+
+        # Prepare settings
+        n_wind_condition_splits = self.n_wind_condition_splits
+        n_wind_condition_splits = np.min(
+            [n_wind_condition_splits, self.fmodel.core.flow_field.n_findex]
+        )
+
+        # Prepare the input arguments for parallel execution
+        fmodel_dict = self.fmodel.core.as_dict()
+        wind_condition_id_splits = np.array_split(
+            np.arange(self.fmodel.core.flow_field.n_findex),
+            n_wind_condition_splits,
+        )
+        multiargs = []
+        for wc_id_split in wind_condition_id_splits:
+            # for ws_id_split in wind_speed_id_splits:
+            fmodel_dict_split = copy.deepcopy(fmodel_dict)
+            wind_directions = self.fmodel.core.flow_field.wind_directions[wc_id_split]
+            wind_speeds = self.fmodel.core.flow_field.wind_speeds[wc_id_split]
+            turbulence_intensities = self.fmodel.core.flow_field.turbulence_intensities[wc_id_split]
+            yaw_angles_subset = yaw_angles[wc_id_split[0]:wc_id_split[-1]+1, :]
+            fmodel_dict_split["flow_field"]["wind_directions"] = wind_directions
+            fmodel_dict_split["flow_field"]["wind_speeds"] = wind_speeds
+            fmodel_dict_split["flow_field"]["turbulence_intensities"] = turbulence_intensities
+
+            # Prepare lightweight data to pass along
+            multiargs.append((fmodel_dict_split, yaw_angles_subset))
+
+        return multiargs
+
+    # Function to merge subsets in dictionaries
+    def _merge_subsets(self, field, subset):
+        i, j, k = np.shape(subset)
+        subset_reshape = np.reshape(subset, (i*j, k))
+        return [eval("f.{:s}".format(field) for f in subset_reshape)]
+
+    def _postprocessing(self, output):
+        # Split results
+        power_subsets = [p[0] for p in output]
+        flowfield_subsets = [p[1] for p in output]
+
+        # Retrieve and merge turbine power productions
+        turbine_powers = np.concatenate(power_subsets, axis=0)
+
+        # Optionally, also merge flow field dictionaries from individual floris solutions
+        if self.propagate_flowfield_from_workers:
+            self.core = self.fmodel.core  # Refresh static copy of underlying floris class
+            # self.core.flow_field.u_initial = self._merge_subsets("u_initial", flowfield_subsets)
+            # self.core.flow_field.v_initial = self._merge_subsets("v_initial", flowfield_subsets)
+            # self.core.flow_field.w_initial = self._merge_subsets("w_initial", flowfield_subsets)
+            self.core.flow_field.u = self._merge_subsets("u", flowfield_subsets)
+            self.core.flow_field.v = self._merge_subsets("v", flowfield_subsets)
+            self.core.flow_field.w = self._merge_subsets("w", flowfield_subsets)
+            self.core.flow_field.turbulence_intensity_field = self._merge_subsets(
+                "turbulence_intensity_field",
+                flowfield_subsets
+            )
+
+        return turbine_powers
+
+    def run(self):
+        raise UserWarning(
+            "'run' not supported on ParallelFlorisModel. Please use "
+            "'get_turbine_powers' or 'get_farm_power' directly."
+        )
+
+    def get_turbine_powers(self, yaw_angles=None):
+        # Retrieve multiargs: preprocessing
+        t0 = timerpc()
+        multiargs = self._preprocessing(yaw_angles)
+        t_preparation = timerpc() - t0
+
+        # Perform parallel calculation
+        t1 = timerpc()
+        with self._PoolExecutor(self.max_workers) as p:
+            if (self.interface == "mpi4py") or (self.interface == "multiprocessing"):
+                out = p.starmap(_get_turbine_powers_serial, multiargs)
             else:
-                print(
-                    "No change in controls suggested for this inflow \
-                        condition..."
+                out = p.map(
+                    _get_turbine_powers_serial,
+                    [j[0] for j in multiargs],
+                    [j[1] for j in multiargs]
                 )
-                opt_yaw_angles = np.array(self.yaw_angles_template, copy=True)
-                power_opt = self.nturbs * [0.0]
+                # out = list(out)
+        t_execution = timerpc() - t1
 
-            # Include turbine weighing terms
-            power_opt = np.multiply(self.turbine_weights, power_opt)
+        # Postprocessing: merge power production (and opt. flow field) from individual runs
+        t2 = timerpc()
+        turbine_powers = self._postprocessing(out)
+        if self._is_uncertain:
+            turbine_powers = map_turbine_powers_uncertain(
+                unique_turbine_powers=turbine_powers,
+                map_to_expanded_inputs=self._map_to_expanded_inputs,
+                weights=self._weights,
+                n_unexpanded=self._n_unexpanded,
+                n_sample_points=self._n_sample_points,
+                n_turbines=self.fmodel.core.farm.n_turbines,
+            )
+        t_postprocessing = timerpc() - t2
+        t_total = timerpc() - t0
 
-            # add variables to dataframe
-            if self.ti is None:
-                df_opt = df_opt.append(
-                    pd.DataFrame(
-                        {
-                            "ws": [self.ws[i]],
-                            "wd": [self.wd[i]],
-                            "power_opt": [np.sum(power_opt)],
-                            "turbine_power_opt": [power_opt],
-                            "yaw_angles": [opt_yaw_angles],
-                        }
-                    )
+        if self.print_timings:
+            print("===============================================================================")
+            print(
+                "Total time spent for parallel calculation "
+                f"({self.max_workers} workers): {t_total:.3f} s"
+            )
+            print(f"  Time spent in parallel preprocessing: {t_preparation:.3f} s")
+            print(f"  Time spent in parallel loop execution: {t_execution:.3f} s.")
+            print(f"  Time spent in parallel postprocessing: {t_postprocessing:.3f} s")
+
+        return turbine_powers
+
+    def get_farm_power(self, yaw_angles=None, turbine_weights=None):
+        if turbine_weights is None:
+            # Default to equal weighing of all turbines when turbine_weights is None
+            turbine_weights = np.ones(
+                (
+                    (self._n_unexpanded if self._is_uncertain
+                     else self.fmodel.core.flow_field.n_findex),
+                    self.fmodel.core.farm.n_turbines
                 )
+            )
+        elif len(np.shape(turbine_weights)) == 1:
+            # Deal with situation when 1D array is provided
+            turbine_weights = np.tile(
+                turbine_weights,
+                (
+                    (self._n_unexpanded if self._is_uncertain
+                     else self.fmodel.core.flow_field.n_findex),
+                    1
+                )
+            )
+
+        # Calculate all turbine powers and apply weights
+        turbine_powers = self.get_turbine_powers(yaw_angles=yaw_angles)
+        turbine_powers = np.multiply(turbine_weights, turbine_powers)
+
+        return np.sum(turbine_powers, axis=1)
+
+    def get_farm_AEP(
+        self,
+        freq,
+        cut_in_wind_speed=None,
+        cut_out_wind_speed=None,
+        yaw_angles=None,
+        turbine_weights=None,
+        no_wake=False,
+    ) -> float:
+        """
+        Estimate annual energy production (AEP) for distributions of wind speed, wind
+        direction, frequency of occurrence, and yaw offset.
+
+        Args:
+            freq (NDArrayFloat): NumPy array with shape (n_wind_directions,
+                n_wind_speeds) with the frequencies of each wind direction and
+                wind speed combination. These frequencies should typically sum
+                up to 1.0 and are used to weigh the wind farm power for every
+                condition in calculating the wind farm's AEP.
+            cut_in_wind_speed (float, optional): No longer supported.
+            cut_out_wind_speed (float, optional): No longer supported.
+            yaw_angles (NDArrayFloat | list[float] | None, optional):
+                The relative turbine yaw angles in degrees. If None is
+                specified, will assume that the turbine yaw angles are all
+                zero degrees for all conditions. Defaults to None.
+            turbine_weights (NDArrayFloat | list[float] | None, optional):
+                weighing terms that allow the user to emphasize power at
+                particular turbines and/or completely ignore the power
+                from other turbines. This is useful when, for example, you are
+                modeling multiple wind farms in a single floris object. If you
+                only want to calculate the power production for one of those
+                farms and include the wake effects of the neighboring farms,
+                you can set the turbine_weights for the neighboring farms'
+                turbines to 0.0. The array of turbine powers from floris
+                is multiplied with this array in the calculation of the
+                objective function. If None, this  is an array with all values
+                1.0 and with shape equal to (n_wind_directions, n_wind_speeds,
+                n_turbines). Defaults to None.
+            no_wake: (bool, optional): When *True* updates the turbine
+                quantities without calculating the wake or adding the wake to
+                the flow field. This can be useful when quantifying the loss
+                in AEP due to wakes. Defaults to *False*.
+
+        Returns:
+            float:
+                The Annual Energy Production (AEP) for the wind farm in
+                watt-hours.
+        """
+
+        # If no_wake==True, ignore parallelization because it's fast enough
+        if no_wake:
+            return self.fmodel.get_farm_AEP(
+                freq=freq,
+                cut_in_wind_speed=cut_in_wind_speed,
+                cut_out_wind_speed=cut_out_wind_speed,
+                yaw_angles=yaw_angles,
+                turbine_weights=turbine_weights,
+                no_wake=no_wake
+            )
+
+        # Verify dimensions of the variable "freq"
+        if ((self._is_uncertain and np.shape(freq)[0] != self._n_unexpanded) or
+            (not self._is_uncertain and np.shape(freq)[0] != self.fmodel.core.flow_field.n_findex)):
+            raise UserWarning(
+                "'freq' should be a one-dimensional array with dimensions (n_findex). "
+                f"Given shape is {np.shape(freq)}"
+            )
+
+        # Check if frequency vector sums to 1.0. If not, raise a warning
+        if np.abs(np.sum(freq) - 1.0) > 0.001:
+            self.logger.warning(
+                "WARNING: The frequency array provided to get_farm_AEP() does not sum to 1.0."
+            )
+
+        # Copy the full wind speed array from the floris object and initialize
+        # the the farm_power variable as an empty array.
+        wind_speeds = np.array(self.fmodel.core.flow_field.wind_speeds, copy=True)
+        wind_directions = np.array(self.fmodel.core.flow_field.wind_directions, copy=True)
+        turbulence_intensities = np.array(
+            self.fmodel.core.flow_field.turbulence_intensities,
+            copy=True,
+        )
+        farm_power = np.zeros(
+            self._n_unexpanded if self._is_uncertain else self.core.flow_field.n_findex
+        )
+
+        # Determine which wind speeds we must evaluate in floris
+        if cut_in_wind_speed is not None or cut_out_wind_speed is not None:
+            raise NotImplementedError(
+                "WARNING: The 'cut_in_wind_speed' and 'cut_out_wind_speed' "
+                "parameters are no longer supported in the 'ParallelFlorisModel.get_farm_AEP' "
+                "method."
+            )
+
+        farm_power = (
+            self.get_farm_power(yaw_angles=yaw_angles, turbine_weights=turbine_weights)
+        )
+
+        # Finally, calculate AEP in GWh
+        aep = np.nansum(np.multiply(freq, farm_power) * 365 * 24)
+
+        # Reset the FLORIS object to the full wind speed array
+        self.fmodel.set(
+            wind_directions=wind_directions,
+            wind_speeds=wind_speeds,
+            turbulence_intensities=turbulence_intensities,
+        )
+
+        return aep
+
+    def optimize_yaw_angles(
+        self,
+        minimum_yaw_angle=-25.0,
+        maximum_yaw_angle=25.0,
+        yaw_angles_baseline=None,
+        x0=None,
+        Ny_passes=[5,4],
+        turbine_weights=None,
+        exclude_downstream_turbines=True,
+        verify_convergence=False,
+        print_worker_progress=False,  # Recommended disabled to avoid clutter. Useful for debugging
+    ):
+
+        # Prepare the inputs to each core for multiprocessing module
+        t0 = timerpc()
+        multiargs = self._preprocessing()
+        for ii in range(len(multiargs)):
+            multiargs[ii] = (
+                multiargs[ii][0],
+                minimum_yaw_angle,
+                maximum_yaw_angle,
+                yaw_angles_baseline,
+                x0,
+                Ny_passes,
+                turbine_weights,
+                exclude_downstream_turbines,
+                verify_convergence,
+                print_worker_progress,
+            )
+        t1 = timerpc()
+
+        # Optimize yaw angles using parallel processing
+        print("Optimizing yaw angles with {:d} workers.".format(self.max_workers))
+        with self._PoolExecutor(self.max_workers) as p:
+            if (self.interface == "mpi4py") or (self.interface == "multiprocessing"):
+                df_opt_splits = p.starmap(_optimize_yaw_angles_serial, multiargs)
             else:
-                df_opt = df_opt.append(
-                    pd.DataFrame(
-                        {
-                            "ws": [self.ws[i]],
-                            "wd": [self.wd[i]],
-                            "ti": [self.ti[i]],
-                            "power_opt": [np.sum(power_opt)],
-                            "turbine_power_opt": [power_opt],
-                            "yaw_angles": [opt_yaw_angles],
-                        }
-                    )
+                df_opt_splits = p.map(
+                    _optimize_yaw_angles_serial,
+                    [j[0] for j in multiargs],
+                    [j[1] for j in multiargs],
+                    [j[2] for j in multiargs],
+                    [j[3] for j in multiargs],
+                    [j[4] for j in multiargs],
+                    [j[5] for j in multiargs],
+                    [j[6] for j in multiargs],
+                    [j[7] for j in multiargs],
+                    [j[8] for j in multiargs],
+                    [j[9] for j in multiargs],
                 )
+        t2 = timerpc()
 
-        df_opt.reset_index(drop=True, inplace=True)
+        # Combine all solutions from multiprocessing into single dataframe
+        df_opt = pd.concat(df_opt_splits, axis=0).reset_index(drop=True).sort_values(
+            by=["wind_direction", "wind_speed", "turbulence_intensity"]
+        )
+        t3 = timerpc()
+
+        if self.print_timings:
+            print("===============================================================================")
+            print(
+                "Total time spent for parallel calculation "
+                f"({self.max_workers} workers): {t3 - t0:.3f} s"
+            )
+            print("  Time spent in parallel preprocessing: {:.3f} s".format(t1 - t0))
+            print("  Time spent in parallel loop execution: {:.3f} s.".format(t2 - t1))
+            print("  Time spent in parallel postprocessing: {:.3f} s".format(t3 - t2))
 
         return df_opt
+
+    @property
+    def layout_x(self):
+        return self.fmodel.layout_x
+
+    @property
+    def layout_y(self):
+        return self.fmodel.layout_y
+
+    @property
+    def wind_speeds(self):
+        return self.fmodel.wind_speeds
+
+    @property
+    def wind_directions(self):
+        return self.fmodel.wind_directions
+
+    @property
+    def turbulence_intensities(self):
+        return self.fmodel.turbulence_intensities
+
+    @property
+    def n_findex(self):
+        return self.fmodel.n_findex
+
+    @property
+    def n_turbines(self):
+        return self.fmodel.n_turbines
+
+
+    # @property
+    # def floris(self):
+    #     return self.fmodel.core
```

### Comparing `FLORIS-3.6/floris/tools/optimization/other/boundary_grid.py` & `FLORIS-4/floris/optimization/other/boundary_grid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import numpy as np
 from shapely.geometry import Point, Polygon
 
 
 def discontinuous_grid(
     nrows,
@@ -253,21 +239,20 @@
     """
     Parameterize the wind farm layout with a grid or the boundary grid method
     """
 
     def __init__(self, fi):
         """
         Initializes a BoundaryGrid object by assigning a
-        FlorisInterface object.
+        FlorisModel object.
 
         Args:
-            fi (:py:class:`~.tools.floris_interface.FlorisInterface`):
-                Interface used to interact with the Floris object.
+            fmodel (FlorisModel): A FlorisModel object.
         """
-        self.fi = fi
+        self.fmodel = fi
 
         self.n_boundary_turbs = 0
         self.start = 0.0
         self.nrows = 0
         self.ncols = 0
         self.farm_width = 0.0
         self.farm_height = 0.0
@@ -342,15 +327,15 @@
             self.center_y,
             self.shrink_boundary,
             self.boundary_x,
             self.boundary_y,
             eps=self.eps,
         )
 
-        self.fi.reinitialize_flow_field(layout_array=(layout_x, layout_y))
+        self.fmodel.reinitialize_flow_field(layout_array=(layout_x, layout_y))
 
 
 if __name__ == "__main__":
 
     nrows = 10
     ncols = 10
     farm_width = 600
```

### Comparing `FLORIS-3.6/floris/tools/optimization/yaw_optimization/yaw_optimizer_geometric.py` & `FLORIS-4/floris/optimization/yaw_optimization/yaw_optimizer_geometric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,79 +1,63 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 import numpy as np
 
 from floris.utilities import rotate_coordinates_rel_west
 
 from .yaw_optimization_base import YawOptimization
 
 
 class YawOptimizationGeometric(YawOptimization):
     """
     YawOptimizationGeometric is a subclass of
-    :py:class:`floris.tools.optimization.general_library.YawOptimization` that is
+    :py:class:`floris.optimization.general_library.YawOptimization` that is
     used to provide a rough estimate of optimal yaw angles based purely on the
     wind farm geometry. Main use case is for coupled layout and yaw optimization.
     """
 
     def __init__(
         self,
-        fi,
+        fmodel,
         minimum_yaw_angle=0.0,
         maximum_yaw_angle=25.0,
-        exploit_layout_symmetry=True,
     ):
         """
-        Instantiate YawOptimizationGeometric object with a FlorisInterface
+        Instantiate YawOptimizationGeometric object with a FlorisModel
         object assign parameter values.
         """
 
         super().__init__(
-            fi=fi,
+            fmodel=fmodel,
             minimum_yaw_angle=minimum_yaw_angle,
             maximum_yaw_angle=maximum_yaw_angle,
-            exploit_layout_symmetry=exploit_layout_symmetry,
             calc_baseline_power=False
         )
 
     def optimize(self):
         """
         Find rough yaw angles based on wind farm geometry.
         Assumes all wind turbines have the same rotor diameter.
 
         Returns:
             opt_yaw_angles (np.array): Optimal yaw angles in degrees. This
             array is equal in length to the number of turbines in the farm.
         """
         # Loop through every WD individually. WS ignored!
-        wd_array = self.fi_subset.floris.flow_field.wind_directions
+        wd_array = self.fmodel_subset.core.flow_field.wind_directions
 
         for nwdi, wd in enumerate(wd_array):
-            self._yaw_angles_opt_subset[nwdi, :, :] = geometric_yaw(
-                self.fi_subset.layout_x,
-                self.fi_subset.layout_y,
+            self._yaw_angles_opt_subset[nwdi, :] = geometric_yaw(
+                self.fmodel_subset.layout_x,
+                self.fmodel_subset.layout_y,
                 wd,
-                self.fi.floris.farm.turbine_definitions[0]["rotor_diameter"],
-                top_left_yaw_upper=self.maximum_yaw_angle[0,0,0],
-                bottom_left_yaw_upper=self.maximum_yaw_angle[0,0,0],
-                top_left_yaw_lower=self.minimum_yaw_angle[0,0,0],
-                bottom_left_yaw_lower=self.minimum_yaw_angle[0,0,0]
+                self.fmodel.core.farm.turbine_definitions[0]["rotor_diameter"],
+                top_left_yaw_upper=self.maximum_yaw_angle[0, 0],
+                bottom_left_yaw_upper=self.maximum_yaw_angle[0, 0],
+                top_left_yaw_lower=self.minimum_yaw_angle[0, 0],
+                bottom_left_yaw_lower=self.minimum_yaw_angle[0, 0],
             )
 
         # Finalize optimization, i.e., retrieve full solutions
         df_opt = self._finalize()
 
         # Otherwise, df_opt will just copy the farm_power_baseline in
         return df_opt
@@ -90,15 +74,15 @@
     top_left_yaw_upper=30.0,
     top_right_yaw_upper=0.0,
     bottom_left_yaw_upper=30.0,
     bottom_right_yaw_upper=0.0,
     top_left_yaw_lower=-30.0,
     top_right_yaw_lower=0.0,
     bottom_left_yaw_lower=-30.0,
-    bottom_right_yaw_lower=0.0
+    bottom_right_yaw_lower=0.0,
 ):
     """
     turbine_x: unrotated x turbine coords
     turbine_y: unrotated y turbine coords
     wind_direction: float, degrees
     rotor_diameter: float
     left_x: where we start the trapezoid. Should be left as 0.
@@ -121,15 +105,15 @@
     turbine_coordinates_array[:,0] = turbine_x[:]
     turbine_coordinates_array[:,1] = turbine_y[:]
 
     rotated_x, rotated_y, _, _, _ = rotate_coordinates_rel_west(
         np.array([wind_direction]),
         turbine_coordinates_array
     )
-    processed_x, processed_y = _process_layout(rotated_x[0][0],rotated_y[0][0],rotor_diameter)
+    processed_x, processed_y = _process_layout(rotated_x[0], rotated_y[0], rotor_diameter)
     yaw_array = np.zeros(nturbs)
     for i in range(nturbs):
         # TODO: fix shape of top left yaw etc?
         yaw_array[i] = _get_yaw_angles(
             processed_x[i],
             processed_y[i],
             left_x,
@@ -139,15 +123,15 @@
             top_left_yaw_upper,
             top_right_yaw_upper,
             bottom_left_yaw_upper,
             bottom_right_yaw_upper,
             top_left_yaw_lower,
             top_right_yaw_lower,
             bottom_left_yaw_lower,
-            bottom_right_yaw_lower
+            bottom_right_yaw_lower,
         )
 
     return yaw_array
 
 def _process_layout(
     turbine_x,
     turbine_y,
```

### Comparing `FLORIS-3.6/floris/tools/visualization.py` & `FLORIS-4/floris/flow_visualization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-# Copyright 2021 NREL
 
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 from __future__ import annotations
 
 import copy
 import warnings
 from typing import Union
 
 import attrs
@@ -23,143 +11,33 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from attrs import define, field
 from matplotlib import rcParams
 from scipy.spatial import ConvexHull
 
-from floris.simulation import Floris
-from floris.tools.cut_plane import CutPlane
-from floris.tools.floris_interface import FlorisInterface
+from floris import FlorisModel
+from floris.core import Core
+from floris.core.turbine.operation_models import POWER_SETPOINT_DEFAULT
+from floris.cut_plane import CutPlane
 from floris.type_dec import (
     floris_array_converter,
     NDArrayFloat,
 )
 from floris.utilities import rotate_coordinates_rel_west, wind_delta
 
 
-def show_plots():
-    plt.show()
-
-def plot_turbines(
-    ax,
-    layout_x,
-    layout_y,
-    yaw_angles,
-    rotor_diameters,
-    color: str | None = None,
-):
+def show():
     """
-    This function is deprecated and will be removed in v3.5, use `plot_turbines_with_fi` instead.
-
-    Plot wind plant layout from turbine locations.
-
-    Args:
-        ax (:py:class:`matplotlib.pyplot.axes`): Figure axes.
-        layout_x (np.array): Wind turbine locations (east-west).
-        layout_y (np.array): Wind turbine locations (north-south).
-        yaw_angles (np.array): Yaw angles of each wind turbine.
-        rotor_diameters (np.array): Wind turbine rotor diameter.
-        color (str): pyplot color option to plot the turbines.
-    """
-    warnings.warn(
-        "The `plot_turbines` function is deprecated and will be removed in v3.5, "
-        "use `plot_turbines_with_fi` instead.",
-        DeprecationWarning,
-        stacklevel=2  # This prints the calling function and this function in the warning
-    )
-
-    if color is None:
-        color = "k"
-
-    for x, y, yaw, d in zip(layout_x, layout_y, yaw_angles, rotor_diameters):
-        R = d / 2.0
-        x_0 = x + np.sin(np.deg2rad(yaw)) * R
-        x_1 = x - np.sin(np.deg2rad(yaw)) * R
-        y_0 = y - np.cos(np.deg2rad(yaw)) * R
-        y_1 = y + np.cos(np.deg2rad(yaw)) * R
-        ax.plot([x_0, x_1], [y_0, y_1], color=color)
-
-
-def plot_turbines_with_fi(
-    fi: FlorisInterface,
-    ax: plt.Axes = None,
-    color: str = None,
-    wd: np.ndarray = None,
-    yaw_angles: np.ndarray = None,
-):
+    Display all open figures.  This is a wrapper for `plt.show()`.
+    This function is useful if the user doesn't wish to import `matplotlib.pyplot`
     """
-    Plot the wind plant layout from turbine locations gotten from a FlorisInterface object.
-    Note that this function automatically uses the first wind direction and first wind speed.
-    Generally, it is most explicit to create a new FlorisInterface with only the single
-    wind condition that should be plotted.
-
-    Args:
-        fi (:py:class:`floris.tools.floris_interface.FlorisInterface`): FlorisInterface object.
-        ax (:py:class:`matplotlib.pyplot.axes`): Figure axes. Defaults to None.
-        color (str, optional): Color to plot turbines. Defaults to None.
-        wd (list, optional): The wind direction to plot the turbines relative to. Defaults to None.
-        yaw_angles (NDArray, optional): The yaw angles for the turbines. Defaults to None.
-    """
-    if not ax:
-        fig, ax = plt.subplots()
-    if yaw_angles is None:
-        yaw_angles = fi.floris.farm.yaw_angles
-    if wd is None:
-        wd = fi.floris.flow_field.wind_directions[0]
-
-    # Rotate yaw angles to inertial frame for plotting turbines relative to wind direction
-    yaw_angles = yaw_angles - wind_delta(np.array(wd))
-
-    if color is None:
-        color = "k"
-
-    rotor_diameters = fi.floris.farm.rotor_diameters.flatten()
-    for x, y, yaw, d in zip(fi.layout_x, fi.layout_y, yaw_angles[0,0], rotor_diameters):
-        R = d / 2.0
-        x_0 = x + np.sin(np.deg2rad(yaw)) * R
-        x_1 = x - np.sin(np.deg2rad(yaw)) * R
-        y_0 = y - np.cos(np.deg2rad(yaw)) * R
-        y_1 = y + np.cos(np.deg2rad(yaw)) * R
-        ax.plot([x_0, x_1], [y_0, y_1], color=color)
-
-
-def add_turbine_id_labels(fi: FlorisInterface, ax: plt.Axes, **kwargs):
-    """
-    Adds index labels to a plot based on the given FlorisInterface.
-    See the pyplot.annotate docs for more info:
-    https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.annotate.html.
-    kwargs are passed to Text
-    (https://matplotlib.org/stable/api/text_api.html#matplotlib.text.Text).
-
-    Args:
-        fi (FlorisInterface): Simulation object to get the layout and index information.
-        ax (plt.Axes): Axes object to add the labels.
-    """
-
-    # Rotate layout to inertial frame for plotting turbines relative to wind direction
-    coordinates_array = np.array([
-        [x, y, 0.0]
-        for x, y in list(zip(fi.layout_x, fi.layout_y))
-    ])
-    wind_direction = fi.floris.flow_field.wind_directions[0]
-    layout_x, layout_y, _, _, _ = rotate_coordinates_rel_west(
-        np.array([wind_direction]),
-        coordinates_array
+    plt.show(
     )
 
-    for i in range(fi.floris.farm.n_turbines):
-        ax.annotate(
-            i,
-            (layout_x[0,0,i], layout_y[0,0,i]),
-            xytext=(0,10),
-            textcoords="offset points",
-            **kwargs
-        )
-
 
 def line_contour_cut_plane(
     cut_plane,
     ax=None,
     levels=None,
     colors=None,
     label_contours=False,
@@ -313,15 +191,15 @@
     ax.set_aspect("equal")
 
     return ax
 
 
 def visualize_heterogeneous_cut_plane(
     cut_plane,
-    fi,
+    fmodel,
     ax=None,
     vel_component='u',
     min_speed=None,
     max_speed=None,
     cmap="coolwarm",
     levels=None,
     clevels=None,
@@ -333,15 +211,15 @@
 ):
     """
     Generate pseudocolor mesh plot of the heterogeneous cut_plane.
 
     Args:
         cut_plane (:py:class:`~.tools.cut_plane.CutPlane`): 2D
             plane through wind plant.
-        fi (:py:class:`~.tools.floris_interface.FlorisInterface`): FlorisInterface object.
+        fmodel (:py:class:`~.floris_model.FlorisModel`): FlorisModel object.
         ax (:py:class:`matplotlib.pyplot.axes`): Figure axes. Defaults
             to None.
         vel_component (str, optional): The velocity component that the cut plane is
             perpendicular to.
         min_speed (float, optional): Minimum value of wind speed for
             contours. Defaults to None.
         max_speed (float, optional): Maximum value of wind speed for
@@ -415,16 +293,16 @@
     )
 
     # Plot the user-defined heterogeneous flow area
     if plot_het_bounds:
         points = np.array(
             list(
                 zip(
-                    fi.floris.flow_field.heterogenous_inflow_config['x'],
-                    fi.floris.flow_field.heterogenous_inflow_config['y'],
+                    fmodel.core.flow_field.heterogeneous_inflow_config['x'],
+                    fmodel.core.flow_field.heterogeneous_inflow_config['y'],
                 )
             )
         )
         hull = ConvexHull(points)
         h = ax.plot(
             points[np.append(hull.vertices, hull.vertices[0]),0],
             points[np.append(hull.vertices, hull.vertices[0]), 1],
@@ -504,34 +382,32 @@
         ax (:py:class:`matplotlib.pyplot.axes`): Figure axes.
     """
     ax.invert_xaxis()
 
 
 def plot_rotor_values(
     values: np.ndarray,
-    wd_index: int,
-    ws_index: int,
+    findex: int,
     n_rows: int,
     n_cols: int,
     t_range: range | None = None,
     cmap: str = "coolwarm",
     return_fig_objects: bool = False,
     save_path: Union[str, None] = None,
     show: bool = False
 ) -> Union[None, tuple[plt.figure, plt.axes, plt.axis, plt.colorbar]]:
     """
     Plots the gridded turbine rotor values. This is intended to be used for
     understanding the differences between two sets of values, so each subplot can be
     used for inspection of what values are differing, and under what conditions.
 
     Parameters:
-        values (np.ndarray): The 5-dimensional array of values to plot. Should be:
-            N wind directions x N wind speeds x N turbines X N rotor points X N rotor points.
-        wd_index (int): The index for the wind direction to plot.
-        ws_index (int): The index of the wind speed to plot.
+        values (np.ndarray): The 4-dimensional array of values to plot. Should be:
+            (N findex, N turbines, N rotor points, N rotor points).
+        findex (int): The index for the sample point to plot.
         n_rows (int): The number of rows to include for subplots. With ncols, this should
             generally add up to the number of turbines in the farm.
         n_cols (int): The number of columns to include for subplots. With ncols, this should
             generally add up to the number of turbines in the farm.
         t_range (range | None): Optional. The turbine count used to create the title for each
             subplot. If not provided, the size of the 2-th dimension of `values` is used.
         cmap (str): Optional. The matplotlib colormap to be used, default "coolwarm".
@@ -543,43 +419,43 @@
 
     Returns:
         None | tuple[plt.figure, plt.axes, plt.axis, plt.colorbar]: If
         `return_fig_objects` is `False, then `None` is returned`, otherwise the primary
         figure objects are returned for custom editing.
 
     Example:
-        from floris.tools.visualization import plot_rotor_values
-        plot_rotor_values(floris.flow_field.u, wd_index=0, ws_index=0, n_rows=1, ncols=4)
-        plot_rotor_values(floris.flow_field.v, wd_index=0, ws_index=0, n_rows=1, ncols=4)
-        plot_rotor_values(floris.flow_field.w, wd_index=0, ws_index=0, n_rows=1, ncols=4, show=True)
+        from floris.visualization import plot_rotor_values
+        plot_rotor_values(floris.flow_field.u, findex=0, n_rows=1, ncols=4)
+        plot_rotor_values(floris.flow_field.v, findex=0, n_rows=1, ncols=4)
+        plot_rotor_values(floris.flow_field.w, findex=0, n_rows=1, ncols=4, show=True)
     """
 
     cmap = plt.cm.get_cmap(name=cmap)
 
     if t_range is None:
-        t_range = range(values.shape[2])
+        t_range = range(values.shape[1])
 
     fig = plt.figure()
     axes = fig.subplots(n_rows, n_cols)
 
     # For 1x1, fig.subplots returns an Axes object, but for more than 1x1 it returns a np.array.
     # In this case, convert to an array so that the rest of this function can be simplified.
     if n_rows == 1 and n_cols == 1:
         axes = np.array([axes])
 
-    titles = np.array([f"T{i}" for i in t_range])
+    titles = np.array([f"tindex: {i}" for i in t_range])
 
     for ax, t, i in zip(axes.flatten(), titles, t_range):
 
-        vmin = np.min(values[wd_index, ws_index])
-        vmax = np.max(values[wd_index, ws_index])
+        vmin = np.min(values[findex])
+        vmax = np.max(values[findex])
 
         norm = mplcolors.Normalize(vmin, vmax)
 
-        ax.imshow(values[wd_index, ws_index, i].T, cmap=cmap, norm=norm, origin="lower")
+        ax.imshow(values[findex, i].T, cmap=cmap, norm=norm, origin="lower")
         ax.invert_xaxis()
 
         ax.set_xticks([])
         ax.set_yticks([])
         ax.set_title(t)
 
     fig.subplots_adjust(right=0.8)
@@ -592,90 +468,106 @@
     if return_fig_objects:
         return fig, axes, cbar_ax, cb
 
     if show:
         plt.show()
 
 def calculate_horizontal_plane_with_turbines(
-    fi_in,
+    fmodel,
     x_resolution=200,
     y_resolution=200,
     x_bounds=None,
     y_bounds=None,
-    wd=None,
-    ws=None,
-    yaw_angles=None,
+    findex_for_viz=None,
 ) -> CutPlane:
         """
         This function creates a :py:class:`~.tools.cut_plane.CutPlane` by
         adding an additional turbine to the farm and moving it through every
         a regular grid throughout the flow field. This method allows for
         visualizing wake models that do not support the FullFlowGrid and
         its associated solver. As the new turbine is moved around the flow
         field, the velocities at its rotor are stored in local variables,
         and the flow field is reset to its initial state for every new
         location. Then, the local velocities are put into a DataFrame and
         then into a CutPlane. This method is much slower than
-        `FlorisInterface.calculate_horizontal_plane`, but it is helpful
+        `FlorisModel.calculate_horizontal_plane`, but it is helpful
         for models where the visualization capability is not yet available.
 
         Args:
-            fi_in (:py:class:`floris.tools.floris_interface.FlorisInterface`):
-                Preinitialized FlorisInterface object.
+            fmodel (:py:class:`floris.floris_model.FlorisModel`):
+                Preinitialized FlorisModel object.
             x_resolution (float, optional): Output array resolution. Defaults to 200 points.
             y_resolution (float, optional): Output array resolution. Defaults to 200 points.
             x_bounds (tuple, optional): Limits of output array (in m). Defaults to None.
             y_bounds (tuple, optional): Limits of output array (in m). Defaults to None.
-            wd (float, optional): Wind direction setting. Defaults to None.
-            ws (float, optional): Wind speed setting. Defaults to None.
-            yaw_angles (np.ndarray, optional): Yaw angles settings. Defaults to None.
+            findex_for_viz (int, optional): Index of the condition to visualize.
 
         Returns:
             :py:class:`~.tools.cut_plane.CutPlane`: containing values of x, y, u, v, w
         """
+        if fmodel.core.flow_field.n_findex > 1 and findex_for_viz is None:
+            print(
+                "Multiple findices detected. Using first findex for visualization."
+            )
+        if findex_for_viz is None:
+            findex_for_viz = 0
 
-        # Make a local copy of fi to avoid editing passed in fi
-        fi = copy.deepcopy(fi_in)
-
-        # If wd/ws not provided, use what is set in fi
-        if wd is None:
-            wd = fi.floris.flow_field.wind_directions
-        if ws is None:
-            ws = fi.floris.flow_field.wind_speeds
-        fi.check_wind_condition_for_viz(wd=wd, ws=ws)
+        # Make a local copy of fmodel to avoid editing passed in fmodel
+        fmodel_viz = copy.deepcopy(fmodel)
 
         # Set the ws and wd
-        fi.reinitialize(wind_directions=wd, wind_speeds=ws)
+        fmodel_viz.set_for_viz(findex_for_viz, None)
 
-        # Re-set yaw angles
-        if yaw_angles is not None:
-            fi.floris.farm.yaw_angles = yaw_angles
-
-        # Now place the yaw_angles back into yaw_angles
-        # to be sure not None
-        yaw_angles = fi.floris.farm.yaw_angles
+        yaw_angles = fmodel_viz.core.farm.yaw_angles
+        power_setpoints = fmodel_viz.core.farm.power_setpoints
+        awc_modes = fmodel_viz.core.farm.awc_modes
+        awc_amplitudes = fmodel_viz.core.farm.awc_amplitudes
+        awc_frequencies = fmodel_viz.core.farm.awc_frequencies
 
         # Grab the turbine layout
-        layout_x = copy.deepcopy(fi.layout_x)
-        layout_y = copy.deepcopy(fi.layout_y)
-        turbine_types = copy.deepcopy(fi.floris.farm.turbine_type)
-        D = fi.floris.farm.rotor_diameters_sorted[0, 0, 0]
+        layout_x = copy.deepcopy(fmodel_viz.layout_x)
+        layout_y = copy.deepcopy(fmodel_viz.layout_y)
+        turbine_types = copy.deepcopy(fmodel_viz.core.farm.turbine_type)
+        D = fmodel_viz.core.farm.rotor_diameters_sorted[0, 0]
 
         # Declare a new layout array with an extra turbine
         layout_x_test = np.append(layout_x,[0])
         layout_y_test = np.append(layout_y,[0])
 
-        # Declare turbine types with an extra turbine in
-        # case of special one type useage
+        # Declare turbine types with an extra turbine in case of special one-type usage
         if len(layout_x) > 1 and len(turbine_types) == 1:
             # Convert to list length len(layout_x) + 1
             turbine_types_test = [turbine_types[0] for i in range(len(layout_x))] + ['nrel_5MW']
         else:
             turbine_types_test = np.append(turbine_types, 'nrel_5MW').tolist()
-        yaw_angles = np.append(yaw_angles, np.zeros([len(wd), len(ws), 1]), axis=2)
+        yaw_angles = np.append(
+            yaw_angles,
+            np.zeros([fmodel_viz.core.flow_field.n_findex, 1]),
+            axis=1
+        )
+        power_setpoints = np.append(
+            power_setpoints,
+            POWER_SETPOINT_DEFAULT * np.ones([fmodel_viz.core.flow_field.n_findex, 1]),
+            axis=1
+        )
+        awc_modes = np.append(
+            awc_modes,
+            np.full((fmodel_viz.core.flow_field.n_findex, 1), "baseline"),
+            axis=1
+        )
+        awc_amplitudes = np.append(
+            awc_amplitudes,
+            np.zeros([fmodel_viz.core.flow_field.n_findex, 1]),
+            axis=1
+        )
+        awc_frequencies = np.append(
+            awc_frequencies,
+            np.zeros([fmodel_viz.core.flow_field.n_findex, 1]),
+            axis=1
+        )
 
         # Get a grid of points test test
         if x_bounds is None:
             x_bounds = (np.min(layout_x) - 2 * D, np.max(layout_x) + 10 * D)
 
         if y_bounds is None:
             y_bounds = (np.min(layout_y) - 2 * D, np.max(layout_y) + 2 * D)
@@ -699,24 +591,29 @@
                 # Save the x and y results
                 x_results[idx] = x
                 y_results[idx] = y
 
                 # Place the test turbine at this location and calculate wake
                 layout_x_test[-1] = x
                 layout_y_test[-1] = y
-                fi.reinitialize(
+                fmodel_viz.set(
                     layout_x=layout_x_test,
                     layout_y=layout_y_test,
+                    yaw_angles=yaw_angles,
+                    power_setpoints=power_setpoints,
+                    awc_modes=awc_modes,
+                    awc_amplitudes=awc_amplitudes,
+                    awc_frequencies=awc_frequencies,
                     turbine_type=turbine_types_test
                 )
-                fi.calculate_wake(yaw_angles=yaw_angles)
+                fmodel_viz.run()
 
                 # Get the velocity of that test turbines central point
-                center_point = int(np.floor(fi.floris.flow_field.u[0,0,-1].shape[0] / 2.0))
-                u_results[idx] = fi.floris.flow_field.u[0,0,-1,center_point,center_point]
+                center_point = int(np.floor(fmodel_viz.core.flow_field.u[0,-1].shape[0] / 2.0))
+                u_results[idx] = fmodel_viz.core.flow_field.u[0,-1,center_point,center_point]
 
                 # Increment index
                 idx = idx + 1
 
         # Make a dataframe
         df = pd.DataFrame({
             'x1':x_results,
```

### Comparing `FLORIS-3.6/floris/turbine_library/turbine_previewer.py` & `FLORIS-4/floris/turbine_library/turbine_previewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,38 @@
-# Copyright 2023 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 from pathlib import Path
 
 import attrs
 import matplotlib.pyplot as plt
 import numpy as np
 from attrs import define, field
 
-from floris.simulation.turbine import (
-    Ct,
+from floris.core.turbine.operation_models import POWER_SETPOINT_DEFAULT
+from floris.core.turbine.turbine import (
     power,
+    thrust_coefficient,
     Turbine,
 )
-from floris.simulation.turbine_multi_dim import (
-    Ct_multidim,
-    multidim_Ct_down_select,
-    multidim_power_down_select,
-    power_multidim,
-    TurbineMultiDimensional,
-)
 from floris.type_dec import convert_to_path, NDArrayFloat
 from floris.utilities import (
     load_yaml,
     round_nearest,
     round_nearest_2_or_5,
 )
 
 
 INTERNAL_LIBRARY = Path(__file__).parent
 DEFAULT_WIND_SPEEDS = np.linspace(0, 40, 81)
 
 
 @define(auto_attribs=True)
 class TurbineInterface:
-    turbine: Turbine | TurbineMultiDimensional = field(
-        validator=attrs.validators.instance_of((Turbine, TurbineMultiDimensional))
-    )
+    turbine: Turbine = field(validator=attrs.validators.instance_of(Turbine))
 
     @classmethod
     def from_library(cls, library_path: str | Path, file_name: str):
         """Loads the turbine definition from a YAML configuration file located in either the
         internal turbine library ``floris/floris/turbine_library/``, or a user-specified location.
 
         Args:
@@ -68,17 +47,14 @@
         if library_path == "internal":
             library_path = INTERNAL_LIBRARY
         else:
             library_path = convert_to_path(library_path)
 
         # Add in the library specification if needed, and load from dict
         turb_dict = load_yaml(library_path / file_name)
-        if turb_dict.get("multi_dimensional_cp_ct", False):
-            turb_dict.setdefault("turbine_library_path", library_path)
-            return cls(turbine=TurbineMultiDimensional.from_dict(turb_dict))
         return cls(turbine=Turbine.from_dict(turb_dict))
 
     @classmethod
     def from_yaml(cls, file_path: str | Path):
         """Loads the turbine definition from a YAML configuration file.
 
         Args:
@@ -88,35 +64,30 @@
         Returns:
             (TurbineInterface): Creates a new ``TurbineInterface`` object.
         """
         file_path = Path(file_path).resolve()
 
         # Add in the library specification if needed, and load from dict
         turb_dict = load_yaml(file_path)
-        if turb_dict.get("multi_dimensional_cp_ct", False):
-            turb_dict.setdefault("turbine_library_path", file_path.parent)
-            return cls(turbine=TurbineMultiDimensional.from_dict(turb_dict))
         return cls(turbine=Turbine.from_dict(turb_dict))
 
     @classmethod
     def from_turbine_dict(cls, config_dict: dict):
         """Loads the turbine definition from a dictionary.
 
         Args:
             config_dict : dict
                 The ``Turbine`` configuration dictionary.
 
         Returns:
             (`TurbineInterface`): Returns a ``TurbineInterface`` object.
         """
-        if config_dict.get("multi_dimensional_cp_ct", False):
-            return cls(turbine=TurbineMultiDimensional.from_dict(config_dict))
         return cls(turbine=Turbine.from_dict(config_dict))
 
-    def  power_curve(
+    def power_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
     ) -> tuple[NDArrayFloat, NDArrayFloat] | tuple[NDArrayFloat, dict[tuple, NDArrayFloat]]:
         """Produces a plot-ready power curve for the turbine for wind speed vs power (MW), assuming
         no tilt or yaw effects.
 
         Args:
@@ -124,88 +95,104 @@
                 0 m/s -> 40 m/s, every 0.5 m/s.
 
         Returns:
             (tuple[NDArrayFloat, NDArrayFloat] | tuple[NDArrayFloat, dict[tuple, NDArrayFloat]]):
                 Returns the wind speed array and the power array, or the wind speed array and a
                 dictionary of the multidimensional parameters and their associated power arrays.
         """
-        shape = (1, wind_speeds.size, 1)
+        shape = (wind_speeds.size, 1)
         if self.turbine.multi_dimensional_cp_ct:
-            power_interps = {
-                k: multidim_power_down_select(
-                    np.full(shape, self.turbine.power_interp),
-                    dict(zip(self.turbine.condition_keys, k)),
-                )
-                for k in self.turbine.power_interp
-            }
             power_mw = {
-                k: power_multidim(
-                    ref_density_cp_ct=np.full(shape, self.turbine.ref_density_cp_ct),
-                    rotor_effective_velocities=wind_speeds.reshape(shape),
-                    power_interp=power_interps[k],
+                k: power(
+                    velocities=wind_speeds.reshape(shape),
+                    air_density=np.full(shape, v["ref_air_density"]),
+                    power_functions={self.turbine.turbine_type: self.turbine.power_function},
+                    yaw_angles=np.zeros(shape),
+                    tilt_angles=np.full(shape, v["ref_tilt"]),
+                    power_setpoints=np.full(shape, POWER_SETPOINT_DEFAULT),
+                    awc_modes=np.full(shape, ["baseline"]),
+                    awc_amplitudes=np.zeros(shape),
+                    tilt_interps={self.turbine.turbine_type: self.turbine.tilt_interp},
+                    turbine_type_map=np.full(shape, self.turbine.turbine_type),
+                    turbine_power_thrust_tables={self.turbine.turbine_type: v},
                 ).flatten() / 1e6
-                for k in self.turbine.power_interp
+                for k,v in self.turbine.power_thrust_table.items()
             }
         else:
             power_mw = power(
-                ref_density_cp_ct=np.full(shape, self.turbine.ref_density_cp_ct),
-                rotor_effective_velocities=wind_speeds.reshape(shape),
-                power_interp={self.turbine.turbine_type: self.turbine.power_interp},
-                turbine_type_map=np.full(shape, self.turbine.turbine_type)
+                velocities=wind_speeds.reshape(shape),
+                air_density=np.full(shape, self.turbine.power_thrust_table["ref_air_density"]),
+                power_functions={self.turbine.turbine_type: self.turbine.power_function},
+                yaw_angles=np.zeros(shape),
+                tilt_angles=np.full(shape, self.turbine.power_thrust_table["ref_tilt"]),
+                power_setpoints=np.full(shape, POWER_SETPOINT_DEFAULT),
+                awc_modes=np.full(shape, ["baseline"]),
+                awc_amplitudes=np.zeros(shape),
+                tilt_interps={self.turbine.turbine_type: self.turbine.tilt_interp},
+                turbine_type_map=np.full(shape, self.turbine.turbine_type),
+                turbine_power_thrust_tables={
+                    self.turbine.turbine_type: self.turbine.power_thrust_table
+                },
             ).flatten() / 1e6
         return wind_speeds, power_mw
 
-    def Ct_curve(
+    def thrust_coefficient_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
     ) -> tuple[NDArrayFloat, NDArrayFloat]:
         """Produces a plot-ready thrust curve for the turbine for wind speed vs thrust coefficient
         assuming no tilt or yaw effects.
 
         Args:
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
 
         Returns:
             tuple[NDArrayFloat, NDArrayFloat]
                 Returns the wind speed array and the thrust coefficient array.
         """
-        shape = (1, wind_speeds.size, 1)
-        shape_single = (1, 1, 1)
+        shape = (wind_speeds.size, 1)
         if self.turbine.multi_dimensional_cp_ct:
-            fCt_interps = {
-                k: multidim_Ct_down_select(
-                    np.full(shape, self.turbine.fCt_interp),
-                    dict(zip(self.turbine.condition_keys, k)),
-                )
-                for k in self.turbine.fCt_interp
-            }
             ct_curve = {
-                k: Ct_multidim(
+                k: thrust_coefficient(
                     velocities=wind_speeds.reshape(shape),
-                    yaw_angle=np.zeros(shape),
-                    tilt_angle=np.full(shape, self.turbine.ref_tilt_cp_ct),
-                    ref_tilt_cp_ct=np.full(shape_single, self.turbine.ref_tilt_cp_ct),
-                    fCt=fCt_interps[k],
-                    tilt_interp={self.turbine.turbine_type: self.turbine.tilt_interp},
-                    correct_cp_ct_for_tilt=np.zeros(shape_single, dtype=bool),
-                    turbine_type_map=np.full(shape_single, self.turbine.turbine_type)
+                    air_density=np.full(shape, v["ref_air_density"]),
+                    yaw_angles=np.zeros(shape),
+                    tilt_angles=np.full(shape, v["ref_tilt"]),
+                    power_setpoints=np.full(shape, POWER_SETPOINT_DEFAULT),
+                    awc_modes=np.full(shape, ["baseline"]),
+                    awc_amplitudes=np.zeros(shape),
+                    thrust_coefficient_functions={
+                        self.turbine.turbine_type: self.turbine.thrust_coefficient_function
+                    },
+                    tilt_interps={self.turbine.turbine_type: self.turbine.tilt_interp},
+                    correct_cp_ct_for_tilt=np.zeros(shape, dtype=bool),
+                    turbine_type_map=np.full(shape, self.turbine.turbine_type),
+                    turbine_power_thrust_tables={self.turbine.turbine_type: v},
                 ).flatten()
-                for k in self.turbine.fCt_interp
+                for k,v in self.turbine.power_thrust_table.items()
             }
         else:
-            ct_curve = Ct(
+            ct_curve = thrust_coefficient(
                 velocities=wind_speeds.reshape(shape),
-                yaw_angle=np.zeros(shape),
-                tilt_angle=np.full(shape, self.turbine.ref_tilt_cp_ct),
-                ref_tilt_cp_ct=np.full(shape, self.turbine.ref_tilt_cp_ct),
-                fCt={self.turbine.turbine_type: self.turbine.fCt_interp},
-                tilt_interp={self.turbine.turbine_type: self.turbine.tilt_interp},
+                air_density=np.full(shape, self.turbine.power_thrust_table["ref_air_density"]),
+                yaw_angles=np.zeros(shape),
+                tilt_angles=np.full(shape, self.turbine.power_thrust_table["ref_tilt"]),
+                power_setpoints=np.full(shape, POWER_SETPOINT_DEFAULT),
+                awc_modes=np.full(shape, ["baseline"]),
+                awc_amplitudes=np.zeros(shape),
+                thrust_coefficient_functions={
+                    self.turbine.turbine_type: self.turbine.thrust_coefficient_function
+                },
+                tilt_interps={self.turbine.turbine_type: self.turbine.tilt_interp},
                 correct_cp_ct_for_tilt=np.zeros(shape, dtype=bool),
                 turbine_type_map=np.full(shape, self.turbine.turbine_type),
+                turbine_power_thrust_tables={
+                    self.turbine.turbine_type: self.turbine.power_thrust_table
+                },
             ).flatten()
         return wind_speeds, ct_curve
 
     def plot_power_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
         fig_kwargs: dict | None =  None,
@@ -271,15 +258,15 @@
         ax.set_ylabel("Power (MW)")
 
         if return_fig:
             return fig, ax
 
         fig.tight_layout()
 
-    def plot_Ct_curve(
+    def plot_thrust_coefficient_curve(
         self,
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
         fig_kwargs: dict | None =  None,
         plot_kwargs: dict | None =  None,
         legend_kwargs: dict | None =  None,
         return_fig: bool = False
     ) -> None | tuple[plt.Figure, plt.Axes]:
@@ -297,15 +284,15 @@
             return_fig (bool, optional): Indicator if the ``Figure`` and ``Axes`` objects should be
                 returned. Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
-        wind_speeds, thrust = self.Ct_curve(wind_speeds=wind_speeds)
+        wind_speeds, thrust = self.thrust_coefficient_curve(wind_speeds=wind_speeds)
 
         # Initialize kwargs if None
         fig_kwargs = {} if fig_kwargs is None else fig_kwargs
         plot_kwargs = {} if plot_kwargs is None else plot_kwargs
         legend_kwargs = {} if legend_kwargs is None else legend_kwargs
 
         # Set the figure defaults if none are provided
@@ -344,16 +331,15 @@
         fig.tight_layout()
 
 
 @define(auto_attribs=True)
 class TurbineLibrary:
     turbine_map: dict[str: TurbineInterface] = field(factory=dict)
     power_curves: dict[str, tuple[NDArrayFloat, NDArrayFloat]] = field(factory=dict)
-    Cp_curves: dict[str, tuple[NDArrayFloat, NDArrayFloat]] = field(factory=dict)
-    Ct_curves: dict[str, tuple[NDArrayFloat, NDArrayFloat]] = field(factory=dict)
+    thrust_coefficient_curves: dict[str, tuple[NDArrayFloat, NDArrayFloat]] = field(factory=dict)
 
     def load_internal_library(self, which: list[str] = [], exclude: list[str] = []) -> None:
         """Loads all of the turbine configurations from ``floris/floris/turbine_libary``,
         except any turbines defined in :py:attr:`exclude`.
 
         Args:
             which (list[str], optional): A list of which file names to include from loading.
@@ -411,27 +397,27 @@
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
         """
         self.power_curves = {
             name: t.power_curve(wind_speeds) for name, t in self.turbine_map.items()
         }
 
-    def compute_Ct_curves(
+    def compute_thrust_coefficient_curves(
             self,
             wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
         ) -> None:
         """Computes the thrust curves for each turbine in ``turbine_map`` and sets the
-        ``Ct_curves`` attribute.
+        ``thrust_coefficient_curves`` attribute.
 
         Args:
             wind_speeds (NDArrayFloat, optional): A 1-D array of wind speeds, in m/s. Defaults to
                 0 m/s -> 40 m/s, every 0.5 m/s.
         """
-        self.Ct_curves = {
-            name: t.Ct_curve(wind_speeds) for name, t in self.turbine_map.items()
+        self.thrust_coefficient_curves = {
+            name: t.thrust_coefficient_curve(wind_speeds) for name, t in self.turbine_map.items()
         }
 
     def plot_power_curves(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
@@ -519,15 +505,15 @@
 
         if return_fig:
             return fig, ax
 
         if show:
             fig.tight_layout()
 
-    def plot_Ct_curves(
+    def plot_thrust_coefficient_curves(
         self,
         fig: plt.Figure | None = None,
         ax: plt.Axes | None = None,
         which: list[str] = [],
         exclude: list[str] = [],
         wind_speeds: NDArrayFloat = DEFAULT_WIND_SPEEDS,
         fig_kwargs: dict | None =  None,
@@ -558,16 +544,16 @@
             show (bool, optional): Indicator if the figure should be automatically displayed.
                 Defaults to False.
 
         Returns:
             None | tuple[plt.Figure, plt.Axes]: None, if :py:attr:`return_fig` is False, otherwise
                 a tuple of the Figure and Axes objects are returned.
         """
-        if self.Ct_curves == {} or wind_speeds is None:
-            self.compute_Ct_curves(wind_speeds=wind_speeds)
+        if self.thrust_coefficient_curves == {} or wind_speeds is None:
+            self.compute_thrust_coefficient_curves(wind_speeds=wind_speeds)
 
         which = [*self.turbine_map] if which == [] else which
 
         # Initialize kwargs if None
         fig_kwargs = {} if fig_kwargs is None else fig_kwargs
         plot_kwargs = {} if plot_kwargs is None else plot_kwargs
         legend_kwargs = {} if legend_kwargs is None else legend_kwargs
@@ -581,15 +567,15 @@
             fig = plt.figure(**fig_kwargs)
         if ax is None:
             ax = fig.add_subplot(111)
 
         min_windspeed = 0
         max_windspeed = 0
         max_thrust = 0
-        for name, (ws, t) in self.Ct_curves.items():
+        for name, (ws, t) in self.thrust_coefficient_curves.items():
             if name in exclude or name not in which:
                 continue
             if isinstance(t, dict):
                 max_windspeed = max(ws.max(), max_windspeed)
                 for k, _t in t.items():
                     max_thrust = max(_t.max(), max_thrust)
                     label = f"{name} - {k}"
@@ -820,15 +806,15 @@
             fig,
             ax1,
             which=which,
             exclude=exclude,
             wind_speeds=wind_speeds,
             plot_kwargs=plot_kwargs,
         )
-        self.plot_Ct_curves(
+        self.plot_thrust_coefficient_curves(
             fig,
             ax3,
             which=which,
             exclude=exclude,
             wind_speeds=wind_speeds,
             plot_kwargs=plot_kwargs,
         )
```

### Comparing `FLORIS-3.6/floris/turbine_library/turbine_utilities.py` & `FLORIS-4/floris/turbine_library/turbine_utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import os.path
+
+from __future__ import annotations
+
+from collections.abc import Iterable
 
 import numpy as np
 import yaml
 
 
-def build_turbine_dict(
+def build_cosine_loss_turbine_dict(
     turbine_data_dict,
     turbine_name,
-    file_path=None,
-    generator_efficiency=1.0,
+    file_name=None,
+    generator_efficiency=None,
     hub_height=90.0,
-    pP=1.88,
-    pT=1.88,
-    rotor_diameter=126.0,
+    cosine_loss_exponent_yaw=1.88,
+    cosine_loss_exponent_tilt=1.88,
+    rotor_diameter=125.88,
     TSR=8.0,
-    air_density=1.225,
-    ref_tilt_cp_ct=5.0
+    ref_air_density=1.225,
+    ref_tilt=5.0
 ):
     """
     Tool for formatting a full turbine dict from data formatted as a
     dictionary.
 
     Default value for turbine physical parameters are from the NREL 5MW reference
     wind turbine.
@@ -27,140 +30,171 @@
     Returns a turbine dictionary object as expected by FLORIS. Optionally,
     prints the dictionary to a yaml to be included in a FLORIS wake model yaml.
 
     turbine_data is a dictionary that contains keys specifying the
     turbine power and thrust as a function of wind speed. The following keys
     are possible:
     - wind_speed [m/s]
-    - power_absolute [kW]
+    - power [kW]
     - power_coefficient [-]
-    - thrust_absolute [kN]
+    - thrust [kN]
     - thrust_coefficient [-]
-    Of these, wind_speed is required. One of power_absolute and power_coefficient
-    must be specified; and one of thrust_absolute and thrust_coefficient must be
-    specified. If both _absolute and _coefficient versions are specified, the
-    _coefficient entry will be used and the _absolute entry ignored.
+    Of these, wind_speed is required. One of power and power_coefficient
+    must be specified; and one of thrust and thrust_coefficient must be
+    specified. If both (absolute) and _coefficient versions are specified, the
+    (absolute) power will be used along with the thrust_coefficient, with the
+    other entries ignored.
 
     Args:
         turbine_data_dict (dict): Dictionary containing performance of the wind
             turbine as a function of wind speed. Described in more detail above.
         turbine_name (string): Name of the turbine, which will be used for the
             turbine_type field as well as the filename.
-        file_path (): Path for placement of the produced yaml. Defaults to None,
-            in which case no yaml is written.
-        generator_efficiency (float): Generator efficiency [-]. Defaults to 1.0.
+        file_name (): Name for the produced yaml, including possibly path.
+            Defaults to None, in which case no yaml is written.
+        generator_efficiency (float): Generator efficiency [-]. Unused if power is specified
+            in absolute terms in the turbine_data_dict. Must be specified if
+            power not specified and power_coefficient specified instead. Defaults to None.
         hub_height (float): Hub height [m]. Defaults to 90.0.
-        pP (float): Cosine exponent for power loss to yaw [-]. Defaults to 1.88.
-        pT (float): Cosine exponent for thrust loss to yaw [-]. Defaults to 1.88.
+        cosine_loss_exponent_yaw (float): Cosine exponent for power loss to yaw [-].
+            Defaults to 1.88.
+        cosine_loss_exponent_tilt (float): Cosine exponent for thrust loss to yaw [-].
+            Defaults to 1.88.
         rotor_diameter (float). Rotor diameter [m]. Defaults to 126.0.
         TSR (float). Turbine optimal tip-speed ratio [-]. Defaults to 8.0.
-        air_density (float). Air density used to specify power and thrust
+        ref_air_density (float). Air density used to specify power and thrust
             curves [kg/m^3]. Defaults to 1.225.
-        ref_tilt_cp_ct (float). Rotor tilt (due to shaft tilt and/or platform
+        ref_tilt (float). Rotor tilt (due to shaft tilt and/or platform
             tilt) used when defining the power and thrust curves [deg]. Defaults
             to 5.0.
 
     Returns:
         turbine_dict (dict): Formatted turbine dictionary as expected by FLORIS.
     """
 
     # Check that necessary columns are specified
     if "wind_speed" not in turbine_data_dict:
         raise KeyError("wind_speed column must be specified.")
     u = np.array(turbine_data_dict["wind_speed"])
     A = np.pi * rotor_diameter**2/4
 
     # Construct the Cp curve
-    if "power_coefficient" in turbine_data_dict:
-        if "power_absolute" in turbine_data_dict:
+    if "power" in turbine_data_dict:
+        if "power_coefficient" in turbine_data_dict:
             print(
-                "Found both power_absolute and power_coefficient."
-                "Ignoring power_absolute."
+                "Found both power and power_coefficient. "
+                "Ignoring power_coefficient."
             )
-        Cp = np.array(turbine_data_dict["power_coefficient"])
+        p = np.array(turbine_data_dict["power"])
 
-    elif "power_absolute" in turbine_data_dict:
-        P = np.array(turbine_data_dict["power_absolute"])
-        if _find_nearest_value_for_wind_speed(P, u, 10) > 20000 or \
-           _find_nearest_value_for_wind_speed(P, u, 10) < 1000:
+    elif "power_coefficient" in turbine_data_dict:
+        if generator_efficiency is None:
+            raise KeyError(
+                "generator_efficiency must be specified to convert power_coefficient to power."
+            )
+        Cp = np.array(turbine_data_dict["power_coefficient"])
+        if _find_nearest_value_for_wind_speed(Cp, u, 10) > 16.0/27.0 or \
+           _find_nearest_value_for_wind_speed(Cp, u, 10) < 0.0:
            print(
-               "Unusual power value detected. Please check that power_absolute",
-               "is specified in kW."
+               "Unusual power coefficient detected. Check that power coefficients"
+               "are physical."
            )
 
-        validity_mask = (P != 0) | (u != 0)
-        Cp = np.zeros_like(P, dtype=float)
+        validity_mask = (Cp != 0) | (u != 0)
+        p = np.zeros_like(Cp, dtype=float)
 
-        Cp[validity_mask] = (P[validity_mask]*1000) / \
-                            (0.5*air_density*A*u[validity_mask]**3)
+        p[validity_mask] = (
+            Cp[validity_mask]
+            * 0.5 * ref_air_density * A * generator_efficiency
+            * u[validity_mask]**3 / 1000
+        )
 
     else:
         raise KeyError(
-            "Either power_absolute or power_coefficient must be specified."
+            "Either power or power_coefficient must be specified."
         )
 
     # Construct Ct curve
     if "thrust_coefficient" in turbine_data_dict:
-        if "thrust_absolute" in turbine_data_dict:
+        if "thrust" in turbine_data_dict:
             print(
-                "Found both thrust_absolute and thrust_coefficient."
-                "Ignoring thrust_absolute."
+                "Found both thrust and thrust_coefficient. "
+                "Ignoring thrust."
             )
         Ct = np.array(turbine_data_dict["thrust_coefficient"])
 
-    elif "thrust_absolute" in turbine_data_dict:
-        T = np.array(turbine_data_dict["thrust_absolute"])
+    elif "thrust" in turbine_data_dict:
+        T = np.array(turbine_data_dict["thrust"])
         if _find_nearest_value_for_wind_speed(T, u, 10) > 3000 or \
            _find_nearest_value_for_wind_speed(T, u, 10) < 100:
            print(
-               "Unusual thrust value detected. Please check that thrust_absolute",
+               "Unusual thrust value detected. Please check that thrust",
                "is specified in kN."
            )
 
         validity_mask = (T != 0) | (u != 0)
         Ct = np.zeros_like(T)
 
         Ct[validity_mask] = (T[validity_mask]*1000)/\
-                            (0.5*air_density*A*u[validity_mask]**2)
+                            (0.5*ref_air_density*A*u[validity_mask]**2)
 
     else:
         raise KeyError(
-            "Either thrust_absolute or thrust_coefficient must be specified."
+            "Either thrust or thrust_coefficient must be specified."
         )
 
     # Build the turbine dict
     power_thrust_dict = {
+        "ref_air_density": ref_air_density,
+        "ref_tilt": ref_tilt,
+        "cosine_loss_exponent_yaw": cosine_loss_exponent_yaw,
+        "cosine_loss_exponent_tilt": cosine_loss_exponent_tilt,
         "wind_speed": u.tolist(),
-        "power": Cp.tolist(),
-        "thrust": Ct.tolist()
+        "power": p.tolist(),
+        "thrust_coefficient": Ct.tolist()
     }
 
     turbine_dict = {
         "turbine_type": turbine_name,
-        "generator_efficiency": generator_efficiency,
         "hub_height": hub_height,
-        "pP": pP,
-        "pT": pT,
         "rotor_diameter": rotor_diameter,
         "TSR": TSR,
-        "ref_density_cp_ct": air_density,
-        "ref_tilt_cp_ct": ref_tilt_cp_ct,
+        "operation_model": "cosine-loss",
         "power_thrust_table": power_thrust_dict
     }
 
     # Create yaml file
-    if file_path is not None:
-        full_name = os.path.join(file_path, turbine_name+".yaml")
+    if file_name is not None:
         yaml.dump(
             turbine_dict,
-            open(full_name, "w"),
+            open(file_name, "w"),
             sort_keys=False
         )
 
-        print(full_name, "created.")
+        print(file_name, "created.")
 
     return turbine_dict
 
 def _find_nearest_value_for_wind_speed(test_vals, ws_vals, ws):
     errs = np.absolute(ws_vals-ws)
     idx = errs.argmin()
     return test_vals[idx]
+
+def check_smooth_power_curve(power, tolerance=0.001):
+    """
+    Check whether there are "wiggles" in the power signal.
+    """
+
+    if power[-1] < 0.95*max(power): # Cut-out or shutdown included
+        expected_changes = 2
+    else: # Shutdown appears not to be included
+        expected_changes = 1
+
+    dirs = np.where(
+        np.abs(np.diff(power)) > tolerance,
+        np.sign(np.diff(power)),
+        np.zeros(len(power)-1)
+    )
+    dir_changes = np.sum(np.abs(np.diff(dirs)))
+    is_smooth = dir_changes <= expected_changes
+
+    return is_smooth
```

### Comparing `FLORIS-3.6/floris/type_dec.py` & `FLORIS-4/floris/type_dec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import copy
 import inspect
 from pathlib import Path
 from typing import (
@@ -36,30 +23,70 @@
 floris_float_type = np.float64
 
 NDArrayFloat = npt.NDArray[floris_float_type]
 NDArrayInt = npt.NDArray[np.int_]
 NDArrayFilter = Union[npt.NDArray[np.int_], npt.NDArray[np.bool_]]
 NDArrayObject = npt.NDArray[np.object_]
 NDArrayBool = npt.NDArray[np.bool_]
+NDArrayStr = npt.NDArray[np.str_]
 
 
 ### Custom callables for attrs objects and functions
 
 def floris_array_converter(data: Iterable) -> np.ndarray:
+    """
+    For a given iterable, convert the data to a numpy array and cast to `floris_float_type`.
+    If the input is a scalar, np.array() creates a 0-dimensional array, and this is not supported
+    in FLORIS so this function raises an error.
+
+    Args:
+        data (Iterable): The input data to be converted to a Numpy array.
+
+    Raises:
+        TypeError: Raises if the input data is not iterable.
+        TypeError: Raises if the input data cannot be converted to a Numpy array.
+
+    Returns:
+        np.ndarray: data converted to a Numpy array and cast to `floris_float_type`.
+    """
     try:
-        a = np.array(data, dtype=floris_float_type)
+        iter(data)
     except TypeError as e:
         raise TypeError(e.args[0] + f". Data given: {data}")
-    return a
 
-def floris_numeric_dict_converter(data: dict) -> dict:
     try:
-        return {k: floris_array_converter(v) for k, v in data.items()}
-    except TypeError as e:
+        a = np.array(data, dtype=floris_float_type)
+    except (TypeError, ValueError) as e:
         raise TypeError(e.args[0] + f". Data given: {data}")
+    return a
+
+def floris_numeric_dict_converter(data: dict) -> dict:
+    """
+    For the given dictionary, convert all the values to a numeric type. If a value is a scalar, it
+    will be converted to a float. If a value is an iterable, it will be converted to a Numpy
+    array and cast to `floris_float_type`. If a value is not a numeric type, a TypeError will be
+    raised.
+
+    Args:
+        data (dict): Dictionary of data to be converted to a numeric type.
+
+    Returns:
+        dict: Dictionary with the same keys and all values converted to a numeric type.
+    """
+    converted_dict = copy.deepcopy(data)  # deepcopy -> data is a container and passed by reference
+    for k, v in data.items():
+        try:
+            iter(v)
+        except TypeError:
+            # Not iterable so try to cast to float
+            converted_dict[k] = float(v)
+        else:
+            # Iterable so convert to Numpy array
+            converted_dict[k] = floris_array_converter(v)
+    return converted_dict
 
 # def array_field(**kwargs) -> Callable:
 #     """
 #     A wrapper for the :py:func:`attr.field` function that converts the input to a Numpy array,
 #     adds a comparison function specific to Numpy arrays, and passes through all additional
 #     keyword arguments.
 #     """
```

### Comparing `FLORIS-3.6/floris/utilities.py` & `FLORIS-4/floris/utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
 import os
 from math import ceil
-from typing import Tuple
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+)
 
 import numpy as np
 import yaml
 from attrs import define, field
 
 from floris.type_dec import floris_array_converter, NDArrayFloat
 
@@ -142,15 +135,15 @@
             input coordinates. Defaults to None.
         y_center_of_rotation (float, optional): The y-coordinate for the rotational center of the
             input coordinates. Defaults to None.
     """
 
     # Calculate the difference in given wind direction from 270 / West
     wind_deviation_from_west = wind_delta(wind_directions)
-    wind_deviation_from_west = np.reshape(wind_deviation_from_west, (len(wind_directions), 1, 1))
+    wind_deviation_from_west = np.reshape(wind_deviation_from_west, (len(wind_directions), 1))
 
     # Construct the arrays storing the turbine locations
     x_coordinates, y_coordinates, z_coordinates = coordinates.T
 
     # Find center of rotation - this is the center of box bounding all of the turbines
     if x_center_of_rotation is None:
         x_center_of_rotation = (np.min(x_coordinates) + np.max(x_coordinates)) / 2
@@ -185,16 +178,14 @@
 ):
     """
     This function reverses the rotation of the given grid so that the coordinates are aligned with
     the original wind direction. The rotation happens about the centroid of the coordinates.
 
     Args:
         wind_directions (NDArrayFloat): Series of wind directions to base the rotation.
-        coordinates (NDArrayFloat): Series of coordinates to rotate with shape (N coordinates, 3)
-            so that each element of the array coordinates[i] yields a three-component coordinate.
         grid_x (NDArrayFloat): X-coordinates to be rotated.
         grid_y (NDArrayFloat): Y-coordinates to be rotated.
         grid_z (NDArrayFloat): Z-coordinates to be rotated.
         x_center_of_rotation (float): The x-coordinate for the rotation center of the
             input coordinates.
         y_center_of_rotation (float): The y-coordinate for the rotational center of the
             input coordinates.
@@ -277,7 +268,73 @@
     Args:
         x (int | float): The number to be rounded.
 
     Returns:
         int: The rounded number.
     """
     return base * ceil((x + 0.5) / base)
+
+
+def nested_get(
+    d: Dict[str, Any],
+    keys: List[str]
+) -> Any:
+    """Get a value from a nested dictionary using a list of keys.
+    Based on:
+    https://stackoverflow.com/questions/14692690/access-nested-dictionary-items-via-a-list-of-keys
+
+    Args:
+        d (Dict[str, Any]): The dictionary to get the value from.
+        keys (List[str]): A list of keys to traverse the dictionary.
+
+    Returns:
+        Any: The value at the end of the key traversal.
+    """
+    for key in keys:
+        d = d[key]
+    return d
+
+def nested_set(
+    d: Dict[str, Any],
+    keys: List[str],
+    value: Any,
+    idx: Optional[int] = None
+) -> None:
+    """Set a value in a nested dictionary using a list of keys.
+    Based on:
+    https://stackoverflow.com/questions/14692690/access-nested-dictionary-items-via-a-list-of-keys
+
+    Args:
+        dic (Dict[str, Any]): The dictionary to set the value in.
+        keys (List[str]): A list of keys to traverse the dictionary.
+        value (Any): The value to set.
+        idx (Optional[int], optional): If the value is an list, the index to change.
+            Defaults to None.
+    """
+    d_in = d.copy()
+
+    for key in keys[:-1]:
+        d = d.setdefault(key, {})
+    if idx is None:
+        # Parameter is a scalar, set directly
+        d[keys[-1]] = value
+    else:
+        # Parameter is a list, need to first get the list, change the values at idx
+
+        # # Get the underlying list
+        par_list = nested_get(d_in, keys)
+        par_list[idx] = value
+        d[keys[-1]] = par_list
+
+def print_nested_dict(dictionary: Dict[str, Any], indent: int = 0) -> None:
+    """Print a nested dictionary with indentation.
+
+    Args:
+        dictionary (Dict[str, Any]): The dictionary to print.
+        indent (int, optional): The number of spaces to indent. Defaults to 0.
+    """
+    for key, value in dictionary.items():
+        print(" " * indent + str(key))
+        if isinstance(value, dict):
+            print_nested_dict(value, indent + 4)
+        else:
+            print(" " * (indent + 4) + str(value))
```

### Comparing `FLORIS-3.6/pyproject.toml` & `FLORIS-4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -112,28 +112,26 @@
 ]
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.per-file-ignores]
 # F841 unused-variable: ignore since this file uses numexpr and many variables look unused
-"floris/simulation/wake_deflection/jimenez.py" = ["F841"]
-"floris/simulation/wake_turbulence/crespo_hernandez.py" = ["F841"]
-"floris/simulation/wake_deflection/gauss.py" = ["F841"]
-"floris/simulation/wake_velocity/jensen.py" = ["F841"]
-"floris/simulation/wake_velocity/gauss.py" = ["F841"]
-"floris/simulation/wake_velocity/empirical_gauss.py" = ["F841"]
+"floris/core/wake_deflection/jimenez.py" = ["F841"]
+"floris/core/wake_turbulence/crespo_hernandez.py" = ["F841"]
+"floris/core/wake_deflection/gauss.py" = ["F841"]
+"floris/core/wake_velocity/jensen.py" = ["F841"]
+"floris/core/wake_velocity/gauss.py" = ["F841"]
+"floris/core/wake_velocity/empirical_gauss.py" = ["F841"]
+# Ignore `F401` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
+"__init__.py" = ["F401"]
 
 # I001 unsorted-imports: ignore because the import order is meaningful to navigate
 # import dependencies
-"floris/simulation/__init__.py" = ["I001"]
-
-# FIXME
-"floris/tools/interface_utilities.py" = ["F821"]
-"floris/tools/wind_rose.py" = ["F821"]
+"floris/core/__init__.py" = ["I001"]
 
 [tool.ruff.isort]
 combine-as-imports = true
 known-first-party = ["floris"]
 order-by-type = false
 # lines-after-imports = 2
```

### Comparing `FLORIS-3.6/setup.py` & `FLORIS-4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-# Copyright 2021 NREL
-
-# Licensed under the Apache License, Version 2.0 (the "License"); you may not
-# use this file except in compliance with the License. You may obtain a copy of
-# the License at http://www.apache.org/licenses/LICENSE-2.0
-
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations under
-# the License.
-
-# See https://floris.readthedocs.io for documentation
-
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
 # Package meta-data.
@@ -38,15 +24,14 @@
     # tools
     "matplotlib~=3.0",
     "pandas~=2.0",
     "shapely~=2.0",
 
     # utilities
     "coloredlogs~=10.0",
-    "flatten_dict~=0.0",
 ]
 
 # What packages are optional?
 # To use:
 #   pip install -e ".[docs,develop]"    install both sets of extras in editable install
 #   pip install -e ".[develop]"         installs only developer packages in editable install
 #   pip install "floris[develop]"       installs developer packages in non-editable install
@@ -78,24 +63,24 @@
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     package_data={
-        'floris': ['turbine_library/*.yaml', 'simulation/wake_velocity/turbopark_lookup_table.mat']
+        'floris': ['turbine_library/*.yaml', 'core/wake_velocity/turbopark_lookup_table.mat']
     },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license="Apache-2.0",
+    license_files = ('LICENSE.txt',),
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: BSD License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy"
```

