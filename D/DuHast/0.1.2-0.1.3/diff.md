# Comparing `tmp/DuHast-0.1.2.tar.gz` & `tmp/DuHast-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DuHast-0.1.2.tar", last modified: Sun Dec  3 07:21:40 2023, max compression
+gzip compressed data, was "DuHast-0.1.3.tar", last modified: Tue Apr  9 10:44:11 2024, max compression
```

## Comparing `DuHast-0.1.2.tar` & `DuHast-0.1.3.tar`

### file list

```diff
@@ -1,569 +1,625 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.553284 DuHast-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-03 07:21:28.000000 DuHast-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-03 07:21:40.553284 DuHast-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-03 07:21:28.000000 DuHast-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-03 07:21:29.000000 DuHast-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-03 07:21:40.553284 DuHast-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-03 07:21:29.000000 DuHast-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.485284 DuHast-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.493284 DuHast-0.1.2/src/DuHast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-03 07:21:40.000000 DuHast-0.1.2/src/DuHast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23468 2023-12-03 07:21:40.000000 DuHast-0.1.2/src/DuHast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-03 07:21:40.000000 DuHast-0.1.2/src/DuHast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-03 07:21:40.000000 DuHast-0.1.2/src/DuHast.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.493284 DuHast-0.1.2/src/duHast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Data/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Data/Objects/Properties/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_design_set_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_element_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_instance_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_phasing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_revit_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_type_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/data_ceiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Objects/data_room.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Data/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Utils/data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Utils/data_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Utils/data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/Utils/data_to_file.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/data_to_shapely.py
--rw-r--r--   0 runner    (1001) docker     (127)    22884 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Data/process_ceilings_to_rooms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.497284 DuHast-0.1.2/src/duHast/Revit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/Annotation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/Annotation/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/arrow_heads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/generic_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/multi_ref_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/spot_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/stair_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Annotation/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/Areas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Areas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Areas/area_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Areas/areas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/BIM360/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BIM360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BIM360/bim_360.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BIM360/util_bim_360.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/BuildingPads/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.501284 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/building_pads.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Categories/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Categories/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/categories_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_property_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/categories_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/change_family_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Categories/family_sub_categories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Ceilings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Ceilings/Export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Ceilings/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Ceilings/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.505284 DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/ceilings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.509284 DuHast-0.1.2/src/duHast/Revit/Common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.509284 DuHast-0.1.2/src/duHast/Revit/Common/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20264 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Geometry/curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    27347 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Geometry/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Geometry/solids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.509284 DuHast-0.1.2/src/duHast/Revit/Common/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/colour_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_graphic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_background.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_graphic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/ParameterDirectiveBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/ParameterMappingDirective.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/Common/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Reporting/groups_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Reporting/worksets_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/Common/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Utility/element_copying.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Utility/element_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/Utility/revit_to_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16101 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/design_set_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/element_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/failure_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11599 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9166 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/parameter_get_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)    15941 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/parameter_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/purge_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/revit_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    15355 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Common/worksets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/DetailItems/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/DetailItems/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/DetailItems/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/detail_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/Doors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Doors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Doors/doors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Doors/doors_create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.513284 DuHast-0.1.2/src/duHast/Revit/Exports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.517284 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
--rw-r--r--   0 runner    (1001) docker     (127)    13561 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    17669 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/export_ifc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Exports/export_navis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.517284 DuHast-0.1.2/src/duHast/Revit/Family/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.517284 DuHast-0.1.2/src/duHast/Revit/Family/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11953 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)    16815 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23829 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_category_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7792 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
--rw-r--r--   0 runner    (1001) docker     (127)    19921 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/family_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Family/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/Utility/loadable_family_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_element_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_load_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_parameter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_reference_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9406 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_rename_files_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16256 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/family_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Family/purge_unused_family_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Floors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Floors/Export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Floors/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Reporting/floors_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Floors/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Utility/floors_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/floors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Floors/purge_unused_floor_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Grids/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/grids_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/grids.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/grids_appearance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/grids_worksets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Grids/purge_unused_grid_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Levels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.521284 DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/levels_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    14838 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/levels_appearance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Levels/purge_unused_level_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/LinePattern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/fill_pattern_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/line_pattern_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/fill_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/line_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/line_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/LinePattern/purge_unused_line_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/Links/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/links_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Reporting/links_report_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/Links/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Utility/link_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/Utility/link_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/cad_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/cad_links_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/image_links.py
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Links/purge_unused_image_link_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.525284 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/cable_trays.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/conduits.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/ducts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/flex_ducts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/pipes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    14331 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/Materials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/materials_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Materials/materials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/ModelHealth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.529284 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/design_set_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/detail_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/families.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/line_styles_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/links_cad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/links_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/rooms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/view.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17519 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/ModelHealth/model_health.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Purge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Purge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Purge/purge_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    25813 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Purge/purge_unused.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Purge/purge_unused_e_transmit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Railings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Railings/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Reporting/railings_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/merge_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railing_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railing_family_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railings_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/balusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Railings/railings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Ramps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Ramps/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Ramps/ramps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Revisions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Revisions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Revisions/new_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)    18321 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Revisions/revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Revisions/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Roofs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.533284 DuHast-0.1.2/src/duHast/Revit/Roofs/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/purge_unused_roof_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Roofs/roofs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/Rooms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/Rooms/Export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Export/to_data_room.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/Rooms/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/Rooms/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/room_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/room_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Rooms/rooms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/SharedParameters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.537284 DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8193 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6674 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Stairs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Stairs/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/stairs_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/cut_marks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/landings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    15680 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/purge_unused_stair_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/stairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Stairs/stringers_carriages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Views/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Views/Geometry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Geometry/view_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Views/Objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.541284 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/category_override_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/filter_override_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Objects/view_graphics_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.545284 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.545284 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/Objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/Objects/json_conversion_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/schedules_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/sheets_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_property_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_property_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_reports_json_props.py
--rw-r--r--   0 runner    (1001) docker     (127)    38516 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    10334 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.545284 DuHast-0.1.2/src/duHast/Revit/Views/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_data_to_override_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10762 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_data_to_revit_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    17648 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_revit_override_to_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/sheet_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/view_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/Utility/view_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/referencing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/views_purge_unused.py
--rw-r--r--   0 runner    (1001) docker     (127)    18334 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8942 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.545284 DuHast-0.1.2/src/duHast/Revit/Walls/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Walls/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Reporting/walls_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Reporting/walls_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Walls/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Utility/walls_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/curtain_wall_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/curtain_walls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/purge_unused_wall_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/stacked_walls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/wall_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Walls/walls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Warnings/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Warnings/Data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Data/warnings_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Data/warnings_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/warnings_overlap_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/warnings_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Warnings/Reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Reporting/warnings_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Reporting/warnings_report_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/Revit/Warnings/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23718 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/Utility/curves_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6294 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/solver_area_separation_lines_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/solver_duplicate_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/solver_room_separation_lines_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/Warnings/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Revit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/UI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.549284 DuHast-0.1.2/src/duHast/UI/Objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/Objects/common_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/file_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/file_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/file_select_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13395 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/ui_file_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/workload_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/UI/workloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.553284 DuHast-0.1.2/src/duHast/Utilities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:40.553284 DuHast-0.1.2/src/duHast/Utilities/Objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/Objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/Objects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/Objects/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/Objects/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29998 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/batch_processor_log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/console_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/date_stamps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/directory_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/files_tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/solibri_ifc_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/system_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/util_batch_p.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/Utilities/worksharing_monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-03 07:21:29.000000 DuHast-0.1.2/src/duHast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.945495 DuHast-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 10:44:03.000000 DuHast-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 10:44:11.945495 DuHast-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-09 10:44:03.000000 DuHast-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-09 10:44:03.000000 DuHast-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-09 10:44:11.945495 DuHast-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-09 10:44:03.000000 DuHast-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.869495 DuHast-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.877495 DuHast-0.1.3/src/DuHast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 10:44:11.000000 DuHast-0.1.3/src/DuHast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25898 2024-04-09 10:44:11.000000 DuHast-0.1.3/src/DuHast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:44:11.000000 DuHast-0.1.3/src/DuHast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 10:44:11.000000 DuHast-0.1.3/src/DuHast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.877495 DuHast-0.1.3/src/duHast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.877495 DuHast-0.1.3/src/duHast/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Data/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Data/Objects/Properties/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_design_set_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_element_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_instance_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_phasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_revit_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_type_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/data_ceiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/data_door.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/data_family_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Objects/data_room.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Data/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Utils/data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Utils/data_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Utils/data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/Utils/data_to_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11244 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/data_to_shapely.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Data/process_ceilings_to_rooms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Excel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Excel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Excel/excel_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.881495 DuHast-0.1.3/src/duHast/Revit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/Annotation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/annotations_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/gen_annotations_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/Annotation/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/arrow_heads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/generic_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_modify_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/multi_ref_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/purge_unused_annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/spot_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/stair_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Annotation/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/Areas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Areas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Areas/area_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Areas/areas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/BIM360/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BIM360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BIM360/bim_360.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BIM360/util_bim_360.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/BuildingPads/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.885495 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/building_pads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/category_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10672 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/category_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Data/category_data_purge_unused.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Objects/object_style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_styles_model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_styles_model_json_props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_property_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/categories_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/categories_styles_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/change_family_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Categories/family_sub_categories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Ceilings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Ceilings/Export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.889495 DuHast-0.1.3/src/duHast/Revit/Ceilings/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.893495 DuHast-0.1.3/src/duHast/Revit/Ceilings/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Reporting/ceilings_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.893495 DuHast-0.1.3/src/duHast/Revit/Ceilings/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/ceilings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.893495 DuHast-0.1.3/src/duHast/Revit/Common/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.893495 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21057 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25141 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Geometry/solids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/Common/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/colour_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_graphic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_graphic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/FailureHandlingConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/FailuresPreProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/ParameterDirectiveBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/ParameterMappingDirective.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/Common/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Reporting/groups_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Reporting/worksets_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Reporting/worksets_report_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/Common/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Utility/element_copying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Utility/element_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/Utility/revit_to_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/design_set_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/element_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/failure_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/parameter_get_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/parameter_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/purge_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/revit_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18101 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Common/worksets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/DetailItems/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/DetailItems/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.897495 DuHast-0.1.3/src/duHast/Revit/DetailItems/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/detail_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.901495 DuHast-0.1.3/src/duHast/Revit/Doors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.901495 DuHast-0.1.3/src/duHast/Revit/Doors/Export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Doors/Export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Doors/Export/to_data_door.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Doors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9758 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Doors/doors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Doors/doors_create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.901495 DuHast-0.1.3/src/duHast/Revit/Exports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.901495 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13561 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17669 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/export_ifc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Exports/export_navis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.901495 DuHast-0.1.3/src/duHast/Revit/Family/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Family/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_base_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_base_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_missing_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21301 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23829 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_category_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_find_host_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_loaded_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16182 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Data/family_report_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Family/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/Utility/loadable_family_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_element_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_load_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_parameter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_reference_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9406 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_rename_files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16256 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/family_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Family/purge_unused_family_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Floors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Floors/Export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Floors/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Reporting/floors_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.905495 DuHast-0.1.3/src/duHast/Revit/Floors/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Utility/floors_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/Utility/floors_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/floors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Floors/purge_unused_floor_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/Grids/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/grid_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/grids_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/grids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/grids_appearance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/grids_worksets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Grids/purge_unused_grid_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/Levels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/levels_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/levels_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9930 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14838 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/levels_appearance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Levels/purge_unused_level_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/LinePattern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/fill_pattern_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/line_pattern_data_purge_unused.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.909494 DuHast-0.1.3/src/duHast/Revit/LinePattern/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Objects/LineStylePurgeModifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/fill_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10640 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/line_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/line_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/purge_unused_fill_patterns_by_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/purge_unused_line_patterns_by_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/LinePattern/purge_unused_line_styles_by_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/Links/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/cad_links_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/links_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Reporting/links_report_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/Links/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Utility/link_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/Utility/link_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9360 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/cad_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/cad_links_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/image_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Links/purge_unused_image_link_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/cable_trays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/conduits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/ducts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/flex_ducts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/pipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.913495 DuHast-0.1.3/src/duHast/Revit/Materials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/materials_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/materials_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Materials/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/ModelHealth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/design_set_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/detail_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/line_styles_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/links_cad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/links_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/ModelHealth/model_health.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/Purge/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/Purge/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/Objects/ModifierBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/purge_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26615 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/purge_unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/purge_unused_by_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Purge/purge_unused_e_transmit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.917495 DuHast-0.1.3/src/duHast/Revit/Railings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Railings/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Reporting/railings_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/merge_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railing_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railing_family_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railings_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railings_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/balusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Railings/railings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Ramps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Ramps/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/purge_unused_ramp_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Ramps/ramps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Revisions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Revisions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Revisions/new_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18321 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Revisions/revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Revisions/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Roofs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Roofs/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.921495 DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/purge_unused_roof_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Roofs/roofs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/Rooms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/Rooms/Export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Export/to_data_room.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/Rooms/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/Rooms/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/room_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/room_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Rooms/rooms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/SharedParameters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/Objects/shared_parameter_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/Objects/shared_parameter_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.925495 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/purge_unused_shared_parameters_by_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Stairs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Stairs/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/stairs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/cut_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/landings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16486 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/purge_unused_stair_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/stairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Stairs/stringers_carriages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Views/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Views/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Geometry/view_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.929494 DuHast-0.1.3/src/duHast/Revit/Views/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/category_override_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/filter_override_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Objects/view_graphics_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/Objects/json_conversion_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/schedules_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/sheets_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_property_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_property_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_reports_json_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38502 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10334 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Views/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_data_to_override_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_data_to_revit_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17648 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_revit_override_to_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/sheet_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/view_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/Utility/view_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/referencing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/views_purge_unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18334 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Walls/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Walls/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Reporting/walls_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Reporting/walls_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.933495 DuHast-0.1.3/src/duHast/Revit/Walls/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Utility/walls_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/Utility/walls_type_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11535 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/curtain_wall_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/curtain_walls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/purge_unused_wall_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/stacked_walls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/wall_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Walls/walls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/warnings_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/warnings_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/warnings_overlap_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/warnings_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/warnings_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/warnings_report_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/Revit/Warnings/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23713 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/Utility/curves_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/solver_area_separation_lines_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/solver_duplicate_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7018 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/solver_room_separation_lines_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/solver_room_tag_to_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/Warnings/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Revit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.937495 DuHast-0.1.3/src/duHast/UI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.941495 DuHast-0.1.3/src/duHast/UI/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/Command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/ProgressBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/ViewModelBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/XamlLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/common_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/file_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/file_select_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/Objects/workload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/file_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.941495 DuHast-0.1.3/src/duHast/UI/files_select/
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/files_select/ViewModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/files_select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/files_select/files_select_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/ui_file_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/UI/workloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.941495 DuHast-0.1.3/src/duHast/Utilities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.945495 DuHast-0.1.3/src/duHast/Utilities/Objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/Objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/Objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/Objects/logger_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/Objects/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/Objects/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30135 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/batch_processor_log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/console_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/date_stamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/directory_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/files_tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/log_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/solibri_ifc_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/sub_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/system_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/util_batch_p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/Utilities/worksharing_monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:11.945495 DuHast-0.1.3/src/duHast/pyRevit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/pyRevit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-09 10:44:03.000000 DuHast-0.1.3/src/duHast/pyRevit/console_output.py
```

### Comparing `DuHast-0.1.2/PKG-INFO` & `DuHast-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DuHast
-Version: 0.1.2
+Version: 0.1.3
 Summary: Revit API sample snippets and Revit Batch Processor flows.
 Home-page: UNKNOWN
 Author: Jan Christel
 Author-email: jan.r.christel@gmail.com
 License: BSD-3-Clause
 Description: # Code samples for the Revit Batch Processor
         This repository contains python code samples for the [Revit Batch Processor](https://github.com/bvn-architecture/RevitBatchProcessor)
```

### Comparing `DuHast-0.1.2/README.md` & `DuHast-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/pyproject.toml` & `DuHast-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires = ["setuptools==43.0.0", "wheel==0.33.6"]
 build-backend = "setuptools.build_meta"
 
 [project.urls]
 Homepage = "https://github.com/jchristel/SampleCodeRevitBatchProcessor"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `DuHast-0.1.2/src/DuHast.egg-info/PKG-INFO` & `DuHast-0.1.3/src/DuHast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DuHast
-Version: 0.1.2
+Version: 0.1.3
 Summary: Revit API sample snippets and Revit Batch Processor flows.
 Home-page: UNKNOWN
 Author: Jan Christel
 Author-email: jan.r.christel@gmail.com
 License: BSD-3-Clause
 Description: # Code samples for the Revit Batch Processor
         This repository contains python code samples for the [Revit Batch Processor](https://github.com/bvn-architecture/RevitBatchProcessor)
```

### Comparing `DuHast-0.1.2/src/DuHast.egg-info/SOURCES.txt` & `DuHast-0.1.3/src/DuHast.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 ./src/DuHast.egg-info/top_level.txt
 ./src/duHast/__init__.py
 ./src/duHast/Data/__init__.py
 ./src/duHast/Data/data_to_shapely.py
 ./src/duHast/Data/process_ceilings_to_rooms.py
 ./src/duHast/Data/Objects/__init__.py
 ./src/duHast/Data/Objects/data_ceiling.py
+./src/duHast/Data/Objects/data_door.py
+./src/duHast/Data/Objects/data_family_base.py
 ./src/duHast/Data/Objects/data_room.py
 ./src/duHast/Data/Objects/Properties/__init__.py
 ./src/duHast/Data/Objects/Properties/data_design_set_option.py
 ./src/duHast/Data/Objects/Properties/data_element_geometry.py
 ./src/duHast/Data/Objects/Properties/data_instance_properties.py
 ./src/duHast/Data/Objects/Properties/data_level.py
 ./src/duHast/Data/Objects/Properties/data_phasing.py
@@ -29,14 +31,16 @@
 ./src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py
 ./src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py
 ./src/duHast/Data/Utils/__init__.py
 ./src/duHast/Data/Utils/data_base.py
 ./src/duHast/Data/Utils/data_export.py
 ./src/duHast/Data/Utils/data_import.py
 ./src/duHast/Data/Utils/data_to_file.py
+./src/duHast/Excel/__init__.py
+./src/duHast/Excel/excel_io.py
 ./src/duHast/Revit/__init__.py
 ./src/duHast/Revit/Annotation/__init__.py
 ./src/duHast/Revit/Annotation/annotation.py
 ./src/duHast/Revit/Annotation/arrow_heads.py
 ./src/duHast/Revit/Annotation/dimensions.py
 ./src/duHast/Revit/Annotation/generic_annotation.py
 ./src/duHast/Revit/Annotation/independent_tags.py
@@ -68,23 +72,29 @@
 ./src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py
 ./src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py
 ./src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py
 ./src/duHast/Revit/BuildingPads/Utility/__init__.py
 ./src/duHast/Revit/Categories/__init__.py
 ./src/duHast/Revit/Categories/categories.py
 ./src/duHast/Revit/Categories/categories_model.py
+./src/duHast/Revit/Categories/categories_styles_model.py
 ./src/duHast/Revit/Categories/change_family_category.py
 ./src/duHast/Revit/Categories/family_sub_categories.py
 ./src/duHast/Revit/Categories/Data/__init__.py
-./src/duHast/Revit/Categories/Data/category_data.py
-./src/duHast/Revit/Categories/Data/category_data_processor.py
 ./src/duHast/Revit/Categories/Data/category_data_purge_unused.py
+./src/duHast/Revit/Categories/Data/Objects/__init__.py
+./src/duHast/Revit/Categories/Data/Objects/category_data.py
+./src/duHast/Revit/Categories/Data/Objects/category_data_processor.py
+./src/duHast/Revit/Categories/Objects/__init__.py
+./src/duHast/Revit/Categories/Objects/object_style.py
 ./src/duHast/Revit/Categories/Reporting/__init__.py
 ./src/duHast/Revit/Categories/Reporting/categories_report_header.py
 ./src/duHast/Revit/Categories/Reporting/categories_report_utils.py
+./src/duHast/Revit/Categories/Reporting/categories_styles_model_io.py
+./src/duHast/Revit/Categories/Reporting/categories_styles_model_json_props.py
 ./src/duHast/Revit/Categories/Utility/__init__.py
 ./src/duHast/Revit/Categories/Utility/category_properties_get_utils.py
 ./src/duHast/Revit/Categories/Utility/category_properties_set_utils.py
 ./src/duHast/Revit/Categories/Utility/category_property_names.py
 ./src/duHast/Revit/Categories/Utility/elements_by_category_utils.py
 ./src/duHast/Revit/Ceilings/__init__.py
 ./src/duHast/Revit/Ceilings/ceilings.py
@@ -116,15 +126,18 @@
 ./src/duHast/Revit/Common/purge_utils.py
 ./src/duHast/Revit/Common/revit_version.py
 ./src/duHast/Revit/Common/transaction.py
 ./src/duHast/Revit/Common/worksets.py
 ./src/duHast/Revit/Common/Geometry/__init__.py
 ./src/duHast/Revit/Common/Geometry/curve.py
 ./src/duHast/Revit/Common/Geometry/geometry.py
+./src/duHast/Revit/Common/Geometry/points.py
 ./src/duHast/Revit/Common/Geometry/solids.py
+./src/duHast/Revit/Common/Objects/FailureHandlingConfiguration.py
+./src/duHast/Revit/Common/Objects/FailuresPreProcessor.py
 ./src/duHast/Revit/Common/Objects/ParameterDirectiveBase.py
 ./src/duHast/Revit/Common/Objects/ParameterMappingDirective.py
 ./src/duHast/Revit/Common/Objects/__init__.py
 ./src/duHast/Revit/Common/Objects/Data/__init__.py
 ./src/duHast/Revit/Common/Objects/Data/colour_base.py
 ./src/duHast/Revit/Common/Objects/Data/line_cut.py
 ./src/duHast/Revit/Common/Objects/Data/line_graphic_base.py
@@ -147,14 +160,16 @@
 ./src/duHast/Revit/DetailItems/Reporting/__init__.py
 ./src/duHast/Revit/DetailItems/Reporting/detail_items_report_header.py
 ./src/duHast/Revit/DetailItems/Utility/__init__.py
 ./src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py
 ./src/duHast/Revit/Doors/__init__.py
 ./src/duHast/Revit/Doors/doors.py
 ./src/duHast/Revit/Doors/doors_create.py
+./src/duHast/Revit/Doors/Export/__init__.py
+./src/duHast/Revit/Doors/Export/to_data_door.py
 ./src/duHast/Revit/Exports/__init__.py
 ./src/duHast/Revit/Exports/export.py
 ./src/duHast/Revit/Exports/export_ifc.py
 ./src/duHast/Revit/Exports/export_navis.py
 ./src/duHast/Revit/Exports/Utility/__init__.py
 ./src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py
 ./src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py
@@ -163,38 +178,41 @@
 ./src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py
 ./src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py
 ./src/duHast/Revit/Exports/Utility/ifc_export_settings.py
 ./src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py
 ./src/duHast/Revit/Family/__init__.py
 ./src/duHast/Revit/Family/family_element_utils.py
 ./src/duHast/Revit/Family/family_functions.py
+./src/duHast/Revit/Family/family_geometry.py
+./src/duHast/Revit/Family/family_instance_create.py
 ./src/duHast/Revit/Family/family_load_option.py
 ./src/duHast/Revit/Family/family_parameter_utils.py
 ./src/duHast/Revit/Family/family_reference_elements.py
 ./src/duHast/Revit/Family/family_reload.py
 ./src/duHast/Revit/Family/family_rename_files_utils.py
 ./src/duHast/Revit/Family/family_utils.py
 ./src/duHast/Revit/Family/purge_unused_family_types.py
 ./src/duHast/Revit/Family/Data/__init__.py
-./src/duHast/Revit/Family/Data/family_base_data.py
 ./src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py
 ./src/duHast/Revit/Family/Data/family_base_data_missing_families.py
-./src/duHast/Revit/Family/Data/family_base_data_processor.py
 ./src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py
 ./src/duHast/Revit/Family/Data/family_base_data_utils.py
 ./src/duHast/Revit/Family/Data/family_category_data_utils.py
-./src/duHast/Revit/Family/Data/family_data_collector.py
 ./src/duHast/Revit/Family/Data/family_reload_advanced_utils.py
 ./src/duHast/Revit/Family/Data/family_rename_files.py
 ./src/duHast/Revit/Family/Data/family_rename_find_host_families.py
 ./src/duHast/Revit/Family/Data/family_rename_loaded_families.py
 ./src/duHast/Revit/Family/Data/family_report_utils.py
-./src/duHast/Revit/Family/Data/ifamily_action.py
-./src/duHast/Revit/Family/Data/ifamily_data.py
-./src/duHast/Revit/Family/Data/ifamily_processor.py
+./src/duHast/Revit/Family/Data/Objects/__init__.py
+./src/duHast/Revit/Family/Data/Objects/family_base_data.py
+./src/duHast/Revit/Family/Data/Objects/family_base_data_processor.py
+./src/duHast/Revit/Family/Data/Objects/family_data_collector.py
+./src/duHast/Revit/Family/Data/Objects/ifamily_action.py
+./src/duHast/Revit/Family/Data/Objects/ifamily_data.py
+./src/duHast/Revit/Family/Data/Objects/ifamily_processor.py
 ./src/duHast/Revit/Family/Utility/__init__.py
 ./src/duHast/Revit/Family/Utility/loadable_family_categories.py
 ./src/duHast/Revit/Floors/__init__.py
 ./src/duHast/Revit/Floors/floors.py
 ./src/duHast/Revit/Floors/purge_unused_floor_types.py
 ./src/duHast/Revit/Floors/Export/__init__.py
 ./src/duHast/Revit/Floors/Reporting/__init__.py
@@ -215,24 +233,28 @@
 ./src/duHast/Revit/Levels/levels_appearance.py
 ./src/duHast/Revit/Levels/purge_unused_level_types.py
 ./src/duHast/Revit/Levels/Reporting/__init__.py
 ./src/duHast/Revit/Levels/Reporting/levels_report_header.py
 ./src/duHast/Revit/Levels/Reporting/levels_report_utils.py
 ./src/duHast/Revit/LinePattern/__init__.py
 ./src/duHast/Revit/LinePattern/fill_patterns.py
-./src/duHast/Revit/LinePattern/line_pattern_data.py
-./src/duHast/Revit/LinePattern/line_pattern_data_processor.py
-./src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py
 ./src/duHast/Revit/LinePattern/line_patterns.py
 ./src/duHast/Revit/LinePattern/line_styles.py
-./src/duHast/Revit/LinePattern/purge_unused_line_patterns.py
+./src/duHast/Revit/LinePattern/purge_unused_fill_patterns_by_delete.py
+./src/duHast/Revit/LinePattern/purge_unused_line_patterns_by_delete.py
+./src/duHast/Revit/LinePattern/purge_unused_line_styles_by_delete.py
+./src/duHast/Revit/LinePattern/Data/__init__.py
+./src/duHast/Revit/LinePattern/Data/line_pattern_data_purge_unused.py
+./src/duHast/Revit/LinePattern/Data/Objects/__init__.py
+./src/duHast/Revit/LinePattern/Data/Objects/fill_pattern_settings.py
+./src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data.py
+./src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data_processor.py
+./src/duHast/Revit/LinePattern/Data/Objects/line_pattern_settings.py
+./src/duHast/Revit/LinePattern/Objects/LineStylePurgeModifier.py
 ./src/duHast/Revit/LinePattern/Objects/__init__.py
-./src/duHast/Revit/LinePattern/Objects/Data/__init__.py
-./src/duHast/Revit/LinePattern/Objects/Data/fill_pattern_settings.py
-./src/duHast/Revit/LinePattern/Objects/Data/line_pattern_settings.py
 ./src/duHast/Revit/Links/__init__.py
 ./src/duHast/Revit/Links/cad_links.py
 ./src/duHast/Revit/Links/cad_links_geometry.py
 ./src/duHast/Revit/Links/image_links.py
 ./src/duHast/Revit/Links/links.py
 ./src/duHast/Revit/Links/purge_unused_image_link_types.py
 ./src/duHast/Revit/Links/Reporting/__init__.py
@@ -280,15 +302,18 @@
 ./src/duHast/Revit/ModelHealth/Reporting/Properties/links_cad.py
 ./src/duHast/Revit/ModelHealth/Reporting/Properties/links_images.py
 ./src/duHast/Revit/ModelHealth/Reporting/Properties/rooms.py
 ./src/duHast/Revit/ModelHealth/Reporting/Properties/view.py
 ./src/duHast/Revit/Purge/__init__.py
 ./src/duHast/Revit/Purge/purge_action.py
 ./src/duHast/Revit/Purge/purge_unused.py
+./src/duHast/Revit/Purge/purge_unused_by_delete.py
 ./src/duHast/Revit/Purge/purge_unused_e_transmit.py
+./src/duHast/Revit/Purge/Objects/ModifierBase.py
+./src/duHast/Revit/Purge/Objects/__init__.py
 ./src/duHast/Revit/Railings/__init__.py
 ./src/duHast/Revit/Railings/balusters.py
 ./src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py
 ./src/duHast/Revit/Railings/railings.py
 ./src/duHast/Revit/Railings/Reporting/__init__.py
 ./src/duHast/Revit/Railings/Reporting/railings_report_header.py
 ./src/duHast/Revit/Railings/Utility/__init__.py
@@ -326,21 +351,27 @@
 ./src/duHast/Revit/Rooms/Export/__init__.py
 ./src/duHast/Revit/Rooms/Export/to_data_room.py
 ./src/duHast/Revit/Rooms/Geometry/__init__.py
 ./src/duHast/Revit/Rooms/Geometry/geometry.py
 ./src/duHast/Revit/Rooms/Reporting/__init__.py
 ./src/duHast/Revit/Rooms/Reporting/revit_rooms_report_header.py
 ./src/duHast/Revit/SharedParameters/__init__.py
+./src/duHast/Revit/SharedParameters/purge_unused_shared_parameters_by_delete.py
 ./src/duHast/Revit/SharedParameters/shared_parameter_add.py
 ./src/duHast/Revit/SharedParameters/shared_parameter_data.py
 ./src/duHast/Revit/SharedParameters/shared_parameter_swap.py
 ./src/duHast/Revit/SharedParameters/shared_parameter_type_change.py
 ./src/duHast/Revit/SharedParameters/shared_parameters.py
 ./src/duHast/Revit/SharedParameters/shared_parameters_delete.py
 ./src/duHast/Revit/SharedParameters/shared_parameters_tuple.py
+./src/duHast/Revit/SharedParameters/Data/__init__.py
+./src/duHast/Revit/SharedParameters/Data/shared_parameter_data_purge_Unused.py
+./src/duHast/Revit/SharedParameters/Data/Objects/__init__.py
+./src/duHast/Revit/SharedParameters/Data/Objects/shared_parameter_data.py
+./src/duHast/Revit/SharedParameters/Data/Objects/shared_parameter_data_processor.py
 ./src/duHast/Revit/SharedParameters/Reporting/__init__.py
 ./src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py
 ./src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py
 ./src/duHast/Revit/Stairs/__init__.py
 ./src/duHast/Revit/Stairs/cut_marks.py
 ./src/duHast/Revit/Stairs/landings.py
 ./src/duHast/Revit/Stairs/path.py
@@ -415,51 +446,64 @@
 ./src/duHast/Revit/Warnings/solver.py
 ./src/duHast/Revit/Warnings/solver_area_separation_lines_overlap.py
 ./src/duHast/Revit/Warnings/solver_duplicate_mark.py
 ./src/duHast/Revit/Warnings/solver_room_separation_lines_overlap.py
 ./src/duHast/Revit/Warnings/solver_room_tag_to_room.py
 ./src/duHast/Revit/Warnings/warnings.py
 ./src/duHast/Revit/Warnings/Data/__init__.py
-./src/duHast/Revit/Warnings/Data/warnings_data.py
-./src/duHast/Revit/Warnings/Data/warnings_data_processor.py
+./src/duHast/Revit/Warnings/Data/Objects/__init__.py
+./src/duHast/Revit/Warnings/Data/Objects/warnings_data.py
+./src/duHast/Revit/Warnings/Data/Objects/warnings_data_processor.py
 ./src/duHast/Revit/Warnings/Objects/__init__.py
 ./src/duHast/Revit/Warnings/Objects/warnings_overlap_storage.py
 ./src/duHast/Revit/Warnings/Objects/warnings_storage.py
 ./src/duHast/Revit/Warnings/Reporting/__init__.py
 ./src/duHast/Revit/Warnings/Reporting/warnings_report.py
 ./src/duHast/Revit/Warnings/Reporting/warnings_report_header.py
 ./src/duHast/Revit/Warnings/Utility/__init__.py
 ./src/duHast/Revit/Warnings/Utility/curves_util.py
 ./src/duHast/UI/__init__.py
-./src/duHast/UI/file_item.py
 ./src/duHast/UI/file_list.py
-./src/duHast/UI/file_select_settings.py
 ./src/duHast/UI/script.py
 ./src/duHast/UI/ui_file_select.py
-./src/duHast/UI/workload_bucket.py
 ./src/duHast/UI/workloader.py
+./src/duHast/UI/Objects/Command.py
+./src/duHast/UI/Objects/ProgressBase.py
+./src/duHast/UI/Objects/ViewModelBase.py
+./src/duHast/UI/Objects/XamlLoader.py
 ./src/duHast/UI/Objects/__init__.py
 ./src/duHast/UI/Objects/common_ui.py
+./src/duHast/UI/Objects/file_item.py
+./src/duHast/UI/Objects/file_select_settings.py
+./src/duHast/UI/Objects/workload_bucket.py
+./src/duHast/UI/files_select/ViewModel.py
+./src/duHast/UI/files_select/__init__.py
+./src/duHast/UI/files_select/files_select_ui.py
 ./src/duHast/Utilities/__init__.py
 ./src/duHast/Utilities/batch_processor_log_utils.py
 ./src/duHast/Utilities/benchmarking.py
 ./src/duHast/Utilities/compare.py
 ./src/duHast/Utilities/console_out.py
 ./src/duHast/Utilities/date_stamps.py
 ./src/duHast/Utilities/directory_io.py
 ./src/duHast/Utilities/files_combine.py
 ./src/duHast/Utilities/files_csv.py
 ./src/duHast/Utilities/files_get.py
 ./src/duHast/Utilities/files_io.py
 ./src/duHast/Utilities/files_json.py
 ./src/duHast/Utilities/files_tab.py
+./src/duHast/Utilities/log_decorator.py
 ./src/duHast/Utilities/padding.py
 ./src/duHast/Utilities/solibri_ifc_optimizer.py
+./src/duHast/Utilities/sub_process.py
 ./src/duHast/Utilities/system_process.py
 ./src/duHast/Utilities/unit_conversion.py
 ./src/duHast/Utilities/util_batch_p.py
 ./src/duHast/Utilities/utility.py
 ./src/duHast/Utilities/worksharing_monitor_process.py
 ./src/duHast/Utilities/Objects/__init__.py
 ./src/duHast/Utilities/Objects/base.py
+./src/duHast/Utilities/Objects/logger_object.py
 ./src/duHast/Utilities/Objects/result.py
-./src/duHast/Utilities/Objects/timer.py
+./src/duHast/Utilities/Objects/timer.py
+./src/duHast/pyRevit/__init__.py
+./src/duHast/pyRevit/console_output.py
```

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/from_revit_conversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Revit Geometry to data geometry conversion helper functions.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -15,24 +16,27 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 from duHast.Data.Objects.Properties.Geometry import geometry_polygon as dGeometryPoly
 from duHast.Revit.Common.Geometry import geometry as rGeo
 from collections import namedtuple
+from duHast.Revit.Common.Geometry.points import get_point_as_doubles, flatten_xyz_point
+
+from Autodesk.Revit.DB import XYZ
 
 
 def convert_xyz_in_data_geometry_polygons(doc, dgObject):
     """
     Converts Revit XYZ objects stored in a data geometry object into groups of doubles for inner and outer loops\
         and stores them in new data geometry object. It also populates translation and rotation matrix data of\
             coordinate system information.
@@ -43,21 +47,21 @@
     :return: A data geometry object.
     :rtype: :class:`.DataGeometryPolygon`
     """
 
     data_geometry = dGeometryPoly.DataPolygon()
     outer_loop = []
     for xyz_point in dgObject.outer_loop:
-        point_as_double = rGeo.get_point_as_doubles(xyz_point)
+        point_as_double = get_point_as_doubles(xyz_point)
         outer_loop.append(point_as_double)
     inner_loops = []
     for inner_loop in dgObject.inner_loops:
         inner_loop_points = []
         for xyz_point in inner_loop:
-            point_as_double = rGeo.get_point_as_doubles(xyz_point)
+            point_as_double = get_point_as_doubles(xyz_point)
             inner_loop_points.append(point_as_double)
         inner_loops.append(inner_loop_points)
     data_geometry.outer_loop = outer_loop
     data_geometry.inner_loops = inner_loops
     # add coordinate system translation and rotation data
     (
         data_geometry.rotation_coord,
@@ -135,7 +139,28 @@
             if len(loopDic[key]) > 0:
                 for hole in loopDic[key]:
                     dataGeometry.inner_loops.append(hole.threeDPoly)
             else:
                 dataGeometry.inner_loops = []
             ceilingGeos.append(dataGeometry)
     return ceilingGeos
+
+
+def convert_bounding_box_to_flattened_2d_points(bounding_box):
+    """
+    Converts a bounding box into a 2D polygon by projecting it onto a plane.( Removes Z values...)
+    :param bounding_box: A bounding box.
+    :type bounding_box: Autodesk.Revit.DB.BoundingBoxXYZ
+    :return: A list of data geometry instances.
+    :rtype: list of :class:`.DataGeometryPolygon`
+    """
+    # get points from bounding box and project them onto a plane ( Z value of bounding box min point)
+    bounding_box_points = [
+        bounding_box.Min,
+        XYZ(bounding_box.Max.X, bounding_box.Min.Y, bounding_box.Min.Z),
+        XYZ(bounding_box.Max.X, bounding_box.Max.Y, bounding_box.Min.Z),
+        XYZ(bounding_box.Min.X, bounding_box.Max.Y, bounding_box.Min.Z),
+    ]
+    # set up data class object and store points in outer loop property
+    dataGeometry = dGeometryPoly.DataPolygon()
+    dataGeometry.outer_loop = bounding_box_points
+    return dataGeometry
```

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/from_revit_elements.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from duHast.Revit.Common.Geometry import solids as rSolid
 
 
 def get_2d_points_from_revit_element_type_in_model(doc, element_instance_getter):
```

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_polygon.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/Geometry/geometry_topo_cell.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_design_set_option.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_design_set_option.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_element_geometry.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_element_geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_instance_properties.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_instance_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_level.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_level.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_phasing.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_phasing.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_revit_model.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_revit_model.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/Properties/data_type_properties.py` & `DuHast-0.1.3/src/duHast/Data/Objects/Properties/data_type_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/data_ceiling.py` & `DuHast-0.1.3/src/duHast/Data/Objects/data_ceiling.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Objects/data_room.py` & `DuHast-0.1.3/src/duHast/Data/Objects/data_room.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Utils/data_base.py` & `DuHast-0.1.3/src/duHast/Data/Utils/data_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Utils/data_export.py` & `DuHast-0.1.3/src/duHast/Data/Utils/data_export.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Data/Utils/data_import.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/warnings_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Data storage reader class.
+This module contains a Revit warnings properties report function. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
-
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -23,167 +22,129 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-
-# import clr
-# clr.AddReference("System.Core")
-# from System import Linq
-# clr.ImportExtensions(Linq)
-
-import json
-
-from duHast.Data.Objects import data_ceiling as dc
-from duHast.Data.Objects import data_room as dr
-
-
-class ReadDataFromFile:
-    def __init__(self, file_path):
-        """
-        Class constructor.
-
-        :param filePath: Fully qualified file path to json formatted data file.
-        :type filePath: str
-        """
-
-        self.data_file_path = file_path
-        self.data_type = ""
-        self.data = []
-
-    def _read_json_file(self, file_path):
-        """
-        Reads a json formatted text file into a dictionary.
-
-        :param file_path: Fully qualified file path to json formatted data file.
-        :type file_path: str
-
-        :return: A dictionary.
-        :rtype: {}
-        """
-
-        data = {}
+from duHast.Revit.Warnings.warnings import get_warnings
+from duHast.Revit.Warnings.Objects.warnings_storage import RevitWarning
+from duHast.Utilities.Objects import result as res
+from duHast.Revit.Warnings.Reporting.warnings_report_header import (
+    REPORT_WARNINGS_HEADER,
+)
+from duHast.Utilities.files_csv import write_report_data_as_csv
+
+
+def get_warnings_report_data(doc, revit_file_name):
+    """
+    Gets warnings data to be written to report file.
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param revit_file_path: The file hostname, which is added to data returned.
+    :type revit_file_path: str
+    :return: list of list of sheet properties.
+    :rtype: list of list of str
+    """
+
+    # get all warnings
+    data = {}
+    warnings = get_warnings(doc)
+    for warning in warnings:
         try:
-            # Opening JSON file
-            f = open(file_path)
-            # returns JSON object as
-            # a dictionary
-            data = json.load(f)
-        except Exception as e:
-            pass
-        return data
-
-    def _get_room_data_from_JSON(self, room_data):
-        """
-        Converts dictionary into data room objects.
-
-        :param room_data: List of dictionaries describing rooms
-        :type room_data:  [{var}]
-
-        :return: List of data room objects.
-        :rtype: [:class:`.DataRoom`]
-        """
-
-        all_rooms = []
-        for d in room_data:
-            p = dr.DataRoom(d)
-            all_rooms.append(p)
-        return all_rooms
-
-    def _get_ceiling_data_from_JSON(self, ceiling_data):
-        """
-        Converts dictionary into data ceiling objects.
-
-        :param ceiling_data: List of dictionaries describing ceilings
-        :type ceiling_data: [{var}]
-
-        :return: List of data ceiling objects.
-        :rtype: [:class:`.DataCeiling`]
-        """
-
-        all_ceilings = []
-
-        for d in ceiling_data:
-            p = dc.DataCeiling(d)
-            all_ceilings.append(p)
-        return all_ceilings
-
-    def load_data(self):
-        """
-        Load json formatted rows into data objects and stores them in this class.
-
-        In the moment the following data objects are supported:
-
-        - :class: `.DataRoom`
-        - :class: `.DataCeiling`
-
-        """
-
-        data_objects = []
-        data_json = self._read_json_file(self.data_file_path)
-
-        if len(data_json) > 0:
-            # load rooms {Root}.rooms
-            room_json = self._get_room_data_from_JSON(data_json[dr.DataRoom.data_type])
-
-            # add to global list
-            for rj in room_json:
-                data_objects.append(rj)
-
-            # load ceiling at {Root}.ceilings
-            ceiling_json = self._get_ceiling_data_from_JSON(
-                data_json[dc.DataCeiling.data_type]
+            failure_id_guid = warning.GetFailureDefinitionId().Guid
+            failure_description = warning.GetDescriptionText()
+            failing_ids = warning.GetFailingElements()
+            failing_ids_as_integer = []
+            for fail_id in failing_ids:
+                failing_ids_as_integer.append(fail_id.IntegerValue)
+
+            warning_stored = RevitWarning(
+                file_name=revit_file_name,
+                id=failure_id_guid,
+                description=failure_description,
+                element_ids=failing_ids_as_integer,
             )
+            if warning_stored.id in data:
+                data[warning_stored.id].append(warning_stored)
+            else:
+                data[warning_stored.id] = [warning_stored]
 
-            # add to global list
-            for cj in ceiling_json:
-                data_objects.append(cj)
-        self.data = data_objects
-
-    def get_data_by_level(self, level_name):
-        """
-        Returns all data objects where level name equals past in value.
-
-        :param level_name: The building level name.
-        :type level_name: str
-
-        :return: A list of room and ceiling data objects
-        :rtype: list [data objects]
-        """
-
-        return list(filter(lambda x: (x.level.name == level_name), self.data))
-
-    def get_data_by_type(self, data_type):
-        """
-        Returns all data objects where type equals past in type name
-
-        :param data_type: The data type name.
-        :type data_type: str
-
-        :return: A list of room and ceiling data objects
-        :rtype: list [data objects]
-        """
-
-        return list(filter(lambda x: (x.data_type == data_type), self.data))
-
-    def get_data_by_level_and_data_type(self, level_name, data_type):
-        """
-        Returns all data objects where level name and data type equal past in values.
-
-        :param level_name: The building level name.
-        :type level_name: str
-        :param data_type: A string describing the data type\
-            refer to property .dataType on data object class
-        :type data_type: str
-
-        :return: A list of data objects
-        :rtype: list [data objects]
-        """
-
-        return list(
-            filter(
-                lambda x: (x.level.name == level_name and x.data_type == data_type),
-                self.data,
+        except Exception as e:
+            # store the exception
+            warning_exception = ResourceWarning(
+                file_name=revit_file_name,
+                id=-1,
+                description="failed to retrieve warning with exception: {}".format(e),
+                element_ids=[],
             )
+            if warning_stored.id in data:
+                data[warning_stored.id].append(warning_exception)
+            else:
+                data[warning_stored.id] = [warning_exception]
+
+    return data
+
+
+def convert_warnings_data_to_list(warnings_data):
+    """
+    Converts a list of dictionaries of view properties names and values to a list of properties only.
+
+    :param view_data: List of dictionaries representing view properties
+    :type view_data: [{}]
+    :return: A list of lists of view property values.
+    :rtype: [[str]]
+    """
+
+    data = []
+    for key, value in warnings_data.items():
+        number_elements_affected = 0
+        dummy = None
+        for warning_data_instance in value:
+            number_elements_affected = number_elements_affected + len(
+                warning_data_instance.element_ids
+            )
+            dummy = warning_data_instance
+        # build a list with entries:
+        # file name, warning GUID, number of warnings belonging to warnings GUID, warnings description, number of elements involved overall
+        data.append(
+            [
+                dummy.file_name,
+                dummy.date,
+                dummy.time,
+                dummy.id,
+                len(warnings_data[key]),
+                dummy.description,
+                number_elements_affected,
+            ]
+        )
+    return data
+
+
+def write_warnings_data(file_name, data):
+    """
+    Writes to file all warnings properties.
+
+    file type: csv
+
+    :param file_name: The fully qualified file path of the report file.
+    :type file_name: str
+    :param current_file_name: The current revit file name which will be appended to data in the report.
+    :type current_file_name: str
+    :return:
+        Result class instance.
+        - .status True if data was written successfully. Otherwise False.
+        - .message will contain write status.
+    :rtype: :class:`.Result`
+    """
+
+    return_value = res.Result()
+    try:
+        data_converted = convert_warnings_data_to_list(warnings_data=data)
+        write_report_data_as_csv(file_name, REPORT_WARNINGS_HEADER, data_converted)
+        return_value.update_sep(
+            True, "Successfully wrote data file at {}".format(file_name)
         )
+    except Exception as e:
+        return_value.update_sep(False, str(e))
+    return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Data/Utils/data_to_file.py` & `DuHast-0.1.3/src/duHast/Data/Utils/data_to_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Utility functions writing data objects to file.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -15,27 +16,29 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 from duHast.Utilities.Objects import result as res
 from duHast.Utilities import date_stamps as dateStamp
 
 import codecs
 import json
 
+CONSTANT_DATA_FIELDS = {"file name": "file name", "date processed": "date processed"}
+
 
 def build_json_for_file(dic, model_name):
     """
     Adds two header keys to json output to be saved to file.
 
     - file name
     - date processed
@@ -46,16 +49,16 @@
     :type model_name: str
 
     :return: A dictionary
     :rtype: {str:[]}
     """
 
     data_json = {
-        "file name": model_name,
-        "date processed": dateStamp.get_date_stamp(
+        CONSTANT_DATA_FIELDS["file name"]: model_name,
+        CONSTANT_DATA_FIELDS["date processed"]: dateStamp.get_date_stamp(
             dateStamp.FILE_DATE_STAMP_YYYY_MM_DD_HH_MM_SEC
         ),
     }
     for key, item in dic.items():
         data_json[key] = item
 
     return data_json
```

### Comparing `DuHast-0.1.2/src/duHast/Data/data_to_shapely.py` & `DuHast-0.1.3/src/duHast/Data/data_to_shapely.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,19 @@
     :return: List of shapely points defining a polygon. (Empty list will be returned if less then 3 points in loop.)
     :rtype: List[shapely.point]
     """
 
     single_polygon_loop = []
     if geometry_object.data_type == geometry_polygon.DataPolygon.data_type:
         for point_double in geometry_object.outer_loop:
+            # check if a 2D or 3D point
+            if len(point_double) == 2:
+                # assume a Z value of 0.0 (room loops are 2D)
+                point_double.append(0.0)
+
             # need to add 1 to list for matrix multiplication
             # number of columns in first matrix (translation) must match number of rows in second matrix (point)
             translated_point = np.dot(
                 translation_matrix,
                 [point_double[0], point_double[1], point_double[2], 1.0],
             )
             p = sg.Point(translated_point[0], translated_point[1], translated_point[2])
@@ -128,14 +133,18 @@
     shapely_points = []
     # get inner loops
     if len(geometry_object.inner_loops) > 0:
         # there might be more then one inner loop
         for inner_loop in geometry_object.inner_loops:
             single_polygon_loop = []
             for point_double in inner_loop:
+                # check if a 2D or 3D point
+                if len(point_double) == 2:
+                    # assume a Z value of 0.0 (room loops are 2D)
+                    point_double.append(0.0)
                 # need to add 1 to list for matrix multiplication
                 # number of columns in first matrix (translation) must match number of rows in second matrix (point)
                 translated_point = np.dot(
                     translation_matrix,
                     [point_double[0], point_double[1], point_double[2], 1.0],
                 )
                 p = sg.Point(
```

### Comparing `DuHast-0.1.2/src/duHast/Data/process_ceilings_to_rooms.py` & `DuHast-0.1.3/src/duHast/Data/process_ceilings_to_rooms.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     - collects ceiling and room data instances by level ( assume a ceiling is always modelled as the room it is in )
     - converts room and ceiling outlines to shapely polygons
     - test for intersection of all ceilings on a given level with all rooms on a given level
     - stores any intersections found ( does a check how much area is  intersecting...if to small its assumed its not an intended intersection)
     - reports all rooms and any associated ceiling(s) found
 
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -29,16 +30,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import codecs
 import csv
@@ -294,14 +295,22 @@
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     # add some exception handling here in case intersect check throws an error
     try:
+        # check if a polygon is empty...if so ignore
+        if ceiling_polygon.is_empty or room_polygon.is_empty:
+            raise Exception(
+                "Ceiling {} or room {} polygon is empty. Ignored!".format(
+                    ceiling_poly_id, room_poly_id
+                )
+            )
+
         # check what exactly is happening
         if ceiling_polygon.intersects(room_polygon):
             # calculates percentage of overlapping ceiling area vs room area
             # anything less then 0.1 will be ignored...
             area_intersection_percentage_of_ceiling_vs_room = (
                 ceiling_polygon.intersection(room_polygon).area / room_polygon.area
             ) * 100
@@ -321,52 +330,69 @@
                 data_object_room = list(
                     filter(
                         lambda x: (x.instance_properties.id == room_poly_id),
                         data_objects[level_name][0],
                     )
                 )[0]
                 # get the ceiling object by its Revit id
-                data_object__ceiling = list(
+                data_object_ceiling = list(
                     filter(
                         lambda x: (x.instance_properties.id == ceiling_poly_id),
                         data_objects[level_name][1],
                     )
                 )[0]
                 # add ceiling object to associated elements list of room object
-                data_object_room.associated_elements.append(data_object__ceiling)
+                data_object_room.associated_elements.append(data_object_ceiling)
                 return_value.append_message(
-                    "Added ceiling {} to room {}".format(room_poly_id, ceiling_poly_id)
+                    "Added ceiling {} to room {}".format(ceiling_poly_id, room_poly_id)
                 )
     except Exception as e:
         # get the offending elements:
         data_object_room = list(
             filter(
                 lambda x: (x.instance_properties.id == room_poly_id),
                 data_objects[level_name][0],
             )
         )[0]
-        data_object__ceiling = list(
+        # set some predefined values in case the room object is not found
+        room_name = "unknown"
+        room_number = "unknown"
+        room_id = "unknown"
+        # populate values if room object is found
+        if data_object_room:
+            room_name = data_object_room.instance_properties.properties["Name"]
+            room_number = data_object_room.instance_properties.properties["Number"]
+            room_id = data_object_room.instance_properties.id
+
+        data_object_ceiling = list(
             filter(
                 lambda x: (x.instance_properties.id == ceiling_poly_id),
                 data_objects[level_name][1],
             )
         )[0]
+        # set some predefined values in case the ceiling object is not found
+        ceiling_id = "unknown"
+        # populate values if ceiling object is found
+        if data_object_ceiling:
+            ceiling_id = data_object_ceiling.instance_properties.id
+        
         return_value.append_message(
-            "Exception: {} \n"
-            + "offending room: room name: {} , room number: {} , room id: {} , is valid polygon: {}\n"
-            + "offending ceiling id: {} , is valid polygon: {}"
-        ).format(
-            e.message,
-            data_object_room.instance_properties.properties["Name"],
-            data_object_room.instance_properties.properties["Number"],
-            data_object_room.instance_properties.id,
-            room_polygon.is_valid,
-            data_object__ceiling.instance_properties.id,
-            ceiling_polygon.is_valid,
+            "Exception: {} \noffending room: room name: {} , room number: {} , room id: {} , \n...is valid polygon: {}\n...is empty polygon: {}\noffending ceiling id: {} , \n...is valid polygon: {}\n...is empty polygon: {}".format(
+                e,
+                room_name,
+                room_number,
+                room_id,
+                room_polygon.is_valid,
+                room_polygon.is_empty,
+                ceiling_id,
+                ceiling_polygon.is_valid,
+                ceiling_polygon.is_empty,
+            )
         )
+        
     return return_value
 
 
 # --------------- main functions ------------------
 
 
 def write_data_to_file(
@@ -483,76 +509,93 @@
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     # read exported ceiling and room data from file
     data_reader = _read_data(data_source_path)
     # check if read returned anything
-    if len(data_reader.data) > 0:
-        # build dictionary of objects by level and object type
-        data_objects = _build_dictionary_by_level_and_data_type(data_reader)
-        # key level name, value tuple ( rooms [index 0] and ceilings [index 1])
-        # loop over dic and process each key (level):
-        #       - check if rooms and ceilings
-        #       - intersection check
-        #       - update room object with ceiling match
-        # print(data_objects)
-        for level_name in data_objects:
-            # check rooms are on this level
-            if len(data_objects[level_name][0]) > 0:
-                # check ceilings are on this level
-                if len(data_objects[level_name][1]) > 0:
-                    polygons_by_type = {}
-                    # convert geometry data off all rooms and ceilings into dictionaries : key is Revit element id, values are shapely polygons
-                    room_polygons = dToS.get_shapely_polygons_from_geo_object(
-                        data_objects[level_name][0], dr.DataRoom.data_type
-                    )
-                    ceiling_polygons = dToS.get_shapely_polygons_from_geo_object(
-                        data_objects[level_name][1], dc.DataCeiling.data_type
+    if len(data_reader.data) == 0:
+        return_value.update_sep(
+            False, "File: {} did not contain any valid data.".format(data_source_path)
+        )
+        return return_value
+
+    print("\n".join(data_reader.debug_messages))
+
+    # build dictionary of objects by level and object type
+    data_objects = _build_dictionary_by_level_and_data_type(data_reader)
+    return_value.append_message(
+        "Data loaded contains {} levels: \n{}".format(
+            len(data_objects),
+            "...\n".join(
+                [
+                    "{}: {} entries, Rooms: {}, Ceilings: {}".format(
+                        key, len(value[0]) + len(value[1]), len(value[0]), len(value[1])
                     )
-                    polygons_by_type[dr.DataRoom.data_type] = room_polygons
-                    polygons_by_type[dc.DataCeiling.data_type] = ceiling_polygons
-                    # loop over rooms ids and find intersecting ceilings
-                    for room_poly_id in polygons_by_type[dr.DataRoom.data_type]:
-                        # check if valid room poly ( just in case that is a room in schedule only >> not placed in model , or unbound, or overlapping with other room)
-                        if len(room_polygons[room_poly_id]) > 0:
-                            # loop over each room polygon per room...there should only be one...
-                            for room_polygon in room_polygons[room_poly_id]:
-                                # find overlapping ceiling polygons
-                                for ceiling_poly_id in polygons_by_type[
-                                    dc.DataCeiling.data_type
+                    for key, value in data_objects.items()
+                ]
+            ),
+        )
+    )
+    # key level name, value tuple ( rooms [index 0] and ceilings [index 1])
+    # loop over dic and process each key (level):
+    #       - check if rooms and ceilings
+    #       - intersection check
+    #       - update room object with ceiling match
+    # print(data_objects)
+    for level_name in data_objects:
+        # check rooms are on this level
+        if len(data_objects[level_name][0]) > 0:
+            # check ceilings are on this level
+            if len(data_objects[level_name][1]) > 0:
+                polygons_by_type = {}
+                # convert geometry data off all rooms and ceilings into dictionaries : key is Revit element id, values are shapely polygons
+                room_polygons = dToS.get_shapely_polygons_from_geo_object(
+                    data_objects[level_name][0], dr.DataRoom.data_type
+                )
+                ceiling_polygons = dToS.get_shapely_polygons_from_geo_object(
+                    data_objects[level_name][1], dc.DataCeiling.data_type
+                )
+                polygons_by_type[dr.DataRoom.data_type] = room_polygons
+                polygons_by_type[dc.DataCeiling.data_type] = ceiling_polygons
+                # loop over rooms ids and find intersecting ceilings
+                for room_poly_id in polygons_by_type[dr.DataRoom.data_type]:
+                    # check if valid room poly ( just in case that is a room in schedule only >> not placed in model , or unbound, or overlapping with other room)
+                    if len(room_polygons[room_poly_id]) > 0:
+                        # loop over each room polygon per room...there should only be one...
+                        for room_polygon in room_polygons[room_poly_id]:
+                            # find overlapping ceiling polygons
+                            for ceiling_poly_id in polygons_by_type[
+                                dc.DataCeiling.data_type
+                            ]:
+                                for ceiling_polygon in ceiling_polygons[
+                                    ceiling_poly_id
                                 ]:
-                                    for ceiling_polygon in ceiling_polygons[
-                                        ceiling_poly_id
-                                    ]:
-                                        return_value.update(
-                                            _intersect_ceiling_vs_room(
-                                                ceiling_poly_id,
-                                                ceiling_polygon,
-                                                room_poly_id,
-                                                room_polygon,
-                                                data_objects,
-                                                level_name,
-                                            )
+                                    return_value.update(
+                                        _intersect_ceiling_vs_room(
+                                            ceiling_poly_id,
+                                            ceiling_polygon,
+                                            room_poly_id,
+                                            room_polygon,
+                                            data_objects,
+                                            level_name,
                                         )
-                        else:
-                            return_value.append_message(
-                                "Room with id {} has no valid room poly lines.".format(
-                                    room_poly_id
-                                )
+                                    )
+                    else:
+                        return_value.append_message(
+                            "Room with id {} has no valid room poly lines.".format(
+                                room_poly_id
                             )
-                else:
-                    return_value.append_message(
-                        "No ceilings found for level: {}".format(
-                            data_objects[level_name][0][0].level.name
                         )
-                    )
             else:
                 return_value.append_message(
-                    "No rooms found for level: {}".format(data_objects[level_name])
+                    "No ceilings found for level: {}".format(
+                        data_objects[level_name][0][0].level.name
+                    )
                 )
-        return_value.result = data_objects
-    else:
-        return_value.update_sep(
-            False, "File: {} did not contain any valid data.".format(data_source_path)
-        )
+        else:
+            return_value.append_message(
+                "No rooms found for level: {}".format(data_objects[level_name])
+            )
+    return_value.result = data_objects
+
     return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/gen_annotations_instance_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/Reporting/tags_independent_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import json
 
 from duHast.Revit.Annotation.independent_tags import get_all_independent_tags
 from duHast.Revit.Annotation.independent_tags_elbow_properties import (
@@ -34,15 +34,15 @@
 )
 from duHast.Revit.Annotation.independent_tags_tagged_elements import get_tagged_elements
 
 from duHast.Revit.Annotation.Reporting import (
     gen_annotations_instance_report_header as props,
 )
 
-from duHast.Revit.Common.Geometry.geometry import get_point_as_doubles
+from duHast.Revit.Common.Geometry.points import get_point_as_doubles
 from duHast.Revit.Common.revit_version import get_revit_version_number
 
 import Autodesk.Revit.DB as rdb
 
 
 def _convert_tagged_element_ids_to_int(data):
     """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/Utility/gen_annotation_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/annotation.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/arrow_heads.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/arrow_heads.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/dimensions.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/dimensions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/generic_annotation.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/generic_annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_elbow_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #
 #
 
 
 from Autodesk.Revit.DB import LeaderEndCondition
 
 from duHast.Revit.Common.revit_version import get_revit_version_number
-from duHast.Revit.Common.Geometry.geometry import get_point_as_doubles
+from duHast.Revit.Common.Geometry.points import get_point_as_doubles
 
 ELBOW_LOCATION = "elbow_location"
 LEADER_END = "leader_end"
 LEADER_REFERENCE = "leader_reference"
 LEADER_ELEMENT_REFERENCE_ID = "leader_element_reference_id"
 LEADER_LINKED_ELEMENT_REFERENCE_ID = "leader_linked_element_reference_id"
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_modify_properties.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_modify_properties.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/independent_tags_tagged_elements.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/multi_ref_annotation.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/multi_ref_annotation.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/purge_unused_annotation_types.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/purge_unused_annotation_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from Autodesk.Revit.DB import (
     BuiltInParameter,
     ElementId,
     FilteredElementCollector,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/spot_dimensions.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/spot_dimensions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/stair_path.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/stair_path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Annotation/text.py` & `DuHast-0.1.3/src/duHast/Revit/Annotation/text.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Areas/area_lines.py` & `DuHast-0.1.3/src/duHast/Revit/Areas/area_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                     "Failed to delete {} area separation line(s) on level {} with exception: {}".format(
                         len(element_ids_to_delete), level_name, e
                     ),
                 )
             return action_return_value
 
         tranny = Transaction(doc, "Deleting area lines on level: {}".format(level_name))
-        result_delete = transaction_manager(tranny, action, doc)
+        result_delete = transaction_manager(tranny, action)
         return_value.update(result_delete)
 
         # return list of lines not deleted!
         if result_delete.status:
             lines_by_level_name.pop(level_name, None)
             area_lines_return = []
             for key, value in lines_by_level_name.items():
@@ -202,15 +202,15 @@
                 ),
             )
         return action_return_value
 
     tranny = Transaction(
         doc, "Creating new area separation line(s) in view ".format(view.Name)
     )
-    result_create = transaction_manager(tranny, action, doc)
+    result_create = transaction_manager(tranny, action)
     return_value.update(result_create)
     return return_value
 
 
 def copy_area_lines_to_level_name(
     doc, view, area_lines, transaction_manager=in_transaction
 ):
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Areas/areas.py` & `DuHast-0.1.3/src/duHast/Revit/Areas/areas.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/BIM360/bim_360.py` & `DuHast-0.1.3/src/duHast/Revit/BIM360/bim_360.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/BIM360/util_bim_360.py` & `DuHast-0.1.3/src/duHast/Revit/BIM360/util_bim_360.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #
 
 import System
 import clr
 
 
 from duHast.Utilities.files_csv import read_csv_file
-from duHast.UI import file_item as fi
+from duHast.UI.Objects import file_item as fi
 
 
 def get_bim_360_revit_files_from_file_list(file_path_csv, extension):
     """
     Method reading BIM360 file data from a CSV file.
 
     :param file_path_csv: Fully qualified file path to CSV to be read.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/BuildingPads/Reporting/building_pads_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py` & `DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py` & `DuHast-0.1.3/src/duHast/Revit/BuildingPads/Utility/RevitBuildingPadsFilter.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 # import Autodesk
 from Autodesk.Revit.DB import BuiltInCategory, BuildingPadType , FilteredElementCollector
 
 def _get_all_building_pad_types_by_category(doc):
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/BuildingPads/building_pads.py` & `DuHast-0.1.3/src/duHast/Revit/BuildingPads/building_pads.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py` & `DuHast-0.1.3/src/duHast/Revit/BuildingPads/purge_unused_building_pad_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/category_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities import utility as util
 from duHast.Revit.Categories import categories as rCat
 from duHast.Revit.Categories.Utility import category_properties_get_utils as rCatPropGet
 from duHast.Revit.Categories.Utility import category_property_names as rCatPropNames
 from duHast.Revit.Categories.Utility import (
     elements_by_category_utils as rElementByCatUtils,
 )
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data_processor.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Data/Objects/category_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data.ifamily_processor import IFamilyProcessor
-from duHast.Revit.Categories.Data import category_data as rCatData
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects.ifamily_processor import IFamilyProcessor
+from duHast.Revit.Categories.Data.Objects import category_data as rCatData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities.Objects import result as res
 from duHast.Revit.Categories.Utility import category_property_names as rCatPropNames
 
 
 class CategoryProcessor(IFamilyProcessor):
     def __init__(self, pre_actions=None, post_actions=None):
         """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Data/category_data_purge_unused.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Data/category_data_purge_unused.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,62 +30,62 @@
 #
 #
 #
 
 # class used for stats reporting
 from duHast.Utilities.Objects import result as res
 from duHast.Revit.Common import delete as rDel
-from duHast.Revit.Family.Data import ifamily_data as IFamData
-from duHast.Revit.Categories.Data import category_data as rCatData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
+from duHast.Revit.Categories.Data.Objects import category_data as rCatData
 
-import Autodesk.Revit.DB as rdb
+from Autodesk.Revit.DB import ElementId
 
 
 def purge_unused_sub_categories(doc, processor):
     """
-This function deletes all user-created subcategories (with IDs greater than 0) that are not used by any element in the family or nested families.
+    This function deletes all user-created subcategories (with IDs greater than 0) that are not used by any element in the family or nested families.
 
-:param doc: Current Revit model document.
-:type doc: Autodesk.Revit.DB.Document
-:param processor: A CategoryProcessor object containing all subcategory information of the family document and any nested families.
-:type processor: :class:`.CategoryProcessor`
-
-:return: Result class instance.
-    - `result.status` (bool): True if all unused subcategories were deleted successfully or none needed to be deleted, otherwise False.
-    - `result.message` (str): Property updated in the format: "Found unused subcategory: family category Name : subcategory Name [subcategory Id]"
-
-On exception:
-    - `status` (bool): False.
-    - `message` (str): Contains the exception message.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param processor: A CategoryProcessor object containing all subcategory information of the family document and any nested families.
+    :type processor: :class:`.CategoryProcessor`
+
+    :return: Result class instance.
+        - `result.status` (bool): True if all unused subcategories were deleted successfully or none needed to be deleted, otherwise False.
+        - `result.message` (str): Property updated in the format: "Found unused subcategory: family category Name : subcategory Name [subcategory Id]"
+
+    On exception:
+        - `status` (bool): False.
+        - `message` (str): Contains the exception message.
 
-:rtype: :class:`.Result`
-"""
+    :rtype: :class:`.Result`
+    """
 
     # from processor instance get all root category entries where usage counter == 0 and subCategoryId > 0 (pointing to a custom sub category and not a built in one).
     # delete those subcategories by id
 
     return_value = res.Result()
 
     ids_to_delete = []
     # get categories found in root processor data only
-    root_fam_data = processor._findRootFamilyData()
+    root_fam_data = processor._find_root_family_data()
     # get all root category entries where usage counter == 0 and subCategoryId > 0 (pointing to a custom sub category and not a built in one).
     for root_fam in root_fam_data:
         if (
             root_fam[IFamData.USAGE_COUNTER] == 0
             and root_fam[rCatData.SUB_CATEGORY_ID] > 0
         ):
             return_value.append_message(
                 "Found unused sub category: {} : {} [{}]".format(
                     root_fam[rCatData.CATEGORY_NAME],
                     root_fam[rCatData.SUB_CATEGORY_NAME],
                     (root_fam[rCatData.SUB_CATEGORY_ID]),
                 )
             )
-            ids_to_delete.append(rdb.ElementId(root_fam[rCatData.SUB_CATEGORY_ID]))
+            ids_to_delete.append(ElementId(root_fam[rCatData.SUB_CATEGORY_ID]))
     # delete any subcategories found
     if len(ids_to_delete) > 0:
         result_delete = rDel.delete_by_element_ids(
             doc, ids_to_delete, "Deleting unused sub categories.", "Subcategories"
         )
         return_value.update(result_delete)
     else:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/categories_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Reporting/categories_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Reporting/categories_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_properties_get_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_properties_set_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Utility/category_property_names.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Utility/category_property_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/Utility/elements_by_category_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/categories.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/categories_model.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/categories_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Revit category helper functions for project files.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
+
 #
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -21,18 +22,18 @@
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
-
+from System import Enum
 from collections import namedtuple
 
-from Autodesk.Revit.DB import Category
+from Autodesk.Revit.DB import BuiltInCategory, Category
 
 
 # tuples containing categories data
 category_data = namedtuple("category_data", "category_name sub_category_name id")
 
 
 def get_categories_in_model(doc):
@@ -66,26 +67,53 @@
             )
 
     return categories
 
 
 def get_category_from_builtInCategory(doc, built_in_category):
     """
-    Returns a category based on the buil in category enum value.
+    Returns a category based on the build in category enum value.
 
     :param doc: The current model document.
     :type doc: Autodesk.Revit.DB.Document
     :param built_in_category: The built in category
     :type built_in_category: Autodesk.Revit.DB.BuiltInCategory
     :return: A category
     :rtype: Autodesk.Revit.DB.Category
     """
-    
+
     return Category.GetCategory(doc, built_in_category)
 
+
+def get_builtInCategory_from_category(doc, category):
+    """
+    Returns a built in category enum value based on the category object.
+
+    :param doc: The current model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param category: The category object
+    :type category: Autodesk.Revit.DB.Category
+    :return: The built in category enum value
+    :rtype: Autodesk.Revit.DB.BuiltInCategory
+    """
+
+    values = Enum.GetValues(BuiltInCategory)
+    names = Enum.GetNames(BuiltInCategory)
+    for value, name in zip(values, names):
+        try:
+            cat = Category.GetCategory(doc, value)
+            if cat == None:
+                continue
+            if cat.Name == category.Name:
+                return value
+        except:
+            continue
+    return None
+
+
 def get_category_by_names(doc, main_category_name, sub_category_name):
     """
     Retrieves a category object from a document based on the given main category name and optional sub category name.
 
     Args:
         doc (document object): The document object from which to retrieve the category.
         main_category_name (str): The name of the main category to search for.
@@ -102,8 +130,25 @@
             if sub_category_name == main_category_name:
                 return main_category
             else:
                 for sub_cat in main_category.SubCategories:
                     if sub_cat.Name == sub_category_name:
                         return sub_cat
     return return_value
-            
+
+
+def get_builtin_category_by_name(category_name):
+    """
+    Returns the built in category enum value based on the category name.(i.e. OST_Walls)
+
+    :param category_name: The category name
+    :type category_name: str
+    :return: The built in category enum value
+    :rtype: Autodesk.Revit.DB.BuiltInCategory
+    """
+
+    values = Enum.GetValues(BuiltInCategory)
+    names = Enum.GetNames(BuiltInCategory)
+    for value, name in zip(values, names):
+        if name == category_name:
+            return value
+    return None
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/change_family_category.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/change_family_category.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Categories/family_sub_categories.py` & `DuHast-0.1.3/src/duHast/Revit/Categories/family_sub_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py` & `DuHast-0.1.3/src/duHast/Revit/Ceilings/Export/to_data_ceiling.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import Autodesk.Revit.DB as rdb
 
 from duHast.Revit.Common import (
     design_set_options as rDesignO,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/Geometry/geometry.py` & `DuHast-0.1.3/src/duHast/Revit/Ceilings/Geometry/geometry.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 import Autodesk.Revit.DB as rdb
 
 from duHast.Revit.Ceilings import ceilings as rCeiling
 from duHast.Data.Objects.Properties.Geometry import from_revit_conversion as rCon
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Ceilings/Utility/ceilings_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import Autodesk.Revit.DB as rdb
 
 
 def _get_all_ceiling_types_by_category(doc):
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/Utility/ceilings_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,44 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit ceilings utility functions. 
+This module contains a number of helper functions relating to Family elements
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-from duHast.Revit.Ceilings.Utility import ceilings_filter as rCeilingsFilter
-
-
-def build_ceiling_type_dictionary(collector, dic):
-    """
-    Returns the dictionary past in with keys and or values added retrieved from collector past in.
-    Keys are built in ceiling family type names.
-    TODO: Use more generic code.
-    :param collector: A filtered element collector containing ceiling types.
-    :type collector: Autodesk.Revit.DB.FilteredElementCollector
-    :param dic: A dictionary containing key: ceiling type family name, value: list of ids belonging to that type.
-    :type dic: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
-    :return: A dictionary containing key: built in ceiling type family name, value: list of ids belonging to that type.
-    :rtype: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
-    """
-
-    for c in collector:
-        if dic.has_key(c.FamilyName):
-            if c.Id not in dic[c.FamilyName]:
-                dic[c.FamilyName].append(c.Id)
-        else:
-            dic[c.FamilyName] = [c.Id]
-    return dic
-
+from Autodesk.Revit.DB import FilteredElementCollector, Family
 
-def sort_ceiling_types_by_family_name(doc):
-    """
-    Returns a dictionary of all ceiling types in the model where key is the build in wall family name, values are ids of associated wall types.
-    TODO: Use more generic code.
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: A dictionary containing key: built in ceiling type family name, value: list of ids belonging to that type.
-    :rtype: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
-    """
+def get_name_to_family_dict(rvt_doc):
+    '''
+    Create a dictionary of family name and the Family element
+    :param rvt_doc: Revit document
+    :type rvt_doc: Autodesk.Revit.DB.Document
+    :return: Dictionary of family name and Family element
+    :rtype: dict
+    '''
 
-    # get all ceiling Type Elements
-    wts = rCeilingsFilter._get_ceiling_types_by_class(doc)
-    # get all ceiling types including in place ceiling families
-    wts_two = rCeilingsFilter._get_all_ceiling_types_by_category(doc)
-    usedWts = {}
-    usedWts = build_ceiling_type_dictionary(wts, usedWts)
-    usedWts = build_ceiling_type_dictionary(wts_two, usedWts)
-    return usedWts
+    #Get all the families in the model
+    all_families = FilteredElementCollector(rvt_doc).OfClass(Family).ToElements()
+    #create a dictionary of family name and family object
+    family_dict = {fam.Name: fam for fam in all_families}
+    return family_dict
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/ceilings.py` & `DuHast-0.1.3/src/duHast/Revit/Ceilings/ceilings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py` & `DuHast-0.1.3/src/duHast/Revit/Ceilings/purge_unused_ceiling_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from duHast.Revit.Family import purge_unused_family_types as rFamPurge
 from duHast.Revit.Common import purge_utils as rPurgeUtils
 from duHast.Revit.Ceilings import ceilings as rCeiling
 from duHast.Revit.Ceilings.Utility import ceilings_type_sorting as rCeilingTypeSort
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Geometry/curve.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Geometry/curve.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from Autodesk.Revit.DB import Arc, Line, Transform, XYZ
 
-from duHast.Revit.Common.Geometry.geometry import is_close
+from duHast.Utilities.compare import is_close
 from duHast.Utilities.Objects import result as res
 
 
 def is_curve_is_within_curve(curve_one, curve_two):
     """
     Checks whether one curve is completely within another curve.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Geometry/geometry.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Geometry/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,54 +5,49 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
+from duHast.Revit.Common.Geometry.points import (
+    are_points_identical,
+    check_duplicate_point,
+    flatten_xyz_point,
+    get_point_as_doubles,
+    get_point_as_string,
+)
+from duHast.Utilities.compare import is_close
+
 clr.AddReference("System.Core")
 from System import Linq
+from System import Math
 
 clr.ImportExtensions(Linq)
 
-from Autodesk.Revit.DB import UV, PlanarFace, XYZ
-
-
-# ---------------------------- debug ----------------------------
-def get_point_as_string(point):
-    """
-    Returns Revit point as a string.
-
-    :param point: A revit point.
-    :type point: Autodesk.Revit.DB.XYZ
-
-    :return: String in format 'X:Y:Z'
-    :rtype: str
-    """
-
-    return str(point.X) + " : " + str(point.Y) + " : " + str(point.Z)
+from Autodesk.Revit.DB import BoundingBoxXYZ, PlanarFace, XYZ
 
 
 def get_edge_as_string(edge):
     """
     Returns a revit edge as a string.
 
     :param edge: A revit edge.
@@ -115,104 +110,14 @@
 
     return is_inside
 
 
 # ---------------------------- math utility ----------------------------
 
 
-def is_close(a, b, rel_tol=1e-09, abs_tol=0.0):
-    """
-    Compares two floats with a tolerance. Returns True if they are close enough, otherwise False
-
-    refer to: https://stackoverflow.com/questions/5595425/what-is-the-best-way-to-compare-floats-for-almost-equality-in-python
-
-    :param a: A float
-    :type a: float
-    :param b: A float
-    :type b: float
-    :param rel_tol: Relative tolerance used to compare the two floats, defaults to 1e-09
-    :type rel_tol: float, optional
-    :param abs_tol: Absolute tolerance used to compare the two floats, defaults to 0.0
-    :type abs_tol: float, optional
-
-    :return: Returns True if they are close enough to be considered equal, otherwise False
-    :rtype: bool
-    """
-
-    return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
-
-
-def are_points_identical(p1, p2):
-    """
-    Compares the X,Y,Z values of two revit point and returns True if they are the same, otherwise False
-
-    :param p1: A revit point.
-    :type p1: Autodesk.Revit.DB.XYZ
-    :param p2: A revit point.
-    :type p2: Autodesk.Revit.DB.XYZ
-
-    :return: True if they are the same, otherwise False.
-    :rtype: bool
-    """
-
-    if is_close(p1.X, p2.X) and is_close(p1.Y, p2.Y) and is_close(p1.Z, p2.Z):
-        return True
-    else:
-        return False
-
-
-def check_duplicate_point(points, point):
-    """
-    Checks whether a collection of points contains another given point and returns True if that is the case.
-
-    :param points: List of revit points
-    :type points: list Autodesk.Revit.DB.XYZ
-    :param point: A revit point.
-    :type point: Autodesk.Revit.DB.XYZ
-
-    :return: True if point is in collection, otherwise False.
-    :rtype: bool
-    """
-
-    for p1 in points:
-        if are_points_identical(p1, point):
-            return True
-    return False
-
-
-def get_point_as_doubles(point):
-    """
-    Converts a revit XYZ to a list of doubles in order x,y,z.
-
-    :param point: A revit point.
-    :type point: Autodesk.Revit.DB.XYZ
-
-    :return: List of doubles in order of x,y,z
-    :rtype: list double
-    """
-
-    return [point.X, point.Y, point.Z]
-
-
-def flatten_xyz_point(point):
-    """
-    Flattens a XYZ point to a UV by omitting the Z value of the XYZ.
-
-    https://thebuildingcoder.typepad.com/blog/2008/12/2d-polygon-areas-and-outer-loop.html
-
-    :param point: A revit point.
-    :type point: Autodesk.Revit.DB.XYZ
-
-    :return: A 2D point (UV)
-    :rtype:  Autodesk.Revit.DB.UV
-    """
-
-    return UV(point.X, point.Y)
-
-
 def flatten_xyz_point_list(polygon):
     """
     Flattens a list of XYZ points to a list of UV points by omitting the Z value of each XYZ.
 
     https://thebuildingcoder.typepad.com/blog/2008/12/2d-polygon-areas-and-outer-loop.html
 
     :param polygon: list of XYZ points
@@ -840,59 +745,32 @@
     :type vector: list or tuple
     :return: The negated vector
     :rtype: list
     """
     return [-x for x in vector]
 
 
-def sort_points_by_min_and_max(min_pt, max_pt):
+def merge_bounding_box_xyz(bounding_box_xyz_0, bounding_box_xyz_1):
     """
-    Takes BoundingBox or Outline Min and Max points and
-    returns the true Min and Max points. This is to ensure
-    no zero thickness geometries are created.
-    :param min_pt: The minimum point
-    :type min_pt: XYZ
-    :param max_pt: The maximum point
-    :type max_pt: XYZ
-    :return: The sorted points
-    :rtype: tuple
-    """
-    min_x = min_pt.X
-    min_y = min_pt.Y
-    min_z = min_pt.Z
-
-    max_x = max_pt.X
-    max_y = max_pt.Y
-    max_z = max_pt.Z
-
-    smin_x = min(min_x, max_x)
-    smin_y = min(min_y, max_y)
-    smax_x = max(min_x, max_x)
-    smax_y = max(min_y, max_y)
-
-    return (XYZ(smin_x, smin_y, min_z), XYZ(smax_x, smax_y, max_z))
-
-def transform_point_by_elem_transform(pt, transform):
-    """
-    Transforms a point by an element transform
-    :param pt: The point to transform
-    :type pt: XYZ
-    :param transform: The transform to use
-    :type transform: Transform
-    :return: The transformed point
-    :rtype: XYZ
-    """
-
-    x = pt.X
-    y = pt.Y
-    z = pt.Z
-
-    b0 = transform.get_Basis(0)
-    b1 = transform.get_Basis(1)
-    b2 = transform.get_Basis(2)
-    origin = transform.Origin
-
-    x_new = x * b0.X + y * b1.X + z * b2.X + origin.X
-    y_new = x * b0.Y + y * b1.Y + z * b2.Y + origin.Y
-    z_new = x * b0.Z + y * b1.Z + z * b2.Z + origin.Z
-
-    return XYZ(x_new, y_new, z_new)
+    Merges two bounding boxes into one.
+    :param bounding_box_xyz_0: The first bounding box
+    :type bounding_box_xyz_0: BoundingBoxXYZ
+    :param bounding_box_xyz_1: The second bounding box
+    :type bounding_box_xyz_1: BoundingBoxXYZ
+
+    :return: The merged bounding box
+    :rtype: BoundingBoxXYZ
+    """
+
+    merged_result = BoundingBoxXYZ()
+    merged_result.Min = XYZ(
+        Math.Min(bounding_box_xyz_0.Min.X, bounding_box_xyz_1.Min.X),
+        Math.Min(bounding_box_xyz_0.Min.Y, bounding_box_xyz_1.Min.Y),
+        Math.Min(bounding_box_xyz_0.Min.Z, bounding_box_xyz_1.Min.Z),
+    )
+
+    merged_result.Max = XYZ(
+        Math.Max(bounding_box_xyz_0.Max.X, bounding_box_xyz_1.Max.X),
+        Math.Max(bounding_box_xyz_0.Max.Y, bounding_box_xyz_1.Max.Y),
+        Math.Max(bounding_box_xyz_0.Max.Z, bounding_box_xyz_1.Max.Z),
+    )
+    return merged_result
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/colour_base.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/colour_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_cut.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_cut.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_graphic_base.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_graphic_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
 from duHast.Revit.Common.Objects.Data.colour_base import ColourBase
-from duHast.Revit.LinePattern.Objects.Data.line_pattern_settings import (
+from duHast.Revit.LinePattern.Data.Objects.line_pattern_settings import (
     LinePatternSettings,
 )
 
 
 class LineGraphicBase(base.Base):
     def __init__(self, data_type="unknown", j=None, **kwargs):
         """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/line_projection.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/line_projection.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_background.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_background.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_foreground.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_graphic_base.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_graphic_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #
 #
 
 import json
 
 from duHast.Utilities.Objects import base
 from duHast.Revit.Common.Objects.Data.colour_base import ColourBase
-from duHast.Revit.LinePattern.Objects.Data.fill_pattern_settings import (
+from duHast.Revit.LinePattern.Data.Objects.fill_pattern_settings import (
     FillPatternSettings,
 )
 
 
 class PatternGraphicBase(base.Base):
     def __init__(self, data_type="unknown", j=None, **kwargs):
         """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/Data/pattern_settings_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Objects/ParameterMappingDirective.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Objects/ParameterMappingDirective.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+"""
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+A parameter mapping class
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Parameter mappings are used to transfer parameter values from one parameter to another. This class is used to define 
+
+- source parameter name
+- source parameter is instance
+- target parameter name
+- parameter value
+- parameter modifier ( of the parameter value retrieved from source parameter)
+- parameter getter ( a function that returns the value of the source parameter)
+
+"""
+# License:
+#
+#
+# Revit Batch Processor Sample Code
+#
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
+#
+#
+#
+
 import json
 
 from duHast.Revit.Common.Objects.ParameterDirectiveBase import ParameterDirectiveBase
 
 
 class ParameterMappingDirective(ParameterDirectiveBase):
     """Class for parameter mapping directives."""
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Reporting/groups_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Reporting/groups_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Reporting/worksets_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Reporting/worksets_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Reporting/worksets_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Reporting/worksets_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Utility/element_copying.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Utility/element_copying.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Utility/element_spatial_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Utility/element_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/Utility/revit_to_data_conversion.py` & `DuHast-0.1.3/src/duHast/Revit/Common/Utility/revit_to_data_conversion.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/common.py` & `DuHast-0.1.3/src/duHast/Revit/Common/common.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter_actions.py` & `DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter_actions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/custom_element_filter_tests.py` & `DuHast-0.1.3/src/duHast/Revit/Common/custom_element_filter_tests.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/delete.py` & `DuHast-0.1.3/src/duHast/Revit/Common/delete.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/design_set_options.py` & `DuHast-0.1.3/src/duHast/Revit/Common/design_set_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import System
 
 # import common library modules
-from duHast.Revit.Common import parameter_get_utils as rParaGet
+#from duHast.Revit.Common import parameter_get_utils as rParaGet
 
 
 # import Autodesk
 from Autodesk.Revit.DB import BuiltInParameter, DesignOption, Element, FilteredElementCollector
 
 # -------------------------------------------- common variables --------------------
 #: header used in reports
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/element_filtering.py` & `DuHast-0.1.3/src/duHast/Revit/Common/element_filtering.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/file_io.py` & `DuHast-0.1.3/src/duHast/Revit/Common/file_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 
 from Autodesk.Revit.DB import (
     RelinquishOptions,
     TransactWithCentralOptions,
@@ -50,15 +50,15 @@
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :param compact_central_file: option to compact the central file, defaults to False
     :type compact_central_file: bool, optional
     :return:
         Result class instance.
-        - .result = True if successfully synced file. Otherwise False.
+        - .status True if successfully synced file. Otherwise False.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     # set up sync settings
     ro = RelinquishOptions(True)
     transaction_options = TransactWithCentralOptions()
@@ -93,15 +93,15 @@
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :param full_file_name: The fully qualified file path of where to save the file.
     :type full_file_name: string
     :return:
         Result class instance.
-        - .result = True if successfully saved file, otherwise False.
+        - .status True if successfully saved file, otherwise False.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         worksharing_save_as_option = WorksharingSaveAsOptions()
         worksharing_save_as_option.OpenWorksetsDefault = (
@@ -141,15 +141,15 @@
     :type name_data: List of string arrays in format[[oldname, newName]]
     :param file_extension: The file extension used for the new file, defaults to '.rfa'
     :type file_extension: str, optional
     :param compact_file: Flag whether family is to be compacted on save, defaults to False
     :type compact_file: bool, optional
     :return:
         Result class instance.
-            - .result = True if successfully saved file, otherwise False.
+            - .status True if successfully saved file, otherwise False.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     revit_file_name = fileIO.get_file_name_without_ext(current_full_file_name)
     new_file_name = ""
     match = False
@@ -200,15 +200,15 @@
     :type current_full_file_name: str
     :param name_data: Old name and new name are revit file names without file extension. Used to rename the model on save from old name to new name.
     :type name_data: List of string arrays in format[[oldname, newName]]
     :param file_extension: The file extension used for the new file, defaults to '.rvt'
     :type file_extension: str, optional
     :return:
         Result class instance.
-        - .result = True if successfully saved file, otherwise False.
+        - .status True if successfully saved file, otherwise False.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     # added str() around this expression to satisfy sphinx auto code documentation
     # it will throw an exception when concatenating the string in the return statement
     revit_file_name = str(fileIO.get_file_name_without_ext(current_full_file_name))
@@ -252,15 +252,15 @@
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :param compact_file: True file will be compacted on save, defaults to False
     :type compact_file: bool, optional
     :return:
             Result class instance.
-            - .result = True if file was saved successfully. Otherwise False.
+            - .status True if file was saved successfully. Otherwise False.
             - .message = 'Saved revit file!'
             On exception:
             - result.status (bool) will be False.
             - result.message will contain exception message.
     :rtype: :class:`.Result`
     """
 
@@ -290,15 +290,15 @@
     :param workset_name_grid_level: _description_, defaults to 'Shared Levels and Grids'
     :type workset_name_grid_level: str, optional
     :param workset_name: _description_, defaults to 'Workset1'
     :type workset_name: str, optional
 
     :return:
             Result class instance.
-            - .result = True if worksharing was enabled successfully. Otherwise False.
+            - .status True if worksharing was enabled successfully. Otherwise False.
             - .message = 'Successfully enabled worksharing.'
             On exception:
             - result.status (bool) will be False.
             - result.message will contain exception message.
     :rtype: :class:`.Result`
     """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/groups.py` & `DuHast-0.1.3/src/duHast/Revit/Common/groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 clr.AddReference("System.Core")
 from System import Linq
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/parameter_get_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Common/parameter_get_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/parameter_grouping.py` & `DuHast-0.1.3/src/duHast/Revit/Common/parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/parameter_set_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Common/parameter_set_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             except Exception as e:
                 action_return_value.update_sep(
                     False, "Failed with exception: {}".format(e)
                 )
             return action_return_value
 
         transaction = rdb.Transaction(doc, transaction_name)
-        return_value = in_transaction(transaction, action, doc)
+        return_value = in_transaction(transaction, action)
     elif para.StorageType == rdb.StorageType.Double:
         # THIS IS THE KEY:  Use SetValueString instead of Set.  Set requires your data to be in
         # whatever internal units of measure Revit uses. SetValueString expects your value to
         # be in whatever the current DisplayUnitType (units of measure) the document is set to
         # for the UnitType associated with the parameter.
         #
         # So SetValueString is basically how the Revit GUI works.
@@ -125,15 +125,15 @@
             except Exception as e:
                 action_return_value.update_sep(
                     False, "Failed with exception: {}".format(e)
                 )
             return action_return_value
 
         transaction = rdb.Transaction(doc, transaction_name)
-        return_value = in_transaction(transaction, action, doc)
+        return_value = in_transaction(transaction, action)
     elif para.StorageType == rdb.StorageType.Integer:
 
         def action():
             action_return_value = res.Result()
             try:
                 para.Set(int(value_as_string))
                 action_return_value.message = "Changed parameter value of type integer.[ {} ] from: {} to: {}".format(
@@ -142,15 +142,15 @@
             except Exception as e:
                 action_return_value.update_sep(
                     False, "Failed with exception: {}".format(e)
                 )
             return action_return_value
 
         transaction = rdb.Transaction(doc, transaction_name)
-        return_value = in_transaction(transaction, action, doc)
+        return_value = in_transaction(transaction, action)
     elif para.StorageType == rdb.StorageType.String:
 
         def action():
             action_return_value = res.Result()
             try:
                 para.Set(value_as_string)
                 action_return_value.message = "Changed parameter value of type string.[ {} ] from: {} to: {}".format(
@@ -159,15 +159,15 @@
             except Exception as e:
                 action_return_value.update_sep(
                     False, "Failed with exception: {}".format(e)
                 )
             return action_return_value
 
         transaction = rdb.Transaction(doc, transaction_name)
-        return_value = in_transaction(transaction, action, doc)
+        return_value = in_transaction(transaction, action)
     else:
         # dead end
         return_value.update_sep(
             False,
             "Dont know what to do with this storage type: {}".format(para.StorageType),
         )
     return return_value
@@ -328,20 +328,27 @@
         On exception:
 
         - Set parameter.status (bool) will be False.
         - Set parameter.message will contain the exception message.
     """
 
     return_value = res.Result()
+    
     if not isinstance(parameter_value, str):
         parameter_value = str(parameter_value)
+    
     para = element.LookupParameter(parameter_name)
-    return_value = set_parameter_value_simple(
-        para=para, value_as_string=parameter_value
-    )
+    
+    if(para != None):
+        return_value = set_parameter_value_simple(
+            para=para, value_as_string=parameter_value
+        )
+    else:
+        return_value.update_sep(False, "Parameter: {} not found.".format(parameter_name))
+    
     return return_value
 
 
 def set_builtin_parameter_without_transaction_wrapper_by_name(
     element, parameter_definition, parameter_value
 ):
     """
@@ -366,14 +373,21 @@
 
         - Set parameter.status (bool) will be False.
         - Set parameter.message will contain the exception message.
 
     """
 
     return_value = res.Result()
+
     if not isinstance(parameter_value, str):
         parameter_value = str(parameter_value)
+    
     para = element.get_Parameter(parameter_definition)
-    return_value = set_parameter_value_simple(
-        para=para, value_as_string=parameter_value
-    )
+    
+    if(para != None):
+        return_value = set_parameter_value_simple(
+            para=para, value_as_string=parameter_value
+        )
+    else:
+        return_value.update_sep(False, "Parameter: {} not found.".format(parameter_definition))
+
     return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/phases.py` & `DuHast-0.1.3/src/duHast/Revit/Common/phases.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 
 def get_all_phases(doc):
     """
     Returns a dictionary where key is the id and value is the name of the phase.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/purge_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Common/purge_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/transaction.py` & `DuHast-0.1.3/src/duHast/Revit/Rooms/room_tags.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Revit transaction wrapper utility functions.
+This module contains a number of helper functions relating to Revit rooms tags. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
-
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
+#
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
 # Copyright 2023, Jan Christel
@@ -17,64 +15,66 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
+#
 
-# class used for stats reporting
+from Autodesk.Revit.DB import Element, Transaction
+from duHast.Revit.Common.transaction import in_transaction
 from duHast.Utilities.Objects import result as res
 
-# type checker
-# from typing import List, Callable
 
-# --------------------------------------------Transactions-----------------------------------------
-
-
-def in_transaction(
-    tranny,  #
-    action,  # type: Callable[[], res.Result]
-    doc=None,  # used as placeholder...
-):
-    # type: (...) -> res.Result
+def move_tag_to_room(doc, tag_id, transaction_manager=in_transaction):
     """
-    Revit transaction wrapper.
-
-    This function is used to execute any actions requiring a transaction in the Revit api. On exception this will roll back the transaction.
+    Moves a room tag to the associated rooms location point.
 
-    :param tranny: The transaction to be executed.
-    :type tranny: Autodesk.Revit.DB.Transaction
-    :param doc: The current model document. (not used in this function)
+    :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param action: The action to be nested within the transaction. This needs to return a Result class instance!
-    :type action: action().
-
-    :return:
-        Result class instance.
-
-        - .result = True if successfully executed transaction, otherwise False.
-
+    :param tag_id: The element id of the tag to be moved to the room.
+    :type tag_id: Autodesk.Revit.DB.ElementId
+    :param transaction_manager: The transaction manager used to perform the modifications.
+    :type transaction_manager: (function)
+    :return: Result class instance.
+
+        - Tag moving status returned in result.status. False if an exception occurred, otherwise True.
+        - result.message will contain the name and number of the room.
+
+        On exception (handled by optimizer itself!):
+
+        - result.status (bool) will be False.
+        - result.message will contain the name and number of the room and the exception message.
+        
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
-    try:
-        tranny.Start()
+    rt = doc.GetElement(tag_id)
+    room_tag_point = rt.Location.Point
+    room_location_point = rt.Room.Location.Point
+    room_data = "{} {}".format(rt.Room.Number, Element.Name.GetValue(rt.Room))
+    translation = room_location_point - room_tag_point
+
+    def action():
+        action_return_value = res.Result()
         try:
-            tranny_result = action()
-            tranny.Commit()
-            # check what came back
-            if tranny_result != None:
-                # store false value
-                return_value = tranny_result
+            rt.Location.Move(translation)
+            action_return_value.message = "Moved tag to room: {}".format(room_data)
         except Exception as e:
-            tranny.RollBack()
-            return_value.update_sep(False, "Failed with exception: {}".format(e))
-    except Exception as e:
-        return_value.update_sep(False, "Failed with exception: {}".format(e))
+            action_return_value.update_sep(
+                False,
+                "Failed to move tag to room: {} with exception: {}".format(
+                    room_data, e
+                ),
+            )
+        return action_return_value
+
+    transaction = Transaction(doc, "Moving room tag to room : {}".format(room_data))
+    return_value.update(transaction_manager(transaction, action))
     return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Common/worksets.py` & `DuHast-0.1.3/src/duHast/Revit/Common/worksets.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 clr.AddReference("System.Core")
 from System import Linq
@@ -49,16 +49,18 @@
     BuiltInParameter,
     Element,
     ElementId,
     ElementWorksetFilter,
     FilteredElementCollector,
     FilteredWorksetCollector,
     Transaction,
+    Workset,
     WorksetKind,
     WorksetDefaultVisibilitySettings,
+    WorksetTable,
 )
 
 # --------------------------------------------- utility functions ------------------
 
 
 def get_workset_id_by_name(doc, workset_name):
     """
@@ -189,15 +191,15 @@
     :type collector: Autodesk.Revit.DB.FilteredElementCollector
     :param element_type_name: A description used in the status message returned.
     :type element_type_name: str
 
     :return:
         Result class instance.
 
-        - .result = True if successfully moved all elements to new workset. Otherwise False.
+        - .status = True if successfully moved all elements to new workset. Otherwise False.
         - .message will contain stats in format [success :: failure]
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     return_value.message = "Changing: {} workset to: {} ".format(
@@ -355,15 +357,15 @@
     :type report_path: str
     :param revit_file_path: The fully qualified file path of the Revit file. Will be used to identify the file in the report data.
     :type revit_file_path: str
 
     :return:
         Result class instance.
 
-        - .result = True if:
+        - .status = True if:
 
             - successfully updated all workset default visibility where different to report
             - or none needed updating.
 
         - Otherwise False:
 
             - An exception occurred.
@@ -437,7 +439,61 @@
                     ),
                 )
     else:
         return_value.update_sep(
             True, "No settings found for file: {}".format(file_name)
         )
     return return_value
+
+
+def create_workset(doc, workset_name):
+    """
+    Creates a workset with a given name in a document.
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param workset_name: The name of the workset to be created
+    :type workset_name: str
+
+    :return:
+        Result class instance.
+
+        - .status = True if:
+
+            - successfully created the workset
+
+        - Otherwise False:
+
+            - An exception occurred.
+            - A workset with that name already exists.
+            - Document is not workshared
+
+        - Common:
+
+            - .message will contain each workset
+
+        .result will contain the workset element in a list if successfully created, otherwise an empty list.
+
+    :rtype: :class:`.Result`
+    """
+
+    return_value = res.Result()
+    if (doc.IsWorkshared):
+        if(WorksetTable.IsWorksetNameUnique(doc, workset_name)):
+            def action():
+                action_return_value = res.Result()
+                try:
+                    new_workset = Workset.Create(doc, workset_name)
+                    action_return_value.update_sep(True, "Workset {} created.".format(workset_name))
+                    action_return_value.result.append(new_workset)
+                except Exception as e:
+                    action_return_value.update_sep(False, "Failed to create workset {} with exception: {}".format(workset_name,e))
+                return action_return_value
+            
+            transaction = Transaction(doc, "Adding workset {}".format(workset_name))
+            tranny_status = rTran.in_transaction(transaction, action)
+            return_value.update(tranny_status)
+        else:
+            return_value.update_sep(False, "Workset name already exists: {}".format(workset_name))
+    else:
+        return_value.update_sep(False, "Cant create a workset in a non workshared file.")
+    return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/DetailItems/Utility/detail_items_type_sorting.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 
 def build_detail_type_ids_dictionary(collector):
     """
     Returns the dictionary keys is autodesk.revit.db element type as string and values are available type ids.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/DetailItems/detail_items.py` & `DuHast-0.1.3/src/duHast/Revit/DetailItems/detail_items.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py` & `DuHast-0.1.3/src/duHast/Revit/DetailItems/purge_unused_detail_item_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 
 from duHast.Revit.Family import purge_unused_family_types as rFamPurge
 from duHast.Revit.Common import purge_utils as rPurgeUtils
 from duHast.Revit.DetailItems import detail_items as rDetail
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Doors/doors.py` & `DuHast-0.1.3/src/duHast/Revit/Doors/doors.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Doors/doors_create.py` & `DuHast-0.1.3/src/duHast/Revit/Doors/doors_create.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2019.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2020.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2021.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2022.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/export_ifc_config_2023.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_coordinates.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_settings.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/Utility/ifc_export_space_boundaries.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/export.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/export.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/export_ifc.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/export_ifc.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Exports/export_navis.py` & `DuHast-0.1.3/src/duHast/Revit/Exports/export_navis.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_base_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities import directory_io as dirIO, files_io as fileIO
 from duHast.Revit.Common import file_io as rFile
 from duHast.Revit.Family.Data import family_base_data_utils as rFamBaseDataUtils
 
 # import Autodesk
 # import Autodesk.Revit.DB as rdb
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_circular_referencing.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import threading
 import os
@@ -233,15 +233,14 @@
         for nested_fam in overall_family_base_nested_data:
             try:
                 # get the index of the match
                 index_match = nested_fam.rootPath.index(
                     overall_family_base_root_data[i].name
                 )
                 if index_match > 0:
-
                     # print('found ', overall_family_base_root_data[i].name ,' in ', nested_fam.rootPath)
                     _extract_parent_families(
                         overall_family_base_root_data[i], nested_fam.rootPath
                     )
 
                     _extract_child_families(
                         overall_family_base_root_data[i], nested_fam.rootPath
@@ -310,29 +309,29 @@
         overall_family_base_nested_data,
     ) = rFamBaseDataUtils.read_overall_family_data_list(
         family_base_data_report_file_path
     )
     return_value.append_message(
         "{} Read overall family base data report. {} root entries found and {} nested entries found.".format(
             t_process.stop(),
-            len(overall_family_base_root_data, len(overall_family_base_nested_data)),
+            len(overall_family_base_root_data),
+            len(overall_family_base_nested_data),
         )
     )
     t_process.start()
 
     before = len(overall_family_base_nested_data)
     # reduce workload by culling not needed nested family data
     overall_family_base_nested_data = _cull_nested_base_data_blocks(
         overall_family_base_nested_data
     )
     return_value.append_message(
         " {} culled nested family base data from : {} to: {} families.".format(
-            t_process.stop(), before
-        ),
-        len(overall_family_base_nested_data),
+            t_process.stop(), before, len(overall_family_base_nested_data)
+        )
     )
     t_process.start()
 
     # set up some multithreading
     core_count = int(os.environ["NUMBER_OF_PROCESSORS"])
     if core_count > 2:
         return_value.append_message("cores: ".format(core_count))
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_missing_families.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_missing_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # from collections import namedtuple
 
@@ -180,17 +180,18 @@
         tProcess.start()
         # get a list of unique families from the nested family data
         uniqueFamilyBaseNestedData = _get_unique_nested_families(
             overallFamilyBaseNestedData
         )
         returnValue.append_message(
             "{} Culled nested family base data from : {} to: {} families".format(
-                tProcess.stop(), len(overallFamilyBaseNestedData)
-            ),
-            len(uniqueFamilyBaseNestedData),
+                tProcess.stop(),
+                len(overallFamilyBaseNestedData),
+                len(uniqueFamilyBaseNestedData),
+            )
         )
 
         tProcess.start()
         # read over nested data and built a list of unique families ( name + category )
         uniqueDic = _build_unique_nested_family_dic(uniqueFamilyBaseNestedData)
         returnValue.append_message(
             "{} Found unique nested families [{}]".format(
@@ -270,17 +271,18 @@
             overallFamilyBaseRootData,
             overallFamilyBaseNestedData,
         ) = rFamBaseDataUtils.read_overall_family_data_list(
             familyBaseDataReportFilePath
         )
         returnValue.append_message(
             "{} Read overall family base data report. {} root entries found and {} nested entries found.".format(
-                tProcess.stop(), len(overallFamilyBaseRootData)
-            ),
-            len(overallFamilyBaseNestedData),
+                tProcess.stop(),
+                len(overallFamilyBaseRootData),
+                len(overallFamilyBaseNestedData),
+            )
         )
 
         tProcess.start()
         hostFamilies = rFamBaseDataUtils.find_all_direct_host_families(
             missingFamilies, overallFamilyBaseNestedData
         )
         # get the root families from host family data
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_processor.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_base_data_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data.ifamily_processor import IFamilyProcessor
-from duHast.Revit.Family.Data import family_base_data as rFamData
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects.ifamily_processor import IFamilyProcessor
+from duHast.Revit.Family.Data.Objects import family_base_data as rFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities import util_batch_p as uBP
 
 
 class FamilyBaseProcessor(IFamilyProcessor):
     def __init__(
         self,
         reference_file_path=None,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_base_data_reload_advanced.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,117 +31,32 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
 from duHast.Utilities.Objects.timer import Timer
 from duHast.Utilities.Objects import result as res
-from duHast.Utilities import (
-    files_get as fileGet,
-    files_io as fileIO,
-    files_tab as fileTab,
-)
-from duHast.Revit.Family.Data import family_base_data_utils as rFamBaseDataUtils
-from duHast.Revit.Family.Data import family_reload_advanced_utils as rFamReloadAdvUtils
-
-_TASK_COUNTER_FILE_PREFIX = "TaskOutput"
-
-
-def _write_reload_list_to_file(reload_families, directory_path, counter=0):
-    """
-    Writes task list file to disk. File contains single column of fully qualified file path.
-
-    :param reload_families: List of tuples representing families requiring their nested families to be re-loaded.
-    :type reload_families: [rootFamily]
-    :param directory_path: Fully qualified directory path to which the task files will be written.
-    :type directory_path: str
-    :param counter: Task file name suffix, defaults to 0
-    :type counter: int, optional
-
-    :return: True if file was written successfully, otherwise False.
-    :rtype: bool
-    """
-
-    # write out file list without header
-    header = []
-    # data to be written to file
-    overall_data = []
-    file_name = (
-        directory_path + "\\" + _TASK_COUNTER_FILE_PREFIX + str(counter) + ".txt"
-    )
-    # loop over families to get file path
-    for r in reload_families:
-        # row data
-        data = []
-        data.append(r.filePath)
-        overall_data.append(data)
-    try:
-        # write data
-        fileTab.write_report_data(file_name, header, overall_data, writeType="w")
-        return True
-    except Exception:
-        return False
-
-
-def _delete_old_task_lists(directory_path):
-    """
-    Deletes all overall task files in given directory.
-
-    :param directory_path: Fully qualified directory path containing the task files to be deleted.
-    :type directory_path: str
-    :return: True if all files got deleted successfully, otherwise False.
-    :rtype: bool
-    """
-
-    flag = True
-    # find all files in folder starting with and delete them
-    files = fileGet.get_files(directory_path, ".txt")
-    if len(files) > 0:
-        for f in files:
-            if fileIO.get_file_name_without_ext(f).startswith(
-                _TASK_COUNTER_FILE_PREFIX
-            ):
-                flag = flag & fileIO.file_delete(f)
-    return flag
-
-
-def _write_out_empty_task_list(directory_path, counter=0):
-    """
-    Writes out an empty task list in case nothing is to be reloaded.
-
-    :param directory_path: Fully qualified directory path to which the task files will be written.
-    :type directory_path: str
-    :param counter: Task file name suffix, defaults to 0
-    :type counter: int, optional
 
-    :return: True if file was written successfully, otherwise False.
-    :rtype: bool
-    """
+from duHast.Revit.Family.Data import family_base_data_utils as rFamBaseDataUtils
 
-    file_name = directory_path + "\\" + "TaskOutput" + str(counter) + ".txt"
-    # write out file list without header
-    header = []
-    # write out empty data
-    overall_data = []
-    try:
-        # write data
-        fileTab.write_report_data(file_name, header, overall_data, writeType="w")
-        return True
-    except Exception:
-        return False
+from duHast.Revit.Family.Data.family_reload_advanced_utils import (
+    read_change_list,
+    write_out_empty_task_list,
+    write_reload_list_to_file,
+)
 
 
 def _remove_duplicates(list_one, list_two):
     """
     Removes any item from list one which is present in list two.
 
     :param list_one: List of tuples containing root family data.
@@ -208,119 +123,114 @@
     """
 
     # set up a timer
     t_process = Timer()
     t_process.start()
 
     return_value = res.Result()
-    change_list = rFamReloadAdvUtils.read_change_list(change_list_file_path)
+    change_list = read_change_list(change_list_file_path)
     return_value.append_message(
-        t_process.stop()
-        + " Change list of length ["
-        + str(len(change_list))
-        + "] loaded."
+        "{} Change list of length [{}] loaded.".format(
+            t_process.stop(), len(change_list)
+        )
     )
 
     t_process.start()
     # read overall family base data from file
     (
         overall_family_base_root_data,
         overall_family_base_nested_data,
     ) = rFamBaseDataUtils.read_overall_family_data_list(
         family_base_data_report_file_path
     )
     return_value.append_message(
-        t_process.stop()
-        + " Nested base data list of length ["
-        + str(len(overall_family_base_nested_data))
-        + "] loaded."
+        "{} Nested base data list of length [{}] loaded.".format(
+            t_process.stop(), len(overall_family_base_nested_data)
+        )
     )
 
     if len(change_list) > 0:
         # list containing the hosts of the host families
         task_next_level = []
         # safety switch in case of infinite loop
         task_list_counter = 0
 
         t_process.start()
         task_current_level = _get_hosts(
             change_list, overall_family_base_nested_data, overall_family_base_root_data
         )
         return_value.append_message(
-            t_process.stop()
-            + " Direct hosts ["
-            + str(len(task_current_level))
-            + "] found."
+            "{} Direct hosts [{}] found.".format(
+                t_process.stop(), len(task_current_level)
+            )
         )
 
         t_process.start()
         task_next_level = _get_hosts(
             task_current_level,
             overall_family_base_nested_data,
             overall_family_base_root_data,
         )
         return_value.append_message(
-            t_process.stop()
-            + " Next level hosts ["
-            + str(len(task_next_level))
-            + "] found."
+            "{} Next level hosts [{}] found.".format(
+                t_process.stop(), len(task_next_level)
+            )
         )
 
         # loop until no more entries in current level tasks
         while len(task_current_level) > 0:
 
             # remove next level hosts from direct hosts list to avoid overlap in reload process
             cleaned_current_tasks, over_lap_tasks = _remove_duplicates(
                 task_current_level, task_next_level
             )
 
             # write out cleaned up list:
             if len(cleaned_current_tasks) > 0:
                 t_process.start()
-                result_write_to_disk = _write_reload_list_to_file(
+                result_write_to_disk = write_reload_list_to_file(
                     cleaned_current_tasks,
                     load_lists_output_directory_path,
                     task_list_counter,
                 )
                 return_value.update_sep(
                     result_write_to_disk,
-                    t_process.stop()
-                    + " Wrote task list to file with status: "
-                    + str(result_write_to_disk),
+                    "{} Wrote task list to file with status: {}".format(
+                        t_process.stop(), result_write_to_disk
+                    ),
                 )
             else:
                 # write out an empty task list!
-                empty_task_list_flag = _write_out_empty_task_list(
+                empty_task_list_flag = write_out_empty_task_list(
                     load_lists_output_directory_path, task_list_counter
                 )
                 return_value.update_sep(
                     empty_task_list_flag,
-                    "Wrote empty task list at counter [" + str(task_list_counter),
+                    "Wrote empty task list at counter [{}]".format(task_list_counter),
                 )
 
             # swap lists to get to next level of loading
             task_current_level = list(task_next_level)
             return_value.append_message(
-                "Swapping next level hosts to direct hosts ["
-                + str(len(task_current_level))
-                + "]"
+                "Swapping next level hosts to direct hosts [{}]".format(
+                    len(task_current_level)
+                )
             )
 
             t_process.start()
             # get next level host families (task)
             task_next_level = _get_hosts(
                 task_current_level,
                 overall_family_base_nested_data,
                 overall_family_base_root_data,
             )
             return_value.append_message(
-                t_process.stop()
-                + " Next level hosts ["
-                + str(len(task_next_level))
-                + "] found."
+                "{} Next level hosts [{}]".format(
+                    t_process.stop(), len(task_next_level)
+                )
             )
 
             # increase task list counter to be used in file name
             task_list_counter = task_list_counter + 1
             if task_list_counter > 20:
                 # trigger fail save
                 return_value.update_sep(
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_base_data_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_report_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Family Base data utility module containing functions to read the data from file.
+Family report data utility module containing functions to read the data from file.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Reads family base data into two list of named tuples.
 
-root_family:
+rootFamily:
 
 - name 
 - category 
 - filePath 
-- parent 
-- child
 
-nested_family:
+
+nestedFamily:
 
 - name 
 - category 
 - filePath 
 - rootPath  [str]
 - categoryPath [str]
 
@@ -35,401 +34,344 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 
 from collections import namedtuple
 
-from duHast.Utilities import (
-    files_csv as fileCSV,
-    files_get as fileGet,
-    files_io as fileIO,
-    utility as util,
+from duHast.Utilities.Objects import result as res
+from duHast.Utilities import files_csv as fileCSV, files_io as fileIO
+from duHast.Revit.Family.Data.family_base_data_utils import (
+    read_overall_family_data_list,
 )
 
 # tuples containing base family data read from file
-root_family = namedtuple("root_family", "name category filePath parent child")
-nested_family = namedtuple(
-    "nested_family", "name category filePath rootPath categoryPath hostFamily"
+rootFamily = namedtuple("rootFamily", "name category filePath")
+nestedFamily = namedtuple(
+    "nestedFamily", "name category filePath rootPath categoryPath"
 )
 
-# row structure of family base data file
-BASE_DATA_LIST_INDEX_FAMILY_NAME = 2
-BASE_DATA_LIST_INDEX_FAMILY_FILE_PATH = 3
-BASE_DATA_LIST_INDEX_CATEGORY = 4
+# row structure of report data file
 BASE_DATA_LIST_INDEX_ROOT_PATH = 0
 BASE_DATA_LIST_INDEX_ROOT_CATEGORY_PATH = 1
-
-# file name identifiers for family base data
-FAMILY_BASE_DATA_FILE_NAME_PREFIX = "FamilyBase"
-FAMILY_BASE_DATA_FILE_EXTENSION = ".csv"
+BASE_DATA_LIST_INDEX_FAMILY_NAME = 2
+BASE_DATA_LIST_INDEX_FAMILY_FILE_PATH = 3
 
 # exceptions
-EXCEPTION_NO_FAMILY_BASE_DATA_FILES = "Families base data list files do not exist."
-EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES = "Empty Families base data list file!"
+EXCEPTION_NO_FAMILY_BASE_DATA_FILES = "Report data list files do not exist."
+EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES = "Empty report data list file!"
 
+# ------------------------------------- combining reports --------------------------------------------
 
-def _get_base_data_file_name(directory_path):
-    """
-    Gets the first family base data file in provided directory or any of it's sub directories.
-
-    :param directory_path: Fully qualified directory path.
-    :type directory_path: str
-    :raises Exception: EXCEPTION_NO_FAMILY_BASE_DATA_FILES
 
-    :return: Fully qualified file path to family base data file.
-    :rtype: str
+def _get_data_rows_from_dictionary(dic):
     """
+    Builds list of data rows from dictionary past in
 
-    # get all base data files in folder
-    files = fileGet.get_files_from_directory_walker_with_filters(
-        directory_path,
-        FAMILY_BASE_DATA_FILE_NAME_PREFIX,
-        "",
-        FAMILY_BASE_DATA_FILE_EXTENSION,
-    )
-    if len(files) > 0:
-        return files[0]
-    else:
-        raise Exception(EXCEPTION_NO_FAMILY_BASE_DATA_FILES)
-
-
-def read_overall_family_data_list(file_path):
-    """
-    Reads list of families from family base data report file into named tuples.
+    :param dic: Dictionary where key is a tuple and values is a list of list of strings
+    :type dic: {named tuple: [[str]]}
+    :param dataList: List of list of strings
+    :type dataList: [[str]]
 
-    :param file_path: Fully qualified file path to family base data report file.
-    :type file_path: str
-    :raises Exception: "Families base data list files does not exist."
-    :raises Exception: "Empty Families base data list file!"
-    :return: Two lists: first list of named tuples contain family root data, second list contains family nested data.
-    :rtype: [root_family], [nested_family]
+    :return: List of list of strings
+    :rtype: [[str]]
     """
+    print(dic)
+    dataList = []
+    # get rows from dictionary
+    for k, v in dic.items():
+        # get data rows for root family
+        for rootData in v[0]:
+            dataList.append(rootData.report_data)
+        # get data rows for any nested families
+        for nestedFamRowValue in v[1]:
+            dataList.append(nestedFamRowValue.report_data)
+    return dataList
 
-    rows = []
-    if fileIO.file_exist(file_path):
-        rows = fileCSV.read_csv_file(file_path)
-    else:
-        raise Exception(EXCEPTION_NO_FAMILY_BASE_DATA_FILES)
-    if len(rows) > 0:
-        pass
-    else:
-        raise Exception(EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES)
 
-    return_value_root_family = []
-    return_value_nested_family = []
-    for i in range(1, len(rows)):
-        # check if root family
-        if "::" not in rows[i][BASE_DATA_LIST_INDEX_ROOT_PATH]:
-            data = root_family(
-                rows[i][BASE_DATA_LIST_INDEX_FAMILY_NAME],
-                rows[i][BASE_DATA_LIST_INDEX_CATEGORY],
-                rows[i][BASE_DATA_LIST_INDEX_FAMILY_FILE_PATH],
-                [],  # set up an empty list for parent families
-                [],  # set up an empty list for child families
-            )
-            return_value_root_family.append(data)
-        else:
-            # found a child family
-            data = nested_family(
-                rows[i][BASE_DATA_LIST_INDEX_FAMILY_NAME],
-                rows[i][BASE_DATA_LIST_INDEX_CATEGORY],
-                rows[i][BASE_DATA_LIST_INDEX_FAMILY_FILE_PATH],
-                rows[i][BASE_DATA_LIST_INDEX_ROOT_PATH].split(
-                    " :: "
-                ),  # split root path into list for ease of searching
-                rows[i][BASE_DATA_LIST_INDEX_ROOT_CATEGORY_PATH].split(
-                    " :: "
-                ),  # split category path into list for ease of searching
-                [],
-            )
-            return_value_nested_family.append(data)
-    return return_value_root_family, return_value_nested_family
-
-
-def read_overall_family_data_list_from_directory(directory_path):
-    """
-    Reads the first family base data file it finds in a folder.
-    Note: This method calls ReadOverallFamilyDataList(filePath) which will raise exceptions if files are empty or dont exist in specified folder.
-
-    :param directory_path: A fully qualified directory path containing family base data file(s)
-    :type directory_path: _str
-
-    :return: Two lists: first list of named tuples contain family root data, second list contains family nested data.
-    :rtype: [root_family], [nested_family]
+def _compare_family_dictionaries(previous_aggregated_data, new_aggregated_data):
     """
+    Compares two aggregate data dictionaries. Any new root family from newAgData ( root family occurring in newAgData only) will be add to the previousAgData dictionary.
+    Any existing root family (root family occurring in previous and new aggregate data dictionaries) will be updated in the previousAgData dictionary with row data from the newAgData data dictionary.
 
-    file_name = _get_base_data_file_name(directory_path)
-    return read_overall_family_data_list(file_name)
 
+    :param previous_aggregated_data: A dictionary containing aggregated family data from the previous report.
+    :type previous_aggregated_data: {key:str, value ([str],[str])}
+    :param new_aggregated_data: A dictionary containing aggregated family data from the new report.
+    :type new_aggregated_data: {key:str, value ([str],[str])}
+    :return:
 
-def read_overall_family_data_list_into_nested(file_path):
-    """
-    Reads list of families from family base data report file into named tuples.
+        If previous_aggregated_data is empty and new_aggregated_data contains data, new_aggregated_data will be returned unchanged.
+        If new_aggregated_data is empty and previous_aggregated_data contains data, previous_aggregated_data will be returned unchanged.
+        if both dictionary are empty an empty dictionary will be returned.
 
-    :param file_path: Fully qualified file path to family base data report file.
-    :type file_path: str
-    :raises Exception: "Families base data list files does not exist."
-    :raises Exception: "Empty Families base data list file!"
-    :return: A list contains family nested data.
-    :rtype: [nested_family]
+    :rtype: {key:str, value ([str],[str])}
     """
 
-    rows = []
-    if fileIO.file_exist(file_path):
-        rows = fileCSV.read_csv_file(file_path)
-    else:
-        raise Exception(EXCEPTION_NO_FAMILY_BASE_DATA_FILES)
-    if len(rows) > 0:
-        pass
-    else:
-        raise Exception(EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES)
-
-    return_value_nested_family = []
-    for i in range(1, len(rows)):
-        # found a child family
-        data = nested_family(
-            rows[i][BASE_DATA_LIST_INDEX_FAMILY_NAME],
-            rows[i][BASE_DATA_LIST_INDEX_CATEGORY],
-            rows[i][BASE_DATA_LIST_INDEX_FAMILY_FILE_PATH],
-            rows[i][BASE_DATA_LIST_INDEX_ROOT_PATH].split(
-                " :: "
-            ),  # split root path into list for ease of searching
-            rows[i][BASE_DATA_LIST_INDEX_ROOT_CATEGORY_PATH].split(
-                " :: "
-            ),  # split category path into list for ease of searching
-            [],
+    return_value = res.Result()
+    # check corner cases:
+    if len(new_aggregated_data) == 0 and len(previous_aggregated_data) > 0:
+        # new is empty, but previous has data
+        return_value.update_sep(
+            True, "New report data is empty, using previous report data only"
+        )
+        return_value.result.append(previous_aggregated_data)
+    elif len(new_aggregated_data) > 0 and len(previous_aggregated_data) == 0:
+        # new has data, but previous is empty
+        return_value.update_sep(
+            True, "Previous report data is empty, using new report data only"
         )
-        return_value_nested_family.append(data)
-    return return_value_nested_family
+        return_value.result.append(new_aggregated_data)
+    elif len(new_aggregated_data) == 0 and len(previous_aggregated_data) == 0:
+        # new is empty, previous is empty
+        return_value.update_sep(
+            True, "Previous report data and new report data are empty!"
+        )
+        return_value.result.append({})
+    else:
+        # other and current have data
+        for family_path, family_data in new_aggregated_data.items():
+            if family_path in previous_aggregated_data:
+                return_value.append_message(
+                    "Substituting family data: {}".format(family_path)
+                )
+            else:
+                return_value.append_message("Adding new family data: {}".format(family_path))
+            previous_aggregated_data[family_path] = new_aggregated_data[family_path]
+        return_value.result.append(previous_aggregated_data)
+    return return_value
 
 
-def read_overall_family_data_list_into_nested_from_directory(directory_path):
+def _get_nested_families_belonging_to_root_families(root_family, nested_families):
     """
-    Reads the first family base data file it finds in a folder.
-    Note: This method calls ReadOverallFamilyIntoNestedDataList(filePath) which will raise exceptions if files are empty or dont exist in specified folder.
+    Returns a list of all row data of nested families belonging to a given root family.
 
-    :param directory_path: A fully qualified directory path containing family base data file(s)
-    :type directory_path: _str
+    :param rootFam: A tuple of a root family from a report.
+    :type rootFam: tuple of type 'rootFamily'
+    :param nestedFamilies: A list of tuples of all nested families in a report
+    :type nestedFamilies: [tuple of type 'nestedFamily']
 
-    :return: A list contains family nested data.
-    :rtype: [nested_family]
+    :return: 
+    :rtype: _type_
     """
 
-    file_name = _get_base_data_file_name(directory_path)
-    return read_overall_family_data_list_into_nested(file_name)
-
-
-# -------------------------------- simplify data set ----------------------------------------------------------------
-
+    nested_families_belonging_to_root_families = []
+    for nested_family in nested_families:
+        if (
+            root_family.name == nested_family.rootPath[0]
+            and root_family.category == nested_family.categoryPath[0]
+        ):
+            nested_families_belonging_to_root_families.append(nested_families[nested_family][0])
+            print("nested family in list", nested_families[nested_family][0])
+        else:
+            print("root family name: [{}] root family category: [{}] nested family root path: [{}] nested family category path: [{}]".format(root_family.name, root_family.category, nested_family.rootPath[0], nested_family.categoryPath[0]))
+    return nested_families_belonging_to_root_families
 
-def _check_data_blocks_for_overlap(block_one, block_two):
-    """
-    Checks whether the root path of families in the first block overlaps with the root path of any family in the second block.
-    Overlap is checked from the start of the root path. Any families from block one which are not overlapping any family in\
-        block two are returned.
 
-    :param block_one: List of family tuples of type nested_family
-    :type block_one: [nested_family]
-    :param block_two: List of family tuples of type nested_family
-    :type block_two: [nested_family]
-    
-    :return: List of family tuples of type nested_family
-    :rtype: [nested_family]
+def _aggregate_family_data(root_families, nested_families):
     """
+    Returns a dictionary where key are all the root family file path from a report and value is a tuple of two list of strings containing
+    the row data read from report file for the root family itself (first list) and the row data read from report file for any nested families (second list).
 
-    unique_tree_nodes = []
-    for fam in block_one:
-        match = False
-        for fam_up in block_two:
-            if " :: ".join(fam_up.rootPath).startswith(" :: ".join(fam.rootPath)):
-                match = True
-                break
-        if match == False:
-            unique_tree_nodes.append(fam)
-    return unique_tree_nodes
-
+    :param rootFamilies: A list containing tuples of all root families in a report.
+    :type rootFamilies: [tuple of type 'rootFamily']
+    :param nestedFamilies: A list of tuples of all nested families in a report
+    :type nestedFamilies: [tuple of type 'nestedFamily']
 
-def _cull_data_block(family_base_nested_data_block):
+    :return: Returns a dictionary where key is the root family file path and value is a tuple of root family at index zero and nested families at index 1
+    :rtype: {key:str, value (root family,[nested families])}
     """
-    Sorts family data blocks into a dictionary where key, from 1 onwards, is the level of nesting indicated by number of '::' in root path string.
 
-    After sorting it compares adjacent blocks in the dictionary (key and key + 1) for overlaps in the root path string. Only unique families will be returned.
+    # key is root family, value is tuple of csv row representing the root family data and list of rows each representing a nested family data
+    aggregated_family_data = {}
+    for root_family in root_families:
+        nested_families_of_root_family_row_data = (
+            _get_nested_families_belonging_to_root_families(root_family, nested_families)
+        )
+        # key is the unique family file path of the root family
+        # value is a tuple of two lists : root  at index 0, nested fam at index 1
+        aggregated_family_data[root_family.filePath] = (
+            root_family,
+            nested_families_of_root_family_row_data,
+        )
+    return aggregated_family_data
 
-    :param family_base_nested_data_block: A list containing all nested families belonging to a single root host family.
-    :type family_base_nested_data_block: [nested_family]
 
-    :return: A list of unique families in terms of root path.
-    :rtype: [nested_family]
+def _check_families_still_exist(family_data):
     """
+    Checks whether families still exist on file server.
 
-    culled_family_base_nested_data_blocks = []
-    data_blocks_by_length = {}
-    # build dic by root path length
-    # start at 1 because for nesting level ( 1 based rather then 0 based )
-    for family in family_base_nested_data_block:
-        if len(family.rootPath) - 1 in data_blocks_by_length:
-            data_blocks_by_length[len(family.rootPath) - 1].append(family)
-        else:
-            data_blocks_by_length[len(family.rootPath) - 1] = [family]
+    Reason why families no longer exist:
 
-    # loop over dictionary and check block entries against next entry up blocks
-    for i in range(1, len(data_blocks_by_length) + 1):
-        # last block get automatically added
-        if i == len(data_blocks_by_length):
-            culled_family_base_nested_data_blocks = (
-                culled_family_base_nested_data_blocks + data_blocks_by_length[i]
-            )
-        else:
-            # check for matches in next one up
-            unique_nodes = _check_data_blocks_for_overlap(
-                data_blocks_by_length[i], data_blocks_by_length[i + 1]
-            )
-            # only add non overlapping blocks
-            culled_family_base_nested_data_blocks = (
-                culled_family_base_nested_data_blocks + unique_nodes
-            )
-    return culled_family_base_nested_data_blocks
-
-
-def cull_nested_base_data_blocks(overall_family_base_nested_data):
-    """
-    Reduce base data families for parent / child finding purposes. Keep the nodes with the root path longes branch only.
-
-    Sample:
-
-    famA :: famB :: famC
-    famA :: famB
-
-    The second of the above examples can be culled since the first contains the same information.
-
-    :param overall_family_base_nested_data: _description_
-    :type overall_family_base_nested_data: _type_
-    """
-
-    current_root_fam_name = ""
-    family_blocks = []
-    block = []
-    # read families into blocks
-    for nested in overall_family_base_nested_data:
-        if nested.rootPath[0] != current_root_fam_name:
-            # read family block
-            if len(block) > 0:
-                family_blocks.append(block)
-                # reset block
-                block = []
-                block.append(nested)
-                current_root_fam_name = nested.rootPath[0]
-            else:
-                block.append(nested)
-                current_root_fam_name = nested.rootPath[0]
-        else:
-            block.append(nested)
+    - family got deleted or moved
+    - family got renamed
 
-    retained_family_base_nested_data = []
-    # cull data per block
-    for family_block in family_blocks:
-        d = _cull_data_block(family_block)
-        retained_family_base_nested_data = retained_family_base_nested_data + d
+    :param famData: A dictionary containing aggregated family data from the a report.
+    :type famData: {key:str, value ([str],[str])}
 
-    return retained_family_base_nested_data
+    :return:
+        Result class instance.
 
+        - .status True if successfully removed any outdated family data or None needed removing. Otherwise False.
+        - .message will contain list of families removed or message nothing needed to be removed.
+        - . result will contain past in dictionary at index 0
 
-# --------------------------------------------  find families in nesting tree data ------------------------------------
+        On exception:
 
-
-def find_direct_host_families(nested_fam, overall_family_base_nested_data):
+        - result.status (bool) will be False.
+        - result.message will contain generic exception message.
+        - result.result will be empty
+    :rtype: :class:`.Result`
     """
-    Finds the direct hosts of the past in family in the base nested family data set.
-
-    :param nested_fam: A tuple containing nested family data.
-    :type nested_fam: nested_family
-    :param overall_family_base_nested_data: List of tuples containing nested family data.
-    :type overall_family_base_nested_data: [nested_family]
 
-    :return: A dictionary where:
-
-        - key is the family name and category concatenated and
-        - value is a tuple in format 0: family name, 1: family category
-
-    :rtype: {str: (str,str)}
-    """
+    return_value = res.Result()
+    try:
+        remove_keys = []
+        # get keys from dic as a list
+        # check which ones do not exist anymore
+        for file_path in family_data.keys():
+            if fileIO.file_exist(file_path) == False:
+                remove_keys.append(file_path)
 
-    host_families = {}
-    # check each base family data whether it contains the missing family in its nesting tree
-    for base_nested_fam in overall_family_base_nested_data:
-        if nested_fam.name in base_nested_fam.rootPath:
-            index_match = util.index_of(base_nested_fam.rootPath, nested_fam.name)
-            # make sure we have a match and it is not the first entry in list (does not have a parent...)
-            if index_match > 0:
-                # confirm category is the same
-                if base_nested_fam.categoryPath[index_match] == nested_fam.category:
-                    # got a direct parent! (index - 1)
-                    key_new = (
-                        base_nested_fam.rootPath[index_match - 1]
-                        + base_nested_fam.categoryPath[index_match - 1]
+        # check if any family requires to be removed from the data set
+        if len(remove_keys) > 0:
+            # remove those keys from dictionary
+            for key in remove_keys:
+                remove_single_key = family_data.pop(key, None)
+                if remove_single_key != None:
+                    return_value.append_message(
+                        "Removed family from data: {}".format(key)
                     )
-                    if key_new not in host_families:
-                        host_families[key_new] = (
-                            base_nested_fam.rootPath[index_match - 1],
-                            base_nested_fam.categoryPath[index_match - 1],
-                        )
-    return host_families
+                else:
+                    return_value.append_message(
+                        "Failed to removed family from data: {}".format(key)
+                    )
+        else:
+            return_value.append_message("No family required removing from data.")
+
+        # update return data
+        return_value.update_sep(True, "Successfully updated family data.")
+        return_value.result.append(family_data)
+
+    except Exception as e:
+        return_value.update_sep(
+            False,
+            "Failed to check whether families still exist with exception: {}".format(e),
+        )
+    return return_value
 
 
-def find_all_direct_host_families(families, overall_family_base_nested_data):
+def combine_reports(previous_report_path, new_report_path):
     """
-    Returns a dictionary of all direct host families of families past in.
+    This combines two reports by:
 
-    :param families: A list of tuples containing nested family data.
-    :type families: [nested_family]
-    :param overall_family_base_nested_data: List of tuples containing nested family data.
-    :type overall_family_base_nested_data: [nested_family]
+    - building an aggregate data dictionary of each report (key root family file path, values lists containing the row data read from file for the root family as well as any nested families)
+    - comparing the previous report dictionary with the new report dictionary and
+        - adding any new families found in the new report dictionary
+        - updating any previous report families found with data matching the root family in the new report dictionary
 
-    :return: A dictionary.
-    :rtype: {str: (str,str)}
-    """
+    All reports start with the following 2 columns:
+    root	rootCategory
 
-    host_families = {}
-    for fam in families:
-        hosts = find_direct_host_families(fam, overall_family_base_nested_data)
-        # update dictionary with new hosts only
-        for h in hosts:
-            if h not in host_families:
-                host_families[h] = hosts[h]
-    return host_families
+    First entry (after split at separator) in each of these columns identifies root family uniquely.
+    Assume that new report only ever adds or substitutes entries in previous report but does not delete from it!
 
+    This function checks at the end whether families still exist on file server. If not, they will be removed from the data set.
 
-def find_root_families_from_hosts(host_families, overall_family_base_root_data):
-    """
-    Returns a list of tuples of type root_family matching the past in host families.
+    :param previous_report_path: A fully qualified file path to the previous report file.
+    :type previous_report_path: str
+    :param new_report_path: A fully qualified file path to the new report file.
+    :type new_report_path: str
 
-    :param host_families: A dictionary where:
+    :return: list of lists of report rows
+    :rtype: [[str]]
+    """
 
-        - key is the family name and category concatenated and
-        - value is a tuple in format 0: family name, 1: family category
+    return_value = res.Result()
+    # read families from both reports
+    # ...compare them:
+    # take all families from current report and all none matching families from the other report
 
-    :type host_families: {str: (str,str)}
-    :param overall_family_base_root_data: List of tuples containing root family data.
-    :type overall_family_base_root_data: [root_family]
+    previous_aggregated_families = {}
+    new_aggregated_families = {}
 
-    :return: List of root family tuples.
-    :rtype: [root_family]
-    """
+    print( "reading previous")
+    # previous report
+    try:
+        previous_root, previous_nested = read_overall_family_data_list(
+            previous_report_path
+        )
+        # previous_root, previous_nested = read_unique_families_with_row_data_from_report(
+        #    previous_report_path
+        # )
+        return_value.append_message(
+            "Previous report: found {} root families.".format(len(previous_root))
+        )
+        return_value.append_message(
+            "Previous report: found {} nested families.".format(len(previous_nested))
+        )
+        # build dictionary containing all family data per root family
+        previous_aggregated_families = _aggregate_family_data(
+            previous_root, previous_nested
+        )
+    except Exception as e:
+        # check whether empty file exception
+        if str(e) != EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES:
+            raise e
+        
+    print( "reading new")
+    # new report
+    try:
+        new_root, new_nested = read_overall_family_data_list(new_report_path)
+        # new_root, new_nested = read_unique_families_with_row_data_from_report(
+        #    new_report_path
+        # )
+        # build dictionary containing all family data per root family
+        new_aggregated_families = _aggregate_family_data(new_root, new_nested)
+        return_value.append_message(
+            "New report: found {} root families.".format(len(new_root)) + ""
+        )
+        return_value.append_message(
+            "New report: found {} nested families.".format(len(new_nested)) + ""
+        )
+    except Exception as e:
+        # check whether empty file exception
+        if str(e) != EXCEPTION_EMPTY_FAMILY_BASE_DATA_FILES:
+            raise e
+
+    print ("comparing")
+    # compare dictionaries: build unique list of families
+    unique_family_data_status = _compare_family_dictionaries(
+        previous_aggregated_families, new_aggregated_families
+    )
+    return_value.update(unique_family_data_status)
+    unique_family_data = unique_family_data_status.result[0]
 
-    base_host_families = []
-    for nested_id, nestedFam in host_families.items():
-        for base_root_fam in overall_family_base_root_data:
-            if (
-                nestedFam[0] == base_root_fam.name
-                and nestedFam[1] == base_root_fam.category
-            ):
-                base_host_families.append(base_root_fam)
-    return base_host_families
+    print( "checking")
+    # check whether families still exist on file server
+    remove_none_existing_families = _check_families_still_exist(unique_family_data)
+    return_value.update(remove_none_existing_families)
+    # only update family data if culling occurred without any exceptions
+    if remove_none_existing_families.status:
+        unique_family_data = remove_none_existing_families.result[0]
+
+    # get report header row (there should be a previous report file...otherwise this will write an empty header row)
+    header_row = fileCSV.get_first_row_in_csv_file(previous_report_path)
+    #header_row = header.split(",")
+    print( "building")
+    # build list of data rows
+    rows_current = _get_data_rows_from_dictionary(unique_family_data)
+    # sort rows by root ( first entry ) since other code (circ reference checker for instance) expects data sorted
+    rows_current.sort()
+    # start with header row
+    rows_current.insert(0, header_row)
+    # overwrite return result value since it is already containing data from previous operations
+    return_value.result = rows_current
+    return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_category_data_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_category_data_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_data_collector.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/family_data_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 from duHast.Utilities.Objects import result as res
 
 # import Autodesk
-import Autodesk.Revit.DB as rdb
+from Autodesk.Revit.DB import Element, FamilySymbol, FilteredElementCollector
 from duHast.Utilities.Objects import base
 
 
 class RevitFamilyDataCollector(base.Base):
     def __init__(self, data_processors):
         """
         Class constructor taking a list of processor instances as argument.
@@ -58,15 +58,15 @@
         :param doc: Current family document.
         :type doc: Autodesk.Revit.DB.Document
         :return: list of family ids
         :rtype: [Autodesk.Revit.DB.ElementId]
         """
 
         family_ids = []
-        col = rdb.FilteredElementCollector(doc).OfClass(rdb.FamilySymbol)
+        col = FilteredElementCollector(doc).OfClass(FamilySymbol)
         # get families from symbols and filter out in place families
         for fam_symbol in col:
             if (
                 fam_symbol.Family.Id not in family_ids
                 and fam_symbol.Family.IsInPlace == False
             ):
                 family_ids.append(fam_symbol.Family.Id)
@@ -91,22 +91,22 @@
         # that family is processed already
         if is_root == False:
             for pro in self.dataProcessors:
                 try:
                     pro.process(doc, root_name, root_category)
                     return_value.append_message(
                         "Processor [{}] of family: {}  [OK]".format(
-                            pro.dataType, doc.Title
+                            pro.data_type, doc.Title
                         )
                     )
                 except Exception as e:
                     return_value.update_sep(
                         False,
                         "Processor [{}] of family: {} [EXCEPTION] {}".format(
-                            pro.dataType, doc.Title, e
+                            pro.data_type, doc.Title, e
                         ),
                     )
 
         # check if family doc
         if doc.IsFamilyDocument:
             # get any nested families
             family_ids = self._get_family_ids(doc)
@@ -129,47 +129,38 @@
                                 root_name + " :: " + fam_name,
                                 root_category + " :: " + fam_category_name,
                             )
                             return_value.update(dive_result)
                     except Exception as e:
                         message = ""
                         if family != None:
-                            message = (
-                                "An exception occurred when opening family "
-                                + rdb.Element.Name.GetValue(family)
-                                + ". Exception: "
-                                + str(e)
+                            message = "An exception occurred when opening family {} . Exception: {}".format(
+                                Element.Name.GetValue(family), e
                             )
                         else:
-                            message = (
-                                "An exception occurred when attempting the get family element by id:"
-                                + str(family_id)
-                                + ". Exception: "
-                                + str(e)
+                            message = "An exception occurred when attempting the get family element by id: {}. Exception: {}".format(
+                                family_id, e
                             )
                         return_value.update_sep(False, message)
             else:
                 # only close any nested family document...not the root one
                 # since that is closed by batch processor!
                 if is_root == False:
                     try:
                         # no more families found. Close the active doc
                         doc.Close(False)
                     except Exception as e:
                         message = ""
                         if doc != None:
-                            message = (
-                                "An exception occurred when closing document: "
-                                + doc.Title
-                                + ". Exception: "
-                                + str(e)
+                            message = "An exception occurred when closing document: {} . Exception: {}".format(
+                                doc.Title, e
                             )
                         else:
-                            message = (
-                                "An exception occurred when closing document: " + str(e)
+                            message = "An exception occurred when closing document: {}".format(
+                                e
                             )
                         return_value.update_sep(False, message)
         return return_value
 
     def process_family(self, doc, root_name, root_category):
         """
         Entry point for recursive family looper.
@@ -184,68 +175,64 @@
         :param root_category: The path of the nested family category in a tree: rootFamilyCategory::nestedFamilyOneCategory::nestedFamilyTwoCategory\
             This includes the actual family category as the last node.
         :type root_category: str
 
         :return: 
             Result class instance.
             
-            - .result = True if all data processor instances ran without an exception. Otherwise False.
+            - .status True if all data processor instances ran without an exception. Otherwise False.
             - .message will contain each processor type and its processing status'
         
         :rtype: :class:`.Result`
         """
 
         return_value = res.Result()
 
         # TODO:
         # action any pre processing actions
         # loop over fam processor instances and process family with each of them
         for pro in self.dataProcessors:
             try:
-                pre_action_result = pro.preProcessActions(doc)
+                pre_action_result = pro.pre_process_actions(doc)
                 return_value.update(pre_action_result)
             except Exception as e:
                 return_value.update_sep(
                     False,
-                    "PreProcessor ["
-                    + pro.dataType
-                    + "] of family: "
-                    + str(doc.Title)
-                    + " [EXCEPTION] "
-                    + str(e),
+                    "PreProcessor [{}] of family: {} [EXCEPTION] {}".format(
+                    pro.data_type,doc.Title,e)
                 )
 
         # loop over fam processor instances and process family with each of them
         for pro in self.dataProcessors:
             try:
                 pro.process(doc, root_name, root_category)
                 return_value.append_message(
-                    "Processor [{}] of family: {} [OK]".format(pro.dataType, doc.Title)
+                    "Processor [{}] of family: {} [OK]".format(pro.data_type, doc.Title)
                 )
             except Exception as e:
                 return_value.update_sep(
                     False,
                     "Processor [{}] of family: {} [EXCEPTION] {}".format(
-                        pro.dataType, doc.Title, e
+                        pro.data_type, doc.Title, e
                     ),
                 )
 
         # check out any nested families
         dive_result = self._dive(doc, root_name, root_category, True)
         return_value.update(dive_result)
 
         # TODO:
         # action any post processing actions
         # loop over fam processor instances and process family with each of them
         for pro in self.dataProcessors:
             try:
-                pro_action_result = pro.postProcessActions(doc)
+                pro_action_result = pro.post_process_actions(doc)
                 return_value.update(pro_action_result)
             except Exception as e:
                 return_value.update_sep(
                     False,
                     "PostProcessor [{}] of family: {} [EXCEPTION] {}".format(
-                        pro.dataTyp, doc.Title, e
+                        pro.data_type, doc.Title, e
                     ),
                 )
 
         return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_reload_advanced_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
-
+import os
 from collections import namedtuple
 
 from duHast.Utilities import (
     files_csv as fileCSV,
     files_get as fileGet,
     files_io as fileIO,
     files_tab as fileTab,
@@ -65,15 +65,17 @@
     :rtype: bool
     """
 
     # write out file list without header
     header = []
     # data to be written to file
     overall_data = []
-    file_name = directory_path + "\\" + TASK_COUNTER_FILE_PREFIX + str(counter) + ".txt"
+    file_name = os.path.join(
+        directory_path, "{} {}.txt".format(TASK_COUNTER_FILE_PREFIX, counter)
+    )
     # loop over families to get file path
     for r in reload_families:
         # row data
         data = []
         data.append(r.filePath)
         overall_data.append(data)
     try:
@@ -112,15 +114,17 @@
     :type directory_path: str
     :param counter: Task file name suffix, defaults to 0
     :type counter: int, optional
     :return: True if file was written successfully, otherwise False.
     :rtype: bool
     """
 
-    file_name = directory_path + "\\" + "TaskOutput" + str(counter) + ".txt"
+    file_name = os.path.join(
+        directory_path, "{} {}.txt".format(TASK_COUNTER_FILE_PREFIX, counter)
+    )
     # write out file list without header
     header = []
     # write out empty data
     overall_data = []
     try:
         # write data
         fileTab.write_report_data(file_name, header, overall_data, writeType="w")
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_files.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     """
 
     return_value = res.Result()
     return_value.update_sep(True, "Renaming families:")
 
     for rename_directive in rename_directives:
         try:
+            return_value.append_message("rename directive: {}".format(rename_directive))
             # check if rename directive includes a file path ( might be empty if nested families only are to be renamed)
             if rename_directive.filePath != "":
                 # attempt to rename family file
                 try:
                     # build the new file name
                     new_full_name = os.path.join(
                         os.path.dirname(rename_directive.filePath),
@@ -88,15 +89,15 @@
                         return_value.append_message(
                             "{} -> {}".format(
                                 rename_directive.name, rename_directive.newName
                             )
                         )
                     else:
                         return_value.update_sep(
-                            False, "File not found: ".format(rename_directive.name)
+                            False, "File not found: {}".format(rename_directive.name)
                         )
                 except Exception as e:
                     return_value.update_sep(
                         False,
                         "Failed to rename file: {} with exception: {}".format(
                             rename_directive.name, e
                         ),
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_find_host_families.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_find_host_families.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 - loop over root families
 -   find match in identified host families
 - write out root family date: family file path, family name, category
 
 """
 
-
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -32,16 +31,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 # import clr
 # import System
@@ -133,33 +132,32 @@
         # check if input file existed and contained data
         if len(overall_family_base_root_data) > 0:
             t_process.start()
             file_rename_list_status = rFamRenameUtils.get_rename_directives(
                 input_directory_path
             )
             return_value.append_message(
-                "{} Read data from file! Rename family entries [{} ] found.".format(
+                "{} Read data from file! Rename family entries [{}] found.".format(
                     t_process.stop(), len(file_rename_list_status.result)
                 )
             )
             # check if any rename directives
             if len(file_rename_list_status.result) > 0:
                 before = len(overall_family_base_nested_data)
                 t_process.start()
                 # reduce workload by culling not needed nested family data
                 overall_family_base_nested_data = (
                     rFamBaseDataUtils.cull_nested_base_data_blocks(
-                        overall_family_base_nested_data
+                        overall_family_base_root_data, overall_family_base_nested_data
                     )
                 )
                 return_value.append_message(
                     "{} Culled nested family base data from : {} to: {} families.".format(
-                        t_process.stop(), before
-                    ),
-                    len(overall_family_base_nested_data),
+                        t_process.stop(), before, len(overall_family_base_nested_data)
+                    )
                 )
 
                 t_process.start()
                 # get a list of simplified root data families extracted from nested family path data
                 root_fam_simple = rFamBaseDataUtils.find_all_direct_host_families(
                     file_rename_list_status.result, overall_family_base_nested_data
                 )
@@ -186,10 +184,10 @@
                 )
         else:
             return_value.update_sep(
                 False, "No base family data found. Aborted operation!"
             )
     except Exception as e:
         return_value.update_sep(
-            False, "Failed to find host families with exception: ".format(e)
+            False, "Failed to find host families with exception: {}".format(e)
         )
     return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/family_rename_loaded_families.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/family_rename_loaded_families.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 from duHast.Revit.Family import family_rename_files_utils as rFamRenameUtils
 from duHast.Revit.Family import family_utils as rFamUtils
 from duHast.Revit.Common import transaction as rTran
 from duHast.Utilities.Objects import result as res
 
 # import Autodesk Revit DataBase namespace
-import Autodesk.Revit.DB as rdb
+from Autodesk.Revit.DB import Transaction
 
 
 def _rename_loaded_families(doc, rename_directives, family_ids):
     """
     Loops over nested families and if a match in rename directives is found will rename the family accordingly.
 
     :param doc: The current family document.
@@ -113,16 +113,16 @@
                                 + "] from: "
                                 + rename_directive.name
                                 + " to: "
                                 + rename_directive.newName,
                             )
                         return action_return_value
 
-                    transaction = rdb.Transaction(
-                        doc, "Renaming: " + rename_directive.name
+                    transaction = Transaction(
+                        doc, "Renaming: {}".format(rename_directive.name)
                     )
                     rename_result = rTran.in_transaction(transaction, action)
                     if rename_result.status:
                         # make sure that this returns true as soon as one family renamed successfully
                         return_value.status = True
                     # update messages
                     return_value.append_message(rename_result.message)
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_action.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_action.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_data.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_data.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Data/ifamily_processor.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Data/Objects/ifamily_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #
 #
 #
 
 import System
 import Autodesk.Revit.DB as rdb
 import json
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities.Objects import result as res
 from duHast.Utilities.Objects import base
 
 
 class IFamilyProcessor(base.Base):
     def __init__(
         self,
@@ -55,15 +55,15 @@
         self.data_type = data_type
         self.string_report_headers = string_report_headers
         self.pre_actions = pre_actions
         self.post_actions = post_actions
 
     # -------------------------------------- utility ----------------------
 
-    def _update_Data(
+    def _update_data(
         self,
         processor,
         identify_by_this_property_name,
         identify_by_this_property_value,
         update_by_property_name,
         updated_to_this_property_value,
     ):
@@ -80,15 +80,15 @@
         Finds the processor instance which processed the root family.
 
         :return: Processor instance
         :rtype: IFamilyProcessor
         """
 
         for processor in self.data:
-            for d in processor.get_Data():
+            for d in processor.get_data():
                 if " :: " not in d[IFamData.ROOT]:
                     return processor
 
     def _find_root_family_data(self):
         """
         Returns all data from root families (top most in tree) from all processor instances.
 
@@ -97,15 +97,15 @@
 
         :return: List of dictionaries.
         :rtype: [{}]
         """
 
         family_data = []
         for processor in self.data:
-            for d in processor.get_Data():
+            for d in processor.get_data():
                 if " :: " not in d[IFamData.ROOT]:
                     family_data.append(d)
         return family_data
 
     def _find_nested_families_data(self):
         """
         Returns all data from nested families from each processor instances.
@@ -115,15 +115,15 @@
 
         :return: List of dictionaries.
         :rtype: [{}]
         """
 
         nested_family_data = []
         for processor in self.data:
-            for d in processor.get_Data():
+            for d in processor.get_data():
                 if " :: " in d[IFamData.ROOT]:
                     nested_family_data.append(d)
         return nested_family_data
 
     def _fix_data_types(self, flattened_dic):
         """
         Replace any ElementId and Byte values with int or string respectively to have JSON working ok.
@@ -209,15 +209,15 @@
 
         :return: List of dictionaries.
         :rtype: [{}]
         """
 
         data_out = []
         for data in self.data:
-            for d in data.get_Data():
+            for d in data.get_data():
                 data_out.append(d)
         return data_out
 
     def get_data_json(self):
         """
         Returns data objects as JSON formatted strings.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/Utility/loadable_family_categories.py` & `DuHast-0.1.3/src/duHast/Revit/Family/Utility/loadable_family_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_element_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_element_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_load_option.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_load_option.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_parameter_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_parameter_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_reference_elements.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_reference_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,15 @@
                 doc, ref_p, rdb.BuiltInParameter.ELEM_REFERENCE_NAME, "12"
             )
             # set overall flag to indicate that at least one element was changed
             if result_change.status == True and match_at_all == False:
                 match_at_all = True
             result.update(result_change)
     if match_at_all == False:
-        result.status = False
-        result.message = "No reference planes found requiring reference type update"
+        result.update_sep(False, "No reference planes found requiring reference type update")
     return result
 
 
 def set_symbolic_and_model_lines_to_not_a_reference(doc):
     """
     This function sets any model or symbolic curve in a family with reference type 'weak' to reference type 'not a reference'.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_reload.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_reload.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_rename_files_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_rename_files_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/family_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Family/family_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Family/purge_unused_family_types.py` & `DuHast-0.1.3/src/duHast/Revit/Family/purge_unused_family_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Floors/Utility/floors_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/Utility/walls_filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,62 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit floors utility functions. 
+This module contains a Revit walls utility functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-# import Autodesk
-from Autodesk.Revit.DB import BuiltInCategory, FilteredElementCollector, FloorType
+from Autodesk.Revit.DB import (
+    BuiltInCategory,
+    FilteredElementCollector,
+    WallType,
+)
 
-
-# doc:   current model document
-def _get_all_floor_types_by_category(doc):
+def _get_all_wall_types_by_class(doc):
     """
-    Function returning a filtered element collector of all floor types in the model.
-
-    This uses builtinCategory as filter. Return types includes:
-    - Floor
-    - In place families or loaded families
-
-    It will therefore not return any foundation slab types.
-
+    This will return a filtered element collector of all wall types by class in the model
+    It will therefore not return any in place wall types since revit treats those as families...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector of floor types.
+    :return: A filtered element collector containing wall types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
-        FilteredElementCollector(doc)
-        .OfCategory(BuiltInCategory.OST_Floors)
-        .WhereElementIsElementType()
-    )
-    return collector
+    return FilteredElementCollector(doc).OfClass(WallType)
 
 
-# doc   current model document
-def _get_floor_types_by_class(doc):
+def _get_all_wall_types_by_category(doc):
     """
-    Function returning a filtered element collector of all floor types in the model.
-
-    - Floor
-    - Foundation Slab
-
-    it will therefore not return any in place family types ...
-
+    Gets all wall types in a model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector of floor types.
+    :return: A filtered element collector containing wall types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = FilteredElementCollector(doc).OfClass(FloorType)
+    collector = (
+        FilteredElementCollector(doc)
+        .OfCategory(BuiltInCategory.OST_Walls)
+        .WhereElementIsElementType()
+    )
     return collector
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Floors/Utility/floors_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit floor utility functions. 
+This module contains a Revit roofs utility functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-from duHast.Revit.Floors.Utility import floors_filter as rFloorsFilter
+# import Autodesk
+import Autodesk.Revit.DB as rdb
 
 
-def build_floor_type_dictionary(collector, dic):
+def _get_all_roof_types_by_category(doc):
     """
-    Returns the dictionary past in with keys and or values added retrieved from collector past in.
-    Keys are built in floor family type names.
-    TODO: This code repeats across a number of modules. Use generic instead!
-    :param collector: A filtered element collector containing floor types.
-    :type collector: Autodesk.Revit.DB.FilteredElementCollector
-    :param dic: A dictionary containing key: floor type family name, value: list of ids belonging to that type.
-    :type dic: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
-    :return: A dictionary containing key: built in floor type family name, value: list of ids belonging to that type.
-    :rtype: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
+    Gets a filtered element collector of all roof types in the model.
+
+    - Basic Roof
+    - In place families or loaded families
+    - sloped glazing
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+
+    :return: A filtered element collector containing roof types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    for c in collector:
-        if dic.has_key(c.FamilyName):
-            if c.Id not in dic[c.FamilyName]:
-                dic[c.FamilyName].append(c.Id)
-        else:
-            dic[c.FamilyName] = [c.Id]
-    return dic
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
+        .WhereElementIsElementType()
+    )
+    return collector
 
 
-def sort_floor_types_by_family_name(doc):
+def _get_roof_types_by_class(doc):
     """
-    Returns a dictionary containing all floor types in the model.
-    Key values are as per BUILTIN_FLOOR_TYPE_FAMILY_NAMES.
-    TODO: This code repeats across a number of modules. Use generic instead!
+    Gets a filtered element collector of all Roof types in the model:
+
+    - Basic Roof
+    - sloped glazing
+
+    Since this is based of class roof it will therefore not return any in place family types!
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A dictionary containing key: floor type family name, value: list of ids.
-    :rtype: dic { str: [Autodesk.Revit.DB.ElementId]}
+
+    :return: A filtered element collector containing roof types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    # get all floor Type Elements
-    wts = rFloorsFilter._get_floor_types_by_class(doc)
-    # get all floor types including in place floor families
-    wts_two = rFloorsFilter._get_all_floor_types_by_category(doc)
-    used_wts = {}
-    used_wts = build_floor_type_dictionary(wts, used_wts)
-    used_wts = build_floor_type_dictionary(wts_two, used_wts)
-    return used_wts
+    collector = rdb.FilteredElementCollector(doc).OfClass(rdb.RoofType)
+    return collector
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Floors/floors.py` & `DuHast-0.1.3/src/duHast/Revit/Floors/floors.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Floors/purge_unused_floor_types.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/cable_trays.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,154 +1,171 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to purging Revit floors. 
+This module contains a number of helper functions relating to Revit cable trays.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-from duHast.Revit.Family import purge_unused_family_types as rFamPurge
-from duHast.Revit.Common import purge_utils as rPurgeUtils
-from duHast.Revit.Floors import floors as rFloor
-from duHast.Revit.Floors.Utility import floors_type_sorting as rFloorTypeSort
+import Autodesk.Revit.DB as rdb
+import Autodesk.Revit.DB.Electrical as rdbE
 
+from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
+    get_symbol_ids_of_mep_system_types,
+    get_unique_ids_of_used_symbols_from_system_type_ids,
+)
+from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
+    CATS_LOADABLE_CABLE_TRAYS,
+)
+from duHast.Revit.Common import common as com
 
-def get_used_floor_type_ids(doc):
-    """
-    Returns all used in Floor type ids.
-    Filters by builtin category.
-    Used: at least one instance of this type is placed in the model.
 
+def get_all_cable_tray_types_by_category(doc):
+    """
+    Gets a filtered element collector of all cable tray types in the model.
+    - with fittings
+    - without fittings
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids representing not used floor types.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: A filtered element collector of cable tray types
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(
-        doc, rFloor.get_all_floor_type_ids_in_model_by_category, 1
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_CableTray)
+        .WhereElementIsElementType()
     )
-    return ids
+    return collector
 
 
-def family_no_types_in_use(fam_type_ids, un_used_type_ids):
+def get_cable_tray_types_by_class(doc):
     """
-    Compares two lists of ids. True if any id is not in un_used_type_ids.
-    TODO: check for more generic list comparison and remove this function.
-
-    :param fam_type_ids: List of family type ids to check.
-    :type fam_type_ids: List of Autodesk.Revit.DB.ElementId
-    :param un_used_type_ids: Reference list of ids.
-    :type un_used_type_ids: List of Autodesk.Revit.DB.ElementId
-    :return: True if any id from fam_type_ids is not in un_used_type_ids.
-    :rtype: bool
+    Gets a filtered element collector of all cable tray types in the model.
+    - with fittings
+    - without fittings
+    Will exclude in place families.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: A filtered element collector of cable tray types
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    match = True
-    for fam_type_id in fam_type_ids:
-        if fam_type_id not in un_used_type_ids:
-            match = False
-            break
-    return match
+    return rdb.FilteredElementCollector(doc).OfClass(rdbE.CableTrayType)
 
 
-def get_unused_non_in_place_floor_type_ids_to_purge(doc):
+def get_all_cable_tray_instances_by_category(doc):
     """
-    Gets all unused floor type id's.
-    This method can be used to safely delete unused wall types:
-    In the case that no wall instance using any of the types is placed this will return all but one type id since\
-        Revit requires at least one wall type definition to be in the model.
-    Filters by class:
-    - Floor
-    - foundation slab
-    It will therefore not return any in place family types.
-
+    Gets all cable tray elements placed in model.
+    TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids representing not used floor types.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: A filtered element collector of cable tray instances
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    # get unused type ids
-    ids = rPurgeUtils.get_used_unused_type_ids(
-        doc, rFloor.get_all_floor_type_ids_in_model_by_class, 0
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_CableTray)
+        .WhereElementIsNotElementType()
     )
-    # make sure there is at least on Floor type per system family left in model
-    floor_types = rFloorTypeSort.sort_floor_types_by_family_name(doc)
-    for key, value in floor_types.items():
-        if key in rFloor.BUILTIN_FLOOR_TYPE_FAMILY_NAMES:
-            if family_no_types_in_use(value, ids) == True:
-                # remove one type of this system family from unused list
-                ids.remove(value[0])
-    return ids
+    return collector
 
 
-def get_used_in_place_floor_type_ids(doc):
+def get_all_cable_tray_instances_by_class(doc):
     """
-    Gets all used in place family symbol (type) ids.
-    Used: at least one instance of this type is placed in the model.
-
+    Gets all cable tray elements placed in model.
+    Will exclude in place families.
+    TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids representing in place floor symbols (types).
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: A filtered element collector of cable tray instances
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(
-        doc, rFloor.get_all_in_place_floor_type_ids_in_model, 1
+    return (
+        rdb.FilteredElementCollector(doc)
+        .OfClass(rdbE.CableTrayType)
+        .WhereElementIsNotElementType()
     )
-    return ids
 
 
-def get_unused_in_place_floor_type_ids(doc):
+def get_all_cable_tray_type_ids_in_model_by_category(doc):
     """
-    Gets all used in place family symbol (type) ids.
-    Unused: Not one instance of this type is placed in the model.
+    Gets all cable tray type ids available in model.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: A list of ids representing cable tray types.
+    :rtype: List Autodesk.Revit.DB.ElementId
+    """
+
+    ids = []
+    col_cat = get_all_cable_tray_types_by_category(doc)
+    ids = com.get_ids_from_element_collector(col_cat)
+    return ids
+
 
+def get_all_cable_tray_type_ids_in_model_by_class(doc):
+    """
+    Gets all cable tray type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids representing in place floor symbols (types).
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: A list of ids representing cable tray types.
+    :rtype: List Autodesk.Revit.DB.ElementId
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(
-        doc, rFloor.get_all_in_place_floor_type_ids_in_model, 0
-    )
+    ids = []
+    col_class = get_cable_tray_types_by_class(doc)
+    ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-def get_unused_in_place_floor_ids_for_purge(doc):
+def get_symbol_ids_used_in_cable_tray_types(doc):
     """
-    Gets symbol(type) ids and family ids (when no type is in use) of in place floor families which can be safely deleted from the model.
-    This method can be used to safely delete unused in place floor types. There is no requirement by Revit to have at least one\
-        in place wall definition in the model.
+    Gets a list of unique symbol ids used in system type properties of cable tray types.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: List of unique ids representing family symbols used in cable tray systems.
+    :rtype: list  Autodesk.Revit.DB.ElementId
+    """
+
+    ids = []
+    tye_ids = get_all_cable_tray_type_ids_in_model_by_category(doc)
+    ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
+    return ids
+
 
+def get_symbol_ids_for_cable_tray_types_in_model(doc):
+    """
+    Gets list of symbol ids of the following categories:
+    - BuiltInCategory.OST_CableTrayFitting
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids representing unused in place floor types and families.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: List of ids representing family symbols.
+    :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
-    ids = rFamPurge.get_unused_in_place_ids_for_purge(
-        doc, get_unused_in_place_floor_type_ids
+    ids = get_symbol_ids_of_mep_system_types(
+        doc, CATS_LOADABLE_CABLE_TRAYS, "GetSymbolIdsForCableTrayTypes"
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/grid_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/grid_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/Reporting/grids_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/Reporting/grids_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/grids.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/grids.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/grids_appearance.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/grids_appearance.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/grids_worksets.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/grids_worksets.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Grids/purge_unused_grid_types.py` & `DuHast-0.1.3/src/duHast/Revit/Grids/purge_unused_grid_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/levels_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/levels_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Levels/Reporting/levels_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Levels/Reporting/levels_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Levels/levels.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/ducts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Revit levels helper functions.
+This module contains a number of helper functions relating to Revit ducts.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -21,157 +21,157 @@
 #
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
+#
 
-import clr
-import System
-
-
-clr.AddReference("System.Core")
-from System import Linq
-
-clr.ImportExtensions(Linq)
+import Autodesk.Revit.DB as rdb
+import Autodesk.Revit.DB.Mechanical as rdbM
 
-# import common library modules
+from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
+    get_symbol_ids_of_mep_system_types,
+    get_unique_ids_of_used_symbols_from_system_type_ids,
+)
+from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
+    CATS_LOADABLE_DUCTS,
+)
 from duHast.Revit.Common import common as com
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
-
 
-def get_levels_in_model(doc):
+def get_all_duct_types_by_category(doc):
     """
-    Get all levels in model
-
-    :param doc: The current model document.
+    Gets a filtered element collector of all duct types in the model.
+    - round
+    - oval
+    - rectangular
+    :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A collector with all levels in model.
+    :return: A filtered element collector of duct types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = rdb.FilteredElementCollector(doc).OfClass(rdb.Level)
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_DuctCurves)
+        .WhereElementIsElementType()
+    )
     return collector
 
 
-# --------------------------------------------- utility functions ------------------
-
-
-def get_levels_list_ascending(doc):
+def get_all_duct_types_by_class(doc):
     """
-    Gets a filtered element collector of all levels in the model ascending by project elevation.
+    Gets a filtered element collector of all duct types in the model.
+    - round
+    - oval
+    - rectangular
+    Will exclude in place families.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: A filtered element collector of duct types
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    """
+
+    return rdb.FilteredElementCollector(doc).OfClass(rdbM.DuctType)
 
-    Filters by category.
 
+def get_all_duct_instances_in_model_by_category(doc):
+    """
+    Gets all duct elements placed in model.
+    TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of levels
+    :return: A filtered element collector of duct instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
+    return (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Levels)
+        .OfCategory(rdb.BuiltInCategory.OST_DuctCurves)
         .WhereElementIsNotElementType()
-        .ToList()
-        .OrderBy(lambda l: l.ProjectElevation)
     )
-    return collector
-
 
-def get_level_elevation_by_name(doc, level_name):
-    level_elevation = None
-    levels = get_levels_in_model(doc=doc)
-    for level in levels:
-        if(level.Name == level_name):
-            return level.Elevation
-    return level_elevation
 
-# ------------------------------------------------- filters --------------------------------------------------------------------
-
-
-def get_all_level_heads_by_category(doc):
+def get_all_duct_instances_in_model_by_class(doc):
     """
-    Gets a filtered element collector of all level head types in the model.
-
-    Filters by category.
-
+    Gets all duct elements placed in model.
+    Will exclude in place families.
+    TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector of level heads
+    :return: A filtered element collector of duct instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
+    return (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_LevelHeads)
-        .WhereElementIsElementType()
+        .OfClass(rdbM.DuctType)
+        .WhereElementIsNotElementType()
     )
-    return collector
 
 
-def get_all_level_types_by_category(doc):
+def get_all_duct_type_ids_in_model_by_category(doc):
     """
-    Gets a filtered element collector of all level types in the model.
-
-    Filters by category.
-
+    Gets all duct type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector of level types.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: A list of ids representing duct types.
+    :rtype: List Autodesk.Revit.DB.ElementId
     """
 
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Levels)
-        .WhereElementIsElementType()
-    )
-    return collector
+    ids = []
+    col_cat = get_all_duct_types_by_category(doc)
+    ids = com.get_ids_from_element_collector(col_cat)
+    return ids
 
 
-def get_all_level_type_ids_by_category(doc):
+def get_all_duct_type_ids_in_model_by_class(doc):
     """
-    Gets a list of all level type ids in the model.
-
+    Gets all duct type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A list of all level type ids.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: A list of ids representing duct types.
+    :rtype: List Autodesk.Revit.DB.ElementId
     """
 
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Levels)
-        .WhereElementIsElementType()
-    )
-    ids = com.get_ids_from_element_collector(collector)
+    ids = []
+    col_class = get_all_duct_types_by_class(doc)
+    ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-# -------------------------------------------------  purge --------------------------------------------------------------------
+# --------------------------------------- symbols used in MEP system types -------------------------------
 
 
-def get_all_level_head_family_type_ids(doc):
+def get_symbol_ids_used_in_duct_types(doc):
     """
-    Gets ids of all level head family symbols (types) in the model.
-
+    Gets a list of unique symbol ids used in system type properties of duct types.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A list of symbol ids.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: List of unique ids representing family symbols used in duct systems.
+    :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    filter = rdb.ElementCategoryFilter(rdb.BuiltInCategory.OST_LevelHeads)
-    col = (
-        rdb.FilteredElementCollector(doc).OfClass(rdb.FamilySymbol).WherePasses(filter)
+    tye_ids = get_all_duct_type_ids_in_model_by_category(doc)
+    ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
+    return ids
+
+
+def get_symbol_ids_for_duct_types_in_model(doc):
+    """
+    Gets list of symbol ids of the following categories:
+    - BuiltInCategory.OST_DuctAccessory,
+    - BuiltInCategory.OST_DuctTerminal,
+    - BuiltInCategory.OST_DuctFitting
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: List of ids representing family symbols.
+    :rtype: list  Autodesk.Revit.DB.ElementId
+    """
+
+    ids = get_symbol_ids_of_mep_system_types(
+        doc, CATS_LOADABLE_DUCTS, "GetSymbolIdsForDuctTypes"
     )
-    ids = com.get_ids_from_element_collector(col)
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Levels/levels_appearance.py` & `DuHast-0.1.3/src/duHast/Revit/Levels/levels_appearance.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Levels/purge_unused_level_types.py` & `DuHast-0.1.3/src/duHast/Revit/Levels/purge_unused_level_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/fill_pattern_settings.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/fill_pattern_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/Objects/Data/line_pattern_settings.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/fill_patterns.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_property_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Revit fill patterns helper functions. 
+This module contains the view property utilities.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -15,49 +15,37 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from Autodesk.Revit.DB import FilteredElementCollector, FillPatternElement
 
-
-def get_all_fill_pattern(doc):
-    """
-    Gets all fill pattern elements in the model.
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of all fill pattern elements.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+def convert_view_data_to_list(view_data, headers):
     """
+    Converts a list of dictionaries of view properties names and values to a list of properties only.
 
-    return FilteredElementCollector(doc).OfClass(FillPatternElement)
-
-
-def pattern_ids_by_name(doc):
-    """
-    Returns a dictionary where fill pattern name is key, values are all ids of line patterns with the exact same name.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-
-    :return: A dictionary where fill pattern name is key, values are all ids of line patterns with the exact same name
-    :rtype: dictionary(key str, value list of Autodesk.Revit.DB.ElementId)
+    :param view_data: List of dictionaries representing view properties
+    :type view_data: [{}]
+    :param headers: list of properties
+    :type headers: [str]
+    :return: A list of lists of view property values.
+    :rtype: [[str]]
     """
 
-    pattern_dic = {}
-    all_fill_pattern = get_all_fill_pattern(doc=doc)
-    for fill_pattern in all_fill_pattern:
-        pattern_name = fill_pattern.GetFillPattern().Name
-        if pattern_name in pattern_dic:
-            pattern_dic[pattern_name].append(fill_pattern.Id)
-        else:
-            pattern_dic[pattern_name] = [fill_pattern.Id]
-    return pattern_dic
+    data = []
+    for view_d in view_data:
+        data_row = []
+        for header in headers:
+            if header in view_d:
+                data_row.append(view_d[header])
+            else:
+                data_row.append("Property does not exist on element.")
+        data.append(data_row)
+    return data
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities import utility as util
 from duHast.Revit.Categories import categories as rCats
 from duHast.Revit.LinePattern.line_patterns import (
     get_line_pattern_from_category,
     get_line_pattern_from_level_element,
     PROPERTY_PATTERN_ID,
 )
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data_processor.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/Objects/line_pattern_data_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Family.Data.ifamily_processor import IFamilyProcessor
-from duHast.Revit.LinePattern import line_pattern_data as rLinePatData
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects.ifamily_processor import IFamilyProcessor
+from duHast.Revit.LinePattern.Data.Objects import line_pattern_data as rLinePatData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities.Objects import result as res
 
 
 class LinePatternProcessor(IFamilyProcessor):
     def __init__(self, pre_actions=None, post_actions=None):
         """
         Class constructor.
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/line_pattern_data_purge_unused.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/Data/line_pattern_data_purge_unused.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 #
 #
 #
 
 # class used for stats reporting
 from duHast.Utilities.Objects import result as res
 from duHast.Revit.Common import delete as rDel
-from duHast.Revit.Family.Data import ifamily_data as IFamData
-from duHast.Revit.LinePattern import line_pattern_data as rLinePatData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
+from duHast.Revit.LinePattern.Data.Objects import line_pattern_data as rLinePatData
 
 import Autodesk.Revit.DB as rdb
 
 
 def purge_unused(doc, processor):
     """
     This will delete all line patterns that are not used by any element in the family or nested families.
@@ -64,15 +64,15 @@
     # from processor instance get all root line pattern entries where usage counter == 0.
     # delete those line patterns by id
 
     return_value = res.Result()
 
     ids_to_delete = []
     # get categories found in root processor data only
-    root_fam_data = processor._findRootFamilyData()
+    root_fam_data = processor._find_root_family_data()
     # get all root line pattern entries where usage counter == 0.
     for root_fam in root_fam_data:
         if root_fam[IFamData.USAGE_COUNTER] == 0:
             return_value.append_message(
                 "Found unused line patterns: {} [{}]".format(
                     root_fam[rLinePatData.PATTERN_NAME],
                     root_fam[rLinePatData.PATTERN_ID],
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/line_patterns.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/line_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param contains: Filter: pattern name needs to contain this string to be deleted.
     :type contains: str
 
     :return:
         Result class instance.
 
-        - .result = True if line pattern where deleted successfully. Otherwise False.
+        - .status True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
     lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
     ids = list(
@@ -165,15 +165,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param starts_with: Filter: pattern name needs to start with this string to be deleted.
     :type starts_with: str
 
     :return:
         Result class instance.
 
-        - .result = True if line pattern where deleted successfully. Otherwise False.
+        - .status True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
     lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
     ids = list(
@@ -196,15 +196,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param contains: Filter: pattern name needs not to contain this string to be deleted.
     :type contains: str
 
     :return:
         Result class instance.
 
-        - .result = True if line pattern where deleted successfully. Otherwise False.
+        - .status True if line pattern where deleted successfully. Otherwise False.
         - .message will contain delete status per pattern.
 
     :rtype: :class:`.Result`
     """
 
     lps = FilteredElementCollector(doc).OfClass(LinePatternElement).ToList()
     ids = list(lp.Id for lp in lps).ToList[ElementId]()
@@ -262,15 +262,15 @@
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
     :return:
         Result class instance.
 
-        - .result = True if all views where deleted. Otherwise False.
+        - .status True if all views where deleted. Otherwise False.
         - .message will contain deletion status.
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     return_value.append_message(
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/line_styles.py` & `DuHast-0.1.3/src/duHast/Revit/Floors/Utility/floors_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Revit line line styles helper functions. 
+This module contains a Revit floors utility functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,59 +22,56 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import clr
+# import Autodesk
+from Autodesk.Revit.DB import BuiltInCategory, FilteredElementCollector, FloorType
 
-clr.AddReference("System.Core")
-from System import Linq
 
-clr.ImportExtensions(Linq)
-
-import Autodesk.Revit.DB as rdb
-from duHast.Revit.Common import delete as rDel
+# doc:   current model document
+def _get_all_floor_types_by_category(doc):
+    """
+    Function returning a filtered element collector of all floor types in the model.
 
+    This uses builtinCategory as filter. Return types includes:
+    - Floor
+    - In place families or loaded families
 
-def delete_line_styles_starts_with(doc, starts_with):
-    """
-    Deletes all line styles where the name starts with provided string
+    It will therefore not return any foundation slab types.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param starts_with: Filter: style name needs to start with this string to be deleted.
-    :type starts_with: str
-    :return: Result class instance.
-
-        - .result = True if all views where deleted. Otherwise False.
-        - .message will contain deletion status.
-        
-    :rtype: :class:`.Result`
+
+    :return: A filtered element collector of floor types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    lc = doc.Settings.Categories[rdb.BuiltInCategory.OST_Lines]
-    ids = list(c.Id for c in lc.SubCategories if c.Name.StartsWith(starts_with)).ToList[
-        rdb.ElementId
-    ]()
-    result = rDel.delete_by_element_ids(
-        doc,
-        ids,
-        "Delete line styles where name starts with: " + str(starts_with),
-        "line styles starting with: " + str(starts_with),
+    collector = (
+        FilteredElementCollector(doc)
+        .OfCategory(BuiltInCategory.OST_Floors)
+        .WhereElementIsElementType()
     )
-    return result
+    return collector
 
 
-def get_all_line_style_ids(doc):
+# doc   current model document
+def _get_floor_types_by_class(doc):
     """
-    Gets all line styles ids in the model.
+    Function returning a filtered element collector of all floor types in the model.
+
+    - Floor
+    - Foundation Slab
+
+    it will therefore not return any in place family types ...
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of all line style ids.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+
+    :return: A filtered element collector of floor types.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    lc = doc.Settings.Categories[rdb.BuiltInCategory.OST_Lines]
-    ids = list(c.Id for c in lc.SubCategories).ToList[rdb.ElementId]()
-    return ids
+    collector = FilteredElementCollector(doc).OfClass(FloorType)
+    return collector
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/LinePattern/purge_unused_line_patterns.py` & `DuHast-0.1.3/src/duHast/Revit/Views/sheets.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Function to purge Revit line patterns.
+This module contains a number of helper functions relating to Revit view sheets. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,128 +22,140 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from Autodesk.Revit.DB import (
-    FilteredElementCollector,
-    LinePatternElement,
-    Transaction,
-    TransactionGroup,
-    TransactionStatus,
-)
+import clr
 
-modified_by_delete = 0
+import Autodesk.Revit.DB as rdb
+from duHast.Utilities import utility as util
+from duHast.Revit.Views.Utility.sheet_parameters import get_sheet_number
+from duHast.Revit.Common import parameter_get_utils as rParaGet
 
+# required in lambda expressions!
+clr.AddReference("System.Core")
+import System
 
-def purge_unused_line_patterns(rvt_doc, DEBUG=False):
+clr.ImportExtensions(System.Linq)
+
+
+def get_sheets_by_filters(doc, view_rules=None):
+    """
+    Gets sheets matching filters provided
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param view_rules: A set of rules. If sheet matches rule it will be returned. Defaults to None which will return all sheets.
+    :type view_rules: array in format [parameter name, condition test method, value to test against], optional
+    :return: Views matching filter
+    :rtype: list of Autodesk.Revit.DB.View
     """
-    This script will ascertain line patterns not used in your model and delete them.
-    It deletes the line patterns one by one and checks if there is modified elements
-    which indicates an element was using the line pattern. The trasaction is rolled
-    back if there is a modified element.
 
-    IMPORTANT: This has flushed out some corrupt families with unresolvable geometry
-    so it is advisable to run on a detached copy of your model first and rectify any
-    family errors
+    collector_views = rdb.FilteredElementCollector(doc).OfClass(rdb.ViewSheet)
+    views = []
+    for v in collector_views:
+        # if no filter rules applied return al sheets
+        if view_rules is not None:
+            paras = v.GetOrderedParameters()
+            rule_match = True
+            for para_name, paraCondition, conditionValue in view_rules:
+                for p in paras:
+                    if p.Definition.Name == para_name:
+                        rule_match = rule_match and rParaGet.check_parameter_value(
+                            p, paraCondition, conditionValue
+                        )
+            if rule_match == True:
+                # delete view
+                views.append(v)
+        else:
+            views.append(v)
+    return views
 
-    Credit for this script goes to Autodesk forum
-    user so-chong from the below forum post
-    https://forums.autodesk.com/t5/revit-api-forum/check-if-linepattern-is-in-use/td-p/7435014
 
-    :param rvt_doc: The Revit document to purge line patterns from
-    :type rvt_doc: Document
-    :param DEBUG: Whether to print debug information or not. Optional. Defaults to False
-    :type DEBUG: bool
+def get_all_sheets(doc):
+    """
+    Gets all sheets in a model
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: list of sheet views
+    :rtype: list of Autodesk.Revit.DB.View
     """
 
-    def document_change_purge_line_patterns(sender, e):
-        """
-        Function to execute on DocumentChanged and inspect the modified & deleted elements.
-        An unused line pattern will have 1 deleted element and 0 modified elements.
-
-        """
-        deleted_elems = e.GetDeletedElementIds()
-        modified_elems = e.GetModifiedElementIds()
-        debug_string = ""
-
-        if DEBUG:
-            if str(e.Operation) == "TransactionCommitted":
-                debug_string += "Deleted elements: {}\n".format(len(deleted_elems))
-                debug_string += "Modified elements: {}\n".format(len(modified_elems))
-
-                if len(modified_elems) == 0:
-                    debug_string += (
-                        "No modified elements. Line pattern will be deleted\n"
-                    )
-                elif len(modified_elems) > 0:
-                    debug_string += (
-                        "Line pattern will not be deleted. Event modified elements:\n"
-                    )
-                    for elem_id in modified_elems:
-                        elem = rvt_doc.GetElement(elem_id)
-                        debug_string += "{}\n".format(elem.Name)
-
-            print(debug_string)
-
-        global modified_by_delete
-        modified_by_delete = len(deleted_elems) + len(modified_elems)
-
-    # Get the application and subscribe to the DocumentChanged event
-    app = rvt_doc.Application
-    app.DocumentChanged += document_change_purge_line_patterns
-
-    # Get all line patterns in the model
-    line_patterns = (
-        FilteredElementCollector(rvt_doc).OfClass(LinePatternElement).ToElements()
-    )
-
-    deleted_line_patterns = ""
-    unused_line_pattern_count = 0
-
-    # Loop through the line patterns and delete them one by one
-    for lp in line_patterns:
-        if DEBUG:
-            print("Processing line pattern: {}".format(lp.Name))
-
-        line_pattern_data = lp.Name + " (id: {})".format(lp.Id)
-
-        # Transaction group is what we will roll back if there is a modified element
-        trans_grp = TransactionGroup(rvt_doc, "Purge Line Patterns")
-        trans_grp.Start()
-
-        # Transaction is what we will commit to trigger DocumentChanged
-        trans = Transaction(rvt_doc, "Purge Line Pattern")
-        trans.Start()
-
-        rvt_doc.Delete(lp.Id)
-        trans.Commit()
-
-        global modified_by_delete
-
-        if modified_by_delete == 1:
-            unused_line_pattern_count += 1
-            deleted_line_patterns += line_pattern_data + "\n"
-            trans_grp.Assimilate()
+    collector_views = rdb.FilteredElementCollector(doc).OfClass(rdb.ViewSheet)
+    return collector_views
 
-        else:
-            trans_grp.RollBack()
 
-    deleted_line_patterns += "\n"
-    out_message = "\nDeleted {} unused line patterns:\n\n{}".format(
-        unused_line_pattern_count, deleted_line_patterns
-    )
-
-    print("\nLine patterns before purge: {}\n\n".format(len(line_patterns)))
-    # Get all line patterns in the model again for a post-task count
-    line_patterns = (
-        FilteredElementCollector(rvt_doc).OfClass(LinePatternElement).ToElements()
-    )
-    print(out_message)
-    print("\nLine patterns after purge: {}".format(len(line_patterns)))
+def get_sheet_rev_by_sheet_number(doc, sheet_number):  # type # type: str
+    """
+    Returns the revision of a sheet identified by its number. Default value is '-'.
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param sheet_number: The number of the sheet of which the revision is to be returned.
+    :type sheet_number: str
+    :raise: Any exception will need to be managed by the function caller.
+
+    :return: The sheet's current revision value. If no matching sheet is found, '-' is returned.
+    :rtype: str
+    """
+
+    rev_value = "-"
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfClass(rdb.ViewSheet)
+        .Where(lambda e: e.SheetNumber == sheet_number)
+    )  # type
+    results = collector.ToList()
+    if len(results) > 0:
+        sheet = results[0]
+        rev_p = sheet.get_Parameter(rdb.BuiltInParameter.SHEET_CURRENT_REVISION)
+        rev_value = rev_p.AsString()
+    return rev_value
+
+
+def get_sheet_rev_by_sheet_name(doc, sheet_name):  # type # type: str
+    """
+    Returns the revision of a sheet identified by its name. Default value is '-'.
+
+    Since multiple sheets can have the same name, it will return the revision of the first sheet matching the name.
+
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param sheet_name: The name of the sheet of which the revision is to be returned.
+    :type sheet_name: str
+    :raise: Any exception will need to be managed by the function caller.
+
+    :return: The sheet's current revision value. If no matching sheet is found, '-' is returned.
+    :rtype: str
+    """
+
+    rev_value = "-"
+    collector = (
+        rdb.FilteredElementCollector(doc)
+        .OfClass(rdb.ViewSheet)
+        .Where(lambda e: e.Name == sheet_name)
+    )  # type
+    results = collector.ToList()
+    if len(results) > 0:
+        sheet = results[0]
+        rev_p = sheet.get_Parameter(rdb.BuiltInParameter.SHEET_CURRENT_REVISION)
+        rev_value = util.pad_single_digit_numeric_string(rev_p.AsString())
+    return rev_value
+
+
+def get_sheet_num_to_elem_dict(rvt_doc):
+    """
+    Get a dictionary of sheet numbers and sheets
+    :param rvt_doc: The Revit document to get the sheets from
+    :type rvt_doc: Document
+    :return: A dictionary of sheet numbers and sheets
+    :rtype: dict
+    """
+    num_elem_dict = {}
+    all_sheets = get_all_sheets(rvt_doc)
 
-    # Unsubscribe from the DocumentChanged event
-    app.DocumentChanged -= document_change_purge_line_patterns
+    for sheet in all_sheets:
+        sht_num = get_sheet_number(sheet)
+        num_elem_dict[sht_num] = sheet
 
-    return out_message
+    return num_elem_dict
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Reporting/cad_links_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Reporting/cad_links_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Reporting/cad_links_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Reporting/links_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Reporting/links_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Reporting/links_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Reporting/links_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Utility/link_path.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Utility/link_path.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/Utility/link_visibility.py` & `DuHast-0.1.3/src/duHast/Revit/Links/Utility/link_visibility.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/cad_links.py` & `DuHast-0.1.3/src/duHast/Revit/Links/cad_links.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 def delete_cad_links(doc):
     """
     Deletes all CAD links in a model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return: Result class instance.
 
-        - .result = True if all CAD links got deleted. Otherwise False.
+        - .status True if all CAD links got deleted. Otherwise False.
         - .message will contain status of deletion.
 
     :rtype: :class:`.Result`
     """
 
     ids = []
     return_value = res.Result()
@@ -175,15 +175,15 @@
     :param host_name_formatted: Not used yet
     :type host_name_formatted: TBC
     :param do_something_with_link_name: A function which amends the link name prior search for a match in folders.\
         I.e. can be used to truncate the link name i.e. the revision details of a link
     :type do_something_with_link_name: func(str) -> str
     :return: Result class instance.
 
-        - .result = True if all CAD links got reloaded successfully. Otherwise False.
+        - .status True if all CAD links got reloaded successfully. Otherwise False.
         - .message will contain status of reload and fully qualified file name. On exception it will also include the exception message.
     
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/cad_links_geometry.py` & `DuHast-0.1.3/src/duHast/Revit/Links/cad_links_geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/image_links.py` & `DuHast-0.1.3/src/duHast/Revit/Links/image_links.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/links.py` & `DuHast-0.1.3/src/duHast/Revit/Links/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     Deletes all revit links in a file.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return:
         Result class instance.
 
-        - .result = True if all revit links got deleted successfully. Otherwise False.
+        - .status True if all revit links got deleted successfully. Otherwise False.
         - .message will contain deletion status. On exception it will also include the exception message.
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     col = FilteredElementCollector(doc).OfCategory(BuiltInCategory.OST_RvtLinks)
@@ -166,15 +166,15 @@
     :type do_something_with_link_name: func(str) -> str
     :param workset_config: To use the previously applied workset config use None, otherwise provide custom config.
     :type workset_config: Autodesk.Revit.DB.WorksetConfiguration
 
     :return: 
         Result class instance.
         
-        - .result = True if all revit links got reloaded successfully. Otherwise False.
+        - .status True if all revit links got reloaded successfully. Otherwise False.
         - .message will contain status of reload and fully qualified file name. On exception it will also include the exception message.
     
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
@@ -238,15 +238,15 @@
     :type do_something_with_link_name: func(str) -> str
     :param workset_config: To use the previously applied workset config use None, otherwise provide custom config.
     :type workset_config: Autodesk.Revit.DB.WorksetConfiguration
 
     :return: 
         Result class instance.
         
-        - .result = True if all revit links got reloaded successfully. Otherwise False.
+        - .status True if all revit links got reloaded successfully. Otherwise False.
         - .message will contain status of reload and fully qualified file name. On exception it will also include the exception message.
     
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Links/purge_unused_image_link_types.py` & `DuHast-0.1.3/src/duHast/Revit/Links/purge_unused_image_link_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Reporting/mep_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/MergeLists.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemCategories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPSystemNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/RevitMEPTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/Utility/SymbolsInSystemTypes.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/cable_trays.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/conduits.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit cable trays.
+This module contains a number of helper functions relating to Revit conduits.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -31,141 +31,141 @@
 import Autodesk.Revit.DB.Electrical as rdbE
 
 from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
     get_symbol_ids_of_mep_system_types,
     get_unique_ids_of_used_symbols_from_system_type_ids,
 )
 from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
-    CATS_LOADABLE_CABLE_TRAYS,
+    CATS_LOADABLE_CONDUITS,
 )
 from duHast.Revit.Common import common as com
 
 
-def get_all_cable_tray_types_by_category(doc):
+def get_all_conduit_types_by_category(doc):
     """
-    Gets a filtered element collector of all cable tray types in the model.
+    Gets a filtered element collector of all conduit types in the model.
     - with fittings
     - without fittings
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of cable tray types
+    :return: A filtered element collector of conduit types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     collector = (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_CableTray)
+        .OfCategory(rdb.BuiltInCategory.OST_Conduit)
         .WhereElementIsElementType()
     )
     return collector
 
 
-def get_cable_tray_types_by_class(doc):
+def get_all_conduit_types_by_class(doc):
     """
-    Gets a filtered element collector of all cable tray types in the model.
+    Gets a filtered element collector of all conduit types in the model.
     - with fittings
     - without fittings
     Will exclude in place families.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of cable tray types
+    :return: A filtered element collector of conduit types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbE.CableTrayType)
+    return rdb.FilteredElementCollector(doc).OfClass(rdbE.ConduitType)
 
 
-def get_all_cable_tray_instances_by_category(doc):
+def get_all_conduit_instances_by_category(doc):
     """
-    Gets all cable tray elements placed in model.
+    Gets all conduit elements placed in model.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of cable tray instances
+    :return: A filtered element collector of conduit instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     collector = (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_CableTray)
+        .OfCategory(rdb.BuiltInCategory.OST_Conduit)
         .WhereElementIsNotElementType()
     )
     return collector
 
 
-def get_all_cable_tray_instances_by_class(doc):
+def get_all_conduit_instances_by_class(doc):
     """
-    Gets all cable tray elements placed in model.
+    Gets all conduit elements placed in model.
     Will exclude in place families.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of cable tray instances
+    :return: A filtered element collector of conduit instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfClass(rdbE.CableTrayType)
+        .OfClass(rdbE.ConduitType)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_cable_tray_type_ids_in_model_by_category(doc):
+def get_all_conduit_type_ids_in_model_by_category(doc):
     """
-    Gets all cable tray type ids available in model.
+    Gets all conduit type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing cable tray types.
+    :return: A list of ids representing conduit types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_cable_tray_types_by_category(doc)
+    col_cat = get_all_conduit_types_by_category(doc)
     ids = com.get_ids_from_element_collector(col_cat)
     return ids
 
 
-def get_all_cable_tray_type_ids_in_model_by_class(doc):
+def get_all_conduit_type_ids_in_model_by_class(doc):
     """
-    Gets all cable tray type ids available in model.
+    Gets all conduit type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing cable tray types.
+    :return: A list of ids representing conduit types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_cable_tray_types_by_class(doc)
+    col_class = get_all_conduit_types_by_class(doc)
     ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-def get_symbol_ids_used_in_cable_tray_types(doc):
+def get_symbol_ids_used_in_conduit_types(doc):
     """
-    Gets a list of unique symbol ids used in system type properties of cable tray types.
+    Gets a list of unique symbol ids used in system type properties of conduit types.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of unique ids representing family symbols used in cable tray systems.
+    :return: List of unique ids representing family symbols used in conduit systems.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    tye_ids = get_all_cable_tray_type_ids_in_model_by_category(doc)
+    tye_ids = get_all_conduit_type_ids_in_model_by_category(doc)
     ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
     return ids
 
 
-def get_symbol_ids_for_cable_tray_types_in_model(doc):
+def get_symbol_ids_for_conduit_types_in_model(doc):
     """
     Gets list of symbol ids of the following categories:
-    - BuiltInCategory.OST_CableTrayFitting
+    - BuiltInCategory.OST_ConduitFitting
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return: List of ids representing family symbols.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = get_symbol_ids_of_mep_system_types(
-        doc, CATS_LOADABLE_CABLE_TRAYS, "GetSymbolIdsForCableTrayTypes"
+        doc, CATS_LOADABLE_CONDUITS, "GetSymbolIdsForConduitTypes"
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/conduits.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/flex_ducts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit conduits.
+This module contains a number of helper functions relating to Revit flex ducts.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -21,151 +21,152 @@
 #
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
-#
 
 import Autodesk.Revit.DB as rdb
-import Autodesk.Revit.DB.Electrical as rdbE
+import Autodesk.Revit.DB.Mechanical as rdbM
 
 from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
     get_symbol_ids_of_mep_system_types,
     get_unique_ids_of_used_symbols_from_system_type_ids,
 )
 from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
-    CATS_LOADABLE_CONDUITS,
+    CATS_LOADABLE_DUCTS,
 )
 from duHast.Revit.Common import common as com
 
 
-def get_all_conduit_types_by_category(doc):
+def get_all_flex_duct_types_by_category(doc):
     """
-    Gets a filtered element collector of all conduit types in the model.
-    - with fittings
-    - without fittings
+    Gets a filtered element collector of all flex duct types in the model.
+    - round
+    - rectangular
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of conduit types
+    :return: A filtered element collector of flex duct types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     collector = (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Conduit)
+        .OfCategory(rdb.BuiltInCategory.OST_FlexDuctCurves)
         .WhereElementIsElementType()
     )
     return collector
 
 
-def get_all_conduit_types_by_class(doc):
+def get_all_flex_duct_types_by_class(doc):
     """
-    Gets a filtered element collector of all conduit types in the model.
-    - with fittings
-    - without fittings
+    Gets a filtered element collector of all flex duct types in the model.
+    - round
+    - rectangular
     Will exclude in place families.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of conduit types
+    :return: A filtered element collector of flex duct types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbE.ConduitType)
+    return rdb.FilteredElementCollector(doc).OfClass(rdbM.FlexDuctType)
 
 
-def get_all_conduit_instances_by_category(doc):
+def get_all_flex_duct_instances_in_model_by_category(doc):
     """
-    Gets all conduit elements placed in model.
+    Gets all flex duct elements placed in model.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of conduit instances
+    :return: A filtered element collector of flex duct instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
+    return (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Conduit)
+        .OfCategory(rdb.BuiltInCategory.OST_FlexDuctCurves)
         .WhereElementIsNotElementType()
     )
-    return collector
 
 
-def get_all_conduit_instances_by_class(doc):
+def get_all_flex_duct_instances_in_model_by_class(doc):
     """
-    Gets all conduit elements placed in model.
+    Gets all flex duct elements placed in model.
     Will exclude in place families.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of conduit instances
+    :return: A filtered element collector of flex duct instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfClass(rdbE.ConduitType)
+        .OfClass(rdbM.FlexDuctType)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_conduit_type_ids_in_model_by_category(doc):
+def get_all_flex_duct_type_ids_in_model_by_category(doc):
     """
-    Gets all conduit type ids available in model.
+    Gets all flex duct type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing conduit types.
+    :return: A list of ids representing flex duct types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_conduit_types_by_category(doc)
+    col_cat = get_all_flex_duct_types_by_category(doc)
     ids = com.get_ids_from_element_collector(col_cat)
     return ids
 
 
-def get_all_conduit_type_ids_in_model_by_class(doc):
+def get_all_flex_duct_type_ids_in_model_by_class(doc):
     """
-    Gets all conduit type ids available in model.
+    Gets all flex duct type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing conduit types.
+    :return: A list of ids representing flex duct types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_all_conduit_types_by_class(doc)
+    col_class = get_all_flex_duct_types_by_class(doc)
     ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-def get_symbol_ids_used_in_conduit_types(doc):
+def get_symbol_ids_used_in_flex_duct_types(doc):
     """
-    Gets a list of unique symbol ids used in system type properties of conduit types.
+    Gets a list of unique symbol ids used in system type properties of flex duct types.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of unique ids representing family symbols used in conduit systems.
+    :return: List of unique ids representing family symbols used in flex duct systems.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    tye_ids = get_all_conduit_type_ids_in_model_by_category(doc)
+    tye_ids = get_all_flex_duct_type_ids_in_model_by_category(doc)
     ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
     return ids
 
 
-def get_symbol_ids_for_conduit_types_in_model(doc):
+def get_symbol_ids_for_flex_duct_types_in_model(doc):
     """
     Gets list of symbol ids of the following categories:
-    - BuiltInCategory.OST_ConduitFitting
+    - BuiltInCategory.OST_DuctAccessory,
+    - BuiltInCategory.OST_DuctTerminal,
+    - BuiltInCategory.OST_DuctFitting
+    TODO: flex duct and duct do not differentiate in terms of filtering...one function will get both
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return: List of ids representing family symbols.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = get_symbol_ids_of_mep_system_types(
-        doc, CATS_LOADABLE_CONDUITS, "GetSymbolIdsForConduitTypes"
+        doc, CATS_LOADABLE_DUCTS, "GetSymbolIdsForDuctTypes"
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/ducts.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/pipes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit ducts.
+This module contains a number of helper functions relating to Revit pipes.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -21,157 +21,147 @@
 #
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
-#
 
 import Autodesk.Revit.DB as rdb
-import Autodesk.Revit.DB.Mechanical as rdbM
+import Autodesk.Revit.DB.Plumbing as rdbP
 
 from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
     get_symbol_ids_of_mep_system_types,
     get_unique_ids_of_used_symbols_from_system_type_ids,
 )
 from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
-    CATS_LOADABLE_DUCTS,
+    CATS_LOADABLE_PIPES,
 )
 from duHast.Revit.Common import common as com
 
 
-def get_all_duct_types_by_category(doc):
+def get_all_pipe_types_by_category(doc):
     """
-    Gets a filtered element collector of all duct types in the model.
-    - round
-    - oval
-    - rectangular
+    Gets a filtered element collector of all pipe types in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of duct types
+    :return: A filtered element collector of pipe tray types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     collector = (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_DuctCurves)
+        .OfCategory(rdb.BuiltInCategory.OST_PipeCurves)
         .WhereElementIsElementType()
     )
     return collector
 
 
-def get_all_duct_types_by_class(doc):
+def get_all_pipe_types_by_class(doc):
     """
-    Gets a filtered element collector of all duct types in the model.
-    - round
-    - oval
-    - rectangular
+    Gets a filtered element collector of all pipe types in the model.
     Will exclude in place families.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of duct types
+    :return: A filtered element collector of pipe tray types
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbM.DuctType)
+    return rdb.FilteredElementCollector(doc).OfClass(rdbP.PipeType)
 
 
-def get_all_duct_instances_in_model_by_category(doc):
+def get_all_pipe_instances_by_category(doc):
     """
-    Gets all duct elements placed in model.
+    Gets all pipe elements placed in model.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of duct instances
+    :return: A filtered element collector of pipe instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return (
+    collector = (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_DuctCurves)
+        .OfCategory(rdb.BuiltInCategory.OST_PipeCurves)
         .WhereElementIsNotElementType()
     )
+    return collector
 
 
-def get_all_duct_instances_in_model_by_class(doc):
+def get_all_pipe_instances_by_class(doc):
     """
-    Gets all duct elements placed in model.
+    Gets all pipe elements placed in model.
     Will exclude in place families.
     TODO: check these actually work...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of duct instances
+    :return: A filtered element collector of pipe instances
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfClass(rdbM.DuctType)
+        .OfClass(rdbP.PipeType)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_duct_type_ids_in_model_by_category(doc):
+def get_all_pipe_type_ids_in_model_by_category(doc):
     """
-    Gets all duct type ids available in model.
+    Gets all pipe type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing duct types.
+    :return: A list of ids representing pipe types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_duct_types_by_category(doc)
+    col_cat = get_all_pipe_types_by_category(doc)
     ids = com.get_ids_from_element_collector(col_cat)
     return ids
 
 
-def get_all_duct_type_ids_in_model_by_class(doc):
+def get_all_pipe_type_ids_in_model_by_class(doc):
     """
-    Gets all duct type ids available in model.
+    Gets all pipe type ids available in model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing duct types.
+    :return: A list of ids representing pipe types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_all_duct_types_by_class(doc)
+    col_class = get_all_pipe_types_by_class(doc)
     ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-# --------------------------------------- symbols used in MEP system types -------------------------------
-
-
-def get_symbol_ids_used_in_duct_types(doc):
+def get_symbol_ids_used_in_pipe_types(doc):
     """
-    Gets a list of unique symbol ids used in system type properties of duct types.
+    Gets a list of unique symbol ids used in system type properties of pipe types.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of unique ids representing family symbols used in duct systems.
+    :return: List of unique ids representing family symbols used in pipe systems.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    tye_ids = get_all_duct_type_ids_in_model_by_category(doc)
+    tye_ids = get_all_pipe_type_ids_in_model_by_category(doc)
     ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
     return ids
 
 
-def get_symbol_ids_for_duct_types_in_model(doc):
+def get_symbol_ids_for_pipe_types_in_model(doc):
     """
     Gets list of symbol ids of the following categories:
-    - BuiltInCategory.OST_DuctAccessory,
-    - BuiltInCategory.OST_DuctTerminal,
-    - BuiltInCategory.OST_DuctFitting
+    - BuiltInCategory.OST_PipeAccessory,
+    - BuiltInCategory.OST_PipeFitting
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return: List of ids representing family symbols.
     :rtype: list  Autodesk.Revit.DB.ElementId
     """
 
     ids = get_symbol_ids_of_mep_system_types(
-        doc, CATS_LOADABLE_DUCTS, "GetSymbolIdsForDuctTypes"
+        doc, CATS_LOADABLE_PIPES, "GetSymbolIdsForPipeTypes"
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/flex_ducts.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/walls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit flex ducts.
+This module contains a number of helper functions relating to Revit walls. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,151 +22,187 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import Autodesk.Revit.DB as rdb
-import Autodesk.Revit.DB.Mechanical as rdbM
+#import clr
 
-from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
-    get_symbol_ids_of_mep_system_types,
-    get_unique_ids_of_used_symbols_from_system_type_ids,
-)
-from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
-    CATS_LOADABLE_DUCTS,
+#clr.AddReference("System.Core")
+#from System import Linq
+
+#clr.ImportExtensions(Linq)
+#import System
+
+# import common library modules
+from duHast.Revit.Common.common import get_ids_from_element_collector
+
+from duHast.Revit.Walls.Utility.walls_type_sorting import sort_wall_types_by_family_name
+from duHast.Revit.Walls.curtain_walls import CURTAIN_WALL_FAMILY_NAME
+from duHast.Revit.Walls.stacked_walls import STACKED_WALL_FAMILY_NAME
+from duHast.Revit.Walls.Utility.walls_filter import _get_all_wall_types_by_category, _get_all_wall_types_by_class
+
+# import Autodesk
+
+from Autodesk.Revit.DB import (
+    BuiltInCategory,
+    ElementCategoryFilter,
+    FamilyInstance,
+    FamilySymbol,
+    FilteredElementCollector,
+    WallKind,
 )
-from duHast.Revit.Common import common as com
+# -------------------------------------------- common variables --------------------
+
+#: Built in wall family name for basic wall
+BASIC_WALL_FAMILY_NAME = WallKind.Basic
+
+#: List of all Built in wall family names
+BUILTIN_WALL_TYPE_FAMILY_NAMES = [
+    STACKED_WALL_FAMILY_NAME,
+    CURTAIN_WALL_FAMILY_NAME,
+    BASIC_WALL_FAMILY_NAME,
+]
 
 
-def get_all_flex_duct_types_by_category(doc):
+def get_all_wall_types_by_category(doc):
     """
-    Gets a filtered element collector of all flex duct types in the model.
-    - round
-    - rectangular
+    Gets all wall types in a model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of flex duct types
+    :return: A filtered element collector containing wall types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_FlexDuctCurves)
-        .WhereElementIsElementType()
-    )
+    collector = _get_all_wall_types_by_category(doc)
     return collector
 
 
-def get_all_flex_duct_types_by_class(doc):
+def get_all_wall_types_by_class(doc):
     """
-    Gets a filtered element collector of all flex duct types in the model.
-    - round
-    - rectangular
-    Will exclude in place families.
+    This will return a filtered element collector of all wall types by class in the model
+
+    It will therefore not return any in place wall types since revit treats those as families...
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of flex duct types
+    :return: A filtered element collector containing wall types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbM.FlexDuctType)
+    collector = _get_all_wall_types_by_class(doc)
+    return collector
 
 
-def get_all_flex_duct_instances_in_model_by_category(doc):
-    """
-    Gets all flex duct elements placed in model.
-    TODO: check these actually work...
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of flex duct instances
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
-    """
-
-    return (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_FlexDuctCurves)
-        .WhereElementIsNotElementType()
-    )
+# -------------------------------- in place wall types -------------------------------------------------------
 
 
-def get_all_flex_duct_instances_in_model_by_class(doc):
+def get_in_place_wall_family_instances(doc):
     """
-    Gets all flex duct elements placed in model.
-    Will exclude in place families.
-    TODO: check these actually work...
+    Returns all instances in place families of category wall in the model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of flex duct instances
+
+    :return: A filtered element collector containing  in place wall instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
+    filter = ElementCategoryFilter(BuiltInCategory.OST_Walls)
     return (
-        rdb.FilteredElementCollector(doc)
-        .OfClass(rdbM.FlexDuctType)
-        .WhereElementIsNotElementType()
+        FilteredElementCollector(doc)
+        .OfClass(FamilyInstance)
+        .WherePasses(filter)
     )
 
 
-def get_all_flex_duct_type_ids_in_model_by_category(doc):
+def get_all_in_place_wall_type_ids(doc):
     """
-    Gets all flex duct type ids available in model.
+    Gets all type ids off all available in place families of category wall.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing flex duct types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+
+    :return: List of element ids representing in place wall types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_flex_duct_types_by_category(doc)
-    ids = com.get_ids_from_element_collector(col_cat)
+    filter = ElementCategoryFilter(BuiltInCategory.OST_Walls)
+    col = (
+        FilteredElementCollector(doc).OfClass(FamilySymbol).WherePasses(filter)
+    )
+    ids = get_ids_from_element_collector(col)
     return ids
 
 
-def get_all_flex_duct_type_ids_in_model_by_class(doc):
+# -------------------------------- basic wall types -------------------------------------------------------
+
+
+def get_all_basic_wall_type_ids(doc):
     """
-    Gets all flex duct type ids available in model.
+    Gets type ids off all available basic wall types in the model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing flex duct types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+
+    :return: List of element ids representing all basic wall types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_all_flex_duct_types_by_class(doc)
-    ids = com.get_ids_from_element_collector(col_class)
+    dic = sort_wall_types_by_family_name(doc)
+    if dic.has_key(BASIC_WALL_FAMILY_NAME):
+        ids = dic[BASIC_WALL_FAMILY_NAME]
     return ids
 
 
-def get_symbol_ids_used_in_flex_duct_types(doc):
+def get_all_basic_wall_instances(doc, available_ids):
     """
-    Gets a list of unique symbol ids used in system type properties of flex duct types.
+    Gets all basic wall elements placed in model...ignores legend elements.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of unique ids representing family symbols used in flex duct systems.
-    :rtype: list  Autodesk.Revit.DB.ElementId
+    :param available_ids:  Filter: curtain wall type ids to check wall instances for.
+    :type available_ids: list of Autodesk.Revit.DB.ElementId
+
+    :return: List of element ids representing all basic wall instances.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = []
-    tye_ids = get_all_flex_duct_type_ids_in_model_by_category(doc)
-    ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
-    return ids
+    instances = []
+    col = (
+        FilteredElementCollector(doc)
+        .OfCategory(BuiltInCategory.OST_Walls)
+        .WhereElementIsNotElementType()
+    )
+    for c in col:
+        if c.GetTypeId() in available_ids:
+            instances.append(c)
+    return instances
 
 
-def get_symbol_ids_for_flex_duct_types_in_model(doc):
+def get_used_basic_wall_type_ids(doc, available_ids):
     """
-    Gets list of symbol ids of the following categories:
-    - BuiltInCategory.OST_DuctAccessory,
-    - BuiltInCategory.OST_DuctTerminal,
-    - BuiltInCategory.OST_DuctFitting
-    TODO: flex duct and duct do not differentiate in terms of filtering...one function will get both
+    Gets all basic wall types used in model.
+
+    Used: at least one instance of this type is placed in the model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of ids representing family symbols.
-    :rtype: list  Autodesk.Revit.DB.ElementId
+    :param available_ids:  Filter: basic wall type ids to check wall instances for.
+    :type available_ids: list of Autodesk.Revit.DB.ElementId
+
+    :return: List of element ids representing all basic wall types in use.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = get_symbol_ids_of_mep_system_types(
-        doc, CATS_LOADABLE_DUCTS, "GetSymbolIdsForDuctTypes"
+    ids = []
+    col = (
+        FilteredElementCollector(doc)
+        .OfCategory(BuiltInCategory.OST_Walls)
+        .WhereElementIsNotElementType()
     )
+    for c in col:
+        if c.GetTypeId() in available_ids:
+            ids.append(c.GetTypeId())
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/pipes.py` & `DuHast-0.1.3/src/duHast/Revit/Roofs/roofs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit pipes.
+This module contains a number of helper functions relating to Revit roofs. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,146 +22,169 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
+import clr
+import System
+
+# import Autodesk
 import Autodesk.Revit.DB as rdb
-import Autodesk.Revit.DB.Plumbing as rdbP
 
-from duHast.Revit.MEP_Systems.Utility.SymbolsInSystemTypes import (
-    get_symbol_ids_of_mep_system_types,
-    get_unique_ids_of_used_symbols_from_system_type_ids,
-)
-from duHast.Revit.MEP_Systems.Utility.RevitMEPSystemCategories import (
-    CATS_LOADABLE_PIPES,
-)
 from duHast.Revit.Common import common as com
+from duHast.Revit.Family import family_utils as rFam
+from duHast.Revit.Roofs.Utility import RevitRoofsFilter as rRoofFilter
+
+# --------------------------------------------- utility functions ------------------
 
 
-def get_all_pipe_types_by_category(doc):
+def get_all_roof_types_by_category(doc):
     """
-    Gets a filtered element collector of all pipe types in the model.
+    Gets a filtered element collector of all roof types in the model.
+
+    - Basic Roof
+    - In place families or loaded families
+    - sloped glazing
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of pipe tray types
+
+    :return: A filtered element collector containing roof types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_PipeCurves)
-        .WhereElementIsElementType()
-    )
+    collector = rRoofFilter._get_all_roof_types_by_category(doc)
     return collector
 
 
-def get_all_pipe_types_by_class(doc):
+def get_all_roof_types_by_class(doc):
     """
-    Gets a filtered element collector of all pipe types in the model.
-    Will exclude in place families.
+    Gets a filtered element collector of all Roof types in the model:
+
+    - Basic Roof
+    - sloped glazing
+
+    Since this is based of class roof it will therefore not return any in place family types!
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of pipe tray types
+
+    :return: A filtered element collector containing roof types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbP.PipeType)
+    collector = rRoofFilter._get_roof_types_by_class(doc)
+    return collector
+
 
+# -------------------------------- none in place Roof types -------------------------------------------------------
 
-def get_all_pipe_instances_by_category(doc):
+
+def get_all_roof_instances_by_category(doc):
     """
-    Gets all pipe elements placed in model.
-    TODO: check these actually work...
+    Gets all Roof elements placed in model...ignores in place families (to be confirmed!)
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of pipe instances
+
+    :return: A filtered element collector containing roof instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
+    return (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_PipeCurves)
+        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
         .WhereElementIsNotElementType()
     )
-    return collector
 
 
-def get_all_pipe_instances_by_class(doc):
+def get_all_roof_instances_by_class(doc):
     """
-    Gets all pipe elements placed in model.
-    Will exclude in place families.
-    TODO: check these actually work...
+    Gets all Roof elements placed in model...ignores roof soffits(???)
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector of pipe instances
+
+    :return: A filtered element collector containing roof instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfClass(rdbP.PipeType)
+        .OfClass(rdb.Roof)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_pipe_type_ids_in_model_by_category(doc):
+def get_all_roof_type_ids_by_category(doc):
     """
-    Gets all pipe type ids available in model.
+    Gets all Roof element type ids available in model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing pipe types.
+
+    :return: List of element ids of roof types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_pipe_types_by_category(doc)
+    col_cat = get_all_roof_types_by_category(doc)
     ids = com.get_ids_from_element_collector(col_cat)
     return ids
 
 
-def get_all_pipe_type_ids_in_model_by_class(doc):
+def get_all_roof_type_ids_by_class(doc):
     """
-    Gets all pipe type ids available in model.
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: A list of ids representing pipe types.
+    Gets all Roof element type ids available in model.
+
+    :param doc: _description_
+    :type doc: _type_
+
+    :return: List of element ids of roof types.
     :rtype: List Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_all_pipe_types_by_class(doc)
+    col_class = get_all_roof_types_by_class(doc)
     ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-def get_symbol_ids_used_in_pipe_types(doc):
+# -------------------------------- In place Roof types -------------------------------------------------------
+
+
+def get_in_place_roof_family_instances(doc):
     """
-    Gets a list of unique symbol ids used in system type properties of pipe types.
+    Gets all instances of in place families of category roof in the model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of unique ids representing family symbols used in pipe systems.
-    :rtype: list  Autodesk.Revit.DB.ElementId
+
+    :return: A filtered element collector containing roof family instances.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    ids = []
-    tye_ids = get_all_pipe_type_ids_in_model_by_category(doc)
-    ids = get_unique_ids_of_used_symbols_from_system_type_ids(doc, tye_ids)
-    return ids
+    filter = rdb.ElementCategoryFilter(rdb.BuiltInCategory.OST_Roofs)
+    return (
+        rdb.FilteredElementCollector(doc)
+        .OfClass(rdb.FamilyInstance)
+        .WherePasses(filter)
+    )
 
 
-def get_symbol_ids_for_pipe_types_in_model(doc):
+def get_all_in_place_roof_type_ids(doc):
     """
-    Gets list of symbol ids of the following categories:
-    - BuiltInCategory.OST_PipeAccessory,
-    - BuiltInCategory.OST_PipeFitting
+    Gets type ids off all available in place families of category roof in the model.
+
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of ids representing family symbols.
-    :rtype: list  Autodesk.Revit.DB.ElementId
+
+    :return: List of element ids of in place roof types.
+    :rtype: List Autodesk.Revit.DB.ElementId
     """
 
-    ids = get_symbol_ids_of_mep_system_types(
-        doc, CATS_LOADABLE_PIPES, "GetSymbolIdsForPipeTypes"
+    ids = rFam.get_all_in_place_type_ids_in_model_of_category(
+        doc, rdb.BuiltInCategory.OST_Roofs
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/purge_unused_mep_symbols.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py` & `DuHast-0.1.3/src/duHast/Revit/MEP_Systems/purge_unused_mep_types.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/materials_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/materials_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Materials/Reporting/materials_report_utils.py` & `DuHast-0.1.3/src/duHast/Revit/Materials/Reporting/materials_report_utils.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Materials/materials.py` & `DuHast-0.1.3/src/duHast/Revit/Materials/materials.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/annotations.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/annotations.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/design_set_options.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/design_set_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/detail_items.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/detail_items.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/families.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/families.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/general.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/rooms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,130 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Model health report functions - general reports.
+Model health report functions - rooms.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Model health report metrics can either be displayed in a family where each parameter is assigned to a metric 
 and or data can be exported to text files which can be used to visualize key metrics over time.
 
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
-import System
-
-
-clr.AddReference("System.Core")
-from System import Linq
+# import System
+# clr.AddReference("System.Core")
+# from System import Linq
+# clr.ImportExtensions(Linq)
 
-clr.ImportExtensions(Linq)
 
 from duHast.Revit.ModelHealth.Reporting.Properties.constants import (
     FAILED_TO_RETRIEVE_VALUE,
 )
 
-from duHast.Utilities.date_stamps import get_file_date_stamp, FILE_DATE_STAMP_YYYY_MM_DD
-from duHast.Utilities.files_io import file_exist, get_file_size
-from duHast.Revit.BIM360.bim_360 import get_model_file_size
-from duHast.Revit.Warnings.warnings import get_warnings
-from duHast.Revit.Common.worksets import get_worksets
+from duHast.Revit.Rooms.rooms import (
+    get_all_rooms,
+    get_unplaced_rooms,
+    get_redundant_rooms,
+    get_not_enclosed_rooms,
+)
+
 
-# --------------------------------------------- GENERAL ---------------------------------------------
+# ---------------------------------------------  Rooms  ---------------------------------------------
 
 
-def get_current_date(doc):
+def get_number_of_rooms(doc):
     """
-    Get the current date
+    Gets the number of rooms in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: The current date in format YYYY_MM_DD.
-    :rtype: str
-
+    :return: Number of rooms in the model. On exception it will return -1
+    :rtype: int
     """
-    return get_file_date_stamp(FILE_DATE_STAMP_YYYY_MM_DD)
+
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_all_rooms(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of rooms: {}".format(e))
+    return number
 
 
-def get_workset_number(doc):
+def get_number_of_unplaced_rooms(doc):
     """
-    Gets the number of worksets in the model.
+    Gets the number of unplaced rooms in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: The number of worksets in a model.
+    :return: Number of unplaced rooms in the model. On exception it will return -1
     :rtype: int
     """
 
-    return len(get_worksets(doc))
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_unplaced_rooms(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of unplaced rooms: {}".format(e))
+    return number
 
 
-def get_current_file_size(doc):
+def get_number_of_redundant_rooms(doc):
     """
-    Gets the file size in MB.
+    Gets the number of redundant rooms in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: File size in MB. On exception it will return -1
+    :return: Number of redundant rooms in the model. On exception it will return -1
     :rtype: int
     """
 
-    size = FAILED_TO_RETRIEVE_VALUE
+    number = FAILED_TO_RETRIEVE_VALUE
     try:
-        # get the path from the document
-        # this will fail if not a file based doc or the document is detached
-        revit_file_path = doc.PathName
-        try:
-            # test if this is a cloud model
-            path = doc.GetCloudModelPath()
-            size = get_model_file_size(doc)
-        except:
-            # local file server model
-            if file_exist(revit_file_path):
-                # get file size in MB
-                size = get_file_size(revit_file_path)
-            else:
-                raise ValueError("File not found: {}".format(revit_file_path))
+        number = len(get_redundant_rooms(doc))
     except Exception as e:
-        raise ValueError("Failed to get file size with: {}".format(e))
-    return size
+        raise ValueError("Failed to get number of redundant rooms: {}".format(e))
+    return number
 
 
-def get_number_of_warnings(doc):
+def get_number_of_not_enclosed_rooms(doc):
     """
-    Gets the number of warnings in the model.
+    Gets the not enclosed number of rooms in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: Number of warnings in model. On exception it will return -1
+    :return: Number of not enclosed rooms in the model. On exception it will return -1
     :rtype: int
     """
 
     number = FAILED_TO_RETRIEVE_VALUE
     try:
-        number = len(get_warnings(doc))
+        number = len(get_not_enclosed_rooms(doc))
     except Exception as e:
-        raise ValueError("Failed to get number of warnings: {}".format(e))
+        raise ValueError("Failed to get number of rooms not enclosed: {}".format(e))
     return number
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/groups.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/groups.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/links_cad.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/links_cad.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 
 import System
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/Properties/view.py` & `DuHast-0.1.3/src/duHast/Revit/Views/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,195 +1,187 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Model health report functions - views.
+This module contains a number of helper functions relating to Revit views. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Model health report metrics can either be displayed in a family where each parameter is assigned to a metric 
-and or data can be exported to text files which can be used to visualize key metrics over time.
-
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
-
-
 import System
 
-clr.AddReference("System.Core")
-from System import Linq
-
-clr.ImportExtensions(Linq)
-
-
-from duHast.Revit.ModelHealth.Reporting.Properties.constants import (
-    FAILED_TO_RETRIEVE_VALUE,
-)
+# import common library modules
+from duHast.Revit.Common import common as com
+from duHast.Revit.Views.Utility.view_types import _get_view_types
+from duHast.Revit.Views.schedules import filter_revision_schedules
 from duHast.Revit.Views.sheets import get_all_sheets
-from duHast.Revit.Views.views import get_views_in_model, get_views_not_on_sheet
-from duHast.Revit.Views.templates import (
-    get_view_templates_ids,
-    get_all_unused_view_template_ids,
-)
-from duHast.Revit.Views.filters import get_all_filters, get_all_unused_view_filters
 
-# --------------------------------------------- VIEWS ---------------------------------------------
+# import Autodesk
+import Autodesk.Revit.DB as rdb
 
 
-def get_number_of_sheets(doc):
+def get_view_types(doc):
     """
-    Gets the number of sheets in the model.
-
+    Returns all view family types in a model
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: Number of sheets in model. On exception it will return -1
-    :rtype: int
+    :return: A filtered element collector.
+    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_all_sheets(doc).ToList())
-    except Exception as e:
-        raise ValueError("Failed to get number of sheets: {}".format(e))
-    return number
+    collector = _get_view_types(doc)
+    return collector
 
 
-def _view_filter(view):
+def get_view_type_ids(doc):
     """
-    generic view filter allowing all views to be selected
+    Returns all view family type ids in a model
 
-    :param view: not used!
-    :type view: Autodesk.Revit.DB.View
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
 
-    :return: returns always True
-    :rtype: bool
+    :return: ids of view family types
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
-    return True
+
+    ids = []
+    col = get_view_types(doc)
+    ids = com.get_ids_from_element_collector(col)
+    return ids
 
 
-def get_number_of_views(doc):
+def get_views_of_type(doc, view_type):
     """
-    Gets the number of views in the model.
+    Gets all views in a model of a given type. Excludes templates.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
+    :param view_type: Filter: the view type
+    :type view_type: Autodesk.Revit.DB.ViewType
 
-    :return: Number of views in model. On exception it will return -1
-    :rtype: int
+    :return: list of views
+    :rtype: list of Autodesk.Revit.DB.View
     """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_views_in_model(doc, _view_filter))
-    except Exception as e:
-        raise ValueError("Failed to get number of views: {}".format(e))
-    return number
 
+    views = []
+    col = rdb.FilteredElementCollector(doc).OfClass(rdb.View)
+    for v in col:
+        if v.ViewType == view_type and v.IsTemplate == False:
+            views.append(v)
+    return views
 
-def get_number_of_unplaced_views(doc):
-    """
-    Gets the number of unplaced views in the model.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
 
-    :return: Number of unplaced views in model. On exception it will return -1
-    :rtype: int
-    """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_views_not_on_sheet(doc))
-    except Exception as e:
-        raise ValueError("Failed to get number of unplaced views: {}".format(e))
-    return number
+# ----------------------------------------------------------------------------------------
 
 
-def get_number_of_view_templates(doc):
+def get_viewport_on_sheets(doc, sheets):
     """
-    Gets the number of view templates in the model.
+    Get all view ports on sheets provided.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
+    :param sheets: list of sheets of which to return the view ports from.
+    :type sheets: list of Autodesk.Revit.DB.ViewSheet
 
-    :return: Number of view templates in model. On exception it will return -1
-    :rtype: int
+    :return: list of view ports
+    :rtype: list of Autodesk.Revit.DB.Viewport
     """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_view_templates_ids(doc))
-    except Exception as e:
-        raise ValueError("Failed to get number of view templates: {}".format(e))
-    return number
-
 
-def get_number_of_unused_view_templates(doc):
-    """
-    Gets the number of unplaced view templates in the model.
+    view_ports = []
+    for sheet in sheets:
+        try:
+            viewport_ids = sheet.GetAllViewports()
+            if viewport_ids != None:
+                for viewport_id in viewport_ids:
+                    viewport = doc.GetElement(viewport_id)
+                    view_ports.append(viewport)
+        except Exception as e:
+            print("Get view ports on sheet: {} threw exception: {}".format(sheet, e))
+    return view_ports
 
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
 
-    :return: Number of unplaced view templates in model. On exception it will return -1
-    :rtype: int
+def get_views_in_model(doc, filter):
     """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_all_unused_view_template_ids(doc))
-    except Exception as e:
-        raise ValueError("Failed to get number of unused view templates: {}".format(e))
-    return number
+    Gets all views in a model which are matching a filter and are:
 
+    - not template views
+    - not system browser
+    - not project browser
+    - not undefined
+    - not Internal
+    - not sheets
 
-def get_number_of_view_filters(doc):
-    """
-    Gets the number of view filters in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
+    :param filter: function checking view
+    :type filter: func(view) returning a bool
 
-    :return: Number of number of view filters in model. On exception it will return -1
-    :rtype: int
+    :return: list of views
+    :rtype: list of Autodesk.Revit.DB.View
     """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_all_filters(doc).ToList())
-    except Exception as e:
-        raise ValueError("Failed to get number of view filters: {}".format(e))
-    return number
+
+    views = []
+    col = rdb.FilteredElementCollector(doc).OfClass(rdb.View)
+    for v in col:
+        # filter out browser organization and other views which cant be deleted
+        if (
+            v.IsTemplate == False
+            and filter(v) == True
+            and v.ViewType != rdb.ViewType.SystemBrowser
+            and v.ViewType != rdb.ViewType.ProjectBrowser
+            and v.ViewType != rdb.ViewType.Undefined
+            and v.ViewType != rdb.ViewType.Internal
+            and v.ViewType != rdb.ViewType.DrawingSheet
+        ):
+            views.append(v)
+    return views
 
 
-def get_number_of_unused_view_filters(doc):
+def get_views_not_on_sheet(doc):
     """
-    Gets the number of unused view filters in the model.
+    Gets all views not placed on a sheet. (Excludes schedules)
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: Number of unused view filters in model. On exception it will return -1
-    :rtype: int
+    :return: A list of views which are currently not placed on a sheet.
+    :rtype: list of Autodesk.Revit.DB.View
     """
-    number = FAILED_TO_RETRIEVE_VALUE
-    try:
-        number = len(get_all_unused_view_filters(doc))
-    except Exception as e:
-        raise ValueError("Failed to get number of unused view filters: {}".format(e))
-    return number
+
+    views_not_on_sheet = []
+    # get all sheets
+    sheets_in_model = get_all_sheets(doc)
+    # get all viewPorts on sheets
+    view_ports_on_sheets = get_viewport_on_sheets(doc, sheets_in_model)
+    # get all views in model
+    views_in_model = get_views_in_model(doc, filter_revision_schedules)
+    # check whether view has a viewport if not ... its not placed on a sheet
+    for view_in_model in views_in_model:
+        match = False
+        for view_ports_on_sheet in view_ports_on_sheets:
+            if view_ports_on_sheet.ViewId == view_in_model.Id:
+                match = True
+                break
+        if match == False:
+            views_not_on_sheet.append(view_in_model)
+    return views_not_on_sheet
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/report_file_names.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 #: header for each report file
 LOG_FILE_HEADER = ["HOSTFILE", "REPORT", "DATE", "TIME", "VALUE"]
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/ModelHealth/model_health.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/model_health.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import os
 import System
 
@@ -211,15 +211,15 @@
     :type fam_instance: Autodesk.Revit.DB.FamilyInstance
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
     :return:
         Result class instance.
 
-        - .result = True if all parameters where found on the family and got updated successfully or no update at all was required. Otherwise False.
+        - .status True if all parameters where found on the family and got updated successfully or no update at all was required. Otherwise False.
         - .message will be 'Failed to get value for'
 
     :rtype: :class:`.Result`
     """
 
     result_value = res.Result()
     flag_update = False
@@ -400,15 +400,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param revit_file_path: Fully qualified revit model file path.
     :type revit_file_path: str
 
     :return:
         Result class instance.
 
-        - .result = True if all model key health metric where updated successfully. Otherwise False.
+        - .status True if all model key health metric where updated successfully. Otherwise False.
         - .message will be listing each parameter update: old value to new value
 
     :rtype: :class:`.Result`
     """
 
     revit_file_name = get_file_name_without_ext(revit_file_path)
     result_value = res.Result()
@@ -444,15 +444,15 @@
     :type revit_file_path: str
     :param output_directory: The directory path of where to write the data to.
     :type output_directory: str
 
     :return:
         Result class instance.
 
-        - .result = True if data was written to files successfully. Otherwise False.
+        - .status True if data was written to files successfully. Otherwise False.
         - .message will be contain data file path for each file.
 
     :rtype: :class:`.Result`
     """
 
     revit_file_name = get_file_name_without_ext(revit_file_path)
     result_value = res.Result()
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Purge/purge_action.py` & `DuHast-0.1.3/src/duHast/Revit/Purge/purge_action.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Purge/purge_unused.py` & `DuHast-0.1.3/src/duHast/Revit/Purge/purge_unused.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 """
 
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import System
 
 from duHast.Utilities import files_io as fileIO
@@ -158,15 +158,15 @@
     :param is_debug: True: will return detailed report and attempt to try to delete elements one by one if an exception occurs, defaults to False\
         Will attempt to delete all elements at once.
     :type is_debug: bool, optional
 
     :return: 
         Result class instance.
         
-        - .result = True if all purge actions completed successfully. Otherwise False.
+        - .status True if all purge actions completed successfully. Otherwise False.
         - .message will be listing each purge action and its status
     
     :rtype: :class:`.Result`
     """
 
     resultValue = res.Result()
     try:
@@ -736,15 +736,15 @@
     :param is_debug: True: will return detailed report and attempt to try to delete elements one by one if an exception occurs. False\
         Will attempt to delete all elements at once, less detailed purge report.
     :type is_debug: bool
 
     :return: 
         Result class instance.
         
-        - .result = True if all purge actions completed successfully. Otherwise False.
+        - .status True if all purge actions completed successfully. Otherwise False.
         - .message will be listing each purge action and its status
     
     :rtype: :class:`.Result`
     """
 
     # the current file name
     revitFileName = fileIO.get_file_name_without_ext(revit_file_path)
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Purge/purge_unused_e_transmit.py` & `DuHast-0.1.3/src/duHast/Revit/Purge/purge_unused_e_transmit.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Reporting/railings_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/Reporting/railings_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Utility/merge_lists.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/Utility/merge_lists.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railing_categories.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railing_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railing_family_names.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railing_family_names.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railings_filter.py` & `DuHast-0.1.3/src/duHast/Revit/LinePattern/purge_unused_line_patterns_by_delete.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,16 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit railings utility functions. 
+Revit purging not used line pattern styles using purge by delete helper functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-"""
-#
-# License:
-#
-#
-# Revit Batch Processor Sample Code
-#
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#
 
-import Autodesk.Revit.DB as rdb
+
 
 """
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit railings utility functions. 
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-"""
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -45,64 +19,90 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import Autodesk.Revit.DB.Architecture as rdbA
+from duHast.Revit.LinePattern.line_patterns import get_all_line_patterns
+from duHast.Revit.Common.common import get_ids_from_element_collector
+from duHast.Revit.Purge.purge_unused_by_delete import purge_unused_elements
+from duHast.Revit.Categories.categories_styles_model import get_category_styles, get_all_used_line_patterns_ids_from_categories
 
-from duHast.Revit.Railings.Utility.railing_categories import RAILING_CATEGORY_FILTER
+from duHast.Utilities.Objects.result import Result
 
 
-def _get_all_railing_types_by_category(doc):
+def get_line_pattern_ids(doc):
     """
-    Gets a filtered element collector of all Railing types in the model.
-
-    Collector will include types of:
-    - Top Rail
-    - Rail support
-    - Hand rail
-    - Rail termination
-    - Railing Systems
-    - In place families or loaded families
+    Returns all line pattern ids in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector of railing related types
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: A list of all line pattern ids in the model.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    multi_cat_filter = rdb.ElementMulticategoryFilter(RAILING_CATEGORY_FILTER)
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .WherePasses(multi_cat_filter)
-        .WhereElementIsElementType()
-    )
-    return collector
+    line_pattern_col = get_all_line_patterns(doc)
+    ids = get_ids_from_element_collector(line_pattern_col)
 
+    # do some pre -purge filtering
+    # remove all line patterns that are used in categories
+    categories_result = get_category_styles(doc)
+    if (categories_result.status):
+        category_styles = categories_result.result
 
-def _get_railing_types_by_class(doc):
-    """
-    Gets a filtered element collector of all Railing types in the model:
+        # get line patterns used in categories
+        used_line_pattern_ids = get_all_used_line_patterns_ids_from_categories(category_styles)
+
+        # remove used line patterns
+        ids = [x for x in ids if x.IntegerValue not in used_line_pattern_ids]
 
-    Collector will include types of:
-    - Railing
+    return ids
 
-    It will therefore not return any top rail or hand rail or in place family types.
+
+def purge_line_pattern_by_delete(doc, progress_callback=None, debug=False):
+    """
+    Purge line pattern by delete.
+
+    Note: This is a very slow process and can take a few hours to complete depending on the size of the model and the number of line patterns.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
+    :param progress_callback: Callback to report progress.
+    :type progress_callback: callable
+    :param debug: Debug mode.
+    :type debug: bool
+    :return: Result class instance.
+
+        - .status True if unused line pattern where deleted or nothing needed to be deleted. Otherwise False.
+        - .message will contain deletion status.
 
-    :return: A filtered element collector of railing types
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    return rdb.FilteredElementCollector(doc).OfClass(rdbA.RailingType)
+    return_value = Result()
+
+    try:
+
+        # purge unused fill patterns
+        purge_result = purge_unused_elements(
+            doc=doc,
+            element_id_getter=get_line_pattern_ids,
+            deleted_elements_modifier=None,
+            modified_elements_modifier=None,
+            progress_callback=progress_callback,
+            debug=debug,
+        )
+
+        return_value.update(purge_result)
+    except Exception as e:
+        return_value.update_sep(
+            False, "Error purging line pattern by delete: {}".format(str(e))
+        )
+
+    return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/Utility/railings_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/Utility/railings_type_sorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/balusters.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/balusters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/purge_unused_railing_and_baluster_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from duHast.Revit.Family import purge_unused_family_types as rFamPurge
 from duHast.Revit.Common import purge_utils as rPurgeUtils
 from duHast.Revit.Railings.balusters import (
     get_all_baluster_symbols_ids,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Railings/railings.py` & `DuHast-0.1.3/src/duHast/Revit/Railings/railings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Ramps/Reporting/ramps_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py` & `DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsFamilyNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py` & `DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsFilter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py` & `DuHast-0.1.3/src/duHast/Revit/Ramps/Utility/RevitRampsTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Ramps/ramps.py` & `DuHast-0.1.3/src/duHast/Revit/Ramps/ramps.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Revisions/new_revision.py` & `DuHast-0.1.3/src/duHast/Revit/Revisions/new_revision.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Revisions/revisions.py` & `DuHast-0.1.3/src/duHast/Revit/Revisions/revisions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Revisions/sequence.py` & `DuHast-0.1.3/src/duHast/Revit/Revisions/sequence.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Roofs/Reporting/roofs_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py` & `DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsFamilyNames.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsFilter.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a Revit roofs utility functions. 
+This module contains a number of helper functions relating to Revit stair path elements. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,52 +22,54 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-# import Autodesk
 import Autodesk.Revit.DB as rdb
+import Autodesk.Revit.DB.Architecture as rdbA
 
+from duHast.Revit.Common import common as com
 
-def _get_all_roof_types_by_category(doc):
-    """
-    Gets a filtered element collector of all roof types in the model.
-
-    - Basic Roof
-    - In place families or loaded families
-    - sloped glazing
 
+def get_stair_path_types_by_class(doc):
+    """
+    Gets a filtered element collector of all Stair path types in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector containing roof types.
+    :return: A filtered element collector containing stair path types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
-        .WhereElementIsElementType()
-    )
-    return collector
+    return rdb.FilteredElementCollector(doc).OfClass(rdbA.StairsPathType)
 
 
-def _get_roof_types_by_class(doc):
+def get_stair_path_types_ids_by_class(doc):
+    """
+    Gets all Stair path element type ids available in model.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :return: List of element ids representing stair path types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
-    Gets a filtered element collector of all Roof types in the model:
 
-    - Basic Roof
-    - sloped glazing
+    ids = []
+    col_class = get_stair_path_types_by_class(doc)
+    ids = com.get_ids_from_element_collector(col_class)
+    return ids
 
-    Since this is based of class roof it will therefore not return any in place family types!
 
+def get_all_stair_path_instances(doc):
+    """
+    Gets a filtered element collector of all Stair path elements in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector containing roof types.
+    :return: A filtered element collector containing stair path elements.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = rdb.FilteredElementCollector(doc).OfClass(rdb.RoofType)
-    return collector
+    return (
+        rdb.FilteredElementCollector(doc)
+        .OfCategory(rdb.BuiltInCategory.OST_StairsPaths)
+        .WhereElementIsNotElementType()
+    )
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py` & `DuHast-0.1.3/src/duHast/Revit/Roofs/Utility/RevitRoofsTypeSorting.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/purge_unused_roof_types.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/purge_unused_curtain_wall_element_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,151 +1,149 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to purging Revit roofs. 
+This module contains a number of helper functions relating to purging Revit curtain wall elements. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-from duHast.Revit.Family import purge_unused_family_types as rFamPurge
-from duHast.Revit.Common import purge_utils as rPurgeUtils
-from duHast.Revit.Roofs.roofs import (
-    get_all_in_place_roof_type_ids,
-    get_all_roof_type_ids_by_class,
-    get_all_roof_type_ids_by_category,
-)
-from duHast.Revit.Roofs.Utility.RevitRoofsFamilyNames import (
-    BUILTIN_ROOF_TYPE_FAMILY_NAMES,
-)
-from duHast.Revit.Roofs.Utility.RevitRoofsTypeSorting import (
-    sort_roof_types_by_family_name,
+from duHast.Revit.Family.purge_unused_family_types import get_unused_in_place_ids_for_purge
+from duHast.Revit.Common.purge_utils import get_used_unused_type_ids
+from duHast.Revit.Walls.curtain_wall_elements import (
+    get_all_curtain_wall_element_type_ids_by_category,
+    get_all_curtain_wall_element_type_ids_by_category_excl_symbols,
+    get_all_curtain_wall_non_shared_symbol_ids_by_category,
+    get_all_curtain_wall_non_shared_symbol_ids_by_category,
 )
 
 
-def get_used_roof_type_ids(doc):
+def get_used_curtain_wall_element_type_ids(doc):
     """
-    Gets all used in Roof type ids in the model.
+    Gets all used Curtain Wall Element element type ids available in model.
     Used: at least one instance of this type is placed in the model.
+    Includes:
+    - curtain wall panels
+    - curtain wall mullions
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids of roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing curtain wall element types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(
-        doc, get_all_roof_type_ids_by_category, 1
+    ids = get_used_unused_type_ids(
+        doc, get_all_curtain_wall_element_type_ids_by_category, 1
     )
     return ids
 
 
-def family_no_types_in_use(famTypeIds, unUsedTypeIds):
+def family_no_types_in_use(fam_type_ids, un_used_type_ids):
     """
-    Compares two lists of element ids and returns False if any element id in first list is not in the second list.
-    Returns False if any symbols (types) of a family (first lists) are in use in a model (second list).
-    TODO: repetitive code...Consider generic function!
-    :param famTypeIds: List of family symbols (types).
-    :type famTypeIds: List of Autodesk.Revit.DB.ElementId
-    :param unUsedTypeIds: List of unused family symbols (types)
-    :type unUsedTypeIds: List of Autodesk.Revit.DB.ElementId
-    :return: True if all ids in first list are also in second list, otherwise False.
+    Compares two lists of ids. True if any id is not in un_used_type_ids.
+    TODO: check for more generic list comparison and remove this function.
+    :param fam_type_ids: List of family type ids to check.
+    :type fam_type_ids: List of Autodesk.Revit.DB.ElementId
+    :param un_used_type_ids: Reference list of ids.
+    :type un_used_type_ids: List of Autodesk.Revit.DB.ElementId
+    :return: True if any id from fam_type_ids is not in un_used_type_ids.
     :rtype: bool
     """
 
     match = True
-    for famTypeId in famTypeIds:
-        if famTypeId not in unUsedTypeIds:
+    for fam_type_id in fam_type_ids:
+        if fam_type_id not in un_used_type_ids:
             match = False
             break
     return match
 
 
-def get_unused_non_in_place_roof_type_ids_to_purge(doc):
+def get_unused_non_symbol_curtain_wall_element_type_ids_to_purge(doc):
     """
-    Gets all unused Roof type ids in the model.
-    This method can be used to safely delete unused roof types. In the case that no roof\
-        instance using any of the types is placed, this will return all but one type id since\
-        Revit requires at least one roof type definition to be in the model.
-    Unused: Not one instance of this type is placed in the model.
-    - Roof Soffit
-    - Compound Roof
-    - Basic Roof
-    It will therefore not return any in place family types.
+    Gets all unused Curtain Wall Element element type ids which can be safely deleted from the model.
+    This method can be used to safely delete unused in curtain wall element types. There is no requirement by Revit to have at least one\
+        curtain wall element definition in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids of roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing unused in curtain wall element types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
     # get unused type ids
-    ids = rPurgeUtils.get_used_unused_type_ids(doc, get_all_roof_type_ids_by_class, 0)
-    # make sure there is at least on Roof type per system family left in model
-    RoofTypes = sort_roof_types_by_family_name(doc)
-    for key, value in RoofTypes.items():
-        if key in BUILTIN_ROOF_TYPE_FAMILY_NAMES:
-            if family_no_types_in_use(value, ids) == True:
-                # remove one type of this system family from unused list
-                ids.remove(value[0])
+    ids = get_used_unused_type_ids(
+        doc,
+        get_all_curtain_wall_element_type_ids_by_category_excl_symbols,
+        0,
+    )
+    # unlike other element types, here I do NOT make sure there is at least on curtain wall element type per system family left in model!!
     return ids
 
 
-def get_used_in_place_roof_type_ids(doc):
+def get_used_curtain_wall_symbol_ids(doc):
     """
-    Gets all used in place roof type ids in the model.
-    Used: at least one instance of this type is placed in the model.
+    Gets a list of all used loadable, non shared, family symbols (types) in the model of categories:
+    - curtain wall panels
+    - curtain wall mullions
+    Used: at least one family instance of this symbol (type) is placed in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids of in place roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing curtain wall family symbols.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(doc, get_all_in_place_roof_type_ids, 1)
+    ids = get_used_unused_type_ids(
+        doc, get_all_curtain_wall_non_shared_symbol_ids_by_category, 1
+    )
     return ids
 
 
-def get_unused_in_place_roof_type_ids(doc):
+def get_unused_curtain_wall_symbol_ids(doc):
     """
-    Gets all unused in place roof type ids in the model.
-    Unused: Not one instance of this type is placed in the model.
+    Gets a list of all used loadable, non shared, family symbols (types) in the model of categories:
+    - curtain wall panels
+    - curtain wall mullions
+    Unused: Not one family instance of this symbol (type) is placed in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids of in place roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing curtain wall family symbols.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = rPurgeUtils.get_used_unused_type_ids(doc, get_all_in_place_roof_type_ids, 0)
+    ids = get_used_unused_type_ids(
+        doc, get_all_curtain_wall_non_shared_symbol_ids_by_category, 0
+    )
     return ids
 
 
-def get_unused_in_place_roof_type_ids_for_purge(doc):
+def get_unused_curtain_wall_symbol_ids_for_purge(doc):
     """
-    Gets symbol(type) ids and family ids (when no type is in use of a family) of in place Roof families which can be purged.
-    This method can be used to safely delete unused in place roof types.
+    Gets symbol(type) ids and family ids (when no type is in use) of curtain wall element families which can be safely deleted from the model.
+    This method can be used to safely delete unused curtain wall element types. There is no requirement by Revit to have at least one\
+        in place wall definition in the model.
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :return: List of element ids of in place roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing unused curtain wall element symbols (types) and families.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
-    ids = rFamPurge.get_unused_in_place_ids_for_purge(
-        doc, get_unused_in_place_roof_type_ids
+    ids = get_unused_in_place_ids_for_purge(
+        doc, get_unused_curtain_wall_symbol_ids
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Roofs/roofs.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/stairs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit roofs. 
+This module contains a number of helper functions relating to Revit stairs. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -25,166 +25,177 @@
 #
 #
 #
 
 import clr
 import System
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
-
 from duHast.Revit.Common import common as com
 from duHast.Revit.Family import family_utils as rFam
-from duHast.Revit.Roofs.Utility import RevitRoofsFilter as rRoofFilter
+from duHast.Revit.Stairs.Utility import stairs_filter as rStairsFilter
 
-# --------------------------------------------- utility functions ------------------
+# import Autodesk
+import Autodesk.Revit.DB as rdb
+import Autodesk.Revit.DB.Architecture as rdbA
 
 
-def get_all_roof_types_by_category(doc):
+def get_all_stair_types_by_category(doc):
     """
-    Gets a filtered element collector of all roof types in the model.
+    Gets a filtered element collector of all Stair types in the model.
 
-    - Basic Roof
+    Return includes:
+    - Stair
+    - Assembled Stair
+    - Precast Stair
+    - Cast-In-Place Stair
     - In place families or loaded families
-    - sloped glazing
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing roof types.
+    :return: A filtered element collector containing stair types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = rRoofFilter._get_all_roof_types_by_category(doc)
+    collector = rStairsFilter._get_all_stair_types_by_category(doc)
     return collector
 
 
-def get_all_roof_types_by_class(doc):
+def get_all_stair_types_by_class(doc):
     """
-    Gets a filtered element collector of all Roof types in the model:
+    Gets a filtered element collector of all Stair types in the model.
+
+    Return includes:
 
-    - Basic Roof
-    - sloped glazing
+    - Assembled Stair
+    - Precast Stair
+    - Cast-In-Place Stair
 
-    Since this is based of class roof it will therefore not return any in place family types!
+    It will not return any in place family or Stair types! These are internally treated as Families or Family Symbols class objects.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing roof types.
+    :return: A filtered element collector containing stair types.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    collector = rRoofFilter._get_roof_types_by_class(doc)
+    collector = rStairsFilter._get_stair_types_by_class(doc)
     return collector
 
 
-# -------------------------------- none in place Roof types -------------------------------------------------------
+# -------------------------------- none in place Stair types -------------------------------------------------------
 
 
-def get_all_roof_instances_by_category(doc):
+def get_all_stair_instances_by_category(doc):
     """
-    Gets all Roof elements placed in model...ignores in place families (to be confirmed!)
+    Gets a filtered element collector of all Stair elements placed in model.
+
+    TODO: Confirm it  ignores in place families?
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing roof instances.
+    :return: A filtered element collector containing stair instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Roofs)
+        .OfCategory(rdb.BuiltInCategory.OST_Stairs)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_roof_instances_by_class(doc):
+def get_all_stair_instances_by_class(doc):
     """
-    Gets all Roof elements placed in model...ignores roof soffits(???)
+    Gets a filtered element collection all Stair elements placed in model...
+
+    TODO: Confirm it ignores Stair soffits.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing roof instances.
+    :return: A filtered element collector containing stair instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     return (
         rdb.FilteredElementCollector(doc)
-        .OfClass(rdb.Roof)
+        .OfClass(rdbA.Stairs)
         .WhereElementIsNotElementType()
     )
 
 
-def get_all_roof_type_ids_by_category(doc):
+def get_all_stair_type_ids_by_category(doc):
     """
-    Gets all Roof element type ids available in model.
+    Gets all Stair element type ids available in model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids of roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing stair types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_cat = get_all_roof_types_by_category(doc)
+    col_cat = get_all_stair_types_by_category(doc)
     ids = com.get_ids_from_element_collector(col_cat)
     return ids
 
 
-def get_all_roof_type_ids_by_class(doc):
+def get_all_stair_type_ids_by_class(doc):
     """
-    Gets all Roof element type ids available in model.
+    Gets all Stair element type ids available in model.
+
+    Ignores in place families of category stair.
 
-    :param doc: _description_
-    :type doc: _type_
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids of roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids representing stair types.
+    :rtype: list of Autodesk.Revit.DB.ElementId
     """
 
     ids = []
-    col_class = get_all_roof_types_by_class(doc)
+    col_class = get_all_stair_types_by_class(doc)
     ids = com.get_ids_from_element_collector(col_class)
     return ids
 
 
-# -------------------------------- In place Roof types -------------------------------------------------------
+# -------------------------------- In place Stair types -------------------------------------------------------
 
 
-def get_in_place_roof_family_instances(doc):
+def get_in_place_stair_family_instances(doc):
     """
-    Gets all instances of in place families of category roof in the model.
+    Gets all instances in place families of category stair.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing roof family instances.
+    :return: A filtered element collector containing in place stair family instances.
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
-    filter = rdb.ElementCategoryFilter(rdb.BuiltInCategory.OST_Roofs)
+    filter = rdb.ElementCategoryFilter(rdb.BuiltInCategory.OST_Stairs)
     return (
         rdb.FilteredElementCollector(doc)
         .OfClass(rdb.FamilyInstance)
         .WherePasses(filter)
     )
 
 
-def get_all_in_place_roof_type_ids(doc):
+def get_all_in_place_stair_type_ids(doc):
     """
-    Gets type ids off all available in place families of category roof in the model.
+    Gets all type ids off all available in place families of category stair.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids of in place roof types.
-    :rtype: List Autodesk.Revit.DB.ElementId
+    :return: List of element ids
+    :rtype: list of Autodesk.Revit.ElementIds
     """
 
     ids = rFam.get_all_in_place_type_ids_in_model_of_category(
-        doc, rdb.BuiltInCategory.OST_Roofs
+        doc, rdb.BuiltInCategory.OST_Stairs
     )
     return ids
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Rooms/Export/to_data_room.py` & `DuHast-0.1.3/src/duHast/Revit/Rooms/Export/to_data_room.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Rooms/Geometry/geometry.py` & `DuHast-0.1.3/src/duHast/Revit/Rooms/Geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Rooms/room_functions.py` & `DuHast-0.1.3/src/duHast/Revit/Rooms/room_functions.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Rooms/room_tags.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit rooms tags. 
+This module contains a number of helper functions relating to sorting Revit stairs by types. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -15,66 +15,63 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from Autodesk.Revit.DB import Element, Transaction
-from duHast.Revit.Common.transaction import in_transaction
-from duHast.Utilities.Objects import result as res
 
+from duHast.Revit.Stairs.Utility import stairs_filter as rStairFilter
 
-def move_tag_to_room(doc, tag_id, transaction_manager=in_transaction):
+
+def build_stair_type_dictionary(collector, dic):
+    """
+    Amends dictionary past in with keys and or values added retrieved from collector past in.
+
+    Key values are as per BUILTIN_STAIR_TYPE_FAMILY_NAMES.
+
+    :param collector: A filtered element collector containing Stair type elements.
+    :type collector: Autodesk.Revit.DB.FilteredElementCollector
+    :param dic: A dictionary containing key: stair type family name, value: list of ids.
+    :type dic: dic { str: [Autodesk.Revit.DB.ElementId]}
+
+    :return: A dictionary containing key: stair type family name, value: list of ids.
+    :rtype: dic { str: [Autodesk.Revit.DB.ElementId]}
     """
-    Moves a room tag to the associated rooms location point.
+
+    for c in collector:
+        if dic.has_key(c.FamilyName):
+            if c.Id not in dic[c.FamilyName]:
+                dic[c.FamilyName].append(c.Id)
+        else:
+            dic[c.FamilyName] = [c.Id]
+    return dic
+
+
+def sort_stair_types_by_family_name(doc):
+    """
+    Returns a dictionary containing all stair types in the model.
+
+    Key values are as per BUILTIN_STAIR_TYPE_FAMILY_NAMES.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param tag_id: The element id of the tag to be moved to the room.
-    :type tag_id: Autodesk.Revit.DB.ElementId
-    :param transaction_manager: The transaction manager used to perform the modifications.
-    :type transaction_manager: (function)
-    :return: Result class instance.
-
-        - Tag moving status returned in result.status. False if an exception occurred, otherwise True.
-        - result.message will contain the name and number of the room.
-
-        On exception (handled by optimizer itself!):
-
-        - result.status (bool) will be False.
-        - result.message will contain the name and number of the room and the exception message.
-        
-    :rtype: :class:`.Result`
+
+    :return: A dictionary containing key: stair type family name, value: list of ids.
+    :rtype: dic { str: [Autodesk.Revit.DB.ElementId]}
     """
 
-    return_value = res.Result()
-    rt = doc.GetElement(tag_id)
-    room_tag_point = rt.Location.Point
-    room_location_point = rt.Room.Location.Point
-    room_data = "{} {}".format(rt.Room.Number, Element.Name.GetValue(rt.Room))
-    translation = room_location_point - room_tag_point
-
-    def action():
-        action_return_value = res.Result()
-        try:
-            rt.Location.Move(translation)
-            action_return_value.message = "Moved tag to room: {}".format(room_data)
-        except Exception as e:
-            action_return_value.update_sep(
-                False,
-                "Failed to move tag to room: {} with exception: {}".format(
-                    room_data, e
-                ),
-            )
-        return action_return_value
-
-    transaction = Transaction(doc, "Moving room tag to room : {}".format(room_data))
-    return_value.update(transaction_manager(transaction, action))
-    return return_value
+    # get all Stair Type Elements
+    wts = rStairFilter._get_stair_types_by_class(doc)
+    # get all stair types including in place stair families
+    wts_two = rStairFilter._get_all_stair_types_by_category(doc)
+    used_wts = {}
+    used_wts = build_stair_type_dictionary(wts, used_wts)
+    used_wts = build_stair_type_dictionary(wts_two, used_wts)
+    return used_wts
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Rooms/rooms.py` & `DuHast-0.1.3/src/duHast/Revit/Rooms/rooms.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/Reporting/shared_parameter_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_add.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_add.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 # custom result class
 from duHast.Utilities.Objects import result as res
 
 # import InTransaction from common module
 from duHast.Revit.Common import transaction as rTran
 
 
-def load_shared_parameter_file(doc, path):
+def load_shared_parameter_file(doc, path=None):
     """
     Loads a shared parameter file.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param path: Fully qualified file path to shared parameter text file.
+    :param path: (Optional) Fully qualified file path to shared parameter text file.
     :type path: str
 
     :return: The opened shared parameter file.
     :rtype: Autodesk.Revit.DB.DefinitionFile
     """
 
     app = doc.Application
-    app.SharedParametersFilename = path
+    if path:
+        app.SharedParametersFilename = path
+
     return app.OpenSharedParameterFile()
 
 
 def bind_shared_parameter(
     doc,
     category,
     parameter_name,
@@ -83,20 +85,18 @@
         - result.message will contain exception message.
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
-
         app = doc.Application
 
         # check if we are going to get something valid:
         if doc.Settings.Categories.get_Item(category) != None:
-
             # This is needed already here to
             # store old ones for re-inserting
             cat_set = app.Create.NewCategorySet()
 
             # Loop all Binding Definitions
             # IMPORTANT NOTE: Categories.Size is ALWAYS 1 !?
             # For multiple categories, there is really one
@@ -282,14 +282,15 @@
         for group in def_file.Groups:
             # loop through para's within definition group
             for def_para in group.Definitions:
                 # check whether this is the parameter we are after
                 if def_para.Name != para.name:
                     # jump to next parameter
                     continue
+
                 # set up an action to add parameter
                 def action():
                     action_return_value = res.Result()
                     try:
                         # add parameter depending on name, parameter group and isInstance
                         fam_para = mgr.AddParameter(
                             def_para, para.builtInParameterGroup, para.isInstance
@@ -325,7 +326,76 @@
     if found_para == False:
         return_value.status = False
         return_value.message = (
             para.name + " : No match for parameter found in shared parameter file."
         )
 
     return return_value
+
+
+def bind_shared_parameters_to_new_category(
+    rvt_doc, target_params, target_cat, target_param_grp, type_binding=False
+):
+    """
+    Takes a list of shared parameter definitions and creates a binding to a new category. Will
+    add category to an existing binding if one exists already
+    :param rvt_doc: Revit document
+    :type rvt_doc: Autodesk.Revit.DB.Document
+    :param target_params: List of shared parameter definitions
+    :type target_params: list[Autodesk.Revit.DB.ExternalDefinition]
+    :param target_cat: Category to bind to
+    :type target_cat: BuiltInCategory
+    :param target_param_grp: Parameter Group new parameters will appear in
+    :type target_param_grp: BuiltInParameterGroup
+    :param type_binding: True if type binding, False if instance binding
+    :type type_binding: bool
+    :return: List of successful bindings, list of errors
+    :rtype: tuple
+    """
+    new_cat_set = rvt_doc.Application.Create.NewCategorySet()
+    new_cat_set.Insert(target_cat)
+    if type_binding:
+        new_binding = rvt_doc.Application.Create.NewTypeBinding(new_cat_set)
+    else:
+        new_binding = rvt_doc.Application.Create.NewInstanceBinding(new_cat_set)
+    binding_map = rvt_doc.ParameterBindings
+    target_cat_name = rdb.Category.GetCategory(rvt_doc, target_cat.Id).Name
+
+    outlist = []
+    errors = []
+
+    t = rdb.Transaction(rvt_doc, "Bind new category to shared parameters")
+    t.Start()
+
+    for sp_def in target_params:
+        ex_binding = binding_map.Item[sp_def]
+        if ex_binding:
+            ex_binding_cats = [cat.Name for cat in ex_binding.Categories]
+            if target_cat_name in ex_binding_cats:
+                outlist.append(
+                    "{} already bound to {}".format(sp_def.Name, target_cat_name)
+                )
+                continue
+            try:
+                ex_binding.Categories.Insert(target_cat)
+                rvt_doc.ParameterBindings.ReInsert(sp_def, ex_binding)
+                outlist.append("Bound {} to {}".format(sp_def.Name, target_cat.Name))
+            except:
+                errors.append(
+                    "Could add {} to existing binding for {}".format(
+                        target_cat.Name, sp_def.Name
+                    )
+                )
+        else:
+            try:
+                binding_map.Insert(sp_def, new_binding, target_param_grp)
+                outlist.append("Bound {} to {}".format(sp_def.Name, target_cat.Name))
+            except:
+                errors.append(
+                    "Could not add {} to new binding for {}".format(
+                        target_cat.Name, sp_def.Name
+                    )
+                )
+
+    t.Commit()
+
+    return outlist, errors
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_data.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/Data/Objects/shared_parameter_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 from duHast.Utilities import utility as util
 from duHast.Revit.SharedParameters import shared_parameters as rSharedPara
 
 # import Autodesk
 import Autodesk.Revit.DB as rdb
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_swap.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_swap.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,38 +23,39 @@
 
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import System
 
 # import common library modules
 # from duHast.APISamples.Common import RevitCommonAPI as com
 from duHast.Utilities.Objects import result as res
 from duHast.Utilities import files_csv as fileCSV
+from duHast.Utilities.files_io import file_exist
 from duHast.Revit.SharedParameters import shared_parameter_add as rSharedPAdd
 from duHast.Revit.SharedParameters import shared_parameters_tuple as rSharedT
 from duHast.Revit.Common import parameter_grouping as rPG
 from duHast.Revit.SharedParameters import shared_parameters as rSharedPara
 from duHast.Revit.SharedParameters import shared_parameters_delete as rSharedParaDelete
 from duHast.Revit.SharedParameters import (
     shared_parameter_type_change as rSharedTypeChange,
@@ -120,81 +121,93 @@
         - result.message will contain exception message.
 
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     _parameter_prefix_ = "_dummy_"
+
+    # check if file exists
+    if(file_exist(change_directive_file_path) == False):
+        return_value.update_sep(False, "Change directive file does not exist: {}".format(change_directive_file_path))
+        return return_value
+    
     # load change directive
     parameter_directives = _load_shared_parameter_data_from_file(
         change_directive_file_path
     )
-    if len(parameter_directives) > 0:
-        # loop over directive and
-        for p_directive in parameter_directives:
-            # load shared para file
-            shared_para_def_file = rSharedPAdd.load_shared_parameter_file(
-                doc, parameter_directives[p_directive].sharedParameterPath
+
+    # check if there are any directives
+    if len(parameter_directives) == 0:
+        return_value.update_sep(False, "No parameter directives in file.")
+        return return_value
+    
+    
+    # loop over directive and
+    for p_directive in parameter_directives:
+        # load shared para file
+        shared_para_def_file = rSharedPAdd.load_shared_parameter_file(
+            doc, parameter_directives[p_directive].sharedParameterPath
+        )
+        return_value.append_message(
+            "Read shared parameter file: {}".format(
+                parameter_directives[p_directive].sharedParameterPath
             )
-            return_value.append_message(
-                "Read shared parameter file: {}".format(
-                    parameter_directives[p_directive].sharedParameterPath
+        )
+
+        if shared_para_def_file != None:
+            #   - swap shared parameter to family parameter
+            status_change_to_fam_para = (
+                rSharedTypeChange.change_shared_parameter_to_family_parameter(
+                    doc, p_directive, _parameter_prefix_
                 )
             )
-            if shared_para_def_file != None:
-                #   - swap shared parameter to family parameter
-                status_change_to_fam_para = (
-                    rSharedTypeChange.change_shared_parameter_to_family_parameter(
-                        doc, p_directive, _parameter_prefix_
+            return_value.update(status_change_to_fam_para)
+            if status_change_to_fam_para.status:
+                #   - delete all shared parameter definition
+                status_delete_old_shared_para_def = (
+                    rSharedParaDelete.delete_shared_parameter_by_name(
+                        doc, p_directive
                     )
                 )
-                return_value.update(status_change_to_fam_para)
-                if status_change_to_fam_para.status:
-                    #   - delete all shared parameter definition
-                    status_delete_old_shared_para_def = (
-                        rSharedParaDelete.delete_shared_parameter_by_name(
-                            doc, p_directive
-                        )
+                return_value.update(status_delete_old_shared_para_def)
+                if status_delete_old_shared_para_def.status:
+                    # get shared parameter definition
+                    s_para_def = rSharedPara.get_shared_parameter_definition(
+                        parameter_directives[p_directive].newParameterData.name,
+                        shared_para_def_file,
                     )
-                    return_value.update(status_delete_old_shared_para_def)
-                    if status_delete_old_shared_para_def.status:
-                        # get shared parameter definition
-                        s_para_def = rSharedPara.get_shared_parameter_definition(
-                            parameter_directives[p_directive].newParameterData.name,
-                            shared_para_def_file,
-                        )
-                        #   - add new shared parameter
-                        if s_para_def != None:
-                            return_value.append_message(
-                                "Retrieved shared parameter definition for: {}".format(
-                                    parameter_directives[
-                                        p_directive
-                                    ].newParameterData.name
-                                )
-                            )
-                            #   - swap family parameter to shared parameter
-                            status_swap_fam_to_shared_p = rSharedTypeChange.change_family_parameter_to_shared_parameter(
-                                doc,
-                                _parameter_prefix_ + p_directive,  # add prefix
-                                parameter_directives[p_directive].newParameterData,
-                                s_para_def,
-                            )
-                            return_value.update(status_swap_fam_to_shared_p)
-                        else:
-                            return_value.update_sep(
-                                False,
-                                "Failed to get shared parameter definition from file.",
+                    #   - add new shared parameter
+                    if s_para_def != None:
+                        return_value.append_message(
+                            "Retrieved shared parameter definition for: {}".format(
+                                parameter_directives[
+                                    p_directive
+                                ].newParameterData.name
                             )
+                        )
+                        #   - swap family parameter to shared parameter
+                        status_swap_fam_to_shared_p = rSharedTypeChange.change_family_parameter_to_shared_parameter(
+                            doc,
+                            _parameter_prefix_ + p_directive,  # add prefix
+                            parameter_directives[p_directive].newParameterData,
+                            s_para_def,
+                        )
+                        return_value.update(status_swap_fam_to_shared_p)
                     else:
-                        return_value.update(status_delete_old_shared_para_def)
+                        return_value.update_sep(
+                            False,
+                            "Failed to get shared parameter definition from file.",
+                        )
                 else:
-                    return_value.update(status_change_to_fam_para)
+                    return_value.update(status_delete_old_shared_para_def)
             else:
-                return_value.update_sep(
-                    False,
-                    "Failed to load shared parameter def file from: "
-                    + parameter_directives[p_directive].sharedParameterPath,
-                )
-    else:
-        return_value.status = False
-        return_value.message = "No change directives in file."
+                return_value.update(status_change_to_fam_para)
+        else:
+            return_value.update_sep(
+                False,
+                "Failed to load shared parameter def file from: {}".format(
+                    parameter_directives[p_directive].sharedParameterPath
+                ),
+            )
+
     return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameter_type_change.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameters.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import System
 
 # import common library modules
 from duHast.Revit.Common.revit_version import get_revit_version_number
+from duHast.Revit.SharedParameters.shared_parameter_add import (
+    load_shared_parameter_file,
+)
 
 # import Autodesk
 import Autodesk.Revit.DB as rdb
 
-
 # --------------------------------------------- utility functions ------------------
 
 
 def get_all_shared_parameters(doc):
     """
     Gets all shared parameters in a model
 
@@ -50,14 +52,40 @@
     :rtype: Autodesk.Revit.DB.FilteredElementCollector
     """
 
     collector = rdb.FilteredElementCollector(doc).OfClass(rdb.SharedParameterElement)
     return collector
 
 
+def get_all_shared_parameters_from_file(rvt_doc, shared_param_file_path=None):
+    """
+    Gets all the shared parameter definitions from a shared parameter file. Can
+    either be set manually or will be loaded from the default location which Revit
+    is pointing at
+    :param rvt_doc: Current Revit model document.
+    :type rvt_doc: Autodesk.Revit.DB.Document
+    :param shared_param_file_path: (Optional) The path to the shared parameter file.
+    :type shared_param_file_path: str
+    :return: A flat list of shared parameter definitions
+    :rtype: list
+    """
+    def_file = load_shared_parameter_file(rvt_doc, shared_param_file_path)
+    shared_params = []
+
+    if def_file:
+        sp_groups = def_file.Groups
+        for sp_gp in sp_groups:
+            for sp_def in sp_gp.Definitions:
+                shared_params.append(sp_def)
+
+        return shared_params
+    else:
+        return None
+
+
 def get_family_shared_parameters(doc):
     """
     Gets all family parameters which are shared parameters.
 
     :param doc: Current Revit family document.
     :type doc: Autodesk.Revit.DB.Document
     :raises Exception: "Document is not a family document." when a non family document is past in.
@@ -116,20 +144,20 @@
     :param parameter_gui_ds: list of shared parameter GUIDs as string values
     :type parameter_gui_ds: list str
 
     :return: list of shared parameter GUIDs as string values
     :rtype: list str
     """
 
-    filtered_gui_ds = []
+    filtered_guids = []
     paras = get_all_shared_parameters(doc)
     for p in paras:
         if p.GuidValue.ToString() in parameter_gui_ds:
-            filtered_gui_ds.append(p.GuidValue.ToString())
-    return filtered_gui_ds
+            filtered_guids.append(p.GuidValue.ToString())
+    return filtered_guids
 
 
 def check_whether_shared_parameters_by_name_is_family_parameter(doc, parameter_name):
     """
     Checks, by name, whether a shared parameter exists as a family parameter in a family.
 
     param doc: Current Revit family document.
@@ -142,15 +170,15 @@
     """
 
     para = None
     paras = get_family_parameters(doc)
     for fam_para in paras:
         if fam_para.Definition.Name == parameter_name:
             try:
-                # only shared parameters hav .GUID property...
+                # only shared parameters have .GUID property...
                 if str(fam_para.GUID) != "":
                     para = fam_para
                     break
             except Exception as e:
                 pass
     return para
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/SharedParameters/shared_parameters_delete.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,20 @@
             break
     if len(delete_ids) > 0:
         return_value = rDel.delete_by_element_ids(
             doc, delete_ids, "Delete Shared Parameter", parameter_name
         )
     else:
         return_value.update_sep(
-            False, "parameter with guid: " + guid + " does not exist in file."
+            False, "parameter with guid: {} does not exist in file.".format(guid)
         )
     return return_value
 
 
-def delete_shared_parameters(doc, parameter_gui_ds):
+def delete_shared_parameters(doc, parameter_guids):
     """
     Deletes shared parameters by GUID from document.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :param parameter_gui_ds: List of shared parameter GUIDs as string.
     :type parameter_gui_ds: list str
@@ -147,17 +147,17 @@
         - result.message will contain generic exception message.
         
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     one_got_deleted = False
-    delete_gui_ds = check_whether_shared_parameters_are_in_file(doc, parameter_gui_ds)
-    if len(delete_gui_ds) > 0:
-        for delete_guid in delete_gui_ds:
+    delete_guids = check_whether_shared_parameters_are_in_file(doc, parameter_guids)
+    if len(delete_guids) > 0:
+        for delete_guid in delete_guids:
             delete_status = delete_shared_parameter_by_guid(doc, delete_guid)
             # preserve TRUE value!
             if delete_status.status == True:
                 one_got_deleted = True
             return_value.update(delete_status)
         return_value.update_sep(one_got_deleted, "Finished deleting parameters!")
     else:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/Reporting/stairs_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/stairs_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/Utility/stairs_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 # import Autodesk
 import Autodesk.Revit.DB as rdb
 import Autodesk.Revit.DB.Architecture as rdbA
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/Utility/stairs_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Floors/Utility/floors_type_sorting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to sorting Revit stairs by types. 
+This module contains a Revit floor utility functions. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,56 +22,51 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
+from duHast.Revit.Floors.Utility import floors_filter as rFloorsFilter
 
-from duHast.Revit.Stairs.Utility import stairs_filter as rStairFilter
 
-
-def build_stair_type_dictionary(collector, dic):
+def build_floor_type_dictionary(collector, dic):
     """
-    Amends dictionary past in with keys and or values added retrieved from collector past in.
-
-    Key values are as per BUILTIN_STAIR_TYPE_FAMILY_NAMES.
-
-    :param collector: A filtered element collector containing Stair type elements.
+    Returns the dictionary past in with keys and or values added retrieved from collector past in.
+    Keys are built in floor family type names.
+    TODO: This code repeats across a number of modules. Use generic instead!
+    :param collector: A filtered element collector containing floor types.
     :type collector: Autodesk.Revit.DB.FilteredElementCollector
-    :param dic: A dictionary containing key: stair type family name, value: list of ids.
-    :type dic: dic { str: [Autodesk.Revit.DB.ElementId]}
-
-    :return: A dictionary containing key: stair type family name, value: list of ids.
-    :rtype: dic { str: [Autodesk.Revit.DB.ElementId]}
+    :param dic: A dictionary containing key: floor type family name, value: list of ids belonging to that type.
+    :type dic: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
+    :return: A dictionary containing key: built in floor type family name, value: list of ids belonging to that type.
+    :rtype: dictionary (key str, value list of Autodesk.Revit.DB.ElementId)
     """
 
     for c in collector:
         if dic.has_key(c.FamilyName):
             if c.Id not in dic[c.FamilyName]:
                 dic[c.FamilyName].append(c.Id)
         else:
             dic[c.FamilyName] = [c.Id]
     return dic
 
 
-def sort_stair_types_by_family_name(doc):
+def sort_floor_types_by_family_name(doc):
     """
-    Returns a dictionary containing all stair types in the model.
-
-    Key values are as per BUILTIN_STAIR_TYPE_FAMILY_NAMES.
-
+    Returns a dictionary containing all floor types in the model.
+    Key values are as per BUILTIN_FLOOR_TYPE_FAMILY_NAMES.
+    TODO: This code repeats across a number of modules. Use generic instead!
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-
-    :return: A dictionary containing key: stair type family name, value: list of ids.
+    :return: A dictionary containing key: floor type family name, value: list of ids.
     :rtype: dic { str: [Autodesk.Revit.DB.ElementId]}
     """
 
-    # get all Stair Type Elements
-    wts = rStairFilter._get_stair_types_by_class(doc)
-    # get all stair types including in place stair families
-    wts_two = rStairFilter._get_all_stair_types_by_category(doc)
+    # get all floor Type Elements
+    wts = rFloorsFilter._get_floor_types_by_class(doc)
+    # get all floor types including in place floor families
+    wts_two = rFloorsFilter._get_all_floor_types_by_category(doc)
     used_wts = {}
-    used_wts = build_stair_type_dictionary(wts, used_wts)
-    used_wts = build_stair_type_dictionary(wts_two, used_wts)
+    used_wts = build_floor_type_dictionary(wts, used_wts)
+    used_wts = build_floor_type_dictionary(wts_two, used_wts)
     return used_wts
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/cut_marks.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/cut_marks.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import Autodesk.Revit.DB as rdb
 import Autodesk.Revit.DB.Architecture as rdbA
 
 from duHast.Revit.Common import common as com
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/purge_unused_stair_types.py` & `DuHast-0.1.3/src/duHast/Revit/Stairs/purge_unused_stair_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from duHast.Revit.Family import purge_unused_family_types as rFamPurge
 from duHast.Revit.Common import purge_utils as rPurgeUtils
 from duHast.Revit.Common import parameter_get_utils as rParaGet
 from duHast.Revit.Stairs import stairs as rStair
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Stairs/stairs.py` & `DuHast-0.1.3/src/duHast/Revit/ModelHealth/Reporting/Properties/view.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,201 +1,195 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit stairs. 
+Model health report functions - views.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Model health report metrics can either be displayed in a family where each parameter is assigned to a metric 
+and or data can be exported to text files which can be used to visualize key metrics over time.
+
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
-import System
 
-from duHast.Revit.Common import common as com
-from duHast.Revit.Family import family_utils as rFam
-from duHast.Revit.Stairs.Utility import stairs_filter as rStairsFilter
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
-import Autodesk.Revit.DB.Architecture as rdbA
+import System
 
+clr.AddReference("System.Core")
+from System import Linq
 
-def get_all_stair_types_by_category(doc):
-    """
-    Gets a filtered element collector of all Stair types in the model.
+clr.ImportExtensions(Linq)
 
-    Return includes:
-    - Stair
-    - Assembled Stair
-    - Precast Stair
-    - Cast-In-Place Stair
-    - In place families or loaded families
 
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-
-    :return: A filtered element collector containing stair types.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
-    """
+from duHast.Revit.ModelHealth.Reporting.Properties.constants import (
+    FAILED_TO_RETRIEVE_VALUE,
+)
+from duHast.Revit.Views.sheets import get_all_sheets
+from duHast.Revit.Views.views import get_views_in_model, get_views_not_on_sheet
+from duHast.Revit.Views.templates import (
+    get_view_templates_ids,
+    get_all_unused_view_template_ids,
+)
+from duHast.Revit.Views.filters import get_all_filters, get_all_unused_view_filters
 
-    collector = rStairsFilter._get_all_stair_types_by_category(doc)
-    return collector
+# --------------------------------------------- VIEWS ---------------------------------------------
 
 
-def get_all_stair_types_by_class(doc):
+def get_number_of_sheets(doc):
     """
-    Gets a filtered element collector of all Stair types in the model.
-
-    Return includes:
-
-    - Assembled Stair
-    - Precast Stair
-    - Cast-In-Place Stair
-
-    It will not return any in place family or Stair types! These are internally treated as Families or Family Symbols class objects.
+    Gets the number of sheets in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing stair types.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: Number of sheets in model. On exception it will return -1
+    :rtype: int
     """
 
-    collector = rStairsFilter._get_stair_types_by_class(doc)
-    return collector
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_all_sheets(doc).ToList())
+    except Exception as e:
+        raise ValueError("Failed to get number of sheets: {}".format(e))
+    return number
 
 
-# -------------------------------- none in place Stair types -------------------------------------------------------
+def _view_filter(view):
+    """
+    generic view filter allowing all views to be selected
 
+    :param view: not used!
+    :type view: Autodesk.Revit.DB.View
 
-def get_all_stair_instances_by_category(doc):
+    :return: returns always True
+    :rtype: bool
     """
-    Gets a filtered element collector of all Stair elements placed in model.
+    return True
+
 
-    TODO: Confirm it  ignores in place families?
+def get_number_of_views(doc):
+    """
+    Gets the number of views in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing stair instances.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: Number of views in model. On exception it will return -1
+    :rtype: int
     """
-
-    return (
-        rdb.FilteredElementCollector(doc)
-        .OfCategory(rdb.BuiltInCategory.OST_Stairs)
-        .WhereElementIsNotElementType()
-    )
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_views_in_model(doc, _view_filter))
+    except Exception as e:
+        raise ValueError("Failed to get number of views: {}".format(e))
+    return number
 
 
-def get_all_stair_instances_by_class(doc):
+def get_number_of_unplaced_views(doc):
     """
-    Gets a filtered element collection all Stair elements placed in model...
-
-    TODO: Confirm it ignores Stair soffits.
+    Gets the number of unplaced views in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing stair instances.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: Number of unplaced views in model. On exception it will return -1
+    :rtype: int
     """
-
-    return (
-        rdb.FilteredElementCollector(doc)
-        .OfClass(rdbA.Stairs)
-        .WhereElementIsNotElementType()
-    )
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_views_not_on_sheet(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of unplaced views: {}".format(e))
+    return number
 
 
-def get_all_stair_type_ids_by_category(doc):
+def get_number_of_view_templates(doc):
     """
-    Gets all Stair element type ids available in model.
+    Gets the number of view templates in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids representing stair types.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: Number of view templates in model. On exception it will return -1
+    :rtype: int
     """
-
-    ids = []
-    col_cat = get_all_stair_types_by_category(doc)
-    ids = com.get_ids_from_element_collector(col_cat)
-    return ids
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_view_templates_ids(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of view templates: {}".format(e))
+    return number
 
 
-def get_all_stair_type_ids_by_class(doc):
+def get_number_of_unused_view_templates(doc):
     """
-    Gets all Stair element type ids available in model.
-
-    Ignores in place families of category stair.
+    Gets the number of unplaced view templates in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids representing stair types.
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: Number of unplaced view templates in model. On exception it will return -1
+    :rtype: int
     """
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_all_unused_view_template_ids(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of unused view templates: {}".format(e))
+    return number
 
-    ids = []
-    col_class = get_all_stair_types_by_class(doc)
-    ids = com.get_ids_from_element_collector(col_class)
-    return ids
-
-
-# -------------------------------- In place Stair types -------------------------------------------------------
 
-
-def get_in_place_stair_family_instances(doc):
+def get_number_of_view_filters(doc):
     """
-    Gets all instances in place families of category stair.
+    Gets the number of view filters in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: A filtered element collector containing in place stair family instances.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
+    :return: Number of number of view filters in model. On exception it will return -1
+    :rtype: int
     """
-
-    filter = rdb.ElementCategoryFilter(rdb.BuiltInCategory.OST_Stairs)
-    return (
-        rdb.FilteredElementCollector(doc)
-        .OfClass(rdb.FamilyInstance)
-        .WherePasses(filter)
-    )
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_all_filters(doc).ToList())
+    except Exception as e:
+        raise ValueError("Failed to get number of view filters: {}".format(e))
+    return number
 
 
-def get_all_in_place_stair_type_ids(doc):
+def get_number_of_unused_view_filters(doc):
     """
-    Gets all type ids off all available in place families of category stair.
+    Gets the number of unused view filters in the model.
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: List of element ids
-    :rtype: list of Autodesk.Revit.ElementIds
+    :return: Number of unused view filters in model. On exception it will return -1
+    :rtype: int
     """
-
-    ids = rFam.get_all_in_place_type_ids_in_model_of_category(
-        doc, rdb.BuiltInCategory.OST_Stairs
-    )
-    return ids
+    number = FAILED_TO_RETRIEVE_VALUE
+    try:
+        number = len(get_all_unused_view_filters(doc))
+    except Exception as e:
+        raise ValueError("Failed to get number of unused view filters: {}".format(e))
+    return number
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Geometry/view_geometry.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Geometry/view_geometry.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 clr.AddReference("System.Core")
 from System import Linq
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_base.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_category.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_category.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_by_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_by_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_cut.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_cut.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/Data/override_projection.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/Data/override_projection.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/category_override_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/category_override_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/filter_override_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/filter_override_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Objects/view_graphics_settings.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Objects/view_graphics_settings.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/Objects/json_conversion_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/Objects/json_conversion_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/schedules_report.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/schedules_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param file_name: The fully qualified file path of the report file.
     :type file_name: str
     :param current_file_name: The current revit file name which will be appended to data in the report.
     :type current_file_name: str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_schedules_report_data(doc, current_file_name)
@@ -165,15 +165,15 @@
     :type file_name: str
     :param current_file_name: The current Revit file name which will be appended to data in the report.
     :type current_file_name: str
     :param sheet_properties: List of sheet properties to be extracted from sheets.
     :type sheet_properties: list of str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_schedules_report_data_filtered(
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/sheets_report.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/sheets_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param file_name: The fully qualified file path of the report file.
     :type file_name: str
     :param current_file_name: The current revit file name which will be appended to data in the report.
     :type current_file_name: str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_sheet_report_data(doc, current_file_name)
@@ -151,15 +151,15 @@
     :type file_name: str
     :param current_file_name: The current Revit file name which will be appended to data in the report.
     :type current_file_name: str
     :param sheet_properties: List of sheet properties to be extracted from sheets.
     :type sheet_properties: list of str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_sheets_report_data_filtered(doc, current_file_name, sheet_properties)
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_property_filter.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_property_filter.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_property_utils.py` & `DuHast-0.1.3/src/duHast/Revit/SharedParameters/shared_parameters_tuple.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains the view property utilities.
+This module contains a tuple used to store settings retrieved from a file.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -22,30 +22,12 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
+from collections import namedtuple
 
-def convert_view_data_to_list(view_data, headers):
-    """
-    Converts a list of dictionaries of view properties names and values to a list of properties only.
 
-    :param view_data: List of dictionaries representing view properties
-    :type view_data: [{}]
-    :param headers: list of properties
-    :type headers: [str]
-    :return: A list of lists of view property values.
-    :rtype: [[str]]
-    """
-
-    data = []
-    for view_d in view_data:
-        data_row = []
-        for header in headers:
-            if header in view_d:
-                data_row.append(view_d[header])
-            else:
-                data_row.append("Property does not exist on element.")
-        data.append(data_row)
-    return data
+# tuples containing base family data read from file
+PARAMETER_DATA = namedtuple("parameterData", "name isInstance builtInParameterGroup")
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/view_reports_json_props.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/view_reports_json_props.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
     :return:
         Result class instance.
-        - .result = True if padded array was successfully assigned. Otherwise False.
+        - .status True if padded array was successfully assigned. Otherwise False.
         - .message will contain array size.
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
         call_back_progress_counter = 0
@@ -370,15 +370,15 @@
 
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
     :return:
         Result class instance.
-        - .result = True if row and column index pointers where successfully assigned. Otherwise False.
+        - .status True if row and column index pointers where successfully assigned. Otherwise False.
         - .message will contain array size.
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
         call_back_progress_counter = 0
@@ -450,15 +450,15 @@
 
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
     :return:
         Result class instance.
-        - .result = True if default arrays where successfully updated with values from file specific arrays. Otherwise False.
+        - .status True if default arrays where successfully updated with values from file specific arrays. Otherwise False.
         - .message will contain array size.
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
         call_back_progress_counter = 0
@@ -515,15 +515,15 @@
     """
     Combine 2D default hash arrays from all files into single 3D hash array.
 
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :return:
         Result class instance.
-        - .result = True if 3D array was successfully created. Otherwise False.
+        - .status True if 3D array was successfully created. Otherwise False.
         - .message will contain array size.
         -. result will contain the 3D array for categories as first value in list and the 3D array for filters as the second value in list
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
@@ -582,15 +582,15 @@
     :type model_names: [str]
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
     :return:
         Result class instance.
-        - .result = True if 3D array was successfully created. Otherwise False.
+        - .status True if 3D array was successfully created. Otherwise False.
         - .message will contain array size.
         -. result will contain the flatten array as first value in list
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
@@ -633,15 +633,15 @@
     :type model_names: [str]
     :param hash_data_by_file: A dictionary where key is the file name without extension and value is an instance of a custom storage object
     :type hash_data_by_file: {str: [:class:`.JSONThreeDStorage`]}
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
     :return:
         Result class instance.
-        - .result = True if 3D array was successfully created. Otherwise False.
+        - .status True if 3D array was successfully created. Otherwise False.
         - .message will contain array size.
         -. result will contain the flatten array as first value in list
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
@@ -677,15 +677,15 @@
     :param json_files: List of files containing view template data of Revit project files. ( One json file per Revit project file)
     :type json_files: [str]
     :param progress_call_back: A call back function accepting as arguments the number of the current file processed and the number of overall files to be processed, defaults to None
     :type progress_call_back: func(counter, overall_counter), optional
 
     :return:
         Result class instance.
-        - .result = True if flattened array was successfully created. Otherwise False.
+        - .status True if flattened array was successfully created. Otherwise False.
         - .message will contain array size.
         -. result will contain the flatten array as first value in list
     :rtype: :class:`.Result`
     """
 
     result = res.Result()
     try:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report_utilities.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_3d_hash_report_utilities.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_data_report.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_data_report.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_report.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param file_name: The fully qualified file path of the report file.
     :type file_name: str
     :param current_file_name: The current revit file name which will be appended to data in the report.
     :type current_file_name: str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_views_report_data(doc, current_file_name)
@@ -174,15 +174,15 @@
     :type file_name: str
     :param current_file_name: The current Revit file name which will be appended to data in the report.
     :type current_file_name: str
     :param sheet_properties: List of sheet properties to be extracted from sheets.
     :type sheet_properties: list of str
     :return:
         Result class instance.
-        - .result = True if data was written successfully. Otherwise False.
+        - .status True if data was written successfully. Otherwise False.
         - .message will contain write status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     try:
         data = get_views_report_data_filtered(doc, current_file_name, view_properties)
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Reporting/views_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Reporting/views_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_data_to_override_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_data_to_override_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_data_to_revit_override.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_data_to_revit_override.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/convert_revit_override_to_data.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/convert_revit_override_to_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 from duHast.Revit.Views.Objects.Data.override_by_filter import OverrideByFilter
 from duHast.Revit.Views.Objects.Data.override_projection import OverrideProjection
 from duHast.Revit.Views.Objects.Data.override_cut import OverrideCut
 from duHast.Revit.Common.Objects.Data.pattern_background import PatternBackground
 from duHast.Revit.Common.Objects.Data.pattern_foreground import PatternForeground
 from duHast.Revit.Common.Objects.Data.line_projection import LineProjection
 from duHast.Revit.Common.Objects.Data.line_cut import LineCut
-from duHast.Revit.LinePattern.Objects.Data.line_pattern_settings import (
+from duHast.Revit.LinePattern.Data.Objects.line_pattern_settings import (
     LinePatternSettings,
 )
-from duHast.Revit.LinePattern.Objects.Data.fill_pattern_settings import (
+from duHast.Revit.LinePattern.Data.Objects.fill_pattern_settings import (
     FillPatternSettings,
 )
 from duHast.Revit.Common.Objects.Data.pattern_settings_base import PatternSettingBase
 from duHast.Revit.Common.Utility.revit_to_data_conversion import (
     to_colour,
     VIEW_DETAIL_LEVEL_NAME_MAPPING,
 )
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/sheet_parameters.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/sheet_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,49 +33,51 @@
     """
     Get the sheet number of a sheet
     :param sht: The sheet to get the number of
     :type sht: ViewSheet
     :return: The sheet number
     :rtype: str
     """
+
     try:
         return sht.get_Parameter(BuiltInParameter.SHEET_NUMBER).AsString()
     except:
         return None
 
 
 def get_sheet_name(sht):
     """
     Get the sheet name of a sheet
     :param sht: The sheet to get the name of
     :type sht: ViewSheet
     :return: The sheet name
     :rtype: str
     """
+
     try:
         return sht.get_Parameter(BuiltInParameter.SHEET_NAME).AsString()
     except:
         return None
 
 
 def get_sheet_num_name_comb(sht, num_first=True, separator=" - "):
     """
     Get the sheet number and name of a sheet and returns the the combination
     of the two. Typically helpful for logging/printing.
 
     :type sht: ViewSheet
-    :param num_first: Whether the sheet number should be first in the string.
-    Defaults to True
+    :param num_first: Whether the sheet number should be first in the string. Defaults to True
     :type num_first: bool
-    :param splitter: The string to split the sheet number and name with. Defaults
-    to ' - '
+    :param splitter: The string to split the sheet number and name with. Defaults to ' - '
     :type splitter: str
     :return: The sheet number and name
     :rtype: str
+
     """
+
     num = get_sheet_number(sht)
     name = get_sheet_name(sht)
 
     if all([num, name]):
         if num_first:
             return num + separator + name
         else:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/view_parameters.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/view_parameters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/Utility/view_types.py` & `DuHast-0.1.3/src/duHast/Revit/Views/Utility/view_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import Autodesk.Revit.DB as rdb
 from System import Enum
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/delete.py` & `DuHast-0.1.3/src/duHast/Revit/Views/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     :type doc: Autodesk.Revit.DB.Document
     :param view_rules: A set of rules. If view matches rule it will be deleted.
     :type view_rules: array in format [parameter name, condition test method, value to test against
     :param collector_views: A filtered element collector containing view instances.
     :type collector_views: Autodesk.Revit.DB.FilteredElementCollector
     :return:
         Result class instance.
-        - .result = True if all sheets matching filter where deleted. Otherwise False.
+        - .status True if all sheets matching filter where deleted. Otherwise False.
         - .message will contain deletion status.
     :rtype: :class:`.Result`
     """
 
     ids = []
     for v in collector_views:
         if v.ViewType == rdb.ViewType.DrawingSheet:
@@ -196,15 +196,15 @@
     """
     Deletes all sheets in a model
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
     :return:
         Result class instance.
-        - .result = True if all sheets where deleted. Otherwise False.
+        - .status True if all sheets where deleted. Otherwise False.
         - .message will contain deletion status.
     :rtype: :class:`.Result`
     """
 
     return_value = res.Result()
     ids = []
     collector_sheets = rdb.FilteredElementCollector(doc).OfClass(rdb.View)
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/filters.py` & `DuHast-0.1.3/src/duHast/Revit/Views/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from Autodesk.Revit.DB import (
     Element,
     FilteredElementCollector,
     ParameterFilterElement,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/referencing.py` & `DuHast-0.1.3/src/duHast/Revit/Views/referencing.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 
 clr.AddReference("System.Core")
 from System import Linq
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/schedules.py` & `DuHast-0.1.3/src/duHast/Revit/Views/schedules.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/sheets.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/solver_duplicate_mark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit view sheets. 
+Duplicate mark warnings solver class.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -22,140 +24,131 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import clr
-
-import Autodesk.Revit.DB as rdb
-from duHast.Utilities import utility as util
-from duHast.Revit.Views.Utility.sheet_parameters import get_sheet_number
 from duHast.Revit.Common import parameter_get_utils as rParaGet
+from duHast.Revit.Common import parameter_set_utils as rParaSet
+from duHast.Utilities.Objects import result as res
 
-# required in lambda expressions!
-clr.AddReference("System.Core")
-import System
-
-clr.ImportExtensions(System.Linq)
-
-
-def get_sheets_by_filters(doc, view_rules=None):
-    """
-    Gets sheets matching filters provided
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :param view_rules: A set of rules. If sheet matches rule it will be returned. Defaults to None which will return all sheets.
-    :type view_rules: array in format [parameter name, condition test method, value to test against], optional
-    :return: Views matching filter
-    :rtype: list of Autodesk.Revit.DB.View
-    """
-
-    collector_views = rdb.FilteredElementCollector(doc).OfClass(rdb.ViewSheet)
-    views = []
-    for v in collector_views:
-        # if no filter rules applied return al sheets
-        if view_rules is not None:
-            paras = v.GetOrderedParameters()
-            rule_match = True
-            for para_name, paraCondition, conditionValue in view_rules:
-                for p in paras:
-                    if p.Definition.Name == para_name:
-                        rule_match = rule_match and rParaGet.check_parameter_value(
-                            p, paraCondition, conditionValue
-                        )
-            if rule_match == True:
-                # delete view
-                views.append(v)
-        else:
-            views.append(v)
-    return views
+
+# import Autodesk
+import Autodesk.Revit.DB as rdb
+from duHast.Utilities.Objects import base
 
 
-def get_all_sheets(doc):
-    """
-    Gets all sheets in a model
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: list of sheet views
-    :rtype: list of Autodesk.Revit.DB.View
-    """
-
-    collector_views = rdb.FilteredElementCollector(doc).OfClass(rdb.ViewSheet)
-    return collector_views
-
-
-def get_sheet_rev_by_sheet_number(doc, sheet_number):  # type # type: str
-    """
-    Returns the revision of a sheet identified by its number. Default value is '-'.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :param sheet_number: The number of the sheet of which the revision is to be returned.
-    :type sheet_number: str
-    :raise: Any exception will need to be managed by the function caller.
-
-    :return: The sheet's current revision value. If no matching sheet is found, '-' is returned.
-    :rtype: str
-    """
-
-    rev_value = "-"
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfClass(rdb.ViewSheet)
-        .Where(lambda e: e.SheetNumber == sheet_number)
-    )  # type
-    results = collector.ToList()
-    if len(results) > 0:
-        sheet = results[0]
-        rev_p = sheet.get_Parameter(rdb.BuiltInParameter.SHEET_CURRENT_REVISION)
-        rev_value = rev_p.AsString()
-    return rev_value
-
-
-def get_sheet_rev_by_sheet_name(doc, sheet_name):  # type # type: str
-    """
-    Returns the revision of a sheet identified by its name. Default value is '-'.
-
-    Since multiple sheets can have the same name, it will return the revision of the first sheet matching the name.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :param sheet_name: The name of the sheet of which the revision is to be returned.
-    :type sheet_name: str
-    :raise: Any exception will need to be managed by the function caller.
-
-    :return: The sheet's current revision value. If no matching sheet is found, '-' is returned.
-    :rtype: str
-    """
-
-    rev_value = "-"
-    collector = (
-        rdb.FilteredElementCollector(doc)
-        .OfClass(rdb.ViewSheet)
-        .Where(lambda e: e.Name == sheet_name)
-    )  # type
-    results = collector.ToList()
-    if len(results) > 0:
-        sheet = results[0]
-        rev_p = sheet.get_Parameter(rdb.BuiltInParameter.SHEET_CURRENT_REVISION)
-        rev_value = util.pad_single_digit_numeric_string(rev_p.AsString())
-    return rev_value
-
-
-def get_sheet_num_to_elem_dict(rvt_doc):
-    """
-    Get a dictionary of sheet numbers and sheets
-    :param rvt_doc: The Revit document to get the sheets from
-    :type rvt_doc: Document
-    :return: A dictionary of sheet numbers and sheets
-    :rtype: dict
-    """
-    num_elem_dict = {}
-    all_sheets = get_all_sheets(rvt_doc)
-
-    for sheet in all_sheets:
-        sht_num = get_sheet_number(sheet)
-        num_elem_dict[sht_num] = sheet
+class RevitWarningsSolverDuplicateMark(base.Base):
 
-    return num_elem_dict
+    def __init__(self, filter_func, filter_values=[]):
+        """
+        Constructor: this solver takes two arguments: a filter function and a list of values to filter by
+
+        :param filter_func: A function to filter elements in warnings by
+        :type filter_func: func(document, elementId, list of filter values)
+        :param filter_values: A list of filter values, defaults to []
+        :type filter_values: list, optional
+        """
+
+        # ini super class to allow multi inheritance in children!
+        super(RevitWarningsSolverDuplicateMark, self).__init__()
+
+        self.filter = filter_func
+        self.filter_values = filter_values
+        self.filter_name = "Duplicate mark value."
+
+    # --------------------------- duplicate mark guid ---------------------------
+    #: guid identifying this specific warning
+    GUID = "6e1efefe-c8e0-483d-8482-150b9f1da21a"
+
+    IGNORED_WARNINGS = ["Type Mark"]
+
+    def solve_warnings(self, doc, warnings):
+        """
+        Solver setting element mark to nothing, provided it passes the filter.
+
+        :param doc: Current Revit model document.
+        :type doc: Autodesk.Revit.DB.Document
+        :param warnings: List of warnings to be solved.
+        :type warnings: Autodesk.Revit.DB.FailureMessage
+
+        :return:
+            Result class instance.
+
+            - .status True if all duplicate mark warnings could be solved. Otherwise False.
+            - .message will contain stats in format parameter value set to ''
+
+        :rtype: :class:`.Result`
+        """
+
+        return_value = res.Result()
+        if len(warnings) > 0:
+            for warning in warnings:
+                # Flag to indicate if we should continue the outer loop
+                should_continue_outer = False
+                # check for any duplicate Type Mark warnings...which are not to be addressed!
+                for ignore in self.IGNORED_WARNINGS:
+                    if ignore in warning.GetDescriptionText():
+                        element_ids = warning.GetFailingElements()
+                        for el_id in element_ids:
+                            element = doc.GetElement(el_id)
+                            return_value.update_sep(
+                                True,
+                                "{} Warning of type: duplicate {}. {} will be ignored.".format(
+                                    self.filter_name,
+                                    rdb.Element.Name.GetValue(element),
+                                    ignore,
+                                ),
+                            )
+                        should_continue_outer = True
+                        break  # Break out of the inner loop
+                if should_continue_outer:
+                    continue  # Continue the outer loop
+                element_ids = warning.GetFailingElements()
+                for el_id in element_ids:
+                    element = doc.GetElement(el_id)
+                    # check whether element passes filter
+                    if self.filter(doc, el_id, self.filter_values):
+
+                        try:
+                            p_value = rParaGet.get_built_in_parameter_value(
+                                element, rdb.BuiltInParameter.ALL_MODEL_MARK
+                            )
+                            if p_value != None:
+                                result = rParaSet.set_built_in_parameter_value(
+                                    doc,
+                                    element,
+                                    rdb.BuiltInParameter.ALL_MODEL_MARK,
+                                    "",
+                                )
+                                return_value.update(result)
+                            else:
+                                return_value.update_sep(
+                                    True,
+                                    "{}:  Element has no mark value: {}".format(
+                                        self.filter_name,
+                                        rdb.Element.Name.GetValue(element),
+                                    ),
+                                )
+                        except Exception as e:
+                            return_value.update_sep(
+                                False,
+                                "{}: Failed to solve warning duplicate mark with exception: {}".format(
+                                    self.filter_name, e
+                                ),
+                            )
+                    else:
+                        return_value.update_sep(
+                            True,
+                            "{}: Element removed by filter: {}".format(
+                                self.filter_name, rdb.Element.Name.GetValue(element)
+                            ),
+                        )
+        else:
+            return_value.update_sep(
+                True,
+                "{}: No warnings of type: duplicate mark in model.".format(
+                    self.filter_name
+                ),
+            )
+        return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/templates.py` & `DuHast-0.1.3/src/duHast/Revit/Views/templates.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/views.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/warnings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of helper functions relating to Revit views. 
+This module contains a number of helper functions relating to Revit warnings. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
@@ -25,163 +25,129 @@
 #
 #
 #
 
 import clr
 import System
 
-# import common library modules
-from duHast.Revit.Common import common as com
-from duHast.Revit.Views.Utility.view_types import _get_view_types
-from duHast.Revit.Views.schedules import filter_revision_schedules
-from duHast.Revit.Views.sheets import get_all_sheets
+# -------------------------------------------- common variables --------------------
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
 
+# --------------------------------------------- utility functions ------------------
 
-def get_view_types(doc):
-    """
-    Returns all view family types in a model
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :return: A filtered element collector.
-    :rtype: Autodesk.Revit.DB.FilteredElementCollector
-    """
 
-    collector = _get_view_types(doc)
-    return collector
-
-
-def get_view_type_ids(doc):
+def get_warnings(doc):
     """
-    Returns all view family type ids in a model
+    Returns a list of warnings from the model
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
 
-    :return: ids of view family types
-    :rtype: list of Autodesk.Revit.DB.ElementId
+    :return: List of all failure messages in model.
+    :rtype: list of Autodesk.Revit.DB.FailureMessage
     """
 
-    ids = []
-    col = get_view_types(doc)
-    ids = com.get_ids_from_element_collector(col)
-    return ids
+    return doc.GetWarnings()
 
 
-def get_views_of_type(doc, view_type):
+def get_warnings_by_guid(doc, guid):
     """
-    Gets all views in a model of a given type. Excludes templates.
+    Returns all failure message objects where failure definition has matching GUID
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param view_type: Filter: the view type
-    :type view_type: Autodesk.Revit.DB.ViewType
+    :param guid: Filter: Identifying a specific failure of which the corresponding messages are to be returned.
+    :type guid: Autodesk.Revit.DB.Guid
 
-    :return: list of views
-    :rtype: list of Autodesk.Revit.DB.View
+    :return: list of all failure messages with matching guid
+    :rtype: list of Autodesk.Revit.DB.FailureMessage
     """
 
-    views = []
-    col = rdb.FilteredElementCollector(doc).OfClass(rdb.View)
-    for v in col:
-        if v.ViewType == view_type and v.IsTemplate == False:
-            views.append(v)
-    return views
-
+    filtered_warnings = []
+    warnings = doc.GetWarnings()
+    for warning in warnings:
+        if str(warning.GetFailureDefinitionId().Guid) == guid:
+            filtered_warnings.append(warning)
+    return filtered_warnings
 
-# ----------------------------------------------------------------------------------------
 
-
-def get_viewport_on_sheets(doc, sheets):
+def get_warnings_grouped_by_relation(doc, guid):
     """
-    Get all view ports on sheets provided.
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-    :param sheets: list of sheets of which to return the view ports from.
-    :type sheets: list of Autodesk.Revit.DB.ViewSheet
-
-    :return: list of view ports
-    :rtype: list of Autodesk.Revit.DB.Viewport
-    """
-
-    view_ports = []
-    for sheet in sheets:
-        try:
-            viewport_ids = sheet.GetAllViewports()
-            if viewport_ids != None:
-                for viewport_id in viewport_ids:
-                    viewport = doc.GetElement(viewport_id)
-                    view_ports.append(viewport)
-        except Exception as e:
-            print("Get view ports on sheet: {} threw exception: {}".format(sheet, e))
-    return view_ports
-
-
-def get_views_in_model(doc, filter):
-    """
-    Gets all views in a model which are matching a filter and are:
-
-    - not template views
-    - not system browser
-    - not project browser
-    - not undefined
-    - not Internal
-    - not sheets
+    Returns a dictionary of warnings where all warnings specified by guid related to each other are grouped together.
+    Key will be the element with the lowest element id, value will be a list of element ids, in ascending order, of all warnings in the group (including the key!)
 
+    Note:
+    Revit must report exactly two elements per warning for this to work
 
     :param doc: Current Revit model document.
     :type doc: Autodesk.Revit.DB.Document
-    :param filter: function checking view
-    :type filter: func(view) returning a bool
+    :param guid: Filter: Identifying a specific failure of which the corresponding messages are to be returned.
+    :type guid: Autodesk.Revit.DB.Guid
 
-    :return: list of views
-    :rtype: list of Autodesk.Revit.DB.View
+    :return: Dictionary of warnings grouped by element id
+    :rtype: dict
     """
 
-    views = []
-    col = rdb.FilteredElementCollector(doc).OfClass(rdb.View)
-    for v in col:
-        # filter out browser organization and other views which cant be deleted
-        if (
-            v.IsTemplate == False
-            and filter(v) == True
-            and v.ViewType != rdb.ViewType.SystemBrowser
-            and v.ViewType != rdb.ViewType.ProjectBrowser
-            and v.ViewType != rdb.ViewType.Undefined
-            and v.ViewType != rdb.ViewType.Internal
-            and v.ViewType != rdb.ViewType.DrawingSheet
-        ):
-            views.append(v)
-    return views
+    # get all warning relating to a guid
+    warnings = get_warnings_by_guid(doc, guid)
 
-
-def get_views_not_on_sheet(doc):
-    """
-    Gets all views not placed on a sheet. (Excludes schedules)
-
-    :param doc: Current Revit model document.
-    :type doc: Autodesk.Revit.DB.Document
-
-    :return: A list of views which are currently not placed on a sheet.
-    :rtype: list of Autodesk.Revit.DB.View
-    """
-
-    views_not_on_sheet = []
-    # get all sheets
-    sheets_in_model = get_all_sheets(doc)
-    # get all viewPorts on sheets
-    view_ports_on_sheets = get_viewport_on_sheets(doc, sheets_in_model)
-    # get all views in model
-    views_in_model = get_views_in_model(doc, filter_revision_schedules)
-    # check whether view has a viewport if not ... its not placed on a sheet
-    for view_in_model in views_in_model:
+    warning_grouping = {}
+    counter = 0
+    for warning in warnings:
         match = False
-        for view_ports_on_sheet in view_ports_on_sheets:
-            if view_ports_on_sheet.ViewId == view_in_model.Id:
+        element_ids = warning.GetFailingElements()
+
+        # just in case there are more than 2 elements in the warning
+        if len(element_ids) != 2:
+            continue
+
+        # initialise the first warning group
+        if len(warning_grouping) == 0:
+            warning_grouping[counter] = [
+                element_ids[0].IntegerValue,
+                element_ids[1].IntegerValue,
+            ]
+            continue
+
+        # check if the warning relates to an existing group
+        for key, value in warning_grouping.items():
+            if (
+                element_ids[0].IntegerValue in value
+                and element_ids[1].IntegerValue not in value
+            ):
+                warning_grouping[key].append(element_ids[1].IntegerValue)
+                # print("added {} to group {}".format( element_ids[1].IntegerValue, counter))
+                match = True
+                break
+            elif (
+                element_ids[1].IntegerValue in value
+                and element_ids[0].IntegerValue not in value
+            ):
+                warning_grouping[key].append(element_ids[0].IntegerValue)
+                # print("added {} to group {}".format( element_ids[0].IntegerValue, counter))
+                match = True
+                break
+            elif (
+                element_ids[1].IntegerValue in value
+                and element_ids[0].IntegerValue in value
+            ):
+                # print("matched {} {} to group {} {}".format( element_ids[0].IntegerValue, element_ids[1].IntegerValue, counter, value))
                 match = True
                 break
-        if match == False:
-            views_not_on_sheet.append(view_in_model)
-    return views_not_on_sheet
+            else:
+                pass
+                # print("no match for {} {} in {}".format(element_ids[0].IntegerValue, element_ids[1].IntegerValue, value))
+        if not match:
+            counter += 1
+            warning_grouping[counter] = [
+                element_ids[0].IntegerValue,
+                element_ids[1].IntegerValue,
+            ]
+            # print("new counter group: {} to group {}, {}".format(counter, element_ids[0].IntegerValue, element_ids[1].IntegerValue,))
+            # new warning grouping is required
+
+    sorted_warning_grouping = {}
+    # sort the values in the dictionary
+    for key, value in warning_grouping.items():
+        warning_grouping[key] = sorted(value)
+        sorted_warning_grouping[sorted(value)[0]] = sorted(value)
+    return sorted_warning_grouping
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/views_purge_unused.py` & `DuHast-0.1.3/src/duHast/Revit/Views/views_purge_unused.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics.py` & `DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics_categories.py` & `DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics_categories.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Views/visibility_graphics_filters.py` & `DuHast-0.1.3/src/duHast/Revit/Views/visibility_graphics_filters.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Walls/Utility/walls_type_sorting.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/Utility/walls_type_sorting.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from duHast.Revit.Walls.Utility.walls_filter import (
     _get_all_wall_types_by_class,
     _get_all_wall_types_by_category,
 )
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Walls/curtain_wall_elements.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/curtain_wall_elements.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 import clr
 import System
 from System.Collections.Generic import List
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Walls/curtain_walls.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/curtain_walls.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 from Autodesk.Revit.DB import (
     BuiltInCategory,
     FilteredElementCollector,
     WallKind,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Walls/purge_unused_wall_types.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/purge_unused_wall_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 
 # required for .ToList() call
 #import clr
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Walls/stacked_walls.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/stacked_walls.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
+#
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
 # import Autodesk
 from Autodesk.Revit.DB import (
     BuiltInCategory,
     FilteredElementCollector,
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Data/warnings_data.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/warnings_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 
 # from duHast.Utilities import Utility as util
 from duHast.Revit.Warnings import warnings as rWarn
 
 # import Autodesk
 # import Autodesk.Revit.DB as rdb
 
@@ -80,16 +80,16 @@
                     war_other_element_ids_as_integer.append(el.IntegerValue)
             except Exception as e:
                 pass
 
             # build data
             self.data.append(
                 {
-                    IFamData.ROOT: self.rootPath,
-                    IFamData.ROOT_CATEGORY: self.rootCategoryPath,
+                    IFamData.ROOT: self.root_path,
+                    IFamData.ROOT_CATEGORY: self.root_category_path,
                     IFamData.FAMILY_NAME: doc.Title,
                     IFamData.FAMILY_FILE_PATH: doc.PathName,
                     WARNING_TEXT: war_text,
                     WARNING_GUID: war_guid,
                     WARNING_RELATED_IDS: war_element_ids_as_integer,
                     WARNING_OTHER_IDS: war_other_element_ids_as_integer,
                 }
@@ -97,16 +97,16 @@
 
         # check if any shared parameter was found
         if len(self.data) == 0:
             # add message no warnings found
             # build data
             self.data.append(
                 {
-                    IFamData.ROOT: self.rootPath,
-                    IFamData.ROOT_CATEGORY: self.rootCategoryPath,
+                    IFamData.ROOT: self.root_path,
+                    IFamData.ROOT_CATEGORY: self.root_category_path,
                     IFamData.FAMILY_NAME: doc.Title,
                     IFamData.FAMILY_FILE_PATH: doc.PathName,
                     WARNING_TEXT: "No warnings present in family.",
                     WARNING_GUID: "",
                     WARNING_RELATED_IDS: [],
                     WARNING_OTHER_IDS: [],
                 }
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Data/warnings_data_processor.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Data/Objects/warnings_data_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-from duHast.Revit.Family.Data.ifamily_processor import IFamilyProcessor
-from duHast.Revit.Warnings.Data import warnings_data as rWarnData
-from duHast.Revit.Family.Data import ifamily_data as IFamData
+from duHast.Revit.Family.Data.Objects.ifamily_processor import IFamilyProcessor
+from duHast.Revit.Warnings.Data.Objects import warnings_data as rWarnData
+from duHast.Revit.Family.Data.Objects import ifamily_data as IFamData
 
 
 class WarningsProcessor(IFamilyProcessor):
     def __init__(self, pre_actions=None, post_actions=None):
         """
         Class constructor.
         """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/warnings_overlap_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/warnings_overlap_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Objects/warnings_storage.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Objects/warnings_storage.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Reporting/warnings_report_header.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Reporting/warnings_report_header.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/Utility/curves_util.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/Utility/curves_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
                         ),
                     )
                 return action_return_value
 
             transaction = Transaction(
                 doc, "Updating separation line geometry: {}".format(curve.id)
             )
-            update_curve_geometry = transaction_manager(transaction, action, doc)
+            update_curve_geometry = transaction_manager(transaction, action)
             # update_sep_geo = in_transaction(transaction, action)
             return_value.update(update_curve_geometry)
     return return_value
 
 
 def modify_curves_by_lengthening(doc, guid, transaction_manager, group_id, callback):
     """
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/solver.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         It will get all warnings in model, filter them by available solver GUIDs and finally will attempt to solve the warnings matched up with a solver.
 
         :param doc: Current Revit model document.
         :type doc: Autodesk.Revit.DB.Document
         :return:
             Result class instance.
 
-            - .result = True if all warnings could be solved. Otherwise False.
+            - .status True if all warnings could be solved. Otherwise False.
             - .message will contain all messages solver returned.
 
         :rtype: :class:`.Result`
         """
 
         return_value = res.Result()
         try:
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/solver_area_separation_lines_overlap.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/solver_area_separation_lines_overlap.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         :type doc: Autodesk.Revit.DB.Document
         :param warnings: List of warnings to be solved.
         :type warnings: Autodesk.Revit.DB.FailureMessage
 
         :return:
             Result class instance.
 
-            - .result = True if all area separation lines could be deleted / modified without an exception. Otherwise False.
+            - .status True if all area separation lines could be deleted / modified without an exception. Otherwise False.
             - .message will be 'moved tag to area xyz'
 
         :rtype: :class:`.Result`
         """
 
         return_value = res.Result()
         if len(warnings) > 0:
@@ -143,10 +143,10 @@
                     group_id=self.group_id,
                     transaction_manager=self.transaction_manager,
                     callback=self.callback,
                 )
                 return_value.update(modify_curves_status)
         else:
             return_value.update_sep(
-                True, "No warnings of type: area separation lines overlap in model."
+                True, "{}: No warnings of type: area separation lines overlap in model.".format(self.filter_name)
             )
         return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/solver_duplicate_mark.py` & `DuHast-0.1.3/src/duHast/Utilities/files_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Duplicate mark warnings solver class.
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Utility functions writing / reading json objects to/ from file.
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -23,96 +22,94 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Revit.Common import parameter_get_utils as rParaGet
-from duHast.Revit.Common import parameter_set_utils as rParaSet
 from duHast.Utilities.Objects import result as res
 
+import codecs
+import json
 
-# import Autodesk
-import Autodesk.Revit.DB as rdb
-from duHast.Utilities.Objects import base
-
-
-class RevitWarningsSolverDuplicateMark(base.Base):
-    def __init__(self, filter_func, filter_values=[]):
-        """
-        Constructor: this solver takes two arguments: a filter function and a list of values to filter by
-
-        :param filter_func: A function to filter elements in warnings by
-        :type filter_func: func(document, elementId, list of filter values)
-        :param filter_values: A list of filter values, defaults to []
-        :type filter_values: list, optional
-        """
-
-        # ini super class to allow multi inheritance in children!
-        super(RevitWarningsSolverDuplicateMark, self).__init__()
-
-        self.filter = filter_func
-        self.filter_values = filter_values
-        self.filter_name = "Duplicate mark value."
-
-    # --------------------------- duplicate mark guid ---------------------------
-    #: guid identifying this specific warning
-    GUID = "6e1efefe-c8e0-483d-8482-150b9f1da21a"
-
-    def solve_warnings(self, doc, warnings):
-        """
-        Solver setting element mark to nothing, provided it passes the filter.
-
-        :param doc: Current Revit model document.
-        :type doc: Autodesk.Revit.DB.Document
-        :param warnings: List of warnings to be solved.
-        :type warnings: Autodesk.Revit.DB.FailureMessage
-
-        :return:
-            Result class instance.
-
-            - .result = True if all duplicate mark warnings could be solved. Otherwise False.
-            - .message will contain stats in format parameter value set to ''
-
-        :rtype: :class:`.Result`
-        """
-
-        return_value = res.Result()
-        if len(warnings) > 0:
-            for warning in warnings:
-                element_ids = warning.GetFailingElements()
-                for el_id in element_ids:
-                    element = doc.GetElement(el_id)
-                    # check whether element passes filter
-                    if self.filter(doc, el_id, self.filter_values):
-                        try:
-                            p_value = rParaGet.get_built_in_parameter_value(
-                                element, rdb.BuiltInParameter.ALL_MODEL_MARK
-                            )
-                            if p_value != None:
-                                result = rParaSet.set_built_in_parameter_value(
-                                    doc,
-                                    element,
-                                    rdb.BuiltInParameter.ALL_MODEL_MARK,
-                                    "",
-                                )
-                                return_value.update(result)
-                        except Exception as e:
-                            return_value.update_sep(
-                                False,
-                                "Failed to solve warning duplicate mark with exception: {}".format(
-                                    e
-                                ),
-                            )
-                    else:
-                        return_value.update_sep(
-                            True,
-                            "Element removed by filter: {} : {}".format(
-                                self.filter_name, rdb.Element.Name.GetValue(element)
-                            ),
-                        )
+def _custom_default(o):
+    '''
+    Encode string values to utf-8 for json formatted outputs
+
+    :param o: The value to be encoded if of type string
+    :type o: var
+    :return: Encoded string or var
+    :rtype: str, var
+    '''
+
+    if isinstance(o, str):
+        # only encode if required
+        if any(ord(char) > 127 for char in o):
+            return o.encode('utf-8').decode('utf-8')  # Encoding and decoding to ensure the type is str
+    return o.__dict__
+
+def write_json_to_file(json_data, data_output_file_path, enforce_utf8 = True):
+    """
+    Writes collected data to a new json formatted file.
+
+    :param json_data: A dictionary to be written to file.
+    :type json_data: json object (dictionary)
+    :param data_output_file_path: Fully qualified file path to json data file.
+    :type data_output_file_path: str
+    :param enforce_utf8: Will encode any string value as utf-8, Default is true (recommended!!).
+    :type enforce_utf8: bool
+    :return:
+        Result class instance.
+        - result.status. True if json data file was written successfully, otherwise False.
+        - result.message will confirm path of json data file.
+        - result.result empty list
+        On exception:
+        - result.status (bool) will be False.
+        - result.message will contain exception message.
+        - result.result will be empty
+    :rtype: :class:`.Result`
+    """
+
+    result = res.Result()
+
+    try:
+        json_object = None
+        # check if utf-8 is to be enforced
+        if(enforce_utf8):
+            json_object = json.dumps(json_data, indent=None, default=_custom_default, ensure_ascii=False)
         else:
-            return_value.update_sep(
-                True, "No warnings of type: duplicate mark in model."
-            )
-        return return_value
+            json_object = json.dumps(json_data, indent=None, default=lambda o: o.__dict__)
+        with codecs.open(data_output_file_path, "w", encoding="utf-8") as f:
+            f.write(json_object)
+            f.close()
+
+        result.update_sep(
+            True, "Data written to file: {}".format(data_output_file_path)
+        )
+    except Exception as e:
+        result.update_sep(
+            False, "Failed to write data to file with exception: {}".format(e)
+        )
+    return result
+
+
+def read_json_data_from_file(file_path):
+    """
+    Reads json from file
+
+    :param revit_file_path: Fully qualified file path of report file.
+    :type file_path: str
+    :return: json object
+    :rtype: {}
+    """
+
+    data = {}
+    try:
+        # Opening JSON file
+        with open(file_path) as f:
+            # returns JSON object as
+            # a dictionary
+            data = json.load(f)
+            f.close()
+    except Exception as e:
+        pass
+    return data
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/solver_room_separation_lines_overlap.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/solver_room_separation_lines_overlap.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         :type doc: Autodesk.Revit.DB.Document
         :param warnings: List of warnings to be solved.
         :type warnings: Autodesk.Revit.DB.FailureMessage
 
         :return:
             Result class instance.
 
-            - .result = True if all room separation lines could be deleted / modified without an exception. Otherwise False.
+            - .status True if all room separation lines could be deleted / modified without an exception. Otherwise False.
             - .message will be 'moved tag to room xyz'
 
         :rtype: :class:`.Result`
         """
 
         return_value = res.Result()
         if len(warnings) > 0:
@@ -142,10 +142,10 @@
                     group_id=self.group_id,
                     transaction_manager=self.transaction_manager,
                     callback=self.callback,
                 )
                 return_value.update(modify_curves_status)
         else:
             return_value.update_sep(
-                True, "No warnings of type: room separation lines overlap in model."
+                True, "{}: No warnings of type: room separation lines overlap in model.".format(self.filter_name)
             )
         return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/Revit/Warnings/solver_room_tag_to_room.py` & `DuHast-0.1.3/src/duHast/Revit/Warnings/solver_room_tag_to_room.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         :type doc: Autodesk.Revit.DB.Document
         :param warnings: List of warnings to be solved.
         :type warnings: Autodesk.Revit.DB.FailureMessage
 
         :return:
             Result class instance.
 
-            - .result = True if all room tags within warnings could be moved to room location point. Otherwise False.
+            - .status True if all room tags within warnings could be moved to room location point. Otherwise False.
             - .message will be 'moved tag to room xyz'
 
         :rtype: :class:`.Result`
         """
 
         return_value = res.Result()
         if len(warnings) > 0:
@@ -87,10 +87,10 @@
                         tag_id=el_id,
                         transaction_manager=self.transaction_manager,
                     )
                     return_value.update(result)
                 counter = counter + 1
         else:
             return_value.update_sep(
-                True, "No warnings of type: room tag outside of room in model."
+                True, "{}: No warnings of type: room tag outside of room in model.".format(self.filter_name)
             )
         return return_value
```

### Comparing `DuHast-0.1.2/src/duHast/UI/Objects/common_ui.py` & `DuHast-0.1.3/src/duHast/UI/Objects/common_ui.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/UI/file_item.py` & `DuHast-0.1.3/src/duHast/UI/Objects/file_select_settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A class to store file information.
+A class to store file select UI settings.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 
 #
 # License:
 #
 #
@@ -23,44 +23,46 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-# An item to represent a file name in a row in a grid.
-
 from duHast.Utilities.Objects import base
 
-
-class MyFileItem(base.Base):
+# An item to represent a file name in a row in a grid.
+class FileSelectionSettings(base.Base):
     def __init__(
         self,
-        name,
-        size,
-        bim360_project_guid=None,
-        bim360_file_guid=None,
-        bim360_revit_version="-",
+        input_path,
+        include_sub_dirs_in_search,
+        output_directory,
+        output_file_number,
+        revit_file_extension,
+        filters,
+        filter_type,
     ):
         """
-        Class constructor.
+        Class constructor
 
-        :param name: The fully qualified file path.
-        :type name: str
-        :param size: The file size.
-        :type size: int
-        :param  bim360_project_guid: The BIM360 project GUID, defaults to None
-        :type  bim360_project_guid: str, optional
-        :param bim360_file_guid: The BIM360 file GUID, defaults to None
-        :type bim360_file_guid: str, optional
-        :param bim360_revit_version: The revit file version (year only), defaults to '-'
-        :type bim360_revit_version: str, optional
+        :param inputDirectory: A fully qualified directory path containing files to be shown in UI.
+        :type inputDirectory: str
+        :param include_sub_dirs_in_search: If True include subdirectories in file search, otherwise just root directory.
+        :type include_sub_dirs_in_search: bool
+        :param output_directory: A fully qualified directory path to where task files will be written.
+        :type output_directory: str
+        :param output_file_number: The number of task files to be written out.
+        :type output_file_number: int
+        :param revitFileExtension: A file extension filter applied to directory search.
+        :type revitFileExtension: str
         """
 
-        # ini super class to allow multi inheritance in children!
-        super(MyFileItem, self).__init__()
+        self.input_directory = input_path
+        self.incl_sub_dirs = include_sub_dirs_in_search
+        self.output_dir = output_directory
+        self.output_file_num = output_file_number
+        self.revit_file_extension = revit_file_extension
+        self.filters = filters
+        self.filter_type = filter_type
 
-        self.name = name
-        self.size = size
-        self.bim_360_project_guid = bim360_project_guid
-        self.bim_360_file_guid = bim360_file_guid
-        self.bim_360_revit_version = bim360_revit_version
+        # ini super class to allow multi inheritance in children!
+        super(FileSelectionSettings, self).__init__()
```

### Comparing `DuHast-0.1.2/src/duHast/UI/file_list.py` & `DuHast-0.1.3/src/duHast/Utilities/worksharing_monitor_process.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,263 +1,248 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Helper functions for the file selection GUI.
+Helper functions relating to Revit worksharing monitor process. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
-
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
-# Copyright (c) 2021  Jan Christel
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+# BSD License
+# Copyright 2023, Jan Christel
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+# - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+# - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+# - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
-# You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 #
 
-# this sample shows how to write out a number of task files using bucket distribution by file size
+from duHast.Utilities import (
+    files_csv as filesCSV,
+    files_get as fileGet,
+    files_io as fileIO,
+)
+from duHast.Utilities.Objects import result as res
+from duHast.Utilities import system_process as sp
 
-import clr
-import System
-import os
 
+""" 
+Process name of work sharing monitor
+"""
 
-# import file item class
-from duHast.UI import file_item as fi
+PROCESS_NAME_WSM = "WorksharingMonitor.exe"
+PROCESS_MARKER_FILENAME = "WSMProcessList"
+PROCESS_MARKER_FILE_EXTENSION = ".plist"
 
-# import workloader utils
-from duHast.UI import workloader as wl
 
-# custom result class
-from duHast.Utilities.Objects import result as res
-from duHast.Utilities.files_io import is_back_up_file
+# --------------------------------- worksharing monitor specific ---------------------------------------
 
-# -------------
-# my code here:
-# -------------
 
+def get_work_sharing_monitor_processes():
+    """
+    Get all currently running worksharing monitor processes
 
-def get_revit_files(directory, file_extension):
+    :return: _description_
+    :rtype: [[HandleCount, Name, Priority, ProcessId, ThreadCount, WorkingSetSize]]
     """
-    Returns files in a given directory and of a given file extension.
+    all_processes = sp.get_all_running_processes()
+    wsm_processes = sp.filter_by_process_name([PROCESS_NAME_WSM], all_processes)
+    return wsm_processes
 
-    :param directory: The fully qualified directory path.
-    :type directory: str
-    :param file_extension: The file extension filter in format '.ext'
-    :type file_extension: str
 
-    :return: List of file items
-    :rtype: [:class:`.FileItem`]
+def write_out_wsm_data_to_file(directory_path):
     """
+    Writes out all running worksharing monitor processes data to file
 
-    files = []
-    list_of_files = os.listdir(directory)
-    for f in list_of_files:
-        # check for file extension match
-        if f.lower().endswith(file_extension.lower()):
-            # check if this is a back up file
-            if is_back_up_file(f) == False:
-                # Use join to get full file path.
-                location = os.path.join(directory, f)
-                # Get size and add to list of files.
-                size = os.path.getsize(location)
-                files.append(fi.MyFileItem(location, size))
-    return files
+    :param directory_path: The directory path to where the marker file is to be saved.
+    :type directory_path: str
 
+    :return:
+        Result class instance.
 
-def get_revit_files_incl_sub_dirs(directory, file_extension):
-    """
-    Returns files in a given directory and its sub directories of a given file extension.
+        - Export status returned in result.status. False if an exception occurred, otherwise True.
+        - result.message will contain the fully qualified file path of the exported file.
 
-    :param directory: The fully qualified directory path.
-    :type directory: str
-    :param file_extension: The file extension filter in format '.ext'
-    :type file_extension: str
+        On exception:
+
+        - result.status (bool) will be False.
+        - result.message will contain the exception message.
 
-    :return: List of file items
-    :rtype: [:class:`.FileItem`]
+    :rtype: :class:`.Result`
     """
 
-    files = []
-    # Get the list of all files in directory tree at given path
-    list_of_files = list()
-    for dirpath, dirnames, filenames in os.walk(directory):
-        list_of_files += [os.path.join(dirpath, file) for file in filenames]
-    for f in list_of_files:
-        # check for file extension match
-        if f.lower().endswith(file_extension.lower()):
-            # check if this is a back up file,
-            if is_back_up_file(f) == False:
-                # Get size and add to list of files.
-                size = os.path.getsize(f)
-                files.append(fi.MyFileItem(f, size))
-    return files
+    status = res.Result()
+    process_list = get_work_sharing_monitor_processes()
+    status_write_out = sp.write_out_process_data(
+        directory_path,
+        process_list,
+        PROCESS_MARKER_FILENAME,
+        PROCESS_MARKER_FILE_EXTENSION,
+    )
+    if status_write_out:
+        status.update_sep(
+            True,
+            "Successfully wrote WSM process marker file to: " + str(directory_path),
+        )
+    else:
+        status.update_sep(
+            False, "Failed to write WSM process marker file to: " + str(directory_path)
+        )
+    return status
 
 
-def get_file_size(item):
+def delete_wsm_data_files(directory_path):
     """
-    Helper used to define workload size (same as file size)
+    Deletes all WSM marker files in a directory.
 
-    :param item: A file item object instance.
-    :type item: :class:`.FileItem`
+    WSM marker files got a specific file extension: Check: PROCESS_MARKER_FILE_EXTENSION
+
+    :param directory_path: The directory path containing marker files to be deleted.
+    :type directory_path: str
 
-    :return: The file size.
-    :rtype: int
+    :return: True if all files where deleted successfully, otherwise False.
+    :rtype: bool
     """
 
-    return item.size
+    status = True
+    # get files in directory
+    files_to_delete = fileGet.get_files_with_filter(
+        directory_path, PROCESS_MARKER_FILE_EXTENSION
+    )
+    if len(files_to_delete) > 0:
+        status_delete = True
+        for file in files_to_delete:
+            status_delete = status_delete and fileIO.file_delete(file)
+    return status
 
 
-def bucket_to_task_list_file_system(item):
+def read_wsm_data_from_file(directory_path):
     """
-    Default task list content for files on a file server location.
+    Reads all worksharing monitor processes data from marker file(s) in a given directory
+
+    WSM marker files got a specific file extension: Check: PROCESS_MARKER_FILE_EXTENSION
 
-    :param item: A file item object instance.
-    :type item: :class:`.FileItem`
+    :param directory_path: The directory path to where marker files are to be read from.
+    :type directory_path: str
 
-    :return: The item name.(fully qualified file path)
-    :rtype: str
+    :return: list of list of str
+    :rtype: [[HandleCount, Name, Priority, ProcessId, ThreadCount, WorkingSetSize]]
     """
 
-    return item.name
+    process_data = []
+    files = fileGet.get_files_with_filter(directory_path, PROCESS_MARKER_FILE_EXTENSION)
+    if len(files) > 0:
+        for file in files:
+            rows = filesCSV.read_csv_file(file)
+            if len(rows) > 0:
+                process_data = process_data + rows
+    return process_data
 
 
-def bucket_to_task_list_bim_360(item):
+def get_wsm_sessions_to_delete(ws_ms_to_keep):
     """
-    Default task list content for files on a BIM 360 cloud drive.
+    Returns Worksharing monitor process sessions filtered by provided list (not in list)
 
-    :param item: A file item object instance.
-    :type item: :class:`.FileItem`
+    :param ws_ms_to_keep: List of worksharing monitor sessions to filter by. WSM included in this list will be removed from past in list.
+    :type ws_ms_to_keep: List of list of str in format: [[HandleCount, Name, Priority, ProcessId, ThreadCount, WorkingSetSize]]
 
-    :return: The revit version, project guid, file guid separated by a space ' '
-    :rtype: str
+    :return: Filtered list of list of str of worksharing monitor sessions
+    :rtype: [[HandleCount, Name, Priority, ProcessId, ThreadCount, WorkingSetSize]]
     """
 
-    return " ".join(
-        [item.bim_360_revit_version, item.bim_360_project_guid, item.bim_360_file_guid]
-    )
+    all_running_wsm_processes = get_work_sharing_monitor_processes()
+    if len(ws_ms_to_keep) > 0:
+        # get ids from list
+        ids = []
+        for wsm_p in ws_ms_to_keep:
+            ids.append(wsm_p[3])
+        filtered_processes = sp.filter_by_process_ids(ids, ws_ms_to_keep, False)
+        return filtered_processes
+    else:
+        return all_running_wsm_processes
 
 
-def write_revit_task_file(file_name, bucket, get_data=bucket_to_task_list_file_system):
+def clean_up_wsm_data_files(directory_path):
     """
-    Writes out a task list file.
+    Removes all wsm data marker files in a given directory.
 
-    :param file_name: Fully qualified file path of the task file name including extension.
-    :type file_name: str
-    :param bucket: Workload bucket object instance.
-    :type bucket: :class:`.WorkloadBucket`
-    :param get_data: Returns data from file item object to be written to file, defaults to BucketToTaskListFileSystem
-    :type get_data: func(:class:`.FileItem`) -> str, optional
+    WSM marker files got a specific file extension: Check: PROCESS_MARKER_FILE_EXTENSION.
+
+    :param directory_path: The directory path containing the marker files to be deleted.
+    :type directory_path: str
 
     :return:
         Result class instance.
 
-        - Write file status (bool) returned in result.status. False if an exception occurred, otherwise True.
-        - Result.message property contains fully qualified file path to task list file.
+        - Delete status returned in result.status. False if an exception occurred, otherwise True.
+        - result.message will confirm successful deletion of all files.
 
         On exception:
 
-        - .status (bool) will be False.
-        - .message will contain the exception message.
+        - result.status (bool) will be False.
+        - result.message will contain the exception message.
 
     :rtype: :class:`.Result`
     """
 
-    return_value = res.Result()
-    try:
-        f = open(file_name, "w")
-        row_counter = 0
-        for p in bucket.items:
-            data = get_data(p)
-            # check whether first row
-            if row_counter != 0:
-                # if not first row add line feed character before data written
-                data = "\n" + data
-            else:
-                row_counter += 1
-            # this looks horrible: but:
-            # string.encode('utf-8') returns a byte string b''
-            # so it needs to be converted to an actual string again
-            f.write(data.encode("utf-8").decode("utf-8"))
-        f.close()
-        return_value.append_message("wrote task list: {} [TRUE]".format(file_name))
-    except Exception as e:
-        return_value.update_sep(
-            False,
-            "Failed to write task list: {} with exception {}".format(file_name, e),
-        )
-    return return_value
+    status = res.Result()
+    # attempt to delete old marker files
+    status_delete = delete_wsm_data_files(directory_path)
+    if status_delete:
+        status.update_sep(True, "Successfully deleted WSM marker file(s)!")
+    else:
+        status.update_sep(False, "Failed to delete WSM marker file(s)!")
+    return status
 
 
-def write_file_list(
-    directory_path,
-    file_extension,
-    task_list_directory,
-    task_files_number,
-    file_getter,
-    file_data_processor=bucket_to_task_list_file_system,
-):
+def die_wsm_die(directory_path, ignore_marker_files=False):
     """
-    Writes out all task list(s) to file(s).
+    Kills all worksharing monitor processes currently active.
+
+    Unless marker files are used. In that case only worksharing monitor sessions identified in marker files will be killed.
 
-    :param directory_path: Fully qualified directory path containing files to be added to task lists.
+    :param directory_path: The directory path to where marker files are to be read from.
     :type directory_path: str
-    :param file_extension: A file extension filter in format '.ext'
-    :type file_extension: str
-    :param task_list_directory: The fully qualified directory path where the task files will be written .
-    :type task_list_directory: str
-    :param task_files_number: The number of task files to be written.
-    :type task_files_number: int
-    :param file_getter: Function accepting a directory and file extension filter and returns file items from directory.
-    :type file_getter: func(str, str) -> :class:`.FileItem`
-    :param file_data_processor: Function processing file item and returns a string to be written to task list file, defaults to BucketToTaskListFileSystem
-    :type file_data_processor: func(:class:`.FileItem`) -> str, optional
+    :param ignore_marker_files: True no marker file data will be read and all WSM sessions running will be killed., defaults to False
+    :type ignore_marker_files: bool, optional
 
     :return:
         Result class instance.
 
-        - Write file status (bool) returned in result.status. False if an exception occurred, otherwise True.
-        - Result.message property contains fully qualified file path for each task list file.
+        - Kill status returned in result.status. False if an exception occurred, otherwise True.
+        - result.message will confirm successful killing of all WSM processes.
 
         On exception:
 
-        - .status (bool) will be False.
-        - .message will contain the exception message.
+        - result.status (bool) will be False.
+        - result.message will contain the exception message.
 
     :rtype: :class:`.Result`
     """
 
-    return_value = res.Result()
-    return_value.status = True
-    # get revit files in input dir
-    revit_files = file_getter(directory_path, file_extension)
-    # build bucket list
-    buckets = wl.distribute_workload(task_files_number, revit_files, get_file_size)
+    status = res.Result()
     try:
-        # write out file lists
-        counter = 0
-        for bucket in buckets:
-            file_name = os.path.join(
-                task_list_directory, "Tasklist_" + str(counter) + ".txt"
-            )
-            status_write = write_revit_task_file(file_name, bucket, file_data_processor)
-            return_value.update(status_write)
-            counter += 1
-        return_value.append_message("Finished writing out task files")
+        wsm_running_prior = []
+        if ignore_marker_files == False:
+            # read out worksharing monitor sessions running before script started
+            wsm_running_prior = read_wsm_data_from_file(directory_path)
+        wsm_to_delete = get_wsm_sessions_to_delete(wsm_running_prior)
+        status_kill = sp.kill_processes(wsm_to_delete)
+        if status_kill:
+            status.update_sep(True, "All WSM sessions where killed.")
+        else:
+            status.update_sep(False, "Failed to kill all WSM sessions.")
     except Exception as e:
-        return_value.update_sep(False, "Failed to save file list! " + str(e))
-    return return_value
+        status.update_sep(
+            False, "Failed to kill wsm sessions with exceptions: " + str(e)
+        )
+    return status
```

### Comparing `DuHast-0.1.2/src/duHast/UI/file_select_settings.py` & `DuHast-0.1.3/src/duHast/Utilities/benchmarking.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-A class to store file select UI settings.
+Helper functions for benchmarking:. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-"""
 
+- two values
+- whether a text value starts or does not start with a given text value
+
+"""
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -16,49 +19,65 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Utilities.Objects import base
+import time
+import functools
 
-# An item to represent a file name in a row in a grid.
-class FileSelectionSettings(base.Base):
-    def __init__(
-        self,
-        inputDirectory,
-        include_sub_dirs_in_search,
-        output_directory,
-        output_file_number,
-        revitFileExtension,
-    ):
-        """
-        Class constructor
-
-        :param inputDirectory: A fully qualified directory path containing files to be shown in UI.
-        :type inputDirectory: str
-        :param include_sub_dirs_in_search: If True include subdirectories in file search, otherwise just root directory.
-        :type include_sub_dirs_in_search: bool
-        :param output_directory: A fully qualified directory path to where task files will be written.
-        :type output_directory: str
-        :param output_file_number: The number of task files to be written out.
-        :type output_file_number: int
-        :param revitFileExtension: A file extension filter applied to directory search.
-        :type revitFileExtension: str
-        """
-
-        self.input_directory = inputDirectory
-        self.incl_sub_dirs = include_sub_dirs_in_search
-        self.output_dir = output_directory
-        self.output_file_num = output_file_number
-        self.revit_file_extension = revitFileExtension
 
-        # ini super class to allow multi inheritance in children!
-        super(FileSelectionSettings, self).__init__()
+def measure_time_wrapper(func, logger=None, measure=True):
+    # Get the function name for the print statement
+    func_name = func.__name__
+
+    @functools.wraps(func)
+    def wrapper_func(*args, **kwargs):
+        # Get the start time
+        start = time.time()
+        # Execute the function
+        result = func(*args, **kwargs)
+        # Get the end time
+        end = time.time()
+        # Calculate the elapsed time
+        elapsed = round(float(end - start), 5)
+        message = "Elapsed time for {} is : {}".format(func_name, elapsed)
+        if logger:
+            # Log the elapsed time
+            logger.info(message)
+        else:
+            # Print the elapsed time
+            print(message)
+        # Return the result of the function
+        return result
+
+    if measure:
+        return wrapper_func
+    else:
+        return func
+
+
+def add_measure_time(func, should_output=True):
+    """
+    Decorator function to measure the time a function takes to execute and then print it to the console.
+
+    Use like
+    @measure_time(should_output = show_benchmarking_output_bool)
+    def function_to_measure():
+        
+
+    :param should_output: Whether the elapsed time should be printed to the console
+    :type should_output: bool
+    """
+
+    if should_output:
+        return measure_time_wrapper(func, measure=should_output)
+    else:
+        return func
```

### Comparing `DuHast-0.1.2/src/duHast/UI/script.py` & `DuHast-0.1.3/src/duHast/UI/script.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,48 +16,52 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import sys, getopt, os
 
-import duHast.Utilities.files_io
-
 # to get to the root folder of this repo
 sys.path.append(
     os.path.join(os.path.realpath(__file__), os.pardir, os.pardir, os.pardir)
 )
 
 # import file item class
 # from duHast.UI import file_item as fi
 # import file list methods
 from duHast.UI import file_list as fl
 
 # import UI class
 from duHast.UI import ui_file_select as UIFs
 
 # import settings class
-from duHast.UI import file_select_settings as set
+from duHast.UI.Objects import file_select_settings as set
 
 # import workloader utils
 from duHast.UI import workloader as wl
 
 from duHast.Utilities.files_csv import read_csv_file, get_first_row_in_csv_file
 from duHast.Utilities.files_tab import get_first_row_in_file_no_strip
-from duHast.Utilities.files_io import file_exist, get_file_size, FILE_SIZE_IN_KB, is_back_up_file
-from duHast.UI.file_item import MyFileItem
+from duHast.Utilities.files_io import (
+    file_exist,
+    get_file_size,
+    FILE_SIZE_IN_KB,
+    is_back_up_file,
+)
+from duHast.Utilities.console_out import output_with_time_stamp
+from duHast.UI.Objects.file_item import MyFileItem
 
 # import bim360 utils from Library
 from duHast.Revit.BIM360 import util_bim_360 as ub360
 
 
 def main(argv):
     """
@@ -91,25 +95,25 @@
                 # write out file lists
                 counter = 0
                 for bucket in buckets:
                     file_name = os.path.join(
                         settings.output_dir, "Tasklist_" + str(counter) + ".txt"
                     )
                     status_write = fl.write_revit_task_file(file_name, bucket, get_data)
-                    print(status_write.message)
+                    output_with_time_stamp(status_write.message)
                     counter += 1
-                print("Finished writing out task files")
+                output_with_time_stamp("Finished writing out task files")
                 sys.exit(0)
             else:
                 # do nothing...
-                print("No files selected!")
+                output_with_time_stamp("No files selected!")
                 sys.exit(2)
         else:
             # show message box
-            print("No files found!")
+            output_with_time_stamp("No files found!")
             sys.exit(2)
     else:
         # invalid or no args provided... get out
         sys.exit(1)
 
 
 def process_args(argv):
@@ -133,22 +137,24 @@
     got_args = False
     try:
         opts, args = getopt.getopt(
             argv,
             "hsi:o:n:e:",
             ["subDir", "input=", "outputDir=", "numberFiles=", "fileExtension="],
         )
-    except getopt.GetoptError:
-        print(
-            "test.py -s -i <input> -o <output_directory> -n <numberOfOutputFiles> -e <fileExtension>"
+    except getopt.GetoptError as e:
+        output_with_time_stamp(
+            "script.py -s -i <input> -o <output_directory> -n <numberOfOutputFiles> -e <fileExtension> failed with exception: {}".format(
+                e
+            )
         )
     for opt, arg in opts:
         if opt == "-h":
-            print(
-                "test.py -i <input> -o <output_directory> -n <numberOfOutputFiles> -e <fileExtension>"
+            output_with_time_stamp(
+                "script.py -i <input> -o <output_directory> -n <numberOfOutputFiles> -e <fileExtension>"
             )
         elif opt in ("-s", "--subDir"):
             include_sub_dirs_in_search = True
         elif opt in ("-i", "--input"):
             input_dir_file = arg
             got_args = True
         elif opt in ("-o", "--outputDir"):
@@ -156,36 +162,43 @@
             got_args = True
         elif opt in ("-n", "--numberFiles"):
             try:
                 value = int(arg)
                 output_file_number = value
                 got_args = True
             except ValueError:
-                print(arg + " value is not an integer")
+                output_with_time_stamp("{}: value is not an integer".format(arg))
                 got_args = False
         elif opt in ("-e", "--fileExtension"):
-            revit_file_extension = arg
+            revit_file_extension = arg.strip()
             got_args = True
 
     # check if input values are valid
     if output_file_number < 0 or output_file_number > 100:
         got_args = False
-        print("The number of output files must be bigger then 0 and smaller then 100")
+        output_with_time_stamp(
+            "The number of output files must be bigger then 0 and smaller then 100"
+        )
     if not file_exist(input_dir_file):
         got_args = False
-        print("Invalid input directory or file path: " + str(input_dir_file))
+        output_with_time_stamp(
+            "Invalid input directory or file path: {}".format(input_dir_file)
+        )
     if not file_exist(output_directory):
         got_args = False
-        print("Invalid output directory: " + str(output_directory))
-    if revit_file_extension != ".rvt" and revit_file_extension != ".rfa":
+        output_with_time_stamp("Invalid output directory: {}".format(output_directory))
+    if (
+        revit_file_extension.lower() != ".rvt"
+        and revit_file_extension.lower() != ".rfa"
+    ):
         got_args = False
-        print(
-            "Invalid file extension: ["
-            + str(revit_file_extension)
-            + "] expecting: .rvt or .rfa"
+        output_with_time_stamp(
+            "Invalid file extension: [{}] expecting: .rvt or .rfa".format(
+                revit_file_extension
+            )
         )
 
     return got_args, set.FileSelectionSettings(
         input_dir_file,
         include_sub_dirs_in_search,
         output_directory,
         output_file_number,
@@ -257,18 +270,22 @@
                 if is_back_up_file(os.path.basename(revit_file.name)) == False:
                     if (
                         len(os.path.dirname(os.path.abspath(revit_file.name))) < 248
                         and len(revit_file.name) < 260
                     ):
                         revit_files.append(revit_file)
                     else:
-                        print("Max path length violation: {}".format(revit_file.name))
-                        print("File has been removed from selection!")
+                        output_with_time_stamp(
+                            "Max path length violation: {}".format(revit_file.name)
+                        )
+                        output_with_time_stamp("File has been removed from selection!")
     except Exception as e:
-        print("An exception occurred during BIM360 file read! {}".format(e))
+        output_with_time_stamp(
+            "An exception occurred during BIM360 file read! {}".format(e)
+        )
         # return an empty list which will cause this script to abort
         revit_files = []
     return revit_files
 
 
 def get_files_from_list_file(file_path_csv):
     """
@@ -290,15 +307,17 @@
             # process rows
             for rowData in rows:
                 if len(rowData) > 0:
                     file_size = get_file_size(rowData[0], FILE_SIZE_IN_KB)
                     dummy = MyFileItem(rowData[0], file_size)
                     revit_files.append(dummy)
     except Exception as e:
-        print("An exception occurred during row processing! " + str(e))
+        output_with_time_stamp(
+            "An exception occurred during row processing! {}".format(e)
+        )
         # return an empty list which will cause this script to abort
         revit_files = []
     return revit_files
 
 
 def get_file_data_from_text_file(file_path):
     """
```

### Comparing `DuHast-0.1.2/src/duHast/UI/workload_bucket.py` & `DuHast-0.1.3/src/duHast/UI/Objects/workload_bucket.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/UI/workloader.py` & `DuHast-0.1.3/src/duHast/UI/workloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import clr
 
 clr.AddReference("System.Core")
 from System import Linq
 
 clr.ImportExtensions(Linq)
 
-from duHast.UI import workload_bucket as wb
+from duHast.UI.Objects import workload_bucket as wb
 
 
 def distribute_workload(number_of_buckets, items, getWorkloadSize):
     """
     Distributes a given number of items evenly by workload size into workload buckets.
 
     :param numberOfBuckets: The number of buckets items are to be distributed to
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/Objects/base.py` & `DuHast-0.1.3/src/duHast/Utilities/Objects/base.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/Objects/result.py` & `DuHast-0.1.3/src/duHast/Utilities/Objects/result.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/Objects/timer.py` & `DuHast-0.1.3/src/duHast/Utilities/Objects/timer.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/batch_processor_log_utils.py` & `DuHast-0.1.3/src/duHast/Utilities/batch_processor_log_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 #       - timed out occurred and revit process got killed
 #           "WARNING: Timed-out"
 #   - delete process id pointer file
 #   - show user processing results (only when something went wrong(?))
 
 import clr
 import System
-from System.IO import Path
+
 import glob
 import time
 import os
 import json
 
 # custom result class from common library
 from duHast.Utilities.Objects import result as res
@@ -162,38 +162,41 @@
         f = open(file_name, "w")
         f.close()
     except:
         status = False
     return status
 
 
-def get_current_session_ids(folder_path):
+def get_current_session_ids(folder_path, delete_marker_files=True):
     """
     Returns file names of all text files in a given directory representing session Ids.
 
     Files will be deleted immediately after reading
 
     :param folder_path: Directory of where test files are located
     :type folder_path: str
 
     :return: A list of ids in string format.
     :rtype: [str]
     """
     ids = []
     file_list = glob.glob(folder_path + "\\*" + ".txt")
-    # delete marker files
-    result_delete = True
-    for fd in file_list:
-        if debug_mode_ == False:
-            result_delete = result_delete & fileIO.file_delete(fd)
-    if not result_delete:
-        output("Failed to delete a marker file!")
+    # delete marker files if required
+    if(delete_marker_files == True):
+        for fd in file_list:
+            fileIO.file_delete(fd)
+        result_delete = True
+        for fd in file_list:
+            if debug_mode_ == False:
+                result_delete = result_delete & fileIO.file_delete(fd)
+        if not result_delete:
+            output("Failed to delete a marker file!")
     for f in file_list:
         ids.append(
-            adjust_session_id_file_name_back(Path.GetFileNameWithoutExtension(f))
+            adjust_session_id_file_name_back(fileIO.get_file_name_without_ext(f))
         )
     return ids
 
 
 def get_log_files(list_of_session_ids):
     """
     Returns a list of fully qualified filepath to log files matching the provided session Ids.
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/benchmarking.py` & `DuHast-0.1.3/src/duHast/Utilities/unit_conversion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Helper functions for benchmarking:. 
+This module contains a number of unit conversion functions
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-- two values
-- whether a text value starts or does not start with a given text value
-
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -19,66 +16,62 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-import time
-import functools
 
+def convert_imperial_feet_to_metric_mm(value):
+    """
+    Converts feet and inches to mm
+    :param value: The value in feet to be converted
+    :type value: float
+    :return: The converted value
+    :rtype: float
+    """
+
+    return value * 304.8
+
+
+def convert_imperial_square_feet_to_metric_square_metre(value):
+    """
+    Converts square feet and inches to square m
+
+    :param value: The value in square feet to be converted
+    :type value: float
+    :return: The converted value
+    :rtype: float
+    """
+
+    return value * 0.092903
 
-def measure_time_wrapper(func, logger=None, measure=True):
-    # Get the function name for the print statement
-    func_name = func.__name__
-
-    @functools.wraps(func)
-    def wrapper_func(*args, **kwargs):
-        # Get the start time
-        start = time.time()
-        # Execute the function
-        result = func(*args, **kwargs)
-        # Get the end time
-        end = time.time()
-        # Calculate the elapsed time
-        elapsed = round(float(end - start), 5)
-        message = "Elapsed time for {} is : {}".format(func_name, elapsed)
-        if logger:
-            # Log the elapsed time
-            logger.info(message)
-        else:
-            # Print the elapsed time
-            print(message)
-        # Return the result of the function
-        return result
-
-    if measure:
-        return wrapper_func
-    else:
-        return func
-
-
-def add_measure_time(func, should_output=True):
-    """
-    Decorator function to measure the time a function takes to execute
-    and then print it to the console.
-
-    Use like:
-    @measure_time(should_output = show_benchmarking_output_bool)
-    def function_to_measure():
-        do_stuff()
-
-    :param should_output: Whether the elapsed time should be printed to the console
-    :type should_output: bool
-    """
-
-    if should_output:
-        return measure_time_wrapper(func, measure=should_output)
-    else:
-        return func
+
+def convert_imperial_cubic_feet_to_metric_cubic_metre(value):
+    """
+    Converts cubic feet and inches to cubic m
+
+    :param value: The value in cubic feet to be converted
+    :type value: float
+    :return: The converted value
+    :rtype: float
+    """
+
+    return value * 0.02831685
+
+
+def convert_mm_to_imperial_feet(length):
+    """
+    Convert a length value in millimeters to imperial feet.
+    
+    :param length: A float value representing the length in millimeters.
+    :type length: float
+    :return: A float value representing the length in imperial feet.
+    """
+    return length / 304.8
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/compare.py` & `DuHast-0.1.3/src/duHast/Utilities/compare.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,7 +93,29 @@
     :rtype: bool
     """
 
     if valueTwo.startswith(valueOne):
         return False
     else:
         return True
+
+
+def is_close(a, b, rel_tol=1e-09, abs_tol=0.0):
+    """
+    Compares two floats with a tolerance. Returns True if they are close enough, otherwise False
+
+    refer to: https://stackoverflow.com/questions/5595425/what-is-the-best-way-to-compare-floats-for-almost-equality-in-python
+
+    :param a: A float
+    :type a: float
+    :param b: A float
+    :type b: float
+    :param rel_tol: Relative tolerance used to compare the two floats, defaults to 1e-09
+    :type rel_tol: float, optional
+    :param abs_tol: Absolute tolerance used to compare the two floats, defaults to 0.0
+    :type abs_tol: float, optional
+
+    :return: Returns True if they are close enough to be considered equal, otherwise False
+    :rtype: bool
+    """
+
+    return abs(a - b) <= max(rel_tol * max(abs(a), abs(b)), abs_tol)
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/console_out.py` & `DuHast-0.1.3/src/duHast/Utilities/console_out.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/date_stamps.py` & `DuHast-0.1.3/src/duHast/Utilities/date_stamps.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/directory_io.py` & `DuHast-0.1.3/src/duHast/Utilities/directory_io.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_combine.py` & `DuHast-0.1.3/src/duHast/Utilities/files_combine.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_csv.py` & `DuHast-0.1.3/src/duHast/Utilities/files_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Helper functions relating to comma separated text files. 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
+
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
@@ -15,16 +16,16 @@
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 #
-# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
-# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
+# This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed.
+# In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits;
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 import codecs
 import csv
@@ -69,30 +70,30 @@
     Read a csv file into a list of rows, where each row is another list.
     :param filepathCSV: The fully qualified file path to the csv file.
     :type filepathCSV: str
     :return: A list of list of strings representing the data in each row.
     :rtype: list of list of str
     """
 
-    rowList = []
+    row_list = []
 
     # hard coded hack
     if increaseMaxFieldSizeLimit:
         csv.field_size_limit(2147483647)
 
     try:
         with open(filepathCSV) as csv_file:
             reader = csv.reader(csv_file)
             for row in reader:  # each row is a list
-                rowList.append(row)
+                row_list.append(row)
             csv_file.close()
     except Exception as e:
         print(str(e))
-        rowList = []
-    return rowList
+        row_list = []
+    return row_list
 
 
 def get_first_row_in_csv_file(filePath):
     """
     Reads the first line of a csv text file and returns it as a list of strings
     :param filePath: The fully qualified file path.
     :type filePath: str
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_get.py` & `DuHast-0.1.3/src/duHast/Utilities/files_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,17 @@
         else:
             file_dic[file_name] = [file_path]
     return file_dic
 
 
 def get_files(folder_path, file_extension=".rvt"):
     """
-    Gets a list of files from a given folder with a given file extension
+    Gets a list of files from a given folder with a given file extension.
+    (Returns the full path for each file!)
+
     :param folder_path: Folder path from which to get files to be combined and to which the combined file will be saved.
     :type folder_path: str
     :param file_extension: Filter: File needs to have this file extension, defaults to '.rvt'
     :type file_extension: str, optional
     :return: List of file path
     :rtype: list of str
     """
@@ -165,14 +167,15 @@
     file_list = glob.glob(os.path.join(folder_path, "*" + file_extension))
     return file_list
 
 
 def get_files_with_filter(folder_path, file_extension=".rvt", filter="*"):
     """
     Gets a list of files from a given folder with a given file extension and a matching a file name filter.
+    (Returns the full path for each file!)
 
     :param folder_path: Folder path from which to get files.
     :type folder_path: str
     :param file_extension: Filter: File needs to have this file extension, defaults to '.rvt'
     :type file_extension: str, optional
     :param filter: File name filter ('something*'), defaults to '*'
     :type filter: str, optional
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_io.py` & `DuHast-0.1.3/src/duHast/Utilities/files_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,31 @@
     value = True
     try:
         shutil.copy(old_name, new_name)
     except Exception:
         value = False
     return value
 
+def file_move(old_name, new_name):
+    """
+    Moves a file
+    :param old_name: Fully qualified file path to file to be moved.
+    :type old_name: str
+    :param new_name: Fully qualified path to new file location and name.
+    :type new_name: str
+    :return: True file moved, otherwise False
+    :rtype: bool
+    """
+
+    value = True
+    try:
+        shutil.move(old_name, new_name)
+    except Exception:
+        value = False
+    return value
 
 #: file size in KB conversion
 FILE_SIZE_IN_KB = 1024
 #: file size in MB conversion
 FILE_SIZE_IN_MB = 1024 * 1024
 #: file size in GB conversion
 FILE_SIZE_IN_GB = 1024 * 1024 * 1024
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_json.py` & `DuHast-0.1.3/src/duHast/Revit/Walls/Reporting/walls_report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Utility functions writing / reading json objects to/ from file.
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+This module contains a Revit walls properties report function. 
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
@@ -22,94 +22,76 @@
 # This software is provided by the copyright holder "as is" and any express or implied warranties, including, but not limited to, the implied warranties of merchantability and fitness for a particular purpose are disclaimed. 
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
-from duHast.Utilities.Objects import result as res
+from duHast.Revit.Materials.materials import get_material_name_by_id
+from duHast.Revit.Common.common import get_element_mark
+from duHast.Revit.Walls.walls import get_all_wall_types_by_category
+from duHast.Utilities.unit_conversion import convert_imperial_feet_to_metric_mm
+from duHast.Utilities.utility import encode_ascii
 
-import codecs
-import json
+from Autodesk.Revit.DB import Element
 
-def _custom_default(o):
-    '''
-    Encode string values to utf-8 for json formatted outputs
-
-    :param o: The value to be encoded if of type string
-    :type o: var
-    :return: Encoded string or var
-    :rtype: str, var
-    '''
-
-    if isinstance(o, str):
-        # only encode if required
-        if any(ord(char) > 127 for char in o):
-            return o.encode('utf-8').decode('utf-8')  # Encoding and decoding to ensure the type is str
-    return o.__dict__
-
-def write_json_to_file(json_data, data_output_file_path, enforce_utf8 = True):
-    """
-    Writes collected data to a new json formatted file.
-
-    :param json_data: A dictionary to be written to file.
-    :type json_data: json object (dictionary)
-    :param data_output_file_path: Fully qualified file path to json data file.
-    :type data_output_file_path: str
-    :param enforce_utf8: Will encode any string value as utf-8, Default is true (recommended!!).
-    :type enforce_utf8: bool
-    :return:
-        Result class instance.
-        - result.status. True if json data file was written successfully, otherwise False.
-        - result.message will confirm path of json data file.
-        - result.result empty list
-        On exception:
-        - result.status (bool) will be False.
-        - result.message will contain exception message.
-        - result.result will be empty
-    :rtype: :class:`.Result`
+def get_wall_report_data(doc, revit_file_path):
     """
-
-    result = res.Result()
-
-    try:
-        json_object = None
-        # check if utf-8 is to be enforced
-        if(enforce_utf8):
-            json_object = json.dumps(json_data, indent=None, default=_custom_default, ensure_ascii=False)
-        else:
-            json_object = json.dumps(json_data, indent=None, default=lambda o: o.__dict__)
-        with codecs.open(data_output_file_path, "w", encoding="utf-8") as f:
-            f.write(json_object)
-            f.close()
-
-        result.update_sep(
-            True, "Data written to file: {}".format(data_output_file_path)
-        )
-    except Exception as e:
-        result.update_sep(
-            False, "Failed to write data to file with exception: {}".format(e)
-        )
-    return result
-
-
-def read_json_data_from_file(file_path):
-    """
-    Reads json from file
-
-    :param revit_file_path: Fully qualified file path of report file.
-    :type file_path: str
-    :return: json object
-    :rtype: {}
+    Gets wall data to be written to report file.
+    :param doc: Current Revit model document.
+    :type doc: Autodesk.Revit.DB.Document
+    :param revit_file_path: The file hostname, which is added to data returned.
+    :type revit_file_path: str
+    :return: list of list of sheet properties.
+    :rtype: list of list of str
     """
 
-    data = {}
-    try:
-        # Opening JSON file
-        with open(file_path) as f:
-            # returns JSON object as
-            # a dictionary
-            data = json.load(f)
-            f.close()
-    except Exception as e:
-        pass
+    data = []
+    wall_types = get_all_wall_types_by_category(doc)
+    for wt in wall_types:
+        try:
+            wall_type_name = str(Element.Name.GetValue(wt))
+            cs = wt.GetCompoundStructure()
+            if cs != None:
+                cs_layers = cs.GetLayers()
+                # print(len(cs_layers))
+                for cs_layer in cs_layers:
+                    layer_mat = doc.GetElement(cs_layer.MaterialId)
+                    material_mark = material_name = "N/A"
+                    # not all layers may have assigned a material (could be Default)
+                    if layer_mat is not None:
+                        material_mark = get_element_mark(layer_mat)
+                        material_name = get_material_name_by_id(
+                            doc, cs_layer.MaterialId
+                        )
+                    layer_function = str(cs_layer.Function)
+                    layer_width = str(
+                        convert_imperial_feet_to_metric_mm(
+                            cs_layer.Width
+                        )
+                    )  # conversion from imperial to metric
+                    data.append(
+                        [
+                            revit_file_path,
+                            str(wt.Id),
+                            encode_ascii(wall_type_name),
+                            layer_function,
+                            layer_width,
+                            encode_ascii(material_name),
+                            encode_ascii(material_mark),
+                        ]
+                    )
+            else:
+                data.append(
+                    [
+                        revit_file_path,
+                        str(wt.Id),
+                        encode_ascii(wall_type_name),
+                        "no layers - in place family or curtain wall",
+                        str(0.0),
+                        "NA",
+                        "NA",
+                    ]
+                )
+        except:
+            data.append([revit_file_path, str(wt.Id)])
     return data
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/files_tab.py` & `DuHast-0.1.3/src/duHast/Utilities/files_tab.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/padding.py` & `DuHast-0.1.3/src/duHast/Utilities/padding.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/solibri_ifc_optimizer.py` & `DuHast-0.1.3/src/duHast/Utilities/solibri_ifc_optimizer.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/system_process.py` & `DuHast-0.1.3/src/duHast/Utilities/system_process.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/unit_conversion.py` & `DuHast-0.1.3/src/duHast/Data/Objects/data_door.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-This module contains a number of unit conversion functions
+Data storage class for Revit door properties.
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 """
 #
 # License:
 #
 #
 # Revit Batch Processor Sample Code
 #
 # BSD License
-# Copyright 2023, Jan Christel
+# Copyright 2024, Jan Christel
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 # - Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 # - Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 # - Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
@@ -24,54 +23,14 @@
 # In no event shall the copyright holder be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to, procurement of substitute goods or services; loss of use, data, or profits; 
 # or business interruption) however caused and on any theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
 #
 #
 #
 
 
-def convert_imperial_feet_to_metric_mm(value):
-    """
-    Converts feet and inches to mm
-    :param value: The value in feet to be converted
-    :type value: float
-    :return: The converted value
-    :rtype: float
-    """
-
-    return value * 304.8
-
-
-def convert_imperial_square_feet_to_metric_square_metre(value):
-    """
-    Converts square feet and inches to square m
-
-    :param value: The value in square feet to be converted
-    :type value: float
-    :return: The converted value
-    :rtype: float
-    """
-
-    return value * 0.092903
-
-
-def convert_imperial_cubic_feet_to_metric_cubic_metre(value):
-    """
-    Converts cubic feet and inches to cubic m
-
-    :param value: The value in cubic feet to be converted
-    :type value: float
-    :return: The converted value
-    :rtype: float
-    """
-
-    return value * 0.02831685
-
-
-def convert_mm_to_imperial_feet(length):
-    """
-    Convert a length value in millimeters to imperial feet.
-    
-    :param length: A float value representing the length in millimeters.
-    :type length: float
-    :return: A float value representing the length in imperial feet.
-    """
-    return length / 304.8
+from duHast.Data.Objects.data_family_base import DataFamilyBase
+
+class DataDoor(DataFamilyBase):
+
+    data_type = "door"
+
+
```

### Comparing `DuHast-0.1.2/src/duHast/Utilities/util_batch_p.py` & `DuHast-0.1.3/src/duHast/Utilities/util_batch_p.py`

 * *Files identical despite different names*

### Comparing `DuHast-0.1.2/src/duHast/Utilities/utility.py` & `DuHast-0.1.3/src/duHast/Utilities/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,7 +212,24 @@
     for k, v in d.items():
         new_key = parent_key + sep + k if parent_key else k
         if isinstance(v, collections.MutableMapping):
             items.extend(flatten(v, new_key, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
+
+def flatten_list(lst):
+    """
+    Function to flatten a nested list
+    
+    :param lst: The list to be flattened
+    :type lst: list
+    :return: The flattened list
+    :rtype: list
+    """
+    flattened = []
+    for item in lst:
+        if isinstance(item, list):
+            flattened.extend(flatten_list(item))
+        else:
+            flattened.append(item)
+    return flattened
```

