# Comparing `tmp/static-frame-2.5.1.tar.gz` & `tmp/static-frame-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-2.5.1.tar", last modified: Sun Mar 24 23:12:28 2024, max compression
+gzip compressed data, was "static-frame-2.5.2.tar", last modified: Tue Apr  9 14:10:57 2024, max compression
```

## Comparing `static-frame-2.5.1.tar` & `static-frame-2.5.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.779450 static-frame-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-24 23:11:56.000000 static-frame-2.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-24 23:11:56.000000 static-frame-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-03-24 23:12:28.779450 static-frame-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23373 2024-03-24 23:11:56.000000 static-frame-2.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-24 23:11:56.000000 static-frame-2.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-24 23:11:56.000000 static-frame-2.5.1/requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-24 23:11:56.000000 static-frame-2.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-24 23:12:28.779450 static-frame-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-24 23:11:56.000000 static-frame-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.755450 static-frame-2.5.1/static_frame/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.767450 static-frame-2.5.1/static_frame/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    53865 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    74108 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35749 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/display_html_datatables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/display_visidata.py
--rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/doc_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   389646 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/generic_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   108897 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/interface_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_re.py
--rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    34568 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_str.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/node_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/protocol_dfi_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   130408 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/series.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_client_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    60093 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   136563 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/www.py
--rw-r--r--   0 runner    (1001) docker     (127)    28780 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/core/yarn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.771450 static-frame-2.5.1/static_frame/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.779450 static-frame-2.5.1/static_frame/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    84900 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame_via_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_frame_via_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_series_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    69155 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_www.py
--rw-r--r--   0 runner    (1001) docker     (127)    47825 2024-03-24 23:11:56.000000 static-frame-2.5.1/static_frame/test/unit/test_yarn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:12:28.755450 static-frame-2.5.1/static_frame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-03-24 23:12:28.000000 static-frame-2.5.1/static_frame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-03-24 23:12:28.000000 static-frame-2.5.1/static_frame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 23:12:28.000000 static-frame-2.5.1/static_frame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-24 23:12:28.000000 static-frame-2.5.1/static_frame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-24 23:12:28.000000 static-frame-2.5.1/static_frame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.848351 static-frame-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-09 14:10:23.000000 static-frame-2.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-09 14:10:23.000000 static-frame-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-09 14:10:57.848351 static-frame-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23373 2024-04-09 14:10:23.000000 static-frame-2.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-09 14:10:23.000000 static-frame-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 14:10:23.000000 static-frame-2.5.2/requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 14:10:23.000000 static-frame-2.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 14:10:57.852351 static-frame-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-09 14:10:23.000000 static-frame-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.824351 static-frame-2.5.2/static_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.840351 static-frame-2.5.2/static_frame/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53865 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74108 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35749 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_html_datatables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/display_visidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/doc_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   389646 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/generic_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108897 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/interface_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34568 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/node_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/protocol_dfi_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130408 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_client_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60093 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136685 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29258 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/core/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.840351 static-frame-2.5.2/static_frame/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.848351 static-frame-2.5.2/static_frame/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84900 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_frame_via_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_series_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69155 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48834 2024-04-09 14:10:23.000000 static-frame-2.5.2/static_frame/test/unit/test_yarn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:10:57.828351 static-frame-2.5.2/static_frame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 14:10:57.000000 static-frame-2.5.2/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-2.5.1/LICENSE.txt` & `static-frame-2.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/PKG-INFO` & `static-frame-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.5.1
+Version: 2.5.2
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `static-frame-2.5.1/README.rst` & `static-frame-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/pyproject.toml` & `static-frame-2.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/setup.py` & `static-frame-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/__init__.py` & `static-frame-2.5.2/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 from static_frame.core.util import TLocSelectorCompound as TLocSelectorCompound
 from static_frame.core.util import TPathSpecifierOrBinaryIO as TPathSpecifierOrBinaryIO
 from static_frame.core.util import TPathSpecifierOrTextIO as TPathSpecifierOrTextIO
 from static_frame.core.util import TSeriesInitializer as TSeriesInitializer
 from static_frame.core.www import WWW as WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '2.5.1'
+__version__ = '2.5.2'
```

### Comparing `static-frame-2.5.1/static_frame/__main__.py` & `static-frame-2.5.2/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/archive_npy.py` & `static-frame-2.5.2/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/archive_zip.py` & `static-frame-2.5.2/static_frame/core/archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/axis_map.py` & `static-frame-2.5.2/static_frame/core/axis_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from functools import partial
+from itertools import repeat
 
 import typing_extensions as tp
 from arraykit import array_deepcopy
 
 from static_frame.core.bus import Bus
 from static_frame.core.exception import AxisInvalid
-from static_frame.core.frame import Frame
+from static_frame.core.generic_aliases import TBusAny
+from static_frame.core.generic_aliases import TFrameAny
+from static_frame.core.index import Index
 from static_frame.core.index_auto import IndexAutoConstructorFactory
 from static_frame.core.index_base import IndexBase
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.index_hierarchy import IndexHierarchyGO
 from static_frame.core.index_hierarchy import TTreeNode
+from static_frame.core.util import DTYPE_INT_DEFAULT
 from static_frame.core.util import TCallableAny
 from static_frame.core.util import TLabel
+from static_frame.core.util import TName
+from static_frame.core.util import TNDArrayObject
 
 if tp.TYPE_CHECKING:
     from static_frame.core.yarn import Yarn  # pragma: no cover
     TYarnAny = Yarn[tp.Any] #pragma: no cover
 
-TFrameAny = Frame[tp.Any, tp.Any, tp.Unpack[tp.Tuple[tp.Any, ...]]]
-TBusAny = Bus[tp.Any]
-
 def get_extractor(
         deepcopy_from_bus: bool,
         is_array: bool,
         memo_active: bool,
         ) -> TCallableAny:
     '''
     Args:
@@ -123,28 +126,52 @@
 
     # NOTE: we could try to collect index constructors by using the index of the Bus and observing the indices of the contained Frames, but it is not clear that will be better then using IndexAutoConstructorFactory
 
     return IndexHierarchy.from_tree(tree,
             index_constructors=IndexAutoConstructorFactory), opposite
 
 
-def buses_to_hierarchy(
+def buses_to_iloc_hierarchy(
         buses: tp.Iterable[TBusAny],
-        labels: tp.Iterable[TLabel],
         deepcopy_from_bus: bool,
         init_exception_cls: tp.Type[Exception],
         ) -> IndexHierarchy:
     '''
-    Given an iterable of named :obj:`Bus` derive a :obj:`Series` with an :obj:`IndexHierarchy`.
+    Given an iterable of named :obj:`Bus` derive a obj:`IndexHierarchy` with iloc labels on the outer depth, loc labels on the inner depth.
     '''
-    # NOTE: for now, the Returned Series will have bus Names as values; this requires the Yarn to store a dict, not a list
     extractor = get_extractor(deepcopy_from_bus, is_array=False, memo_active=False)
 
-    tree = {}
-    for label, bus in zip(labels, buses):
+    tree: TTreeNode = {}
+    for label, bus in enumerate(buses):
         if not isinstance(bus, Bus):
             raise init_exception_cls('Must provide an interable of Bus.')
-        if label in tree:
-            raise init_exception_cls(f'Bus names must be unique: {label} duplicated')
         tree[label] = extractor(bus._index)
 
-    return IndexHierarchy.from_tree(tree, index_constructors=IndexAutoConstructorFactory)
+    ctor: tp.Callable[..., IndexBase] = partial(Index, dtype=DTYPE_INT_DEFAULT)
+    return IndexHierarchy.from_tree(tree,
+            index_constructors=[ctor, IndexAutoConstructorFactory], # type: ignore
+            )
+
+def buses_to_loc_hierarchy(
+        buses: tp.Sequence[TBusAny] | TNDArrayObject,
+        deepcopy_from_bus: bool,
+        init_exception_cls: tp.Type[Exception],
+        ) -> IndexHierarchy:
+    '''
+    Given an iterable of named :obj:`Bus` derive a obj:`IndexHierarchy` with loc labels on the outer depth, loc labels on the inner depth.
+    '''
+    # NOTE: for now, the Returned Series will have bus Names as values; this requires the Yarn to store a dict, not a list
+    extractor = get_extractor(deepcopy_from_bus, is_array=False, memo_active=False)
+
+    bus_names = set(bus.name for bus in buses)
+    if len(bus_names) == len(buses):
+        # reuse indexes
+        tree = {}
+        for bus in buses:
+            tree[bus.name] = extractor(bus._index)
+        return IndexHierarchy.from_tree(tree, index_constructors=IndexAutoConstructorFactory)
+
+    # if Bus names are not unique, doing this permits discovering if resultant labels are unique
+    def labels() -> tp.Iterator[tuple[TName, TLabel]]:
+        for bus in buses:
+            yield from zip(repeat(bus.name), bus.index)
+    return IndexHierarchy.from_labels(labels(), index_constructors=IndexAutoConstructorFactory)
```

### Comparing `static-frame-2.5.1/static_frame/core/batch.py` & `static-frame-2.5.2/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/bus.py` & `static-frame-2.5.2/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/container.py` & `static-frame-2.5.2/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/container_util.py` & `static-frame-2.5.2/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/display.py` & `static-frame-2.5.2/static_frame/core/display.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/display_color.py` & `static-frame-2.5.2/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/display_config.py` & `static-frame-2.5.2/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/display_html_datatables.py` & `static-frame-2.5.2/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/display_visidata.py` & `static-frame-2.5.2/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/doc_str.py` & `static-frame-2.5.2/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/exception.py` & `static-frame-2.5.2/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/fill_value_auto.py` & `static-frame-2.5.2/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/frame.py` & `static-frame-2.5.2/static_frame/core/frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/generic_aliases.py` & `static-frame-2.5.2/static_frame/core/generic_aliases.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/hloc.py` & `static-frame-2.5.2/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index.py` & `static-frame-2.5.2/static_frame/core/index.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_auto.py` & `static-frame-2.5.2/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_base.py` & `static-frame-2.5.2/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_correspondence.py` & `static-frame-2.5.2/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_datetime.py` & `static-frame-2.5.2/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_hierarchy.py` & `static-frame-2.5.2/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-2.5.2/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/interface.py` & `static-frame-2.5.2/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/interface_meta.py` & `static-frame-2.5.2/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/join.py` & `static-frame-2.5.2/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/loc_map.py` & `static-frame-2.5.2/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/memory_measure.py` & `static-frame-2.5.2/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/metadata.py` & `static-frame-2.5.2/static_frame/core/metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_dt.py` & `static-frame-2.5.2/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_fill_value.py` & `static-frame-2.5.2/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_hashlib.py` & `static-frame-2.5.2/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_iter.py` & `static-frame-2.5.2/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_re.py` & `static-frame-2.5.2/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_selector.py` & `static-frame-2.5.2/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_str.py` & `static-frame-2.5.2/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_transpose.py` & `static-frame-2.5.2/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/node_values.py` & `static-frame-2.5.2/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/pivot.py` & `static-frame-2.5.2/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/platform.py` & `static-frame-2.5.2/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/protocol_dfi.py` & `static-frame-2.5.2/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/protocol_dfi_abc.py` & `static-frame-2.5.2/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/quilt.py` & `static-frame-2.5.2/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/rank.py` & `static-frame-2.5.2/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/series.py` & `static-frame-2.5.2/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store.py` & `static-frame-2.5.2/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_client_mixin.py` & `static-frame-2.5.2/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_config.py` & `static-frame-2.5.2/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_filter.py` & `static-frame-2.5.2/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_hdf5.py` & `static-frame-2.5.2/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_sqlite.py` & `static-frame-2.5.2/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_xlsx.py` & `static-frame-2.5.2/static_frame/core/store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/store_zip.py` & `static-frame-2.5.2/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/style_config.py` & `static-frame-2.5.2/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/type_blocks.py` & `static-frame-2.5.2/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/type_clinic.py` & `static-frame-2.5.2/static_frame/core/type_clinic.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/util.py` & `static-frame-2.5.2/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 TNDArrayAny = np.ndarray[tp.Any, tp.Any]
 TNDArrayBool = np.ndarray[tp.Any, np.dtype[np.bool_]]
 TNDArrayObject = np.ndarray[tp.Any, np.dtype[np.object_]]
 
 TNDArrayIntDefault = np.ndarray[tp.Any, np.dtype[np.int64]]
 
 TDtypeAny = np.dtype[tp.Any]
+TDtypeObject = np.dtype[np.object_] #pragma: no cover
 TOptionalArrayList = tp.Optional[tp.List[TNDArrayAny]]
 
 # dtype.kind
 #     A character code (one of ‘biufcmMOSUV’) identifying the general kind of data.
 #     b 	boolean
 #     i 	signed integer
 #     u 	unsigned integer
@@ -430,22 +431,23 @@
 TIndexInitializer = tp.Union[
         'IndexBase',
         tp.Iterable[TLabel],
         tp.Iterable[tp.Sequence[TLabel]], # only for IndexHierarchy
         # tp.Type['IndexAutoFactory'],
         ]
 
-TIndexCtor = tp.Union[tp.Callable[..., 'IndexBase'], tp.Type['Index']]
+# NOTE: this should include tp.Type['IndexAutoConstructorFactory']
+TIndexCtor = tp.Union[tp.Callable[..., 'IndexBase'], tp.Type['Index'],]
 TIndexHierarchyCtor = tp.Union[tp.Callable[..., 'IndexHierarchy'], tp.Type['IndexHierarchy']]
 
 TIndexCtorSpecifier = tp.Optional[TIndexCtor]
 
 TIndexCtorSpecifiers = tp.Union[TIndexCtorSpecifier,
         tp.Sequence[TIndexCtorSpecifier],
-        tp.Iterator[TIndexCtorSpecifier],
+        tp.Iterable[TIndexCtorSpecifier],
         TNDArrayObject, # object array of constructors
         None,
         tp.Type['IndexAutoConstructorFactory'],
         ]
 
 TExplicitIndexCtor = tp.Union[
         TIndexCtorSpecifier,
```

### Comparing `static-frame-2.5.1/static_frame/core/www.py` & `static-frame-2.5.2/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/core/yarn.py` & `static-frame-2.5.2/static_frame/core/yarn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from collections.abc import Set
 from itertools import chain
 
 import numpy as np
 import typing_extensions as tp
 
-from static_frame.core.axis_map import buses_to_hierarchy
+from static_frame.core.axis_map import buses_to_iloc_hierarchy
+from static_frame.core.axis_map import buses_to_loc_hierarchy
 from static_frame.core.bus import Bus
 from static_frame.core.container import ContainerBase
 from static_frame.core.container_util import index_from_optional_constructor
 from static_frame.core.container_util import index_many_concat
 from static_frame.core.container_util import iter_component_signature_bytes
 from static_frame.core.container_util import rehierarch_from_index_hierarchy
 from static_frame.core.display import Display
@@ -34,84 +35,85 @@
 from static_frame.core.node_selector import InterGetItemILocReduces
 from static_frame.core.node_selector import InterGetItemLocReduces
 from static_frame.core.series import Series
 from static_frame.core.store_client_mixin import StoreClientMixin
 from static_frame.core.style_config import StyleConfig
 from static_frame.core.util import DTYPE_OBJECT
 from static_frame.core.util import NAME_DEFAULT
+from static_frame.core.util import TDtypeObject
 from static_frame.core.util import TILocSelector
 from static_frame.core.util import TIndexCtorSpecifier
 from static_frame.core.util import TIndexCtorSpecifiers
 from static_frame.core.util import TIndexInitializer
 from static_frame.core.util import TLabel
 from static_frame.core.util import TLocSelector
 from static_frame.core.util import TName
+from static_frame.core.util import TNDArrayAny
+from static_frame.core.util import TNDArrayObject
 from static_frame.core.util import is_callable_or_mapping
-
-if tp.TYPE_CHECKING:
-    TNDArrayAny = np.ndarray[tp.Any, tp.Any] #pragma: no cover
-    TDtypeAny = np.dtype[tp.Any] #pragma: no cover
-    TDtypeObject = np.dtype[np.object_] #pragma: no cover
+from static_frame.core.util import iterable_to_array_1d
 
 TSeriesObject = Series[tp.Any, np.object_]
 TFrameAny = Frame[tp.Any, tp.Any, tp.Unpack[tp.Tuple[tp.Any, ...]]]
 TBusAny = Bus[tp.Any]
 
 #-------------------------------------------------------------------------------
 TVIndex = tp.TypeVar('TVIndex', bound=IndexBase, default=tp.Any)
 
 class Yarn(ContainerBase, StoreClientMixin, tp.Generic[TVIndex]):
     '''
     A :obj:`Series`-like container made of an ordered collection of :obj:`Bus`. :obj:`Yarn` can be indexed independently of the contained :obj:`Bus`, permitting independent labels per contained :obj:`Frame`.
     '''
 
     __slots__ = (
-            '_series',
+            '_values',
             '_hierarchy',
             '_index',
+            '_name',
             '_deepcopy_from_bus',
             )
 
-    _series: TSeriesObject
+    _values: TNDArrayObject
     _hierarchy: IndexHierarchy
     _index: IndexBase
+    _name: TName
 
     _NDIM: int = 1
 
     @classmethod
     def from_buses(cls,
             buses: tp.Iterable[TBusAny],
             *,
             name: TName = None,
             retain_labels: bool,
             deepcopy_from_bus: bool = False,
             ) -> tp.Self:
         '''Return a :obj:`Yarn` from an iterable of :obj:`Bus`; labels will be drawn from :obj:`Bus.name`.
         '''
-        series: TSeriesObject = Series.from_items(
-                    ((b.name, b) for b in buses),
-                    dtype=DTYPE_OBJECT,
-                    name=name,
-                    )
+        values, _ = iterable_to_array_1d(buses, dtype=DTYPE_OBJECT)
 
-        hierarchy = buses_to_hierarchy(
-                series.values,
-                series.index,
+        hierarchy = buses_to_iloc_hierarchy(
+                values,
                 deepcopy_from_bus=deepcopy_from_bus,
                 init_exception_cls=ErrorInitYarn,
                 )
 
         if retain_labels:
-            index = hierarchy
+            index = buses_to_loc_hierarchy(
+                    values,
+                    deepcopy_from_bus=deepcopy_from_bus,
+                    init_exception_cls=ErrorInitYarn,
+                    )
         else:
             index = hierarchy.level_drop(1) #type: ignore
 
-        return cls(series,
+        return cls(values,
                 hierarchy=hierarchy,
                 index=index,
+                name=name,
                 deepcopy_from_bus=deepcopy_from_bus,
                 )
 
     @classmethod
     def from_concat(cls,
             containers: tp.Iterable[TYarnAny],
             *,
@@ -128,73 +130,78 @@
             name:
             deepcopy_from_bus:
         '''
         bus_components: tp.List[TBusAny] = []
         index_components: tp.Optional[tp.List[IndexBase]] = None if index is not None else []
         for element in containers:
             if isinstance(element, Yarn):
-                bus_components.extend(element._series.values)
+                bus_components.extend(element._values)
                 if index_components is not None:
                     index_components.append(element.index)
             else:
                 raise NotImplementedError(f'cannot instantiate from {type(element)}')
 
         array = np.empty(len(bus_components), dtype=DTYPE_OBJECT)
         for i, bus in enumerate(bus_components):
             array[i] = bus
         array.flags.writeable = False
 
         if index_components is not None:
             index = index_many_concat(index_components, Index)
 
-        series: TSeriesObject = Series(array, name=name)
-        return cls(series,
+        # series: TSeriesObject = Series(array)
+        return cls(array,
                 deepcopy_from_bus=deepcopy_from_bus,
                 index=index,
+                name=name,
                 )
 
     #---------------------------------------------------------------------------
     def __init__(self,
-            series: tp.Union[TSeriesObject, tp.Iterable[TBusAny]],
+            series: tp.Union[TSeriesObject, tp.Iterable[TBusAny]], # rename: values
             *,
             index: TIndexInitializer | TIndexAutoFactory | None = None,
             index_constructor: tp.Optional[TIndexCtorSpecifier] = None,
             deepcopy_from_bus: bool = False,
             hierarchy: tp.Optional[IndexHierarchy] = None,
+            name: TName = None,
             own_index: bool = False,
             ) -> None:
         '''
         Args:
-            series: An iterable (or :obj:`Series`) of :obj:`Bus`. The length of this container is not the same as ``index``, if provided.
+            series: An iterable (or :obj:`Series`) of :obj:`Bus`. The length of this container may not be the same as ``index``, if provided.
             index: Optionally provide an index for the :obj:`Frame` contained in all :obj:`Bus`.
             index_constructor:
             deepcopy_from_bus:
-            hierarchy:
+            hierarchy: Optionally provide a depth-two `IndexHierarchy` constructed from `Bus` integer positions on the outer level, and contained `Frame` labels on the inner level.
+            name:
             own_index:
         '''
 
         if isinstance(series, Series):
             if series.dtype != DTYPE_OBJECT:
                 raise ErrorInitYarn(
                         f'Series passed to initializer must have dtype object, not {series.dtype}')
-            self._series = series # Bus by Bus label
+            self._values = series.values
         else:
-            self._series = Series(series, dtype=DTYPE_OBJECT) # get a default index
+            try:
+                self._values, _ = iterable_to_array_1d(series, dtype=DTYPE_OBJECT)
+            except RuntimeError as e:
+                raise ErrorInitYarn(e) from None
 
+        self._name = name
         self._deepcopy_from_bus = deepcopy_from_bus
 
-        # _hierarchy might be None while we still need to set self._index
         if hierarchy is None:
-            self._hierarchy = buses_to_hierarchy(
-                    self._series.values,
-                    self._series.index,
+            self._hierarchy = buses_to_iloc_hierarchy(
+                    self._values,
                     deepcopy_from_bus=self._deepcopy_from_bus,
                     init_exception_cls=ErrorInitYarn,
                     )
-        else:
+        else: # NOTE: we assume this hierarchy is well-formed
             self._hierarchy = hierarchy
 
         if own_index:
             self._index = index #type: ignore
         elif index is None or index is IndexAutoFactory:
             self._index = IndexAutoFactory.from_optional_constructor(
                     len(self._hierarchy),
@@ -212,15 +219,15 @@
 
     #---------------------------------------------------------------------------
     # deferred loading of axis info
 
     def unpersist(self) -> None:
         '''For the :obj:`Bus` contained in this object, replace all loaded :obj:`Frame` with :obj:`FrameDeferred`.
         '''
-        for b in self._series.values:
+        for b in self._values:
             b.unpersist()
 
     #---------------------------------------------------------------------------
     def __reversed__(self) -> tp.Iterator[TLabel]:
         '''
         Returns a reverse iterator on the :obj:`Yarn` index.
 
@@ -232,28 +239,28 @@
     #---------------------------------------------------------------------------
     # name interface
 
     @property
     @doc_inject()
     def name(self) -> TName:
         '''{}'''
-        return self._series._name
+        return self._name
 
     def rename(self, name: TName) -> tp.Self:
         '''
         Return a new :obj:`Yarn` with an updated name attribute.
 
         Args:
             name
         '''
         # NOTE: do not need to call _update_index_labels; can continue to defer
-        series = self._series.rename(name)
-        return self.__class__(series,
+        return self.__class__(self._values,
                 index=self._index,
                 hierarchy=self._hierarchy,
+                name=name,
                 deepcopy_from_bus=self._deepcopy_from_bus,
                 )
 
     #---------------------------------------------------------------------------
     # interfaces
 
     @property
@@ -401,27 +408,28 @@
             return default
         return self.__getitem__(key)
 
     def items(self) -> tp.Iterator[tp.Tuple[TLabel, TFrameAny]]:
         '''Iterator of pairs of :obj:`Yarn` label and contained :obj:`Frame`.
         '''
         labels = iter(self._index)
-        for bus in self._series.values:
+        for bus in self._values:
             # NOTE: cannot use Bus.items() as it may not have the same index representation as the Yarn; Bus._axis_element is optimized for handling max_persist > 1 loading
             for f in bus._axis_element():
                 yield next(labels), f
 
     _items_store = items
 
     @property
     def values(self) -> TNDArrayAny:
         '''A 1D object array of all :obj:`Frame` contained in all contained :obj:`Bus`.
         '''
+        # NOTE self._values is likely not the same size as self.values
         array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
-        np.concatenate([b.values for b in self._series.values], out=array)
+        np.concatenate([b.values for b in self._values], out=array)
         array.flags.writeable = False
         return array
 
 
     #---------------------------------------------------------------------------
     @doc_inject()
     def equals(self,
@@ -448,15 +456,15 @@
             return True
 
         if compare_class and self.__class__ != other.__class__:
             return False
         elif not isinstance(other, Yarn):
             return False
 
-        if compare_name and self._series._name != other._series._name:
+        if compare_name and self._name != other._name:
             return False
 
         # length of series in Yarn might be different but may still have the same frames, so look at realized length
         if len(self) != len(other):
             return False
 
         if not self._index.equals(
@@ -516,49 +524,48 @@
         '''
         Returns:
             Yarn or, if an element is selected, a Frame
         '''
         target_hierarchy = self._hierarchy._extract_iloc(key)
         if isinstance(target_hierarchy, tuple):
             # got a single element, return a Frame
-            return self._series[target_hierarchy[0]][target_hierarchy[1]] #type: ignore
+            b_pos, frame_label = target_hierarchy
+            return self._values[b_pos]._extract_loc(frame_label) # type: ignore
 
-        # get the outer-most index of the hierarchical index
-        target_bus_index = target_hierarchy.unique(depth_level=0, order_by_occurrence=True)
-        target_bus_index = next(iter(target_hierarchy._index_constructors))(target_bus_index)
+        # get the outer-most index of the hierarchical index; we cannot use index_at_depth
+        target_bus_labels = target_hierarchy.unique(
+                depth_level=0,
+                order_by_occurrence=True)
+        ctor = next(iter(target_hierarchy._index_constructors))
+        target_bus_index = ctor(target_bus_labels)
 
         # create a Boolean array equal to the entire realized length
         valid = np.full(len(self._index), False)
         valid[key] = True
-        index = self._index.iloc[key]
 
         buses = np.empty(len(target_bus_index), dtype=DTYPE_OBJECT)
 
         pos = 0
-        for bus_label, width in self._hierarchy.label_widths_at_depth(0):
-            if bus_label not in target_bus_index:
+        for b_pos, width in self._hierarchy.label_widths_at_depth(0):
+            if b_pos not in target_bus_index:
                 pos += width
                 continue
-            extract_per_bus = valid[pos: pos+width]
+            # create Boolean selection within this Bus
+            extract_per_bus = valid[pos: pos + width]
             pos += width
-
-            idx = target_bus_index.loc_to_iloc(bus_label)
-            buses[idx] = self._series[bus_label]._extract_iloc(extract_per_bus) # type: ignore
+            # given original bus position, look-up the bus position in returned array
+            idx = target_bus_index.loc_to_iloc(b_pos)
+            buses[idx] = self._values[b_pos]._extract_iloc(extract_per_bus) # type: ignore
 
         buses.flags.writeable = False
-        target_series: TSeriesObject = Series(buses,
-                index=target_bus_index,
-                own_index=True,
-                name=self._series._name,
-                )
 
-        return self.__class__(target_series,
-                index=index,
-                hierarchy=target_hierarchy,
+        return self.__class__(buses,
+                index=self._index.iloc[key],
                 deepcopy_from_bus=self._deepcopy_from_bus,
+                name=self._name,
                 own_index=True,
                 )
 
     def _extract_loc(self, key: TLocSelector) -> TYarnAny | TFrameAny:
         # use the index active for this Yarn
         key_iloc = self._index._loc_to_iloc(key)
         return self._extract_iloc(key_iloc)
@@ -592,15 +599,15 @@
         '''Generator of index, value pairs, equivalent to Series.items(). Repeated to have a common signature as other axis functions.
         '''
         yield from self.items()
 
     def _axis_element(self,
             ) -> tp.Iterator[tp.Any]:
 
-        for bus in self._series.values:
+        for bus in self._values:
             yield from bus._axis_element()
 
     #---------------------------------------------------------------------------
     def __len__(self) -> int:
         '''Length of values.
         '''
         return self._index.__len__()
@@ -615,81 +622,77 @@
 
         Args:
             {config}
         '''
         # NOTE: the key change over serires is providing the Bus as the displayed class
         config = config or DisplayActive.get()
         display_cls = Display.from_values((),
-                header=DisplayHeader(self.__class__, self._series._name),
+                header=DisplayHeader(self.__class__, self._name),
                 config=config)
 
         # NOTE: do not load FrameDeferred, so concatenate contained Series's values directly
         array = np.empty(shape=len(self._index), dtype=DTYPE_OBJECT)
         np.concatenate(
-            [b._values_mutable for b in self._series.values],
+            [b._values_mutable for b in self._values],
             out=array)
         array.flags.writeable = False
 
+        # create temporary series just for display
         series: TSeriesObject = Series(array, index=self._index, own_index=True)
-
         return series._display(config,
-
                 display_cls=display_cls,
                 style_config=style_config,
                 )
 
     #---------------------------------------------------------------------------
     # extended discriptors; in general, these do not force loading Frame
 
     @property
     def mloc(self) -> TSeriesObject:
         '''Returns a :obj:`Series` showing a tuple of memory locations within each loaded Frame.
         '''
-        return Series.from_concat((b.mloc for b in self._series.values),
+        return Series.from_concat((b.mloc for b in self._values),
                 index=self._index)
 
     @property
     def dtypes(self) -> TFrameAny:
         '''Returns a Frame of dtypes for all loaded Frames.
         '''
         return Frame.from_concat(
-                frames=(f.dtypes for f in self._series.values),
+                frames=(f.dtypes for f in self._values),
                 fill_value=None,
                 ).relabel(index=self._index)
 
     @property
     def shapes(self) -> TSeriesObject:
         '''A :obj:`Series` describing the shape of each loaded :obj:`Frame`. Unloaded :obj:`Frame` will have a shape of None.
 
         Returns:
             :obj:`tp.Series`
         '''
-        return Series.from_concat((b.shapes for b in self._series.values),
+        return Series.from_concat((b.shapes for b in self._values),
                 index=self._index)
 
     @property
     def nbytes(self) -> int:
         '''Total bytes of data currently loaded in :obj:`Bus` contained in this :obj:`Yarn`.
         '''
-        return sum(b.nbytes for b in self._series.values)
+        return sum(b.nbytes for b in self._values)
 
     @property
     def status(self) -> TFrameAny:
         '''
         Return a :obj:`Frame` indicating loaded status, size, bytes, and shape of all loaded :obj:`Frame` in :obj:`Bus` contined in this :obj:`Yarn`.
         '''
         f: TFrameAny = Frame.from_concat(
-                (b.status for b in self._series.values),
+                (b.status for b in self._values),
                 index=IndexAutoFactory)
         return f.relabel(index=self._index)
 
 
-
-
-
     #---------------------------------------------------------------------------
     # exporter
 
     def to_series(self) -> TSeriesObject: # can get generic Bus index
         '''Return a :obj:`Series` with the :obj:`Frame` contained in all contained :obj:`Bus`.
         '''
         # NOTE: this should load all deferred Frame
@@ -748,30 +751,30 @@
             index_init = self._index.relabel(index)
             own_index = True
         elif isinstance(index, Set):
             raise RelabelInvalid()
         else:
             index_init = index #type: ignore
 
-        return self.__class__(self._series, # no change to Buses
+        return self.__class__(self._values, # no change to Buses
                 index=index_init, # pyright: ignore
                 deepcopy_from_bus=self._deepcopy_from_bus,
                 hierarchy=self._hierarchy, # no change
                 own_index=own_index,
                 )
 
     @doc_inject(selector='relabel_flat', class_name='Yarn')
     def relabel_flat(self) -> tp.Self:
         '''
         {doc}
         '''
         if not isinstance(self._index, IndexHierarchy):
             raise RuntimeError('cannot flatten an Index that is not an IndexHierarchy')
 
-        return self.__class__(self._series, # no change to Buses
+        return self.__class__(self._values, # no change to Buses
                 index=self._index.flat(),
                 deepcopy_from_bus=self._deepcopy_from_bus,
                 hierarchy=self._hierarchy, # no change
                 own_index=True,
                 )
 
     @doc_inject(selector='relabel_level_add', class_name='Yarn')
@@ -780,15 +783,15 @@
             ) -> tp.Self:
         '''
         {doc}
 
         Args:
             level: {level}
         '''
-        return self.__class__(self._series, # no change to Buses
+        return self.__class__(self._values, # no change to Buses
                 index=self._index.level_add(level),
                 deepcopy_from_bus=self._deepcopy_from_bus,
                 hierarchy=self._hierarchy, # no change
                 own_index=True,
                 )
 
     @doc_inject(selector='relabel_level_drop', class_name='Yarn')
@@ -800,15 +803,15 @@
 
         Args:
             count: {count}
         '''
         if not isinstance(self._index, IndexHierarchy):
             raise RuntimeError('cannot drop level of an Index that is not an IndexHierarchy')
 
-        return self.__class__(self._series, # no change to Buses
+        return self.__class__(self._values, # no change to Buses
                 index=self._index.level_drop(count),
                 deepcopy_from_bus=self._deepcopy_from_bus,
                 hierarchy=self._hierarchy, # no change
                 own_index=True,
                 )
 
     def rehierarch(self,
```

### Comparing `static-frame-2.5.1/static_frame/test/test_case.py` & `static-frame-2.5.2/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_archive_npy.py` & `static-frame-2.5.2/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_archive_zip.py` & `static-frame-2.5.2/static_frame/test/unit/test_archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_axis_map.py` & `static-frame-2.5.2/static_frame/test/unit/test_axis_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import frame_fixtures as ff
 import numpy as np
 import typing_extensions as tp
 
 from static_frame.core.axis_map import bus_to_hierarchy
-from static_frame.core.axis_map import buses_to_hierarchy
+from static_frame.core.axis_map import buses_to_iloc_hierarchy
 from static_frame.core.bus import Bus
 from static_frame.core.exception import AxisInvalid
 from static_frame.core.exception import ErrorInitBus
 from static_frame.core.exception import ErrorInitQuilt
 from static_frame.core.exception import ErrorInitYarn
 from static_frame.core.frame import Frame
 from static_frame.core.index import Index
@@ -27,30 +27,14 @@
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
 
         b1 = Bus.from_frames((f1, f2, f3))
 
         with self.assertRaises(AxisInvalid):
             bus_to_hierarchy(b1, deepcopy_from_bus=False, axis=3, init_exception_cls=ErrorInitQuilt)
 
-    def test_index_map_a(self) -> None:
-
-        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
-        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
-        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
-        b1 = Bus.from_frames((f1, f2, f3), name='a')
-
-        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
-        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
-        b2 = Bus.from_frames((f4, f5), name='b')
-
-        post = buses_to_hierarchy((b1, b2), (b1.name, b2.name), deepcopy_from_bus=False, init_exception_cls=ErrorInitYarn)
-
-        self.assertEqual(post.values.tolist(),
-                [['a', 'f1'], ['a', 'f2'], ['a', 'f3'], ['b', 'f4'], ['b', 'f5']])
-
     def compare_trees(self, tree1: TTreeNode, tree2: TTreeNode) -> None:
         self.assertSequenceEqual(tree1.keys(), tree2.keys())
 
         for k, v1 in tree1.items():
             v2 = tree2[k]
             if isinstance(v1, Index):
                 self.assertTrue(v1.equals(v2))
@@ -146,32 +130,47 @@
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='a')
 
         f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
         f5 = ff.parse('s(4,4)|v(str)').rename('f5')
         b2 = Bus.from_frames((f4, f5), name='b')
 
-        post = buses_to_hierarchy((b1, b2), (b1.name, b2.name), deepcopy_from_bus=False, init_exception_cls=ErrorInitYarn)
-
+        post = buses_to_iloc_hierarchy((b1, b2), deepcopy_from_bus=False, init_exception_cls=ErrorInitYarn)
         self.assertEqual(post.values.tolist(),
-                [['a', 'f1'], ['a', 'f2'], ['a', 'f3'], ['b', 'f4'], ['b', 'f5']])
+                [[0, 'f1'], [0, 'f2'], [0, 'f3'], [1, 'f4'], [1, 'f5']]
+                )
 
     def test_buses_to_hierarchy_b(self) -> None:
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
         b1 = Bus.from_frames((f1, f2, f3), name='foo')
 
         f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
         f5 = ff.parse('s(4,4)|v(str)').rename('f5')
         b2 = Bus.from_frames((f4, f5), name='foo')
 
-        with self.assertRaises(ErrorInitYarn):
-            _ = buses_to_hierarchy((b1, b2),
-                    (b1.name, b2.name),
-                    deepcopy_from_bus=False,
-                    init_exception_cls=ErrorInitYarn)
+        post = buses_to_iloc_hierarchy((b1, b2),
+                deepcopy_from_bus=False,
+                init_exception_cls=ErrorInitYarn)
+        self.assertEqual(post.values.tolist(),
+                [[0, 'f1'], [0, 'f2'], [0, 'f3'], [1, 'f4'], [1, 'f5']],
+                )
+    def test_buses_to_hierarchy_c(self) -> None:
+
+        f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
+        f2 = ff.parse('s(4,4)|v(str)').rename('f2')
+        f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
+        b1 = Bus.from_frames((f1, f2, f3), name='a')
+
+        f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
+        f5 = ff.parse('s(4,4)|v(str)').rename('f5')
+        b2 = Bus.from_frames((f4, f5), name='b')
 
+        post = buses_to_iloc_hierarchy((b1, b2), deepcopy_from_bus=False, init_exception_cls=ErrorInitYarn)
+        self.assertEqual(post.values.tolist(),
+                [[0, 'f1'], [0, 'f2'], [0, 'f3'], [1, 'f4'], [1, 'f5']]
+                )
 
 if __name__ == '__main__':
     import unittest
     unittest.main()
```

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_batch.py` & `static-frame-2.5.2/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_bus.py` & `static-frame-2.5.2/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_container.py` & `static-frame-2.5.2/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_container_util.py` & `static-frame-2.5.2/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_display.py` & `static-frame-2.5.2/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_display_color.py` & `static-frame-2.5.2/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_doc.py` & `static-frame-2.5.2/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-2.5.2/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame_he.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame_iter.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame_join.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_frame_via_re.py` & `static-frame-2.5.2/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_hloc.py` & `static-frame-2.5.2/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index.py` & `static-frame-2.5.2/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_auto.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_base.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_correspondence.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_datetime.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-2.5.2/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_interface.py` & `static-frame-2.5.2/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_loc_map.py` & `static-frame-2.5.2/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_memory_measure.py` & `static-frame-2.5.2/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-2.5.2/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,15 +569,15 @@
         f4 = ff.parse('s(4,4)|v(int,float)').rename('f4')
         f5 = ff.parse('s(4,4)|v(str)').rename('f5')
         b2 = Bus.from_frames((f4, f5))
 
         y = Yarn((b1, b2))
         seen: tp.Set[int] = set()
         self.assertEqual(memory_total(y), sum(memory_total(e, seen=seen) for e in (
-            y._series,
+            y._values,
             y._hierarchy,
             y._index,
             y._deepcopy_from_bus,
         )) + getsizeof(y))
 
     #---------------------------------------------------------------------------
     # Quilt
```

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_metadata.py` & `static-frame-2.5.2/static_frame/test/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_pivot.py` & `static-frame-2.5.2/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-2.5.2/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_quilt.py` & `static-frame-2.5.2/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_rank.py` & `static-frame-2.5.2/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_series.py` & `static-frame-2.5.2/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_series_he.py` & `static-frame-2.5.2/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store.py` & `static-frame-2.5.2/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store_filter.py` & `static-frame-2.5.2/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store_hdf5.py` & `static-frame-2.5.2/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store_sqlite.py` & `static-frame-2.5.2/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store_xlsx.py` & `static-frame-2.5.2/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_store_zip.py` & `static-frame-2.5.2/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_style_config.py` & `static-frame-2.5.2/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_type_blocks.py` & `static-frame-2.5.2/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_type_clinic.py` & `static-frame-2.5.2/static_frame/test/unit/test_type_clinic.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_util.py` & `static-frame-2.5.2/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_www.py` & `static-frame-2.5.2/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.5.1/static_frame/test/unit/test_yarn.py` & `static-frame-2.5.2/static_frame/test/unit/test_yarn.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame import HLoc
 from static_frame import ILoc
 from static_frame.core.bus import Bus
 from static_frame.core.display_config import DisplayConfig
-from static_frame.core.exception import ErrorInitSeries
 from static_frame.core.exception import ErrorInitYarn
 from static_frame.core.exception import RelabelInvalid
 from static_frame.core.frame import Frame
 from static_frame.core.index_auto import IndexAutoFactory
 from static_frame.core.index_datetime import IndexDate
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.series import Series
@@ -25,15 +24,15 @@
 
 class TestUnit(TestCase):
 
     #---------------------------------------------------------------------------
 
     def test_yarn_init_a(self) -> None:
 
-        with self.assertRaises(ErrorInitSeries):
+        with self.assertRaises(ErrorInitYarn):
             Yarn(np.array([3, 4]))
 
     def test_yarn_init_b(self) -> None:
 
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
@@ -67,14 +66,39 @@
             Yarn(Series((ff.parse('s(2,2)'),), dtype=object))
 
     def test_yarn_init_d(self) -> None:
 
         with self.assertRaises(ErrorInitYarn):
             Yarn(Series(np.array((False, True))))
 
+    def test_yarn_init_e1(self) -> None:
+        b1 = Bus.from_frames((ff.parse("s(3,3)").rename("f1"),)).rename('x')
+        b2 = Bus.from_frames((ff.parse("s(3,4)").rename("f2"),)).rename('x')
+        b3 = Bus.from_frames((ff.parse("s(3,2)").rename("f3"),)).rename('x')
+        y1 = Yarn.from_buses((b1, b2, b3), retain_labels=True)
+        self.assertEqual(y1.index.values.tolist(),
+            [['x', 'f1'], ['x', 'f2'], ['x', 'f3']]
+            )
+        self.assertEqual(y1[('x', 'f3')].shape, (3, 2))
+
+        y2 = y1[('x', 'f2'):]
+        self.assertEqual(y2.index.values.tolist(),
+            [['x', 'f2'], ['x', 'f3']]
+            )
+
+
+    def test_yarn_init_e2(self) -> None:
+        b1 = Bus.from_frames((ff.parse("s(3,3)").rename("f1"),))
+        b2 = Bus.from_frames((ff.parse("s(3,4)").rename("f2"),))
+        b3 = Bus.from_frames((ff.parse("s(3,2)").rename("f3"),))
+        y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
+        self.assertEqual(y1.index.values.tolist(), ['f1', 'f2', 'f3'])
+        self.assertEqual(y1['f3'].shape, (3, 2))
+
+
     #---------------------------------------------------------------------------
 
     def test_yarn_from_buses_a(self) -> None:
 
         f1 = ff.parse('s(4,4)|v(int,float)').rename('f1')
         f2 = ff.parse('s(4,4)|v(str)').rename('f2')
         f3 = ff.parse('s(4,4)|v(bool)').rename('f3')
@@ -882,15 +906,15 @@
         b1 = Bus.from_frames((f1, f2, f3), name='b1')
         b2 = Bus.from_frames((f4,), name='b2')
         b3 = Bus.from_frames((f5, f6), name='b3')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
 
         y2 = y1.drop['f3':'f5'] #type: ignore
-        self.assertEqual(len(y2._series), 2) # 2 buses remain
+        self.assertEqual(len(y2._values), 2) # 2 buses remain
         self.assertEqual([(f.name, f.shape) for f in y2.values],
                 [('f1', (4, 2)), ('f2', (4, 5)), ('f6', (6, 4))]
                 )
 
         y3 = y1.drop[y1.index.isin(('f1', 'f6'))]
         self.assertEqual([(f.name, f.shape) for f in y3.values],
                 [('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8)), ('f5', (4, 4))]
@@ -917,15 +941,15 @@
         b1 = Bus.from_frames((f1, f2, f3), name='b1')
         b2 = Bus.from_frames((f4,), name='b2')
         b3 = Bus.from_frames((f5, f6), name='b3')
 
         y1 = Yarn.from_buses((b1, b2, b3), retain_labels=False)
 
         y2 = y1.drop.iloc[2: 5]
-        self.assertEqual(len(y2._series), 2) # 2 buses remain
+        self.assertEqual(len(y2._values), 2) # 2 buses remain
         self.assertEqual([(f.name, f.shape) for f in y2.values],
                 [('f1', (4, 2)), ('f2', (4, 5)), ('f6', (6, 4))]
                 )
 
         y3 = y1.drop.iloc[np.array([True, False, False, False, False, True])]
         self.assertEqual([(f.name, f.shape) for f in y3.values],
                 [('f2', (4, 5)), ('f3', (2, 2)), ('f4', (2, 8)), ('f5', (4, 4))]
```

### Comparing `static-frame-2.5.1/static_frame.egg-info/PKG-INFO` & `static-frame-2.5.2/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.5.1
+Version: 2.5.2
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `static-frame-2.5.1/static_frame.egg-info/SOURCES.txt` & `static-frame-2.5.2/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

