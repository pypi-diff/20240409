# Comparing `tmp/pylib_0xe-0.0.4.tar.gz` & `tmp/pylib-0xe-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib_0xe-0.0.4.tar", last modified: Sat Dec  2 16:02:35 2023, max compression
+gzip compressed data, was "pylib-0xe-0.0.5.tar", last modified: Tue Apr  9 11:25:11 2024, max compression
```

## Comparing `pylib_0xe-0.0.4.tar` & `pylib-0xe-0.0.5.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1093 2023-11-25 12:41:02.000000 pylib_0xe-0.0.4/LICENSE
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       65 2023-11-25 20:49:20.000000 pylib_0xe-0.0.4/MANIFEST.in
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     9292 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/PKG-INFO
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     7521 2023-12-02 13:33:15.000000 pylib_0xe-0.0.4/README.md
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      822 2023-12-02 16:02:24.000000 pylib_0xe-0.0.4/pyproject.toml
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/setup.cfg
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.913132 pylib_0xe-0.0.4/src/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        1 2023-08-07 06:45:27.000000 pylib_0xe-0.0.4/src/pylib_0xe/__init__.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.913132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/flows/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2997 2023-11-19 12:02:38.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/flows/maxflow.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1248 2023-11-19 12:02:59.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/mst.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1372 2023-11-19 12:03:05.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/tsp.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/math/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     7012 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/math/geometry.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.913132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     3170 2023-12-02 13:18:41.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/divide_and_conquer.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       85 2023-11-19 12:05:03.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/merge_types.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      261 2023-11-19 12:09:55.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/node_wrapper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/string_processing/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      742 2023-11-19 12:08:57.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/string_processing/lis.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.913132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/avl_tree/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1182 2023-12-02 13:17:32.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/avl_tree/avl_node.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     3736 2023-11-19 12:50:14.000000 pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/avl_tree/avl_tree.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/argument/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1720 2023-11-19 11:57:39.000000 pylib_0xe-0.0.4/src/pylib_0xe/argument/argument_parser.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      273 2023-11-19 12:57:54.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/buffer.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     3053 2023-11-19 13:19:34.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/buffer_reader.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      768 2023-11-19 12:27:01.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/buffer_writer.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      504 2023-08-07 06:20:55.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/file_buffer.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/helpers/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1749 2023-08-07 07:47:05.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/helpers/character_detector.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      208 2023-08-07 07:47:12.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/helpers/character_types.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      687 2023-11-19 13:27:33.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/standard_input_buffer.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      249 2023-11-19 11:57:39.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/standard_output_buffer.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      712 2023-08-07 06:20:55.000000 pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/string_buffer.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/config/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      987 2023-12-02 09:43:14.000000 pylib_0xe-0.0.4/src/pylib_0xe/config/config.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/data/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1082 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/data/data_transfer_object.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      725 2023-11-19 11:57:39.000000 pylib_0xe-0.0.4/src/pylib_0xe/data/variable_type_modifier.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/debug_tools/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1513 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/debug_tools/debug_text.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1807 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/debug_tools/terminal_process.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/file/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     2245 2023-11-19 12:21:52.000000 pylib_0xe-0.0.4/src/pylib_0xe/file/file.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/json/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     5792 2023-11-19 12:23:49.000000 pylib_0xe-0.0.4/src/pylib_0xe/json/json_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/path/
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1231 2023-12-02 13:22:05.000000 pylib_0xe-0.0.4/src/pylib_0xe/path/path_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/py.typed
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/string/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      393 2023-11-19 12:11:17.000000 pylib_0xe-0.0.4/src/pylib_0xe/string/hash_generator.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1658 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/string/string_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe/tests/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      299 2023-11-19 13:43:42.000000 pylib_0xe-0.0.4/src/pylib_0xe/tests/test_debug_text.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1112 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/tests/test_dto.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1712 2023-11-19 12:25:34.000000 pylib_0xe-0.0.4/src/pylib_0xe/tests/test_json_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      271 2023-12-02 13:25:08.000000 pylib_0xe-0.0.4/src/pylib_0xe/tests/test_path_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      803 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/src/pylib_0xe/tests/test_string_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     9292 2023-12-02 16:02:35.000000 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/PKG-INFO
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1947 2023-12-02 16:02:35.000000 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/SOURCES.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2023-12-02 16:02:35.000000 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/dependency_links.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2023-12-02 16:02:35.000000 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/requires.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       10 2023-12-02 16:02:35.000000 pylib_0xe-0.0.4/src/pylib_0xe.egg-info/top_level.txt
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-12-02 16:02:35.917132 pylib_0xe-0.0.4/tests/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      299 2023-11-19 13:43:42.000000 pylib_0xe-0.0.4/tests/test_debug_text.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1112 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/tests/test_dto.py
--rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1712 2023-11-19 12:25:34.000000 pylib_0xe-0.0.4/tests/test_json_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      271 2023-12-02 13:25:08.000000 pylib_0xe-0.0.4/tests/test_path_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      803 2023-11-28 17:19:40.000000 pylib_0xe-0.0.4/tests/test_string_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1093 2023-11-25 12:41:02.000000 pylib-0xe-0.0.5/LICENSE
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       65 2024-04-09 11:19:59.000000 pylib-0xe-0.0.5/MANIFEST.in
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)    11180 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/PKG-INFO
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     9409 2024-04-07 22:53:08.000000 pylib-0xe-0.0.5/README.md
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      822 2024-04-09 11:24:51.000000 pylib-0xe-0.0.5/pyproject.toml
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/setup.cfg
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     9409 2024-04-07 22:53:08.000000 pylib-0xe-0.0.5/src/pylib_0xe/README.md
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        1 2023-08-07 06:45:27.000000 pylib-0xe-0.0.5/src/pylib_0xe/__init__.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/flows/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2997 2023-11-19 12:02:38.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/flows/maxflow.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1248 2023-11-19 12:02:59.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/mst.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1372 2023-11-19 12:03:05.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/tsp.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/math/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     7012 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/math/geometry.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     3170 2023-12-02 13:18:41.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/divide_and_conquer.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       85 2023-11-19 12:05:03.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/merge_types.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      261 2023-11-19 12:09:55.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/node_wrapper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/string_processing/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      742 2023-11-19 12:08:57.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/string_processing/lis.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.549825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/avl_tree/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1182 2023-12-02 13:17:32.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/avl_tree/avl_node.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     3736 2023-11-19 12:50:14.000000 pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/avl_tree/avl_tree.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/argument/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1720 2023-11-19 11:57:39.000000 pylib-0xe-0.0.5/src/pylib_0xe/argument/argument_parser.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      273 2023-11-19 12:57:54.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/buffer.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     3053 2023-11-19 13:19:34.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/buffer_reader.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      768 2023-11-19 12:27:01.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/buffer_writer.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      504 2023-08-07 06:20:55.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/file_buffer.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/helpers/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1749 2023-08-07 07:47:05.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/helpers/character_detector.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      208 2023-08-07 07:47:12.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/helpers/character_types.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      687 2023-11-19 13:27:33.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/standard_input_buffer.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      249 2023-11-19 11:57:39.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/standard_output_buffer.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      712 2023-08-07 06:20:55.000000 pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/string_buffer.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/config/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      996 2024-04-08 12:39:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/config/config.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/data/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1508 2024-04-08 14:42:26.000000 pylib-0xe-0.0.5/src/pylib_0xe/data/data_transfer_object.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)      725 2023-11-19 11:57:39.000000 pylib-0xe-0.0.5/src/pylib_0xe/data/variable_type_modifier.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/debug_tools/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1513 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/debug_tools/debug_text.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1807 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/debug_tools/terminal_process.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/file/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     2245 2023-11-19 12:21:52.000000 pylib-0xe-0.0.5/src/pylib_0xe/file/file.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/json/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     5792 2023-11-19 12:23:49.000000 pylib-0xe-0.0.5/src/pylib_0xe/json/json_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/path/
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1274 2024-04-08 13:20:51.000000 pylib-0xe-0.0.5/src/pylib_0xe/path/path_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/py.typed
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/string/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      393 2023-11-19 12:11:17.000000 pylib-0xe-0.0.5/src/pylib_0xe/string/hash_generator.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1658 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/string/string_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe/tests/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      299 2023-11-19 13:43:42.000000 pylib-0xe-0.0.5/src/pylib_0xe/tests/test_debug_text.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1112 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/tests/test_dto.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1712 2023-11-19 12:25:34.000000 pylib-0xe-0.0.5/src/pylib_0xe/tests/test_json_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      271 2023-12-02 13:25:08.000000 pylib-0xe-0.0.5/src/pylib_0xe/tests/test_path_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      803 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/src/pylib_0xe/tests/test_string_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)    11180 2024-04-09 11:25:11.000000 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/PKG-INFO
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1971 2024-04-09 11:25:11.000000 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/SOURCES.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2024-04-09 11:25:11.000000 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/dependency_links.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2024-04-09 11:25:11.000000 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/requires.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       10 2024-04-09 11:25:11.000000 pylib-0xe-0.0.5/src/pylib_0xe.egg-info/top_level.txt
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:25:11.553825 pylib-0xe-0.0.5/tests/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      299 2023-11-19 13:43:42.000000 pylib-0xe-0.0.5/tests/test_debug_text.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1112 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/tests/test_dto.py
+-rwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)     1712 2023-11-19 12:25:34.000000 pylib-0xe-0.0.5/tests/test_json_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      271 2023-12-02 13:25:08.000000 pylib-0xe-0.0.5/tests/test_path_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      803 2023-11-28 17:19:40.000000 pylib-0xe-0.0.5/tests/test_string_helper.py
```

### Comparing `pylib_0xe-0.0.4/LICENSE` & `pylib-0xe-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/PKG-INFO` & `pylib-0xe-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: pylib_0xe
-Version: 0.0.4
-Summary: Yet Another Python Library
-Author-email: shamir0xe <shamir0xe@gmail.com>
-License: The MIT License (MIT)
-        Copyright © 2023 <copyright holders>
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-        
-Project-URL: Homepage, https://github.com/shamir0xe/pylib
-Keywords: library,buffer,reader/writer,algorithm,datastructure,file
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: unittest; extra == "dev"
-
 
 <h1 align="center" style="display: block; font-size: 2.5em; font-weight: bold; margin-block-start: 1em; margin-block-end: 1em;">
 <a name="logo" href="#"><img align="center" src="https://github.com/shamir0xe/pylib/blob/main/assets/logos/pylib.png?raw=true" alt="pylib" style="width:100%;height:100%"/></a>
 <br/><br/><strong>pylib</strong>
 </h1>
 
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@@ -76,44 +49,98 @@
 This module provides several ways to read, write and edit buffers.
 You can define `file`, `str` and `standard-input` buffers.
 
 - [Buffer](buffer_io/buffer.py)
 - [BufferReader](buffer_io/buffer_reader.py)
 - [BufferWriter](buffer_io/buffer_writer.py)
 - [StandardInputBuffer](buffer_io/standard_input_buffer.py)
+- [StandardOutputBuffer](buffer_io/standard_output_buffer.py)
 - [FileBuffer](buffer_io/file_buffer.py)
 - [StringBuffer](buffer_io/string_buffer.py)
 
 for example you can simply read a whole file like this:
 
 ```python
-reader = BufferReader(FileBuffer(file_path))
+reader = BufferReader(FileBuffer(file_path, "r+"))
 while not reader.end_of_buffer():
     line = reader.next_line()
 ```
 
 or you can define a string as a buffer and treat it in the same way:
 
 ```python
 reader = BufferReader(StringBuffer('some awesome text'))
 while not reader.end_of_buffer():
     a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
 ```
 
+you can also read from `standard_input` and write to `standard_output`
+in this way:
+
+```python
+reader = BufferReader(StandardInputBuffer())
+writer = BufferWriter(StandardOutputBuffer())
+while not reader.end_of_buffer():
+    a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
+    writer.write_line(f"We have recieved these: ({a}, {b}, {c})")
+```
+
 ### Data
 
 - [DataTransferObject](data/data_transfer_object.py):
 A tool for converting dictionaries to objects. example:
 
  ```python
  obj = DataTransferObject.from_dict({'a': 123})
  print(obj.a)
 #  123
  ```
 
+DataTransferObject is a dataclass itself. The best practice to use
+this dto class is inheritting it as the base
+class for your model. For example If your new model is named Bob and
+has two parameters `name` and `height` with types `str` and `Optional[int]`
+respectively, it should be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+```
+
+and then you can instantiate it in this way:
+
+```python
+  bob_marley = Bob({name: "Bob Marley"})
+```
+
+and you can use `bob_marley.name` and `bob_marley.height` in your code
+since now on.
+Another cool feature of this dto is implementing `mapper` function for
+any variable of your choice. It works this way that you can define a
+mapper function with this style: `VARIABLENAME_mapper`. It recieves
+it's argument from the dictionary you provided to instantiate it and convert
+the input to whatever you implement it in the function. This could be
+useful if the types of the input data differs from the expected type
+provided in the class or if you want to change the value of the variable
+in some way before creating it. For example if you want `Bob` to convert it's
+name to upper_case letters, it could be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+
+  def name_mapper(name: str) -> str:
+    return name.lower()
+
+```
+
 - [VariableTypeModifier](data/variable_type_modifier.py):
 Converting types by casting it in a better way.
 
 ### Debug Tools
 
 - [debug_text](debug_tools/debug_text.py): Alternative way to debuging
 the code via prints into the stderr. example:
@@ -209,25 +236,26 @@
   as a kwarg.
   Then the above example could be rewritten as something like this:
 
 ```python
 path = PathHelper.from_root(..., root_name="custom_name")
 ```
 
-The best practice to use it with custom root directory is to write a new PathHelper
-  class that extends this class and apply your custom `root_name` to it. It should
-be implemented like this:
+The best practice to use it with the custom root directory is to write a new PathHelper
+class that extends `PathHelper` and apply your custom `root_name` to it. You can
+also get rid of `__file__` argument in this way. It should be implemented
+something like this:
 
   ```python
   from pylib_0xe.path.path_helper import PathHelper as PH
 
 
   class PathHelper(PH):
     @classmethod
-    def from_root(cls, *path: str) -> str:
+    def root(cls, *path: str) -> str:
       return cls.from_root(__file__, *path, root_name="custom_name")
   ```
 
 ### Argument
 
 - [ArgumentParser](argument/argument_parser.py):
 Useful tool to reading arguments passed to a python program executed via command line interface (terminal).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pylib_0xe-0.0.4/README.md` & `pylib-0xe-0.0.5/src/pylib_0xe/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,44 +49,98 @@
 This module provides several ways to read, write and edit buffers.
 You can define `file`, `str` and `standard-input` buffers.
 
 - [Buffer](buffer_io/buffer.py)
 - [BufferReader](buffer_io/buffer_reader.py)
 - [BufferWriter](buffer_io/buffer_writer.py)
 - [StandardInputBuffer](buffer_io/standard_input_buffer.py)
+- [StandardOutputBuffer](buffer_io/standard_output_buffer.py)
 - [FileBuffer](buffer_io/file_buffer.py)
 - [StringBuffer](buffer_io/string_buffer.py)
 
 for example you can simply read a whole file like this:
 
 ```python
-reader = BufferReader(FileBuffer(file_path))
+reader = BufferReader(FileBuffer(file_path, "r+"))
 while not reader.end_of_buffer():
     line = reader.next_line()
 ```
 
 or you can define a string as a buffer and treat it in the same way:
 
 ```python
 reader = BufferReader(StringBuffer('some awesome text'))
 while not reader.end_of_buffer():
     a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
 ```
 
+you can also read from `standard_input` and write to `standard_output`
+in this way:
+
+```python
+reader = BufferReader(StandardInputBuffer())
+writer = BufferWriter(StandardOutputBuffer())
+while not reader.end_of_buffer():
+    a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
+    writer.write_line(f"We have recieved these: ({a}, {b}, {c})")
+```
+
 ### Data
 
 - [DataTransferObject](data/data_transfer_object.py):
 A tool for converting dictionaries to objects. example:
 
  ```python
  obj = DataTransferObject.from_dict({'a': 123})
  print(obj.a)
 #  123
  ```
 
+DataTransferObject is a dataclass itself. The best practice to use
+this dto class is inheritting it as the base
+class for your model. For example If your new model is named Bob and
+has two parameters `name` and `height` with types `str` and `Optional[int]`
+respectively, it should be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+```
+
+and then you can instantiate it in this way:
+
+```python
+  bob_marley = Bob({name: "Bob Marley"})
+```
+
+and you can use `bob_marley.name` and `bob_marley.height` in your code
+since now on.
+Another cool feature of this dto is implementing `mapper` function for
+any variable of your choice. It works this way that you can define a
+mapper function with this style: `VARIABLENAME_mapper`. It recieves
+it's argument from the dictionary you provided to instantiate it and convert
+the input to whatever you implement it in the function. This could be
+useful if the types of the input data differs from the expected type
+provided in the class or if you want to change the value of the variable
+in some way before creating it. For example if you want `Bob` to convert it's
+name to upper_case letters, it could be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+
+  def name_mapper(name: str) -> str:
+    return name.lower()
+
+```
+
 - [VariableTypeModifier](data/variable_type_modifier.py):
 Converting types by casting it in a better way.
 
 ### Debug Tools
 
 - [debug_text](debug_tools/debug_text.py): Alternative way to debuging
 the code via prints into the stderr. example:
@@ -182,25 +236,26 @@
   as a kwarg.
   Then the above example could be rewritten as something like this:
 
 ```python
 path = PathHelper.from_root(..., root_name="custom_name")
 ```
 
-The best practice to use it with custom root directory is to write a new PathHelper
-  class that extends this class and apply your custom `root_name` to it. It should
-be implemented like this:
+The best practice to use it with the custom root directory is to write a new PathHelper
+class that extends `PathHelper` and apply your custom `root_name` to it. You can
+also get rid of `__file__` argument in this way. It should be implemented
+something like this:
 
   ```python
   from pylib_0xe.path.path_helper import PathHelper as PH
 
 
   class PathHelper(PH):
     @classmethod
-    def from_root(cls, *path: str) -> str:
+    def root(cls, *path: str) -> str:
       return cls.from_root(__file__, *path, root_name="custom_name")
   ```
 
 ### Argument
 
 - [ArgumentParser](argument/argument_parser.py):
 Useful tool to reading arguments passed to a python program executed via command line interface (terminal).
```

### Comparing `pylib_0xe-0.0.4/pyproject.toml` & `pylib-0xe-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pyproject.toml
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "pylib_0xe"
-version = "0.0.4"
+name = "pylib-0xe"
+version = "0.0.5"
 description = "Yet Another Python Library"
 readme = "README.md"
 authors = [{ name = "shamir0xe", email = "shamir0xe@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/flows/maxflow.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/flows/maxflow.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/mst.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/mst.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/graph/tsp.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/graph/tsp.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/math/geometry.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/math/geometry.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/divide_and_conquer.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/paradigms/divide_and_conquer/divide_and_conquer.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/string_processing/lis.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/string_processing/lis.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/avl_tree/avl_node.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/avl_tree/avl_node.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/algorithms/trees/avl_tree/avl_tree.py` & `pylib-0xe-0.0.5/src/pylib_0xe/algorithms/trees/avl_tree/avl_tree.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/argument/argument_parser.py` & `pylib-0xe-0.0.5/src/pylib_0xe/argument/argument_parser.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/buffer_reader.py` & `pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/buffer_reader.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/buffer_writer.py` & `pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/buffer_writer.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/helpers/character_detector.py` & `pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/helpers/character_detector.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/standard_input_buffer.py` & `pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/standard_input_buffer.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/buffer_io/string_buffer.py` & `pylib-0xe-0.0.5/src/pylib_0xe/buffer_io/string_buffer.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/config/config.py` & `pylib-0xe-0.0.5/src/pylib_0xe/config/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Any
+from dataclasses import dataclass
 from ..file.file import File
 from ..path.path_helper import PathHelper
 from ..json.json_helper import JsonHelper
 
 
+@dataclass
 class Config:
-    DEFAULT_CONFIG_FOLDER_NAME = "configs"
+    file_path: str = __file__
+    file_format: str = ".json"
+    folder_name: str = "configs"
 
-    def __init__(
-        self,
-        filename: str,
-        config_folder_name: str = DEFAULT_CONFIG_FOLDER_NAME,
-    ) -> None:
-        filename += ".json"
-        self.json = File.read_json(
-            PathHelper.from_root(__file__, config_folder_name, filename)
+    def get(self, filename: str, selector: str = "", default: Any = None) -> Any:
+        json = File.read_json(
+            PathHelper.from_root(
+                self.file_path, self.folder_name, filename + self.file_format
+            )
         )
-
-    def get(self, selector: str = "", default: Any = None) -> Any:
-        value = JsonHelper.selector_get_value(self.json, selector)
+        value = JsonHelper.selector_get_value(json, selector)
         if value != {}:
             return value
         return default
 
-    @staticmethod
-    def read(selector: str, **kwargs) -> Any:
+    def read(self, selector: str, **kwargs) -> Any:
         index = selector.find(".")
         if index < 0:
-            return Config(selector).get(**kwargs)
-        filename = selector[:index]
-        selector = selector[index + 1 :]
-        return Config(filename).get(selector, **kwargs)
+            filename = selector
+            selector = ""
+        else:
+            filename = selector[:index]
+            selector = selector[index + 1 :]
+        return self.get(filename, selector, **kwargs)
```

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/data/variable_type_modifier.py` & `pylib-0xe-0.0.5/src/pylib_0xe/data/variable_type_modifier.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/debug_tools/debug_text.py` & `pylib-0xe-0.0.5/src/pylib_0xe/debug_tools/debug_text.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/debug_tools/terminal_process.py` & `pylib-0xe-0.0.5/src/pylib_0xe/debug_tools/terminal_process.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/file/file.py` & `pylib-0xe-0.0.5/src/pylib_0xe/file/file.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/json/json_helper.py` & `pylib-0xe-0.0.5/src/pylib_0xe/json/json_helper.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/path/path_helper.py` & `pylib-0xe-0.0.5/src/pylib_0xe/path/path_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,23 @@
         res = ""
         try:
             res = PathHelper.backward(path)
         except Exception:
             pass
         return res
 
-    @classmethod
-    def from_root(cls, file_path: str, *path: str, **kwargs) -> str:
+    @staticmethod
+    def from_root(file_path: str, *path: str, **kwargs) -> str:
         """
         assuming the arcitecture is like src/... or root/...,
         it'll go back till reach {src, root} folders
         """
-        instance = PathHelper(file_path)
+        instance: PathHelper
         if "root_name" in kwargs:
             instance = PathHelper(file_path, [kwargs["root_name"]])
+        else:
+            instance = PathHelper(file_path)
         return os.path.normpath(os.path.join(instance.root_path(), *path))
 
     @staticmethod
     def backward(path: str) -> str:
         return os.path.normpath(os.path.join(path, ".."))
```

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/string/string_helper.py` & `pylib-0xe-0.0.5/src/pylib_0xe/string/string_helper.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/tests/test_dto.py` & `pylib-0xe-0.0.5/src/pylib_0xe/tests/test_dto.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/tests/test_json_helper.py` & `pylib-0xe-0.0.5/src/pylib_0xe/tests/test_json_helper.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe/tests/test_string_helper.py` & `pylib-0xe-0.0.5/src/pylib_0xe/tests/test_string_helper.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe.egg-info/PKG-INFO` & `pylib-0xe-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylib-0xe
-Version: 0.0.4
+Version: 0.0.5
 Summary: Yet Another Python Library
 Author-email: shamir0xe <shamir0xe@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -76,44 +76,98 @@
 This module provides several ways to read, write and edit buffers.
 You can define `file`, `str` and `standard-input` buffers.
 
 - [Buffer](buffer_io/buffer.py)
 - [BufferReader](buffer_io/buffer_reader.py)
 - [BufferWriter](buffer_io/buffer_writer.py)
 - [StandardInputBuffer](buffer_io/standard_input_buffer.py)
+- [StandardOutputBuffer](buffer_io/standard_output_buffer.py)
 - [FileBuffer](buffer_io/file_buffer.py)
 - [StringBuffer](buffer_io/string_buffer.py)
 
 for example you can simply read a whole file like this:
 
 ```python
-reader = BufferReader(FileBuffer(file_path))
+reader = BufferReader(FileBuffer(file_path, "r+"))
 while not reader.end_of_buffer():
     line = reader.next_line()
 ```
 
 or you can define a string as a buffer and treat it in the same way:
 
 ```python
 reader = BufferReader(StringBuffer('some awesome text'))
 while not reader.end_of_buffer():
     a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
 ```
 
+you can also read from `standard_input` and write to `standard_output`
+in this way:
+
+```python
+reader = BufferReader(StandardInputBuffer())
+writer = BufferWriter(StandardOutputBuffer())
+while not reader.end_of_buffer():
+    a, b, c = reader.next_int(), reader.next_string(), reader.next_char()
+    writer.write_line(f"We have recieved these: ({a}, {b}, {c})")
+```
+
 ### Data
 
 - [DataTransferObject](data/data_transfer_object.py):
 A tool for converting dictionaries to objects. example:
 
  ```python
  obj = DataTransferObject.from_dict({'a': 123})
  print(obj.a)
 #  123
  ```
 
+DataTransferObject is a dataclass itself. The best practice to use
+this dto class is inheritting it as the base
+class for your model. For example If your new model is named Bob and
+has two parameters `name` and `height` with types `str` and `Optional[int]`
+respectively, it should be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+```
+
+and then you can instantiate it in this way:
+
+```python
+  bob_marley = Bob({name: "Bob Marley"})
+```
+
+and you can use `bob_marley.name` and `bob_marley.height` in your code
+since now on.
+Another cool feature of this dto is implementing `mapper` function for
+any variable of your choice. It works this way that you can define a
+mapper function with this style: `VARIABLENAME_mapper`. It recieves
+it's argument from the dictionary you provided to instantiate it and convert
+the input to whatever you implement it in the function. This could be
+useful if the types of the input data differs from the expected type
+provided in the class or if you want to change the value of the variable
+in some way before creating it. For example if you want `Bob` to convert it's
+name to upper_case letters, it could be implemented like this:
+
+```python
+@dataclass
+class Bob(DataTransferObject):
+  name: str
+  height: int | None = 185
+
+  def name_mapper(name: str) -> str:
+    return name.lower()
+
+```
+
 - [VariableTypeModifier](data/variable_type_modifier.py):
 Converting types by casting it in a better way.
 
 ### Debug Tools
 
 - [debug_text](debug_tools/debug_text.py): Alternative way to debuging
 the code via prints into the stderr. example:
@@ -209,25 +263,26 @@
   as a kwarg.
   Then the above example could be rewritten as something like this:
 
 ```python
 path = PathHelper.from_root(..., root_name="custom_name")
 ```
 
-The best practice to use it with custom root directory is to write a new PathHelper
-  class that extends this class and apply your custom `root_name` to it. It should
-be implemented like this:
+The best practice to use it with the custom root directory is to write a new PathHelper
+class that extends `PathHelper` and apply your custom `root_name` to it. You can
+also get rid of `__file__` argument in this way. It should be implemented
+something like this:
 
   ```python
   from pylib_0xe.path.path_helper import PathHelper as PH
 
 
   class PathHelper(PH):
     @classmethod
-    def from_root(cls, *path: str) -> str:
+    def root(cls, *path: str) -> str:
       return cls.from_root(__file__, *path, root_name="custom_name")
   ```
 
 ### Argument
 
 - [ArgumentParser](argument/argument_parser.py):
 Useful tool to reading arguments passed to a python program executed via command line interface (terminal).
```

### Comparing `pylib_0xe-0.0.4/src/pylib_0xe.egg-info/SOURCES.txt` & `pylib-0xe-0.0.5/src/pylib_0xe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+src/pylib_0xe/README.md
 src/pylib_0xe/__init__.py
 src/pylib_0xe/py.typed
 src/pylib_0xe.egg-info/PKG-INFO
 src/pylib_0xe.egg-info/SOURCES.txt
 src/pylib_0xe.egg-info/dependency_links.txt
 src/pylib_0xe.egg-info/requires.txt
 src/pylib_0xe.egg-info/top_level.txt
```

### Comparing `pylib_0xe-0.0.4/tests/test_dto.py` & `pylib-0xe-0.0.5/tests/test_dto.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/tests/test_json_helper.py` & `pylib-0xe-0.0.5/tests/test_json_helper.py`

 * *Files identical despite different names*

### Comparing `pylib_0xe-0.0.4/tests/test_string_helper.py` & `pylib-0xe-0.0.5/tests/test_string_helper.py`

 * *Files identical despite different names*

