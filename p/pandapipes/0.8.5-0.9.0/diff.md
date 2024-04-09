# Comparing `tmp/pandapipes-0.8.5.zip` & `tmp/pandapipes-0.9.0.zip`

## zipinfo {}

```diff
@@ -1,474 +1,500 @@
-Zip file size: 1450360 bytes, number of entries: 472
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/
--rw-r--r--  2.0 unx      109 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/setup.cfg
--rw-r--r--  2.0 unx     3036 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/README.rst
--rw-r--r--  2.0 unx    16876 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/PKG-INFO
--rw-r--r--  2.0 unx      159 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/MANIFEST.in
--rw-r--r--  2.0 unx     1676 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/LICENSE
--rw-r--r--  2.0 unx      618 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/AUTHORS
--rw-r--r--  2.0 unx     2338 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/setup.py
--rw-r--r--  2.0 unx    12702 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/CHANGELOG.rst
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/
--rw-r--r--  2.0 unx     4700 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/run_tests_develop.yml
--rw-r--r--  2.0 unx     3315 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/release.yml
--rw-r--r--  2.0 unx     3404 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/.github/workflows/run_tests_master.yml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/
--rw-r--r--  2.0 unx    87241 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/create.py
--rw-r--r--  2.0 unx    28258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/toolbox.py
--rw-r--r--  2.0 unx    15103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pipeflow.py
--rw-r--r--  2.0 unx      928 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/idx_node.py
--rw-r--r--  2.0 unx     3231 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pandapipes_net.py
--rw-r--r--  2.0 unx      745 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/__init__.py
--rw-r--r--  2.0 unx     1894 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/idx_branch.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/constants.py
--rw-r--r--  2.0 unx     1690 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/run_control.py
--rw-r--r--  2.0 unx      320 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/control/__init__.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/__init__.py
--rw-r--r--  2.0 unx     5243 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/
--rw-r--r--  2.0 unx     2477 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py
--rw-r--r--  2.0 unx     6379 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py
--rw-r--r--  2.0 unx     4518 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/valve_component.py
--rw-r--r--  2.0 unx     4857 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py
--rw-r--r--  2.0 unx      740 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/source_component.py
--rw-r--r--  2.0 unx     8723 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pump_component.py
--rw-r--r--  2.0 unx     4385 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py
--rw-r--r--  2.0 unx     5596 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/junction_component.py
--rw-r--r--  2.0 unx     6978 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py
--rw-r--r--  2.0 unx    16471 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/pipe_component.py
--rw-r--r--  2.0 unx     1665 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py
--rw-r--r--  2.0 unx     5428 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py
--rw-r--r--  2.0 unx     2110 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/__init__.py
--rw-r--r--  2.0 unx      735 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/sink_component.py
--rw-r--r--  2.0 unx     2416 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/compressor_component.py
--rw-r--r--  2.0 unx     5300 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py
--rw-r--r--  2.0 unx     5808 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_models.py
--rw-r--r--  2.0 unx     1976 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
--rw-r--r--  2.0 unx     1949 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py
--rw-r--r--  2.0 unx     3707 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
--rw-r--r--  2.0 unx     8489 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py
--rw-r--r--  2.0 unx     5328 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/circulation_pump.py
--rw-r--r--  2.0 unx     3722 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py
--rw-r--r--  2.0 unx      575 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/
--rw-r--r--  2.0 unx     3295 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/multinet.py
--rw-r--r--  2.0 unx      567 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/__init__.py
--rw-r--r--  2.0 unx     2913 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/create_multinet.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/
--rw-r--r--  2.0 unx      311 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/__init__.py
--rw-r--r--  2.0 unx    13431 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py
--rw-r--r--  2.0 unx    30354 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py
--rw-r--r--  2.0 unx      297 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/control/controller/__init__.py
--rw-r--r--  2.0 unx     6314 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/multinet/timeseries/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/
--rw-r--r--  2.0 unx      344 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/
--rw-r--r--  2.0 unx     6108 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py
--rw-r--r--  2.0 unx     9988 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py
--rw-r--r--  2.0 unx      366 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/__init__.py
--rw-r--r--  2.0 unx    21992 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py
--rw-r--r--  2.0 unx    56282 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py
--rw-r--r--  2.0 unx     4068 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
--rw-r--r--  2.0 unx     5066 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
--rw-r--r--  2.0 unx     9385 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
--rw-r--r--  2.0 unx      369 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/__init__.py
--rw-r--r--  2.0 unx     6384 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/file_io.py
--rw-r--r--  2.0 unx     3069 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/convert_format.py
--rw-r--r--  2.0 unx     4881 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/io_utils.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/io/__init__.py
--rw-r--r--  2.0 unx     6682 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py
--rw-r--r--  2.0 unx    12526 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/result_extraction.py
--rw-r--r--  2.0 unx     8666 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py
--rw-r--r--  2.0 unx    29751 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py
--rw-r--r--  2.0 unx      403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/__init__.py
--rw-r--r--  2.0 unx     5374 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py
--rw-r--r--  2.0 unx     8103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py
--rw-r--r--  2.0 unx     8985 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py
--rw-r--r--  2.0 unx     3255 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/graph_searches.py
--rw-r--r--  2.0 unx      450 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/__init__.py
--rw-r--r--  2.0 unx     9234 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/topology/create_graph.py
--rw-r--r--  2.0 unx     1391 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py
--rw-r--r--  2.0 unx     2753 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/geo.py
--rw-r--r--  2.0 unx     4867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py
--rw-r--r--  2.0 unx    19547 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/simple_plot.py
--rw-r--r--  2.0 unx    10253 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/patch_makers.py
--rw-r--r--  2.0 unx    31552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/collections.py
--rw-r--r--  2.0 unx     1026 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/__init__.py
--rw-r--r--  2.0 unx     2503 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/
--rw-r--r--  2.0 unx     5775 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py
--rw-r--r--  2.0 unx      308 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/__init__.py
--rw-r--r--  2.0 unx    26389 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/fluids.py
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/higher_heating_value.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/compressibility.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/molar_mass.txt
--rw-r--r--  2.0 unx      175 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/density.txt
--rw-r--r--  2.0 unx      180 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/heat_capacity.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/der_compressibility.txt
--rw-r--r--  2.0 unx      174 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/viscosity.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/methane/lower_heating_value.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/molar_mass.txt
--rw-r--r--  2.0 unx       79 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/density.txt
--rw-r--r--  2.0 unx      103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/heat_capacity.txt
--rw-r--r--  2.0 unx      103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/carbondioxide/viscosity.txt
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/higher_heating_value.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/compressibility.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/molar_mass.txt
--rw-r--r--  2.0 unx      244 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/density.txt
--rw-r--r--  2.0 unx      241 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/heat_capacity.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/der_compressibility.txt
--rw-r--r--  2.0 unx      271 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/viscosity.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/lgas/lower_heating_value.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/molar_mass.txt
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/density.txt
--rw-r--r--  2.0 unx      119 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/heat_capacity.txt
--rw-r--r--  2.0 unx      116 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/ethane/viscosity.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/compressibility.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/molar_mass.txt
--rw-r--r--  2.0 unx      266 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/density.txt
--rw-r--r--  2.0 unx      301 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/heat_capacity.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/der_compressibility.txt
--rw-r--r--  2.0 unx      326 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/air/viscosity.txt
--rw-r--r--  2.0 unx        3 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/compressibility.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/molar_mass.txt
--rw-r--r--  2.0 unx      216 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/density.txt
--rw-r--r--  2.0 unx      111 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/heat_capacity.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/der_compressibility.txt
--rw-r--r--  2.0 unx      261 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/water/viscosity.txt
--rw-r--r--  2.0 unx       35 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/molar_mass.txt
--rw-r--r--  2.0 unx     1495 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt
--rw-r--r--  2.0 unx     1456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt
--rw-r--r--  2.0 unx     1629 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt
--rw-r--r--  2.0 unx       65 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/higher_heating_value.txt
--rw-r--r--  2.0 unx       54 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/compressibility.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/molar_mass.txt
--rw-r--r--  2.0 unx      243 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/density.txt
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/heat_capacity.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/der_compressibility.txt
--rw-r--r--  2.0 unx      267 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/viscosity.txt
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hgas/lower_heating_value.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/molar_mass.txt
--rw-r--r--  2.0 unx     1552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt
--rw-r--r--  2.0 unx     1454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt
--rw-r--r--  2.0 unx     1630 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt
--rw-r--r--  2.0 unx       84 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/higher_heating_value.txt
--rw-r--r--  2.0 unx      384 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/compressibility.txt
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/molar_mass.txt
--rw-r--r--  2.0 unx     1552 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt
--rw-r--r--  2.0 unx     1392 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt
--rw-r--r--  2.0 unx      496 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/der_compressibility.txt
--rw-r--r--  2.0 unx     1723 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt
--rw-r--r--  2.0 unx       83 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/properties/hydrogen/lower_heating_value.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/
--rw-r--r--  2.0 unx     8846 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/std_types.py
--rw-r--r--  2.0 unx    10196 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/std_type_class.py
--rw-r--r--  2.0 unx      360 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/
--rw-r--r--  2.0 unx     8971 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv
--rw-r--r--  2.0 unx       51 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P3.csv
--rw-r--r--  2.0 unx       45 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P1.csv
--rw-r--r--  2.0 unx       58 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/std_types/library/Pump/P2.csv
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/
--rw-r--r--  2.0 unx      744 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/test_imports.py
--rw-r--r--  2.0 unx     4258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/run_tests.py
--rw-r--r--  2.0 unx    14678 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/test_toolbox.py
--rw-r--r--  2.0 unx      541 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/
--rw-r--r--  2.0 unx     3987 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
--rw-r--r--  2.0 unx    24386 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py
--rw-r--r--  2.0 unx    15454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
--rw-r--r--  2.0 unx     2493 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py
--rw-r--r--  2.0 unx      346 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/__init__.py
--rw-r--r--  2.0 unx     1271 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py
--rw-r--r--  2.0 unx     7253 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/
--rw-r--r--  2.0 unx      325 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/hydraulics.csv
--rw-r--r--  2.0 unx      152 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_valve.csv
--rw-r--r--  2.0 unx      196 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
--rw-r--r--  2.0 unx       71 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pump.csv
--rw-r--r--  2.0 unx      332 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
--rw-r--r--  2.0 unx     3427 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
--rw-r--r--  2.0 unx      300 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
--rw-r--r--  2.0 unx     1178 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
--rw-r--r--  2.0 unx       57 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
--rw-r--r--  2.0 unx      266 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
--rw-r--r--  2.0 unx      182 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
--rw-r--r--  2.0 unx     1893 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
--rw-r--r--  2.0 unx      133 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
--rw-r--r--  2.0 unx      127 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
--rw-r--r--  2.0 unx       56 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
--rw-r--r--  2.0 unx     3431 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     1181 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     1171 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
--rw-r--r--  2.0 unx     5381 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
--rw-r--r--  2.0 unx     5944 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
--rw-r--r--  2.0 unx     5737 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
--rw-r--r--  2.0 unx     4901 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
--rw-r--r--  2.0 unx     6176 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py
--rw-r--r--  2.0 unx    16572 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py
--rw-r--r--  2.0 unx      238 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/multinet/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/__init__.py
--rw-r--r--  2.0 unx     3518 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py
--rw-r--r--  2.0 unx   592867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
--rw-r--r--  2.0 unx   899403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
--rw-r--r--  2.0 unx   618341 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
--rw-r--r--  2.0 unx   618340 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/__init__.py
--rw-r--r--  2.0 unx     6422 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/io/test_file_io.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/
--rw-r--r--  2.0 unx      688 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py
--rw-r--r--  2.0 unx     3814 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py
--rw-r--r--  2.0 unx    36831 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_create.py
--rw-r--r--  2.0 unx    12568 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_std_types.py
--rw-r--r--  2.0 unx     2507 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/__init__.py
--rw-r--r--  2.0 unx     4584 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py
--rw-r--r--  2.0 unx      721 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_time_series.py
--rw-r--r--  2.0 unx    18462 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py
--rw-r--r--  2.0 unx     1548 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py
--rw-r--r--  2.0 unx     3152 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py
--rw-r--r--  2.0 unx     3615 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py
--rw-r--r--  2.0 unx    10376 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py
--rw-r--r--  2.0 unx     2966 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py
--rw-r--r--  2.0 unx     3898 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/__init__.py
--rw-r--r--  2.0 unx     1099 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py
--rw-r--r--  2.0 unx     2469 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py
--rw-r--r--  2.0 unx     2565 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py
--rw-r--r--  2.0 unx    23456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_water.json
--rw-r--r--  2.0 unx    23709 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json
--rw-r--r--  2.0 unx    34898 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json
--rw-r--r--  2.0 unx    24263 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_gas.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json
--rw-r--r--  2.0 unx    37279 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json
--rw-r--r--  2.0 unx    23570 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json
--rw-r--r--  2.0 unx    23456 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json
--rw-r--r--  2.0 unx    31791 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json
--rw-r--r--  2.0 unx    23777 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json
--rw-r--r--  2.0 unx    23578 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json
--rw-r--r--  2.0 unx    37548 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
--rw-r--r--  2.0 unx      123 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
--rw-r--r--  2.0 unx    12229 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
--rw-r--r--  2.0 unx    11348 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
--rw-r--r--  2.0 unx     4103 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/__init__.py
--rw-r--r--  2.0 unx     7984 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py
--rw-r--r--  2.0 unx     1460 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py
--rw-r--r--  2.0 unx     1987 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/__init__.py
--rw-r--r--  2.0 unx     9471 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py
--rw-r--r--  2.0 unx     2564 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py
--rw-r--r--  2.0 unx    19769 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/properties/__init__.py
--rw-r--r--  2.0 unx    11373 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py
--rw-r--r--  2.0 unx    11177 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py
--rw-r--r--  2.0 unx     6912 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/stanet_comparison/__init__.py
--rw-r--r--  2.0 unx      983 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/test_networks.py
--rw-r--r--  2.0 unx      264 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/test/networks/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/
--rw-r--r--  2.0 unx     2180 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/nw_aux.py
--rw-r--r--  2.0 unx    19224 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py
--rw-r--r--  2.0 unx     3330 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py
--rw-r--r--  2.0 unx      439 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/__init__.py
--rw-r--r--  2.0 unx    10258 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/
--rw-r--r--  2.0 unx   909128 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
--rw-r--r--  2.0 unx    82067 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
--rw-r--r--  2.0 unx    60010 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
--rw-r--r--  2.0 unx   122940 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
--rw-r--r--  2.0 unx    87743 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
--rw-r--r--  2.0 unx   114320 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
--rw-r--r--  2.0 unx    74935 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
--rw-r--r--  2.0 unx    93171 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
--rw-r--r--  2.0 unx   135170 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
--rw-r--r--  2.0 unx    83798 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
--rw-r--r--  2.0 unx    64695 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
--rw-r--r--  2.0 unx    68396 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
--rw-r--r--  2.0 unx    93714 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
--rw-r--r--  2.0 unx    56039 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
--rw-r--r--  2.0 unx    56037 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
--rw-r--r--  2.0 unx    56989 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
--rw-r--r--  2.0 unx    57068 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
--rw-r--r--  2.0 unx    57070 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
--rw-r--r--  2.0 unx    61403 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
--rw-r--r--  2.0 unx    56349 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
--rw-r--r--  2.0 unx    56327 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
--rw-r--r--  2.0 unx    58261 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
--rw-r--r--  2.0 unx    56823 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
--rw-r--r--  2.0 unx    58259 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
--rw-r--r--  2.0 unx    56859 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
--rw-r--r--  2.0 unx    57188 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
--rw-r--r--  2.0 unx    56826 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
--rw-r--r--  2.0 unx    56961 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
--rw-r--r--  2.0 unx    56947 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
--rw-r--r--  2.0 unx    55786 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
--rw-r--r--  2.0 unx    55789 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
--rw-r--r--  2.0 unx    55786 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
--rw-r--r--  2.0 unx    55789 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
--rw-r--r--  2.0 unx    55950 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
--rw-r--r--  2.0 unx    55950 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
--rw-r--r--  2.0 unx    56917 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
--rw-r--r--  2.0 unx    57824 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
--rw-r--r--  2.0 unx    57259 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
--rw-r--r--  2.0 unx    57823 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
--rw-r--r--  2.0 unx    61200 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
--rw-r--r--  2.0 unx    59850 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
--rw-r--r--  2.0 unx    61178 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
--rw-r--r--  2.0 unx    59829 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
--rw-r--r--  2.0 unx    56252 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
--rw-r--r--  2.0 unx    56252 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
--rw-r--r--  2.0 unx    58149 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
--rw-r--r--  2.0 unx    58148 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
--rw-r--r--  2.0 unx    56759 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
--rw-r--r--  2.0 unx    57075 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
--rw-r--r--  2.0 unx    56017 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
--rw-r--r--  2.0 unx    56017 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
--rw-r--r--  2.0 unx    55710 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
--rw-r--r--  2.0 unx    55729 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
--rw-r--r--  2.0 unx    55711 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
--rw-r--r--  2.0 unx    55710 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
--rw-r--r--  2.0 unx    55711 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
--rw-r--r--  2.0 unx    55729 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
--rw-r--r--  2.0 unx    56240 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
--rw-r--r--  2.0 unx    56990 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
--rw-r--r--  2.0 unx    55467 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
--rw-r--r--  2.0 unx    56454 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
--rw-r--r--  2.0 unx    56166 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
--rw-r--r--  2.0 unx    56131 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
--rw-r--r--  2.0 unx    55867 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
--rw-r--r--  2.0 unx    57799 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
--rw-r--r--  2.0 unx    57835 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
--rw-r--r--  2.0 unx    56504 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
--rw-r--r--  2.0 unx    56329 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
--rw-r--r--  2.0 unx    55322 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
--rw-r--r--  2.0 unx    64589 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
--rw-r--r--  2.0 unx    56599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
--rw-r--r--  2.0 unx    55598 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
--rw-r--r--  2.0 unx    56141 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
--rw-r--r--  2.0 unx    55689 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
--rw-r--r--  2.0 unx    56878 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
--rw-r--r--  2.0 unx    56034 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
--rw-r--r--  2.0 unx    56506 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
--rw-r--r--  2.0 unx    55367 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
--rw-r--r--  2.0 unx    55223 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
--rw-r--r--  2.0 unx    57679 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
--rw-r--r--  2.0 unx    57834 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
--rw-r--r--  2.0 unx    56504 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
--rw-r--r--  2.0 unx    56328 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
--rw-r--r--  2.0 unx    57684 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
--rw-r--r--  2.0 unx    55322 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
--rw-r--r--  2.0 unx    64589 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
--rw-r--r--  2.0 unx    56599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
--rw-r--r--  2.0 unx    55599 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
--rw-r--r--  2.0 unx    56138 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
--rw-r--r--  2.0 unx    55688 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
--rw-r--r--  2.0 unx    57295 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
--rw-r--r--  2.0 unx    56878 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
--rw-r--r--  2.0 unx    56033 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
--rw-r--r--  2.0 unx    56508 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
--rw-r--r--  2.0 unx    54582 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
--rw-r--r--  2.0 unx    55365 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
--rw-r--r--  2.0 unx    55223 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
--rw-r--r--  2.0 unx    55168 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
--rw-r--r--  2.0 unx    16876 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/top_level.txt
--rw-r--r--  2.0 unx    23750 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      263 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 12:00 pandapipes-0.8.5/pandapipes.egg-info/dependency_links.txt
-472 files, 11631818 bytes uncompressed, 1342604 bytes compressed:  88.5%
+Zip file size: 1482992 bytes, number of entries: 498
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/.github/
+-rw-r--r--  2.0 unx    18582 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/PKG-INFO
+-rw-r--r--  2.0 unx    14504 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/CHANGELOG.rst
+-rw-r--r--  2.0 unx      109 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/setup.cfg
+-rw-r--r--  2.0 unx     2402 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/setup.py
+-rw-r--r--  2.0 unx     1676 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/LICENSE
+-rw-r--r--  2.0 unx       77 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/MANIFEST.in
+-rw-r--r--  2.0 unx     2889 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/README.rst
+-rw-r--r--  2.0 unx      624 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/AUTHORS
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/timeseries/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/topology/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/control/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/
+-rw-r--r--  2.0 unx     1817 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/idx_branch.py
+-rw-r--r--  2.0 unx    26646 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/toolbox.py
+-rw-r--r--  2.0 unx    90149 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/create.py
+-rw-r--r--  2.0 unx     3231 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pandapipes_net.py
+-rw-r--r--  2.0 unx    14958 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pipeflow.py
+-rw-r--r--  2.0 unx     1011 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/constants.py
+-rw-r--r--  2.0 unx      916 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/idx_node.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/__init__.py
+-rw-r--r--  2.0 unx    19547 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/simple_plot.py
+-rw-r--r--  2.0 unx     2753 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/geo.py
+-rw-r--r--  2.0 unx    10253 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/patch_makers.py
+-rw-r--r--  2.0 unx     4705 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/generic_geodata.py
+-rw-r--r--  2.0 unx     2503 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/plotting_toolbox.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/__init__.py
+-rw-r--r--  2.0 unx     1391 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/pipeflow_results.py
+-rw-r--r--  2.0 unx    31552 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/plotting/collections.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/
+-rw-r--r--  2.0 unx    21761 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/preparing_steps.py
+-rw-r--r--  2.0 unx      366 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/__init__.py
+-rw-r--r--  2.0 unx    59568 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/table_creation.py
+-rw-r--r--  2.0 unx     6108 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/data_cleaning.py
+-rw-r--r--  2.0 unx    10401 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/stanet2pandapipes.py
+-rw-r--r--  2.0 unx     4068 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
+-rw-r--r--  2.0 unx      369 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/__init__.py
+-rw-r--r--  2.0 unx     5066 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
+-rw-r--r--  2.0 unx     9385 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/io/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/topology/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/multinet/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/properties/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/
+-rw-r--r--  2.0 unx      744 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/test_imports.py
+-rw-r--r--  2.0 unx    14678 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/test_toolbox.py
+-rw-r--r--  2.0 unx      541 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/__init__.py
+-rw-r--r--  2.0 unx      131 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pytest.ini
+-rw-r--r--  2.0 unx     4258 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/run_tests.py
+-rw-r--r--  2.0 unx     1987 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/test_pipeflow_results.py
+-rw-r--r--  2.0 unx     9471 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/test_collections.py
+-rw-r--r--  2.0 unx     1460 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/test_generic_coordinates.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/__init__.py
+-rw-r--r--  2.0 unx     7984 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/plotting/test_simple_collections.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/
+-rw-r--r--  2.0 unx     3518 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/test_stanet_converter.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/__init__.py
+-rw-r--r--  2.0 unx   899403 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
+-rw-r--r--  2.0 unx   592867 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
+-rw-r--r--  2.0 unx   618340 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
+-rw-r--r--  2.0 unx   618341 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
+-rw-r--r--  2.0 unx     6414 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/io/test_file_io.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/io/__init__.py
+-rw-r--r--  2.0 unx     1265 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/topology/test_nxgraph.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/topology/__init__.py
+-rw-r--r--  2.0 unx      985 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/topology/test_graph_searches.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/
+-rw-r--r--  2.0 unx     4584 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_network_tables.py
+-rw-r--r--  2.0 unx      721 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_time_series.py
+-rw-r--r--  2.0 unx    12568 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_std_types.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/__init__.py
+-rw-r--r--  2.0 unx      688 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_aux_function.py
+-rw-r--r--  2.0 unx    36831 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_create.py
+-rw-r--r--  2.0 unx     3811 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_special_networks.py
+-rw-r--r--  2.0 unx     2507 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_convert_format.py
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_gas.json
+-rw-r--r--  2.0 unx    23456 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.0.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_water.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_gas.json
+-rw-r--r--  2.0 unx    23777 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.5.0.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_water.json
+-rw-r--r--  2.0 unx    34898 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.7.0.json
+-rw-r--r--  2.0 unx    23709 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.4.0.json
+-rw-r--r--  2.0 unx    33347 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.9.0_gas.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_water.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_gas.json
+-rw-r--r--  2.0 unx    23570 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.2.json
+-rw-r--r--  2.0 unx    23456 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.1.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_gas.json
+-rw-r--r--  2.0 unx    23578 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.2.0.json
+-rw-r--r--  2.0 unx    37548 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_water.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_gas.json
+-rw-r--r--  2.0 unx    39080 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.9.0_water.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_water.json
+-rw-r--r--  2.0 unx    24263 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.6.0.json
+-rw-r--r--  2.0 unx    37279 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_water.json
+-rw-r--r--  2.0 unx    31791 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_gas.json
+-rw-r--r--  2.0 unx     1099 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_mass_storage.py
+-rw-r--r--  2.0 unx     2966 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pressure_control.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_compressor.py
+-rw-r--r--  2.0 unx    10376 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pump.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/__init__.py
+-rw-r--r--  2.0 unx     1548 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_heat_exchanger.py
+-rw-r--r--  2.0 unx     2469 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_mass.py
+-rw-r--r--  2.0 unx     3152 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_valve.py
+-rw-r--r--  2.0 unx    18462 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_ext_grid.py
+-rw-r--r--  2.0 unx     3615 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_flow_control.py
+-rw-r--r--  2.0 unx     3898 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pipe_results.py
+-rw-r--r--  2.0 unx     2565 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_pressure.py
+-rw-r--r--  2.0 unx      123 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
+-rw-r--r--  2.0 unx       92 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
+-rw-r--r--  2.0 unx    10784 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_network.py
+-rw-r--r--  2.0 unx     6176 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/multinet/test_time_series_multinet.py
+-rw-r--r--  2.0 unx    16572 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/multinet/test_control_multinet.py
+-rw-r--r--  2.0 unx      238 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/multinet/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/
+-rw-r--r--  2.0 unx     7253 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_time_series.py
+-rw-r--r--  2.0 unx     3994 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
+-rw-r--r--  2.0 unx    29309 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_inservice.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/__init__.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_options.py
+-rw-r--r--  2.0 unx     1416 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_non_convergence.py
+-rw-r--r--  2.0 unx     1271 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_update_matrix.py
+-rw-r--r--  2.0 unx    15454 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/
+-rw-r--r--  2.0 unx      152 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_valve.csv
+-rw-r--r--  2.0 unx      325 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
+-rw-r--r--  2.0 unx     3427 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
+-rw-r--r--  2.0 unx      196 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
+-rw-r--r--  2.0 unx       57 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
+-rw-r--r--  2.0 unx       11 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
+-rw-r--r--  2.0 unx       56 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
+-rw-r--r--  2.0 unx     1893 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
+-rw-r--r--  2.0 unx      332 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
+-rw-r--r--  2.0 unx      133 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
+-rw-r--r--  2.0 unx       71 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_pump.csv
+-rw-r--r--  2.0 unx       93 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
+-rw-r--r--  2.0 unx      300 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
+-rw-r--r--  2.0 unx     1178 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
+-rw-r--r--  2.0 unx       22 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/hydraulics.csv
+-rw-r--r--  2.0 unx      127 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
+-rw-r--r--  2.0 unx      182 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
+-rw-r--r--  2.0 unx      266 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
+-rw-r--r--  2.0 unx     1171 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx     4901 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
+-rw-r--r--  2.0 unx     5737 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
+-rw-r--r--  2.0 unx     5381 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
+-rw-r--r--  2.0 unx     5944 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
+-rw-r--r--  2.0 unx     3431 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx     1181 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/properties/__init__.py
+-rw-r--r--  2.0 unx     2564 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/properties/test_fluid_specials.py
+-rw-r--r--  2.0 unx    19769 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/properties/test_properties_toolbox.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/__init__.py
+-rw-r--r--  2.0 unx     6912 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
+-rw-r--r--  2.0 unx    11373 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_water_stanet.py
+-rw-r--r--  2.0 unx    11177 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_gas_stanet.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/networks/__init__.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/networks/test_networks.py
+-rw-r--r--  2.0 unx    12229 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
+-rw-r--r--  2.0 unx     4103 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
+-rw-r--r--  2.0 unx      264 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/__init__.py
+-rw-r--r--  2.0 unx    11348 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
+-rw-r--r--  2.0 unx      406 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/timeseries/__init__.py
+-rw-r--r--  2.0 unx     5205 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/timeseries/run_time_series.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/io/__init__.py
+-rw-r--r--  2.0 unx     4881 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/io/io_utils.py
+-rw-r--r--  2.0 unx     3069 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/io/convert_format.py
+-rw-r--r--  2.0 unx     6333 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/io/file_io.py
+-rw-r--r--  2.0 unx     3255 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/topology/graph_searches.py
+-rw-r--r--  2.0 unx      450 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/topology/__init__.py
+-rw-r--r--  2.0 unx     9237 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/topology/create_graph.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/timeseries/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/
+-rw-r--r--  2.0 unx     2874 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/create_multinet.py
+-rw-r--r--  2.0 unx     3295 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/multinet.py
+-rw-r--r--  2.0 unx      567 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/__init__.py
+-rw-r--r--  2.0 unx      318 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/timeseries/__init__.py
+-rw-r--r--  2.0 unx     6320 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/timeseries/run_time_series_multinet.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/controller/
+-rw-r--r--  2.0 unx      311 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/__init__.py
+-rw-r--r--  2.0 unx    13431 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/run_control_multinet.py
+-rw-r--r--  2.0 unx      297 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/controller/__init__.py
+-rw-r--r--  2.0 unx    30354 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/multinet/control/controller/multinet_control.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/
+-rw-r--r--  2.0 unx     1665 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/mass_storage_component.py
+-rw-r--r--  2.0 unx     4434 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/heat_exchanger_component.py
+-rw-r--r--  2.0 unx     9300 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/pump_component.py
+-rw-r--r--  2.0 unx     3284 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/compressor_component.py
+-rw-r--r--  2.0 unx     3634 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/valve_component.py
+-rw-r--r--  2.0 unx     4263 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/ext_grid_component.py
+-rw-r--r--  2.0 unx     8820 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/component_toolbox.py
+-rw-r--r--  2.0 unx     5940 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/pressure_control_component.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/__init__.py
+-rw-r--r--  2.0 unx      740 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/source_component.py
+-rw-r--r--  2.0 unx      735 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/sink_component.py
+-rw-r--r--  2.0 unx    16326 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/pipe_component.py
+-rw-r--r--  2.0 unx     5973 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/junction_component.py
+-rw-r--r--  2.0 unx     2381 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_mass_component.py
+-rw-r--r--  2.0 unx     2013 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_pressure_component.py
+-rw-r--r--  2.0 unx     5180 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/flow_control_component.py
+-rw-r--r--  2.0 unx     1918 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_models.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
+-rw-r--r--  2.0 unx     1404 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_element_models.py
+-rw-r--r--  2.0 unx     3594 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
+-rw-r--r--  2.0 unx     4930 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/base_component.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/__init__.py
+-rw-r--r--  2.0 unx     8409 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_w_internals_models.py
+-rw-r--r--  2.0 unx     3126 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_models.py
+-rw-r--r--  2.0 unx     3619 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/const_flow_models.py
+-rw-r--r--  2.0 unx     5088 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/circulation_pump.py
+-rw-r--r--  2.0 unx     1690 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/control/run_control.py
+-rw-r--r--  2.0 unx      320 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/control/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/oxygen/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/nitrogen/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/ethane/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/
+-rw-r--r--  2.0 unx     5775 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/properties_toolbox.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/__init__.py
+-rw-r--r--  2.0 unx    26380 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/fluids.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/oxygen/molar_mass.txt
+-rw-r--r--  2.0 unx     1630 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/oxygen/viscosity.txt
+-rw-r--r--  2.0 unx     1552 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/oxygen/density.txt
+-rw-r--r--  2.0 unx     1454 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/oxygen/heat_capacity.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/molar_mass.txt
+-rw-r--r--  2.0 unx        3 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/compressibility.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/der_compressibility.txt
+-rw-r--r--  2.0 unx      261 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/viscosity.txt
+-rw-r--r--  2.0 unx      216 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/density.txt
+-rw-r--r--  2.0 unx      111 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/water/heat_capacity.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/molar_mass.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/compressibility.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/der_compressibility.txt
+-rw-r--r--  2.0 unx      326 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/viscosity.txt
+-rw-r--r--  2.0 unx      266 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/density.txt
+-rw-r--r--  2.0 unx      301 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/air/heat_capacity.txt
+-rw-r--r--  2.0 unx       35 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/nitrogen/molar_mass.txt
+-rw-r--r--  2.0 unx     1629 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/nitrogen/viscosity.txt
+-rw-r--r--  2.0 unx     1495 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/nitrogen/density.txt
+-rw-r--r--  2.0 unx     1456 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/nitrogen/heat_capacity.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/molar_mass.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/compressibility.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/der_compressibility.txt
+-rw-r--r--  2.0 unx      267 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/viscosity.txt
+-rw-r--r--  2.0 unx      243 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/density.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/lower_heating_value.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/higher_heating_value.txt
+-rw-r--r--  2.0 unx      238 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hgas/heat_capacity.txt
+-rw-r--r--  2.0 unx       72 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/molar_mass.txt
+-rw-r--r--  2.0 unx      162 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/compressibility.txt
+-rw-r--r--  2.0 unx      133 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/der_compressibility.txt
+-rw-r--r--  2.0 unx     1765 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/viscosity.txt
+-rw-r--r--  2.0 unx     1560 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/density.txt
+-rw-r--r--  2.0 unx      255 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/gas_composition.txt
+-rw-r--r--  2.0 unx      111 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/higher_heating_value.txt
+-rw-r--r--  2.0 unx     1534 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/heat_capacity.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/ethane/molar_mass.txt
+-rw-r--r--  2.0 unx      116 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/ethane/viscosity.txt
+-rw-r--r--  2.0 unx      105 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/ethane/density.txt
+-rw-r--r--  2.0 unx      119 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/ethane/heat_capacity.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/molar_mass.txt
+-rw-r--r--  2.0 unx      384 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/compressibility.txt
+-rw-r--r--  2.0 unx      496 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/der_compressibility.txt
+-rw-r--r--  2.0 unx     1723 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/viscosity.txt
+-rw-r--r--  2.0 unx     1552 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/density.txt
+-rw-r--r--  2.0 unx       83 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/lower_heating_value.txt
+-rw-r--r--  2.0 unx       84 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/higher_heating_value.txt
+-rw-r--r--  2.0 unx     1392 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/hydrogen/heat_capacity.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/molar_mass.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/compressibility.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/der_compressibility.txt
+-rw-r--r--  2.0 unx      271 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/viscosity.txt
+-rw-r--r--  2.0 unx      244 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/density.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/lower_heating_value.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/higher_heating_value.txt
+-rw-r--r--  2.0 unx      241 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/lgas/heat_capacity.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/molar_mass.txt
+-rw-r--r--  2.0 unx       54 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/compressibility.txt
+-rw-r--r--  2.0 unx       47 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/der_compressibility.txt
+-rw-r--r--  2.0 unx      174 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/viscosity.txt
+-rw-r--r--  2.0 unx      175 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/density.txt
+-rw-r--r--  2.0 unx       64 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/lower_heating_value.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/higher_heating_value.txt
+-rw-r--r--  2.0 unx      180 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/methane/heat_capacity.txt
+-rw-r--r--  2.0 unx       65 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/molar_mass.txt
+-rw-r--r--  2.0 unx      162 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/compressibility.txt
+-rw-r--r--  2.0 unx      133 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/der_compressibility.txt
+-rw-r--r--  2.0 unx     1770 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/viscosity.txt
+-rw-r--r--  2.0 unx     1561 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/density.txt
+-rw-r--r--  2.0 unx      226 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/gas_composition.txt
+-rw-r--r--  2.0 unx      110 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/higher_heating_value.txt
+-rw-r--r--  2.0 unx     1533 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/heat_capacity.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/molar_mass.txt
+-rw-r--r--  2.0 unx      103 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/viscosity.txt
+-rw-r--r--  2.0 unx       79 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/density.txt
+-rw-r--r--  2.0 unx      103 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/heat_capacity.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/
+-rw-r--r--  2.0 unx     8846 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/std_types.py
+-rw-r--r--  2.0 unx      360 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/__init__.py
+-rw-r--r--  2.0 unx    10196 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/std_type_class.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/
+-rw-r--r--  2.0 unx     8971 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/Pipe.csv
+-rw-r--r--  2.0 unx       45 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P1.csv
+-rw-r--r--  2.0 unx       58 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P2.csv
+-rw-r--r--  2.0 unx       51 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P3.csv
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/
+-rw-r--r--  2.0 unx     2180 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/nw_aux.py
+-rw-r--r--  2.0 unx    10258 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/simple_gas_networks.py
+-rw-r--r--  2.0 unx      439 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/__init__.py
+-rw-r--r--  2.0 unx     3330 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/simple_heat_transfer_networks.py
+-rw-r--r--  2.0 unx    19224 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/simple_water_networks.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/
+-rw-r--r--  2.0 unx   909128 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
+-rw-r--r--  2.0 unx    56039 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
+-rw-r--r--  2.0 unx    56037 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
+-rw-r--r--  2.0 unx    56989 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
+-rw-r--r--  2.0 unx    56961 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
+-rw-r--r--  2.0 unx    56947 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
+-rw-r--r--  2.0 unx    55786 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
+-rw-r--r--  2.0 unx    55786 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
+-rw-r--r--  2.0 unx    55789 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
+-rw-r--r--  2.0 unx    55789 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
+-rw-r--r--  2.0 unx    57068 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
+-rw-r--r--  2.0 unx    61403 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
+-rw-r--r--  2.0 unx    57070 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
+-rw-r--r--  2.0 unx    56327 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
+-rw-r--r--  2.0 unx    56349 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
+-rw-r--r--  2.0 unx    56859 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
+-rw-r--r--  2.0 unx    56823 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
+-rw-r--r--  2.0 unx    58259 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
+-rw-r--r--  2.0 unx    56826 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
+-rw-r--r--  2.0 unx    57188 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
+-rw-r--r--  2.0 unx    58261 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
+-rw-r--r--  2.0 unx    55950 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
+-rw-r--r--  2.0 unx    55950 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
+-rw-r--r--  2.0 unx    57824 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
+-rw-r--r--  2.0 unx    57823 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
+-rw-r--r--  2.0 unx    57259 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
+-rw-r--r--  2.0 unx    56917 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
+-rw-r--r--  2.0 unx    56017 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
+-rw-r--r--  2.0 unx    56017 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
+-rw-r--r--  2.0 unx    55711 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
+-rw-r--r--  2.0 unx    55710 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
+-rw-r--r--  2.0 unx    55711 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
+-rw-r--r--  2.0 unx    55710 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
+-rw-r--r--  2.0 unx    55729 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
+-rw-r--r--  2.0 unx    55729 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
+-rw-r--r--  2.0 unx    59850 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
+-rw-r--r--  2.0 unx    59829 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
+-rw-r--r--  2.0 unx    61178 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
+-rw-r--r--  2.0 unx    61200 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
+-rw-r--r--  2.0 unx    56252 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
+-rw-r--r--  2.0 unx    56252 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
+-rw-r--r--  2.0 unx    58148 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
+-rw-r--r--  2.0 unx    56759 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
+-rw-r--r--  2.0 unx    57075 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
+-rw-r--r--  2.0 unx    58149 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
+-rw-r--r--  2.0 unx   135170 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
+-rw-r--r--  2.0 unx   122940 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
+-rw-r--r--  2.0 unx    93714 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
+-rw-r--r--  2.0 unx    83798 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
+-rw-r--r--  2.0 unx    93171 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
+-rw-r--r--  2.0 unx    60010 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
+-rw-r--r--  2.0 unx   114320 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
+-rw-r--r--  2.0 unx    74935 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
+-rw-r--r--  2.0 unx    82067 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
+-rw-r--r--  2.0 unx    87743 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
+-rw-r--r--  2.0 unx    64695 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
+-rw-r--r--  2.0 unx    68396 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
+-rw-r--r--  2.0 unx    56454 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
+-rw-r--r--  2.0 unx    56131 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
+-rw-r--r--  2.0 unx    56240 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
+-rw-r--r--  2.0 unx    57799 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
+-rw-r--r--  2.0 unx    56990 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
+-rw-r--r--  2.0 unx    56166 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
+-rw-r--r--  2.0 unx    55867 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
+-rw-r--r--  2.0 unx    55467 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
+-rw-r--r--  2.0 unx    57834 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
+-rw-r--r--  2.0 unx    57684 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
+-rw-r--r--  2.0 unx    56328 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
+-rw-r--r--  2.0 unx    56504 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
+-rw-r--r--  2.0 unx    55322 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
+-rw-r--r--  2.0 unx    57679 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
+-rw-r--r--  2.0 unx    54582 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
+-rw-r--r--  2.0 unx    55365 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
+-rw-r--r--  2.0 unx    55223 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
+-rw-r--r--  2.0 unx    64589 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
+-rw-r--r--  2.0 unx    56599 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
+-rw-r--r--  2.0 unx    56138 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
+-rw-r--r--  2.0 unx    55599 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
+-rw-r--r--  2.0 unx    56878 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
+-rw-r--r--  2.0 unx    57295 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
+-rw-r--r--  2.0 unx    56508 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
+-rw-r--r--  2.0 unx    56033 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
+-rw-r--r--  2.0 unx    55688 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
+-rw-r--r--  2.0 unx    57835 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
+-rw-r--r--  2.0 unx    56329 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
+-rw-r--r--  2.0 unx    56504 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
+-rw-r--r--  2.0 unx    55322 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
+-rw-r--r--  2.0 unx    55367 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
+-rw-r--r--  2.0 unx    55168 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+-rw-r--r--  2.0 unx    55223 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+-rw-r--r--  2.0 unx    64589 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+-rw-r--r--  2.0 unx    56599 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+-rw-r--r--  2.0 unx    56141 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+-rw-r--r--  2.0 unx    55598 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+-rw-r--r--  2.0 unx    56878 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+-rw-r--r--  2.0 unx    56506 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+-rw-r--r--  2.0 unx    56034 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+-rw-r--r--  2.0 unx    55689 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+-rw-r--r--  2.0 unx     9392 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/derivative_calculation.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/__init__.py
+-rw-r--r--  2.0 unx    34186 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/pipeflow_setup.py
+-rw-r--r--  2.0 unx     6802 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox.py
+-rw-r--r--  2.0 unx     5374 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/internals_toolbox.py
+-rw-r--r--  2.0 unx     8985 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/build_system_matrix.py
+-rw-r--r--  2.0 unx     8905 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox_numba.py
+-rw-r--r--  2.0 unx    15666 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes/pf/result_extraction.py
+-rw-r--r--  2.0 unx    18582 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx    26550 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      263 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/requires.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/src/pandapipes.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Dec-22 10:37 pandapipes-0.9.0/.github/workflows/
+-rw-r--r--  2.0 unx     3459 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/.github/workflows/release.yml
+-rw-r--r--  2.0 unx     5186 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/.github/workflows/run_tests_develop.yml
+-rw-r--r--  2.0 unx     3808 b- defN 23-Dec-22 10:37 pandapipes-0.9.0/.github/workflows/run_tests_master.yml
+498 files, 11753282 bytes uncompressed, 1365884 bytes compressed:  88.4%
```

## zipnote {}

```diff
@@ -1,1417 +1,1495 @@
-Filename: pandapipes-0.8.5/
+Filename: pandapipes-0.9.0/
 Comment: 
 
-Filename: pandapipes-0.8.5/.github/
+Filename: pandapipes-0.9.0/src/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/
+Filename: pandapipes-0.9.0/.github/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/
+Filename: pandapipes-0.9.0/PKG-INFO
 Comment: 
 
-Filename: pandapipes-0.8.5/setup.cfg
+Filename: pandapipes-0.9.0/CHANGELOG.rst
 Comment: 
 
-Filename: pandapipes-0.8.5/README.rst
+Filename: pandapipes-0.9.0/setup.cfg
 Comment: 
 
-Filename: pandapipes-0.8.5/PKG-INFO
+Filename: pandapipes-0.9.0/setup.py
 Comment: 
 
-Filename: pandapipes-0.8.5/MANIFEST.in
+Filename: pandapipes-0.9.0/LICENSE
 Comment: 
 
-Filename: pandapipes-0.8.5/LICENSE
+Filename: pandapipes-0.9.0/MANIFEST.in
 Comment: 
 
-Filename: pandapipes-0.8.5/AUTHORS
+Filename: pandapipes-0.9.0/README.rst
 Comment: 
 
-Filename: pandapipes-0.8.5/setup.py
+Filename: pandapipes-0.9.0/AUTHORS
 Comment: 
 
-Filename: pandapipes-0.8.5/CHANGELOG.rst
+Filename: pandapipes-0.9.0/src/pandapipes/
 Comment: 
 
-Filename: pandapipes-0.8.5/.github/workflows/
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/
 Comment: 
 
-Filename: pandapipes-0.8.5/.github/workflows/run_tests_develop.yml
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/
 Comment: 
 
-Filename: pandapipes-0.8.5/.github/workflows/release.yml
+Filename: pandapipes-0.9.0/src/pandapipes/converter/
 Comment: 
 
-Filename: pandapipes-0.8.5/.github/workflows/run_tests_master.yml
+Filename: pandapipes-0.9.0/src/pandapipes/test/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/control/
+Filename: pandapipes-0.9.0/src/pandapipes/timeseries/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/timeseries/
+Filename: pandapipes-0.9.0/src/pandapipes/io/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/
+Filename: pandapipes-0.9.0/src/pandapipes/topology/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/io/
+Filename: pandapipes-0.9.0/src/pandapipes/control/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/topology/
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/
+Filename: pandapipes-0.9.0/src/pandapipes/pf/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/
+Filename: pandapipes-0.9.0/src/pandapipes/idx_branch.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/
+Filename: pandapipes-0.9.0/src/pandapipes/toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/
+Filename: pandapipes-0.9.0/src/pandapipes/create.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/create.py
+Filename: pandapipes-0.9.0/src/pandapipes/pandapipes_net.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/pipeflow.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pipeflow.py
+Filename: pandapipes-0.9.0/src/pandapipes/constants.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/idx_node.py
+Filename: pandapipes-0.9.0/src/pandapipes/idx_node.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pandapipes_net.py
+Filename: pandapipes-0.9.0/src/pandapipes/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/simple_plot.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/idx_branch.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/geo.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/constants.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/patch_makers.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/control/run_control.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/generic_geodata.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/control/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/plotting_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/timeseries/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/pipeflow_results.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/
+Filename: pandapipes-0.9.0/src/pandapipes/plotting/collections.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/valve_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/preparing_steps.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/source_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/table_creation.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/pump_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/data_cleaning.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/stanet2pandapipes.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/junction_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/pipe_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/io/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/sink_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/topology/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/compressor_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/multinet/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/properties/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/circulation_pump.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/test_imports.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/test_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/pytest.ini
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/
+Filename: pandapipes-0.9.0/src/pandapipes/test/run_tests.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/test_pipeflow_results.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/test_collections.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/test_generic_coordinates.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/create_multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/
+Filename: pandapipes-0.9.0/src/pandapipes/test/plotting/test_simple_collections.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/test_stanet_converter.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/control/controller/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/multinet/timeseries/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/
+Filename: pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/io/test_file_io.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/
+Filename: pandapipes-0.9.0/src/pandapipes/test/io/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/topology/test_nxgraph.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/topology/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/topology/test_graph_searches.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_network_tables.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_std_types.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/io/file_io.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/io/convert_format.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_aux_function.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/io/io_utils.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_create.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/io/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_special_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_convert_format.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/result_extraction.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.5.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.7.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/topology/graph_searches.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.4.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/topology/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.9.0_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/topology/create_graph.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/geo.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.2.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.1.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/simple_plot.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/patch_makers.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.2.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/collections.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.9.0_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.6.0.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_water.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/ethane/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_gas.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_mass_storage.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pressure_control.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_compressor.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pump.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_heat_exchanger.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_mass.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_valve.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/fluids.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_ext_grid.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/higher_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_flow_control.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pipe_results.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_pressure.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/api/release_cycle/release_control_test_network.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/multinet/test_time_series_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/methane/lower_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/multinet/test_control_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/multinet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/carbondioxide/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/higher_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_inservice.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_options.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_non_convergence.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_update_matrix.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/lgas/lower_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_valve.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/ethane/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/ethane/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/ethane/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/ethane/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/air/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_pump.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/hydraulics.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/water/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/higher_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hgas/lower_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/properties/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/properties/test_fluid_specials.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/properties/test_properties_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/higher_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/molar_mass.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_water_stanet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_gas_stanet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/networks/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/der_compressibility.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/networks/test_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/properties/hydrogen/lower_heating_value.txt
+Filename: pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/
+Filename: pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/std_types.py
+Filename: pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/std_type_class.py
+Filename: pandapipes-0.9.0/src/pandapipes/timeseries/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/timeseries/run_time_series.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/
+Filename: pandapipes-0.9.0/src/pandapipes/io/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv
+Filename: pandapipes-0.9.0/src/pandapipes/io/io_utils.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P3.csv
+Filename: pandapipes-0.9.0/src/pandapipes/io/convert_format.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P1.csv
+Filename: pandapipes-0.9.0/src/pandapipes/io/file_io.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/std_types/library/Pump/P2.csv
+Filename: pandapipes-0.9.0/src/pandapipes/topology/graph_searches.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/
+Filename: pandapipes-0.9.0/src/pandapipes/topology/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/multinet/
+Filename: pandapipes-0.9.0/src/pandapipes/topology/create_graph.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/timeseries/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/io/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/create_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/properties/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/timeseries/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/timeseries/run_time_series_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/networks/
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/controller/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/test_imports.py
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/run_tests.py
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/run_control_multinet.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/test_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/controller/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/multinet/control/controller/multinet_control.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/mass_storage_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/heat_exchanger_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/pump_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/compressor_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/valve_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/ext_grid_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/component_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/pressure_control_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/source_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/hydraulics.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/sink_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_valve.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/pipe_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/junction_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pump.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_mass_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_pressure_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/flow_control_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_element_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/base_component.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_w_internals_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/const_flow_models.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
+Filename: pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/circulation_pump.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
+Filename: pandapipes-0.9.0/src/pandapipes/control/run_control.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/
+Filename: pandapipes-0.9.0/src/pandapipes/control/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/oxygen/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/nitrogen/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/ethane/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/properties_toolbox.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/multinet/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/fluids.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/oxygen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/oxygen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/oxygen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/oxygen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/io/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/io/test_file_io.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/water/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_create.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_std_types.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/air/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/nitrogen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/nitrogen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_time_series.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/nitrogen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/nitrogen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hgas/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/gas_composition.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_treated/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/ethane/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/ethane/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/ethane/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/ethane/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/hydrogen/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/lgas/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/lower_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/methane/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/properties/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/der_compressibility.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/stanet_comparison/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/networks/test_networks.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/gas_composition.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/test/networks/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/higher_heating_value.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/
+Filename: pandapipes-0.9.0/src/pandapipes/properties/biomethane_pure/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/nw_aux.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/molar_mass.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/viscosity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/density.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/__init__.py
+Filename: pandapipes-0.9.0/src/pandapipes/properties/carbondioxide/heat_capacity.txt
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/std_types.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/std_type_class.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/Pipe.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P1.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P2.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/std_types/library/Pump/P3.csv
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/nw_aux.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/simple_gas_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/__init__.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/simple_heat_transfer_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/simple_water_networks.py
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/top_level.txt
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/requires.txt
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
 Comment: 
 
-Filename: pandapipes-0.8.5/pandapipes.egg-info/dependency_links.txt
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/derivative_calculation.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/__init__.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/pipeflow_setup.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/internals_toolbox.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/build_system_matrix.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox_numba.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes/pf/result_extraction.py
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/PKG-INFO
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/dependency_links.txt
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/SOURCES.txt
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/requires.txt
+Comment: 
+
+Filename: pandapipes-0.9.0/src/pandapipes.egg-info/top_level.txt
+Comment: 
+
+Filename: pandapipes-0.9.0/.github/workflows/
+Comment: 
+
+Filename: pandapipes-0.9.0/.github/workflows/release.yml
+Comment: 
+
+Filename: pandapipes-0.9.0/.github/workflows/run_tests_develop.yml
+Comment: 
+
+Filename: pandapipes-0.9.0/.github/workflows/run_tests_master.yml
 Comment: 
 
 Zip file comment:
```

## Comparing `pandapipes-0.8.5/README.rst` & `pandapipes-0.9.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,14 @@
    :target: https://pypi.python.org/pypi/pandapipes
    :alt: versions
 
 .. image:: https://readthedocs.org/projects/pandapipes/badge/
    :target: http://pandapipes.readthedocs.io/
    :alt: docs
 
-.. image:: https://travis-ci.org/e2nIEE/pandapipes.svg?branch=master
-   :target: https://travis-ci.org/e2nIEE/pandapipes/branches
-   :alt: travis
-
 .. image:: https://codecov.io/gh/e2nIEE/pandapipes/branch/master/graph/badge.svg
    :target: https://codecov.io/github/e2nIEE/pandapipes?branch=master
    :alt: codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/86c876ab23fc40d98e85f7d59bdef928
    :target: https://app.codacy.com/gh/e2nIEE/pandapipes/dashboard
    :alt: Codacy Badge
```

## Comparing `pandapipes-0.8.5/PKG-INFO` & `pandapipes-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandapipes
-Version: 0.8.5
+Version: 0.9.0
 Summary: A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids
 Home-page: http://www.pandapipes.org
 Author: Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse
 Author-email: simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, jolando.kisse@uni-kassel.de
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,17 +12,18 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plotting
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
@@ -42,18 +43,14 @@
    :target: https://pypi.python.org/pypi/pandapipes
    :alt: versions
 
 .. image:: https://readthedocs.org/projects/pandapipes/badge/
    :target: http://pandapipes.readthedocs.io/
    :alt: docs
 
-.. image:: https://travis-ci.org/e2nIEE/pandapipes.svg?branch=master
-   :target: https://travis-ci.org/e2nIEE/pandapipes/branches
-   :alt: travis
-
 .. image:: https://codecov.io/gh/e2nIEE/pandapipes/branch/master/graph/badge.svg
    :target: https://codecov.io/github/e2nIEE/pandapipes?branch=master
    :alt: codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/86c876ab23fc40d98e85f7d59bdef928
    :target: https://app.codacy.com/gh/e2nIEE/pandapipes/dashboard
    :alt: Codacy Badge
@@ -109,14 +106,40 @@
 We welcome contributions to pandapipes of any kind - if you want to contribute, please check out
 the `pandapipes contribution guidelines <https://github.com/e2nIEE/pandapipes/blob/develop/CONTRIBUTING.rst>`_.
 
 
 Change Log
 =============
 
+[0.9.0] - 2023-12-22
+-------------------------------
+
+- [ADDED] multiple creation of heat exchanger
+- [ADDED] support Python 3.11 (now included in test pipeline)
+- [ADDED] after the connectivity check, intercept the pipeflow if no more nodes are in-service (heat and hydraulic)
+- [ADDED] adding biomethane (pure and treated) as additonal fluid
+- [ADDED] result tables can be assembled modularly
+- [CHANGED] dropped support for Python 3.7 (no longer included in test pipeline)
+- [CHANGED] connectivity check now separated by hydraulics and heat_transfer calculation, so that also results can differ in some rows (NaN or not)
+- [CHANGED] dynamic creation of lookups for getting pit as pandas tables
+- [CHANGED] components can have their own internal arrays for specific calculations (e.g. for compressor pressure ratio), so that the pit does not need to include such component specific entries
+- [CHANGED] .readthedocs.yml due to deprecation
+- [CHANGED] changing from setuptools flat-layout into src-layout
+- [CHANGED] calculate thermal derivative globally, adaptions before/after can be done component-wise
+- [CHANGED] moving 'PipeflowNotConverged' error from pipeflow to pipeflow_setup
+- [CHANGED] moving 'result_extraction' under pf folder
+- [FIXED] in STANET converter: bug fix for heat exchanger creation and external temperatures of pipes added
+- [FIXED] build igraph considers all components
+- [FIXED] creating nxgraph and considering pressure circulation pumps correctly
+- [FIXED] error in tutorial 'circular flow in a district heating grid'
+- [FIXED] caused error during 'pip install pandapipes'
+- [REMOVED] broken travis badge removed from readme
+- [REMOVED] branch TINIT removed as it is not a solution variable, temperature determined on the fly
+- [REMOVED] 'converged' setting from options
+
 [0.8.5] - 2023-06-19
 -------------------------------
 - [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
 - [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
 - [FIXED] use igraph package instead of python-igraph (has been renamed)
 - [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
 - [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
```

## Comparing `pandapipes-0.8.5/LICENSE` & `pandapipes-0.9.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 and Energy System Technology (IEE), Kassel, and University of Kassel. Further
 contributions by individual contributors (see AUTHORS file for details). All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted 
 provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions
```

## Comparing `pandapipes-0.8.5/AUTHORS` & `pandapipes-0.9.0/AUTHORS`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 
 Lead Developers:
     - Daniel Lohmeier
-    - Simon Ruben Drauz
+    - Simon Ruben Drauz-Mauel
     - Jolando Marius Kisse
     
 Main Contributors:
     - Tabea Trummel
     - Michel Diesing
     - Vanessa Kiesewetter
```

## Comparing `pandapipes-0.8.5/setup.py` & `pandapipes-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
-from setuptools import find_packages
-from setuptools import setup
 import re
 
+from setuptools import find_namespace_packages
+from setuptools import setup
+
 with open('README.rst', 'rb') as f:
     install = f.read().decode('utf-8')
 
 with open('CHANGELOG.rst', 'rb') as f:
     changelog = f.read().decode('utf-8')
 
 classifiers = [
@@ -30,26 +31,27 @@
     for version in versions:
         classifiers.append('Programming Language :: Python :: %s' % version)
 
 long_description = '\n\n'.join((install, changelog))
 
 setup(
     name='pandapipes',
-    version='0.8.5',
+    version='0.9.0',
     author='Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse',
     author_email='simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, '
                  'jolando.kisse@uni-kassel.de',
     description='A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids',
     long_description=long_description,
-	long_description_content_type='text/x-rst',
+    long_description_content_type='text/x-rst',
     url='http://www.pandapipes.org',
     license='BSD',
-    install_requires=["pandapower>=2.11.1", "matplotlib", "shapely"],
+    install_requires=["pandapower>=2.13.1", "matplotlib", "shapely"],
     extras_require={"docs": ["numpydoc", "sphinx", "sphinx_rtd_theme", "sphinxcontrib.bibtex"],
                     "plotting": ["plotly", "igraph"],
                     "test": ["pytest", "pytest-xdist", "nbmake"],
                     "all": ["numpydoc", "sphinx", "sphinx_rtd_theme", "sphinxcontrib.bibtex",
                             "plotly", "igraph", "pytest", "pytest-xdist", "nbmake"]},
-    packages=find_packages(),
+    packages=find_namespace_packages(where='src'),
+    package_dir={"": "src"},
     include_package_data=True,
     classifiers=classifiers
 )
```

## Comparing `pandapipes-0.8.5/CHANGELOG.rst` & `pandapipes-0.9.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 Change Log
 =============
 
+[0.9.0] - 2023-12-22
+-------------------------------
+
+- [ADDED] multiple creation of heat exchanger
+- [ADDED] support Python 3.11 (now included in test pipeline)
+- [ADDED] after the connectivity check, intercept the pipeflow if no more nodes are in-service (heat and hydraulic)
+- [ADDED] adding biomethane (pure and treated) as additonal fluid
+- [ADDED] result tables can be assembled modularly
+- [CHANGED] dropped support for Python 3.7 (no longer included in test pipeline)
+- [CHANGED] connectivity check now separated by hydraulics and heat_transfer calculation, so that also results can differ in some rows (NaN or not)
+- [CHANGED] dynamic creation of lookups for getting pit as pandas tables
+- [CHANGED] components can have their own internal arrays for specific calculations (e.g. for compressor pressure ratio), so that the pit does not need to include such component specific entries
+- [CHANGED] .readthedocs.yml due to deprecation
+- [CHANGED] changing from setuptools flat-layout into src-layout
+- [CHANGED] calculate thermal derivative globally, adaptions before/after can be done component-wise
+- [CHANGED] moving 'PipeflowNotConverged' error from pipeflow to pipeflow_setup
+- [CHANGED] moving 'result_extraction' under pf folder
+- [FIXED] in STANET converter: bug fix for heat exchanger creation and external temperatures of pipes added
+- [FIXED] build igraph considers all components
+- [FIXED] creating nxgraph and considering pressure circulation pumps correctly
+- [FIXED] error in tutorial 'circular flow in a district heating grid'
+- [FIXED] caused error during 'pip install pandapipes'
+- [REMOVED] broken travis badge removed from readme
+- [REMOVED] branch TINIT removed as it is not a solution variable, temperature determined on the fly
+- [REMOVED] 'converged' setting from options
+
 [0.8.5] - 2023-06-19
 -------------------------------
 - [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
 - [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
 - [FIXED] use igraph package instead of python-igraph (has been renamed)
 - [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
 - [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
```

## Comparing `pandapipes-0.8.5/.github/workflows/run_tests_develop.yml` & `pandapipes-0.9.0/.github/workflows/run_tests_develop.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,116 +10,121 @@
   push:
     branches-ignore: [ master ]
   pull_request:
     branches-ignore: [ master ]
 
 jobs:
   build:
-
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        os:  [ ubuntu-latest, windows-latest ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split
+          if [${{ matrix.python-version != '3.11' }}]; then python -m pip install numba; fi
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@develop#egg=pandapower
-          pip install .
+          python -m pip install .
+        shell: bash
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Test with pytest
         if: ${{ matrix.python-version != '3.9' }}
         run: |
-          pytest
+          python -m pytest
       - name: Test with pytest and Codecov
         if: ${{ matrix.python-version == '3.9' }}
         run: |
           python -m pip install pytest-cov
-          pytest --cov=./ --cov-report=xml
+          python -m pytest --cov=./ --cov-report=xml
       - name: Upload coverage to Codecov
         if: ${{ matrix.python-version == '3.9' }}
         uses: codecov/codecov-action@v1
         with:
           verbose: true
 
   linting:
-
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8']
-
+        python-version: ['3.10']
+        os:  [ ubuntu-latest, windows-latest ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flake8
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@develop#egg=pandapower
-          pip install .
+          python -m pip install .
+        shell: bash
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Lint with flake8 (syntax errors and undefinded names)
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
       - name: Lint with flake8 (all errors/warnings)
         run: |
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
   tutorial_tests:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        os:  [ ubuntu-latest, windows-latest ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest nbmake pytest-xdist pytest-split igraph numba 
+          python -m pip install pytest nbmake pytest-xdist pytest-split igraph
+          if [${{ matrix.python-version != '3.11' }}]; then python -m pip install numba; fi
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@develop#egg=pandapower
-          pip install .
+          python -m pip install .
+        shell: bash
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Test with pytest
         run: |
-          pytest --nbmake -n=auto "./tutorials"
+          python -m pytest --nbmake -n=auto "./tutorials"
 
   docs_check:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.8' ]
+        python-version: [ '3.10' ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Check docs for Python ${{ matrix.python-version }}
         uses: e2nIEE/sphinx-action@master
         with:
           pre-build-command: "apt-get update -y && apt-get install -y git;
                               git --version;
```

## Comparing `pandapipes-0.8.5/.github/workflows/release.yml` & `pandapipes-0.9.0/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -71,32 +71,34 @@
 
   build:
 
     runs-on: ${{ matrix.os }}
     needs: upload
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         os:  [ ubuntu-latest, windows-latest ]
     steps:
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split
+          if [${{ matrix.python-version != '3.11' }}]; then python -m pip install numba; fi
+        shell: bash
       - name: Install pandapipes from TestPyPI
         if: ${{ inputs.upload_server == 'testpypi'}}
         run: |
-          pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple pandapipes
+          python -m pip install --no-cache-dir -i https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple pandapipes
       - name: Install pandapipes from PyPI
         if: ${{ inputs.upload_server == 'pypi'}}
         run: |
-          pip install pandapipes
+          python -m pip install pandapipes
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Test with pytest
         run: |
           pytest --pyargs pandapipes.test
```

## Comparing `pandapipes-0.8.5/.github/workflows/run_tests_master.yml` & `pandapipes-0.9.0/.github/workflows/run_tests_master.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,97 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-# pandapipes-master branch has to work with pandapower-master branch
+# pandapipes-master branch is designed to work with pandapower-master branch
 
 name: ppipes_master
 
 on:
   push:
     branches: [ master ]
   pull_request:
     branches: [ master ]
 
 jobs:
   build:
-
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
-
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        os:  [ ubuntu-latest, windows-latest ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest igraph pytest-split numba
+          python -m pip install pytest igraph pytest-split
+          if [${{ matrix.python-version != '3.11' }}]; then python -m pip install numba; fi
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@master#egg=pandapower;
-          pip install .
+          python -m pip install .
+        shell: bash
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Test with pytest
         if: ${{ matrix.python-version != '3.9' }}
         run: |
-          pytest
+          python -m pytest
       - name: Test with pytest and Codecov
         if: ${{ matrix.python-version == '3.9' }}
         run: |
           python -m pip install pytest-cov
-          pytest --cov=./ --cov-report=xml
+          python -m pytest --cov=./ --cov-report=xml
       - name: Upload coverage to Codecov
         if: ${{ matrix.python-version == '3.9' }}
         uses: codecov/codecov-action@v1
         with:
           verbose: true
 
   tutorial_tests:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
+        os:  [ ubuntu-latest, windows-latest ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install pytest nbmake pytest-xdist pytest-split igraph numba 
+          python -m pip install pytest nbmake pytest-xdist pytest-split igraph
+          if [${{ matrix.python-version != '3.11' }}]; then python -m pip install numba; fi
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
           python -m pip install git+https://github.com/e2nIEE/pandapower@master#egg=pandapower
-          pip install .
+          python -m pip install .
+        shell: bash
       - name: List all installed packages
         run: |
-          pip list
+          python -m pip list
       - name: Test with pytest
         run: |
-          pytest --nbmake -n=auto "./tutorials"
+          python -m pytest --nbmake -n=auto "./tutorials"
 
   docs_check:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.8' ]
+        python-version: [ '3.10' ]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Check docs for Python ${{ matrix.python-version }}
         uses: e2nIEE/sphinx-action@master
         with:
           pre-build-command: "apt-get update -y && apt-get install -y git;
                               git --version;
```

## Comparing `pandapipes-0.8.5/pandapipes/create.py` & `pandapipes-0.9.0/src/pandapipes/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 from pandapower.create import _get_multiple_index_with_check, _get_index_with_check, _set_entries, \
     _check_node_element, _check_multiple_node_elements, _set_multiple_entries, \
@@ -200,14 +200,15 @@
 
     cols = ["name", "junction", "mdot_kg_per_s", "scaling", "in_service", "type"]
     vals = [name, junction, mdot_kg_per_s, scaling, bool(in_service), type]
     _set_entries(net, "source", index, **dict(zip(cols, vals)), **kwargs)
 
     return index
 
+
 def create_mass_storage(net, junction, mdot_kg_per_s, init_m_stored_kg=0, min_m_stored_kg=0.,
                         max_m_stored_kg=np.inf, scaling=1., name=None, index=None,
                         in_service=True, type="mass_storage", **kwargs):
     """
     Adds one storage entry in table net["mass_storage"]. Not suitable for thermal storage tanks.
 
     :param net: The net for which this storage unit should be created
@@ -1498,15 +1499,15 @@
     entries = {"name": name, "from_junction": from_junctions, "to_junction": to_junctions,
                "controlled_junction": controlled_junctions, "controlled_p_bar": controlled_p_bar,
                "control_active": control_active, "loss_coefficient": loss_coefficient,
                "in_service": in_service, "type": type}
     _set_multiple_entries(net, "press_control", index, **entries, **kwargs)
 
     controlled_elsewhere = (controlled_junctions != from_junctions) \
-        & (controlled_junctions != to_junctions)
+                           & (controlled_junctions != to_junctions)
     if np.any(controlled_elsewhere):
         controllers_warn = index[controlled_elsewhere]
         logger.warning("The pressure controllers %s control the pressure at junctions that they are"
                        " not connected to. Please note that this can lead to errors in the pipeflow"
                        " calculation that will not be displayed properly. Make sure that your grid "
                        "configuration is valid." % controllers_warn)
 
@@ -1568,19 +1569,72 @@
                "controlled_mdot_kg_per_s": controlled_mdot_kg_per_s, "diameter_m": diameter_m,
                "control_active": control_active, "in_service": in_service, "type": type}
     _set_multiple_entries(net, "flow_control", index, **entries, **kwargs)
 
     return index
 
 
+def create_heat_exchangers(net, from_junctions, to_junctions, diameter_m, qext_w, loss_coefficient=0,
+                           name=None, index=None, in_service=True, type="heat_exchanger", **kwargs):
+    """
+    Convenience function for creating many heat exchangers at once. Parameters 'from_junctions'\
+    and 'to_junctions' must be arrays of equal length. Other parameters may be either arrays of the\
+    same length or single values.
+
+    :param net: The net for which the heat exchangers should be created
+    :type net: pandapipesNet
+    :param from_junctions: ID of the junctions on one side the heat exchangers will be\
+            connected with
+    :type from_junctions: Iterable(int)
+    :param to_junctions: ID of the junctions on the other side the heat exchangers will be\
+            connected with
+    :type to_junctions: Iterable(int)
+    :param diameter_m: The heat exchangers inner diameter in [m]
+    :type diameter_m: Iterable(float) or float
+    :param qext_w: External heat flux in [W]. If positive, heat is derived from the network. If
+            negative, heat is being fed into the network from a heat source.
+    :type qext_w: Iterable(float) or float
+    :param loss_coefficient: An additional pressure loss coefficient, introduced by e.g. bends
+    :type loss_coefficient: Iterable(float) or float
+    :param name: The name of the heat exchangers
+    :type name: str, default None
+    :param index: Force a specified ID if it is available. If None, the index one higher than the\
+            highest already existing index is selected.
+    :type index: Iterable(str) or str, default None
+    :param in_service: True if the heat exchangers are in service or False if they are out of service
+    :type in_service: Iterable(bool) or bool, default True
+    :param type: Not used yet
+    :type type: Iterable(str) or str, default "heat exchanger"
+    :param kwargs: Additional keyword arguments will be added as further columns to the\
+                    net["heat_exchanger"] table
+    :return: index - The unique IDs of the created heat exchangers
+    :rtype: Iterable(int), default None
+
+    :Example:
+        >>> create_heat_exchangers(net, from_junctions=[0,1], to_junctions=[2,3],
+        >>>                       diameter_m=40e-3, qext_w=2000)
+    """
+    add_new_component(net, HeatExchanger)
+
+    index = _get_multiple_index_with_check(net, "heat_exchanger", index, len(from_junctions))
+    _check_branches(net, from_junctions, to_junctions, "heat_exchanger")
+
+    entries = {"name": name, "from_junction": from_junctions, "to_junction": to_junctions,
+               "diameter_m": diameter_m, "qext_w": qext_w, "loss_coefficient": loss_coefficient,
+               "in_service": bool(in_service), "type": type}
+    _set_multiple_entries(net, "heat_exchanger", index, **entries, **kwargs)
+
+    return index
+
+
 def create_fluid_from_lib(net, name, overwrite=True):
     """
     Creates a fluid from library (if there is an entry) and sets net["fluid"] to this value.
-    Currently, existing fluids in the library are: "hgas", "lgas", "hydrogen", "methane", "water",
-    "air".
+    Currently, existing fluids in the library are: "hgas", "lgas", "hydrogen", "methane", "water","biomethane_pure",
+    "biomethane_treated", "air".
 
     :param net: The net for which this fluid should be created
     :type net: pandapipesNet
     :param name: The name of the fluid that shall be extracted from the fluid lib
     :type name: str
     :param overwrite: Flag if a possibly existing fluid in the net shall be overwritten
     :type overwrite: bool, default True
```

## Comparing `pandapipes-0.8.5/pandapipes/toolbox.py` & `pandapipes-0.9.0/src/pandapipes/toolbox.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import copy
+import os
 from collections.abc import Iterable
 
 import numpy as np
 import pandas as pd
 from networkx import has_path
-from pandapower.auxiliary import get_indices
-from pandapower.toolbox import dataframes_equal, clear_result_tables
+from pandapower import get_indices, dataframes_equal, clear_result_tables
 
 import pandapipes
 from pandapipes.component_models.abstract_models.branch_models import BranchComponent
 from pandapipes.component_models.abstract_models.node_element_models import NodeElementComponent
 from pandapipes.create import create_empty_network
-from pandapipes.idx_branch import TABLE_IDX as TABLE_IDX_BRANCH, ELEMENT_IDX as ELEMENT_IDX_BRANCH, \
-    FROM_NODE as FROM_NODE_BRANCH, TO_NODE as TO_NODE_BRANCH, ACTIVE as ACTIVE_BRANCH, \
-    LENGTH as LENGTH_BRANCH, D as D_BRANCH, AREA as AREA_BRANCH, RHO as RHO_BRANCH, \
-    ETA as ETA_BRANCH, K as K_BRANCH, TINIT as TINIT_BRANCH, VINIT as VINIT_BRANCH, \
-    RE as RE_BRANCH, LAMBDA as LAMBDA_BRANCH, JAC_DERIV_DV as JAC_DERIV_DV_BRANCH, \
-    JAC_DERIV_DP as JAC_DERIV_DP_BRANCH, JAC_DERIV_DP1 as JAC_DERIV_DP1_BRANCH, \
-    LOAD_VEC_BRANCHES as LOAD_VEC_BRANCHES_BRANCH, JAC_DERIV_DV_NODE as JAC_DERIV_DV_NODE_BRANCH, \
-    LOAD_VEC_NODES as LOAD_VEC_NODES_BRANCH, LOSS_COEFFICIENT as LOSS_COEFFICIENT_BRANCH, \
-    CP as CP_BRANCH, ALPHA as ALPHA_BRANCH, JAC_DERIV_DT as JAC_DERIV_DT_BRANCH, \
-    JAC_DERIV_DT1 as JAC_DERIV_DT1_BRANCH, LOAD_VEC_BRANCHES_T as LOAD_VEC_BRANCHES_T_BRANCH, \
-    T_OUT as T_OUT_BRANCH, JAC_DERIV_DT_NODE as JAC_DERIV_DT_NODE_BRANCH, \
-    LOAD_VEC_NODES_T as LOAD_VEC_NODES_T_BRANCH, VINIT_T as VINIT_T_BRANCH, \
-    FROM_NODE_T as FROM_NODE_T_BRANCH, TO_NODE_T as TO_NODE_T_BRANCH, QEXT as QEXT_BRANCH, \
-    TEXT as TEXT_BRANCH, STD_TYPE as STD_TYPE_BRANCH, PL as PL_BRANCH, TL as TL_BRANCH, \
-    BRANCH_TYPE as BRANCH_TYPE_BRANCH, PRESSURE_RATIO as PRESSURE_RATIO_BRANCH, branch_cols
-from pandapipes.idx_node import TABLE_IDX as TABLE_IDX_NODE, ELEMENT_IDX as ELEMENT_IDX_NODE, \
-    NODE_TYPE as NODE_TYPE_NODE, ACTIVE as ACTIVE_NODE, RHO as RHO_NODE, PINIT as PINIT_NODE, \
-    LOAD as LOAD_NODE, HEIGHT as HEIGHT_NODE, TINIT as TINIT_NODE, PAMB as PAMB_NODE, \
-    LOAD_T as LOAD_T_NODE, NODE_TYPE_T as NODE_TYPE_T_NODE, \
-    EXT_GRID_OCCURENCE as EXT_GRID_OCCURENCE_NODE, \
-    EXT_GRID_OCCURENCE_T as EXT_GRID_OCCURENCE_T_NODE, node_cols, \
+from pandapipes.idx_branch import branch_cols
+from pandapipes.idx_node import node_cols, \
     T as TYPE_T, P as TYPE_P, PC as TYPE_PC, NONE as TYPE_NONE, L as TYPE_L
 from pandapipes.pandapipes_net import pandapipesNet
 from pandapipes.topology import create_nxgraph
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
@@ -539,84 +520,56 @@
 #     # drop the trafos
 #     net[table].drop(trafos, inplace=True)
 #     res_trafos = net["res_" + table].index.intersection(trafos)
 #     net["res_" + table].drop(res_trafos, inplace=True)
 #     logger.info("dropped %d %s elements with %d switches" % (len(trafos), table, num_switches))
 
 
-node_pit_indices = {
-    TABLE_IDX_NODE: "TABLE_IDX",
-    ELEMENT_IDX_NODE: "ELEMENT_IDX",
-    NODE_TYPE_NODE: "NODE_TYPE",
-    ACTIVE_NODE: "ACTIVE",
-    RHO_NODE: "RHO",
-    PINIT_NODE: "PINIT",
-    LOAD_NODE: "LOAD",
-    HEIGHT_NODE: "HEIGHT",
-    TINIT_NODE: "TINIT",
-    PAMB_NODE: "PAMB",
-    LOAD_T_NODE: "LOAD_T",
-    NODE_TYPE_T_NODE: "NODE_TYPE_T",
-    EXT_GRID_OCCURENCE_NODE: "EXT_GRID_OCCURENCE",
-    EXT_GRID_OCCURENCE_T_NODE: "EXT_GRID_OCCURENCE_T",
-}
-
-branch_pit_indices = {
-    TABLE_IDX_BRANCH: "TABLE_IDX",
-    ELEMENT_IDX_BRANCH: "ELEMENT_IDX",
-    FROM_NODE_BRANCH: "FROM_NODE",
-    TO_NODE_BRANCH: "TO_NODE",
-    ACTIVE_BRANCH: "ACTIVE",
-    LENGTH_BRANCH: "LENGTH",
-    D_BRANCH: "D",
-    AREA_BRANCH: "AREA",
-    RHO_BRANCH: "RHO",
-    ETA_BRANCH: "ETA",
-    K_BRANCH: "K",
-    TINIT_BRANCH: "TINIT",
-    VINIT_BRANCH: "VINIT",
-    RE_BRANCH: "RE",
-    LAMBDA_BRANCH: "LAMBDA",
-    JAC_DERIV_DV_BRANCH: "JAC_DERIV_DV",
-    JAC_DERIV_DP_BRANCH: "JAC_DERIV_DP",
-    JAC_DERIV_DP1_BRANCH: "JAC_DERIV_DP1",
-    LOAD_VEC_BRANCHES_BRANCH: "LOAD_VEC_BRANCHES",
-    JAC_DERIV_DV_NODE_BRANCH: "JAC_DERIV_DV_NODE",
-    LOAD_VEC_NODES_BRANCH: "LOAD_VEC_NODES",
-    LOSS_COEFFICIENT_BRANCH: "LOSS_COEFFICIENT",
-    CP_BRANCH: "CP",
-    ALPHA_BRANCH: "ALPHA",
-    JAC_DERIV_DT_BRANCH: "JAC_DERIV_DT",
-    JAC_DERIV_DT1_BRANCH: "JAC_DERIV_DT1",
-    LOAD_VEC_BRANCHES_T_BRANCH: "LOAD_VEC_BRANCHES_T",
-    T_OUT_BRANCH: "T_OUT",
-    JAC_DERIV_DT_NODE_BRANCH: "JAC_DERIV_DT_NODE",
-    LOAD_VEC_NODES_T_BRANCH: "LOAD_VEC_NODES_T",
-    VINIT_T_BRANCH: "VINIT_T",
-    FROM_NODE_T_BRANCH: "FROM_NODE_T",
-    TO_NODE_T_BRANCH: "TO_NODE_T",
-    QEXT_BRANCH: "QEXT",
-    TEXT_BRANCH: "TEXT",
-    STD_TYPE_BRANCH: "STD_TYPE",
-    PL_BRANCH: "PL",
-    TL_BRANCH: "TL",
-    BRANCH_TYPE_BRANCH: "BRANCH_TYPE",
-    PRESSURE_RATIO_BRANCH: "PRESSURE_RATIO",
-}
+pit_types = {TYPE_P: "P", TYPE_L: "L", TYPE_NONE: "NONE", TYPE_T: "T", TYPE_PC: "PC", 0: "NONE"}
+int_cols = ["FROM_NODE", "TO_NODE", "ELEMENT_IDX", "EXT_GRID_OCCURENCE", "EXT_GRID_OCCURENCE_T"]
+bool_cols = ["ACTIVE"]
 
 
-pit_types = {TYPE_P: "P", TYPE_L: "L", TYPE_NONE: "NONE", TYPE_T: "T", TYPE_PC: "PC", 0: "NONE"}
+def get_pit_lookup(pit_type="node"):
+    """
+    Retrieve a lookup for "indices" and "types" from the idx_branch or idx_node files.
+
+    :param pit_type: the pit for which the lookup is generated ("branch" or "node")
+    :type pit_type: str, default "node"
+    :return: idx_lookup: dictionary of structure {column: name} derived from idx_node.py or \
+        idx_branch.py to describe the structure of the pit
+    :rtype: dict
+    """
+    idx_lookup = {"indices": dict(), "types": dict()}
+    with open(os.path.join(pandapipes.pp_dir, f"idx_{pit_type}.py")) as f:
+        lookup_type = None
+        for ln in f.readlines():
+            if ln.strip().startswith("#"):
+                if "indices" in ln:
+                    lookup_type = "indices"
+                elif "types" in ln:
+                    lookup_type = "types"
+            if lookup_type is None:
+                continue
+            txt = ln.split("#")[0]
+            if "=" not in txt:
+                continue
+            part1, part2 = txt.split("=")
+            idx_lookup[lookup_type][int(part2.strip())] = part1.strip()
+    return idx_lookup
 
 
-def get_internal_tables_pandas(net):
+def get_internal_tables_pandas(net, convert_types=True):
     """
     Convert the internal structure (pit) for nodes and branches into readable pandas DataFrames.
 
     :param net: pandapipes network
     :type net: pandapipesNet
+    :param convert_types: if True, convert some columns into a more readable form
+    :type convert_types: bool, default True
     :return: node_table, branch_table
     :rtype: pandas.DataFrame
     """
     if "_pit" not in net:
         logger.warning("The net does not contain an internal pandapipes structure. Please try "
                        "running a pipeflow first.")
         return None, None
@@ -629,21 +582,36 @@
     if missing_nodes > 0:
         logger.warning("%d node pit entries are missing. Please verify the correctness of the "
                        "table." % missing_nodes)
     if missing_branches > 0:
         logger.warning("%d branch pit entries are missing. Please verify the correctness of the "
                        "table." % missing_branches)
 
+    node_lookup = get_pit_lookup("node")
+    branch_lookup = get_pit_lookup("branch")
+
     node_table_lookup = pandapipes.get_lookup(net, "node", "table")
     node_table = pd.DataFrame(node_pit)
-    node_table.rename(columns=node_pit_indices, inplace=True)
-    node_table["NODE_TYPE"].replace(pit_types, inplace=True)
-    node_table["NODE_TYPE_T"].replace(pit_types, inplace=True)
-    node_table["TABLE_IDX"].replace(node_table_lookup["n2t"], inplace=True)
+    node_table.rename(columns=node_lookup["indices"], inplace=True)
 
     branch_table_lookup = pandapipes.get_lookup(net, "branch", "table")
     branch_table = pd.DataFrame(branch_pit)
-    branch_table.rename(columns=branch_pit_indices, inplace=True)
-    branch_table["BRANCH_TYPE"].replace(pit_types, inplace=True)
-    branch_table["TABLE_IDX"].replace(branch_table_lookup["n2t"], inplace=True)
+    branch_table.rename(columns=branch_lookup["indices"], inplace=True)
+
+    if convert_types:
+        # TODO: replace types with a version retrieved from get_pit_lookup, but before, the types
+        #       need to be defined properly inside the files!
+        node_table["NODE_TYPE"].replace(pit_types, inplace=True)
+        node_table["NODE_TYPE_T"].replace(pit_types, inplace=True)
+        node_table["TABLE_IDX"].replace(node_table_lookup["n2t"], inplace=True)
+
+        branch_table["BRANCH_TYPE"].replace(pit_types, inplace=True)
+        branch_table["TABLE_IDX"].replace(branch_table_lookup["n2t"], inplace=True)
+
+        for col in int_cols + bool_cols:
+            for tbl in (node_table, branch_table):
+                if col in tbl.columns:
+                    tbl[col] = tbl[col].astype(np.int32)
+                    if col in bool_cols:
+                        tbl[col] = tbl[col].astype(np.bool_)
 
     return node_table, branch_table
```

## Comparing `pandapipes-0.8.5/pandapipes/pipeflow.py` & `pandapipes-0.9.0/src/pandapipes/pipeflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import linalg
-from pandapower.auxiliary import ppException
 from scipy.sparse.linalg import spsolve
 
-from pandapipes.idx_branch import ACTIVE as ACTIVE_BR, FROM_NODE, TO_NODE, FROM_NODE_T, \
-    TO_NODE_T, VINIT, T_OUT, VINIT_T
-from pandapipes.idx_node import PINIT, TINIT, ACTIVE as ACTIVE_ND
+from pandapipes.idx_branch import FROM_NODE, TO_NODE, FROM_NODE_T, TO_NODE_T, VINIT, TOUTINIT, VINIT_T
+from pandapipes.idx_node import PINIT, TINIT
 from pandapipes.pf.build_system_matrix import build_system_matrix
-from pandapipes.pf.derivative_calculation import calculate_derivatives_hydraulic
+from pandapipes.pf.derivative_calculation import calculate_derivatives_hydraulic, calculate_derivatives_thermal
 from pandapipes.pf.pipeflow_setup import get_net_option, get_net_options, set_net_option, \
     init_options, create_internal_results, write_internal_results, get_lookup, create_lookups, \
-    initialize_pit, check_connectivity, reduce_pit, \
-    set_user_pf_options, init_all_result_tables
+    initialize_pit, reduce_pit, set_user_pf_options, init_all_result_tables, \
+    identify_active_nodes_branches, PipeflowNotConverged
 from pandapipes.pf.result_extraction import extract_all_results, extract_results_active_pit
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
@@ -62,58 +60,61 @@
     # Inputs & initialization of variables
     # ------------------------------------------------------------------------------------------
 
     # Init physical constants and options
     init_options(net, local_params)
 
     # init result tables
-    net["converged"] = False
+    net.converged = False
     init_all_result_tables(net)
 
     create_lookups(net)
     node_pit, branch_pit = initialize_pit(net)
-    if (len(node_pit) == 0) & (len(branch_pit) == 0):
-        logger.warning("There are no node and branch entries defined. This might mean that your net"
-                       " is empty")
+    if len(node_pit) == 0:
+        logger.warning("There are no nodes defined. "
+                       "You need at least one node! "
+                       "Without any nodes, you are not able to conduct a pipeflow!")
         return
+
     calculation_mode = get_net_option(net, "mode")
     calculate_hydraulics = calculation_mode in ["hydraulics", "all"]
     calculate_heat = calculation_mode in ["heat", "all"]
 
-    if get_net_option(net, "check_connectivity"):
-        nodes_connected, branches_connected = check_connectivity(
-            net, branch_pit, node_pit, check_heat=calculate_heat)
-    else:
-        nodes_connected = node_pit[:, ACTIVE_ND].astype(np.bool_)
-        branches_connected = branch_pit[:, ACTIVE_BR].astype(np.bool_)
-
-    reduce_pit(net, node_pit, branch_pit, nodes_connected, branches_connected)
-
-    if calculation_mode == "heat" and not net.user_pf_options["hyd_flag"]:
-        raise UserWarning("Converged flag not set. Make sure that hydraulic calculation results "
-                          "are available.")
-    elif calculation_mode == "heat" and net.user_pf_options["hyd_flag"]:
-        net["_active_pit"]["node"][:, PINIT] = sol_vec[:len(node_pit)]
-        net["_active_pit"]["branch"][:, VINIT] = sol_vec[len(node_pit):]
+    # cannot be moved to calculate_hydraulics as the active node/branch hydraulics lookup is also required to
+    # determine the active node/branch heat transfer lookup
+    identify_active_nodes_branches(net, branch_pit, node_pit)
+
+    if calculation_mode == "heat":
+        if not net.user_pf_options["hyd_flag"]:
+            raise UserWarning("Converged flag not set. Make sure that hydraulic calculation "
+                              "results are available.")
+        else:
+            net["_pit"]["node"][:, PINIT] = sol_vec[:len(node_pit)]
+            net["_pit"]["branch"][:, VINIT] = sol_vec[len(node_pit):]
 
     if calculate_hydraulics:
-        converged, _ = hydraulics(net)
-        if not converged:
+        reduce_pit(net, node_pit, branch_pit, mode="hydraulics")
+        hydraulics(net)
+        if not net.converged:
             raise PipeflowNotConverged("The hydraulic calculation did not converge to a solution.")
+        extract_results_active_pit(net, mode="hydraulics")
 
     if calculate_heat:
-        converged, _ = heat_transfer(net)
-        if not converged:
+        node_pit, branch_pit = net["_pit"]["node"], net["_pit"]["branch"]
+        identify_active_nodes_branches(net, branch_pit, node_pit, False)
+        reduce_pit(net, node_pit, branch_pit, mode="heat_transfer")
+        heat_transfer(net)
+        if not net.converged:
             raise PipeflowNotConverged("The heat transfer calculation did not converge to a "
                                        "solution.")
+        extract_results_active_pit(net, mode="heat_transfer")
     elif not calculate_hydraulics:
         raise UserWarning("No proper calculation mode chosen.")
 
-    extract_results_active_pit(net, node_pit, branch_pit, nodes_connected, branches_connected)
-    extract_all_results(net, nodes_connected, branches_connected)
+    extract_all_results(net, calculation_mode)
 
 
 def hydraulics(net):
     max_iter, nonlinear_method, tol_p, tol_v, tol_res = get_net_options(
         net, "iter", "nonlinear_method", "tol_p", "tol_v", "tol_res")
 
     # Start of nonlinear loop
@@ -123,15 +124,15 @@
     if not get_net_option(net, "reuse_internal_data") or "_internal_data" not in net:
         net["_internal_data"] = dict()
 
     # This branch is used to stop the solver after a specified error tolerance is reached
     error_v, error_p, residual_norm = [], [], None
 
     # This loop is left as soon as the solver converged
-    while not get_net_option(net, "converged") and niter <= max_iter:
+    while not net.converged and niter <= max_iter:
         logger.debug("niter %d" % niter)
 
         # solve_hydraulics is where the calculation takes place
         v_init, p_init, v_init_old, p_init_old, epsilon = solve_hydraulics(net)
 
         # Error estimation & convergence plot
         dv_init = np.abs(v_init - v_init_old)
@@ -143,72 +144,64 @@
 
         finalize_iteration(net, niter, error_p, error_v, residual_norm, nonlinear_method, tol_p,
                            tol_v, tol_res, p_init_old, v_init_old)
         niter += 1
     write_internal_results(net, iterations=niter, error_p=error_p[niter - 1],
                            error_v=error_v[niter - 1], residual_norm=residual_norm)
 
-    converged = get_net_option(net, "converged")
-    net['converged'] = converged
-    if converged:
+    if net.converged:
         set_user_pf_options(net, hyd_flag=True)
 
-    log_final_results(net, converged, niter, residual_norm)
+    log_final_results(net, niter, residual_norm)
     if not get_net_option(net, "reuse_internal_data"):
         net.pop("_internal_data", None)
 
-    return converged, niter
-
 
 def heat_transfer(net):
     max_iter, nonlinear_method, tol_t, tol_res = get_net_options(
         net, "iter", "nonlinear_method", "tol_T", "tol_res")
 
     # Start of nonlinear loop
     # ---------------------------------------------------------------------------------------------
 
     if net.fluid.is_gas:
         logger.info("Caution! Temperature calculation does currently not affect hydraulic "
                     "properties!")
 
     error_t, error_t_out, residual_norm = [], [], None
 
-    set_net_option(net, "converged", False)
+    net.converged = False
     niter = 0
 
     # This loop is left as soon as the solver converged
-    while not get_net_option(net, "converged") and niter <= max_iter:
+    while not net.converged and niter <= max_iter:
         logger.debug("niter %d" % niter)
 
         # solve_hydraulics is where the calculation takes place
         t_out, t_out_old, t_init, t_init_old, epsilon = solve_temperature(net)
 
         # Error estimation & convergence plot
         delta_t_init = np.abs(t_init - t_init_old)
         delta_t_out = np.abs(t_out - t_out_old)
 
         residual_norm = (linalg.norm(epsilon) / (len(epsilon)))
         error_t.append(linalg.norm(delta_t_init) / (len(delta_t_init)))
         error_t_out.append(linalg.norm(delta_t_out) / (len(delta_t_out)))
 
         finalize_iteration(net, niter, error_t, error_t_out, residual_norm, nonlinear_method, tol_t,
-                           tol_t, tol_res, t_init_old, t_out_old, hyraulic_mode=True)
+                           tol_t, tol_res, t_init_old, t_out_old, hydraulic_mode=False)
         logger.debug("F: %s" % epsilon.round(4))
         logger.debug("T_init_: %s" % t_init.round(4))
         logger.debug("T_out_: %s" % t_out.round(4))
         niter += 1
 
     write_internal_results(net, iterations_T=niter, error_T=error_t[niter - 1],
                            residual_norm_T=residual_norm)
 
-    converged = get_net_option(net, "converged")
-    net['converged'] = converged
-    log_final_results(net, converged, niter, residual_norm, hyraulic_mode=False)
-
-    return converged, niter
+    log_final_results(net, niter, residual_norm, hyraulic_mode=False)
 
 
 def solve_hydraulics(net):
     """
     Create and solve the linearized system of equations (based on a jacobian in form of a scipy
     sparse matrix and a load vector in form of a numpy array) in order to calculate the hydraulic
     magnitudes (pressure and velocity) for the network nodes and branches.
@@ -218,15 +211,15 @@
     :return:
 
     """
     options = net["_options"]
     branch_pit = net["_active_pit"]["branch"]
     node_pit = net["_active_pit"]["node"]
 
-    branch_lookups = get_lookup(net, "branch", "from_to_active")
+    branch_lookups = get_lookup(net, "branch", "from_to_active_hydraulics")
     for comp in net['component_list']:
         comp.adaption_before_derivatives_hydraulic(
             net, branch_pit, node_pit, branch_lookups, options)
     calculate_derivatives_hydraulic(net, branch_pit, node_pit, options)
     for comp in net['component_list']:
         comp.adaption_after_derivatives_hydraulic(
             net, branch_pit, node_pit, branch_lookups, options)
@@ -254,38 +247,43 @@
     :return: branch_pit
 
     """
 
     options = net["_options"]
     branch_pit = net["_active_pit"]["branch"]
     node_pit = net["_active_pit"]["node"]
-    branch_lookups = get_lookup(net, "branch", "from_to_active")
+    branch_lookups = get_lookup(net, "branch", "from_to_active_heat_transfer")
 
     # Negative velocity values are turned to positive ones (including exchange of from_node and
     # to_node for temperature calculation
     branch_pit[:, VINIT_T] = branch_pit[:, VINIT]
     branch_pit[:, FROM_NODE_T] = branch_pit[:, FROM_NODE]
     branch_pit[:, TO_NODE_T] = branch_pit[:, TO_NODE]
     mask = branch_pit[:, VINIT] < 0
     branch_pit[mask, VINIT_T] = -branch_pit[mask, VINIT]
     branch_pit[mask, FROM_NODE_T] = branch_pit[mask, TO_NODE]
     branch_pit[mask, TO_NODE_T] = branch_pit[mask, FROM_NODE]
 
     for comp in net['component_list']:
-        comp.calculate_derivatives_thermal(net, branch_pit, node_pit, branch_lookups, options)
+        comp.adaption_before_derivatives_thermal(
+            net, branch_pit, node_pit, branch_lookups, options)
+    calculate_derivatives_thermal(net, branch_pit, node_pit, options)
+    for comp in net['component_list']:
+        comp.adaption_after_derivatives_thermal(
+            net, branch_pit, node_pit, branch_lookups, options)
     jacobian, epsilon = build_system_matrix(net, branch_pit, node_pit, True)
 
     t_init_old = node_pit[:, TINIT].copy()
-    t_out_old = branch_pit[:, T_OUT].copy()
+    t_out_old = branch_pit[:, TOUTINIT].copy()
 
     x = spsolve(jacobian, epsilon)
     node_pit[:, TINIT] += x[:len(node_pit)] * options["alpha"]
-    branch_pit[:, T_OUT] += x[len(node_pit):]
+    branch_pit[:, TOUTINIT] += x[len(node_pit):]
 
-    return branch_pit[:, T_OUT], t_out_old, node_pit[:, TINIT], t_init_old, epsilon
+    return branch_pit[:, TOUTINIT], t_out_old, node_pit[:, TINIT], t_init_old, epsilon
 
 
 def set_damping_factor(net, niter, error):
     """
     Set the value of the damping factor (factor for the newton step width) from current results.
 
     :param net: the net for which to perform the pipeflow
@@ -310,16 +308,16 @@
     else:
         set_net_option(net, "alpha", current_alpha * 10 if current_alpha <= 0.1 else 1.0)
 
     return error_x0_increased, error_x1_increased
 
 
 def finalize_iteration(net, niter, error_1, error_2, residual_norm, nonlinear_method, tol_1, tol_2,
-                       tol_res, vals_1_old, vals_2_old, hyraulic_mode=True):
-    col1, col2 = (PINIT, VINIT) if hyraulic_mode else (TINIT, T_OUT)
+                       tol_res, vals_1_old, vals_2_old, hydraulic_mode=True):
+    col1, col2 = (PINIT, VINIT) if hydraulic_mode else (TINIT, TOUTINIT)
 
     # Control of damping factor
     if nonlinear_method == "automatic":
         error_x0_increased, error_x1_increased = set_damping_factor(net, niter,
                                                                     [error_1, error_2])
         if error_x0_increased:
             net["_active_pit"]["node"][:, col1] = vals_1_old
@@ -327,45 +325,38 @@
             net["_active_pit"]["branch"][:, col2] = vals_2_old
     elif nonlinear_method != "constant":
         logger.warning("No proper nonlinear method chosen. Using constant settings.")
 
     # Setting convergence flag
     if error_2[niter] <= tol_2 and error_1[niter] <= tol_1 and residual_norm < tol_res:
         if nonlinear_method != "automatic":
-            set_net_option(net, "converged", True)
+            net.converged = True
         elif get_net_option(net, "alpha") == 1:
-            set_net_option(net, "converged", True)
+            net.converged = True
 
-    if hyraulic_mode:
+    if hydraulic_mode:
         logger.debug("errorv: %s" % error_1[niter])
         logger.debug("errorp: %s" % error_2[niter])
         logger.debug("alpha: %s" % get_net_option(net, "alpha"))
     else:
         logger.debug("errorT: %s" % error_1[niter])
         logger.debug("alpha: %s" % get_net_option(net, "alpha"))
 
 
-def log_final_results(net, converged, niter, residual_norm, hyraulic_mode=True):
+def log_final_results(net, niter, residual_norm, hyraulic_mode=True):
     if hyraulic_mode:
         solver = "hydraulics"
         outputs = ["tol_p", "tol_v"]
     else:
         solver = "heat transfer"
         outputs = ["tol_T"]
     logger.debug("--------------------------------------------------------------------------------")
-    if not converged:
+    if not net.converged:
         logger.debug("Maximum number of iterations reached but %s solver did not converge."
                      % solver)
         logger.debug("Norm of residual: %s" % residual_norm)
     else:
         logger.debug("Calculation completed. Preparing results...")
         logger.debug("Converged after %d iterations." % niter)
         logger.debug("Norm of residual: %s" % residual_norm)
         for out in outputs:
             logger.debug("%s: %s" % (out, get_net_option(net, out)))
-
-
-class PipeflowNotConverged(ppException):
-    """
-    Exception being raised in case pipeflow did not converge.
-    """
-    pass
```

## Comparing `pandapipes-0.8.5/pandapipes/idx_node.py` & `pandapipes-0.9.0/src/pandapipes/idx_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
-# define bus types
+# node types
 P = 1  # Reference node, pressure is fixed
 L = 2  # All other nodes
 T = 10  # Reference node with fixed temperature, otherwise 0
 PC = 20  # Controlled node with fixed pressure p
 NONE = 3  # None
 
-# define the indices
+# node indices
 TABLE_IDX = 0  # number of the table that this node belongs to
 ELEMENT_IDX = 1  # index of the element that this node belongs to (within the given table)
 NODE_TYPE = 2  # junction type
 ACTIVE = 3
 RHO = 4  # Density in [kg/m^3]
 PINIT = 5
 LOAD = 6
```

## Comparing `pandapipes-0.8.5/pandapipes/pandapipes_net.py` & `pandapipes-0.9.0/src/pandapipes/pandapipes_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/__init__.py` & `pandapipes-0.9.0/src/pandapipes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
-__version__ = '0.8.5'
+__version__ = '0.9.0'
 __format_version__ = '0.8.0'
 
 import pandas as pd
 import os
 
 pd.options.mode.chained_assignment = None  # default='warn'
 pp_dir = os.path.dirname(os.path.realpath(__file__))
```

## Comparing `pandapipes-0.8.5/pandapipes/idx_branch.py` & `pandapipes-0.9.0/src/pandapipes/idx_branch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
+# branch types
+# no types defined
+
+# branch indices
 TABLE_IDX = 0  # number of the table that this branch belongs to
 ELEMENT_IDX = 1  # index of the element that this branch belongs to (within the given table)
 FROM_NODE = 2  # f, from bus number
 TO_NODE = 3  # t, to bus number
 ACTIVE = 4
 LENGTH = 5  # Pipe length in [m]
 D = 6  # Diameter in [m]
 AREA = 7  # Area in [m²]
 RHO = 8  # Density in [kg/m^3
 ETA = 9  # Dynamic viscosity in [Pas]
 K = 10  # Pipe roughness in [m]
-TINIT = 11  # Temperature in [K]
-VINIT = 12  # velocity in  [m/s]
-RE = 13  # Reynolds number
-LAMBDA = 14  # Lambda
-JAC_DERIV_DV = 15  # Slot for the derivative by velocity
-JAC_DERIV_DP = 16  # Slot for the derivative by pressure from_node
-JAC_DERIV_DP1 = 17  # Slot for the derivative by pressure to_node
-LOAD_VEC_BRANCHES = 18  # Slot for the load vector for the branches
-JAC_DERIV_DV_NODE = 19  # Slot for the derivative by velocity for the nodes connected to branch
-LOAD_VEC_NODES = 20  # Slot for the load vector of the nodes connected to branch
-LOSS_COEFFICIENT = 21
-CP = 22  # Slot for fluid heat capacity values
-ALPHA = 23  # Slot for heat transfer coefficient
-JAC_DERIV_DT = 24
-JAC_DERIV_DT1 = 25
-LOAD_VEC_BRANCHES_T = 26
-T_OUT = 27  # Internal slot for outlet pipe temperature
-JAC_DERIV_DT_NODE = 28  # Slot for the derivative fpr T for the nodes connected to branch
-LOAD_VEC_NODES_T = 29
-VINIT_T = 30
-FROM_NODE_T = 31
-TO_NODE_T = 32
-QEXT = 33  # heat input in [W]
-TEXT = 34
-STD_TYPE = 35
-PL = 36
-TL = 37  # Temperature lift [K]
-BRANCH_TYPE = 38  # branch type relevant for the pressure controller
-PRESSURE_RATIO = 39  # boost ratio for compressors with proportional pressure lift
+VINIT = 11  # velocity in  [m/s]
+RE = 12 # Reynolds number
+LAMBDA = 13  # Lambda
+JAC_DERIV_DV = 14  # Slot for the derivative by velocity
+JAC_DERIV_DP = 15  # Slot for the derivative by pressure from_node
+JAC_DERIV_DP1 = 16  # Slot for the derivative by pressure to_node
+LOAD_VEC_BRANCHES = 17  # Slot for the load vector for the branches
+JAC_DERIV_DV_NODE = 18  # Slot for the derivative by velocity for the nodes connected to branch
+LOAD_VEC_NODES = 19  # Slot for the load vector of the nodes connected to branch
+LOSS_COEFFICIENT = 20
+CP = 21  # Slot for fluid heat capacity values
+ALPHA = 22  # Slot for heat transfer coefficient
+JAC_DERIV_DT = 23
+JAC_DERIV_DT1 = 24
+LOAD_VEC_BRANCHES_T = 25
+TOUTINIT = 26  # Internal slot for outlet pipe temperature
+JAC_DERIV_DT_NODE = 27  # Slot for the derivative fpr T for the nodes connected to branch
+LOAD_VEC_NODES_T = 28
+VINIT_T = 29
+FROM_NODE_T = 30
+TO_NODE_T = 31
+QEXT = 32  # heat input in [W]
+TEXT = 33
+PL = 34
+TL = 35 # Temperature lift [K]
+BRANCH_TYPE = 36  # branch type relevant for the pressure controller
 
-branch_cols = 40
+branch_cols = 37
```

## Comparing `pandapipes-0.8.5/pandapipes/constants.py` & `pandapipes-0.9.0/src/pandapipes/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 # physical constants
 GRAVITATION_CONSTANT = 9.81  # earth acceleration constant in m/s²
 NORMAL_TEMPERATURE = 273.15  # normal temperature (= 0°C) in K
 NORMAL_PRESSURE = 1.01325  # pressure under normal conditions (at sea level) in bar
```

## Comparing `pandapipes-0.8.5/pandapipes/control/run_control.py` & `pandapipes-0.9.0/src/pandapipes/control/run_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapower.control import run_control as run_control_pandapower, \
     prepare_run_ctrl as prepare_run_control_pandapower
 import pandapipes as ppipe
 from pandapipes.pipeflow import PipeflowNotConverged
```

## Comparing `pandapipes-0.8.5/pandapipes/timeseries/run_time_series.py` & `pandapipes-0.9.0/src/pandapipes/timeseries/run_time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import tempfile
 
 from pandapower.control import NetCalculationNotConverged
-
-from pandapipes.pipeflow import PipeflowNotConverged, pipeflow
 from pandapower.control.util.diagnostic import control_diagnostic
 from pandapower.timeseries.output_writer import OutputWriter
-from pandapower.timeseries.run_time_series import init_time_series as init_time_series_pp, cleanup,\
+from pandapower.timeseries.run_time_series import init_time_series as init_time_series_pp, cleanup, \
     run_loop
 
+from pandapipes.pipeflow import PipeflowNotConverged, pipeflow
+
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
-logger.setLevel(level=logging.WARNING)
 
 
 def init_default_outputwriter(net, time_steps, **kwargs):
     """
     Creates a default output writer for the time series calculation.
 
     :param net: The pandapipes format network
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/circulation_pump_mass_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_mass_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
 from pandapipes.component_models.junction_component import Junction
@@ -68,10 +68,7 @@
         juncts, loads_sum = _sum_by_group(get_net_option(net, "use_numba"),
                                           circ_pump.return_junction.values, mass_flow_loads)
         junction_idx_lookups = get_lookup(net, "node", "index")[
             cls.get_connected_node_type().table_name()]
         index = junction_idx_lookups[juncts]
         node_pit[index, LOAD] += loads_sum
 
-    @classmethod
-    def calculate_temperature_lift(cls, net, pipe_pit, node_pit):
-        pass
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/pressure_control_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/pressure_control_component.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
 from pandapipes.component_models.abstract_models.branch_wzerolength_models import \
     BranchWZeroLengthComponent
 from pandapipes.component_models.junction_component import Junction
-from pandapipes.idx_branch import D, AREA, TL, \
+from pandapipes.idx_branch import D, AREA, \
     JAC_DERIV_DP, JAC_DERIV_DP1, JAC_DERIV_DV, BRANCH_TYPE, LOSS_COEFFICIENT as LC
 from pandapipes.idx_node import PINIT, NODE_TYPE, PC
 from pandapipes.pf.pipeflow_setup import get_lookup
 from pandapipes.pf.result_extraction import extract_branch_results_without_internals
 from pandapipes.properties.fluids import get_fluid
 
 
@@ -76,61 +76,44 @@
         press_pit = branch_pit[f:t, :]
         pc_branch = press_pit[:, BRANCH_TYPE] == PC
         press_pit[pc_branch, JAC_DERIV_DP] = 0
         press_pit[pc_branch, JAC_DERIV_DP1] = 0
         press_pit[pc_branch, JAC_DERIV_DV] = 0
 
     @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
-        """
-
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
-        :param node_pit:
-        :type node_pit:
-        :return:
-        :rtype:
-        """
-        branch_component_pit[:, TL] = 0
-
-    @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
+        :param mode:
+        :type mode:
         :param branch_results:
         :type branch_results:
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
         :return: No Output.
         """
-        required_results = [
-            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("t_from_k", "temp_from"),
-            ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to"), ("mdot_from_kg_per_s", "mf_from"),
-            ("vdot_norm_m3_per_s", "vf")
+        required_results_hyd = [
+            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("mdot_from_kg_per_s", "mf_from"),
+            ("mdot_to_kg_per_s", "mf_to"), ("vdot_norm_m3_per_s", "vf")
         ]
+        required_results_ht = [("t_from_k", "temp_from"), ("t_to_k", "temp_to")]
 
         if get_fluid(net).is_gas:
-            required_results.extend([
+            required_results_hyd.extend([
                 ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
                 ("normfactor_from", "normfactor_from"), ("normfactor_to", "normfactor_to")
             ])
         else:
-            required_results.extend([("v_mean_m_per_s", "v_mps")])
+            required_results_hyd.extend([("v_mean_m_per_s", "v_mps")])
 
-        extract_branch_results_without_internals(net, branch_results, required_results,
-                                                 cls.table_name(), branches_connected)
+        extract_branch_results_without_internals(net, branch_results, required_results_hyd,
+                                                 required_results_ht, cls.table_name(), mode)
 
         res_table = net["res_" + cls.table_name()]
         f, t = get_lookup(net, "branch", "from_to")[cls.table_name()]
         p_to = branch_results["p_to"][f:t]
         p_from = branch_results["p_from"][f:t]
         res_table["deltap_bar"].values[:] = p_to - p_from
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/valve_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/heat_exchanger_component.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
+from pandapipes.component_models import standard_branch_wo_internals_result_lookup
 from pandapipes.component_models.abstract_models.branch_wzerolength_models import \
     BranchWZeroLengthComponent
 from pandapipes.component_models.junction_component import Junction
-from pandapipes.idx_branch import D, AREA, LOSS_COEFFICIENT as LC, TL
+from pandapipes.idx_branch import ALPHA, TEXT, QEXT, D, AREA, LOSS_COEFFICIENT as LC, TOUTINIT
+from pandapipes.pf.pipeflow_setup import get_fluid
 from pandapipes.pf.result_extraction import extract_branch_results_without_internals
-from pandapipes.properties.fluids import get_fluid
 
+try:
+    import pandaplan.core.pplog as logging
+except ImportError:
+    import logging
 
-class Valve(BranchWZeroLengthComponent):
-    """
-    Valves are branch elements that can separate two junctions.
-    They have a length of 0, but can introduce a lumped pressure loss.
-    """
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+
+class HeatExchanger(BranchWZeroLengthComponent):
 
     @classmethod
     def from_to_node_cols(cls):
         return "from_junction", "to_junction"
 
     @classmethod
     def table_name(cls):
-        return "valve"
+        return "heat_exchanger"
 
     @classmethod
     def active_identifier(cls):
-        return "opened"
+        return "in_service"
 
     @classmethod
     def get_connected_node_type(cls):
         return Junction
 
     @classmethod
     def create_pit_branch_entries(cls, net, branch_pit):
@@ -42,70 +47,62 @@
 
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param branch_pit:
         :type branch_pit:
         :return: No Output.
         """
-        valve_pit = super().create_pit_branch_entries(net, branch_pit)
-        valve_pit[:, D] = net[cls.table_name()].diameter_m.values
-        valve_pit[:, AREA] = valve_pit[:, D] ** 2 * np.pi / 4
-        valve_pit[:, LC] = net[cls.table_name()].loss_coefficient.values
+        heat_exchanger_pit = super().create_pit_branch_entries(net, branch_pit)
+        heat_exchanger_pit[:, D] = net[cls.table_name()].diameter_m.values
+        heat_exchanger_pit[:, AREA] = heat_exchanger_pit[:, D] ** 2 * np.pi / 4
+        heat_exchanger_pit[:, LC] = net[cls.table_name()].loss_coefficient.values
+        heat_exchanger_pit[:, ALPHA] = 0
+        heat_exchanger_pit[:, QEXT] = net[cls.table_name()].qext_w.values
+        heat_exchanger_pit[:, TEXT] = 293.15
+        heat_exchanger_pit[:, TOUTINIT] = 307
 
     @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
+    def extract_results(cls, net, options, branch_results, mode):
         """
+        Class method to extract pipeflow results from the internal structure into the results table.
 
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
-        :param node_pit:
-        :type node_pit:
-        :return:
-        :rtype:
+        :param net: The pandapipes network
+        :type net: pandapipesNet
+        :param options: pipeflow options
+        :type options: dict
+        :param branch_results: important branch results
+        :type branch_results: dict
+        :param mode: simulation mode
+        :type mode: str
+        :return: No Output.
+        :rtype: None
         """
-        branch_component_pit[:, TL] = 0
+        required_results_hyd, required_results_ht = standard_branch_wo_internals_result_lookup(net)
+
+        extract_branch_results_without_internals(net, branch_results, required_results_hyd,
+                                                 required_results_ht, cls.table_name(), mode)
+
 
     @classmethod
     def get_component_input(cls):
         """
 
         :return:
         :rtype:
         """
         return [("name", dtype(object)),
-                ("from_junction", "i8"),
-                ("to_junction", "i8"),
+                ("from_junction", "u4"),
+                ("to_junction", "u4"),
                 ("diameter_m", "f8"),
-                ("opened", "bool"),
+                ("qext_w", 'f8'),
                 ("loss_coefficient", "f8"),
+                ("in_service", 'bool'),
                 ("type", dtype(object))]
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
-        required_results = [
-            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("t_from_k", "temp_from"),
-            ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to"), ("mdot_from_kg_per_s", "mf_from"),
-            ("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"), ("reynolds", "reynolds")
-        ]
-
-        if get_fluid(net).is_gas:
-            required_results.extend([
-                ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
-                ("v_mean_m_per_s", "v_gas_mean"), ("normfactor_from", "normfactor_from"),
-                ("normfactor_to", "normfactor_to")
-            ])
-        else:
-            required_results.extend([("v_mean_m_per_s", "v_mps")])
-
-        extract_branch_results_without_internals(net, branch_results, required_results,
-                                                 cls.table_name(), branches_connected)
-
-    @classmethod
     def get_result_table(cls, net):
         """
 
         :param net: The pandapipes network
         :type net: pandapipesNet
         :return: (columns, all_float) - the column names and whether they are all float type. Only
                 if False, returns columns as tuples also specifying the dtypes
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/heat_exchanger_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/flow_control_component.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,123 +1,126 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
-# and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
+# and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
-from pandapipes.component_models.abstract_models.branch_wzerolength_models import \
-    BranchWZeroLengthComponent
+from pandapipes.component_models.abstract_models import BranchWZeroLengthComponent, get_fluid
+from pandapipes.component_models.component_toolbox import \
+    standard_branch_wo_internals_result_lookup, get_component_array
 from pandapipes.component_models.junction_component import Junction
-from pandapipes.idx_branch import TL, ALPHA, TEXT, QEXT, T_OUT, D, AREA, LOSS_COEFFICIENT as LC
-from pandapipes.pf.pipeflow_setup import get_fluid
+from pandapipes.idx_branch import D, AREA, JAC_DERIV_DP, JAC_DERIV_DP1, JAC_DERIV_DV, VINIT, \
+    RHO, LOAD_VEC_BRANCHES
 from pandapipes.pf.result_extraction import extract_branch_results_without_internals
 
-try:
-    import pandaplan.core.pplog as logging
-except ImportError:
-    import logging
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.DEBUG)
+class FlowControlComponent(BranchWZeroLengthComponent):
+    """
 
+    """
+    CONTROL_ACTIVE = 0
 
-class HeatExchanger(BranchWZeroLengthComponent):
-
-    @classmethod
-    def from_to_node_cols(cls):
-        return "from_junction", "to_junction"
+    internal_cols = 1
 
     @classmethod
     def table_name(cls):
-        return "heat_exchanger"
+        return "flow_control"
 
     @classmethod
     def active_identifier(cls):
         return "in_service"
 
     @classmethod
+    def from_to_node_cols(cls):
+        return "from_junction", "to_junction"
+
+    @classmethod
     def get_connected_node_type(cls):
         return Junction
 
     @classmethod
     def create_pit_branch_entries(cls, net, branch_pit):
         """
         Function which creates pit branch entries with a specific table.
-
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param branch_pit:
         :type branch_pit:
         :return: No Output.
         """
-        heat_exchanger_pit = super().create_pit_branch_entries(net, branch_pit)
-        heat_exchanger_pit[:, D] = net[cls.table_name()].diameter_m.values
-        heat_exchanger_pit[:, AREA] = heat_exchanger_pit[:, D] ** 2 * np.pi / 4
-        heat_exchanger_pit[:, LC] = net[cls.table_name()].loss_coefficient.values
-        heat_exchanger_pit[:, ALPHA] = 0
-        heat_exchanger_pit[:, QEXT] = net[cls.table_name()].qext_w.values
-        heat_exchanger_pit[:, TEXT] = 293.15
-        heat_exchanger_pit[:, T_OUT] = 307
-
-    @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
-        required_results = [
-            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("t_from_k", "temp_from"),
-            ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to"), ("mdot_from_kg_per_s", "mf_from"),
-            ("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"), ("reynolds", "reynolds")
-        ]
-
-        if get_fluid(net).is_gas:
-            required_results.extend([
-                ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
-                ("v_mean_m_per_s", "v_gas_mean"), ("normfactor_from", "normfactor_from"),
-                ("normfactor_to", "normfactor_to")
-            ])
-        else:
-            required_results.extend([("v_mean_m_per_s", "v_mps")])
-
-        extract_branch_results_without_internals(net, branch_results, required_results,
-                                                 cls.table_name(), branches_connected)
-
-    @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
-        """
-
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
-        :param node_pit:
-        :type node_pit:
+        fc_branch_pit = super().create_pit_branch_entries(net, branch_pit)
+        fc_branch_pit[:, D] = net[cls.table_name()].diameter_m.values
+        fc_branch_pit[:, AREA] = fc_branch_pit[:, D] ** 2 * np.pi / 4
+        fc_branch_pit[:, VINIT] = net[cls.table_name()].controlled_mdot_kg_per_s.values / \
+            (fc_branch_pit[:, AREA] * fc_branch_pit[:, RHO])
+
+    @classmethod
+    def create_component_array(cls, net, component_pits):
+        """
+        Function which creates an internal array of the component in analogy to the pit, but with
+        component specific entries, that are not needed in the pit.
+
+        :param net: The pandapipes network
+        :type net: pandapipesNet
+        :param component_pits: dictionary of component specific arrays
+        :type component_pits: dict
         :return:
         :rtype:
         """
-        branch_component_pit[:, TL] = 0
+        tbl = net[cls.table_name()]
+        fc_pit = np.zeros(shape=(len(tbl), cls.internal_cols), dtype=np.float64)
+        fc_pit[:, cls.CONTROL_ACTIVE] = tbl.control_active.values
+        component_pits[cls.table_name()] = fc_pit
+
+
+    @classmethod
+    def adaption_after_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
+        # set all pressure derivatives to 0 and velocity to 1; load vector must be 0, as no change
+        # of velocity is allowed during the pipeflow iteration
+        f, t = idx_lookups[cls.table_name()]
+        fc_branch_pit = branch_pit[f:t, :]
+        fc_array = get_component_array(net, cls.table_name())
+        active = fc_array[:, cls.CONTROL_ACTIVE].astype(np.bool_)
+        fc_branch_pit[active, JAC_DERIV_DP] = 0
+        fc_branch_pit[active, JAC_DERIV_DP1] = 0
+        fc_branch_pit[active, JAC_DERIV_DV] = 1
+        fc_branch_pit[active, LOAD_VEC_BRANCHES] = 0
+
+    @classmethod
+    def extract_results(cls, net, options, branch_results, mode):
+        required_results_hyd, required_results_ht = standard_branch_wo_internals_result_lookup(net)
+
+        extract_branch_results_without_internals(net, branch_results, required_results_hyd,
+                                                 required_results_ht, cls.table_name(), mode)
 
     @classmethod
     def get_component_input(cls):
         """
 
+        Get component input.
+
         :return:
         :rtype:
         """
         return [("name", dtype(object)),
                 ("from_junction", "u4"),
                 ("to_junction", "u4"),
+                ("controlled_mdot_kg_per_s", "f8"),
                 ("diameter_m", "f8"),
-                ("qext_w", 'f8'),
-                ("loss_coefficient", "f8"),
+                ("control_active", "bool"),
                 ("in_service", 'bool'),
                 ("type", dtype(object))]
 
     @classmethod
     def get_result_table(cls, net):
         """
 
+        Gets the result table.
+
         :param net: The pandapipes network
         :type net: pandapipesNet
         :return: (columns, all_float) - the column names and whether they are all float type. Only
                 if False, returns columns as tuples also specifying the dtypes
         :rtype: (list, bool)
         """
         if get_fluid(net).is_gas:
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/source_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/source_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 from pandapipes.component_models.junction_component import Junction
 from pandapipes.component_models.abstract_models.const_flow_models import ConstFlow
 
 
 class Source(ConstFlow):
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/pump_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/pump_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from operator import itemgetter
 
 import numpy as np
 from numpy import dtype
 
-from pandapipes.component_models.junction_component import Junction
 from pandapipes.component_models.abstract_models.branch_wzerolength_models import \
     BranchWZeroLengthComponent
+from pandapipes.component_models.component_toolbox import get_component_array
+from pandapipes.component_models.junction_component import Junction
 from pandapipes.constants import NORMAL_TEMPERATURE, NORMAL_PRESSURE, R_UNIVERSAL, P_CONVERSION
-from pandapipes.idx_branch import STD_TYPE, VINIT, D, AREA, TL, LOSS_COEFFICIENT as LC, FROM_NODE, \
-    TINIT, PL
+from pandapipes.idx_branch import VINIT, D, AREA, LOSS_COEFFICIENT as LC, FROM_NODE, PL
 from pandapipes.idx_node import PINIT, PAMB, TINIT as TINIT_NODE
 from pandapipes.pf.pipeflow_setup import get_fluid, get_net_option, get_lookup
 from pandapipes.pf.result_extraction import extract_branch_results_without_internals
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
@@ -25,14 +25,17 @@
 logger = logging.getLogger(__name__)
 
 
 class Pump(BranchWZeroLengthComponent):
     """
 
     """
+    STD_TYPE = 0
+
+    internal_cols = 1
 
     @classmethod
     def from_to_node_cols(cls):
         return "from_junction", "to_junction"
 
     @classmethod
     def table_name(cls):
@@ -54,101 +57,105 @@
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param branch_pit:
         :type branch_pit:
         :return: No Output.
         """
         pump_pit = super().create_pit_branch_entries(net, branch_pit)
-        std_types_lookup = np.array(list(net.std_types[cls.table_name()].keys()))
-        std_type, pos = np.where(net[cls.table_name()]['std_type'].values
-                                 == std_types_lookup[:, np.newaxis])
-        pump_pit[pos, STD_TYPE] = std_type
         pump_pit[:, D] = 0.1
         pump_pit[:, AREA] = pump_pit[:, D] ** 2 * np.pi / 4
         pump_pit[:, LC] = 0
 
     @classmethod
+    def create_component_array(cls, net, component_pits):
+        """
+        Function which creates an internal array of the component in analogy to the pit, but with
+        component specific entries, that are not needed in the pit.
+
+        :param net: The pandapipes network
+        :type net: pandapipesNet
+        :param component_pits: dictionary of component specific arrays
+        :type component_pits: dict
+        :return:
+        :rtype:
+        """
+        tbl = net[cls.table_name()]
+        pump_array = np.zeros(shape=(len(tbl), cls.internal_cols), dtype=np.float64)
+        std_types_lookup = get_std_type_lookup(net, cls.table_name())
+        std_type, pos = np.where(net[cls.table_name()]['std_type'].values
+                                 == std_types_lookup[:, np.newaxis])
+        pump_array[pos, cls.STD_TYPE] = std_type
+        component_pits[cls.table_name()] = pump_array
+
+    @classmethod
     def adaption_before_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
         # calculation of pressure lift
         f, t = idx_lookups[cls.table_name()]
-        pump_pit = branch_pit[f:t, :]
-        area = pump_pit[:, AREA]
-        idx = pump_pit[:, STD_TYPE].astype(int)
-        std_types = np.array(list(net.std_types['pump'].keys()))[idx]
-        from_nodes = pump_pit[:, FROM_NODE].astype(np.int32)
-        # to_nodes = pump_pit[:, TO_NODE].astype(np.int32)
+        pump_branch_pit = branch_pit[f:t, :]
+        area = pump_branch_pit[:, AREA]
+
+        pump_array = get_component_array(net, cls.table_name())
+        idx = pump_array[:, cls.STD_TYPE].astype(np.int32)
+        std_types = get_std_type_lookup(net, cls.table_name())[idx]
+
+        from_nodes = pump_branch_pit[:, FROM_NODE].astype(np.int32)
+        # to_nodes = pump_branch_pit[:, TO_NODE].astype(np.int32)
         fluid = get_fluid(net)
         p_from = node_pit[from_nodes, PAMB] + node_pit[from_nodes, PINIT]
         # p_to = node_pit[to_nodes, PAMB] + node_pit[to_nodes, PINIT]
-        numerator = NORMAL_PRESSURE * pump_pit[:, TINIT]
-        v_mps = pump_pit[:, VINIT]
+        t_from = node_pit[from_nodes, TINIT_NODE]
+        numerator_from = NORMAL_PRESSURE * t_from
+        v_mps = pump_branch_pit[:, VINIT]
         if fluid.is_gas:
             # consider volume flow at inlet
-            normfactor_from = numerator * fluid.get_property("compressibility", p_from) \
+            normfactor_from = numerator_from * fluid.get_property("compressibility", p_from) \
                               / (p_from * NORMAL_TEMPERATURE)
-            v_mean = v_mps * normfactor_from
+            v_from = v_mps * normfactor_from
         else:
-            v_mean = v_mps
-        vol = v_mean * area
+            v_from = v_mps
+        vol = v_from * area
         if len(std_types):
             fcts = itemgetter(*std_types)(net['std_types']['pump'])
             fcts = [fcts] if not isinstance(fcts, tuple) else fcts
             pl = np.array(list(map(lambda x, y: x.get_pressure(y), fcts, vol)))
-            pump_pit[:, PL] = pl
+            pump_branch_pit[:, PL] = pl
 
     @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
-        """
-
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
-        :param node_pit:
-        :type node_pit:
-        :return:
-        :rtype:
-        """
-        branch_component_pit[:, TL] = 0
-
-    @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
         :param branch_results:
         :type branch_results:
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
+        :param mode:
+        :type mode:
         :return: No Output.
         """
         calc_compr_pow = options['calc_compression_power']
 
-        required_results = [
-            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("t_from_k", "temp_from"),
-            ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to"), ("mdot_from_kg_per_s", "mf_from"),
-            ("vdot_norm_m3_per_s", "vf"), ("deltap_bar", "pl")
+        required_results_hyd = [
+            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("mdot_to_kg_per_s", "mf_to"),
+            ("mdot_from_kg_per_s", "mf_from"), ("vdot_norm_m3_per_s", "vf"), ("deltap_bar", "pl"),
         ]
+        required_results_ht = [("t_from_k", "temp_from"), ("t_to_k", "temp_to")]
 
         if get_fluid(net).is_gas:
-            required_results.extend([
+            required_results_hyd.extend([
                 ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
                 ("normfactor_from", "normfactor_from"), ("normfactor_to", "normfactor_to")
             ])
         else:
-            required_results.extend([("v_mean_m_per_s", "v_mps")])
+            required_results_hyd.extend([("v_mean_m_per_s", "v_mps")])
 
-        extract_branch_results_without_internals(net, branch_results, required_results,
-                                                 cls.table_name(), branches_connected)
+        extract_branch_results_without_internals(net, branch_results, required_results_hyd,
+                                                 required_results_ht, cls.table_name(), mode)
 
         if calc_compr_pow:
             f, t = get_lookup(net, "branch", "from_to")[cls.table_name()]
             from_nodes = branch_results["from_nodes"][f:t]
 
             res_table = net["res_" + cls.table_name()]
             if net.fluid.is_gas:
@@ -218,7 +225,11 @@
         else:
             output = ["deltap_bar", "v_mean_m_per_s", "p_from_bar", "p_to_bar", "t_from_k",
                       "t_to_k", "mdot_from_kg_per_s", "mdot_to_kg_per_s", "vdot_norm_m3_per_s"]
         if calc_compr_pow:
             output += ["compr_power_mw"]
 
         return output, True
+
+
+def get_std_type_lookup(net, table_name):
+    return np.array(list(net.std_types[table_name].keys()))
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/ext_grid_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/ext_grid_component.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
 from pandapipes.component_models.abstract_models.node_element_models import NodeElementComponent
@@ -58,28 +58,26 @@
         press = ext_grids.p_bar.values
         set_fixed_node_entries(net, node_pit, junction, ext_grids.type.values, press,
                                ext_grids.t_k.values, cls.get_connected_node_type())
 
         return ext_grids, press
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
         :param branch_results:
         :type branch_results:
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
+        :param mode:
+        :type mode:
         :return: No Output.
         """
         ext_grids = net[cls.table_name()]
 
         if len(ext_grids) == 0:
             return
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/junction_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/junction_component.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from warnings import warn
 
 import numpy as np
 from numpy import dtype
@@ -84,45 +84,52 @@
         junction_pit[:, PINIT] = junctions.pn_bar.values
         junction_pit[:, TINIT] = junctions.tfluid_k.values
         junction_pit[:, RHO] = get_fluid(net).get_density(junction_pit[:, TINIT])
         junction_pit[:, PAMB] = p_correction_height_air(junction_pit[:, HEIGHT])
         junction_pit[:, ACTIVE_ND] = junctions.in_service.values
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
-        :param branch_results:
-        :type branch_results:
+        :param mode:
+        :type mode:
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
+        :param branch_results:
+        :type branch_results:
+        :param mode:
+        :type mode:
         :return: No Output.
         """
         res_table = net["res_" + cls.table_name()]
 
         f, t = get_lookup(net, "node", "from_to")[cls.table_name()]
-        fa, ta = get_lookup(net, "node", "from_to_active")[cls.table_name()]
-
-        junction_pit = net["_active_pit"]["node"][fa:ta, :]
-        junctions_active = get_lookup(net, "node", "active")[f:t]
+        junction_pit = net["_pit"]["node"][f:t, :]
 
-        if np.any(junction_pit[:, PINIT] < 0):
-            warn(UserWarning('Pipeflow converged, however, the results are physically incorrect '
-                             'as pressure is negative at nodes %s'
-                             % junction_pit[junction_pit[:, PINIT] < 0, ELEMENT_IDX]))
+        if mode in ["hydraulics", "all"]:
+            junctions_connected_hydraulic = get_lookup(net, "node", "active_hydraulics")[f:t]
 
-        res_table["p_bar"].values[junctions_active] = junction_pit[:, PINIT]
-        res_table["t_k"].values[junctions_active] = junction_pit[:, TINIT]
+            if np.any(junction_pit[junctions_connected_hydraulic, PINIT] < 0):
+                warn(UserWarning('Pipeflow converged, however, the results are physically incorrect '
+                                 'as pressure is negative at nodes %s'
+                                 % junction_pit[junction_pit[:, PINIT] < 0, ELEMENT_IDX]))
+
+        #     res_table["p_bar"].values[junctions_connected_hydraulic] = junction_pit[:, PINIT]
+        #     if mode == "hydraulics":
+        #         res_table["t_k"].values[junctions_connected_hydraulic] = junction_pit[:, TINIT]
+        #
+        # if mode in ["heat", "all"]:
+        #     junctions_connected_ht = get_lookup(net, "node", "active_heat_transfer")[f:t]
+        #     res_table["t_k"].values[junctions_connected_ht] = junction_pit[:, TINIT]
+        res_table["p_bar"].values[:] = junction_pit[:, PINIT]
+        res_table["t_k"].values[:] = junction_pit[:, TINIT]
 
     @classmethod
     def get_component_input(cls):
         """
 
         :return:
         :rtype:
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/component_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/component_models/component_toolbox.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 
+from pandapipes import get_fluid
 from pandapipes.constants import NORMAL_PRESSURE, TEMP_GRADIENT_KPM, AVG_TEMPERATURE_K, \
     HEIGHT_EXPONENT
 from pandapipes.idx_branch import LOAD_VEC_NODES, FROM_NODE, TO_NODE
 from pandapipes.idx_node import EXT_GRID_OCCURENCE, EXT_GRID_OCCURENCE_T
 from pandapipes.idx_node import PINIT, NODE_TYPE, P, TINIT, NODE_TYPE_T, T, LOAD
 from pandapipes.pf.internals_toolbox import _sum_by_group
 from pandapipes.pf.pipeflow_setup import get_net_option, get_lookup
@@ -173,7 +174,49 @@
     all_mass_flows = np.concatenate([-mass_flow_from, mass_flow_to, -loads])
     nodes, sum_mass_flows = _sum_by_group(get_net_option(net, "use_numba"), all_index_nodes,
                                           all_mass_flows)
     if not np.all(nodes == node_uni):
         raise UserWarning("In component %s: Something went wrong with the mass flow balance. "
                           "Please report this error at github." % comp.__name__)
     return sum_mass_flows, inverse_nodes, counts
+
+
+def standard_branch_wo_internals_result_lookup(net):
+    required_results_hyd = [
+        ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("mdot_to_kg_per_s", "mf_to"),
+        ("mdot_from_kg_per_s", "mf_from"), ("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"),
+        ("reynolds", "reynolds")
+    ]
+    required_results_ht = [("t_from_k", "temp_from"), ("t_to_k", "temp_to")]
+
+    if get_fluid(net).is_gas:
+        required_results_hyd.extend([
+            ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
+            ("v_mean_m_per_s", "v_gas_mean"), ("normfactor_from", "normfactor_from"),
+            ("normfactor_to", "normfactor_to")
+        ])
+    else:
+        required_results_hyd.extend([("v_mean_m_per_s", "v_mps")])
+
+    return required_results_hyd, required_results_ht
+
+
+def get_component_array(net, component_name, component_type="branch", only_active=True):
+    """
+    Returns the internal array of a component.
+
+    :param net: The pandapipes network
+    :type net: pandapipesNet
+    :param component_name: Table name of the component for which to extract internal array
+    :type component_name: str
+    :param component_type: Type of component that is considered ("branch" or "node")
+    :type component_type: str, default "branch"
+    :param only_active: If True, only return entries of active elements (included in _active_pit)
+    :type only_active: bool
+    :return: component_array - internal array of the component
+    :rtype: numpy.ndarray
+    """
+    f_all, t_all = get_lookup(net, component_type, "from_to")[component_name]
+    if not only_active:
+        return net["_pit"]["components"][component_name]
+    in_service_elm = get_lookup(net, component_type, "active_hydraulics")[f_all:t_all]
+    return net["_pit"]["components"][component_name][in_service_elm]
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/pipe_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/pipe_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy import dtype
 from pandapipes.component_models.abstract_models import BranchWInternalsComponent
 from pandapipes.component_models.component_toolbox import p_correction_height_air, \
     vinterp, set_entry_check_repeat
 from pandapipes.component_models.junction_component import Junction
 from pandapipes.constants import NORMAL_TEMPERATURE, NORMAL_PRESSURE
 from pandapipes.idx_branch import FROM_NODE, TO_NODE, LENGTH, D, AREA, K, \
-    VINIT, ALPHA, QEXT, TEXT, LOSS_COEFFICIENT as LC, T_OUT, TL
+    VINIT, ALPHA, QEXT, TEXT, LOSS_COEFFICIENT as LC
 from pandapipes.idx_node import PINIT, HEIGHT, TINIT as TINIT_NODE, \
     RHO as RHO_NODES, PAMB, ACTIVE as ACTIVE_ND
 from pandapipes.pf.pipeflow_setup import get_fluid, get_lookup
 from pandapipes.pf.result_extraction import extract_branch_results_with_internals, \
     extract_branch_results_without_internals
 
 try:
@@ -147,55 +147,46 @@
         set_entry_check_repeat(
             pipe_pit, TEXT, net[tbl].text_k.values, internal_pipe_number, has_internals)
         set_entry_check_repeat(
             pipe_pit, D, net[tbl].diameter_m.values, internal_pipe_number, has_internals)
         set_entry_check_repeat(
             pipe_pit, LC, net[tbl].loss_coefficient.values, internal_pipe_number, has_internals)
 
-        pipe_pit[:, T_OUT] = 293
         pipe_pit[:, AREA] = pipe_pit[:, D] ** 2 * np.pi / 4
 
     @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
-        """
-
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
-        :param node_pit:
-        :type node_pit:
-        :return:
-        :rtype:
-        """
-        branch_component_pit[:, TL] = 0
-
-    @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
-        res_nodes_from = [("p_from_bar", "p_from"), ("t_from_k", "temp_from"),
-                          ("mdot_from_kg_per_s", "mf_from")]
-        res_nodes_to = [("p_to_bar", "p_to"), ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to")]
-        res_mean = [("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"), ("reynolds", "reynolds")]
+    def extract_results(cls, net, options, branch_results, mode):
+        res_nodes_from_hyd = [("p_from_bar", "p_from"), ("mdot_from_kg_per_s", "mf_from")]
+        res_nodes_from_ht = [("t_from_k", "temp_from")]
+        res_nodes_to_hyd = [("p_to_bar", "p_to"), ("mdot_to_kg_per_s", "mf_to")]
+        res_nodes_to_ht = [("t_to_k", "temp_to")]
+        res_mean_hyd = [("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"),
+                        ("reynolds", "reynolds")]
 
         if get_fluid(net).is_gas:
-            res_nodes_from.extend(
-                [("v_from_m_per_s", "v_gas_from"), ("normfactor_from", "normfactor_from")])
-            res_nodes_to.extend([("v_to_m_per_s", "v_gas_to"), ("normfactor_to", "normfactor_to")])
-            res_mean.extend([("v_mean_m_per_s", "v_gas_mean")])
+            res_nodes_from_hyd.extend([("v_from_m_per_s", "v_gas_from"),
+                                       ("normfactor_from", "normfactor_from")])
+            res_nodes_to_hyd.extend([("v_to_m_per_s", "v_gas_to"),
+                                     ("normfactor_to", "normfactor_to")])
+            res_mean_hyd.extend([("v_mean_m_per_s", "v_gas_mean")])
         else:
-            res_mean.extend([("v_mean_m_per_s", "v_mps")])
+            res_mean_hyd.extend([("v_mean_m_per_s", "v_mps")])
 
         if np.any(cls.get_internal_pipe_number(net) > 1):
             extract_branch_results_with_internals(
-                net, branch_results, cls.table_name(), res_nodes_from, res_nodes_to, res_mean,
-                cls.get_connected_node_type().table_name(), branches_connected)
+                net, branch_results, cls.table_name(), res_nodes_from_hyd, res_nodes_from_ht,
+                res_nodes_to_hyd, res_nodes_to_ht, res_mean_hyd, [],
+                cls.get_connected_node_type().table_name(), mode)
         else:
-            required_results = res_nodes_from + res_nodes_to + res_mean
-            extract_branch_results_without_internals(net, branch_results, required_results,
-                                                     cls.table_name(), branches_connected)
+            required_results_hyd = res_nodes_from_hyd + res_nodes_to_hyd + res_mean_hyd
+            required_results_ht = res_nodes_from_ht + res_nodes_to_ht
+            extract_branch_results_without_internals(
+                net, branch_results, required_results_hyd, required_results_ht, cls.table_name(),
+                mode
+            )
 
     @classmethod
     def get_internal_results(cls, net, pipe):
         """
         Retrieve velocity (at to/from node; mean), pressure and temperature of the internal sections
         of pipes. The pipes have to have at least 2 internal sections.
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/mass_storage_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/mass_storage_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 from pandapipes.component_models.junction_component import Junction
 from pandapipes.component_models.abstract_models import ConstFlow
 from numpy import dtype
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/flow_control_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/circulation_pump.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,140 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
-# and Energy System Technology (IEE), Kassel. All rights reserved.
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
+# and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
-from numpy import dtype
 
-from pandapipes.component_models.junction_component import Junction
-from pandapipes.component_models.abstract_models import BranchWZeroLengthComponent, get_fluid
-from pandapipes.idx_branch import D, AREA, TL, JAC_DERIV_DP, JAC_DERIV_DP1, JAC_DERIV_DV, VINIT, \
-    RHO, LOAD_VEC_BRANCHES, ELEMENT_IDX
-from pandapipes.pf.result_extraction import extract_branch_results_without_internals
+from pandapipes.component_models.abstract_models.branch_wzerolength_models import \
+    BranchWZeroLengthComponent
+from pandapipes.component_models.component_toolbox import set_fixed_node_entries, \
+    get_mass_flow_at_nodes
+from pandapipes.idx_branch import D, AREA, ACTIVE
+from pandapipes.idx_node import PINIT
+from pandapipes.pf.pipeflow_setup import get_lookup
+
+try:
+    import pandaplan.core.pplog as logging
+except ImportError:
+    import logging
 
+logger = logging.getLogger(__name__)
 
-class FlowControlComponent(BranchWZeroLengthComponent):
-    """
 
-    """
+class CirculationPump(BranchWZeroLengthComponent):
 
     @classmethod
     def table_name(cls):
-        return "flow_control"
+        raise NotImplementedError
+
+    @classmethod
+    def get_component_input(cls):
+        raise NotImplementedError
+
+    @classmethod
+    def get_result_table(cls, net):
+        """
+
+        :param net: The pandapipes network
+        :type net: pandapipesNet
+        :return: (columns, all_float) - the column names and whether they are all float type. Only
+                if False, returns columns as tuples also specifying the dtypes
+        :rtype: (list, bool)
+        """
+        return ["mdot_flow_kg_per_s", "deltap_bar"], True
 
     @classmethod
     def active_identifier(cls):
-        return "in_service"
+        raise NotImplementedError
 
     @classmethod
     def from_to_node_cols(cls):
-        return "from_junction", "to_junction"
+        return "return_junction", "flow_junction"
 
     @classmethod
     def get_connected_node_type(cls):
+        from pandapipes.component_models.junction_component import Junction
         return Junction
 
     @classmethod
-    def create_pit_branch_entries(cls, net, branch_pit):
+    def create_pit_node_entries(cls, net, node_pit):
         """
-        Function which creates pit branch entries with a specific table.
+        Function which creates pit node entries.
+
         :param net: The pandapipes network
         :type net: pandapipesNet
-        :param branch_pit:
-        :type branch_pit:
-        :return: No Output.
-        """
-        fc_pit = super().create_pit_branch_entries(net, branch_pit)
-        fc_pit[:, D] = net[cls.table_name()].diameter_m.values
-        fc_pit[:, AREA] = fc_pit[:, D] ** 2 * np.pi / 4
-        fc_pit[:, VINIT] = net[cls.table_name()].controlled_mdot_kg_per_s.values / \
-            (fc_pit[:, AREA] * fc_pit[:, RHO])
-
-    @classmethod
-    def adaption_before_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
-        pass
-
-    @classmethod
-    def adaption_after_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
-        # set all pressure derivatives to 0 and velocity to 1; load vector must be 0, as no change
-        # of velocity is allowed during the pipeflow iteration
-        f, t = idx_lookups[cls.table_name()]
-        fc_pit = branch_pit[f:t, :]
-        in_service_elm = np.isin(net[cls.table_name()].index.values,
-                                 fc_pit[:, ELEMENT_IDX].astype(np.int32))
-        active = net[cls.table_name()].control_active.values[in_service_elm]
-        fc_pit[active, JAC_DERIV_DP] = 0
-        fc_pit[active, JAC_DERIV_DP1] = 0
-        fc_pit[active, JAC_DERIV_DV] = 1
-        fc_pit[active, LOAD_VEC_BRANCHES] = 0
-
-    @classmethod
-    def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
-        """
-
-        :param net:
-        :type net:
-        :param branch_component_pit:
-        :type branch_component_pit:
         :param node_pit:
         :type node_pit:
-        :return:
-        :rtype:
+        :return: No Output.
         """
-        branch_component_pit[:, TL] = 0
+        circ_pump_tbl = net[cls.table_name()][net[cls.table_name()][cls.active_identifier()].values]
 
-    @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
-        required_results = [
-            ("p_from_bar", "p_from"), ("p_to_bar", "p_to"), ("t_from_k", "temp_from"),
-            ("t_to_k", "temp_to"), ("mdot_to_kg_per_s", "mf_to"), ("mdot_from_kg_per_s", "mf_from"),
-            ("vdot_norm_m3_per_s", "vf"), ("lambda", "lambda"), ("reynolds", "reynolds")
-        ]
-
-        if get_fluid(net).is_gas:
-            required_results.extend([
-                ("v_from_m_per_s", "v_gas_from"), ("v_to_m_per_s", "v_gas_to"),
-                ("v_mean_m_per_s", "v_gas_mean"), ("normfactor_from", "normfactor_from"),
-                ("normfactor_to", "normfactor_to")
-            ])
-        else:
-            required_results.extend([("v_mean_m_per_s", "v_mps")])
+        junction = net[cls.table_name()][cls.from_to_node_cols()[1]].values
 
-        extract_branch_results_without_internals(net, branch_results, required_results,
-                                                 cls.table_name(), branches_connected)
+        # TODO: there should be a warning, if any p_bar value is not given or any of the types does
+        #       not contain "p", as this should not be allowed for this component
+        press = circ_pump_tbl.p_flow_bar.values
+        set_fixed_node_entries(net, node_pit, junction, circ_pump_tbl.type.values, press,
+                               circ_pump_tbl.t_flow_k.values, cls.get_connected_node_type())
+        return circ_pump_tbl, press
 
     @classmethod
-    def get_component_input(cls):
+    def create_pit_branch_entries(cls, net, branch_pit):
         """
-
-        Get component input.
-
-        :return:
-        :rtype:
+        Function which creates pit branch entries with a specific table.
+        :param net: The pandapipes network
+        :type net: pandapipesNet
+        :param branch_pit:
+        :type branch_pit:
+        :return: No Output.
         """
-        return [("name", dtype(object)),
-                ("from_junction", "u4"),
-                ("to_junction", "u4"),
-                ("controlled_mdot_kg_per_s", "f8"),
-                ("diameter_m", "f8"),
-                ("control_active", "bool"),
-                ("in_service", 'bool'),
-                ("type", dtype(object))]
+        circ_pump_pit = super().create_pit_branch_entries(net, branch_pit)
+        circ_pump_pit[:, D] = 0.1
+        circ_pump_pit[:, AREA] = circ_pump_pit[:, D] ** 2 * np.pi / 4
+        circ_pump_pit[:, ACTIVE] = False
 
     @classmethod
-    def get_result_table(cls, net):
+    def extract_results(cls, net, options, branch_results, mode):
         """
+        Function that extracts certain results.
 
-        Gets the result table.
-
+        :param mode:
+        :type mode:
+        :param branch_results:
+        :type branch_results:
         :param net: The pandapipes network
         :type net: pandapipesNet
-        :return: (columns, all_float) - the column names and whether they are all float type. Only
-                if False, returns columns as tuples also specifying the dtypes
-        :rtype: (list, bool)
+        :param options:
+        :type options:
+        :return: No Output.
         """
-        if get_fluid(net).is_gas:
-            output = ["v_from_m_per_s", "v_to_m_per_s", "v_mean_m_per_s", "p_from_bar", "p_to_bar",
-                      "t_from_k", "t_to_k", "mdot_from_kg_per_s", "mdot_to_kg_per_s",
-                      "vdot_norm_m3_per_s", "reynolds", "lambda", "normfactor_from",
-                      "normfactor_to"]
-        else:
-            output = ["v_mean_m_per_s", "p_from_bar", "p_to_bar", "t_from_k", "t_to_k",
-                      "mdot_from_kg_per_s", "mdot_to_kg_per_s", "vdot_norm_m3_per_s", "reynolds",
-                      "lambda"]
-        return output, True
+        circ_pump_tbl = net[cls.table_name()]
+
+        if len(circ_pump_tbl) == 0:
+            return
+
+        res_table = net["res_" + cls.table_name()]
+
+        branch_pit = net['_pit']['branch']
+        node_pit = net["_pit"]["node"]
+
+        junction_lookup = get_lookup(net, "node", "index")[
+            cls.get_connected_node_type().table_name()]
+        fn_col, tn_col = cls.from_to_node_cols()
+        # get indices in internal structure for flow_junctions in circ_pump tables which are
+        # "active"
+        flow_junctions = circ_pump_tbl[tn_col].values
+        flow_nodes = junction_lookup[flow_junctions]
+        in_service = circ_pump_tbl.in_service.values
+        p_grids = np.isin(circ_pump_tbl.type.values, ["p", "pt"]) & in_service
+        sum_mass_flows, inverse_nodes, counts = get_mass_flow_at_nodes(net, node_pit, branch_pit,
+                                                                       flow_nodes[p_grids], cls)
+
+        # positive results mean that the circ_pump feeds in, negative means that the ext grid
+        # extracts (like a load)
+        res_table["mdot_flow_kg_per_s"].values[p_grids] = - (sum_mass_flows / counts)[inverse_nodes]
+
+        return_junctions = circ_pump_tbl[fn_col].values
+        return_nodes = junction_lookup[return_junctions]
+
+        deltap_bar = node_pit[flow_nodes, PINIT] - node_pit[return_nodes, PINIT]
+        res_table["deltap_bar"].values[in_service] = deltap_bar[in_service]
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/circulation_pump_pressure_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/circulation_pump_pressure_component.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from numpy import dtype
 
 from pandapipes.component_models.abstract_models.circulation_pump import CirculationPump
 from pandapipes.component_models.component_toolbox import set_fixed_node_entries
@@ -59,11 +59,7 @@
         """
         circ_pump, press = super().create_pit_node_entries(net, node_pit)
 
         junction = circ_pump[cls.from_to_node_cols()[0]].values
         p_in = press - circ_pump.plift_bar.values
         set_fixed_node_entries(net, node_pit, junction, circ_pump.type.values, p_in, None,
                                cls.get_connected_node_type(), "p")
-
-    @classmethod
-    def calculate_temperature_lift(cls, net, pipe_pit, node_pit):
-        pass
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/__init__.py` & `pandapipes-0.9.0/src/pandapipes/component_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.junction_component import *
 from pandapipes.component_models.pipe_component import *
 from pandapipes.component_models.valve_component import *
 from pandapipes.component_models.ext_grid_component import *
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/sink_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/sink_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 from pandapipes.component_models.junction_component import Junction
 from pandapipes.component_models.abstract_models.const_flow_models import ConstFlow
 
 
 class Sink(ConstFlow):
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/base_component.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/base_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.component_toolbox import init_results_element
 
 try:
     import pandaplan.core.pplog as logging
@@ -29,28 +29,26 @@
         """
         output, all_float = cls.get_result_table(net)
         init_results_element(net, cls.table_name(), output, all_float)
         res_table = net["res_" + cls.table_name()]
         return res_table
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
         :param branch_results:
         :type branch_results:
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
+        :param mode:
+        :type mode:
         :return: No Output.
         """
         raise NotImplementedError
 
     @classmethod
     def get_component_input(cls):
         """
@@ -77,14 +75,23 @@
         pass
 
     @classmethod
     def adaption_after_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
         pass
 
     @classmethod
+    def adaption_before_derivatives_thermal(cls, net, branch_pit, node_pit, idx_lookups, options):
+        pass
+
+    @classmethod
+    def adaption_after_derivatives_thermal(cls, net, branch_pit, node_pit, idx_lookups, options):
+        pass
+
+
+    @classmethod
     def create_node_lookups(cls, net, ft_lookups, table_lookup, idx_lookups, current_start,
                             current_table, internal_nodes_lookup):
         """
         Function which creates node lookups.
 
         :param net: The pandapipes network
         :type net: pandapipesNet
@@ -124,69 +131,47 @@
         :param current_start:
         :type current_start:
         :return: No Output.
         """
         return current_start, current_table
 
     @classmethod
-    def create_pit_node_entries(cls, net, node_pit):
+    def create_component_array(cls, net, component_pits):
         """
-        Function which creates pit branch entries.
+        Function which creates an internal array of the component in analogy to the pit, but with
+        component specific entries, that are not needed in the pit.
 
         :param net: The pandapipes network
         :type net: pandapipesNet
-        :param node_pit:
-        :type node_pit:
-        :return: No Output.
+        :param component_pits: dictionary of component specific arrays
+        :type component_pits: dict
+        :return:
+        :rtype:
         """
         pass
 
     @classmethod
-    def create_pit_branch_entries(cls, net, branch_pit):
+    def create_pit_node_entries(cls, net, node_pit):
         """
         Function which creates pit branch entries.
 
         :param net: The pandapipes network
         :type net: pandapipesNet
-        :param branch_pit:
-        :type branch_pit:
-        :return: No Output.
-        """
-        pass
-
-    @classmethod
-    def calculate_derivatives_hydraulic(cls, net, branch_pit, node_pit, idx_lookups, options):
-        """
-        Function which creates derivatives.
-
-        :param net: The pandapipes network
-        :type net: pandapipesNet
-        :param branch_pit:
-        :type branch_pit:
         :param node_pit:
         :type node_pit:
-        :param idx_lookups:
-        :type idx_lookups:
-        :param options:
-        :type options:
         :return: No Output.
         """
         pass
 
     @classmethod
-    def calculate_derivatives_thermal(cls, net, branch_pit, node_pit, idx_lookups, options):
+    def create_pit_branch_entries(cls, net, branch_pit):
         """
-        Function which creates derivatives.
+        Function which creates pit branch entries.
 
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param branch_pit:
         :type branch_pit:
-        :param node_pit:
-        :type node_pit:
-        :param idx_lookups:
-        :type idx_lookups:
-        :param options:
-        :type options:
         :return: No Output.
         """
         pass
+
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wzerolength_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wzerolength_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.abstract_models.branch_wo_internals_models import \
     BranchWOInternalsComponent
 from pandapipes.idx_branch import LENGTH, K
 
@@ -57,13 +57,13 @@
         branch_wzerolength_pit = \
             super().create_pit_branch_entries(net, branch_pit)
         branch_wzerolength_pit[:, LENGTH] = 0
         branch_wzerolength_pit[:, K] = 1000
         return branch_wzerolength_pit
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         raise NotImplementedError
 
     @classmethod
     def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
         raise NotImplementedError
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.abstract_models.base_component import Component
 
 try:
     import pandaplan.core.pplog as logging
@@ -62,9 +62,9 @@
         raise NotImplementedError
 
     @classmethod
     def get_result_table(cls, net):
         raise NotImplementedError
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         raise NotImplementedError
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_wo_internals_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_wo_internals_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.abstract_models.branch_models import BranchComponent
 
-from pandapipes.idx_branch import FROM_NODE, TO_NODE, TINIT, ELEMENT_IDX, RHO, ETA, CP, ACTIVE
+from pandapipes.idx_branch import FROM_NODE, TO_NODE, TOUTINIT, ELEMENT_IDX, RHO, ETA, CP, ACTIVE
 from pandapipes.idx_node import TINIT as TINIT_NODE
 
 from pandapipes.pf.pipeflow_setup import add_table_lookup
 from pandapipes.properties.fluids import get_fluid
 
 try:
     import pandaplan.core.pplog as logging
@@ -78,27 +78,27 @@
         :return: No Output.
         """
         branch_wo_internals_pit, node_pit, from_nodes, to_nodes \
             = super().create_pit_branch_entries(net, branch_pit)
         branch_wo_internals_pit[:, ELEMENT_IDX] = net[cls.table_name()].index.values
         branch_wo_internals_pit[:, FROM_NODE] = from_nodes
         branch_wo_internals_pit[:, TO_NODE] = to_nodes
-        branch_wo_internals_pit[:, TINIT] = (node_pit[from_nodes, TINIT_NODE]
-                                             + node_pit[to_nodes, TINIT_NODE]) / 2
+        branch_wo_internals_pit[:, TOUTINIT] = node_pit[to_nodes, TINIT_NODE]
+        tm = (node_pit[from_nodes, TINIT_NODE] + branch_wo_internals_pit[:, TOUTINIT]) / 2
         fluid = get_fluid(net)
-        branch_wo_internals_pit[:, RHO] = fluid.get_density(branch_wo_internals_pit[:, TINIT])
-        branch_wo_internals_pit[:, ETA] = fluid.get_viscosity(branch_wo_internals_pit[:, TINIT])
-        branch_wo_internals_pit[:, CP] = fluid.get_heat_capacity(branch_wo_internals_pit[:, TINIT])
+        branch_wo_internals_pit[:, RHO] = fluid.get_density(tm)
+        branch_wo_internals_pit[:, ETA] = fluid.get_viscosity(tm)
+        branch_wo_internals_pit[:, CP] = fluid.get_heat_capacity(tm)
         branch_wo_internals_pit[:, ACTIVE] = net[cls.table_name()][cls.active_identifier()].values
         return branch_wo_internals_pit
 
     @classmethod
     def calculate_temperature_lift(cls, net, branch_component_pit, node_pit):
         raise NotImplementedError
 
     @classmethod
     def get_connected_node_type(cls):
         raise NotImplementedError
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         raise NotImplementedError
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/branch_w_internals_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/branch_w_internals_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 
 from pandapipes.component_models.abstract_models.branch_models import BranchComponent
 from pandapipes.component_models.component_toolbox import set_entry_check_repeat
-from pandapipes.idx_branch import ACTIVE, FROM_NODE, TO_NODE, TINIT, RHO, ETA, CP, ELEMENT_IDX
+from pandapipes.idx_branch import ACTIVE, FROM_NODE, TO_NODE, RHO, ETA, CP, ELEMENT_IDX, TOUTINIT
 from pandapipes.idx_node import L, node_cols, TINIT as TINIT_NODE
 from pandapipes.pf.pipeflow_setup import add_table_lookup, get_lookup, get_table_number
 from pandapipes.properties.fluids import get_fluid
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
@@ -192,36 +192,35 @@
             branch_w_internals_pit, ELEMENT_IDX, net[cls.table_name()].index.values,
             internal_pipe_number, has_internals)
         set_entry_check_repeat(
             branch_w_internals_pit, ACTIVE, net[cls.table_name()][cls.active_identifier()].values,
             internal_pipe_number, has_internals)
         branch_w_internals_pit[:, FROM_NODE] = from_nodes
         branch_w_internals_pit[:, TO_NODE] = to_nodes
-        branch_w_internals_pit[:, TINIT] = (node_pit[from_nodes, TINIT_NODE] + node_pit[
-            to_nodes, TINIT_NODE]) / 2
+        branch_w_internals_pit[:, TOUTINIT] = node_pit[to_nodes, TINIT_NODE]
+        tm = (node_pit[from_nodes, TINIT_NODE] + branch_w_internals_pit[:, TOUTINIT]) / 2
         fluid = get_fluid(net)
-        branch_w_internals_pit[:, RHO] = fluid.get_density(branch_w_internals_pit[:, TINIT])
-        branch_w_internals_pit[:, ETA] = fluid.get_viscosity(branch_w_internals_pit[:, TINIT])
-        branch_w_internals_pit[:, CP] = fluid.get_heat_capacity(branch_w_internals_pit[:, TINIT])
-
+        branch_w_internals_pit[:, RHO] = fluid.get_density(tm)
+        branch_w_internals_pit[:, ETA] = fluid.get_viscosity(tm)
+        branch_w_internals_pit[:, CP] = fluid.get_heat_capacity(tm)
         return branch_w_internals_pit, internal_pipe_number
 
     @classmethod
     def get_internal_pipe_number(cls, net):
         """
 
         :param net: The pandapipes network
         :type net: pandapipesNet
         :return:
         :rtype:
         """
         return np.array(net[cls.table_name()].sections.values)
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         raise NotImplementedError
 
     @classmethod
     def get_internal_results(cls, net, branch):
         """
 
         :param net:
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/const_flow_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/const_flow_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 from pandapipes.component_models.abstract_models.node_element_models import NodeElementComponent
 from pandapipes.idx_node import LOAD, ELEMENT_IDX
@@ -47,22 +47,20 @@
                                           mass_flow_loads)
         junction_idx_lookups = get_lookup(net, "node", "index")[
             cls.get_connected_node_type().table_name()]
         index = junction_idx_lookups[juncts]
         node_pit[index, LOAD] += loads_sum
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         """
         Function that extracts certain results.
 
-        :param nodes_connected:
-        :type nodes_connected:
-        :param branches_connected:
-        :type branches_connected:
+        :param mode:
+        :type mode:
         :param branch_results:
         :type branch_results:
         :param net: The pandapipes network
         :type net: pandapipesNet
         :param options:
         :type options:
         :return: No Output.
@@ -70,16 +68,16 @@
         res_table = net["res_" + cls.table_name()]
 
         loads = net[cls.table_name()]
 
         is_loads = loads.in_service.values
         fj, tj = get_lookup(net, "node", "from_to")[cls.get_connected_node_type().table_name()]
         junct_pit = net["_pit"]["node"][fj:tj, :]
-        nodes_connected = get_lookup(net, "node", "active")[fj:tj]
-        is_juncts = np.isin(loads.junction.values, junct_pit[nodes_connected, ELEMENT_IDX])
+        nodes_connected_hyd = get_lookup(net, "node", "active_hydraulics")[fj:tj]
+        is_juncts = np.isin(loads.junction.values, junct_pit[nodes_connected_hyd, ELEMENT_IDX])
 
         is_calc = is_loads & is_juncts
         res_table["mdot_kg_per_s"].values[is_calc] = loads.mdot_kg_per_s.values[is_calc] \
             * loads.scaling.values[is_calc]
 
     @classmethod
     def get_component_input(cls):
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/__init__.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from .base_component import *
 from .branch_models import *
 from .branch_w_internals_models import *
 from .branch_wo_internals_models import *
```

## Comparing `pandapipes-0.8.5/pandapipes/component_models/abstract_models/node_element_models.py` & `pandapipes-0.9.0/src/pandapipes/component_models/abstract_models/node_element_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.component_models.abstract_models.base_component import Component
 
 try:
     import pandaplan.core.pplog as logging
@@ -47,9 +47,9 @@
         :param node_pit:
         :type node_pit:
         :return: No Output.
         """
         raise NotImplementedError
 
     @classmethod
-    def extract_results(cls, net, options, branch_results, nodes_connected, branches_connected):
+    def extract_results(cls, net, options, branch_results, mode):
         raise NotImplementedError
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/multinet.py` & `pandapipes-0.9.0/src/pandapipes/multinet/multinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import pandas as pd
 from numpy import dtype
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/__init__.py` & `pandapipes-0.9.0/src/pandapipes/multinet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes.multinet.control.controller import *
 from pandapipes.multinet.control.run_control_multinet import run_control
 from pandapipes.multinet.timeseries.run_time_series_multinet import run_timeseries
 from pandapipes.multinet.create_multinet import *
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/create_multinet.py` & `pandapipes-0.9.0/src/pandapipes/multinet/create_multinet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 from pandapipes.multinet.multinet import MultiNet, get_default_multinet_structure
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
-logger.setLevel(level=logging.WARNING)
 
 
 def create_empty_multinet(name=""):
     """
     This function initializes the multinet datastructure.
 
     :param name: Name for the multi net
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/control/run_control_multinet.py` & `pandapipes-0.9.0/src/pandapipes/multinet/control/run_control_multinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 
 import pandapipes as ppipes
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/control/controller/multinet_control.py` & `pandapipes-0.9.0/src/pandapipes/multinet/control/controller/multinet_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapower.control import ConstControl
 from pandapipes.properties.fluids import get_fluid
 from pandapower.control.basic_controller import Controller
 from pandas.errors import InvalidIndexError
```

## Comparing `pandapipes-0.8.5/pandapipes/multinet/timeseries/run_time_series_multinet.py` & `pandapipes-0.9.0/src/pandapipes/multinet/timeseries/run_time_series_multinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import tqdm
+from pandapipes.multinet.control.run_control_multinet import prepare_run_ctrl, run_control
+from pandapipes.timeseries.run_time_series import init_default_outputwriter as init_default_ow_pps
 from pandapower import pandapowerNet
 from pandapower.control.util.diagnostic import control_diagnostic
 from pandapower.timeseries.run_time_series import get_recycle_settings, init_time_steps, \
     output_writer_routine, cleanup, run_loop, init_default_outputwriter as init_default_ow_pp, \
     init_output_writer
 
 from pandapipes import pandapipesNet
-from pandapipes.multinet.control.run_control_multinet import prepare_run_ctrl, run_control
-from pandapipes.timeseries.run_time_series import init_default_outputwriter as init_default_ow_pps
 
 try:
     import pandaplan.core.pplog as pplog
 except ImportError:
     import logging as pplog
 
 logger = pplog.getLogger(__name__)
-logger.setLevel(level=pplog.WARNING)
 
 
 def _call_output_writer(multinet, time_step, pf_converged, ctrl_converged, ts_variables):
     """
     Calling the output writer routine for each net in multinet.
 
     :param multinet: multinet with multinet controllers, net distinct controllers and several pandapipes/pandapower nets
@@ -37,15 +36,16 @@
     :param ts_variables: contains all relevant information and boundaries required for time series and control analyses
     :type ts_variables: dict
     :return: calling each output writer in order to save the results which are retrieved
     :rtype: None
     """
     for net_name in multinet['nets'].keys():
         net = multinet['nets'][net_name]
-        output_writer_routine(net, time_step, pf_converged, ctrl_converged, ts_variables['nets'][net_name]["recycle_options"])
+        output_writer_routine(net, time_step, pf_converged, ctrl_converged,
+                              ts_variables['nets'][net_name]["recycle_options"])
 
 
 def init_time_series(multinet, time_steps, continue_on_divergence=False, verbose=True,
                      **kwargs):
     """
     Initializes the time series calculation.
     Besides it creates the dict ts_variables, which includes necessary variables for the time series / control loop.
@@ -77,15 +77,16 @@
             init_default_ow_pps(net, time_steps, **kwargs)
         else:
             raise ValueError('the given nets are neither pandapipes nor pandapower nets')
         recycle_options = None
         if hasattr(run, "__name__") and run.__name__ == "runpp":
             # use faster runpp options if possible
             recycle_options = get_recycle_settings(net, **kwargs)
-        ts_variables['nets'][net_name]['run'] = run[net_name] if run is not None else ts_variables['nets'][net_name]['run']
+        ts_variables['nets'][net_name]['run'] = run[
+            net_name] if run is not None else ts_variables['nets'][net_name]['run']
         ts_variables['nets'][net_name]['recycle_options'] = recycle_options
         init_output_writer(net, time_steps)
 
     # time steps to be calculated (list or range)
     ts_variables["time_steps"] = time_steps
     # If True, a diverged run is ignored and the next step is calculated
     ts_variables["continue_on_divergence"] = continue_on_divergence
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/data_cleaning.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/data_cleaning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 import os
 
 import numpy as np
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/stanet2pandapipes.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/stanet2pandapipes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 
 from pandapipes.converter.stanet.preparing_steps import get_net_params, get_pipe_geo, \
     connection_pipe_section_table, get_stanet_raw_data, create_meter_table, create_house_table
 from pandapipes.converter.stanet.table_creation import create_junctions_from_nodes, \
     create_valve_and_pipe, create_pumps, create_junctions_from_connections, \
-    create_pipes_from_connections, create_heat_exchangers, create_slider_valves, \
+    create_pipes_from_connections, create_heat_exchangers_stanet, create_slider_valves, \
     create_pipes_from_remaining_pipe_table, create_nodes_house_connections, \
     create_sinks_meters, create_sinks_from_nodes, create_control_components, \
     create_sinks_from_customers, create_pipes_house_connections
 from pandapipes.create import create_empty_network
 
 try:
     import pandaplan.core.pplog as logging
@@ -27,15 +27,16 @@
 #         - in case of house connection calculation in STANET, the connections have results VMA and
 #           VMB. These results can be used for comparison, but also for sorting of connections on a
 #           main pipe --> especially if connection nodes on the main pipe have the same coordinates.
 #         - some TODOs in table_creation
 #         - maybe it will be necessary to remove deleted data from the STANET tables, otherwise they
 #           might be inserted into the pandapipes net erroneously
 def stanet_to_pandapipes(stanet_path, name="net", remove_unused_household_connections=True,
-                         stanet_like_valves=False, read_options=None, add_layers=True, **kwargs):
+                         stanet_like_valves=False, read_options=None, add_layers=True,
+                         guess_slider_valve_types=False, **kwargs):
     """Converts STANET csv-file to pandapipesNet.
 
     :param stanet_path: path to csv-file exported from STANET
     :type stanet_path: str
     :param name: name for the created network
     :type name: str, default "net"
     :param remove_unused_household_connections: if True, the intermediate nodes on pipes that are \
@@ -46,14 +47,17 @@
     :type stanet_like_valves: bool, default False
     :param read_options: Additional kwargs for the tables to be read with pd.read_csv. If None, no\
             kwargs will be handed over.
     :type read_options: dict, default None
     :param add_layers: If True, adds information on layers of different components if provided by \
             STANET
     :type add_layers: bool, default True
+    :param guess_slider_valve_types: If set to True, the slider valve status (opened / closed) is \
+            guessed based on the logic "even number = opened; odd number = closed".
+    :type guess_slider_valve_types: bool, default False
     :return: net
     :rtype: pandapipesNet
     """
     net = create_empty_network(name=name)
 
     # stored_data contains different dataframes read from the STANET CSV file for different
     # components, such as junctions, pipes etc., but in the raw STANET form
@@ -88,21 +92,22 @@
     create_pipes_from_connections(net, stored_data, connections, index_mapping, pipe_geodata,
                                   add_layers)
 
     # create pipes, while considering already created pipe sections
     create_pipes_from_remaining_pipe_table(net, stored_data, connections, index_mapping,
                                            pipe_geodata, add_layers)
 
-    create_heat_exchangers(net, stored_data, connections, index_mapping, add_layers)
+    create_heat_exchangers_stanet(net, stored_data, index_mapping, add_layers,
+                                  add_flow=kwargs.pop("add_heat_exchanger_flow", False))
 
     # valves always have a length in STANET, therefore, they are created as valve with pipe in
     # pandapipes
     create_valve_and_pipe(net, stored_data, index_mapping, net_params, stanet_like_valves, add_layers)
 
-    create_slider_valves(net, stored_data, index_mapping, add_layers)
+    create_slider_valves(net, stored_data, index_mapping, add_layers, guess_slider_valve_types)
 
     if "pumps_water" in stored_data:
         create_pumps(net, stored_data['pumps_water'], index_mapping, add_layers)
 
     if "pumps_gas" in stored_data:
         create_pumps(net, stored_data['pumps_gas'], index_mapping, add_layers)
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/preparing_steps.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/preparing_steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from itertools import chain, product
 
 import numpy as np
 import pandas as pd
@@ -21,14 +21,36 @@
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
 
 
+DEFAULT_STANET_KEYWORDS = {
+    "pipes": ['REM Leitungsdaten'],
+    "house_pipes": ['REM HA Leitungsdaten'],
+    "nodes": ['REM Knotendaten'],
+    "house_nodes": ["REM HA Knotendaten"],
+    "valves": ['REM Ventiledaten'],
+    "pumps_gas": ['REM Kompressorendaten'],
+    "pumps_water": ['REM Pumpendaten'],
+    "net_parameters": ['REM Netzparameterdaten'],
+    "houses": ["REM Hausdaten"],
+    "house_connections": ["REM HA Verbindungsdaten"],
+    "meters": ["REM HA Zählerdaten"],
+    "controllers": ["REM Reglerdaten"],
+    "slider_valves": ["REM Schieberdaten"],
+    "inflexion_points": ["REM Knickpunktdaten"],
+    "heat_exchangers": ["REM Wärmetauscherdaten"],
+    "customers": ["REM Abnehmerdaten"],
+    "house_inflexion_points": ["REM HA Knickpunktdaten"],
+    "layers": ["REM Layerdaten"]
+}
+
+
 def get_stanet_raw_data(stanet_path, read_options=None, add_layers=True, return_line_info=False,
                         keywords=None):
     """
     Extract raw data from STANET file.
     :param stanet_path:  Path to STANET .csv file
     :type stanet_path: string
     :param read_options:
@@ -48,32 +70,15 @@
         # the following rule:
         # 1st line: keyword (e.g. "REM Leitungsdaten")
         # 2nd line: human-readable header of table
         # 3rd line: units
         # 4th line: STANET internal header of table (this is the first line to convert to pandas
         #           dataframe and return to the converter)
         # everything until the next empty line will be added to the dataframe
-        keywords = {"pipes": ['REM Leitungsdaten'],
-                    "house_pipes": ['REM HA Leitungsdaten'],
-                    "nodes": ['REM Knotendaten'],
-                    "house_nodes": ["REM HA Knotendaten"],
-                    "valves": ['REM Ventiledaten'],
-                    "pumps_gas": ['REM Kompressorendaten'],
-                    "pumps_water": ['REM Pumpendaten'],
-                    "net_parameters": ['REM Netzparameterdaten'],
-                    "houses": ["REM Hausdaten"],
-                    "house_connections": ["REM HA Verbindungsdaten"],
-                    "meters": ["REM HA Zählerdaten"],
-                    "controllers": ["REM Reglerdaten"],
-                    "slider_valves": ["REM Schieberdaten"],
-                    "inflexion_points": ["REM Knickpunktdaten"],
-                    "heat_exchangers": ["REM Wärmetauscherdaten"],
-                    "customers": ["REM Abnehmerdaten"],
-                    "house_inflexion_points": ["REM HA Knickpunktdaten"],
-                    "layers": ["REM Layerdaten"]}
+        keywords = DEFAULT_STANET_KEYWORDS
     stored_data = dict()
 
     logger.info("Reading STANET csv-file.")
     # read full csv file
     read_line_info = dict()
     encoding = read_options.get("encoding", "cp1252")
     with open(stanet_path, 'rt', encoding=encoding) as f:
@@ -226,17 +231,17 @@
 
 def adapt_pipe_data_according_to_nodes(pipe_data, pipes_to_check, node_geo, pipe_rec, is_x,
                                        is_start, node_type, node_cols, coord_names):
     node_name = "XRECHTS" if is_x else "YHOCH"
     coord = "x" if is_x else "y"
     locat = "from" if is_start else "to"
     run = 0 if is_x else 2
-    run += 0 if is_start else 1
+    run += 1 - int(is_start)
     pipe_name = coord_names[run]
-    node_nr = node_cols[0] if is_start else node_cols[1]
+    node_nr = node_cols[1 - int(is_start)]
     node_val = node_geo.loc[pipe_data.loc[pipes_to_check, node_nr].values, node_name].values
 
     if pipe_name not in pipe_data.columns:
         pipe_data[pipe_name] = np.NaN
         pipe_data.loc[pipes_to_check, pipe_name] = node_val
     current_pipe_data = pipe_data.loc[pipes_to_check]
     if not np.allclose(node_val, current_pipe_data[pipe_name].values):
@@ -269,15 +274,15 @@
         node_data = stored_data[node_name]
         node_geo = node_data.loc[:, ["XRECHTS", "YHOCH"]]
         node_geo.index = node_data.RECNO.values
         node_cols = ["CLIENTNO", "CLIENT2NO"] if use_clients else ["ANFNR", "ENDNR"]
 
         # the following code is just a check whether pipe and node geodata fit together
         # in case of deviations, the pipe geodata is adapted on the basis of the node geodata
-        pipe_rec = pipe_data.RECNO.values
+        pipe_rec = pipe_data.index.values
         for is_x, is_start in product([True, False], [True, False]):
             current_index_range = indices[0] if is_start else indices[1]
             current_pipe_nums = pipe_rec[current_index_range.values]
             adapt_pipe_data_according_to_nodes(
                 pipe_data, current_index_range, node_geo, current_pipe_nums, is_x, is_start,
                 node_name, node_cols, coord_names
             )
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/table_creation.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/table_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from itertools import chain
 
 import numpy as np
 import pandas as pd
@@ -62,14 +62,16 @@
     node_table = stored_data["nodes"]
     stanet_nrs = node_table.RECNO.astype(np.int32)
     knams = node_table.KNAM.astype(str).values
     add_info = {"stanet_id": node_table.STANETID.astype(str).values
                 if "STANETID" in node_table.columns else knams,
                 "p_stanet": node_table.PRECH.values.astype(np.float64),
                 "stanet_valid": ~node_table.CALCBAD.values.astype(np.bool_)}
+    if "TEMP" in node_table.columns:
+        add_info["t_stanet"] = node_table.TEMP.values.astype(np.float64)
     if hasattr(node_table, "KFAK"):
         add_info["K_stanet"] = node_table.KFAK.values.astype(np.float64)
     if add_layers:
         add_info["stanet_layer"] = node_table.LAYER.values.astype(str)
     temperatures = pd.Series(net_params["medium_temp_K"], index=node_table.index, dtype=np.float64)
     eg_ind = ((node_table.FSTATUS == '?') & (node_table.DSTATUS == '!')).values
     eg_temps = node_table.loc[eg_ind, "TMESS"].values + 273.15
@@ -148,87 +150,116 @@
             j_ref_geodata = net.junction_geodata.loc[node_mapping[from_stanet_nr], :]
             j_aux = pandapipes.create_junction(
                 net, np.NaN, tfluid_k=net_params["medium_temp_K"], height_m=j_ref['height_m'],
                 name='aux_' + j_ref['stanet_id'], geodata=(j_ref_geodata.x, j_ref_geodata.y),
                 stanet_nr=-999, stanet_id='aux_' + j_ref['stanet_id'], p_stanet=np.NaN,
                 stanet_active=bool(row.ISACTIVE), **add_info
             )
+            text_k = 293
+            if hasattr(row, "TU"):
+                text_k = row.TU + 273.15
             pandapipes.create_pipe_from_parameters(
                 net, node_mapping[from_stanet_nr], j_aux, length_km=row.RORL / 1000,
                 diameter_m=float(row.DM / 1000), k_mm=row.RAU, loss_coefficient=row.ZETA,
                 name="pipe_%s_%s" % (str(row.ANFNAM), 'aux_' + str(row.ENDNAM)),
-                in_service=bool(row.ISACTIVE), stanet_nr=-999,
+                text_k=text_k, in_service=bool(row.ISACTIVE), stanet_nr=-999,
                 stanet_id='pipe_valve_' + str(row.STANETID), v_stanet=row.VM,
                 stanet_active=bool(row.ISACTIVE), stanet_valid=False, **add_info
             )
             pandapipes.create_valve(
                 net, j_aux, node_mapping[to_stanet_nr], diameter_m=float(row.DM / 1000),
                 opened=row.AUF == 'J', loss_coefficient=0,
                 name="valve_%s_%s" % ('aux_' + str(row.ENDNAM), str(row.ENDNAM)),
                 stanet_nr=int(row.RECNO), stanet_id=str(row.STANETID), v_stanet=np.NaN,
                 stanet_active=bool(row.ISACTIVE), **add_info
             )
 
 
-def create_slider_valves(net, stored_data, index_mapping, add_layers):
+def create_slider_valves(net, stored_data, index_mapping, add_layers,
+                         guess_opened_from_types=False):
     """
     Creates pandapipes slider valves from STANET data.
-    :param net:
-    :type net:
-    :param stored_data:
-    :type stored_data:
-    :param index_mapping:
-    :type index_mapping:
-    :param add_layers:
-    :type add_layers:
-    :return:
-    :rtype:
+
+    :param net: pandapipes net to which to add slider valves
+    :type net: pandapipesNet
+    :param stored_data: dictionary of STANET element tables
+    :type stored_data: dict
+    :param index_mapping: dictionary of mappings between STANET and pandapipes indices
+    :type index_mapping: dict
+    :param add_layers: if True, the layer info will be added to the slider valve table
+    :type add_layers: bool
+    :param guess_opened_from_types: if True, the status of slider valves with unknown types is \
+        guessed based on the logic "even type number = opened, odd type number = closed"
+    :type guess_opened_from_types: bool, default False
+    :return: No output
+    :rtype: None
     """
-    if "slider_valves" not in stored_data:
+    if "slider_valves" not in stored_data and "house_slider_valves" not in stored_data:
         return
     logger.info("Creating all slider valves.")
-    slider_valves = stored_data["slider_valves"]
 
-    # identify all junctions that are connected on each side of the slider valves
-    svf = index_mapping["slider_valves_from"]
-    svt = index_mapping["slider_valves_to"]
-    from_junctions = np.array([svf[sv] for sv in slider_valves.RECNO.values])
-    to_junctions = np.array([svt[sv] for sv in slider_valves.RECNO.values])
-
-    # these types can be converted to normal valves
-    # --> there are many types of slider valves in STANET, the behavior is not always clear, so
-    #     if you want to convert another type, identify the correct valve behavior in pandapipes
-    #     that matches this type.
-    opened_sv = [2, 6, 10, 18]
-    closed_sv = [3, 7, 11, 19]
-    opened_types = {o: True for o in opened_sv}
-    opened_types.update({c: False for c in closed_sv})
-    sv_types = set(slider_valves.TYP.values.astype(np.int32))
-    if len(sv_types - set(opened_types.keys())):
-        raise UserWarning("The slider valve types %s cannot be converted."
-                          % (sv_types - set(opened_types.keys())))
+    for tbl_name in ("slider_valves", "house_slider_valves"):
+        if tbl_name not in stored_data:
+            continue
+        slider_valves = stored_data[tbl_name]
+
+        # identify all junctions that are connected on each side of the slider valves
+        svf = index_mapping["slider_valves_from"]
+        svt = index_mapping["slider_valves_to"]
+        from_junctions = np.array([svf[sv] for sv in slider_valves.RECNO.values])
+        to_junctions = np.array([svt[sv] for sv in slider_valves.RECNO.values])
+
+        # these types can be converted to normal valves
+        # --> there are many types of slider valves in STANET, the behavior is not always clear, so
+        #     if you want to convert another type, identify the correct valve behavior in pandapipes
+        #     that matches this type.
+        opened_sv = [2, 6, 10, 18]
+        closed_sv = [3, 7, 11, 19]
+        # TODO: Is it possible that there is always a "CONNECTED" column and it says whether the
+        #       valve is opened or closed? Maybe the type is only used for graphical purpose.
+        opened_types = {o: True for o in opened_sv}
+        opened_types.update({c: False for c in closed_sv})
+        sv_types = set(slider_valves.TYP.values.astype(np.int32))
+        if len(sv_types - set(opened_types.keys())):
+            if guess_opened_from_types:
+                logger.warning(
+                    "The slider valve types %s are not (yet) known. Their status (opened/closed) "
+                    "will be guessed based on the logic: even number = opened, odd number = closed."
+                    % (sv_types - set(opened_types.keys()))
+                )
+                opened_types.update(
+                    {t: bool(t % 2 + 1) for t in sv_types - set(opened_types.keys())}
+                )
+            else:
+                raise UserWarning("The slider valve types %s cannot be converted."
+                                  % (sv_types - set(opened_types.keys())))
 
-    # create all slider valves --> most important are the opened and loss_coefficient entries
-    valve_system = slider_valves.CLIENTTYP.replace(CLIENT_TYPES_OF_PIPES).values
-    add_info = dict()
-    if add_layers:
-        add_info["stanet_layer"] = slider_valves.LAYER.values.astype(str)
-    # account for sliders with diameter 0 m
-    if any(slider_valves.DM == 0):
-        logger.warning(f"{sum(slider_valves.DM == 0)} sliders have a inner diameter of 0 m! "
-                       f"The diameter will be set to 1 m.")
-        slider_valves.DM[slider_valves.DM == 0] = 1e3
-    pandapipes.create_valves(
-        net, from_junctions, to_junctions, slider_valves.DM.values / 1000,
-        opened=slider_valves.TYP.astype(np.int32).replace(opened_types).values,
-        loss_coefficient=slider_valves.ZETA.values, name=slider_valves.STANETID.values,
-        type="slider_valve_" + valve_system, stanet_nr=slider_valves.RECNO.values.astype(np.int32),
-        stanet_id=slider_valves.STANETID.values.astype(str), stanet_system=valve_system,
-        stanet_active=slider_valves.ISACTIVE.values.astype(np.bool_), **add_info
-    )
+        # create all slider valves --> most important are the opened and loss_coefficient entries
+        valve_system = slider_valves.CLIENTTYP.replace(CLIENT_TYPES_OF_PIPES).values
+        add_info = dict()
+        if add_layers:
+            add_info["stanet_layer"] = slider_valves.LAYER.values.astype(str)
+        # account for sliders with diameter 0 m
+        if "DM" not in slider_valves.columns:
+            logger.warning(f"The table {tbl_name} does not contain the slider valve inner diameter!"
+                           f"The diameter will be set to 1 m.")
+            slider_valves["DM"] = 1e3
+        if any(slider_valves.DM == 0):
+            logger.warning(f"{sum(slider_valves.DM == 0)} sliders have an inner diameter of 0 m! "
+                           f"The diameter will be set to 1 m.")
+            slider_valves.DM[slider_valves.DM == 0] = 1e3
+        pandapipes.create_valves(
+            net, from_junctions, to_junctions, slider_valves.DM.values / 1000,
+            opened=slider_valves.TYP.astype(np.int32).replace(opened_types).values,
+            loss_coefficient=slider_valves.ZETA.values, name=slider_valves.STANETID.values,
+            type="slider_valve_" + valve_system,
+            stanet_nr=slider_valves.RECNO.values.astype(np.int32),
+            stanet_id=slider_valves.STANETID.values.astype(str), stanet_system=valve_system,
+            stanet_active=slider_valves.ISACTIVE.values.astype(np.bool_), **add_info
+        )
 
 
 # noinspection PyTypeChecker
 def create_pumps(net, pump_table, index_mapping, add_layers):
     """
     Creates pandapipes pumps from STANET data.
     :param net:
@@ -309,15 +340,15 @@
     if not all([np.all((control_table[col] == "J") | (control_table[col] == "N"))
                 for col in ["OFFEN", "ZU", "AKTIV"]]):
         logger.warning("There is an error in the control table! Please check the columns 'OFFEN',"
                        " 'ZU' and 'AKTIV', which should only contain 'J' or 'N'.")
 
     control_active = (control_table.AKTIV.values == "J").astype(np.bool_)
     if consider_controlled:
-        control_active &= fully_open
+        control_active &= ~fully_open
     in_service = control_table.ISACTIVE.values.astype(np.bool_)
     if consider_controlled:
         in_service &= ~(control_table.ZU.values == "J")
 
     is_pc = control_table.RTYP.values == "P"
     is_fc = control_table.RTYP.values == "Q"
     if not np.all(is_pc | is_fc):
@@ -390,15 +421,15 @@
     Returns the connection types contained in the STANET raw values.
 
     :param connection_table: table of connections on pipes
     :type connection_table: pd.DataFrame
     :return:
     :rtype:
     """
-    extend_from_to = ["slider_valves"]
+    extend_from_to = ["slider_valves", "house_slider_valves"]
     connection_types = list(chain.from_iterable([
         [(ct, ct)] if ct not in extend_from_to else [(ct, ct + "_from"), (ct, ct + "_to")]
         for ct in set(connection_table.type)
     ]))
     return extend_from_to, connection_types
 
 
@@ -424,14 +455,16 @@
     houses_in_calculation = net_params["household_results_valid"]
     # there are two types of connections: those that require just one additional junction and those
     # that require two additional junctions (inserting a branch component there), which is why we
     # need "from" and "to" junctions for those connection types
     extend_from_to, connection_types = get_connection_types(connection_table)
     for con_type, node_type in connection_types:
         cons = connection_table.loc[connection_table.type == con_type]
+        if cons.empty:
+            continue
         stanet_ids = cons.STANETID.astype(str).values
         stanet_nrs = cons.RECNO.astype(np.int32).values
         p_stanet = cons.PRECH.astype(np.float64).values if houses_in_calculation else np.NaN
         names = stanet_ids if con_type not in extend_from_to else \
             stanet_ids + node_type.replace(con_type, "")
         geo = np.array([cons.geo.apply(lambda g: g[0]), cons.geo.apply(lambda g: g[1])]).transpose()
         in_service = np.array([True] * len(cons))
@@ -555,50 +588,56 @@
     pipe_sections["section_geo"] = pipe_sections.apply(create_geodata_sections, axis=1)
 
     pipes = pipe_data.loc[pipe_numbers, :]
     add_info = dict()
     if add_layers:
         add_info["stanet_layer"] = pipes.LAYER.values.astype(str)
     # TODO: v_stanet might have to be extended by house connections VMA and VMB
+    text_k = 293
+    if "TU" in pipes.columns:
+        text_k = pipes.TU.values.astype(np.float64) + 273.15
+    alpha = 0
+    if "WDZAHL" in pipes.columns:
+        alpha = pipes.WDZAHL.values.astype(np.float64)
     pandapipes.create_pipes_from_parameters(
         net, pipe_sections.fj.values, pipe_sections.tj.values, pipe_sections.length.values / 1000,
         pipes.DM.values / 1000, pipes.RAU.values, pipes.ZETA.values, type="main_pipe",
-        stanet_std_type=pipes.ROHRTYP.values, in_service=pipes.ISACTIVE.values,
+        stanet_std_type=pipes.ROHRTYP.values, in_service=pipes.ISACTIVE.values, text_k=text_k,
+        alpha_w_per_m2k=alpha,
         name=["pipe_%s_%s_%s" % (nf, nt, sec) for nf, nt, sec in zip(
             pipes.ANFNAM.values, pipes.ENDNAM.values, pipe_sections.section_no.values)],
         stanet_nr=pipes.RECNO.values, stanet_id=pipes.STANETID.values,
         geodata=pipe_sections.section_geo.values, v_stanet=pipe_sections.vm.values,
         stanet_system=CLIENT_TYPES_OF_PIPES[MAIN_PIPE_TYPE],
         stanet_active=pipes.ISACTIVE.values.astype(np.bool_),
         stanet_valid=~pipes.CALCBAD.values.astype(np.bool_),
         **add_info
     )
 
 
-def create_heat_exchangers(net, stored_data, connection_table, index_mapping, add_layers):
+def create_heat_exchangers_stanet(net, stored_data, index_mapping, add_layers, add_flow=False):
     """
     Creates pandapipes heat exchangers from STANET connections.
     :param net:
     :type net:
     :param stored_data:
     :type stored_data:
-    :param connection_table:
-    :type connection_table:
     :param index_mapping:
     :type index_mapping:
     :param add_layers:
     :type add_layers:
+    :param add_flow:
+    :type add_flow:
     :return:
     :rtype:
     """
     if "heat_exchangers" not in stored_data:
         return
-    heat_ex_table = stored_data["heat_exchangers"]
+    heat_exchanger = stored_data["heat_exchangers"]
     logger.info("Creating all heat exchangers.")
-    heat_exchanger = heat_ex_table.loc[~heat_ex_table.RECNO.isin(connection_table.SNUM.values)]
     node_mapping = index_mapping["nodes"]
 
     for row in heat_exchanger.itertuples():
         ex_name = str(row.STANETID)
         from_stanet_nr, to_stanet_nr = int(row.ANFNR), int(row.ENDNR)
         from_name, to_name = str(row.ANFNAM), str(row.ENDNAM)
         contained = [from_stanet_nr in node_mapping, to_stanet_nr in node_mapping]
@@ -612,18 +651,23 @@
                                " %s (%d) is missing in the pandapipes net."
                                % (ex_name, to_name, to_stanet_nr))
             continue
 
         add_info = dict()
         if add_layers:
             add_info["stanet_layer"] = str(row.LAYER)
+        if add_flow:
+            add_info["flow_stanet"] = row.FLUSS
+        qext = 0
+        if hasattr(row, "WAERMECALC"):
+            qext = getattr(row, "WAERMECALC") * (-1000)
         # TODO: there is no qext given!!!
         pandapipes.create_heat_exchanger(
-            net, node_mapping[from_stanet_nr], node_mapping[to_stanet_nr], qext_w=0,
-            diameter_m=float(row.DM / 1000), loss_coefficient=row.ZETA, std_type=row.ROHRTYP,
+            net, node_mapping[from_stanet_nr], node_mapping[to_stanet_nr], qext_w=qext,
+            diameter_m=float(row.DM / 1000), loss_coefficient=row.ZETA,
             in_service=bool(row.ISACTIVE), name="heat_exchanger_%s_%s" % (row.ANFNAM, row.ENDNAM),
             stanet_nr=int(row.RECNO), stanet_id=str(row.STANETID), v_stanet=row.VM,
             stanet_active=bool(row.ISACTIVE), **add_info
         )
 
 
 def create_pipes_from_remaining_pipe_table(net, stored_data, connection_table, index_mapping,
@@ -675,54 +719,65 @@
     from_junctions = [node_mapping[jn] for jn in from_stanet_nr[valid]]
     to_junctions = [node_mapping[jn] for jn in to_stanet_nr[valid]]
     p_tbl = remaining_pipes.loc[valid, :]
     geodata = pipe_geodata.loc[p_tbl.RECNO.values].values
     add_info = dict()
     if add_layers:
         add_info["stanet_layer"] = p_tbl.LAYER.values.astype(str)
+    text_k = 293
+    if "TU" in p_tbl.columns:
+        text_k = p_tbl.TU.values.astype(np.float64) + 273.15
+    alpha = 0
+    if "WDZAHL" in p_tbl.columns:
+        alpha = p_tbl.WDZAHL.values.astype(np.float64)
     pandapipes.create_pipes_from_parameters(
         net, from_junctions, to_junctions, length_km=p_tbl.RORL.values.astype(np.float64) / 1000,
         type="main_pipe", diameter_m=p_tbl.DM.values.astype(np.float64) / 1000,
         loss_coefficient=p_tbl.ZETA.values, stanet_std_type=p_tbl.ROHRTYP.values,
         k_mm=p_tbl.RAU.values, in_service=p_tbl.ISACTIVE.values.astype(np.bool_),
         name=["pipe_%s_%s" % (anf, end) for anf, end in zip(from_names[valid], to_names[valid])],
-        stanet_nr=p_tbl.RECNO.values.astype(np.int32),
+        alpha_w_per_m2k=alpha, text_k=text_k, stanet_nr=p_tbl.RECNO.values.astype(np.int32),
         stanet_id=p_tbl.STANETID.values.astype(str), v_stanet=p_tbl.VM.values, geodata=geodata,
         stanet_system=CLIENT_TYPES_OF_PIPES[MAIN_PIPE_TYPE],
         stanet_active=p_tbl.ISACTIVE.values.astype(np.bool_),
         stanet_valid=~p_tbl.CALCBAD.values.astype(np.bool_),
         **add_info
     )
 
 
-def check_connection_client_types(hh_pipes, all_client_types, node_client_types):
+def check_connection_client_types(hh_pipes, all_client_types, node_client_types,
+                                  fail_on_connection_check=True):
     # create pipes for household connections (from house to supply pipe), which is a separate table
     # in the STANET CSV file
     # --> there are many ways how household connections can be created in STANET,
     # therefore this approach might not be sufficient for new data sets, please verify your
     # output network
     if not np.all(hh_pipes.CLIENTTYP.isin(all_client_types)):
         raise UserWarning("The connection types %s can not all be converted for house connections "
                           "pipes." % set(hh_pipes.CLIENTTYP))
     if not np.all(hh_pipes.CLIENT2TYP.isin(all_client_types)):
         raise UserWarning("The connection types %s can not all be converted for house connections "
                           "pipes." % set(hh_pipes.CLIENT2TYP))
     clientnodetype = hh_pipes.CLIENTTYP.isin(node_client_types)
     client2nodetype = hh_pipes.CLIENT2TYP.isin(node_client_types)
     if not np.all(clientnodetype | client2nodetype):
-        raise UserWarning(
-            f"One of the household connection sides must be connected to a node (type {NODE_TYPE} element)\n"
-            f"or a connection (type {HOUSE_CONNECTION_TYPE} element with ID CON...) "
-            f"or a house node (type {HOUSE_CONNECTION_TYPE} element). \n"
-            f"Please check that the input data is correct. \n"
-            f"Check these CLIENTTYP / CLIENT2TYP: "
-            f"{set(hh_pipes.loc[~clientnodetype, 'CLIENTTYP'].values) | set(hh_pipes.loc[~client2nodetype, 'CLIENT2TYP'].values)} "
-            f"in the HA LEI table (max. 10 entries shown): \n "
-            f"{hh_pipes.loc[~clientnodetype & ~client2nodetype].head(10)}"
-            )
+        not_node_type = (set(hh_pipes.loc[~clientnodetype, 'CLIENTTYP'].values)
+                         | set(hh_pipes.loc[~client2nodetype, 'CLIENT2TYP'].values))
+        msg = (f"One of the household connection sides must be connected to a node (type "
+               f"{NODE_TYPE} element)\n or a connection (type {HOUSE_CONNECTION_TYPE} element with"
+               f" ID CON...) or a house node (type {HOUSE_CONNECTION_TYPE} element). \n"
+               f"Please check that the input data is correct. \n"
+               f"Check these CLIENTTYP / CLIENT2TYP: "
+               f"{not_node_type} in the HA LEI table (max. 10 entries shown): \n"
+               f"{hh_pipes.loc[~clientnodetype & ~client2nodetype].head(10)}")
+        if fail_on_connection_check:
+            raise UserWarning(msg)
+        else:
+            logger.warning(f"{msg} \nWill ignore this error and continue net setup, please check "
+                           f"your network configuration carefully!")
     return clientnodetype, client2nodetype
 
 
 def build_house_junctions(net, index_mapping, hh_types, hh_recno, house_table, meter_table,
                           node_table, net_params, houses_in_calculation, add_layers):
     client_is_house = hh_types == HOUSE_TYPE
     if np.any(client_is_house):
@@ -986,23 +1041,29 @@
     hp_data.loc[has_con, "section_geo"] = hp_data.loc[has_con].apply(create_geodata_sections,
                                                                      axis=1)
 
     add_info = dict()
     if add_layers:
         add_info["stanet_layer"] = hp_data.LAYER.values.astype(str)
     # TODO: v_stanet might have to be extended by house connections VMA and VMB
+    text_k = 293
+    if "TU" in hp_data.columns:
+        text_k = hp_data.TU.values.astype(np.float64) + 273.15
+    alpha = 0
+    if "WDZAHL" in hp_data.columns:
+        alpha = hp_data.WDZAHL.values.astype(np.float64)
     pandapipes.create_pipes_from_parameters(
         net, hp_data.fj.values, hp_data.tj.values, hp_data.length.values / 1000,
         hp_data.DM.values / 1000, hp_data.RAU.values, hp_data.ZETA.values, type="house_pipe",
-        stanet_std_type=hp_data.ROHRTYP.values,
-        in_service=hp_data.ISACTIVE.values if houses_in_calculation else False,
+        in_service=hp_data.ISACTIVE.values if houses_in_calculation else False, text_k=text_k,
+        alpha_w_per_m2k=alpha, geodata=hp_data.section_geo.values,
         name=["pipe_%s_%s_%s" % (nf, nt, sec) for nf, nt, sec in zip(
             hp_data.CLIENTID.values, hp_data.CLIENT2ID.values, hp_data.section_no.values)],
-        stanet_nr=hp_data.RECNO.values, stanet_id=hp_data.STANETID.values,
-        geodata=hp_data.section_geo.values, v_stanet=hp_data.VM.values,
+        stanet_std_type=hp_data.ROHRTYP.values, stanet_nr=hp_data.RECNO.values,
+        stanet_id=hp_data.STANETID.values, v_stanet=hp_data.VM.values,
         stanet_active=hp_data.ISACTIVE.values.astype(np.bool_),
         stanet_valid=houses_in_calculation, **add_info
     )
 
 
 def create_sinks_meters(net, meter_table, index_mapping, net_params, add_layers):
     """
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import dtype
 
 from pandapipes.component_models.junction_component import Junction
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from functools import partial
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py` & `pandapipes-0.9.0/src/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapower.create import _get_index_with_check, load_std_type, _set_entries
 
 from pandapipes.component_models.component_toolbox import add_new_component
 from pandapipes.converter.stanet.valve_pipe_component.valve_pipe_component import ValvePipe
```

## Comparing `pandapipes-0.8.5/pandapipes/io/file_io.py` & `pandapipes-0.9.0/src/pandapipes/io/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import json
 import os
 import pickle
 from functools import partial
@@ -146,16 +146,15 @@
 
         >>> net = pandapipes.from_json_string(json_str)
 
     """
     if encryption_key is not None:
         json_string = decrypt_string(json_string, encryption_key)
 
-    net = json.loads(json_string, cls=PPJSONDecoder,
-                     object_hook=partial(pp_hook, registry_class=FromSerializableRegistryPpipe))
+    net = json.loads(json_string, cls=PPJSONDecoder, registry_class=FromSerializableRegistryPpipe)
 
     if convert and isinstance(net, pandapipesNet):
         convert_format(net)
     elif convert and isinstance(net, MultiNet):
         for n in net['nets']:
             if isinstance(n, pandapipesNet):
                 convert_format(net)
```

## Comparing `pandapipes-0.8.5/pandapipes/io/convert_format.py` & `pandapipes-0.9.0/src/pandapipes/io/convert_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from packaging import version
 
 from pandapipes import __format_version__, __version__
 from pandapipes.pandapipes_net import add_default_components
```

## Comparing `pandapipes-0.8.5/pandapipes/io/io_utils.py` & `pandapipes-0.9.0/src/pandapipes/io/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import importlib
 import json
 from copy import deepcopy
 from functools import partial
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/derivative_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from numpy import linalg
 
 from pandapipes.constants import P_CONVERSION, GRAVITATION_CONSTANT, NORMAL_PRESSURE, \
     NORMAL_TEMPERATURE
-from pandapipes.idx_branch import LENGTH, LAMBDA, D, LOSS_COEFFICIENT as LC, RHO, PL, AREA, TINIT, \
-    VINIT
+from pandapipes.idx_branch import LENGTH, LAMBDA, D, LOSS_COEFFICIENT as LC, RHO, PL, AREA, \
+    VINIT, TOUTINIT, FROM_NODE
 from pandapipes.idx_node import HEIGHT, PINIT, PAMB, TINIT as TINIT_NODE
 
 
 def derivatives_hydraulic_incomp_np(branch_pit, der_lambda, p_init_i_abs, p_init_i1_abs,
                                     height_difference):
     v_init_abs = np.abs(branch_pit[:, VINIT])
     v_init2 = v_init_abs * branch_pit[:, VINIT]
@@ -28,28 +28,29 @@
     df_dv_nodes = mass_flow_dv
     load_vec_nodes = mass_flow_dv * branch_pit[:, VINIT]
     df_dp = np.ones_like(der_lambda) * (-1)
     df_dp1 = np.ones_like(der_lambda)
     return load_vec, load_vec_nodes, df_dv, df_dv_nodes, df_dp, df_dp1
 
 
-def derivatives_hydraulic_comp_np(branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs,
+def derivatives_hydraulic_comp_np(node_pit, branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs,
                                   height_difference, comp_fact, der_comp, der_comp1):
     # Formulas for gas pressure loss according to laminar version
     v_init_abs = np.abs(branch_pit[:, VINIT])
     v_init2 = branch_pit[:, VINIT] * v_init_abs
     p_diff = p_init_i_abs - p_init_i1_abs
     p_sum = p_init_i_abs + p_init_i1_abs
     p_sum_div = np.divide(1, p_sum)
-
-    const_lambda = np.divide(NORMAL_PRESSURE * branch_pit[:, RHO] * branch_pit[:, TINIT],
+    from_nodes = branch_pit[:, FROM_NODE].astype(np.int32)
+    tm = (node_pit[from_nodes, TINIT_NODE] + branch_pit[:, TOUTINIT]) / 2
+    const_lambda = np.divide(NORMAL_PRESSURE * branch_pit[:, RHO] * tm,
                              NORMAL_TEMPERATURE * P_CONVERSION)
     const_height = np.divide(
         branch_pit[:, RHO] * NORMAL_TEMPERATURE * GRAVITATION_CONSTANT * height_difference,
-        2 * NORMAL_PRESSURE * branch_pit[:, TINIT] * P_CONVERSION)
+        2 * NORMAL_PRESSURE * tm * P_CONVERSION)
     friction_term = np.divide(lambda_ * branch_pit[:, LENGTH], branch_pit[:, D]) + branch_pit[:, LC]
 
     load_vec = p_diff + branch_pit[:, PL] + const_height * p_sum \
                - const_lambda * comp_fact * v_init2 * friction_term * p_sum_div
 
     p_deriv = const_lambda * v_init2 * friction_term * p_sum_div
     df_dp = -1. + p_deriv * (der_comp - comp_fact * p_sum_div) + const_height
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/derivative_toolbox_numba.py` & `pandapipes-0.9.0/src/pandapipes/pf/derivative_toolbox_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 from numpy import linalg
 
 from pandapipes.constants import P_CONVERSION, GRAVITATION_CONSTANT, NORMAL_PRESSURE, \
     NORMAL_TEMPERATURE
-from pandapipes.idx_branch import LENGTH, LAMBDA, D, LOSS_COEFFICIENT as LC, RHO, PL, AREA, TINIT, \
-    VINIT
+from pandapipes.idx_branch import LENGTH, LAMBDA, D, LOSS_COEFFICIENT as LC, RHO, PL, AREA, \
+    VINIT, FROM_NODE, TO_NODE
 from pandapipes.idx_node import HEIGHT, PAMB, PINIT, TINIT as TINIT_NODE
 
 try:
     from numba import jit
     from numba import int32, float64, int64
 except ImportError:
     from pandapower.pf.no_numba import jit
@@ -39,40 +39,45 @@
                               - v_init2 * lambda_term)
         mass_flow_dv = branch_pit[i][RHO] * branch_pit[i][AREA]
         df_dv_nodes[i] = mass_flow_dv
         load_vec_nodes[i] = mass_flow_dv * branch_pit[i][VINIT]
     return load_vec, load_vec_nodes, df_dv, df_dv_nodes, df_dp, df_dp1
 
 
-@jit((float64[:, :], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
+@jit((float64[:, :], float64[:, :], float64[:], float64[:], float64[:], float64[:], float64[:], float64[:],
       float64[:], float64[:]), nopython=True, cache=False)
-def derivatives_hydraulic_comp_numba(branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs,
+def derivatives_hydraulic_comp_numba(node_pit, branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs,
                                      height_difference, comp_fact, der_comp, der_comp1):
     le = lambda_.shape[0]
     load_vec = np.zeros_like(lambda_)
     df_dv = np.zeros_like(lambda_)
     df_dp = np.zeros_like(lambda_)
     df_dp1 = np.zeros_like(lambda_) * (-1)
     load_vec_nodes = np.zeros_like(der_lambda)
     df_dv_nodes = np.zeros_like(der_lambda)
+    from_nodes = branch_pit[:, FROM_NODE].astype(np.int32)
+    to_nodes = branch_pit[:, TO_NODE].astype(np.int32)
 
     # Formulas for gas pressure loss according to laminar version
     for i in range(le):
         # compressibility settings
         v_init_abs = np.abs(branch_pit[i][VINIT])
         v_init2 = branch_pit[i][VINIT] * v_init_abs
         p_diff = p_init_i_abs[i] - p_init_i1_abs[i]
         p_sum = p_init_i_abs[i] + p_init_i1_abs[i]
         p_sum_div = np.divide(1, p_sum)
+        fn = from_nodes[i]
+        tn = to_nodes[i]
+        tm = (node_pit[fn, TINIT_NODE] + node_pit[tn, TINIT_NODE]) / 2
 
-        const_lambda = np.divide(NORMAL_PRESSURE * branch_pit[i][RHO] * branch_pit[i][TINIT],
+        const_lambda = np.divide(NORMAL_PRESSURE * branch_pit[i][RHO] * tm,
                                  NORMAL_TEMPERATURE * P_CONVERSION)
         const_height = np.divide(
             branch_pit[i][RHO] * NORMAL_TEMPERATURE * GRAVITATION_CONSTANT * height_difference[i],
-            2 * NORMAL_PRESSURE * branch_pit[i][TINIT] * P_CONVERSION)
+            2 * NORMAL_PRESSURE * tm * P_CONVERSION)
         friction_term = np.divide(lambda_[i] * branch_pit[i][LENGTH],
                                   branch_pit[i][D]) + branch_pit[i][LC]
 
         load_vec[i] = p_diff + branch_pit[i][PL] + const_height * p_sum \
             - const_lambda * comp_fact[i] * v_init2 * friction_term * p_sum_div
 
         p_deriv = const_lambda * v_init2 * friction_term * p_sum_div
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/pipeflow_setup.py` & `pandapipes-0.9.0/src/pandapipes/pf/pipeflow_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 import inspect
 
 import numpy as np
+from pandapower.auxiliary import ppException
 from scipy.sparse import coo_matrix, csgraph
 
 from pandapipes.idx_branch import FROM_NODE, TO_NODE, branch_cols, \
-    ACTIVE as ACTIVE_BR
+    ACTIVE as ACTIVE_BR, VINIT
 from pandapipes.idx_node import NODE_TYPE, P, NODE_TYPE_T, node_cols, T, ACTIVE as ACTIVE_ND, \
     TABLE_IDX as TABLE_IDX_ND, ELEMENT_IDX as ELEMENT_IDX_ND
+from pandapipes.pf.internals_toolbox import _sum_by_group
 from pandapipes.properties.fluids import get_fluid
 
 try:
     import numba
     from numba import jit
 
     numba_installed = True
 except ImportError:
     from pandapower.pf.no_numba import jit
+
     numba_installed = False
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
 
-default_options = {"friction_model": "nikuradse", "converged": False, "tol_p": 1e-4, "tol_v": 1e-4,
+default_options = {"friction_model": "nikuradse", "tol_p": 1e-4, "tol_v": 1e-4,
                    "tol_T": 1e-3, "tol_res": 1e-3, "iter": 10, "error_flag": False, "alpha": 1,
                    "nonlinear_method": "constant", "mode": "hydraulics",
                    "ambient_temperature": 293, "check_connectivity": True,
                    "max_iter_colebrook": 100, "only_update_hydraulic_matrix": False,
                    "reuse_internal_data": False, "use_numba": True,
                    "quit_on_inconsistency_connectivity": False, "calc_compression_power": True}
 
@@ -157,16 +160,17 @@
     :return: lookup - A lookup (mostly a dict with mappings from pandapipesNet to internal
             structure)
     :rtype: dict, np.array, ....
 
     """
     pit_type = pit_type.lower()
     lookup_type = lookup_type.lower()
-    all_lookup_types = ["index", "table", "from_to", "active", "length", "from_to_active",
-                        "index_active"]
+    all_lookup_types = ["index", "table", "from_to", "active_hydraulics", "active_heat_transfer",
+                        "length", "from_to_active_hydraulics", "from_to_active_heat_transfer",
+                        "index_active_hydraulics", "index_active_heat_transfer"]
     if lookup_type not in all_lookup_types:
         type_names = "', '".join(all_lookup_types)
         logger.error("No lookup type '%s' exists. Please choose one of '%s'."
                      % (lookup_type, type_names))
         return None
     if pit_type not in ["node", "branch"]:
         logger.error("No pit type '%s' exists. Please choose one of 'node' and 'branch'."
@@ -183,15 +187,15 @@
     At the same time, user-defined arguments for `pandapipes.pipeflow()` always have a higher
     priority. To remove user_pf_options, set "reset = True" and provide no additional arguments.
 
     :param net: pandapipes network for which to create user options
     :type net: pandapipesNet
     :param reset: Specifies whether the user_pf_options is removed before setting new options
     :type reset: bool, default False
-    :param kwargs: pipeflow options that shall be set, e. g. tol_v = 1e-7
+    :param kwargs: pipeflow options that shall be set, e.g. tol_v = 1e-7
     :return: No output
     """
     if reset or 'user_pf_options' not in net.keys():
         net['user_pf_options'] = dict()
 
     additional_kwargs = set(kwargs.keys()) - set(default_options.keys()) - {"fluid", "hyd_flag"}
     if len(additional_kwargs) > 0:
@@ -235,15 +239,15 @@
 
         - **nonlinear_method** (str): "constant" - The option of how the damping factor **alpha** \
                 is determined in each iteration. It can be "constant" (i.e. **alpha** is always the\
                  same in each iteration) or "automatic", in which case **alpha** is adapted \
                  automatically with respect to the convergence behaviour.
 
         - **mode** (str): "hydraulics" - Define the calculation mode: what shall be calculated - \
-                solely hydraulics ('hydraulic'), solely heat transfer('heat') or both combined \
+                solely hydraulics ('hydraulics'), solely heat transfer('heat') or both combined \
                 ('all').
 
         - **only_update_hydraulic_matrix** (bool): False - If True, the system matrix is not \
                 created in every iteration, but only the data is updated according to a lookup that\
                 is identified in the first iteration. This speeds up calculation, but has not yet\
                 been tested extensively.
 
@@ -346,14 +350,15 @@
 
     """
     pit = create_empty_pit(net)
 
     for comp in net['component_list']:
         comp.create_pit_node_entries(net, pit["node"])
         comp.create_pit_branch_entries(net, pit["branch"])
+        comp.create_component_array(net, pit["components"])
     return pit["node"], pit["branch"]
 
 
 def create_empty_pit(net):
     """
     Creates an empty internal structure which is called pit (pandapipes internal tables). The\
     structure is a dictionary which should contain one array for all nodes and one array for all\
@@ -369,15 +374,16 @@
     :rtype: dict
 
     """
     node_length = get_lookup(net, "node", "length")
     branch_length = get_lookup(net, "branch", "length")
     # init empty pit
     pit = {"node": np.empty((node_length, node_cols), dtype=np.float64),
-           "branch": np.empty((branch_length, branch_cols), dtype=np.float64)}
+           "branch": np.empty((branch_length, branch_cols), dtype=np.float64),
+           "components": {}}
     net["_pit"] = pit
     return pit
 
 
 def init_all_result_tables(net):
     """
     Initialize the result tables of all components in the net.
@@ -431,15 +437,95 @@
     net["_lookups"] = {"node_from_to": node_ft_lookups, "branch_from_to": branch_ft_lookups,
                        "node_table": node_table_lookups, "branch_table": branch_table_lookups,
                        "node_index": node_idx_lookups, "branch_index": branch_idx_lookups,
                        "node_length": node_from, "branch_length": branch_from,
                        "internal_nodes_lookup": internal_nodes_lookup}
 
 
-def check_connectivity(net, branch_pit, node_pit, check_heat):
+def identify_active_nodes_branches(net, branch_pit, node_pit, hydraulic=True):
+    """
+    Function that creates the connectivity lookup for nodes and branches. If the option \
+    "check_connectivity" is set, a full connectivity check is performed based on a sparse matrix \
+    graph search. Otherwise, only the nodes and branches are identified that are inactive, which \
+    means:\
+      - in case of hydraulics, just use the "ACTIVE" identifier of the respective components\
+      - in case of heat transfer, use the hydraulic result to check which branches are traversed \
+        by the fluid and a simple rule to make sure that active nodes are connected to at least one\
+        traversed branch\
+    The result of this connectivity search is stored in the lookups (e.g. as \
+    net["_lookups"]["node_active_hydraulics"])
+
+    :param net: the pandapipes net for which to identify the connectivity
+    :type net: pandapipes.pandapipesNet
+    :param branch_pit: Internal array with branch entries
+    :type branch_pit: np.array
+    :param node_pit: Internal array with node entries
+    :type node_pit: np.array
+    :param hydraulic: flag for the mode (if True, do the check for the hydraulic simulation, \
+        otherwise for the heat transfer simulation with other considerations)
+    :type hydraulic: bool, default True
+    :return: No output
+    """
+    if hydraulic:
+        # connectivity check for hydraulic simulation
+        if get_net_option(net, "check_connectivity"):
+            nodes_connected, branches_connected = check_connectivity(net, branch_pit, node_pit)
+        else:
+            # if connectivity check is switched off, still consider oos elements
+            nodes_connected = node_pit[:, ACTIVE_ND].astype(np.bool_)
+            branches_connected = branch_pit[:, ACTIVE_BR].astype(np.bool_)
+    else:
+        # connectivity check for heat simulation (needs to consider branches with 0 velocity as
+        # well)
+        if get_net_option(net, "check_connectivity"):
+            # full connectivity check for hydraulic simulation
+            nodes_connected, branches_connected = check_connectivity(net, branch_pit, node_pit,
+                                                                     mode="heat_transfer")
+        else:
+            # if no full connectivity check is performed, all nodes that are not connected to the
+            # rest of the network wrt. flow can be identified by a more performant sum_by_group_call
+            # check for branches that are not traversed (for temperature calculation, this means
+            # that they are "out of service")
+            branches_connected = get_lookup(net, "branch", "active_hydraulics") \
+                                 & branches_connected_flow(branch_pit)
+            fn = branch_pit[:, FROM_NODE].astype(np.int32)
+            tn = branch_pit[:, TO_NODE].astype(np.int32)
+            fn_tn, flow = _sum_by_group(
+                get_net_option(net, "use_numba"), np.concatenate([fn, tn]),
+                np.concatenate([branches_connected, branches_connected]).astype(np.int32)
+            )
+            nodes_connected = np.copy(get_lookup(net, "node", "active_hydraulics"))
+            # set nodes oos that are not connected to any branches with flow > 0 (0.1 is arbitrary
+            # here, any value between 0 and 1 should work, excluding 0 and 1)
+            nodes_connected[fn_tn] = nodes_connected[fn_tn] & (flow > 0.1)
+    mode = "hydraulics" if hydraulic else "heat_transfer"
+    if np.all(~nodes_connected):
+        mode = 'hydraulic' if hydraulic else 'heat transfer'
+        raise PipeflowNotConverged(" All nodes are set out of service. Probably they are not supplied."
+                                   " Therefore, the %s pipeflow did not converge. "
+                                   " Have you forgotten to define an external grid?" % mode)
+    net["_lookups"]["node_active_" + mode] = nodes_connected
+    net["_lookups"]["branch_active_" + mode] = branches_connected
+
+
+def branches_connected_flow(branch_pit):
+    """
+    Simple function to identify branches with flow based on the calculated velocity.
+
+    :param branch_pit: The pandapipes internal table of the network (including hydraulics results)
+    :type branch_pit: np.array
+    :return: branches_connected_flow - lookup array if branch is connected wrt. flow
+    :rtype: np.array
+    """
+    # TODO: is this formulation correct or could there be any caveats?
+    return ~np.isnan(branch_pit[:, VINIT]) \
+        & ~np.isclose(branch_pit[:, VINIT], 0, rtol=1e-10, atol=1e-10)
+
+
+def check_connectivity(net, branch_pit, node_pit, mode="hydraulics"):
     """
     Perform a connectivity check which means that network nodes are identified that don't have any
     connection to an external grid component. Quick overview over the steps of this function:
 
       - Build a sparse matrix graph (scipy.sparse.csr_matrix) from all branches that are in_service\
         (nodes of this graph are taken from FROM_NODE and TO_NODE column in pit).
       - Add a node that represents all external grids and connect all nodes that are connected to\
@@ -457,48 +543,38 @@
 
     :param net: The pandapipesNet for which to perform the check
     :type net: pandapipesNet
     :param branch_pit: Internal array with branch entries
     :type branch_pit: np.array
     :param node_pit: Internal array with node entries
     :type node_pit: np.array
-    :param check_heat: Flag which determines whether to also check for connectivity to heat \
-        external grids
-    :type check_heat: bool
-    :return: (nodes_connected_hyd, branches_connected) - Lookups of np.arrays stating which of the
+    :return: (nodes_connected, branches_connected) - Lookups of np.arrays stating which of the
             internal nodes and branches are reachable from any of the hyd_slacks (np mask).
     :rtype: tuple(np.array)
     """
-    active_branch_lookup = branch_pit[:, ACTIVE_BR].astype(bool)
-    active_node_lookup = node_pit[:, ACTIVE_ND].astype(bool)
-    from_nodes = branch_pit[:, FROM_NODE].astype(np.int32)
-    to_nodes = branch_pit[:, TO_NODE].astype(np.int32)
-    hyd_slacks = np.where((node_pit[:, NODE_TYPE] == P) & active_node_lookup)[0]
-    # hyd_slacks = np.where(((node_pit[:, NODE_TYPE] == P) | (node_pit[:, NODE_TYPE] == PC))
-    #                       & active_node_lookup)[0]
-
-    nodes_connected, branches_connected = perform_connectivity_search(
-        net, node_pit, hyd_slacks, from_nodes, to_nodes, active_node_lookup, active_branch_lookup,
-        mode="hydraulics")
-    if not check_heat:
-        return nodes_connected, branches_connected
-
-    heat_slacks = np.where((node_pit[:, NODE_TYPE_T] == T) & nodes_connected)[0]
-    if len(heat_slacks) == len(hyd_slacks) and np.all(heat_slacks == hyd_slacks):
-        return nodes_connected, branches_connected
-
-    nodes_connected, branches_connected = perform_connectivity_search(
-        net, node_pit, heat_slacks, from_nodes, to_nodes, nodes_connected, branches_connected,
-        mode="heat transfer")
-    return nodes_connected, branches_connected
+    if mode == "hydraulics":
+        active_branch_lookup = branch_pit[:, ACTIVE_BR].astype(np.bool_)
+        active_node_lookup = node_pit[:, ACTIVE_ND].astype(np.bool_)
+        slacks = np.where((node_pit[:, NODE_TYPE] == P) & active_node_lookup)[0]
+    else:
+        active_branch_lookup = branches_connected_flow(branch_pit) \
+                               & get_lookup(net, "branch", "active_hydraulics")
+        active_node_lookup = node_pit[:, ACTIVE_ND].astype(np.bool_) \
+                             & get_lookup(net, "node", "active_hydraulics")
+        slacks = np.where((node_pit[:, NODE_TYPE_T] == T) & active_node_lookup)[0]
 
+    return perform_connectivity_search(net, node_pit, branch_pit, slacks, active_node_lookup,
+                                       active_branch_lookup, mode=mode)
 
-def perform_connectivity_search(net, node_pit, slack_nodes, from_nodes, to_nodes,
+
+def perform_connectivity_search(net, node_pit, branch_pit, slack_nodes,
                                 active_node_lookup, active_branch_lookup, mode="hydraulics"):
     len_nodes = len(node_pit)
+    from_nodes = branch_pit[:, FROM_NODE].astype(np.int32)
+    to_nodes = branch_pit[:, TO_NODE].astype(np.int32)
     nobranch = np.sum(active_branch_lookup)
     active_from_nodes = from_nodes[active_branch_lookup]
     active_to_nodes = to_nodes[active_branch_lookup]
 
     # we create a "virtual" node that is connected to all slack nodes and start the connectivity
     # search at this node
     fn_matrix = np.concatenate([active_from_nodes, slack_nodes])
@@ -561,82 +637,89 @@
     :type pit_type: str, default "node"
     :return: List of table names and table indices belonging to the pit indices
     """
     int_pit = pit_array[pit_indices, :]
     tables = np.unique(int_pit[:, TABLE_IDX_ND])
     table_lookup = get_lookup(net, pit_type, "table")
     return [(get_table_name(table_lookup, tbl), list(int_pit[int_pit[:, TABLE_IDX_ND] == tbl,
-                                                             ELEMENT_IDX_ND].astype(np.int32)))
+    ELEMENT_IDX_ND].astype(np.int32)))
             for tbl in tables]
 
 
-def reduce_pit(net, node_pit, branch_pit, nodes_connected, branches_connected):
+def reduce_pit(net, node_pit, branch_pit, mode="hydraulics"):
     """
     Create an internal ("active") pit with all nodes and branches that are actually in_service. This
     is also done for different lookups (e.g. the from_to indices for this pit and the node index
     lookup). A specialty that needs to be considered is that from_nodes and to_nodes change to new
     indices.
 
     :param net: The pandapipesNet for which the pit shall be reduced
     :type net: pandapipesNet
     :param node_pit: The internal structure node array
     :type node_pit: np.array
     :param branch_pit: The internal structure branch array
     :type branch_pit: np.array
-    :param nodes_connected: A mask array stating which nodes are actually connected to the rest of\
-            the net
-    :type nodes_connected: np.array
-    :param branches_connected: A mask array stating which branches are actually connected to the \
-             rest of the net
-    :type branches_connected: np.array
+    :param mode: the mode of the calculation (either "hydraulics" or "heat_transfer") for storing /\
+        retrieving correct lookups
+    :type mode: str, default "hydraulics"
     :return: No output
     """
     active_pit = dict()
     els = dict()
     reduced_node_lookup = None
+    nodes_connected = get_lookup(net, "node", "active_" + mode)
+    branches_connected = get_lookup(net, "branch", "active_" + mode)
     if np.alltrue(nodes_connected):
-        net["_lookups"]["node_from_to_active"] = copy.deepcopy(get_lookup(net, "node", "from_to"))
-        net["_lookups"]["node_index_active"] = copy.deepcopy(get_lookup(net, "node", "index"))
+        net["_lookups"]["node_from_to_active_" + mode] = copy.deepcopy(
+            get_lookup(net, "node", "from_to"))
+        net["_lookups"]["node_index_active_" + mode] = copy.deepcopy(
+            get_lookup(net, "node", "index"))
         active_pit["node"] = np.copy(node_pit)
     else:
         active_pit["node"] = np.copy(node_pit[nodes_connected, :])
         reduced_node_lookup = np.cumsum(nodes_connected) - 1
         node_idx_lookup = get_lookup(net, "node", "index")
-        net["_lookups"]["node_index_active"] = {
+        net["_lookups"]["node_index_active_" + mode] = {
             tbl: reduced_node_lookup[idx_lookup[idx_lookup != -1]]
             for tbl, idx_lookup in node_idx_lookup.items()}
         els["node"] = nodes_connected
     if np.alltrue(branches_connected):
-        net["_lookups"]["branch_from_to_active"] = copy.deepcopy(get_lookup(net, "branch",
-                                                                            "from_to"))
+        net["_lookups"]["branch_from_to_active_" + mode] = copy.deepcopy(
+            get_lookup(net, "branch", "from_to"))
         active_pit["branch"] = np.copy(branch_pit)
-        net["_lookups"]["branch_index_active"] = copy.deepcopy(get_lookup(net, "branch", "index"))
+        net["_lookups"]["branch_index_active_" + mode] = copy.deepcopy(
+            get_lookup(net, "branch", "index"))
     else:
         active_pit["branch"] = np.copy(branch_pit[branches_connected, :])
         branch_idx_lookup = get_lookup(net, "branch", "index")
         if len(branch_idx_lookup):
             reduced_branch_lookup = np.cumsum(branches_connected) - 1
-            net["_lookups"]["branch_index_active"] = {
+            net["_lookups"]["branch_index_active_" + mode] = {
                 tbl: reduced_branch_lookup[idx_lookup[idx_lookup != -1]]
                 for tbl, idx_lookup in branch_idx_lookup.items()}
         else:
-            net["_lookups"]["branch_index_active"] = dict()
+            net["_lookups"]["branch_index_active_" + mode] = dict()
         els["branch"] = branches_connected
     if reduced_node_lookup is not None:
         active_pit["branch"][:, FROM_NODE] = reduced_node_lookup[
             branch_pit[branches_connected, FROM_NODE].astype(np.int32)]
         active_pit["branch"][:, TO_NODE] = reduced_node_lookup[
             branch_pit[branches_connected, TO_NODE].astype(np.int32)]
     net["_active_pit"] = active_pit
-    net["_lookups"]["node_active"] = nodes_connected
-    net["_lookups"]["branch_active"] = branches_connected
 
     for el, connected_els in els.items():
         ft_lookup = get_lookup(net, el, "from_to")
         aux_lookup = {table: (ft[0], ft[1], np.sum(connected_els[ft[0]: ft[1]]))
                       for table, ft in ft_lookup.items() if ft is not None}
         from_to_active_lookup = copy.deepcopy(ft_lookup)
         count = 0
         for table, (_, _, len_new) in sorted(aux_lookup.items(), key=lambda x: x[1][0]):
             from_to_active_lookup[table] = (count, count + len_new)
             count += len_new
-        net["_lookups"]["%s_from_to_active" % el] = from_to_active_lookup
+        net["_lookups"]["%s_from_to_active_%s" % (el, mode)] = from_to_active_lookup
+
+
+class PipeflowNotConverged(ppException):
+    """
+    Exception being raised in case pipeflow did not converge.
+    """
+    pass
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/internals_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/pf/internals_toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import logging
 try:
     from numba import jit
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/derivative_calculation.py` & `pandapipes-0.9.0/src/pandapipes/pf/derivative_calculation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 
-from pandapipes.idx_branch import LENGTH, ETA, RHO, D, K, RE, LAMBDA, TINIT, LOAD_VEC_BRANCHES, \
+from pandapipes.idx_branch import LENGTH, ETA, RHO, D, K, RE, LAMBDA, LOAD_VEC_BRANCHES, \
     JAC_DERIV_DV, JAC_DERIV_DP, JAC_DERIV_DP1, LOAD_VEC_NODES, JAC_DERIV_DV_NODE, VINIT, \
-    FROM_NODE, TO_NODE
+    FROM_NODE, TO_NODE, CP, VINIT_T, FROM_NODE_T, TOUTINIT, TEXT, AREA, ALPHA, TL, QEXT, LOAD_VEC_NODES_T, \
+    LOAD_VEC_BRANCHES_T, JAC_DERIV_DT, JAC_DERIV_DT1, JAC_DERIV_DT_NODE
+from pandapipes.idx_node import TINIT as TINIT_NODE
 from pandapipes.properties.fluids import get_fluid
 
 
 def calculate_derivatives_hydraulic(net, branch_pit, node_pit, options):
     """
     Function which creates derivatives.
 
@@ -31,15 +33,14 @@
                                  branch_pit[:, D], branch_pit[:, K], friction_model, lambda_)
     branch_pit[:, RE] = re
     branch_pit[:, LAMBDA] = lambda_
     from_nodes = branch_pit[:, FROM_NODE].astype(np.int32)
     to_nodes = branch_pit[:, TO_NODE].astype(np.int32)
     tinit_branch, height_difference, p_init_i_abs, p_init_i1_abs = \
         get_derived_values(node_pit, from_nodes, to_nodes, options["use_numba"])
-    branch_pit[:, TINIT] = tinit_branch
 
     if not gas_mode:
         if options["use_numba"]:
             from pandapipes.pf.derivative_toolbox_numba import derivatives_hydraulic_incomp_numba \
                 as derivatives_hydraulic_incomp
         else:
             from pandapipes.pf.derivative_toolbox import derivatives_hydraulic_incomp_np \
@@ -58,25 +59,52 @@
                 calc_medium_pressure_with_derivative
         p_m, der_p_m, der_p_m1 = calc_medium_pressure_with_derivative(p_init_i_abs, p_init_i1_abs)
         comp_fact = fluid.get_compressibility(p_m)
         # TODO: this might not be required
         der_comp = fluid.get_der_compressibility() * der_p_m
         der_comp1 = fluid.get_der_compressibility() * der_p_m1
         load_vec, load_vec_nodes, df_dv, df_dv_nodes, df_dp, df_dp1 = derivatives_hydraulic_comp(
-            branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs, height_difference,
+            node_pit, branch_pit, lambda_, der_lambda, p_init_i_abs, p_init_i1_abs, height_difference,
             comp_fact, der_comp, der_comp1)
 
     branch_pit[:, LOAD_VEC_BRANCHES] = load_vec
     branch_pit[:, JAC_DERIV_DV] = df_dv
     branch_pit[:, JAC_DERIV_DP] = df_dp
     branch_pit[:, JAC_DERIV_DP1] = df_dp1
     branch_pit[:, LOAD_VEC_NODES] = load_vec_nodes
     branch_pit[:, JAC_DERIV_DV_NODE] = df_dv_nodes
 
 
+def calculate_derivatives_thermal(net, branch_pit, node_pit, options):
+    cp = branch_pit[:, CP]
+    rho = branch_pit[:, RHO]
+    v_init = branch_pit[:, VINIT_T]
+    from_nodes = branch_pit[:, FROM_NODE_T].astype(np.int32)
+    t_init_i = node_pit[from_nodes, TINIT_NODE]
+    t_init_i1 = branch_pit[:, TOUTINIT]
+    t_amb = branch_pit[:, TEXT]
+    area = branch_pit[:, AREA]
+    length = branch_pit[:, LENGTH]
+    alpha = branch_pit[:, ALPHA] * np.pi * branch_pit[:, D]
+    tl = branch_pit[:, TL]
+    qext = branch_pit[:, QEXT]
+    t_m = (t_init_i1 + t_init_i) / 2
+
+    branch_pit[:, LOAD_VEC_BRANCHES_T] = \
+        -(rho * area * cp * v_init * (-t_init_i + t_init_i1 - tl)
+          - alpha * (t_amb - t_m) * length + qext)
+
+    branch_pit[:, JAC_DERIV_DT] = - rho * area * cp * v_init + alpha / 2 * length
+    branch_pit[:, JAC_DERIV_DT1] = rho * area * cp * v_init + alpha / 2 * length
+
+    branch_pit[:, JAC_DERIV_DT_NODE] = rho * v_init * branch_pit[:, AREA]
+    branch_pit[:, LOAD_VEC_NODES_T] = rho * v_init * branch_pit[:, AREA] \
+                                      * t_init_i1
+
+
 def get_derived_values(node_pit, from_nodes, to_nodes, use_numba):
     if use_numba:
         from pandapipes.pf.derivative_toolbox_numba import calc_derived_values_numba
         return calc_derived_values_numba(node_pit, from_nodes, to_nodes)
     from pandapipes.pf.derivative_toolbox import calc_derived_values_np
     return calc_derived_values_np(node_pit, from_nodes, to_nodes)
 
@@ -106,19 +134,19 @@
     :param options:
     :type options:
     :return:
     :rtype:
     """
     if options["use_numba"]:
         from pandapipes.pf.derivative_toolbox_numba import calc_lambda_nikuradse_incomp_numba as \
-            calc_lambda_nikuradse_incomp, colebrook_numba as colebrook,\
+            calc_lambda_nikuradse_incomp, colebrook_numba as colebrook, \
             calc_lambda_nikuradse_comp_numba as calc_lambda_nikuradse_comp
     else:
         from pandapipes.pf.derivative_toolbox import calc_lambda_nikuradse_incomp_np as \
-            calc_lambda_nikuradse_incomp, colebrook_np as colebrook,\
+            calc_lambda_nikuradse_incomp, colebrook_np as colebrook, \
             calc_lambda_nikuradse_comp_np as calc_lambda_nikuradse_comp
     if gas_mode:
         re, lambda_laminar, lambda_nikuradse = calc_lambda_nikuradse_comp(v, d, k, eta, rho)
     else:
         re, lambda_laminar, lambda_nikuradse = calc_lambda_nikuradse_incomp(v, d, k, eta, rho)
 
     if friction_model == "colebrook":
@@ -130,15 +158,15 @@
         if not converged:
             raise PipeflowNotConverged(
                 "The Colebrook-White algorithm did not converge. There might be model "
                 "inconsistencies. The maximum iterations can be given as 'max_iter_colebrook' "
                 "argument to the pipeflow.")
         return lambda_colebrook, re
     elif friction_model == "swamee-jain":
-        lambda_swamee_jain = 0.25 / ((np.log10(k/(3.7*d) + 5.74/(re**0.9)))**2)
+        lambda_swamee_jain = 0.25 / ((np.log10(k / (3.7 * d) + 5.74 / (re ** 0.9))) ** 2)
         return lambda_swamee_jain, re
     else:
         # lambda_tot = np.where(re > 2300, lambda_laminar + lambda_nikuradse, lambda_laminar)
         lambda_tot = lambda_laminar + lambda_nikuradse
         return lambda_tot, re
 
 
@@ -178,15 +206,15 @@
         df_dlambda = -0.5 * lambda_pipe ** (-3 / 2) - (2.51 * eta / (rho * d * v_corr)) \
                      * lambda_pipe ** (-3 / 2) / (np.log(10) * b_term)
 
         lambda_colebrook_der = df_dv / df_dlambda
 
         return lambda_colebrook_der
     elif friction_model == "swamee-jain":
-        param = k/(3.7*d) + 5.74 * (np.abs(eta))**0.9 / ((np.abs(rho*v_corr*d))**0.9)
+        param = k / (3.7 * d) + 5.74 * (np.abs(eta)) ** 0.9 / ((np.abs(rho * v_corr * d)) ** 0.9)
         # 0.5 / (log(10) * log(param)^3 * param) * 5.166 * abs(eta)^0.9  / (abs(rho * d)^0.9
         # * abs(v_corr)^1.9)
         lambda_swamee_jain_der = 0.5 / np.log(10) / (np.log(param) ** 3) / param * 5.166 \
                                  * np.abs(eta) ** 0.9 / ((np.abs(rho * d) ** 0.9)
                                                          * np.abs(v_corr) ** 1.9)
         return lambda_swamee_jain_der
     else:
```

## Comparing `pandapipes-0.8.5/pandapipes/pf/build_system_matrix.py` & `pandapipes-0.9.0/src/pandapipes/pf/build_system_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from pandapipes.idx_branch import FROM_NODE, TO_NODE, JAC_DERIV_DV, JAC_DERIV_DP, JAC_DERIV_DP1, \
     JAC_DERIV_DV_NODE, LOAD_VEC_NODES, LOAD_VEC_BRANCHES, JAC_DERIV_DT, JAC_DERIV_DT1, \
     JAC_DERIV_DT_NODE, LOAD_VEC_NODES_T, LOAD_VEC_BRANCHES_T, FROM_NODE_T, TO_NODE_T, BRANCH_TYPE
```

## Comparing `pandapipes-0.8.5/pandapipes/topology/graph_searches.py` & `pandapipes-0.9.0/src/pandapipes/topology/graph_searches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import networkx as nx
 import pandas as pd
 from pandapipes.topology.create_graph import create_nxgraph
```

## Comparing `pandapipes-0.8.5/pandapipes/topology/create_graph.py` & `pandapipes-0.9.0/src/pandapipes/topology/create_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import networkx as nx
 import numpy as np
 from pandapower.topology.create_graph import add_edges, get_edge_table
 
@@ -109,15 +109,15 @@
         mg = nx.Graph()
 
     branch_kw = ["include", "respect_status", "weighting"]
     branch_params = {k: v for k, v in kwargs.items() if any(k.startswith(par) for par in branch_kw)}
     loc = locals()
     branch_params.update({"%s_%s" % (par, bc): loc.get("%s_%s" % (par, bc)) for par in branch_kw
                           for bc in ["pipes", "valves", "pumps", "press_controls",
-                                     "mass_circ_pumps", "press_circ_pumps", "valve_pipes",
+                                     "mass_circ_pumps", "pressure_circ_pumps", "valve_pipes",
                                      "flow_controls"]})
 
     for comp in net.component_list:
         if not issubclass(comp, BranchComponent):
             continue
         table_name = comp.table_name()
         include_kw = "%ss" % table_name
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/pipeflow_results.py` & `pandapipes-0.9.0/src/pandapipes/plotting/pipeflow_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 
 import pandapipes.topology as top
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/geo.py` & `pandapipes-0.9.0/src/pandapipes/plotting/geo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapower.plotting.geo import _node_geometries_from_geodata, \
     _transform_node_geometry_to_geodata, _branch_geometries_from_geodata, \
     _transform_branch_geometry_to_coords, _convert_xy_epsg
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/generic_geodata.py` & `pandapipes-0.9.0/src/pandapipes/plotting/generic_geodata.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from pandapower.plotting.generic_geodata import coords_from_igraph, \
     _prepare_geodata_table, _get_element_mask_from_nodes, _igraph_meshed
 
@@ -16,15 +16,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def build_igraph_from_ppipes(net, junctions=None):
     """
     This function uses the igraph library to create an igraph graph for a given pandapipes network.
-    Pipes and valves are respected.
+    Any branch component is respected.
     Performance vs. networkx: https://graph-tool.skewed.de/performance
 
     :param net: The pandapipes network
     :type net: pandapipesNet
     :param junctions: subset of junctions that should be part of the graph
     :type junctions: list
     :return: The returned values are:
@@ -46,27 +46,23 @@
     g = ig.Graph(directed=True)
     junction_index = net.junction.index if junctions is None else np.array(junctions)
     nr_junctions = len(junction_index)
     g.add_vertices(nr_junctions)
     g.vs["label"] = list(junction_index)
     pp_junction_mapping = dict(list(zip(junction_index, list(range(nr_junctions)))))
 
-    mask = _get_element_mask_from_nodes(net, "pipe", ["from_junction", "to_junction"], junctions)
-    for pipe in net.pipe[mask].itertuples():
-        g.add_edge(pp_junction_mapping[pipe.from_junction], pp_junction_mapping[pipe.to_junction],
-                   weight=pipe.length_km)
-
     for comp in net['component_list']:
-        if not isinstance(comp, BranchComponent):
+        if not issubclass(comp, BranchComponent):
             continue
         fjc, tjc = comp.from_to_node_cols()
         mask = _get_element_mask_from_nodes(net, comp.table_name(), [fjc, tjc], junctions)
         for comp_data in net[comp.table_name()][mask].itertuples():
-            g.add_edge(pp_junction_mapping[comp_data[fjc]], pp_junction_mapping[comp_data[tjc]],
-                       weight=0.001)
+            weight = 0.001 if 'length_km' not in dir(comp_data) else getattr(comp_data, 'length_km')
+            g.add_edge(pp_junction_mapping[getattr(comp_data, fjc)], pp_junction_mapping[getattr(comp_data, tjc)],
+                       weight=weight)
 
     meshed = _igraph_meshed(g)
     roots = [pp_junction_mapping[s] for s in net.ext_grid.junction.values if s in junction_index]
     return g, meshed, roots  # g, (not g.is_dag())
 
 
 def create_generic_coordinates(net, mg=None, library="igraph", geodata_table="junction_geodata",
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/simple_plot.py` & `pandapipes-0.9.0/src/pandapipes/plotting/simple_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from itertools import chain
 
 import matplotlib.pyplot as plt
 from pandapower.plotting import draw_collections
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/patch_makers.py` & `pandapipes-0.9.0/src/pandapipes/plotting/patch_makers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from matplotlib.patches import RegularPolygon, Rectangle, Circle, PathPatch, FancyArrow
 from matplotlib.path import Path
 from pandapower.plotting.plotting_toolbox import get_color_list, _rotate_dim2, get_angle_list, \
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/collections.py` & `pandapipes-0.9.0/src/pandapipes/plotting/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 from pandapower.plotting.collections import _create_node_collection, \
     _create_node_element_collection, _create_line2d_collection, _create_complex_branch_collection, \
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/__init__.py` & `pandapipes-0.9.0/src/pandapipes/plotting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import types
 
 from matplotlib.backend_bases import GraphicsContextBase, RendererBase
```

## Comparing `pandapipes-0.8.5/pandapipes/plotting/plotting_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/plotting/plotting_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 def get_collection_sizes(net, junction_size=1.0, ext_grid_size=1.0, sink_size=1.0, source_size=1.0,
                          valve_size=2.0, pump_size=1.0, heat_exchanger_size=1.0,
                          pressure_control_size=1.0, compressor_size=1.0, flow_control_size=1.0):
     """
```

## Comparing `pandapipes-0.8.5/pandapipes/properties/properties_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/properties/properties_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 
 
 def calculate_mixture_viscosity(components_viscosities, components_molar_proportions,
```

## Comparing `pandapipes-0.8.5/pandapipes/properties/fluids.py` & `pandapipes-0.9.0/src/pandapipes/properties/fluids.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
@@ -14,14 +14,17 @@
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
 
+_LIQUIDS = ["water"]
+_GASES = ["air", "lgas", "hgas", "hydrogen", "methane", "biomethane_pure", "biomethane_treated"]
+
 
 class Fluid(JSONSerializableClass):
     """
 
     """
 
     def __init__(self, name, fluid_type, **kwargs):
@@ -664,44 +667,42 @@
         return FluidPropertyConstant.from_path(
             os.path.join(pp_dir, "properties", fluid_name, prop + ".txt"))
 
     def linear_property(prop):
         return FluidPropertyLinear.from_path(
             os.path.join(pp_dir, "properties", fluid_name, prop + ".txt"))
 
-    liquids = ["water"]
-    gases = ["air", "lgas", "hgas", "hydrogen", "methane"]
-
     if fluid_name == "natural_gas":
         logger.error("'natural_gas' is ambigious. Please choose 'hgas' or 'lgas' "
                      "(high- or low calorific natural gas)")
-    if fluid_name not in liquids and fluid_name not in gases:
+    if fluid_name not in _LIQUIDS and fluid_name not in _GASES:
         raise AttributeError("Fluid '%s' not found in the fluid library. It might not be "
                              "implemented yet." % fluid_name)
 
-    phase = "liquid" if fluid_name in liquids else "gas"
+    phase = "liquid" if fluid_name in _LIQUIDS else "gas"
+
+    properties = dict()
+    properties["density"] = interextra_property("density")
+    properties["viscosity"] = interextra_property("viscosity")
+    properties["heat_capacity"] = interextra_property("heat_capacity")
+    properties["molar_mass"] = constant_property("molar_mass")
+    properties["der_compressibility"] = constant_property("der_compressibility")
+    properties["compressibility"] = linear_property("compressibility")
+
+    if phase == 'gas':
+        for entry, name in [("lhv", "lower_heating_value"), ("hhv", "higher_heating_value")]:
+            try:
+                properties[entry] = constant_property(name)
+            except FileNotFoundError:
+                logger.warning(
+                    f"Unable to find {' '.join([n.capitalize() for n in name.split('_')])} for "
+                    f"{fluid_name}"
+                )
 
-    density = interextra_property("density")
-    viscosity = interextra_property("viscosity")
-    heat_capacity = interextra_property("heat_capacity")
-    molar_mass = constant_property("molar_mass")
-    der_compr = constant_property("der_compressibility")
-    compr = linear_property("compressibility")
-
-    if (phase == 'gas') & (fluid_name != 'air'):
-        lhv = constant_property("lower_heating_value")
-        hhv = constant_property("higher_heating_value")
-
-        return Fluid(fluid_name, phase, density=density, viscosity=viscosity,
-                     heat_capacity=heat_capacity, molar_mass=molar_mass,
-                     compressibility=compr, der_compressibility=der_compr, lhv=lhv, hhv=hhv)
-    else:
-        return Fluid(fluid_name, phase, density=density, viscosity=viscosity,
-                     heat_capacity=heat_capacity, molar_mass=molar_mass, compressibility=compr,
-                     der_compressibility=der_compr)
+    return Fluid(fluid_name, phase, **properties)
 
 
 def get_fluid(net):
     """
     This function shows which fluid is used in the net.
 
     :param net: Current network
```

## Comparing `pandapipes-0.8.5/pandapipes/properties/nitrogen/density.txt` & `pandapipes-0.9.0/src/pandapipes/properties/nitrogen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/nitrogen/heat_capacity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/nitrogen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/nitrogen/viscosity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/nitrogen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/oxygen/density.txt` & `pandapipes-0.9.0/src/pandapipes/properties/oxygen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/oxygen/heat_capacity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/oxygen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/oxygen/viscosity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/oxygen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/hydrogen/density.txt` & `pandapipes-0.9.0/src/pandapipes/properties/hydrogen/density.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/hydrogen/heat_capacity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/hydrogen/heat_capacity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/properties/hydrogen/viscosity.txt` & `pandapipes-0.9.0/src/pandapipes/properties/hydrogen/viscosity.txt`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/std_types/std_types.py` & `pandapipes-0.9.0/src/pandapipes/std_types/std_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 import warnings
 import re
```

## Comparing `pandapipes-0.8.5/pandapipes/std_types/std_type_class.py` & `pandapipes-0.9.0/src/pandapipes/std_types/std_type_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/std_types/library/Pipe.csv` & `pandapipes-0.9.0/src/pandapipes/std_types/library/Pipe.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/test_imports.py` & `pandapipes-0.9.0/src/pandapipes/test/test_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 
 import importlib.util
 import os
```

## Comparing `pandapipes-0.8.5/pandapipes/test/run_tests.py` & `pandapipes-0.9.0/src/pandapipes/test/run_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 import shutil
 import tempfile
```

## Comparing `pandapipes-0.8.5/pandapipes/test/test_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/test/test_toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 import os
 
 import numpy as np
```

## Comparing `pandapipes-0.8.5/pandapipes/test/__init__.py` & `pandapipes-0.9.0/src/pandapipes/test/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 from pandapipes import pp_dir
 
 test_path = os.path.join(pp_dir, 'test')
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 import os
 
 import numpy as np
@@ -90,16 +90,16 @@
     pandapipes.create_sink(ntw, 1, mdot_kg_per_s=1)
 
     pandapipes.create_fluid_from_lib(ntw, "water", overwrite=True)
 
     pandapipes.pipeflow(ntw, stop_condition="tol", iter=50, friction_model="nikuradse",
                         nonlinear_method="automatic", mode="hydraulics", use_numba=use_numba)
 
-    p = ntw._pit["node"][:, 5]
-    v = ntw._pit["branch"][:, 12]
+    p = ntw._pit["node"][:, PINIT]
+    v = ntw._pit["branch"][:, VINIT]
     u = np.concatenate((p, v))
 
     pandapipes.pipeflow(ntw, sol_vec=u, stop_condition="tol", iter=50, friction_model="nikuradse",
                         nonlinear_method="automatic", mode="heat", use_numba=use_numba)
 
     temp_net = net.res_junction.t_k
     temp_ntw = ntw.res_junction.t_k
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_inservice.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_inservice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import numpy as np
 import pytest
 
 import pandapipes
 from pandapipes.pf.pipeflow_setup import get_lookup
-from pandapipes.pipeflow import logger as pf_logger
 from pandapipes.pipeflow import PipeflowNotConverged
+from pandapipes.pipeflow import logger as pf_logger
 
 try:
     import pandaplan.core.pplog as logging
 except ImportError:
     import logging
 
 logger = logging.getLogger(__name__)
@@ -83,15 +83,15 @@
     pandapipes.create_pipe_from_parameters(net, j1, j2, 0.1, 0.1, alpha_w_per_m2k=5, index=3)
     pandapipes.create_pipe_from_parameters(net, j1, j3, 0.1, 0.1, alpha_w_per_m2k=5, index=4)
     pandapipes.create_pipe_from_parameters(net, j2, j4, 0.1, 0.1, alpha_w_per_m2k=5,
                                            in_service=False, index=5)
     pandapipes.create_pipe_from_parameters(net, j3, j5, 0.1, 0.1, alpha_w_per_m2k=5,
                                            in_service=False, index=7)
     pandapipes.create_pipe_from_parameters(net, j6, j7, 0.1, 0.1, alpha_w_per_m2k=5, index=9)
-    pandapipes.create_pipe_from_parameters(net, j5, 8, 0.1, 0.1, alpha_w_per_m2k=5,
+    pandapipes.create_pipe_from_parameters(net, j5, j8, 0.1, 0.1, alpha_w_per_m2k=5,
                                            in_service=False, index=8)
     pandapipes.create_pipe_from_parameters(net, j8, j10, 0.1, 0.1, alpha_w_per_m2k=5, index=1)
     pandapipes.create_pipe_from_parameters(net, j9, j10, 0.1, 0.1, alpha_w_per_m2k=5, index=2)
 
     pandapipes.create_valve(net, j5, j6, 0.1, index=10)
     pandapipes.create_valve(net, j4, j5, 0.1, opened=False, index=12)
 
@@ -121,14 +121,36 @@
     pandapipes.create_sinks(net, [10, 6, 15, 7], 0.1, index=[3, 5, 1, 2],
                             in_service=[True, False, True, True])
     pandapipes.create_source(net, 12, 0.05, index=2)
     pandapipes.create_source(net, 9, 0.06, index=4, in_service=False)
     return net
 
 
+@pytest.fixture
+def create_net_wo_ext_grid():
+    net = pandapipes.create_empty_network("net", add_stdtypes=False)
+    pandapipes.create_fluid_from_lib(net, "hgas", overwrite=True)
+    pandapipes.create_junction(net, index=3, pn_bar=16, tfluid_k=283, height_m=0,
+                               name="Junction 3", in_service=True,
+                               type="junction", geodata=(0, 0))
+    pandapipes.create_junction(net, index=9, pn_bar=16, tfluid_k=283, height_m=0,
+                               name="Junction 9", in_service=True,
+                               type="junction", geodata=(1, 0))
+    pandapipes.create_junction(net, index=10, pn_bar=16, tfluid_k=283, height_m=0,
+                               name="Junction 10", in_service=True,
+                               type="junction", geodata=(2, 0))
+    pandapipes.create_pipe_from_parameters(net, 9, 10, length_km=1, diameter_m=0.03, k_mm=.1, sections=10,
+                                           alpha_w_per_m2k=1, name="Pipe 6")
+    pandapipes.create_sink(net, 9, mdot_kg_per_s=0.01, name="Sink 3")
+    pandapipes.create_source(net, junction=10, mdot_kg_per_s=0.04, name="Source 3")
+    pandapipes.create_compressor(net, from_junction=9, to_junction=3, pressure_ratio=1.1,
+                                 name="Compressor 0", index=None, in_service=True)
+    return net
+
+
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_inservice_gas(create_test_net, use_numba):
     """
 
     :param create_test_net:
     :type create_test_net:
     :return:
@@ -139,15 +161,15 @@
     pandapipes.create_fluid_from_lib(net, "lgas")
 
     pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
                         use_numba=use_numba)
 
     assert np.all(np.isnan(net.res_pipe.loc[~net.pipe.in_service, :].values))
     assert np.all(np.isnan(net.res_valve.loc[~net.valve.opened, :].values))
-    assert np.all(np.isnan(net.res_junction.loc[~net.junction.in_service, :].values))
+    assert np.all(np.isnan(net.res_junction.p_bar.loc[~net.junction.in_service].values))
 
     oos_sinks = np.isin(net.sink.junction.values, net.junction.index[~net.junction.in_service]) \
         | ~net.sink.in_service.values
     assert np.all(np.isnan(net.res_sink.loc[oos_sinks, :].values))
 
     assert not np.any(np.isnan(net.res_pipe.v_mean_m_per_s.loc[net.pipe.in_service].values))
     assert not np.any(np.isnan(net.res_valve.v_mean_m_per_s.loc[net.valve.opened].values))
@@ -172,15 +194,15 @@
     pandapipes.create_fluid_from_lib(net, "water")
 
     pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
                         use_numba=use_numba)
 
     assert np.all(np.isnan(net.res_pipe.loc[~net.pipe.in_service, :].values))
     assert np.all(np.isnan(net.res_valve.loc[~net.valve.opened, :].values))
-    assert np.all(np.isnan(net.res_junction.loc[~net.junction.in_service, :].values))
+    assert np.all(np.isnan(net.res_junction.p_bar.loc[~net.junction.in_service].values))
 
     oos_sinks = np.isin(net.sink.junction.values, net.junction.index[~net.junction.in_service]) \
         | ~net.sink.in_service.values
     assert np.all(np.isnan(net.res_sink.loc[oos_sinks, :].values))
 
     assert not any(np.isnan(net.res_pipe.v_mean_m_per_s.loc[net.pipe.in_service].values))
     assert not any(np.isnan(net.res_valve.v_mean_m_per_s.loc[net.valve.opened].values))
@@ -206,28 +228,28 @@
     net.pipe.in_service = [True, False, False, True, True]
 
     pandapipes.create_fluid_from_lib(net, "water")
 
     pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
                         use_numba=use_numba)
 
-    assert np.all(np.isnan(net.res_junction.loc[[2, 5, 6], :].values))
+    assert np.all(np.isnan(net.res_junction.p_bar.loc[[2, 5, 6]].values))
     assert np.all(np.isnan(net.res_pipe.loc[[1, 2, 3], :].values))
     assert not np.any(np.isnan(net.res_junction.loc[[0, 1, 3, 4], :].values))
     assert not np.any(np.isnan(net.res_pipe.loc[[0, 4],
                                                 ["v_mean_m_per_s", "p_from_bar",
                                                  "p_to_bar"]].values))
     assert not np.any(np.isnan(net.res_sink.loc[[0, 2], "mdot_kg_per_s"].values))
     assert np.all(np.isnan(net.res_sink.loc[[1, 3, 4], "mdot_kg_per_s"].values))
 
     assert np.allclose(net.res_ext_grid.mdot_kg_per_s.sum(), -net.res_sink.mdot_kg_per_s.sum(),
                        rtol=1e-10, atol=0)
 
-    active_branches = get_lookup(net, "branch", "active")
-    active_nodes = get_lookup(net, "node", "active")
+    active_branches = get_lookup(net, "branch", "active_hydraulics")
+    active_nodes = get_lookup(net, "node", "active_hydraulics")
 
     assert np.all(active_nodes == np.array([True, True, False, True, True, False, False, False,
                                             False, True]))
     assert np.all(active_branches == np.array([True, False, False, False, False, False, True,
                                                True, True, False]))
 
 
@@ -253,46 +275,59 @@
     pandapipes.create_pipe_from_parameters(net, 0, j, 0.1, 0.1)
 
     pandapipes.create_sink(net, j, 0.1)
 
     pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
                         use_numba=use_numba)
 
-    active_branches = get_lookup(net, "branch", "active")
-    active_nodes = get_lookup(net, "node", "active")
+    active_branches = get_lookup(net, "branch", "active_hydraulics")
+    active_nodes = get_lookup(net, "node", "active_hydraulics")
 
     assert np.all(active_nodes == np.array([True, True, True, True, True, True, True, False,
                                             False, True, False, False, True, True, True]))
     assert np.all(active_branches)
 
-    assert not np.all(np.isnan(net.res_junction.loc[[0, 1, 2, 3, 4, 5, 9], :].values))
+    assert not np.all(np.isnan(net.res_junction.p_bar.loc[[0, 1, 2, 3, 4, 5, 9]].values))
     assert not np.all(np.isnan(net.res_pipe.values))
-    assert np.any(np.isnan(net.res_junction.loc[[7, 8, 10, 11], :].values))
+    assert np.all(np.isnan(net.res_junction.p_bar.loc[[7, 8, 10, 11]].values))
+
+    with pytest.raises(PipeflowNotConverged):
+        pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
+                            use_numba=use_numba, check_connectivity=False)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_connectivity_heat1(complex_heat_connectivity_grid, use_numba):
     net = copy.deepcopy(complex_heat_connectivity_grid)
     pandapipes.pipeflow(net, mode="all", check_connectivity=True, use_numba=use_numba)
 
-    assert set(net.res_junction.loc[net.res_junction.p_bar.notnull()].index) == {8, 9, 10}
-    assert set(net.res_junction.loc[net.res_junction.p_bar.isnull()].index) \
-           == set(net.junction.index) - {8, 9, 10}
-    assert set(net.res_pipe.loc[net.res_pipe.v_mean_m_per_s.notnull()].index) == {1, 2}
-    assert set(net.res_pipe.loc[net.res_pipe.v_mean_m_per_s.isnull()].index) \
-           == set(net.pipe.index) - {1, 2}
+    oos_juncs_hyd = {4, 5, 6, 7}
+    oos_pipe_hyd = {5, 7, 8, 9}
+    oos_sink_hyd = {4, 5}
+    oos_source_hyd = {7}
+
+    assert set(net.res_junction.loc[net.res_junction.p_bar.notnull()].index) == \
+           set(net.junction.index) - oos_juncs_hyd
+    assert set(net.res_junction.loc[net.res_junction.p_bar.isnull()].index) == oos_juncs_hyd
+
+    assert set(net.res_pipe.loc[net.res_pipe.v_mean_m_per_s.notnull()].index) == \
+           set(net.pipe.index) - oos_pipe_hyd
+    assert set(net.res_pipe.loc[net.res_pipe.v_mean_m_per_s.isnull()].index) == oos_pipe_hyd
+
     assert set(net.res_valve.loc[net.res_valve.v_mean_m_per_s.notnull()].index) == set()
     assert set(net.res_valve.loc[net.res_valve.v_mean_m_per_s.isnull()].index) \
            == set(net.valve.index)
-    assert set(net.res_sink.loc[net.res_sink.mdot_kg_per_s.isnull()].index) == {3, 4, 5}
+
+    assert set(net.res_sink.loc[net.res_sink.mdot_kg_per_s.isnull()].index) == oos_sink_hyd
     assert set(net.res_sink.loc[net.res_sink.mdot_kg_per_s.notnull()].index) == \
-           set(net.sink.index) - {3, 4, 5}
-    assert set(net.res_source.loc[net.res_source.mdot_kg_per_s.isnull()].index) == \
-           set(net.source.index)
-    assert set(net.res_source.loc[net.res_source.mdot_kg_per_s.notnull()].index) == set()
+           set(net.sink.index) - oos_sink_hyd
+
+    assert set(net.res_source.loc[net.res_source.mdot_kg_per_s.isnull()].index) == oos_source_hyd
+    assert (set(net.res_source.loc[net.res_source.mdot_kg_per_s.notnull()].index) ==
+            set(net.source.index) - oos_source_hyd)
 
     assert np.allclose(net.res_ext_grid.mdot_kg_per_s.sum(),
                        -net.res_sink.mdot_kg_per_s.sum() + net.res_source.mdot_kg_per_s.sum(),
                        rtol=1e-10, atol=0)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
@@ -349,14 +384,50 @@
 
     assert np.allclose(net.res_ext_grid.mdot_kg_per_s.sum(),
                        -net.res_sink.mdot_kg_per_s.sum() + net.res_source.mdot_kg_per_s.sum(),
                        rtol=1e-10, atol=0)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
+def test_connectivity_heat4(complex_heat_connectivity_grid, use_numba):
+    net = copy.deepcopy(complex_heat_connectivity_grid)
+
+    net.pipe.in_service.loc[[7, 8]] = True
+    j_new = pandapipes.create_junction(net, 1, 320.15)
+    pandapipes.create_pipe_from_parameters(net, 8, j_new, 0.1, 0.1, alpha_w_per_m2k=5)
+
+    net2 = copy.deepcopy(net)
+
+    pandapipes.pipeflow(net, mode="all", check_connectivity=True, use_numba=use_numba)
+    pandapipes.pipeflow(net2, mode="all", check_connectivity=False, use_numba=use_numba)
+
+    assert pandapipes.nets_equal(net, net2, check_only_results=True)
+
+
+@pytest.mark.parametrize("use_numba", [True, False])
+def test_connectivity_heat5(complex_heat_connectivity_grid, use_numba):
+    net = copy.deepcopy(complex_heat_connectivity_grid)
+    net.pipe.in_service.loc[[7, 8]] = True
+
+    j_from, j_to = pandapipes.create_junctions(net, 2, 1, 320.15)
+
+    pandapipes.create_pipe_from_parameters(net, j_from, j_to, 0.1, 0.1, alpha_w_per_m2k=5)
+    pandapipes.create_sink(net, j_to, 0.1)
+    pandapipes.create_ext_grid(net, j_from, 1, 320.15)
+
+    net.ext_grid.loc[2, 'in_service'] = False
+    net.ext_grid.loc[1, 'type'] = 'p'
+
+    pandapipes.pipeflow(net, check_connectivity=True, mode='all', use_numba=use_numba)
+
+    with pytest.raises(PipeflowNotConverged):
+        pandapipes.pipeflow(net, check_connectivity=False, mode='all', use_numba=use_numba)
+
+
+@pytest.mark.parametrize("use_numba", [True, False])
 def test_exclude_unconnected_junction(use_numba):
     """
     test if unconnected junctions that do not have the highest index are excluded correctly
     (pipeflow fails if reduced_pit does not reindex the reduced nodes correctly)
     :return:
     :rtype:
     """
@@ -386,14 +457,20 @@
     return get_oos(net, tbl) | net[tbl].junction.isin(oosj)
 
 
 def get_oos_branch(net, tbl, oosj=()):
     return get_oos(net, tbl) | net[tbl].from_junction.isin(oosj) | net[tbl].to_junction.isin(oosj)
 
 
+def get_col_slice_null(tbl):
+    if tbl == "junction":
+        return "p_bar"
+    return slice(None)
+
+
 all_tbls_funcs = {"junction": get_oos, "pipe": get_oos_branch, "sink": get_oos_node_elem,
                   "source": get_oos_node_elem, "ext_grid": get_oos_node_elem,
                   "press_control": get_oos_branch}
 
 
 def check_mass_flows(net):
     return np.isclose(net.res_ext_grid.mdot_kg_per_s.sum(),
@@ -436,15 +513,16 @@
 
     with pytest.raises(PipeflowNotConverged):
         pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=False)
 
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_mixed_indexing_oos3(create_mixed_indexing_grid, use_numba):
     net = copy.deepcopy(create_mixed_indexing_grid)
@@ -453,15 +531,16 @@
 
     with pytest.raises(PipeflowNotConverged):
         pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=False)
 
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_mixed_indexing_oos4(create_mixed_indexing_grid, use_numba):
     net = copy.deepcopy(create_mixed_indexing_grid)
@@ -470,15 +549,16 @@
 
     with pytest.raises(PipeflowNotConverged):
         pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=False)
 
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_mixed_indexing_oos5(create_mixed_indexing_grid, use_numba):
     net = copy.deepcopy(create_mixed_indexing_grid)
@@ -487,15 +567,16 @@
 
     with pytest.raises(PipeflowNotConverged):
         pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=False)
 
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
 
 @pytest.mark.parametrize("use_numba", [True, False])
 def test_mixed_indexing_oos6(create_mixed_indexing_grid, use_numba):
     net = copy.deepcopy(create_mixed_indexing_grid)
@@ -504,22 +585,48 @@
 
     with pytest.raises(PipeflowNotConverged):
         pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=False)
 
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
     net.ext_grid.at[1, "in_service"] = False
     pandapipes.pipeflow(net, mode="hydraulics", use_numba=use_numba, check_connectivity=True)
     assert all(np.all(net["res_" + tbl].loc[~oos_func(net, tbl, oos_juncs)].notnull())
                for tbl, oos_func in all_tbls_funcs.items())
-    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs)].isnull())
+    assert all(np.all(net["res_" + tbl].loc[oos_func(net, tbl, oos_juncs),
+                                            get_col_slice_null(tbl)].isnull())
                for tbl, oos_func in all_tbls_funcs.items())
     assert check_mass_flows(net)
 
 
+@pytest.mark.parametrize("use_numba", [True, False])
+def test_pipeflow_all_oos(create_net_wo_ext_grid, use_numba):
+    net = create_net_wo_ext_grid
+    ex1 = pandapipes.create_ext_grid(net, junction=3, t_k=300)
+    ex2 = pandapipes.create_ext_grid(net, junction=3, p_bar=1)
+    with pytest.raises(PipeflowNotConverged):
+        net.ext_grid.at[ex2, 'in_service'] = False
+        pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
+                            use_numba=use_numba, check_connectivity=True)
+    assert ~net.converged
+    net.ext_grid.at[ex1, 'in_service'] = False
+    net.ext_grid.at[ex2, 'in_service'] = True
+
+    pandapipes.pipeflow(net, iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
+                        use_numba=use_numba, check_connectivity=True)
+    assert not np.all(np.isnan(net.res_junction.p_bar.values))
+    assert net.converged
+
+    with pytest.raises(PipeflowNotConverged):
+        pandapipes.pipeflow(net, mode='all', iter=100, tol_p=1e-7, tol_v=1e-7, friction_model="nikuradse",
+                            use_numba=use_numba, check_connectivity=True)
+    assert ~net.converged
+
+
 if __name__ == "__main__":
     pytest.main([r'pandapipes/test/pipeflow_internals/test_inservice.py'])
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_options.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import pandapipes.pf.pipeflow_setup
 import pandapipes
 import copy
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_non_convergence.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_non_convergence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import numpy as np
 import pandas as pd
 import pytest
 
 import pandapipes
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_update_matrix.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_update_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pytest
 
 import pandapipes.networks.simple_gas_networks as nw
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/test_time_series.py` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/test_time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 import tempfile
 
 import numpy as np
```

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv` & `pandapipes-0.9.0/src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/multinet/test_time_series_multinet.py` & `pandapipes-0.9.0/src/pandapipes/test/multinet/test_time_series_multinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandas as pd
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/multinet/test_control_multinet.py` & `pandapipes-0.9.0/src/pandapipes/test/multinet/test_control_multinet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import numpy as np
 import pandapower
```

## Comparing `pandapipes-0.8.5/pandapipes/test/converter/test_stanet_converter.py` & `pandapipes-0.9.0/src/pandapipes/test/converter/test_stanet_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv` & `pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv` & `pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv` & `pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv` & `pandapipes-0.9.0/src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/io/test_file_io.py` & `pandapipes-0.9.0/src/pandapipes/test/io/test_file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import pandapipes
 import pytest
 from pandas.testing import assert_frame_equal
 from pandapipes.test.multinet.test_control_multinet import get_gas_example, get_power_example_simple
 from pandapipes.multinet.create_multinet import create_empty_multinet, add_nets_to_multinet
 from pandapipes.multinet import MultiNet
-from pandapower.toolbox import nets_equal as nets_equal_pandapower
+from pandapower import nets_equal as nets_equal_pandapower
 from pandapipes.toolbox import nets_equal
 
 
 # @pytest.fixture()
 def load_net():
     # create test network
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_aux_function.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_aux_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 from pandapipes.pf.internals_toolbox import select_from_pit
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_special_networks.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_special_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import numpy as np
 import pytest
@@ -113,12 +113,12 @@
 
 
 @pytest.mark.xfail(reason="The test net is not set up properly.")
 def test_wild_indexing(create_net_changed_indices):
     net = copy.deepcopy(create_net_changed_indices)
 
     pandapipes.pipeflow(net)
-    assert net["converged"]
+    assert net.converged
 
 
 if __name__ == "__main__":
     pytest.main([r'pandapipes/test/api/test_special_networks.py'])
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_create.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import pytest
 import pandapipes
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_std_types.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_std_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 
 import pytest
 
 import pandapipes
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_convert_format.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_convert_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 from pandapipes import pp_dir
 import pandapipes as pp
 import numpy as np
 import os
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_network_tables.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_network_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import pandapipes
 from pandapipes.component_models import Sink, Source, Pump, \
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_time_series.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_time_series.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_ext_grid.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_ext_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_heat_exchanger.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_heat_exchanger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_valve.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_valve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_flow_control.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_flow_control.py`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pump.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pressure_control.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pressure_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_compressor.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_compressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pytest
 
 import pandapipes
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_pipe_results.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_pipe_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import numpy as np
 import pytest
 
 import pandapipes
 from pandapipes.properties.fluids import _add_fluid_to_net
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_mass_storage.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_mass_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pytest
 
 import pandapipes
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_mass.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/test_components/test_circ_pump_pressure.py` & `pandapipes-0.9.0/src/pandapipes/test/api/test_components/test_circ_pump_pressure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.1.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.4.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.4.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.7.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.7.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.3_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.3_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.6.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.6.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.5_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.5_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.1_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.1_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.4_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.4_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.2.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.1.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.1.1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.2_gas.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.2_gas.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.5.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.5.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.2.0.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.2.0.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/api/old_versions/example_0.8.0_water.json` & `pandapipes-0.9.0/src/pandapipes/test/api/old_versions/example_0.8.0_water.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py` & `pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 import pytest
 import numpy as np
 import pandapipes.networks.simple_water_networks as nw
```

## Comparing `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py` & `pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import statistics as st
 
 import numpy as np
 import pandas as pd
```

## Comparing `pandapipes-0.8.5/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py` & `pandapipes-0.9.0/src/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 import pytest
 import numpy as np
 import pandapipes.networks.simple_heat_transfer_networks as nw
```

## Comparing `pandapipes-0.8.5/pandapipes/test/plotting/test_simple_collections.py` & `pandapipes-0.9.0/src/pandapipes/test/plotting/test_simple_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import pandapipes
 import pandapipes.plotting as plot
```

## Comparing `pandapipes-0.8.5/pandapipes/test/plotting/test_generic_coordinates.py` & `pandapipes-0.9.0/src/pandapipes/test/plotting/test_generic_coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import pytest
 import copy
 from pandapipes.plotting.generic_geodata import create_generic_coordinates
 from pandapipes.test.test_toolbox import base_net_is_with_pumps
```

## Comparing `pandapipes-0.8.5/pandapipes/test/plotting/test_pipeflow_results.py` & `pandapipes-0.9.0/src/pandapipes/test/plotting/test_pipeflow_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 
 import pandapipes.plotting as plot
 import numpy as np
 import pandapipes as pp
```

## Comparing `pandapipes-0.8.5/pandapipes/test/plotting/test_collections.py` & `pandapipes-0.9.0/src/pandapipes/test/plotting/test_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import copy
 
 import numpy as np
 import pytest
```

## Comparing `pandapipes-0.8.5/pandapipes/test/properties/test_fluid_specials.py` & `pandapipes-0.9.0/src/pandapipes/test/properties/test_fluid_specials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import pytest
 import pandapipes
 from pandapipes.properties.fluids import _add_fluid_to_net
```

## Comparing `pandapipes-0.8.5/pandapipes/test/properties/test_properties_toolbox.py` & `pandapipes-0.9.0/src/pandapipes/test/properties/test_properties_toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import pandas as pd
 import numpy as np
 import os
 from pandapipes import pp_dir
```

## Comparing `pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_water_stanet.py` & `pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_water_stanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandapipes.networks.simple_water_networks as nw
 import pytest
 from pandapipes.pipeflow import logger as pf_logger
```

## Comparing `pandapipes-0.8.5/pandapipes/test/stanet_comparison/test_gas_stanet.py` & `pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/test_gas_stanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandapipes.networks.simple_gas_networks as nw
 import pytest
 from pandapipes.pipeflow import logger as pf_logger
```

## Comparing `pandapipes-0.8.5/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py` & `pandapipes-0.9.0/src/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import numpy as np
 import pandapipes
 import pandas as pd
 from pandapipes.properties.fluids import get_fluid
```

## Comparing `pandapipes-0.8.5/pandapipes/test/networks/test_networks.py` & `pandapipes-0.9.0/src/pandapipes/test/networks/test_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import pandapipes as pp
 import pytest
 from pandapipes import networks
```

## Comparing `pandapipes-0.8.5/pandapipes/networks/nw_aux.py` & `pandapipes-0.9.0/src/pandapipes/networks/nw_aux.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 method_transfer_dict = {"n": "Nikuradse", "nik": "Nikuradse", "nikuradse": "Nikuradse",
                         "pc": "Prandtl-Colebrook", "prandtl": "Prandtl-Colebrook",
                         "prandtl-colebrook": "Prandtl-Colebrook", "sj": "Swamee-Jain",
                         "swamee": "Swamee-Jain", "jain": "Swamee-Jain", "s": "Swamee-Jain",
```

## Comparing `pandapipes-0.8.5/pandapipes/networks/simple_water_networks.py` & `pandapipes-0.9.0/src/pandapipes/networks/simple_water_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 from pandapipes.io.file_io import from_json
 from pandapipes import pp_dir
 from pandapipes.networks.nw_aux import log_result_upon_loading
```

## Comparing `pandapipes-0.8.5/pandapipes/networks/simple_heat_transfer_networks.py` & `pandapipes-0.9.0/src/pandapipes/networks/simple_heat_transfer_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 from pandapipes.io.file_io import from_json
 from pandapipes import pp_dir
 try:
```

## Comparing `pandapipes-0.8.5/pandapipes/networks/simple_gas_networks.py` & `pandapipes-0.9.0/src/pandapipes/networks/simple_gas_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2023 by Fraunhofer Institute for Energy Economics
+# Copyright (c) 2020-2024 by Fraunhofer Institute for Energy Economics
 # and Energy System Technology (IEE), Kassel, and University of Kassel. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be found in the LICENSE file.
 
 import os
 from pandapipes.io.file_io import from_json
 from pandapipes import pp_dir, drop_junctions
 from pandapipes.networks.nw_aux import log_result_upon_loading
```

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json` & `pandapipes-0.9.0/src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json`

 * *Files identical despite different names*

## Comparing `pandapipes-0.8.5/pandapipes.egg-info/PKG-INFO` & `pandapipes-0.9.0/src/pandapipes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandapipes
-Version: 0.8.5
+Version: 0.9.0
 Summary: A pipeflow calculation tool that complements pandapower in the simulation of multi energy grids
 Home-page: http://www.pandapipes.org
 Author: Simon Ruben Drauz-Mauel, Daniel Lohmeier, Jolando Marius Kisse
 Author-email: simon.ruben.drauz-mauel@iee.fraunhofer.de, daniel.lohmeier@retoflow.de, jolando.kisse@uni-kassel.de
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -12,17 +12,18 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: plotting
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
@@ -42,18 +43,14 @@
    :target: https://pypi.python.org/pypi/pandapipes
    :alt: versions
 
 .. image:: https://readthedocs.org/projects/pandapipes/badge/
    :target: http://pandapipes.readthedocs.io/
    :alt: docs
 
-.. image:: https://travis-ci.org/e2nIEE/pandapipes.svg?branch=master
-   :target: https://travis-ci.org/e2nIEE/pandapipes/branches
-   :alt: travis
-
 .. image:: https://codecov.io/gh/e2nIEE/pandapipes/branch/master/graph/badge.svg
    :target: https://codecov.io/github/e2nIEE/pandapipes?branch=master
    :alt: codecov
 
 .. image:: https://api.codacy.com/project/badge/Grade/86c876ab23fc40d98e85f7d59bdef928
    :target: https://app.codacy.com/gh/e2nIEE/pandapipes/dashboard
    :alt: Codacy Badge
@@ -109,14 +106,40 @@
 We welcome contributions to pandapipes of any kind - if you want to contribute, please check out
 the `pandapipes contribution guidelines <https://github.com/e2nIEE/pandapipes/blob/develop/CONTRIBUTING.rst>`_.
 
 
 Change Log
 =============
 
+[0.9.0] - 2023-12-22
+-------------------------------
+
+- [ADDED] multiple creation of heat exchanger
+- [ADDED] support Python 3.11 (now included in test pipeline)
+- [ADDED] after the connectivity check, intercept the pipeflow if no more nodes are in-service (heat and hydraulic)
+- [ADDED] adding biomethane (pure and treated) as additonal fluid
+- [ADDED] result tables can be assembled modularly
+- [CHANGED] dropped support for Python 3.7 (no longer included in test pipeline)
+- [CHANGED] connectivity check now separated by hydraulics and heat_transfer calculation, so that also results can differ in some rows (NaN or not)
+- [CHANGED] dynamic creation of lookups for getting pit as pandas tables
+- [CHANGED] components can have their own internal arrays for specific calculations (e.g. for compressor pressure ratio), so that the pit does not need to include such component specific entries
+- [CHANGED] .readthedocs.yml due to deprecation
+- [CHANGED] changing from setuptools flat-layout into src-layout
+- [CHANGED] calculate thermal derivative globally, adaptions before/after can be done component-wise
+- [CHANGED] moving 'PipeflowNotConverged' error from pipeflow to pipeflow_setup
+- [CHANGED] moving 'result_extraction' under pf folder
+- [FIXED] in STANET converter: bug fix for heat exchanger creation and external temperatures of pipes added
+- [FIXED] build igraph considers all components
+- [FIXED] creating nxgraph and considering pressure circulation pumps correctly
+- [FIXED] error in tutorial 'circular flow in a district heating grid'
+- [FIXED] caused error during 'pip install pandapipes'
+- [REMOVED] broken travis badge removed from readme
+- [REMOVED] branch TINIT removed as it is not a solution variable, temperature determined on the fly
+- [REMOVED] 'converged' setting from options
+
 [0.8.5] - 2023-06-19
 -------------------------------
 - [FIXED] consider ambient pressure in calculation of compression power for pumps/compressors
 - [FIXED] np.bool error in pipeflow calculation due to deprecation of np.bool
 - [FIXED] use igraph package instead of python-igraph (has been renamed)
 - [ADDED] gas specific calculation of heat capacity ration kappa = cp/cv (for pumps/compressors)
 - [REMOVED] Python 3.7 removed from test pipeline due to inconsistencies with pandapower
```

## Comparing `pandapipes-0.8.5/pandapipes.egg-info/SOURCES.txt` & `pandapipes-0.9.0/src/pandapipes.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,378 +4,400 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 .github/workflows/release.yml
 .github/workflows/run_tests_develop.yml
 .github/workflows/run_tests_master.yml
-pandapipes/__init__.py
-pandapipes/constants.py
-pandapipes/create.py
-pandapipes/idx_branch.py
-pandapipes/idx_node.py
-pandapipes/pandapipes_net.py
-pandapipes/pipeflow.py
-pandapipes/toolbox.py
-pandapipes.egg-info/PKG-INFO
-pandapipes.egg-info/SOURCES.txt
-pandapipes.egg-info/dependency_links.txt
-pandapipes.egg-info/requires.txt
-pandapipes.egg-info/top_level.txt
-pandapipes/component_models/__init__.py
-pandapipes/component_models/circulation_pump_mass_component.py
-pandapipes/component_models/circulation_pump_pressure_component.py
-pandapipes/component_models/component_toolbox.py
-pandapipes/component_models/compressor_component.py
-pandapipes/component_models/ext_grid_component.py
-pandapipes/component_models/flow_control_component.py
-pandapipes/component_models/heat_exchanger_component.py
-pandapipes/component_models/junction_component.py
-pandapipes/component_models/mass_storage_component.py
-pandapipes/component_models/pipe_component.py
-pandapipes/component_models/pressure_control_component.py
-pandapipes/component_models/pump_component.py
-pandapipes/component_models/sink_component.py
-pandapipes/component_models/source_component.py
-pandapipes/component_models/valve_component.py
-pandapipes/component_models/abstract_models/__init__.py
-pandapipes/component_models/abstract_models/base_component.py
-pandapipes/component_models/abstract_models/branch_models.py
-pandapipes/component_models/abstract_models/branch_w_internals_models.py
-pandapipes/component_models/abstract_models/branch_wo_internals_models.py
-pandapipes/component_models/abstract_models/branch_wzerolength_models.py
-pandapipes/component_models/abstract_models/circulation_pump.py
-pandapipes/component_models/abstract_models/const_flow_models.py
-pandapipes/component_models/abstract_models/node_element_models.py
-pandapipes/component_models/abstract_models/node_models.py
-pandapipes/control/__init__.py
-pandapipes/control/run_control.py
-pandapipes/converter/__init__.py
-pandapipes/converter/stanet/__init__.py
-pandapipes/converter/stanet/data_cleaning.py
-pandapipes/converter/stanet/preparing_steps.py
-pandapipes/converter/stanet/stanet2pandapipes.py
-pandapipes/converter/stanet/table_creation.py
-pandapipes/converter/stanet/valve_pipe_component/__init__.py
-pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
-pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
-pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
-pandapipes/io/__init__.py
-pandapipes/io/convert_format.py
-pandapipes/io/file_io.py
-pandapipes/io/io_utils.py
-pandapipes/multinet/__init__.py
-pandapipes/multinet/create_multinet.py
-pandapipes/multinet/multinet.py
-pandapipes/multinet/control/__init__.py
-pandapipes/multinet/control/run_control_multinet.py
-pandapipes/multinet/control/controller/__init__.py
-pandapipes/multinet/control/controller/multinet_control.py
-pandapipes/multinet/timeseries/__init__.py
-pandapipes/multinet/timeseries/run_time_series_multinet.py
-pandapipes/networks/__init__.py
-pandapipes/networks/nw_aux.py
-pandapipes/networks/simple_gas_networks.py
-pandapipes/networks/simple_heat_transfer_networks.py
-pandapipes/networks/simple_water_networks.py
-pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
-pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
-pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
-pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
-pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
-pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
-pandapipes/pf/__init__.py
-pandapipes/pf/build_system_matrix.py
-pandapipes/pf/derivative_calculation.py
-pandapipes/pf/derivative_toolbox.py
-pandapipes/pf/derivative_toolbox_numba.py
-pandapipes/pf/internals_toolbox.py
-pandapipes/pf/pipeflow_setup.py
-pandapipes/pf/result_extraction.py
-pandapipes/plotting/__init__.py
-pandapipes/plotting/collections.py
-pandapipes/plotting/generic_geodata.py
-pandapipes/plotting/geo.py
-pandapipes/plotting/patch_makers.py
-pandapipes/plotting/pipeflow_results.py
-pandapipes/plotting/plotting_toolbox.py
-pandapipes/plotting/simple_plot.py
-pandapipes/properties/__init__.py
-pandapipes/properties/fluids.py
-pandapipes/properties/properties_toolbox.py
-pandapipes/properties/air/compressibility.txt
-pandapipes/properties/air/density.txt
-pandapipes/properties/air/der_compressibility.txt
-pandapipes/properties/air/heat_capacity.txt
-pandapipes/properties/air/molar_mass.txt
-pandapipes/properties/air/viscosity.txt
-pandapipes/properties/carbondioxide/density.txt
-pandapipes/properties/carbondioxide/heat_capacity.txt
-pandapipes/properties/carbondioxide/molar_mass.txt
-pandapipes/properties/carbondioxide/viscosity.txt
-pandapipes/properties/ethane/density.txt
-pandapipes/properties/ethane/heat_capacity.txt
-pandapipes/properties/ethane/molar_mass.txt
-pandapipes/properties/ethane/viscosity.txt
-pandapipes/properties/hgas/compressibility.txt
-pandapipes/properties/hgas/density.txt
-pandapipes/properties/hgas/der_compressibility.txt
-pandapipes/properties/hgas/heat_capacity.txt
-pandapipes/properties/hgas/higher_heating_value.txt
-pandapipes/properties/hgas/lower_heating_value.txt
-pandapipes/properties/hgas/molar_mass.txt
-pandapipes/properties/hgas/viscosity.txt
-pandapipes/properties/hydrogen/compressibility.txt
-pandapipes/properties/hydrogen/density.txt
-pandapipes/properties/hydrogen/der_compressibility.txt
-pandapipes/properties/hydrogen/heat_capacity.txt
-pandapipes/properties/hydrogen/higher_heating_value.txt
-pandapipes/properties/hydrogen/lower_heating_value.txt
-pandapipes/properties/hydrogen/molar_mass.txt
-pandapipes/properties/hydrogen/viscosity.txt
-pandapipes/properties/lgas/compressibility.txt
-pandapipes/properties/lgas/density.txt
-pandapipes/properties/lgas/der_compressibility.txt
-pandapipes/properties/lgas/heat_capacity.txt
-pandapipes/properties/lgas/higher_heating_value.txt
-pandapipes/properties/lgas/lower_heating_value.txt
-pandapipes/properties/lgas/molar_mass.txt
-pandapipes/properties/lgas/viscosity.txt
-pandapipes/properties/methane/compressibility.txt
-pandapipes/properties/methane/density.txt
-pandapipes/properties/methane/der_compressibility.txt
-pandapipes/properties/methane/heat_capacity.txt
-pandapipes/properties/methane/higher_heating_value.txt
-pandapipes/properties/methane/lower_heating_value.txt
-pandapipes/properties/methane/molar_mass.txt
-pandapipes/properties/methane/viscosity.txt
-pandapipes/properties/nitrogen/density.txt
-pandapipes/properties/nitrogen/heat_capacity.txt
-pandapipes/properties/nitrogen/molar_mass.txt
-pandapipes/properties/nitrogen/viscosity.txt
-pandapipes/properties/oxygen/density.txt
-pandapipes/properties/oxygen/heat_capacity.txt
-pandapipes/properties/oxygen/molar_mass.txt
-pandapipes/properties/oxygen/viscosity.txt
-pandapipes/properties/water/compressibility.txt
-pandapipes/properties/water/density.txt
-pandapipes/properties/water/der_compressibility.txt
-pandapipes/properties/water/heat_capacity.txt
-pandapipes/properties/water/molar_mass.txt
-pandapipes/properties/water/viscosity.txt
-pandapipes/std_types/__init__.py
-pandapipes/std_types/std_type_class.py
-pandapipes/std_types/std_types.py
-pandapipes/std_types/library/Pipe.csv
-pandapipes/std_types/library/Pump/P1.csv
-pandapipes/std_types/library/Pump/P2.csv
-pandapipes/std_types/library/Pump/P3.csv
-pandapipes/test/__init__.py
-pandapipes/test/run_tests.py
-pandapipes/test/test_imports.py
-pandapipes/test/test_toolbox.py
-pandapipes/test/api/__init__.py
-pandapipes/test/api/test_aux_function.py
-pandapipes/test/api/test_convert_format.py
-pandapipes/test/api/test_create.py
-pandapipes/test/api/test_network_tables.py
-pandapipes/test/api/test_special_networks.py
-pandapipes/test/api/test_std_types.py
-pandapipes/test/api/test_time_series.py
-pandapipes/test/api/old_versions/example_0.1.0.json
-pandapipes/test/api/old_versions/example_0.1.1.json
-pandapipes/test/api/old_versions/example_0.1.2.json
-pandapipes/test/api/old_versions/example_0.2.0.json
-pandapipes/test/api/old_versions/example_0.4.0.json
-pandapipes/test/api/old_versions/example_0.5.0.json
-pandapipes/test/api/old_versions/example_0.6.0.json
-pandapipes/test/api/old_versions/example_0.7.0.json
-pandapipes/test/api/old_versions/example_0.8.0_gas.json
-pandapipes/test/api/old_versions/example_0.8.0_water.json
-pandapipes/test/api/old_versions/example_0.8.1_gas.json
-pandapipes/test/api/old_versions/example_0.8.1_water.json
-pandapipes/test/api/old_versions/example_0.8.2_gas.json
-pandapipes/test/api/old_versions/example_0.8.2_water.json
-pandapipes/test/api/old_versions/example_0.8.3_gas.json
-pandapipes/test/api/old_versions/example_0.8.3_water.json
-pandapipes/test/api/old_versions/example_0.8.4_gas.json
-pandapipes/test/api/old_versions/example_0.8.4_water.json
-pandapipes/test/api/old_versions/example_0.8.5_gas.json
-pandapipes/test/api/old_versions/example_0.8.5_water.json
-pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
-pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
-pandapipes/test/api/test_components/__init__.py
-pandapipes/test/api/test_components/test_circ_pump_mass.py
-pandapipes/test/api/test_components/test_circ_pump_pressure.py
-pandapipes/test/api/test_components/test_compressor.py
-pandapipes/test/api/test_components/test_ext_grid.py
-pandapipes/test/api/test_components/test_flow_control.py
-pandapipes/test/api/test_components/test_heat_exchanger.py
-pandapipes/test/api/test_components/test_mass_storage.py
-pandapipes/test/api/test_components/test_pipe_results.py
-pandapipes/test/api/test_components/test_pressure_control.py
-pandapipes/test/api/test_components/test_pump.py
-pandapipes/test/api/test_components/test_valve.py
-pandapipes/test/converter/__init__.py
-pandapipes/test/converter/test_stanet_converter.py
-pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
-pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
-pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
-pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
-pandapipes/test/io/__init__.py
-pandapipes/test/io/test_file_io.py
-pandapipes/test/multinet/__init__.py
-pandapipes/test/multinet/test_control_multinet.py
-pandapipes/test/multinet/test_time_series_multinet.py
-pandapipes/test/networks/__init__.py
-pandapipes/test/networks/test_networks.py
-pandapipes/test/openmodelica_comparison/__init__.py
-pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
-pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
-pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
-pandapipes/test/pipeflow_internals/__init__.py
-pandapipes/test/pipeflow_internals/test_inservice.py
-pandapipes/test/pipeflow_internals/test_non_convergence.py
-pandapipes/test/pipeflow_internals/test_options.py
-pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
-pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
-pandapipes/test/pipeflow_internals/test_time_series.py
-pandapipes/test/pipeflow_internals/test_update_matrix.py
-pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
-pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
-pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
-pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
-pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
-pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
-pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
-pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
-pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
-pandapipes/test/pipeflow_internals/data/hydraulics.csv
-pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
-pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
-pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
-pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
-pandapipes/test/pipeflow_internals/data/test_pump.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
-pandapipes/test/pipeflow_internals/data/test_valve.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
-pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
-pandapipes/test/plotting/__init__.py
-pandapipes/test/plotting/test_collections.py
-pandapipes/test/plotting/test_generic_coordinates.py
-pandapipes/test/plotting/test_pipeflow_results.py
-pandapipes/test/plotting/test_simple_collections.py
-pandapipes/test/properties/__init__.py
-pandapipes/test/properties/test_fluid_specials.py
-pandapipes/test/properties/test_properties_toolbox.py
-pandapipes/test/stanet_comparison/__init__.py
-pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
-pandapipes/test/stanet_comparison/test_gas_stanet.py
-pandapipes/test/stanet_comparison/test_water_stanet.py
-pandapipes/timeseries/__init__.py
-pandapipes/timeseries/run_time_series.py
-pandapipes/topology/__init__.py
-pandapipes/topology/create_graph.py
-pandapipes/topology/graph_searches.py
+src/pandapipes/__init__.py
+src/pandapipes/constants.py
+src/pandapipes/create.py
+src/pandapipes/idx_branch.py
+src/pandapipes/idx_node.py
+src/pandapipes/pandapipes_net.py
+src/pandapipes/pipeflow.py
+src/pandapipes/toolbox.py
+src/pandapipes.egg-info/PKG-INFO
+src/pandapipes.egg-info/SOURCES.txt
+src/pandapipes.egg-info/dependency_links.txt
+src/pandapipes.egg-info/requires.txt
+src/pandapipes.egg-info/top_level.txt
+src/pandapipes/component_models/__init__.py
+src/pandapipes/component_models/circulation_pump_mass_component.py
+src/pandapipes/component_models/circulation_pump_pressure_component.py
+src/pandapipes/component_models/component_toolbox.py
+src/pandapipes/component_models/compressor_component.py
+src/pandapipes/component_models/ext_grid_component.py
+src/pandapipes/component_models/flow_control_component.py
+src/pandapipes/component_models/heat_exchanger_component.py
+src/pandapipes/component_models/junction_component.py
+src/pandapipes/component_models/mass_storage_component.py
+src/pandapipes/component_models/pipe_component.py
+src/pandapipes/component_models/pressure_control_component.py
+src/pandapipes/component_models/pump_component.py
+src/pandapipes/component_models/sink_component.py
+src/pandapipes/component_models/source_component.py
+src/pandapipes/component_models/valve_component.py
+src/pandapipes/component_models/abstract_models/__init__.py
+src/pandapipes/component_models/abstract_models/base_component.py
+src/pandapipes/component_models/abstract_models/branch_models.py
+src/pandapipes/component_models/abstract_models/branch_w_internals_models.py
+src/pandapipes/component_models/abstract_models/branch_wo_internals_models.py
+src/pandapipes/component_models/abstract_models/branch_wzerolength_models.py
+src/pandapipes/component_models/abstract_models/circulation_pump.py
+src/pandapipes/component_models/abstract_models/const_flow_models.py
+src/pandapipes/component_models/abstract_models/node_element_models.py
+src/pandapipes/component_models/abstract_models/node_models.py
+src/pandapipes/control/__init__.py
+src/pandapipes/control/run_control.py
+src/pandapipes/converter/stanet/__init__.py
+src/pandapipes/converter/stanet/data_cleaning.py
+src/pandapipes/converter/stanet/preparing_steps.py
+src/pandapipes/converter/stanet/stanet2pandapipes.py
+src/pandapipes/converter/stanet/table_creation.py
+src/pandapipes/converter/stanet/valve_pipe_component/__init__.py
+src/pandapipes/converter/stanet/valve_pipe_component/create_valve_pipe.py
+src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_component.py
+src/pandapipes/converter/stanet/valve_pipe_component/valve_pipe_plotting.py
+src/pandapipes/io/__init__.py
+src/pandapipes/io/convert_format.py
+src/pandapipes/io/file_io.py
+src/pandapipes/io/io_utils.py
+src/pandapipes/multinet/__init__.py
+src/pandapipes/multinet/create_multinet.py
+src/pandapipes/multinet/multinet.py
+src/pandapipes/multinet/control/__init__.py
+src/pandapipes/multinet/control/run_control_multinet.py
+src/pandapipes/multinet/control/controller/__init__.py
+src/pandapipes/multinet/control/controller/multinet_control.py
+src/pandapipes/multinet/timeseries/__init__.py
+src/pandapipes/multinet/timeseries/run_time_series_multinet.py
+src/pandapipes/networks/__init__.py
+src/pandapipes/networks/nw_aux.py
+src/pandapipes/networks/simple_gas_networks.py
+src/pandapipes/networks/simple_heat_transfer_networks.py
+src/pandapipes/networks/simple_water_networks.py
+src/pandapipes/networks/network_files/gas_net_schutterwald_1bar.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/delta_2sinks.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/heights.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_pipe.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/one_source.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/section_variation.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/t_cross.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/heat_transfer_cases/two_pipes.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/mixed_net.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/combined_networks/versatility.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/delta.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/heights.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/pumps.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/meshed_networks/two_valves.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_1.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_2.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/one_pipe/pipe_3.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/cross_3ext.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/strand_net.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pipes.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/strand_net/two_pumps.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/t_cross.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/t_cross/valves.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_colebrook/two_pressure_junctions/two_pipes.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/mixed_net.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/combined_networks/versatility.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/delta.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/heights.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/one_valve_stanet.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/pumps.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/meshed_networks/two_valves.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_1.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_2.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/one_pipe/pipe_3.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/cross_3ext.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation1.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/strand_net_stanet_variation2.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pipes.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/strand_net/two_pumps.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/t_cross.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/t_cross/valves.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/one_pipe_stanet.json
+src/pandapipes/networks/network_files/openmodelica_test_networks/water_cases_swamee-jain/two_pressure_junctions/two_pipes.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural1--0-sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural2--0-sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-rural3--0-sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb4--0-sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-semiurb5--0-sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-no_sw.json
+src/pandapipes/networks/network_files/simbench_test_networks/1-LV-urban6--0-sw.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/parallel_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/combined_networks/versatility_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/delta_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/pumps_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/square_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/meshed_networks/two_valves_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_1_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/one_pipe/pipe_2_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/pump_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/strand_net/two_pipes_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross1_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/t_cross/t_cross2_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/gas_cases/two_pressure_junctions/H_net_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/district_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/combined_networks/versatility_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/delta_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/pumps_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/meshed_networks/two_valves_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_1_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_2_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/one_pipe/pipe_3_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/cross_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/pump_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/strand_net_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/strand_net/two_pipes_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/t_cross/t_cross_PC.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_N.json
+src/pandapipes/networks/network_files/stanet_test_networks/water_cases/two_pressure_junctions/two_pipes_PC.json
+src/pandapipes/pf/__init__.py
+src/pandapipes/pf/build_system_matrix.py
+src/pandapipes/pf/derivative_calculation.py
+src/pandapipes/pf/derivative_toolbox.py
+src/pandapipes/pf/derivative_toolbox_numba.py
+src/pandapipes/pf/internals_toolbox.py
+src/pandapipes/pf/pipeflow_setup.py
+src/pandapipes/pf/result_extraction.py
+src/pandapipes/plotting/__init__.py
+src/pandapipes/plotting/collections.py
+src/pandapipes/plotting/generic_geodata.py
+src/pandapipes/plotting/geo.py
+src/pandapipes/plotting/patch_makers.py
+src/pandapipes/plotting/pipeflow_results.py
+src/pandapipes/plotting/plotting_toolbox.py
+src/pandapipes/plotting/simple_plot.py
+src/pandapipes/properties/__init__.py
+src/pandapipes/properties/fluids.py
+src/pandapipes/properties/properties_toolbox.py
+src/pandapipes/properties/air/compressibility.txt
+src/pandapipes/properties/air/density.txt
+src/pandapipes/properties/air/der_compressibility.txt
+src/pandapipes/properties/air/heat_capacity.txt
+src/pandapipes/properties/air/molar_mass.txt
+src/pandapipes/properties/air/viscosity.txt
+src/pandapipes/properties/biomethane_pure/compressibility.txt
+src/pandapipes/properties/biomethane_pure/density.txt
+src/pandapipes/properties/biomethane_pure/der_compressibility.txt
+src/pandapipes/properties/biomethane_pure/gas_composition.txt
+src/pandapipes/properties/biomethane_pure/heat_capacity.txt
+src/pandapipes/properties/biomethane_pure/higher_heating_value.txt
+src/pandapipes/properties/biomethane_pure/molar_mass.txt
+src/pandapipes/properties/biomethane_pure/viscosity.txt
+src/pandapipes/properties/biomethane_treated/compressibility.txt
+src/pandapipes/properties/biomethane_treated/density.txt
+src/pandapipes/properties/biomethane_treated/der_compressibility.txt
+src/pandapipes/properties/biomethane_treated/gas_composition.txt
+src/pandapipes/properties/biomethane_treated/heat_capacity.txt
+src/pandapipes/properties/biomethane_treated/higher_heating_value.txt
+src/pandapipes/properties/biomethane_treated/molar_mass.txt
+src/pandapipes/properties/biomethane_treated/viscosity.txt
+src/pandapipes/properties/carbondioxide/density.txt
+src/pandapipes/properties/carbondioxide/heat_capacity.txt
+src/pandapipes/properties/carbondioxide/molar_mass.txt
+src/pandapipes/properties/carbondioxide/viscosity.txt
+src/pandapipes/properties/ethane/density.txt
+src/pandapipes/properties/ethane/heat_capacity.txt
+src/pandapipes/properties/ethane/molar_mass.txt
+src/pandapipes/properties/ethane/viscosity.txt
+src/pandapipes/properties/hgas/compressibility.txt
+src/pandapipes/properties/hgas/density.txt
+src/pandapipes/properties/hgas/der_compressibility.txt
+src/pandapipes/properties/hgas/heat_capacity.txt
+src/pandapipes/properties/hgas/higher_heating_value.txt
+src/pandapipes/properties/hgas/lower_heating_value.txt
+src/pandapipes/properties/hgas/molar_mass.txt
+src/pandapipes/properties/hgas/viscosity.txt
+src/pandapipes/properties/hydrogen/compressibility.txt
+src/pandapipes/properties/hydrogen/density.txt
+src/pandapipes/properties/hydrogen/der_compressibility.txt
+src/pandapipes/properties/hydrogen/heat_capacity.txt
+src/pandapipes/properties/hydrogen/higher_heating_value.txt
+src/pandapipes/properties/hydrogen/lower_heating_value.txt
+src/pandapipes/properties/hydrogen/molar_mass.txt
+src/pandapipes/properties/hydrogen/viscosity.txt
+src/pandapipes/properties/lgas/compressibility.txt
+src/pandapipes/properties/lgas/density.txt
+src/pandapipes/properties/lgas/der_compressibility.txt
+src/pandapipes/properties/lgas/heat_capacity.txt
+src/pandapipes/properties/lgas/higher_heating_value.txt
+src/pandapipes/properties/lgas/lower_heating_value.txt
+src/pandapipes/properties/lgas/molar_mass.txt
+src/pandapipes/properties/lgas/viscosity.txt
+src/pandapipes/properties/methane/compressibility.txt
+src/pandapipes/properties/methane/density.txt
+src/pandapipes/properties/methane/der_compressibility.txt
+src/pandapipes/properties/methane/heat_capacity.txt
+src/pandapipes/properties/methane/higher_heating_value.txt
+src/pandapipes/properties/methane/lower_heating_value.txt
+src/pandapipes/properties/methane/molar_mass.txt
+src/pandapipes/properties/methane/viscosity.txt
+src/pandapipes/properties/nitrogen/density.txt
+src/pandapipes/properties/nitrogen/heat_capacity.txt
+src/pandapipes/properties/nitrogen/molar_mass.txt
+src/pandapipes/properties/nitrogen/viscosity.txt
+src/pandapipes/properties/oxygen/density.txt
+src/pandapipes/properties/oxygen/heat_capacity.txt
+src/pandapipes/properties/oxygen/molar_mass.txt
+src/pandapipes/properties/oxygen/viscosity.txt
+src/pandapipes/properties/water/compressibility.txt
+src/pandapipes/properties/water/density.txt
+src/pandapipes/properties/water/der_compressibility.txt
+src/pandapipes/properties/water/heat_capacity.txt
+src/pandapipes/properties/water/molar_mass.txt
+src/pandapipes/properties/water/viscosity.txt
+src/pandapipes/std_types/__init__.py
+src/pandapipes/std_types/std_type_class.py
+src/pandapipes/std_types/std_types.py
+src/pandapipes/std_types/library/Pipe.csv
+src/pandapipes/std_types/library/Pump/P1.csv
+src/pandapipes/std_types/library/Pump/P2.csv
+src/pandapipes/std_types/library/Pump/P3.csv
+src/pandapipes/test/__init__.py
+src/pandapipes/test/pytest.ini
+src/pandapipes/test/run_tests.py
+src/pandapipes/test/test_imports.py
+src/pandapipes/test/test_toolbox.py
+src/pandapipes/test/api/__init__.py
+src/pandapipes/test/api/test_aux_function.py
+src/pandapipes/test/api/test_convert_format.py
+src/pandapipes/test/api/test_create.py
+src/pandapipes/test/api/test_network_tables.py
+src/pandapipes/test/api/test_special_networks.py
+src/pandapipes/test/api/test_std_types.py
+src/pandapipes/test/api/test_time_series.py
+src/pandapipes/test/api/old_versions/example_0.1.0.json
+src/pandapipes/test/api/old_versions/example_0.1.1.json
+src/pandapipes/test/api/old_versions/example_0.1.2.json
+src/pandapipes/test/api/old_versions/example_0.2.0.json
+src/pandapipes/test/api/old_versions/example_0.4.0.json
+src/pandapipes/test/api/old_versions/example_0.5.0.json
+src/pandapipes/test/api/old_versions/example_0.6.0.json
+src/pandapipes/test/api/old_versions/example_0.7.0.json
+src/pandapipes/test/api/old_versions/example_0.8.0_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.0_water.json
+src/pandapipes/test/api/old_versions/example_0.8.1_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.1_water.json
+src/pandapipes/test/api/old_versions/example_0.8.2_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.2_water.json
+src/pandapipes/test/api/old_versions/example_0.8.3_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.3_water.json
+src/pandapipes/test/api/old_versions/example_0.8.4_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.4_water.json
+src/pandapipes/test/api/old_versions/example_0.8.5_gas.json
+src/pandapipes/test/api/old_versions/example_0.8.5_water.json
+src/pandapipes/test/api/old_versions/example_0.9.0_gas.json
+src/pandapipes/test/api/old_versions/example_0.9.0_water.json
+src/pandapipes/test/api/release_cycle/release_control_test_network.py
+src/pandapipes/test/api/release_cycle/release_control_test_sink_profiles.csv
+src/pandapipes/test/api/release_cycle/release_control_test_source_profiles.csv
+src/pandapipes/test/api/test_components/__init__.py
+src/pandapipes/test/api/test_components/test_circ_pump_mass.py
+src/pandapipes/test/api/test_components/test_circ_pump_pressure.py
+src/pandapipes/test/api/test_components/test_compressor.py
+src/pandapipes/test/api/test_components/test_ext_grid.py
+src/pandapipes/test/api/test_components/test_flow_control.py
+src/pandapipes/test/api/test_components/test_heat_exchanger.py
+src/pandapipes/test/api/test_components/test_mass_storage.py
+src/pandapipes/test/api/test_components/test_pipe_results.py
+src/pandapipes/test/api/test_components/test_pressure_control.py
+src/pandapipes/test/api/test_components/test_pump.py
+src/pandapipes/test/api/test_components/test_valve.py
+src/pandapipes/test/converter/__init__.py
+src/pandapipes/test/converter/test_stanet_converter.py
+src/pandapipes/test/converter/converter_test_files/Exampelonia_mini.csv
+src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_2valvepipe.csv
+src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_closed.csv
+src/pandapipes/test/converter/converter_test_files/Exampelonia_mini_with_valve_2sliders_open.csv
+src/pandapipes/test/io/__init__.py
+src/pandapipes/test/io/test_file_io.py
+src/pandapipes/test/multinet/__init__.py
+src/pandapipes/test/multinet/test_control_multinet.py
+src/pandapipes/test/multinet/test_time_series_multinet.py
+src/pandapipes/test/networks/__init__.py
+src/pandapipes/test/networks/test_networks.py
+src/pandapipes/test/openmodelica_comparison/__init__.py
+src/pandapipes/test/openmodelica_comparison/pipeflow_openmodelica_comparison.py
+src/pandapipes/test/openmodelica_comparison/test_heat_transfer_openmodelica.py
+src/pandapipes/test/openmodelica_comparison/test_water_openmodelica.py
+src/pandapipes/test/pipeflow_internals/__init__.py
+src/pandapipes/test/pipeflow_internals/test_inservice.py
+src/pandapipes/test/pipeflow_internals/test_non_convergence.py
+src/pandapipes/test/pipeflow_internals/test_options.py
+src/pandapipes/test/pipeflow_internals/test_pipeflow_analytic_comparison.py
+src/pandapipes/test/pipeflow_internals/test_pipeflow_modes.py
+src/pandapipes/test/pipeflow_internals/test_time_series.py
+src/pandapipes/test/pipeflow_internals/test_update_matrix.py
+src/pandapipes/test/pipeflow_internals/data/Temperature_2zu_2ab_an.csv
+src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_an.csv
+src/pandapipes/test/pipeflow_internals/data/Temperature_masche_1load_direction_an.csv
+src/pandapipes/test/pipeflow_internals/data/Temperature_one_pipe_an.csv
+src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2ab_1zu_an.csv
+src/pandapipes/test/pipeflow_internals/data/Temperature_tee_2zu_1ab_an.csv
+src/pandapipes/test/pipeflow_internals/data/ext_grid_p.csv
+src/pandapipes/test/pipeflow_internals/data/gas_sections_an.csv
+src/pandapipes/test/pipeflow_internals/data/heat_exchanger_test.csv
+src/pandapipes/test/pipeflow_internals/data/hydraulics.csv
+src/pandapipes/test/pipeflow_internals/data/pressure_control_test_analytical.csv
+src/pandapipes/test/pipeflow_internals/data/test_circ_pump_mass.csv
+src/pandapipes/test/pipeflow_internals/data/test_circ_pump_pressure.csv
+src/pandapipes/test/pipeflow_internals/data/test_pressure_control.csv
+src/pandapipes/test/pipeflow_internals/data/test_pump.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_sink_profiles.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_source_profiles.csv
+src/pandapipes/test/pipeflow_internals/data/test_valve.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_ext_grid/mdot_kg_per_s.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_junction/p_bar.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/lambda.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/reynolds.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_pipe/v_mean_m_per_s.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_sink/mdot_kg_per_s.csv
+src/pandapipes/test/pipeflow_internals/data/test_time_series_results/res_source/mdot_kg_per_s.csv
+src/pandapipes/test/plotting/__init__.py
+src/pandapipes/test/plotting/test_collections.py
+src/pandapipes/test/plotting/test_generic_coordinates.py
+src/pandapipes/test/plotting/test_pipeflow_results.py
+src/pandapipes/test/plotting/test_simple_collections.py
+src/pandapipes/test/properties/__init__.py
+src/pandapipes/test/properties/test_fluid_specials.py
+src/pandapipes/test/properties/test_properties_toolbox.py
+src/pandapipes/test/stanet_comparison/__init__.py
+src/pandapipes/test/stanet_comparison/pipeflow_stanet_comparison.py
+src/pandapipes/test/stanet_comparison/test_gas_stanet.py
+src/pandapipes/test/stanet_comparison/test_water_stanet.py
+src/pandapipes/test/topology/__init__.py
+src/pandapipes/test/topology/test_graph_searches.py
+src/pandapipes/test/topology/test_nxgraph.py
+src/pandapipes/timeseries/__init__.py
+src/pandapipes/timeseries/run_time_series.py
+src/pandapipes/topology/__init__.py
+src/pandapipes/topology/create_graph.py
+src/pandapipes/topology/graph_searches.py
```

