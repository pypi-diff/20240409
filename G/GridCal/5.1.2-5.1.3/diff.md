# Comparing `tmp/GridCal-5.1.2.tar.gz` & `tmp/GridCal-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCal-5.1.2.tar", last modified: Mon Apr  8 13:35:54 2024, max compression
+gzip compressed data, was "GridCal-5.1.3.tar", last modified: Tue Apr  9 15:59:24 2024, max compression
```

## Comparing `GridCal-5.1.2.tar` & `GridCal-5.1.3.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-08 13:34:15.971164 GridCal-5.1.2/GridCal/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.2/GridCal/ExecuteGridCal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.2/GridCal/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.2/GridCal/update.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.2/GridCal/templates.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.2/GridCal/Session/results_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Session/export_results_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Session/session.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Session/synchronization_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Session/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.2/GridCal/Session/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.2/GridCal/data/cables.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.2/GridCal/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      376 2023-11-16 09:36:26.518645 GridCal-5.1.2/GridCal/data/sequence_lines.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.2/GridCal/data/transformers.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.2/GridCal/data/wires.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.2/GridCal/Gui/GeneralDialogues.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/update_gui_all.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/messages.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/themes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.2/GridCal/Gui/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    85064 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/GuiFunctions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/plot_config.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/update_gui_common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/Widgets/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/Widgets/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/Widgets/custom_qrangeslider.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.2/GridCal/Gui/CoordinatesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.2/GridCal/Gui/CoordinatesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/CoordinatesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/CoordinatesInput/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.2/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/TowerBuilder/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/TowerBuilder/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.2/GridCal/Gui/TowerBuilder/table_models.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/TowerBuilder/test_.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Gui/TowerBuilder/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Gui/TowerBuilder/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.2/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/graphics_manager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.2/GridCal/Gui/Diagrams/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/diagrams_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   183254 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6687 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6203 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16999 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13480 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4212 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12258 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4852 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9421 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9431 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4683 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    32907 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30218 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21562 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30410 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   160152 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/node_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/map_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19136 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4856 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1854 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.2/GridCal/Gui/AboutDialogue/about_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.2/GridCal/Gui/AboutDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.2/GridCal/Gui/AboutDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.2/GridCal/Gui/AboutDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.2/GridCal/Gui/AboutDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/excel_dialog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/profiles_from_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.2/GridCal/Gui/ProfilesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.2/GridCal/Gui/ProfilesInput/models_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/ProfilesInput/profile_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/Analysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/Analysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/Analysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.2/GridCal/Gui/Analysis/AnalysisDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/Analysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.2/GridCal/Gui/Analysis/object_plot_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.2/GridCal/Gui/CascadingSteps/cascading_steps.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/CascadingSteps/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/CascadingSteps/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.2/GridCal/Gui/CascadingSteps/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.2/GridCal/Gui/Main/ConsoleLogController.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.2/GridCal/Gui/Main/GridCalMain.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   275842 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Main/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.2/GridCal/Gui/Main/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-08 13:34:15.959164 GridCal-5.1.2/GridCal/Gui/Main/ConsoleLog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   762387 2024-04-08 13:34:19.319164 GridCal-5.1.2/GridCal/Gui/Main/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/Main/object_select_window.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/README.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/simulations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33842 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/io.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/base_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Settings/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17616 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Settings/configuration.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45037 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/objects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20949 2024-03-28 10:16:48.960877 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/time_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    71734 2024-04-08 13:34:15.963164 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/diagrams.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Results/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Results/results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/Visualization/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/Visualization/visualization.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/Visualization/palettes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/SyncDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/SyncDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SyncDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Gui/SyncDialogue/sync_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SyncDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/RosetaExplorer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.2/GridCal/Gui/LoadDesigner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.2/GridCal/Gui/LoadDesigner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.2/GridCal/Gui/LoadDesigner/load_designer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.2/GridCal/Gui/LoadDesigner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.2/GridCal/Gui/LoadDesigner/load_designer_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.2/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/WindPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/WindPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/WindPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/WindPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.2/GridCal/Gui/SystemScaler/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.2/GridCal/Gui/SystemScaler/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.2/GridCal/Gui/SystemScaler/system_scaler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.2/GridCal/Gui/SystemScaler/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.2/GridCal/Gui/SystemScaler/system_scaler_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/TreeModelViewer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.2/GridCal/Gui/TreeModelViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/TreeModelViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.2/GridCal/Gui/TreeModelViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.2/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.2/GridCal/Gui/GridGenerator/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.2/GridCal/Gui/GridGenerator/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.2/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.2/GridCal/Gui/GridGenerator/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.2/GridCal/Gui/GridGenerator/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4902 2024-03-11 19:28:12.175075 GridCal-5.1.2/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-08 13:35:54.435167 GridCal-5.1.2/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-08 13:35:54.435167 GridCal-5.1.2/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-08 15:39:56.131418 GridCal-5.1.3/GridCal/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.3/GridCal/ExecuteGridCal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.3/GridCal/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.3/GridCal/update.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.3/GridCal/templates.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.3/GridCal/Session/results_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Session/export_results_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Session/session.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Session/synchronization_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Session/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7043 2024-04-08 13:34:15.971164 GridCal-5.1.3/GridCal/Session/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.3/GridCal/data/cables.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.3/GridCal/data/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      388 2024-04-09 12:55:36.988464 GridCal-5.1.3/GridCal/data/sequence_lines.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.3/GridCal/data/transformers.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.3/GridCal/data/wires.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.3/GridCal/Gui/GeneralDialogues.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/update_gui_all.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/messages.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/themes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.3/GridCal/Gui/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    85064 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/GuiFunctions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/plot_config.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/update_gui_common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/Widgets/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/Widgets/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/Widgets/custom_qrangeslider.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.3/GridCal/Gui/CoordinatesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.3/GridCal/Gui/CoordinatesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/CoordinatesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/CoordinatesInput/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.3/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/TowerBuilder/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/TowerBuilder/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.3/GridCal/Gui/TowerBuilder/table_models.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/TowerBuilder/test_.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Gui/TowerBuilder/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Gui/TowerBuilder/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.3/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6333 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/graphics_manager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.3/GridCal/Gui/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2695 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/diagrams_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   183547 2024-04-08 17:26:45.058329 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6687 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13045 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6090 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6203 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6079 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16999 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4879 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13480 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4338 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4212 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12258 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4852 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4371 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9421 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9485 2024-04-09 12:55:36.984464 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4683 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13960 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    32907 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6403 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6422 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5938 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5983 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6495 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6426 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-08 13:34:15.955164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5635 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19276 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30218 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21562 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30410 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   160152 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/node_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/map_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19136 2024-04-08 13:34:15.959164 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4856 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1854 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.3/GridCal/Gui/AboutDialogue/about_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.3/GridCal/Gui/AboutDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.3/GridCal/Gui/AboutDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.3/GridCal/Gui/AboutDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.3/GridCal/Gui/AboutDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/excel_dialog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/profiles_from_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.3/GridCal/Gui/ProfilesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.3/GridCal/Gui/ProfilesInput/models_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/ProfilesInput/profile_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/Analysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/Analysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/Analysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.3/GridCal/Gui/Analysis/AnalysisDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/Analysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.3/GridCal/Gui/Analysis/object_plot_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.3/GridCal/Gui/CascadingSteps/cascading_steps.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/CascadingSteps/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/CascadingSteps/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.3/GridCal/Gui/CascadingSteps/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.3/GridCal/Gui/Main/ConsoleLogController.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.3/GridCal/Gui/Main/GridCalMain.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   275391 2024-04-09 12:55:36.988464 GridCal-5.1.3/GridCal/Gui/Main/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.3/GridCal/Gui/Main/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-09 12:55:36.984464 GridCal-5.1.3/GridCal/Gui/Main/ConsoleLog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   807547 2024-04-09 12:55:36.988464 GridCal-5.1.3/GridCal/Gui/Main/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/Main/object_select_window.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/README.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)   110018 2024-04-08 13:34:15.963164 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/simulations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33842 2024-04-08 13:34:15.963164 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/io.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31266 2024-04-08 13:34:15.963164 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/base_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Settings/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17616 2024-04-08 13:34:15.963164 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Settings/configuration.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45037 2024-04-08 13:34:15.963164 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/objects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20949 2024-03-28 10:16:48.960877 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/time_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    71734 2024-04-08 17:25:24.166326 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/diagrams.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Results/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Results/results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/Visualization/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/Visualization/visualization.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/Visualization/palettes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/SyncDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/SyncDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SyncDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Gui/SyncDialogue/sync_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SyncDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/RosetaExplorer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.3/GridCal/Gui/LoadDesigner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.3/GridCal/Gui/LoadDesigner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.3/GridCal/Gui/LoadDesigner/load_designer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.3/GridCal/Gui/LoadDesigner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.3/GridCal/Gui/LoadDesigner/load_designer_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.3/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/WindPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/WindPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/WindPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/WindPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.3/GridCal/Gui/SystemScaler/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.3/GridCal/Gui/SystemScaler/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.3/GridCal/Gui/SystemScaler/system_scaler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.3/GridCal/Gui/SystemScaler/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.3/GridCal/Gui/SystemScaler/system_scaler_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/TreeModelViewer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.3/GridCal/Gui/TreeModelViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/TreeModelViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.3/GridCal/Gui/TreeModelViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.3/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.3/GridCal/Gui/GridGenerator/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.3/GridCal/Gui/GridGenerator/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.3/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.3/GridCal/Gui/GridGenerator/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.3/GridCal/Gui/GridGenerator/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4902 2024-03-11 19:28:12.175075 GridCal-5.1.3/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-09 15:59:24.856460 GridCal-5.1.3/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-09 15:59:24.856460 GridCal-5.1.3/setup.cfg
```

### Comparing `GridCal-5.1.2/GridCal/__version__.py` & `GridCal-5.1.3/GridCal/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCal_VERSION__ = "5.1.2"
+__GridCal_VERSION__ = "5.1.3"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCal_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCal-5.1.2/GridCal/__init__.py` & `GridCal-5.1.3/GridCal/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/ExecuteGridCal.py` & `GridCal-5.1.3/GridCal/ExecuteGridCal.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/LICENSE.txt` & `GridCal-5.1.3/GridCal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/update.py` & `GridCal-5.1.3/GridCal/update.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/templates.py` & `GridCal-5.1.3/GridCal/templates.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Session/results_model.py` & `GridCal-5.1.3/GridCal/Session/results_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Session/export_results_driver.py` & `GridCal-5.1.3/GridCal/Session/export_results_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Session/session.py` & `GridCal-5.1.3/GridCal/Session/session.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Session/synchronization_driver.py` & `GridCal-5.1.3/GridCal/Session/synchronization_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Session/file_handler.py` & `GridCal-5.1.3/GridCal/Session/file_handler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/data/cables.csv` & `GridCal-5.1.3/GridCal/data/cables.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/data/transformers.csv` & `GridCal-5.1.3/GridCal/data/transformers.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/data/wires.csv` & `GridCal-5.1.3/GridCal/data/wires.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/GeneralDialogues.py` & `GridCal-5.1.3/GridCal/Gui/GeneralDialogues.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/update_gui_all.py` & `GridCal-5.1.3/GridCal/Gui/update_gui_all.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/messages.py` & `GridCal-5.1.3/GridCal/Gui/messages.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/themes.py` & `GridCal-5.1.3/GridCal/Gui/themes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ConsoleWidget.py` & `GridCal-5.1.3/GridCal/Gui/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/GuiFunctions.py` & `GridCal-5.1.3/GridCal/Gui/GuiFunctions.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/plot_config.py` & `GridCal-5.1.3/GridCal/Gui/plot_config.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/update_gui_common.py` & `GridCal-5.1.3/GridCal/Gui/update_gui_common.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Widgets/matplotlibwidget.py` & `GridCal-5.1.3/GridCal/Gui/Widgets/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Widgets/custom_qrangeslider.py` & `GridCal-5.1.3/GridCal/Gui/Widgets/custom_qrangeslider.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ContingencyPlanner/gui.py` & `GridCal-5.1.3/GridCal/Gui/ContingencyPlanner/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/CoordinatesInput/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/CoordinatesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/CoordinatesInput/gui.py` & `GridCal-5.1.3/GridCal/Gui/CoordinatesInput/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TowerBuilder/table_models.py` & `GridCal-5.1.3/GridCal/Gui/TowerBuilder/table_models.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TowerBuilder/test_.py` & `GridCal-5.1.3/GridCal/Gui/TowerBuilder/test_.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TowerBuilder/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/TowerBuilder/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TowerBuilder/gui.py` & `GridCal-5.1.3/GridCal/Gui/TowerBuilder/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py` & `GridCal-5.1.3/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/graphics_manager.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/graphics_manager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/diagrams_model.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/diagrams_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/diagram_editor_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from GridCalEngine.Devices.Branches.series_reactance import SeriesReactance
 from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
 from GridCalEngine.Devices.Branches.transformer3w import Transformer3W, Winding
 from GridCalEngine.Devices.Injections.generator import Generator
 from GridCalEngine.Devices.Fluid import FluidNode, FluidPath
 from GridCalEngine.Devices.Aggregation.investments_group import InvestmentsGroup
 from GridCalEngine.Devices.Aggregation.investment import Investment
-from GridCalEngine.Devices.Diagrams.bus_branch_diagram import BusBranchDiagram
+from GridCalEngine.Devices.Diagrams.schematic_diagram import SchematicDiagram
 from GridCalEngine.Devices.Diagrams.graphic_location import GraphicLocation
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec, Logger
 from GridCalEngine.Devices.types import BRANCH_TYPES
 
@@ -70,38 +70,52 @@
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.winding_graphics import WindingGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.dc_line_graphics import DcLineGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.transformer2w_graphics import TransformerGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.hvdc_graphics import HvdcGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.vsc_graphics import VscGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.upfc_graphics import UpfcGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.series_reactance_graphics import SeriesReactanceGraphicItem
+from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.switch_graphics import SwitchGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
 from GridCal.Gui.Diagrams.DiagramEditorWidget.generic_graphics import ACTIVE
 from GridCal.Gui.GeneralDialogues import InputNumberDialogue
 import GridCal.Gui.Visualization.visualization as viz
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCal.Gui.GuiFunctions import ObjectsModel, add_menu_entry
 from GridCal.Gui.messages import info_msg, error_msg, warning_msg, yes_no_question
 from matplotlib import pyplot as plt
 
+BRANCH_GRAPHICS = Union[
+    LineGraphicItem,
+    WindingGraphicItem,
+    DcLineGraphicItem,
+    TransformerGraphicItem,
+    HvdcGraphicItem,
+    VscGraphicItem,
+    UpfcGraphicItem,
+    SeriesReactanceGraphicItem,
+    SwitchGraphicItem
+]
+
 '''
 Structure:
 
 {DiagramEditorWidget: QSplitter}
  |
   - .editor_graphics_view {QGraphicsView} (Handles the drag and drop)
  |      
   - .diagram_scene {DiagramScene: QGraphicsScene}
  |       
   - .circuit {MultiCircuit} (Calculation engine)
  |       
-  - .diagram {BusBranchDiagram} records the objects and their position to load and save diagrams
-
+  - .diagram {SchematicDiagram} records the DB objects and their position to load and save diagrams
+ |       
+  - .graphics_manager {GraphicsManager} records the DB objects and their diagram widgets
 
 The graphic objects need to call the API objects and functions inside the MultiCircuit instance.
 To do this the graphic objects call "parent.circuit.<function or object>"
 '''
 
 
 class BusBranchLibraryModel(QStandardItemModel):
@@ -329,15 +343,15 @@
 
 
 class CustomGraphicsView(QGraphicsView):
     """
     CustomGraphicsView to handle the panning of the grid
     """
 
-    def __init__(self, scene: QGraphicsScene, parent: "BusBranchDiagramScene"):
+    def __init__(self, scene: QGraphicsScene, parent: "DiagramEditorWidget"):
         """
         Constructor
         :param scene: QGraphicsScene
         """
         super().__init__(scene)
         self._parent = parent
         self.setRenderHint(QPainter.Antialiasing)
@@ -454,32 +468,32 @@
     """
     DiagramEditorWidget
     This is the bus-branch editor
     """
 
     def __init__(self,
                  circuit: MultiCircuit,
-                 diagram: Union[BusBranchDiagram, None],
+                 diagram: Union[SchematicDiagram, None],
                  default_bus_voltage: float = 10.0,
                  time_index: Union[None, int] = None):
         """
         Creates the Diagram Editor (DiagramEditorWidget)
         :param circuit: Circuit that is handling
-        :param diagram: BusBranchDiagram to use (optional)
+        :param diagram: SchematicDiagram to use (optional)
         :param default_bus_voltage: Default bus voltages (kV)
         :param time_index: time index to represent
         """
 
         QSplitter.__init__(self)
 
         # store a reference to the multi circuit instance
         self.circuit: MultiCircuit = circuit
 
         # diagram to store the objects locations
-        self.diagram: BusBranchDiagram = diagram
+        self.diagram: SchematicDiagram = diagram
         self.graphics_manager = GraphicsManager()
 
         # default_bus_voltage (kV)
         self.default_bus_voltage = default_bus_voltage
 
         # nodes distance "explosion" factor
         self.expand_factor = 1.1
@@ -780,19 +794,19 @@
         :param w: width (px)
         :return: BusBarGraphicItem
         """
 
         graphic_object = BusBarGraphicItem(editor=self, node=node, x=x, y=y, h=h, w=w)
         return graphic_object
 
-    def set_data(self, circuit: MultiCircuit, diagram: BusBranchDiagram):
+    def set_data(self, circuit: MultiCircuit, diagram: SchematicDiagram):
         """
         Set the widget data and redraw
         :param circuit: MultiCircuit
-        :param diagram: BusBranchDiagram
+        :param diagram: SchematicDiagram
         """
         self.clear()
         self.circuit = circuit
         self.diagram = diagram
         self.draw()
 
     def draw(self) -> None:
@@ -1120,18 +1134,18 @@
         Delete device from the diagram registry
         :param device: EditableDevice
         """
         self.diagram.delete_device(device=device)
         graphic_object: QGraphicsItem = self.graphics_manager.delete_device(device=device)
 
         if graphic_object is not None:
-            try:
-                self.remove_from_scene(graphic_object)
-            except:
-                warn(f"Could not remove {graphic_object} from the scene")
+            # try:
+            self.remove_from_scene(graphic_object)
+            # except:
+            #     warn(f"Could not remove {graphic_object} from the scene")
 
     def remove_element(self,
                        device: ALL_DEV_TYPES,
                        graphic_object: Union[QGraphicsItem, None] = None) -> None:
         """
         Remove device from the diagram and the database
         :param device: EditableDevice
@@ -3138,20 +3152,20 @@
     def get_selection_api_objects(self) -> List[ALL_DEV_TYPES]:
         """
         Get a list of the API objects from the selection
         :return: List[EditableDevice]
         """
         return [e.api_object for e in self.diagram_scene.selectedItems()]
 
-    def get_selection_diagram(self) -> BusBranchDiagram:
+    def get_selection_diagram(self) -> SchematicDiagram:
         """
-        Get a BusBranchDiagram of the current selection
-        :return: BusBranchDiagram
+        Get a SchematicDiagram of the current selection
+        :return: SchematicDiagram
         """
-        diagram = BusBranchDiagram(name="Selection diagram")
+        diagram = SchematicDiagram(name="Selection diagram")
 
         # first pass (only buses)
         bus_dict = dict()
         for item in self.diagram_scene.selectedItems():
             if isinstance(item, BusGraphicItem):
                 # check that the bus is in the original diagram
                 location = self.diagram.query_point(item.api_object)
@@ -3160,43 +3174,41 @@
                     diagram.set_point(device=item.api_object, location=location)
                     bus_dict[item.api_object.idtag] = item
                 else:
                     raise Exception('Item was selected but was not registered!')
 
         # second pass (Branches, and include their not selected buses)
         for item in self.diagram_scene.selectedItems():
-            if not isinstance(item, BusGraphicItem):
+            if isinstance(item, BRANCH_GRAPHICS):
 
                 # add the element
                 rect = item.boundingRect()
                 diagram.set_point(device=item.api_object,
                                   location=GraphicLocation(x=rect.x(),
                                                            y=rect.y(),
                                                            h=rect.height(),
                                                            w=rect.width(),
                                                            r=item.rotation(),
                                                            api_object=item.api_object))
 
-                if hasattr(item.api_object, 'bus_from'):  # if the element is a branch ...
-
-                    # get the api buses from and to
-                    bus_from = item.api_object.bus_from
-                    bus_to = item.api_object.bus_to
-
-                    for bus in [bus_from, bus_to]:
-
-                        # check that the bus is in the original diagram
-                        location = self.diagram.query_point(bus)
-
-                        if location and (bus.idtag not in bus_dict):
-                            # if the bus was not added in the first
-                            # pass and is in the original diagram, add it now
-                            diagram.set_point(device=bus, location=location)
-                            graphic_object = self.graphics_manager.query(elm=bus)
-                            bus_dict[bus.idtag] = graphic_object
+                # get the api buses from and to
+                bus_from = item.api_object.bus_from
+                bus_to = item.api_object.bus_to
+
+                for bus in [bus_from, bus_to]:
+
+                    # check that the bus is in the original diagram
+                    location = self.diagram.query_point(bus)
+
+                    if location and (bus.idtag not in bus_dict):
+                        # if the bus was not added in the first
+                        # pass and is in the original diagram, add it now
+                        diagram.set_point(device=bus, location=location)
+                        graphic_object = self.graphics_manager.query(elm=bus)
+                        bus_dict[bus.idtag] = graphic_object
 
         # third pass: we must also add all those branches connecting the selected buses
         for lst in self.circuit.get_branch_lists():
             for api_object in lst:
                 if api_object.bus_from.idtag in bus_dict or api_object.bus_to.idtag in bus_dict:
                     diagram.set_point(device=api_object,
                                       location=GraphicLocation(api_object=api_object))
@@ -4052,15 +4064,15 @@
                                 vsc_devices: List[VSC],
                                 upfc_devices: List[UPFC],
                                 fluid_nodes: List[FluidNode],
                                 fluid_paths: List[FluidPath],
                                 explode_factor=1.0,
                                 prog_func: Union[Callable, None] = None,
                                 text_func: Union[Callable, None] = None,
-                                name='Bus branch diagram') -> BusBranchDiagram:
+                                name='Bus branch diagram') -> SchematicDiagram:
     """
     Add a elements to the schematic scene
     :param buses: list of Bus objects
     :param lines: list of Line objects
     :param dc_lines: list of DcLine objects
     :param transformers2w: list of Transformer Objects
     :param transformers3w: list of Transformer3W Objects
@@ -4072,15 +4084,15 @@
     :param fluid_paths:
     :param explode_factor: factor of "explosion": Separation of the nodes factor
     :param prog_func: progress report function
     :param text_func: Text report function
     :param name: name of the diagram
     """
 
-    diagram = BusBranchDiagram(name=name)
+    diagram = SchematicDiagram(name=name)
 
     # first create the buses
     if text_func is not None:
         text_func('Creating schematic buses')
 
     nn = len(buses)
     for i, bus in enumerate(buses):
@@ -4340,13 +4352,13 @@
     return diagram
 
 # if __name__ == "__main__":
 #     from PySide6.QtWidgets import QApplication
 #     app = QApplication(sys.argv)
 #
 #     window = DiagramEditorWidget(circuit=MultiCircuit(),
-#                                    diagram=BusBranchDiagram(),
+#                                    diagram=SchematicDiagram(),
 #                                    default_bus_voltage=10.0)
 #
 #     window.resize(1.61 * 700.0, 600.0)  # golden ratio
 #     window.show()
 #     sys.exit(app.exec())
```

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/generic_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/terminal_item.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/winding_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/switch_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/series_reactance_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/dc_line_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/hvdc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/upfc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer2w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,15 @@
     def accept_click(self):
         """
         Set the values
         :return:
         """
 
         if self.selected_template is not None:
+            self.line.length = self.l_spinner.value()
             self.line.apply_template(self.selected_template, Sbase=self.Sbase)
         else:
             length = self.l_spinner.value()
             I = self.i_spinner.value()
             R = self.r_spinner.value() * length
             X = self.x_spinner.value() * length
             B = self.b_spinner.value() * length
```

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/vsc_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer3w_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Branches/line_graphics_template.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/static_generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/current_injection_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/injections_template_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/battery_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/external_grid_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/controllable_shunt_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/load_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Injections/generator_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/busbar_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/cn_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/DiagramEditorWidget/Substation/bus_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/map_widget.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/map_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/node_widget.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/node_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/map_events.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/map_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py` & `GridCal-5.1.3/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/AboutDialogue/about_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/AboutDialogue/about_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/AboutDialogue/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/AboutDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/AboutDialogue/gui.py` & `GridCal-5.1.3/GridCal/Gui/AboutDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/excel_dialog.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/excel_dialog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/models_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/models_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/profile_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/profile_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/ProfilesInput/excel_sheet_selection.py` & `GridCal-5.1.3/GridCal/Gui/ProfilesInput/excel_sheet_selection.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Analysis/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/Analysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Analysis/AnalysisDialogue.py` & `GridCal-5.1.3/GridCal/Gui/Analysis/AnalysisDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Analysis/gui.py` & `GridCal-5.1.3/GridCal/Gui/Analysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Analysis/object_plot_analysis.py` & `GridCal-5.1.3/GridCal/Gui/Analysis/object_plot_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/CascadingSteps/cascading_steps.py` & `GridCal-5.1.3/GridCal/Gui/CascadingSteps/cascading_steps.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/CascadingSteps/gui.py` & `GridCal-5.1.3/GridCal/Gui/CascadingSteps/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/ConsoleLogController.py` & `GridCal-5.1.3/GridCal/Gui/Main/ConsoleLogController.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/GridCalMain.py` & `GridCal-5.1.3/GridCal/Gui/Main/GridCalMain.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/MainWindow.py` & `GridCal-5.1.3/GridCal/Gui/Main/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'MainWindow.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.3
+## Created by: Qt User Interface Compiler version 6.6.1
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
@@ -471,15 +471,15 @@
         self.verticalLayout_5.setObjectName(u"verticalLayout_5")
         self.verticalLayout_5.setContentsMargins(0, 0, 0, 0)
         self.diagram_selection_splitter = QSplitter(self.frame_6)
         self.diagram_selection_splitter.setObjectName(u"diagram_selection_splitter")
         self.diagram_selection_splitter.setOrientation(Qt.Horizontal)
         self.schematic_frame = QFrame(self.diagram_selection_splitter)
         self.schematic_frame.setObjectName(u"schematic_frame")
-        sizePolicy = QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
+        sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.schematic_frame.sizePolicy().hasHeightForWidth())
         self.schematic_frame.setSizePolicy(sizePolicy)
         self.schematic_frame.setFrameShape(QFrame.NoFrame)
         self.schematic_frame.setFrameShadow(QFrame.Raised)
         self.verticalLayout_3 = QVBoxLayout(self.schematic_frame)
@@ -610,15 +610,15 @@
 
         self.filter_pushButton = QPushButton(self.frame_54)
         self.filter_pushButton.setObjectName(u"filter_pushButton")
         self.filter_pushButton.setIcon(icon60)
 
         self.horizontalLayout_28.addWidget(self.filter_pushButton)
 
-        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_28.addItem(self.horizontalSpacer_2)
 
         self.structure_analysis_pushButton = QPushButton(self.frame_54)
         self.structure_analysis_pushButton.setObjectName(u"structure_analysis_pushButton")
         icon67 = QIcon()
         icon67.addFile(u":/Icons/icons/histogram.svg", QSize(), QIcon.Normal, QIcon.Off)
@@ -659,15 +659,15 @@
         self.db_step_label.setObjectName(u"db_step_label")
         self.db_step_label.setMinimumSize(QSize(200, 0))
         self.db_step_label.setFont(font)
         self.db_step_label.setAlignment(Qt.AlignLeading|Qt.AlignLeft|Qt.AlignVCenter)
 
         self.horizontalLayout_25.addWidget(self.db_step_label)
 
-        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_9 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_25.addItem(self.horizontalSpacer_9)
 
         self.add_object_pushButton = QPushButton(self.frame_9)
         self.add_object_pushButton.setObjectName(u"add_object_pushButton")
         icon69 = QIcon()
         icon69.addFile(u":/Icons/icons/plus.svg", QSize(), QIcon.Normal, QIcon.Off)
@@ -733,15 +733,15 @@
         icon73 = QIcon()
         icon73.addFile(u":/Icons/icons/import_models.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.edit_profiles_from_models_pushButton.setIcon(icon73)
         self.edit_profiles_from_models_pushButton.setFlat(False)
 
         self.horizontalLayout.addWidget(self.edit_profiles_from_models_pushButton)
 
-        self.horizontalSpacer = QSpacerItem(183, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer = QSpacerItem(183, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout.addItem(self.horizontalSpacer)
 
         self.plot_time_series_pushButton = QPushButton(self.frame)
         self.plot_time_series_pushButton.setObjectName(u"plot_time_series_pushButton")
         icon74 = QIcon()
         icon74.addFile(u":/Icons/icons/plot.svg", QSize(), QIcon.Normal, QIcon.Off)
@@ -793,15 +793,15 @@
 
         self.device_type_magnitude_comboBox_2 = QComboBox(self.frame_12)
         self.device_type_magnitude_comboBox_2.setObjectName(u"device_type_magnitude_comboBox_2")
         self.device_type_magnitude_comboBox_2.setMinimumSize(QSize(200, 0))
 
         self.horizontalLayout_4.addWidget(self.device_type_magnitude_comboBox_2)
 
-        self.horizontalSpacer_13 = QSpacerItem(267, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_13 = QSpacerItem(267, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_4.addItem(self.horizontalSpacer_13)
 
         self.profile_add_pushButton = QPushButton(self.frame_12)
         self.profile_add_pushButton.setObjectName(u"profile_add_pushButton")
         self.profile_add_pushButton.setIcon(icon69)
 
@@ -909,15 +909,15 @@
         self.gridLayout_23.setObjectName(u"gridLayout_23")
         self.gridLayout_23.setContentsMargins(0, 8, -1, -1)
         self.arrayModeComboBox = QComboBox(self.frame_29)
         self.arrayModeComboBox.setObjectName(u"arrayModeComboBox")
 
         self.gridLayout_23.addWidget(self.arrayModeComboBox, 0, 3, 1, 1)
 
-        self.horizontalSpacer_23 = QSpacerItem(510, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_23 = QSpacerItem(510, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.gridLayout_23.addItem(self.horizontalSpacer_23, 0, 5, 1, 1)
 
         self.simulationDataStructureTableView = QTableView(self.frame_29)
         self.simulationDataStructureTableView.setObjectName(u"simulationDataStructureTableView")
 
         self.gridLayout_23.addWidget(self.simulationDataStructureTableView, 1, 0, 1, 7)
@@ -1016,15 +1016,15 @@
         brush1 = QBrush(QColor(190, 190, 190, 255))
         brush1.setStyle(Qt.SolidPattern)
         palette.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.label_16.setPalette(palette)
 
         self.horizontalLayout_34.addWidget(self.label_16)
 
-        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_22 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_34.addItem(self.horizontalSpacer_22)
 
         self.deleteDriverButton = QPushButton(self.frame_62)
         self.deleteDriverButton.setObjectName(u"deleteDriverButton")
         self.deleteDriverButton.setIcon(icon70)
 
@@ -1060,15 +1060,15 @@
         palette1.setBrush(QPalette.Active, QPalette.WindowText, brush)
         palette1.setBrush(QPalette.Inactive, QPalette.WindowText, brush)
         palette1.setBrush(QPalette.Disabled, QPalette.WindowText, brush1)
         self.label_37.setPalette(palette1)
 
         self.horizontalLayout_33.addWidget(self.label_37)
 
-        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_21 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_33.addItem(self.horizontalSpacer_21)
 
         self.loadResultFromDiskButton = QPushButton(self.frame_60)
         self.loadResultFromDiskButton.setObjectName(u"loadResultFromDiskButton")
         self.loadResultFromDiskButton.setIcon(icon1)
 
@@ -1127,15 +1127,15 @@
 
         self.search_results_Button = QPushButton(self.frame_8)
         self.search_results_Button.setObjectName(u"search_results_Button")
         self.search_results_Button.setIcon(icon60)
 
         self.horizontalLayout_2.addWidget(self.search_results_Button)
 
-        self.horizontalSpacer_20 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_20 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_2.addItem(self.horizontalSpacer_20)
 
         self.units_label = QLabel(self.frame_8)
         self.units_label.setObjectName(u"units_label")
 
         self.horizontalLayout_2.addWidget(self.units_label)
@@ -1209,15 +1209,15 @@
         self.frame_56 = QFrame(self.tab_14)
         self.frame_56.setObjectName(u"frame_56")
         self.frame_56.setFrameShape(QFrame.NoFrame)
         self.frame_56.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_5 = QHBoxLayout(self.frame_56)
         self.horizontalLayout_5.setObjectName(u"horizontalLayout_5")
         self.horizontalLayout_5.setContentsMargins(0, 0, 0, 0)
-        self.horizontalSpacer_16 = QSpacerItem(866, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_16 = QSpacerItem(866, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_5.addItem(self.horizontalSpacer_16)
 
         self.saveResultsLogsButton = QPushButton(self.frame_56)
         self.saveResultsLogsButton.setObjectName(u"saveResultsLogsButton")
         self.saveResultsLogsButton.setIcon(icon3)
 
@@ -1272,22 +1272,28 @@
 
         self.saveSourceCodeButton = QPushButton(self.frame_55)
         self.saveSourceCodeButton.setObjectName(u"saveSourceCodeButton")
         self.saveSourceCodeButton.setIcon(icon3)
 
         self.horizontalLayout_3.addWidget(self.saveSourceCodeButton)
 
+        self.label_91 = QLabel(self.frame_55)
+        self.label_91.setObjectName(u"label_91")
+
+        self.horizontalLayout_3.addWidget(self.label_91)
+
         self.sourceCodeNameLineEdit = QLineEdit(self.frame_55)
         self.sourceCodeNameLineEdit.setObjectName(u"sourceCodeNameLineEdit")
 
         self.horizontalLayout_3.addWidget(self.sourceCodeNameLineEdit)
 
-        self.horizontalSpacer_14 = QSpacerItem(237, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.label_98 = QLabel(self.frame_55)
+        self.label_98.setObjectName(u"label_98")
 
-        self.horizontalLayout_3.addItem(self.horizontalSpacer_14)
+        self.horizontalLayout_3.addWidget(self.label_98)
 
         self.runSourceCodeButton = QPushButton(self.frame_55)
         self.runSourceCodeButton.setObjectName(u"runSourceCodeButton")
         icon89 = QIcon()
         icon89.addFile(u":/Icons/icons/next.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.runSourceCodeButton.setIcon(icon89)
 
@@ -1432,15 +1438,15 @@
         self.gridLayout_22.addWidget(self.distributed_slack_checkBox, 4, 0, 1, 2)
 
         self.label_2 = QLabel(self.frame_19)
         self.label_2.setObjectName(u"label_2")
 
         self.gridLayout_22.addWidget(self.label_2, 0, 0, 1, 1)
 
-        self.verticalSpacer_10 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_10 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_22.addItem(self.verticalSpacer_10, 15, 0, 1, 1)
 
         self.label_11 = QLabel(self.frame_19)
         self.label_11.setObjectName(u"label_11")
 
         self.gridLayout_22.addWidget(self.label_11, 11, 0, 1, 1)
@@ -1549,15 +1555,15 @@
         self.verticalLayout_4.addWidget(self.apply_impedance_tolerances_checkBox)
 
         self.override_branch_controls_checkBox = QCheckBox(self.frame_36)
         self.override_branch_controls_checkBox.setObjectName(u"override_branch_controls_checkBox")
 
         self.verticalLayout_4.addWidget(self.override_branch_controls_checkBox)
 
-        self.verticalSpacer_14 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_14 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_4.addItem(self.verticalSpacer_14)
 
 
         self.gridLayout_9.addWidget(self.frame_36, 2, 1, 1, 1)
 
         self.line_14 = QFrame(self.frame_13)
@@ -1609,15 +1615,15 @@
 
 
         self.gridLayout_9.addWidget(self.frame_20, 0, 0, 1, 2)
 
 
         self.horizontalLayout_23.addWidget(self.frame_13)
 
-        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_5 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_23.addItem(self.horizontalSpacer_5)
 
         self.settings_tabWidget.addTab(self.tab_3, icon5, "")
         self.tab_5 = QWidget()
         self.tab_5.setObjectName(u"tab_5")
         self.horizontalLayout_10 = QHBoxLayout(self.tab_5)
@@ -1766,22 +1772,22 @@
 
         self.start_vs_from_default_radioButton = QRadioButton(self.frame_21)
         self.start_vs_from_default_radioButton.setObjectName(u"start_vs_from_default_radioButton")
         self.start_vs_from_default_radioButton.setChecked(True)
 
         self.gridLayout_2.addWidget(self.start_vs_from_default_radioButton, 7, 0, 1, 3)
 
-        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_7 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_2.addItem(self.verticalSpacer_7, 16, 0, 1, 3)
 
 
         self.horizontalLayout_10.addWidget(self.frame_21)
 
-        self.horizontalSpacer_24 = QSpacerItem(589, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_24 = QSpacerItem(589, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_10.addItem(self.horizontalSpacer_24)
 
         self.settings_tabWidget.addTab(self.tab_5, icon10, "")
         self.tab_4 = QWidget()
         self.tab_4.setObjectName(u"tab_4")
         self.gridLayout_10 = QGridLayout(self.tab_4)
@@ -1832,15 +1838,15 @@
         self.gridLayout_18.addWidget(self.opf_time_grouping_comboBox, 1, 1, 1, 1)
 
         self.mip_solver_comboBox = QComboBox(self.groupBox)
         self.mip_solver_comboBox.setObjectName(u"mip_solver_comboBox")
 
         self.gridLayout_18.addWidget(self.mip_solver_comboBox, 0, 1, 1, 1)
 
-        self.verticalSpacer_18 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_18 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_18.addItem(self.verticalSpacer_18, 10, 0, 1, 1)
 
         self.label_132 = QLabel(self.groupBox)
         self.label_132.setObjectName(u"label_132")
 
         self.gridLayout_18.addWidget(self.label_132, 4, 0, 1, 2)
@@ -1854,15 +1860,15 @@
         self.save_mip_checkBox.setObjectName(u"save_mip_checkBox")
 
         self.gridLayout_18.addWidget(self.save_mip_checkBox, 9, 0, 1, 2)
 
 
         self.gridLayout_10.addWidget(self.groupBox, 4, 3, 1, 1)
 
-        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_10 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.gridLayout_10.addItem(self.horizontalSpacer_10, 4, 5, 1, 1)
 
         self.groupBox_3 = QGroupBox(self.tab_4)
         self.groupBox_3.setObjectName(u"groupBox_3")
         self.groupBox_3.setFont(font3)
         self.gridLayout_27 = QGridLayout(self.groupBox_3)
@@ -1878,15 +1884,15 @@
         self.gridLayout_27.addWidget(self.ips_method_comboBox, 0, 1, 1, 1)
 
         self.label_125 = QLabel(self.groupBox_3)
         self.label_125.setObjectName(u"label_125")
 
         self.gridLayout_27.addWidget(self.label_125, 0, 0, 1, 1)
 
-        self.verticalSpacer_21 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_21 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_27.addItem(self.verticalSpacer_21, 7, 0, 1, 1)
 
         self.label_126 = QLabel(self.groupBox_3)
         self.label_126.setObjectName(u"label_126")
 
         self.gridLayout_27.addWidget(self.label_126, 1, 0, 1, 1)
@@ -1977,15 +1983,15 @@
         self.gridLayout_26.addWidget(self.label_128, 1, 0, 1, 1)
 
         self.label_42 = QLabel(self.groupBox_2)
         self.label_42.setObjectName(u"label_42")
 
         self.gridLayout_26.addWidget(self.label_42, 0, 0, 1, 1)
 
-        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_5 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_26.addItem(self.verticalSpacer_5, 7, 0, 1, 1)
 
         self.lpf_solver_comboBox = QComboBox(self.groupBox_2)
         self.lpf_solver_comboBox.setObjectName(u"lpf_solver_comboBox")
 
         self.gridLayout_26.addWidget(self.lpf_solver_comboBox, 0, 1, 1, 1)
@@ -2035,15 +2041,15 @@
         self.gridLayout_13.setObjectName(u"gridLayout_13")
         self.groupBox_6 = QGroupBox(self.tab_12)
         self.groupBox_6.setObjectName(u"groupBox_6")
         self.groupBox_6.setFlat(False)
         self.groupBox_6.setCheckable(False)
         self.gridLayout_29 = QGridLayout(self.groupBox_6)
         self.gridLayout_29.setObjectName(u"gridLayout_29")
-        self.verticalSpacer_24 = QSpacerItem(20, 393, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_24 = QSpacerItem(20, 393, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_29.addItem(self.verticalSpacer_24, 3, 0, 1, 1)
 
         self.n1ConsiderationCheckBox = QCheckBox(self.groupBox_6)
         self.n1ConsiderationCheckBox.setObjectName(u"n1ConsiderationCheckBox")
         self.n1ConsiderationCheckBox.setChecked(True)
 
@@ -2061,15 +2067,15 @@
         self.atcThresholdSpinBox.setValue(0.050000000000000)
 
         self.gridLayout_29.addWidget(self.atcThresholdSpinBox, 1, 0, 1, 2)
 
 
         self.gridLayout_13.addWidget(self.groupBox_6, 3, 3, 2, 1)
 
-        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_6 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.gridLayout_13.addItem(self.horizontalSpacer_6, 3, 4, 2, 1)
 
         self.label_97 = QLabel(self.tab_12)
         self.label_97.setObjectName(u"label_97")
         self.label_97.setMinimumSize(QSize(24, 24))
         self.label_97.setMaximumSize(QSize(24, 24))
@@ -2102,15 +2108,15 @@
 
         self.gridLayout_13.addWidget(self.line_27, 1, 0, 1, 4)
 
         self.groupBox_4 = QGroupBox(self.tab_12)
         self.groupBox_4.setObjectName(u"groupBox_4")
         self.gridLayout_20 = QGridLayout(self.groupBox_4)
         self.gridLayout_20.setObjectName(u"gridLayout_20")
-        self.verticalSpacer_22 = QSpacerItem(20, 325, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_22 = QSpacerItem(20, 325, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_20.addItem(self.verticalSpacer_22, 5, 0, 1, 1)
 
         self.label_30 = QLabel(self.groupBox_4)
         self.label_30.setObjectName(u"label_30")
 
         self.gridLayout_20.addWidget(self.label_30, 3, 0, 1, 1)
@@ -2170,15 +2176,15 @@
 
         self.skipNtcGenerationLimitsCheckBox = QCheckBox(self.groupBox_5)
         self.skipNtcGenerationLimitsCheckBox.setObjectName(u"skipNtcGenerationLimitsCheckBox")
         self.skipNtcGenerationLimitsCheckBox.setChecked(True)
 
         self.gridLayout_15.addWidget(self.skipNtcGenerationLimitsCheckBox, 0, 0, 1, 2)
 
-        self.verticalSpacer_23 = QSpacerItem(20, 168, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_23 = QSpacerItem(20, 168, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_15.addItem(self.verticalSpacer_23, 12, 1, 1, 1)
 
         self.ntcAlphaSpinBox = QSpinBox(self.groupBox_5)
         self.ntcAlphaSpinBox.setObjectName(u"ntcAlphaSpinBox")
         self.ntcAlphaSpinBox.setMaximum(100)
         self.ntcAlphaSpinBox.setValue(5)
@@ -2309,15 +2315,15 @@
         self.splitter_2.addWidget(self.frame_35)
 
         self.gridLayout_4.addWidget(self.splitter_2, 2, 0, 1, 2)
 
 
         self.horizontalLayout_12.addWidget(self.frame_40)
 
-        self.horizontalSpacer_11 = QSpacerItem(553, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_11 = QSpacerItem(553, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_12.addItem(self.horizontalSpacer_11)
 
         icon91 = QIcon()
         icon91.addFile(u":/Icons/icons/area_transfer.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.settings_tabWidget.addTab(self.tab, icon91, "")
         self.tab_9 = QWidget()
@@ -2371,15 +2377,15 @@
         self.line_22.setPalette(palette12)
         self.line_22.setFrameShadow(QFrame.Plain)
         self.line_22.setLineWidth(4)
         self.line_22.setFrameShape(QFrame.HLine)
 
         self.gridLayout_14.addWidget(self.line_22, 1, 0, 1, 2)
 
-        self.verticalSpacer_12 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_12 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_14.addItem(self.verticalSpacer_12, 8, 0, 1, 1)
 
         self.frame_42 = QFrame(self.frame_32)
         self.frame_42.setObjectName(u"frame_42")
         self.frame_42.setFrameShape(QFrame.NoFrame)
         self.frame_42.setFrameShadow(QFrame.Raised)
@@ -2427,15 +2433,15 @@
         self.label_124.setObjectName(u"label_124")
 
         self.gridLayout_14.addWidget(self.label_124, 5, 0, 1, 1)
 
 
         self.horizontalLayout_8.addWidget(self.frame_32)
 
-        self.horizontalSpacer_8 = QSpacerItem(781, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_8 = QSpacerItem(781, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_8.addItem(self.horizontalSpacer_8)
 
         self.settings_tabWidget.addTab(self.tab_9, icon24, "")
         self.tab_11 = QWidget()
         self.tab_11.setObjectName(u"tab_11")
         self.horizontalLayout_42 = QHBoxLayout(self.tab_11)
@@ -2476,15 +2482,15 @@
         self.gridLayout_28.addWidget(self.label_53, 11, 0, 1, 1)
 
         self.label_119 = QLabel(self.frame_76)
         self.label_119.setObjectName(u"label_119")
 
         self.gridLayout_28.addWidget(self.label_119, 3, 0, 1, 2)
 
-        self.verticalSpacer_19 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_19 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_28.addItem(self.verticalSpacer_19, 16, 0, 1, 2)
 
         self.srap_top_n_SpinBox = QSpinBox(self.frame_76)
         self.srap_top_n_SpinBox.setObjectName(u"srap_top_n_SpinBox")
         self.srap_top_n_SpinBox.setMinimum(1)
         self.srap_top_n_SpinBox.setMaximum(9999999)
@@ -2575,24 +2581,24 @@
         self.contingency_deadband_SpinBox.setValue(0.050000000000000)
 
         self.gridLayout_28.addWidget(self.contingency_deadband_SpinBox, 7, 1, 1, 1)
 
 
         self.horizontalLayout_42.addWidget(self.frame_76)
 
-        self.horizontalSpacer_28 = QSpacerItem(828, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_28 = QSpacerItem(828, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_42.addItem(self.horizontalSpacer_28)
 
         self.settings_tabWidget.addTab(self.tab_11, icon41, "")
         self.tab_6 = QWidget()
         self.tab_6.setObjectName(u"tab_6")
         self.gridLayout_12 = QGridLayout(self.tab_6)
         self.gridLayout_12.setObjectName(u"gridLayout_12")
-        self.horizontalSpacer_12 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_12 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.gridLayout_12.addItem(self.horizontalSpacer_12, 2, 2, 1, 1)
 
         self.frame_15 = QFrame(self.tab_6)
         self.frame_15.setObjectName(u"frame_15")
         self.frame_15.setMinimumSize(QSize(300, 0))
         self.frame_15.setFrameShape(QFrame.NoFrame)
@@ -2604,15 +2610,15 @@
         self.max_iterations_stochastic_spinBox.setObjectName(u"max_iterations_stochastic_spinBox")
         self.max_iterations_stochastic_spinBox.setMinimum(10)
         self.max_iterations_stochastic_spinBox.setMaximum(99999999)
         self.max_iterations_stochastic_spinBox.setValue(1000)
 
         self.gridLayout_6.addWidget(self.max_iterations_stochastic_spinBox, 6, 1, 1, 1)
 
-        self.verticalSpacer_8 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_8 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_6.addItem(self.verticalSpacer_8, 7, 0, 1, 1)
 
         self.stochastic_pf_method_comboBox = QComboBox(self.frame_15)
         self.stochastic_pf_method_comboBox.setObjectName(u"stochastic_pf_method_comboBox")
 
         self.gridLayout_6.addWidget(self.stochastic_pf_method_comboBox, 3, 1, 1, 1)
@@ -2747,15 +2753,15 @@
         self.cascading_islands_spinBox.setObjectName(u"cascading_islands_spinBox")
         self.cascading_islands_spinBox.setMinimum(1)
         self.cascading_islands_spinBox.setMaximum(999999)
         self.cascading_islands_spinBox.setValue(2)
 
         self.verticalLayout_11.addWidget(self.cascading_islands_spinBox)
 
-        self.verticalSpacer_6 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_6 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_11.addItem(self.verticalSpacer_6)
 
 
         self.gridLayout_12.addWidget(self.frame_22, 2, 1, 1, 1)
 
         icon92 = QIcon()
@@ -2855,15 +2861,15 @@
         self.label_120.setMinimumSize(QSize(24, 24))
         self.label_120.setMaximumSize(QSize(24, 24))
         self.label_120.setPixmap(QPixmap(u":/Icons/icons/expansion_planning.svg"))
         self.label_120.setScaledContents(True)
 
         self.gridLayout_21.addWidget(self.label_120, 18, 0, 1, 1)
 
-        self.verticalSpacer_16 = QSpacerItem(20, 250, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_16 = QSpacerItem(20, 250, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_21.addItem(self.verticalSpacer_16, 24, 1, 1, 1)
 
         self.label_7 = QLabel(self.frame_18)
         self.label_7.setObjectName(u"label_7")
 
         self.gridLayout_21.addWidget(self.label_7, 12, 0, 1, 2)
@@ -2949,15 +2955,15 @@
         self.max_investments_evluation_number_spinBox.setValue(4)
 
         self.gridLayout_21.addWidget(self.max_investments_evluation_number_spinBox, 23, 0, 1, 2)
 
 
         self.horizontalLayout_6.addWidget(self.frame_18)
 
-        self.horizontalSpacer_3 = QSpacerItem(935, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_3 = QSpacerItem(935, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_6.addItem(self.horizontalSpacer_3)
 
         icon93 = QIcon()
         icon93.addFile(u":/Icons/icons/ml.svg", QSize(), QIcon.Normal, QIcon.Off)
         self.settings_tabWidget.addTab(self.tab_2, icon93, "")
         self.tab_13 = QWidget()
@@ -3066,15 +3072,15 @@
         self.frame_52.setFrameShadow(QFrame.Raised)
         self.horizontalLayout_24 = QHBoxLayout(self.frame_52)
         self.horizontalLayout_24.setObjectName(u"horizontalLayout_24")
         self.horizontalLayout_24.setContentsMargins(0, 0, 0, 0)
 
         self.verticalLayout_36.addWidget(self.frame_52)
 
-        self.verticalSpacer_13 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_13 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_36.addItem(self.verticalSpacer_13)
 
 
         self.gridLayout_17.addWidget(self.frame_39, 0, 1, 1, 1)
 
         self.frame_31 = QFrame(self.tab_13)
@@ -3151,22 +3157,22 @@
         self.rating_override_checkBox.setObjectName(u"rating_override_checkBox")
 
         self.verticalLayout_15.addWidget(self.rating_override_checkBox)
 
 
         self.verticalLayout_25.addWidget(self.frame_23)
 
-        self.verticalSpacer_15 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_15 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_25.addItem(self.verticalSpacer_15)
 
 
         self.gridLayout_17.addWidget(self.frame_31, 0, 2, 1, 1)
 
-        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_18 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.gridLayout_17.addItem(self.horizontalSpacer_18, 0, 3, 1, 1)
 
         self.frame_27 = QFrame(self.tab_13)
         self.frame_27.setObjectName(u"frame_27")
         self.frame_27.setFrameShape(QFrame.NoFrame)
         self.frame_27.setFrameShadow(QFrame.Raised)
@@ -3235,15 +3241,15 @@
 
         self.rxThresholdSpinBox = QSpinBox(self.frame_27)
         self.rxThresholdSpinBox.setObjectName(u"rxThresholdSpinBox")
         self.rxThresholdSpinBox.setValue(5)
 
         self.verticalLayout_21.addWidget(self.rxThresholdSpinBox)
 
-        self.verticalSpacer_11 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_11 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_21.addItem(self.verticalSpacer_11)
 
 
         self.gridLayout_17.addWidget(self.frame_27, 0, 0, 1, 1)
 
         self.settings_tabWidget.addTab(self.tab_13, icon13, "")
@@ -3438,15 +3444,15 @@
         self.gridLayout.addWidget(self.label, 6, 0, 1, 1)
 
         self.palette_comboBox = QComboBox(self.frame_58)
         self.palette_comboBox.setObjectName(u"palette_comboBox")
 
         self.gridLayout.addWidget(self.palette_comboBox, 3, 0, 1, 2)
 
-        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout.addItem(self.verticalSpacer_4, 14, 0, 1, 1)
 
         self.label_113 = QLabel(self.frame_58)
         self.label_113.setObjectName(u"label_113")
 
         self.gridLayout.addWidget(self.label_113, 4, 0, 1, 1)
@@ -3510,15 +3516,15 @@
         self.verticalLayout_38.addWidget(self.label_118)
 
         self.tile_provider_comboBox = QComboBox(self.frame_73)
         self.tile_provider_comboBox.setObjectName(u"tile_provider_comboBox")
 
         self.verticalLayout_38.addWidget(self.tile_provider_comboBox)
 
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_38.addItem(self.verticalSpacer_2)
 
 
         self.horizontalLayout_39.addWidget(self.frame_73)
 
 
@@ -3607,22 +3613,22 @@
         self.plt_style_comboBox.setObjectName(u"plt_style_comboBox")
 
         self.verticalLayout_16.addWidget(self.plt_style_comboBox)
 
 
         self.verticalLayout_7.addWidget(self.frame_24)
 
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_7.addItem(self.verticalSpacer)
 
 
         self.horizontalLayout_18.addWidget(self.frame_3)
 
-        self.horizontalSpacer_15 = QSpacerItem(40, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_15 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_18.addItem(self.horizontalSpacer_15)
 
         self.settings_tabWidget.addTab(self.tab_10, icon66, "")
         self.tab_8 = QWidget()
         self.tab_8.setObjectName(u"tab_8")
         self.horizontalLayout_40 = QHBoxLayout(self.tab_8)
@@ -3676,29 +3682,29 @@
         self.verticalLayout_37.addWidget(self.user_name_label)
 
         self.saveResultsCheckBox = QCheckBox(self.frame_77)
         self.saveResultsCheckBox.setObjectName(u"saveResultsCheckBox")
 
         self.verticalLayout_37.addWidget(self.saveResultsCheckBox)
 
-        self.verticalSpacer_20 = QSpacerItem(20, 436, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_20 = QSpacerItem(20, 436, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_37.addItem(self.verticalSpacer_20)
 
 
         self.horizontalLayout_40.addWidget(self.frame_77)
 
         self.frame_79 = QFrame(self.tab_8)
         self.frame_79.setObjectName(u"frame_79")
         self.frame_79.setMinimumSize(QSize(300, 0))
         self.frame_79.setFrameShape(QFrame.NoFrame)
         self.frame_79.setFrameShadow(QFrame.Raised)
         self.gridLayout_5 = QGridLayout(self.frame_79)
         self.gridLayout_5.setObjectName(u"gridLayout_5")
-        self.verticalSpacer_25 = QSpacerItem(20, 436, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_25 = QSpacerItem(20, 436, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.gridLayout_5.addItem(self.verticalSpacer_25, 5, 0, 1, 1)
 
         self.cgmes_boundary_set_label = QLabel(self.frame_79)
         self.cgmes_boundary_set_label.setObjectName(u"cgmes_boundary_set_label")
 
         self.gridLayout_5.addWidget(self.cgmes_boundary_set_label, 3, 0, 1, 1)
@@ -3732,15 +3738,15 @@
         self.label_134.setFont(font2)
 
         self.gridLayout_5.addWidget(self.label_134, 0, 0, 1, 2)
 
 
         self.horizontalLayout_40.addWidget(self.frame_79)
 
-        self.horizontalSpacer_27 = QSpacerItem(659, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        self.horizontalSpacer_27 = QSpacerItem(659, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
 
         self.horizontalLayout_40.addItem(self.horizontalSpacer_27)
 
         self.settings_tabWidget.addTab(self.tab_8, icon4, "")
 
         self.gridLayout_8.addWidget(self.settings_tabWidget, 0, 2, 1, 1)
 
@@ -3857,15 +3863,15 @@
         self.engineComboBox.setObjectName(u"engineComboBox")
 
         self.verticalLayout_17.addWidget(self.engineComboBox)
 
 
         self.verticalLayout_12.addWidget(self.frame_25)
 
-        self.verticalSpacer_3 = QSpacerItem(20, 363, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding)
+        self.verticalSpacer_3 = QSpacerItem(20, 363, QSizePolicy.Minimum, QSizePolicy.Expanding)
 
         self.verticalLayout_12.addItem(self.verticalSpacer_3)
 
         self.dark_mode_checkBox = QCheckBox(self.frame_7)
         self.dark_mode_checkBox.setObjectName(u"dark_mode_checkBox")
 
         self.verticalLayout_12.addWidget(self.dark_mode_checkBox)
@@ -4037,18 +4043,18 @@
         self.menuBus_Branch_options.addAction(self.actionSmaller_nodes)
         self.menuBus_Branch_options.addAction(self.actionAutoatic_layout)
         self.menuBus_Branch_options.addAction(self.actionTry_to_fix_buses_location)
         self.menuBus_Branch_options.addAction(self.actionDisable_all_results_tags)
         self.menuBus_Branch_options.addAction(self.actionEnable_all_results_tags)
         self.menuBus_Branch_options.addAction(self.actionSet_schematic_positions_from_GPS_coordinates)
         self.menuBus_Branch_options.addSeparator()
+        self.menuBus_Branch_options.addAction(self.actionNew_bus_branch_diagram_from_selection)
         self.menuBus_Branch_options.addAction(self.actionSelect_buses_by_area)
         self.menuBus_Branch_options.addAction(self.actionSelect_buses_by_zone)
         self.menuBus_Branch_options.addAction(self.actionSelect_buses_by_country)
-        self.menuBus_Branch_options.addAction(self.actionNew_bus_branch_diagram_from_selection)
         self.menuBus_Branch_options.addSeparator()
         self.menuBus_Branch_options.addAction(self.actionDelete_selected)
         self.toolBar.addAction(self.actionNew_project)
         self.toolBar.addAction(self.actionOpen_file)
         self.toolBar.addAction(self.actionSave)
         self.toolBar.addSeparator()
         self.toolBar.addAction(self.actionPower_flow)
@@ -4367,16 +4373,16 @@
 #if QT_CONFIG(tooltip)
         self.actionInvestments_evaluation.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Investments</span></p><p>Perform the investments evaluation</p></body></html>", None))
 #endif // QT_CONFIG(tooltip)
 #if QT_CONFIG(shortcut)
         self.actionInvestments_evaluation.setShortcut(QCoreApplication.translate("mainWindow", u"Ctrl+I, Ctrl+E", None))
 #endif // QT_CONFIG(shortcut)
         self.actionNew_bus_branch_diagram_from_selection.setText(QCoreApplication.translate("mainWindow", u"New diagram from selection", None))
-        self.actionAdd_general_bus_branch_diagram.setText(QCoreApplication.translate("mainWindow", u"New bus-branch diagram", None))
-        self.actionAdd_map.setText(QCoreApplication.translate("mainWindow", u"New map view", None))
+        self.actionAdd_general_bus_branch_diagram.setText(QCoreApplication.translate("mainWindow", u"New schematic", None))
+        self.actionAdd_map.setText(QCoreApplication.translate("mainWindow", u"New map", None))
         self.actionRemove_selected_diagram.setText(QCoreApplication.translate("mainWindow", u"Remove selected diagram", None))
         self.actionReport_a_bug.setText(QCoreApplication.translate("mainWindow", u"Report a bug or feature", None))
         self.actionSearchDiagram.setText(QCoreApplication.translate("mainWindow", u"Search", None))
         self.actionProcess_topology.setText(QCoreApplication.translate("mainWindow", u"Process topology", None))
         self.actionEdit_simulation_time_limits.setText(QCoreApplication.translate("mainWindow", u"Edit simulation time limits", None))
 #if QT_CONFIG(tooltip)
         self.actionEdit_simulation_time_limits.setToolTip(QCoreApplication.translate("mainWindow", u"<html><head/><body><p><span style=\" font-weight:700;\">Time series</span></p><p>Edit simulation time limits</p></body></html>", None))
@@ -4599,17 +4605,19 @@
         self.clearSourceCodeButton.setToolTip(QCoreApplication.translate("mainWindow", u"New script, will delete the existing code.", None))
 #endif // QT_CONFIG(tooltip)
         self.clearSourceCodeButton.setText("")
 #if QT_CONFIG(tooltip)
         self.saveSourceCodeButton.setToolTip(QCoreApplication.translate("mainWindow", u"Save the current source code", None))
 #endif // QT_CONFIG(tooltip)
         self.saveSourceCodeButton.setText("")
+        self.label_91.setText("")
 #if QT_CONFIG(tooltip)
         self.sourceCodeNameLineEdit.setToolTip(QCoreApplication.translate("mainWindow", u"Name of the source code file", None))
 #endif // QT_CONFIG(tooltip)
+        self.label_98.setText("")
 #if QT_CONFIG(tooltip)
         self.runSourceCodeButton.setToolTip(QCoreApplication.translate("mainWindow", u"Run the source code in the console", None))
 #endif // QT_CONFIG(tooltip)
         self.runSourceCodeButton.setText("")
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.pythonConsoleTab), QCoreApplication.translate("mainWindow", u"Python console", None))
         self.tabWidget_2.setTabText(self.tabWidget_2.indexOf(self.sourceCodeTab), QCoreApplication.translate("mainWindow", u"Source code", None))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.main_console_tab), QCoreApplication.translate("mainWindow", u"Scripting", None))
@@ -5050,11 +5058,11 @@
         self.menuExport.setTitle(QCoreApplication.translate("mainWindow", u"Export", None))
         self.menuImport.setTitle(QCoreApplication.translate("mainWindow", u"Import", None))
         self.menuAbout.setTitle(QCoreApplication.translate("mainWindow", u"Help", None))
         self.menuActions.setTitle(QCoreApplication.translate("mainWindow", u"Actions", None))
         self.menuSimulations.setTitle(QCoreApplication.translate("mainWindow", u"Simulations", None))
         self.menuModel.setTitle(QCoreApplication.translate("mainWindow", u"Model", None))
         self.menuDiagrams.setTitle(QCoreApplication.translate("mainWindow", u"Diagram", None))
-        self.menuBus_Branch_options.setTitle(QCoreApplication.translate("mainWindow", u"Bus-Branch options", None))
+        self.menuBus_Branch_options.setTitle(QCoreApplication.translate("mainWindow", u"Current schematic", None))
         self.toolBar.setWindowTitle(QCoreApplication.translate("mainWindow", u"toolBar", None))
     # retranslateUi
```

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/update_gui_file.py` & `GridCal-5.1.3/GridCal/Gui/Main/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/ConsoleLog.py` & `GridCal-5.1.3/GridCal/Gui/Main/ConsoleLog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
 ## Form generated from reading UI file 'ConsoleLog.ui'
 ##
-## Created by: Qt User Interface Compiler version 6.6.3
+## Created by: Qt User Interface Compiler version 6.6.1
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
 from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
     QMetaObject, QObject, QPoint, QRect,
     QSize, QTime, QUrl, Qt)
```

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/object_select_window.py` & `GridCal-5.1.3/GridCal/Gui/Main/object_select_window.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/simulations.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/simulations.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/io.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/io.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/base_gui.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/base_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Scripting/scripting.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Scripting/scripting.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Settings/configuration.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Settings/configuration.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/objects.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/objects.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/time_events.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/time_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/diagrams.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/diagrams.py`

 * *Files 0% similar despite different names*

```diff
@@ -935,15 +935,15 @@
         :return:
         """
         self.diagram_widgets_list.clear()
         self.remove_all_diagram_widgets()
 
         for diagram in self.circuit.diagrams:
 
-            if isinstance(diagram, dev.BusBranchDiagram):
+            if isinstance(diagram, dev.SchematicDiagram):
                 diagram_widget = DiagramEditorWidget(self.circuit,
                                                      diagram=diagram,
                                                      default_bus_voltage=self.ui.defaultBusVoltageSpinBox.value(),
                                                      time_index=self.get_diagram_slider_index())
                 diagram_widget.setStretchFactor(1, 10)
                 diagram_widget.center_nodes()
                 self.diagram_widgets_list.append(diagram_widget)
@@ -998,19 +998,19 @@
 
         self.add_diagram_widget_and_diagram(diagram_widget=map_widget, diagram=diagram)
         self.set_diagrams_list_view()
         self.set_diagram_widget(widget=map_widget)
 
     def add_diagram_widget_and_diagram(self,
                                        diagram_widget: ALL_EDITORS,
-                                       diagram: Union[dev.BusBranchDiagram, dev.MapDiagram]):
+                                       diagram: Union[dev.SchematicDiagram, dev.MapDiagram]):
         """
         Add diagram widget, it also adds the diagram to the circuit for later
         :param diagram_widget: Diagram widget object
-        :param diagram: BusBranchDiagram or MapDiagram
+        :param diagram: SchematicDiagram or MapDiagram
         """
 
         # add the widget pointer
         self.diagram_widgets_list.append(diagram_widget)
 
         # add the diagram to the circuit
         self.circuit.add_diagram(diagram)
```

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Main/SubClasses/Results/results.py` & `GridCal-5.1.3/GridCal/Gui/Main/SubClasses/Results/results.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Visualization/visualization.py` & `GridCal-5.1.3/GridCal/Gui/Visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/Visualization/palettes.py` & `GridCal-5.1.3/GridCal/Gui/Visualization/palettes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SyncDialogue/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/SyncDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SyncDialogue/sync_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/SyncDialogue/sync_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SyncDialogue/gui.py` & `GridCal-5.1.3/GridCal/Gui/SyncDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py` & `GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SolarPowerWizard/gui.py` & `GridCal-5.1.3/GridCal/Gui/SolarPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/RosetaExplorer/MainWindow.py` & `GridCal-5.1.3/GridCal/Gui/RosetaExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/RosetaExplorer/update_gui_file.py` & `GridCal-5.1.3/GridCal/Gui/RosetaExplorer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/RosetaExplorer/RosetaExplorer.py` & `GridCal-5.1.3/GridCal/Gui/RosetaExplorer/RosetaExplorer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/RosetaExplorer/ConsoleWidget.py` & `GridCal-5.1.3/GridCal/Gui/RosetaExplorer/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/RosetaExplorer/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/RosetaExplorer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/LoadDesigner/load_designer.py` & `GridCal-5.1.3/GridCal/Gui/LoadDesigner/load_designer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/LoadDesigner/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/LoadDesigner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/LoadDesigner/load_designer_ui.py` & `GridCal-5.1.3/GridCal/Gui/LoadDesigner/load_designer_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py` & `GridCal-5.1.3/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/WindPowerWizard/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/WindPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/WindPowerWizard/gui.py` & `GridCal-5.1.3/GridCal/Gui/WindPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SystemScaler/system_scaler.py` & `GridCal-5.1.3/GridCal/Gui/SystemScaler/system_scaler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SystemScaler/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/SystemScaler/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SystemScaler/system_scaler_ui.py` & `GridCal-5.1.3/GridCal/Gui/SystemScaler/system_scaler_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TreeModelViewer/MainWindow.py` & `GridCal-5.1.3/GridCal/Gui/TreeModelViewer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TreeModelViewer/update_gui_file.py` & `GridCal-5.1.3/GridCal/Gui/TreeModelViewer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TreeModelViewer/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/TreeModelViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/TreeModelViewer/TreeModelViewer.py` & `GridCal-5.1.3/GridCal/Gui/TreeModelViewer/TreeModelViewer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/gui.py` & `GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/GridGenerator/grid_generator_dialogue.py` & `GridCal-5.1.3/GridCal/Gui/GridGenerator/grid_generator_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/GridGenerator/icons_rc.py` & `GridCal-5.1.3/GridCal/Gui/GridGenerator/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/GridCal/Gui/GridGenerator/gui.py` & `GridCal-5.1.3/GridCal/Gui/GridGenerator/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/setup.py` & `GridCal-5.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.2/PKG-INFO` & `GridCal-5.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCal
-Version: 5.1.2
+Version: 5.1.3
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```

