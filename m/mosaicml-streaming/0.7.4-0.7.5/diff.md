# Comparing `tmp/mosaicml-streaming-0.7.4.tar.gz` & `tmp/mosaicml-streaming-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.7.4.tar", last modified: Thu Feb  8 19:21:05 2024, max compression
+gzip compressed data, was "mosaicml-streaming-0.7.5.tar", last modified: Mon Apr  8 23:51:41 2024, max compression
```

## Comparing `mosaicml-streaming-0.7.4.tar` & `mosaicml-streaming-0.7.5.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.641159 mosaicml-streaming-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16170 2024-02-08 19:21:05.641159 mosaicml-streaming-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.613159 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16170 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-08 19:21:05.000000 mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15891 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 19:21:05.641159 mosaicml-streaming-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.613159 mosaicml-streaming-0.7.4/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.617159 mosaicml-streaming-0.7.4/simulation/core/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/last_used_ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/node_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/shard_downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/shuffle_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    24965 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/sim_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/sim_spanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/sim_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/sim_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/core/yaml_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.617159 mosaicml-streaming-0.7.4/simulation/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/sim_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/sim_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/sim_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    23474 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/interfaces/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/simulation/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.617159 mosaicml-streaming-0.7.4/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.621159 mosaicml-streaming-0.7.4/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.621159 mosaicml-streaming-0.7.4/streaming/base/batching/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/batching/per_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/batching/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/batching/stratified.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.621159 mosaicml-streaming-0.7.4/streaming/base/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/converters/dataframe_to_mds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    65897 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.621159 mosaicml-streaming-0.7.4/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.621159 mosaicml-streaming-0.7.4/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/base/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.625159 mosaicml-streaming-0.7.4/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.625159 mosaicml-streaming-0.7.4/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.625159 mosaicml-streaming-0.7.4/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.625159 mosaicml-streaming-0.7.4/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/partition/orig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/partition/relaxed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.625159 mosaicml-streaming-0.7.4/streaming/base/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shared/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/py1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/py1br.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/py1e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/shuffle/py2s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/spanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    45219 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.629159 mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/crawl_webvid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/extract_webvid_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)    21204 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/multimodal/webvid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.633159 mosaicml-streaming-0.7.4/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.633159 mosaicml-streaming-0.7.4/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.633159 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.633159 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.633159 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.637159 mosaicml-streaming-0.7.4/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.637159 mosaicml-streaming-0.7.4/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 19:21:05.641159 mosaicml-streaming-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11958 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_spanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    38925 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_unsafe_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-02-08 19:20:52.000000 mosaicml-streaming-0.7.4/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.839965 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.839965 mosaicml-streaming-0.7.5/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/simulation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/last_used_ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/node_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/shard_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/shuffle_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/yaml_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/simulation/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/batching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/per_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/stratified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/converters/dataframe_to_mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68222 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23447 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/orig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/relaxed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1br.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/spanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45219 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/webvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.863965 mosaicml-streaming-0.7.5/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39855 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_unsafe_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.7.4/LICENSE` & `mosaicml-streaming-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/PKG-INFO` & `mosaicml-streaming-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.7.4
+Version: 0.7.5
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: simulator
 Provides-Extra: spark
 Provides-Extra: databricks
+Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-mode.png" width="50%"/>
@@ -31,15 +32,15 @@
 
 <h2><p align="center">Fast, accurate streaming of training data from cloud storage</p></h2>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
 - <a href="https://streaming.docs.mosaicml.com/en/latest/getting_started/user_guide.html">[Getting Started]</a>
 - <a href="https://streaming.docs.mosaicml.com/">[Docs]
-- <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
+- <a href="https://www.mosaicml.com/careers">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml-streaming/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml-streaming">
     </a>
     <a href="https://pypi.org/project/mosaicml-streaming/">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.4 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.5 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: simulator Provides-Extra: spark Provides-Extra: databricks Provides-
-Extra: all License-File: LICENSE
+Extra: testing Provides-Extra: all License-File: LICENSE
 _[_h_t_t_p_s_:_/_/_s_t_o_r_a_g_e_._g_o_o_g_l_e_a_p_i_s_._c_o_m_/_d_o_c_s_._m_o_s_a_i_c_m_l_._c_o_m_/_i_m_a_g_e_s_/_s_t_r_e_a_m_i_n_g_-_l_o_g_o_-_l_i_g_h_t_-
                                    _m_o_d_e_._p_n_g_]
 ********** FFaasstt,, aaccccuurraattee ssttrreeaammiinngg ooff ttrraaiinniinngg ddaattaa ffrroomm cclloouudd ssttoorraaggee **********
 ****** _[[_WW_ee_bb_ss_ii_tt_ee_]] -- _[[_GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd_]] -- _[[_DD_oo_cc_ss_]]_ _--_ _[[_WW_ee_''_rr_ee_ _HH_ii_rr_ii_nn_gg_!!_]] ******
 _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_U_n_i_t_ _t_e_s_t_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
                             _[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
```

### Comparing `mosaicml-streaming-0.7.4/README.md` & `mosaicml-streaming-0.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 <h2><p align="center">Fast, accurate streaming of training data from cloud storage</p></h2>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
 - <a href="https://streaming.docs.mosaicml.com/en/latest/getting_started/user_guide.html">[Getting Started]</a>
 - <a href="https://streaming.docs.mosaicml.com/">[Docs]
-- <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
+- <a href="https://www.mosaicml.com/careers">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml-streaming/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml-streaming">
     </a>
     <a href="https://pypi.org/project/mosaicml-streaming/">
```

### Comparing `mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.7.4
+Version: 0.7.5
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: simulator
 Provides-Extra: spark
 Provides-Extra: databricks
+Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
       <img src="https://storage.googleapis.com/docs.mosaicml.com/images/streaming-logo-light-mode.png" width="50%"/>
@@ -31,15 +32,15 @@
 
 <h2><p align="center">Fast, accurate streaming of training data from cloud storage</p></h2>
 
 <h4><p align='center'>
 <a href="https://www.mosaicml.com">[Website]</a>
 - <a href="https://streaming.docs.mosaicml.com/en/latest/getting_started/user_guide.html">[Getting Started]</a>
 - <a href="https://streaming.docs.mosaicml.com/">[Docs]
-- <a href="https://www.mosaicml.com/team">[We're Hiring!]</a>
+- <a href="https://www.mosaicml.com/careers">[We're Hiring!]</a>
 </p></h4>
 
 <p align="center">
     <a href="https://pypi.org/project/mosaicml-streaming/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mosaicml-streaming">
     </a>
     <a href="https://pypi.org/project/mosaicml-streaming/">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.4 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.5 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: simulator Provides-Extra: spark Provides-Extra: databricks Provides-
-Extra: all License-File: LICENSE
+Extra: testing Provides-Extra: all License-File: LICENSE
 _[_h_t_t_p_s_:_/_/_s_t_o_r_a_g_e_._g_o_o_g_l_e_a_p_i_s_._c_o_m_/_d_o_c_s_._m_o_s_a_i_c_m_l_._c_o_m_/_i_m_a_g_e_s_/_s_t_r_e_a_m_i_n_g_-_l_o_g_o_-_l_i_g_h_t_-
                                    _m_o_d_e_._p_n_g_]
 ********** FFaasstt,, aaccccuurraattee ssttrreeaammiinngg ooff ttrraaiinniinngg ddaattaa ffrroomm cclloouudd ssttoorraaggee **********
 ****** _[[_WW_ee_bb_ss_ii_tt_ee_]] -- _[[_GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd_]] -- _[[_DD_oo_cc_ss_]]_ _--_ _[[_WW_ee_''_rr_ee_ _HH_ii_rr_ii_nn_gg_!!_]] ******
 _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_U_n_i_t_ _t_e_s_t_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
                             _[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
```

### Comparing `mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/mosaicml_streaming.egg-info/requires.txt` & `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,89 +12,105 @@
 zstd<2,>=1.5.2.5
 oci<3,>=2.88
 azure-storage-blob<13,>=12.0.0
 azure-storage-file-datalake<13,>=12.11.0
 azure-identity>=1.13.0
 
 [all]
-GitPython==3.1.41
+GitPython==3.1.42
 PyYAML<7,>=6.0
 altair<6,>=5.1.1
-databricks-sdk==0.14.0
+databricks-sdk==0.23.0
 datasets<3,>=2.4.0
 docformatter>=1.4
-docutils==0.18.1
-fastapi==0.109.0
-furo==2023.7.26
+docutils==0.17.1
+fastapi==0.110.0
+furo==2022.9.29
 humanize<5,>=4.7.0
 jupyter==1.0.0
-moto<5,>=4.0
-myst-parser==2.0.0
-nbsphinx==0.9.2
+mosaicml-cli<0.7,>=0.5.25
+moto<6,>=4.0
+myst-parser==0.16.1
+nbsphinx==0.9.1
 omegaconf<3,>=2.3.0
 pandas<3,>=2.0.3
 pandoc==2.3
 pre-commit<4,>=2.18.1
 pyarrow>14.0.0
-pydantic==2.5.3
-pypandoc==1.12
+pydantic==2.6.4
+pypandoc==1.13
 pyspark<4,>=3
-pytest-cov<5,>=4
-pytest-split==0.8.1
-pytest==7.4.4
+pytest-cov<6,>=4
+pytest-split==0.8.2
+pytest==8.1.1
 pytest_codeblocks==0.17.0
 sortedcollections<3,>=2.1.0
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
 sphinx-tabs==3.4.5
-sphinx==6.2.1
+sphinx==4.4.0
+sphinxcontrib-applehelp==1.0.0
+sphinxcontrib-devhelp==1.0.0
+sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-qthelp==1.0.0
+sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib.katex==0.9.6
 streamlit<2,>=1.26.0
 toml==0.10.2
-uvicorn==0.26.0
+uvicorn==0.29.0
 wandb<1,>=0.15.5
-yamllint==1.33.0
+yamllint==1.35.1
 
 [databricks]
-databricks-sdk==0.14.0
+databricks-sdk==0.23.0
 
 [dev]
 datasets<3,>=2.4.0
 pyarrow>14.0.0
 docformatter>=1.4
 jupyter==1.0.0
 pre-commit<4,>=2.18.1
-pytest==7.4.4
+pytest==8.1.1
 pytest_codeblocks==0.17.0
-pytest-cov<5,>=4
+pytest-cov<6,>=4
 toml==0.10.2
-yamllint==1.33.0
-moto<5,>=4.0
-fastapi==0.109.0
-pydantic==2.5.3
-uvicorn==0.26.0
-pytest-split==0.8.1
+yamllint==1.35.1
+moto<6,>=4.0
+fastapi==0.110.0
+pydantic==2.6.4
+uvicorn==0.29.0
+pytest-split==0.8.2
 
 [docs]
-GitPython==3.1.41
-docutils==0.18.1
-furo==2023.7.26
-myst-parser==2.0.0
-nbsphinx==0.9.2
+GitPython==3.1.42
+docutils==0.17.1
+furo==2022.9.29
+myst-parser==0.16.1
+nbsphinx==0.9.1
 pandoc==2.3
-pypandoc==1.12
+pypandoc==1.13
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
-sphinx==6.2.1
+sphinx==4.4.0
 sphinx-tabs==3.4.5
+sphinxcontrib.katex==0.9.6
+sphinxcontrib-applehelp==1.0.0
+sphinxcontrib-devhelp==1.0.0
+sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-qthelp==1.0.0
+sphinxcontrib-serializinghtml==1.1.5
 
 [simulator]
 sortedcollections<3,>=2.1.0
 streamlit<2,>=1.26.0
 altair<6,>=5.1.1
 omegaconf<3,>=2.3.0
 PyYAML<7,>=6.0
 pandas<3,>=2.0.3
 wandb<1,>=0.15.5
 humanize<5,>=4.7.0
 
 [spark]
 pyspark<4,>=3
+
+[testing]
+mosaicml-cli<0.7,>=0.5.25
```

### Comparing `mosaicml-streaming-0.7.4/pyproject.toml` & `mosaicml-streaming-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,56 @@
 
 # iSort
 [tool.isort]
 multi_line_output = 0
 line_length = 99
 skip = [ "env", "wandb", "runs", "build", "node_modules" ]
 
+# ruff
+[tool.ruff.lint]
+select = [
+    "C4",
+    "D", # pydocstyle
+    "LOG",
+    "PERF",
+    "PLE",
+]
+ignore = [
+    "C408",
+    "D102",
+    "D105",
+    "D107",
+    "D203", # default ignore
+    "D212", # default ignore
+    "D213", # default ignore
+    "D401",
+    "D404", # default ignore
+    "D417", # ruff only rulecode
+    "E501",
+    "E722",
+    "E741",
+    "PERF2",
+    "PERF4",
+]
+
+[tool.ruff]
+exclude = [
+    "build/**",
+    "docs/**",
+    "node_modules/**",
+]
+
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
+[tool.ruff.lint.per-file-ignores]
+"tests/*" = ["D"]
+"streaming/text/convert/enwiki/*" = ["D"]
+
 # Pyright
 [tool.pyright]
 include = [
     "streaming/**",
     "tests/**",
 ]
 exclude = [
@@ -481,47 +523,14 @@
 # The penalty of splitting the line around the 'and' and 'or'
 # operators.
 split_penalty_logical_operator = 300
 
 # Use the Tab character for indentation.
 use_tabs = false
 
-[tool.ruff]
-select = [
-    "C4",
-    "D", # pydocstyle
-    "PERF",
-]
-
-ignore = [
-    "C408",
-    "D102",
-    "D105",
-    "D107",
-    "D203", # default ignore
-    "D212", # default ignore
-    "D213", # default ignore
-    "D401",
-    "D404", # default ignore
-    "D417", # ruff only rulecode
-    "PERF2",
-    "PERF4",
-]
-exclude = [
-    "build/**",
-    "docs/**",
-    "node_modules/**",
-]
-
-[tool.ruff.lint.pydocstyle]
-convention = "google"
-
-[tool.ruff.lint.per-file-ignores]
-"tests/*" = ["D"]
-
 # Ignore directories
 [tool.yapfignore]
 ignore_patterns = [
     "runs/**/*.py",
     "wandb/**/*.py",
     "build/**/*.py",
 ]
```

### Comparing `mosaicml-streaming-0.7.4/setup.py` & `mosaicml-streaming-0.7.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         break
     else:
         assert end != -1, 'there should be a balanced number of start and ends'
         long_description = long_description[:start] + long_description[end + len(end_tag):]
 
 classifiers = [
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
 ]
 
 install_requires = [
     'boto3>=1.21.45,<2',
     'Brotli>=1.0.9',
     'google-cloud-storage>=2.9.0,<2.11.0',
     'matplotlib>=3.5.2,<4',
@@ -64,38 +64,44 @@
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'pyarrow>14.0.0',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
-    'pytest==7.4.4',
+    'pytest==8.1.1',
     'pytest_codeblocks==0.17.0',
-    'pytest-cov>=4,<5',
+    'pytest-cov>=4,<6',
     'toml==0.10.2',
-    'yamllint==1.33.0',
-    'moto>=4.0,<5',
-    'fastapi==0.109.0',
-    'pydantic==2.5.3',
-    'uvicorn==0.26.0',
-    'pytest-split==0.8.1',
+    'yamllint==1.35.1',
+    'moto>=4.0,<6',
+    'fastapi==0.110.0',
+    'pydantic==2.6.4',
+    'uvicorn==0.29.0',
+    'pytest-split==0.8.2',
 ]
 
 extra_deps['docs'] = [
-    'GitPython==3.1.41',
-    'docutils==0.18.1',
-    'furo==2023.7.26',
-    'myst-parser==2.0.0',
-    'nbsphinx==0.9.2',
+    'GitPython==3.1.42',
+    'docutils==0.17.1',
+    'furo==2022.9.29',
+    'myst-parser==0.16.1',
+    'nbsphinx==0.9.1',
     'pandoc==2.3',
-    'pypandoc==1.12',
+    'pypandoc==1.13',
     'sphinx-argparse==0.4.0',
     'sphinx-copybutton==0.5.2',
-    'sphinx==6.2.1',
+    'sphinx==4.4.0',
     'sphinx-tabs==3.4.5',
+    'sphinxcontrib.katex==0.9.6',
+    'sphinxcontrib-applehelp==1.0.0',
+    'sphinxcontrib-devhelp==1.0.0',
+    'sphinxcontrib-htmlhelp==2.0.0',
+    'sphinxcontrib-qthelp==1.0.0',
+    'sphinxcontrib-serializinghtml==1.1.5',
 ]
 
 extra_deps['simulator'] = [
     'sortedcollections>=2.1.0,<3',
     'streamlit>=1.26.0,<2',
     'altair>=5.1.1,<6',
     'omegaconf>=2.3.0,<3',
@@ -106,15 +112,19 @@
 ]
 
 extra_deps['spark'] = [
     'pyspark>=3,<4',
 ]
 
 extra_deps['databricks'] = [
-    'databricks-sdk==0.14.0',
+    'databricks-sdk==0.23.0',
+]
+
+extra_deps['testing'] = [
+    'mosaicml-cli>=0.5.25,<0.7',
 ]
 
 extra_deps['all'] = sorted({dep for deps in extra_deps.values() for dep in deps})
 
 package_name = os.environ.get('MOSAIC_PACKAGE_NAME', 'mosaicml-streaming')
 
 if package_name != 'mosaicml-streaming':
@@ -137,9 +147,9 @@
     packages=setuptools.find_packages(exclude=['tests*']),
     entry_points={
         'console_scripts': ['simulator = simulation.launcher:launch_simulation_ui',],
     },
     classifiers=classifiers,
     install_requires=install_requires,
     extras_require=extra_deps,
-    python_requires='>=3.8',
+    python_requires='>=3.9',
 )
```

### Comparing `mosaicml-streaming-0.7.4/simulation/core/create_index.py` & `mosaicml-streaming-0.7.5/simulation/core/create_index.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/last_used_ordered_set.py` & `mosaicml-streaming-0.7.5/simulation/core/last_used_ordered_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/main.py` & `mosaicml-streaming-0.7.5/simulation/core/main.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/node_tracker.py` & `mosaicml-streaming-0.7.5/simulation/core/node_tracker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/shard_downloads.py` & `mosaicml-streaming-0.7.5/simulation/core/shard_downloads.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/shuffle_quality.py` & `mosaicml-streaming-0.7.5/simulation/core/shuffle_quality.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/sim_dataset.py` & `mosaicml-streaming-0.7.5/simulation/core/sim_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,17 @@
             nodes of the initial run if ``shuffle_algo`` is ``py1s`` or ``py2s``, and simply the
             number of physical nodes of the initial run otherwise. Defaults to ``None``.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1e``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int, optional): Unit of shuffle. A canonical node's samples are split
             into blocks of this size, and samples within each block are shuffled. If ``None``, its
             value is calculated as ``max(4_000_000 // num_canonical_nodes), 1 << 18)``. Defaults to
@@ -187,15 +188,15 @@
             self.predownload < self.batch_size:
             warnings.warn(f'predownload < batch_size ({self.predownload} < {self.batch_size}).' +
                           f'This may result in slower batch time. Recommendation is to set ' +
                           f'predownload to at-least batch_size.')
         elif self.predownload is None:
             self.predownload = 8 * self.batch_size if self.batch_size is not None else 64
 
-        self.batch_size = batch_size or 1
+        self.batch_size = batch_size
 
         # Convert epoch size from string to int, if needed. Cannot be negative.
         epoch_size_value = None
         if epoch_size:
             epoch_size_value = number_abbrev_to_int(epoch_size)
             if epoch_size_value < 0:
                 raise ValueError(f'Epoch size cannot be negative. Received {epoch_size_value}.')
```

### Comparing `mosaicml-streaming-0.7.4/simulation/core/sim_spanner.py` & `mosaicml-streaming-0.7.5/simulation/core/sim_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/sim_time.py` & `mosaicml-streaming-0.7.5/simulation/core/sim_time.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/sim_world.py` & `mosaicml-streaming-0.7.5/simulation/core/sim_world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/utils.py` & `mosaicml-streaming-0.7.5/simulation/core/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/core/yaml_processing.py` & `mosaicml-streaming-0.7.5/simulation/core/yaml_processing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/interfaces/interface_utils.py` & `mosaicml-streaming-0.7.5/simulation/interfaces/interface_utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/interfaces/sim_cli.py` & `mosaicml-streaming-0.7.5/simulation/interfaces/sim_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/interfaces/sim_script.py` & `mosaicml-streaming-0.7.5/simulation/interfaces/sim_script.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/interfaces/sim_ui.py` & `mosaicml-streaming-0.7.5/simulation/interfaces/sim_ui.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/simulation/interfaces/widgets.py` & `mosaicml-streaming-0.7.5/simulation/interfaces/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,27 @@
                            data, title='Cumulative Network Usage, all nodes').mark_line().encode(
                                x='step', y='cumulative network usage (bytes)'))
 
     # Draw points on the line, and highlight based on selection
     points = lines.transform_filter(hover).mark_circle(size=65)
 
     # Draw a rule at the location of the selection
-    tooltips = (alt.Chart(data).mark_rule().encode(
-        x='step',
-        y='throughput (batches/s)' if throughput else 'cumulative network usage (bytes)',
-        opacity=alt.condition(hover, alt.value(0.3), alt.value(0)),
-        tooltip=[
-            alt.Tooltip('step', title='Step'),
-            alt.Tooltip(
-                'throughput (batches/s)' if throughput else 'cumulative network usage (bytes)',
-                title='Throughput' if throughput else 'Network Usage'),
-        ],
-    ).add_params(hover))
-    return (lines + points + tooltips).interactive()
+    tooltips = (
+        alt.Chart(data).mark_rule().encode(
+            x='step',
+            y='throughput (batches/s)' if throughput else 'cumulative network usage (bytes)',
+            opacity=alt.condition(hover, alt.value(0.3), alt.value(0)),  # pyright: ignore
+            tooltip=[
+                alt.Tooltip('step', title='Step'),
+                alt.Tooltip(
+                    'throughput (batches/s)' if throughput else 'cumulative network usage (bytes)',
+                    title='Throughput' if throughput else 'Network Usage'),
+            ],
+        ).add_params(hover))
+    return (lines + points + tooltips).interactive()  # pyright: ignore
 
 
 def stream_entry(component: DeltaGenerator,
                  streams: dict,
                  key: int,
                  add_stream: bool = True,
                  defaults: Optional[dict] = None):
```

### Comparing `mosaicml-streaming-0.7.4/streaming/__init__.py` & `mosaicml-streaming-0.7.5/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/array.py` & `mosaicml-streaming-0.7.5/streaming/base/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/batching/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/batching/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/batching/per_stream.py` & `mosaicml-streaming-0.7.5/streaming/base/batching/per_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     # First, for each stream, sample each shard of the stream according to
     # stream proportions/repeats/samples. We obtain the resampled size of each shard
     # in the stream and a mapping from the training "big" sample ID to the underlying
     # shard "small" sample ID. Then, we also partition each stream's samples over
     # nodes/devices/workers. We handle sample_in_epoch (for resumption) at the end.
     partition_per_stream = []
 
-    batch_size = dataset.batch_size or 1
+    batch_size = dataset.batch_size
+    assert isinstance(batch_size, int), f'Batch size must be an integer. Got {type(batch_size)}.'
 
     for stream_id, stream in enumerate(dataset.streams):
         shuffle_units, small_per_big = dataset.resample_streams(epoch, stream_id)
         samples_in_stream = len(small_per_big)
         stream_partition = get_partitions(dataset.partition_algo, samples_in_stream,
                                           dataset.num_canonical_nodes, world.num_nodes,
                                           world.ranks_per_node, world.workers_per_rank, batch_size,
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/batching/random.py` & `mosaicml-streaming-0.7.5/streaming/base/batching/random.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,20 +44,23 @@
                            f'Provide a positive integer.')
 
     # Sample each shard of each stream according to their proportions/repeats/samples. This
     # gives us the resampled size of each underlying shard, and a mapping from each fake "big"
     # sample ID to its underlying "small" sample ID.
     shuffle_units, small_per_big = dataset.resample_streams(epoch)
 
+    batch_size = dataset.batch_size
+    assert isinstance(batch_size, int), f'Batch size must be an integer. Got {type(batch_size)}.'
+
     # Partition the global sample space (of resampled "big" sample IDs) into a tensor of shape
     # (num physical nodes, ranks per node, workers per rank, batches per worker, samples per
     # batch) such that we have an elastically deterministic sample order.
     big_ids = get_partitions(dataset.partition_algo, dataset.epoch_size,
                              dataset.num_canonical_nodes, world.num_nodes, world.ranks_per_node,
-                             world.workers_per_rank, dataset.batch_size, sample_in_epoch,
+                             world.workers_per_rank, batch_size, sample_in_epoch,
                              dataset.initial_physical_nodes)
 
     # If we need to shuffle, shuffle in a node-aware and *underlying* shard-aware way.
     if dataset.shuffle:
         if not isinstance(dataset.shuffle_block_size, int):
             raise TypeError(f'Dataset `shuffle_block_size` must be an integer. ' +
                             f'Got {type(dataset.shuffle_block_size)} instead.')
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/batching/stratified.py` & `mosaicml-streaming-0.7.5/streaming/base/batching/stratified.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
 
     # First, for each stream, sample each shard of the stream using proportions/repeats/samples.
     # We obtain the resampled size of each shard in the stream and a mapping from the
     # training "big" sample ID to the underlying shard "small" sample ID.
     # Then, we also partition each stream's samples over nodes/devices/workers.
     # We handle sample_in_epoch (for resumption) at the end.
 
-    batch_size = dataset.batch_size or 1
+    batch_size = dataset.batch_size
+    assert isinstance(batch_size, int), f'Batch size must be an integer. Got {type(batch_size)}.'
+
     global_batch_size = batch_size * world.ranks_per_node * world.num_nodes
     partition_per_stream = []
     batch_portion_per_stream = []
     stream_proportions = []
     for stream_id, stream in enumerate(dataset.streams):
         # find how many samples in each global batch are from each stream.
         batch_portion = int(stream.proportion * global_batch_size)
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/compression.py` & `mosaicml-streaming-0.7.5/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/constant.py` & `mosaicml-streaming-0.7.5/streaming/base/constant.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/converters/dataframe_to_mds.py` & `mosaicml-streaming-0.7.5/streaming/base/converters/dataframe_to_mds.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/dataloader.py` & `mosaicml-streaming-0.7.5/streaming/base/dataloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,16 +67,23 @@
         Args:
             samples_in_epoch (int): The number of samples processed so far in the current epoch.
 
         Returns:
             Optional[Dict[str, Any]]: The state, if a streaming dataset.
         """
         if isinstance(self.dataset, StreamingDataset):
-            world = World()
+            world = World.detect()
             num_samples = self.num_samples_yielded * world.num_ranks
+            if self.dataset.replication is not None:
+                # Check if we are using `replication`. If we are, then we need to adjust the
+                # `num_samples_yielded` to reflect the fact that sample ids are shared across
+                # `replication` consecutive devices. For example, if `replication` is 2, then the
+                # number of samples seen is half the number of samples yielded, since every pair
+                # of devices shares sample ids. So the index into the sample partition is halved.
+                num_samples = num_samples // self.dataset.replication
             return self.dataset.state_dict(num_samples, False)
         return None
 
     def load_state_dict(self, obj: Dict[str, Any]) -> None:
         """Load a dict containing training state (called from non-worker process).
 
         This is called on each copy of the dataset when resuming.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/dataset.py` & `mosaicml-streaming-0.7.5/streaming/base/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """A mid-epoch-resumable streaming/caching pytorch IterableDataset."""
 
 import json
 import logging
 import mmap
 import os
-import sys
 import warnings
 from concurrent.futures import ThreadPoolExecutor, wait
 from concurrent.futures._base import Future
 from enum import IntEnum
 from math import ceil
 from tempfile import gettempdir
 from threading import Event, Lock
@@ -107,22 +106,16 @@
         self._num_exited = 0
 
         # python will attempt to join all threads on shutdown.
         # Here, we register a call to self.non_blocking_exit to run
         # at shutdown to prevent a deadlock.
         # In python version >=3.9 this can be accomplished via
         # threading._register_atexit but not with the atexit module.
-        # In older python versions, the atexit module can be used, and
-        # threading._register_atexit does not exist.
-        if sys.version_info[1] <= 8:  # check if python version <=3.8
-            import atexit
-            atexit.register(self.non_blocking_exit)
-        else:
-            from threading import _register_atexit  # pyright: ignore
-            _register_atexit(self.non_blocking_exit)
+        from threading import _register_atexit  # pyright: ignore
+        _register_atexit(self.non_blocking_exit)
 
     def non_blocking_exit(self) -> None:
         """Signal threads to exit without blocking.
 
         This will be called at process exit.
         """
         with self._lock:
@@ -289,29 +282,33 @@
             nodes of the initial run if ``shuffle_algo`` is ``py1s`` or ``py2s``, and simply the
             number of physical nodes of the initial run otherwise. Defaults to ``None``.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1e``.
         shuffle_seed (int): Seed for deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int, optional): Unit of shuffle. A canonical node's samples are split
             into blocks of this size, and samples within each block are shuffled. If ``None``, its
             value is calculated as ``max(4_000_000 // num_canonical_nodes), 1 << 18)``. Defaults to
             ``None``.
         batching_method (str): Which batching method to use, either ``random``, ``stratified``, or
             ``per_stream``. Defaults to ``random``.
         allow_unsafe_types (bool): If a shard contains Pickle, which allows arbitrary code
             execution during deserialization, whether to keep going if ``True`` or raise an error
             if ``False``. Defaults to ``False``.
+        replication (int, optional): Determines how many consecutive devices will receive the same
+            samples. Useful for training with tensor or sequence parallelism, where multiple
+            devices need to see the same partition of the dataset. Defaults to ``None``.
     """
 
     def __init__(self,
                  *,
                  streams: Optional[Sequence[Stream]] = None,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
@@ -329,32 +326,53 @@
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
                  shuffle_algo: str = 'py1e',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: Optional[int] = None,
                  batching_method: str = 'random',
-                 allow_unsafe_types: bool = False) -> None:
+                 allow_unsafe_types: bool = False,
+                 replication: Optional[int] = None) -> None:
         # Global arguments (which do not live in Streams).
         self.predownload = predownload
         self.cache_limit = cache_limit
         self.sampling_method = sampling_method
         self.sampling_granularity = sampling_granularity
         self.partition_algo = partition_algo
         self.num_canonical_nodes = num_canonical_nodes
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.shuffle_algo = shuffle_algo
         self.shuffle_seed = shuffle_seed
         self.shuffle_block_size = shuffle_block_size
         self.batching_method = batching_method
         self.allow_unsafe_types = allow_unsafe_types
+        self.replication = replication
+
+        # Initialize the World context.
+        #   * This information is for the per-rank or per-worker process.
+        #   * DataLoader worker processes may get a different worker ID and worker count than rank.
+        #   * We save the rank Worlds here because we cannot instantiate a World inside our
+        #     destructor.
+        #   * `unique_` is who are for coordination purposes, where every process must be unique.
+        #   * `parallel_` is who we think we are for iterating purposes, where groups of process
+        #     must act the same if `replication` is specified.
+        #     This can enable tensor or sequence parallelism.
+        world = World.detect()
+        self._unique_rank_world = world
+        if replication is not None:
+            self._parallel_rank_world = world.replicate(replication)
+        else:
+            self._parallel_rank_world = world.copy()
+        self._unique_worker_world: World
+        self._parallel_worker_world: World
 
         # Initialize initial_physical_nodes to None. If we are resuming, then we will set it to the
-        # number of physical nodes of the initial run in the _resume function.
+        # number of physical nodes of the initial run in the _resume function, or the number of
+        # nodes specified in the `_parallel_rank_world` if using `replication`.
         self.initial_physical_nodes = None
 
         # Check streams vs remote/local.
         if bool(streams) == (bool(remote) or bool(local)):
             raise ValueError(
                 'You must provide either `streams` or `remote`/`local`, but not both.')
 
@@ -439,31 +457,24 @@
         # to the trouble of loading them.
         Stream.validate_weights(streams)
 
         # Set streams.
         self.streams = streams
         self.num_streams = len(streams)
 
-        # Initialize the World context.
-        #
-        # Beware: This information is for the per-rank process. DataLoader worker processes may see
-        # different values for these fields. We are saving the rank World here because we cannot
-        # instantiate a World inside the StreamingDataset destructor.
-        self._rank_world = world = World()
-
         # Download each stream's index, load their shards, and map streams <-> shards.
         self.num_samples = 0
         self.shards = []
         stream_per_shard = []
         self.shard_offset_per_stream = np.zeros(self.num_streams, np.int64)
         self.shards_per_stream = np.zeros(self.num_streams, np.int64)
         self.sample_offset_per_stream = np.zeros(self.num_streams, np.int64)
         self.samples_per_stream = np.zeros(self.num_streams, np.int64)
         for stream_id, stream in enumerate(self.streams):
-            stream_shards = stream.get_shards(world, self.allow_unsafe_types)
+            stream_shards = stream.get_shards(self._unique_rank_world, self.allow_unsafe_types)
             num_stream_samples = sum(map(len, stream_shards))
             if not num_stream_samples:
                 index_filename = os.path.join(stream.local, stream.split, get_index_basename())
                 raise RuntimeError(f'Stream contains no samples: {index_filename}.')
             stream_per_shard += [stream_id] * len(stream_shards)
             self.shard_offset_per_stream[stream_id] = len(self.shards)
             self.shards_per_stream[stream_id] = len(stream_shards)
@@ -501,23 +512,23 @@
 
         # Now that we know the number of underlying samples of each stream, derive each stream's
         # true proportion/repeat/choose, as well as the total epoch size.
         self.epoch_size = Stream.apply_weights(self.streams, self.samples_per_stream,
                                                epoch_size_value, self.shuffle_seed)
 
         # Length (__len__) is the resampled epoch size divided over the number of devices.
-        self.length = ceil(self.epoch_size / world.num_ranks)
+        self.length = ceil(self.epoch_size / self._parallel_rank_world.num_ranks)
 
         # Register/lookup our shared memory prefix and filelock root directory.
         streams_local = [os.path.abspath(os.path.join(x.local, x.split)) for x in streams]
         streams_remote = [
             os.path.join(x.remote, x.split) if x.remote is not None else None for x in streams
         ]
         self._shm_prefix_int, self._locals_shm = get_shm_prefix(streams_local, streams_remote,
-                                                                world)
+                                                                self._unique_rank_world)
         self._filelock_root = os.path.join(gettempdir(), 'streaming')
         os.makedirs(self._filelock_root, exist_ok=True)
 
         # Create the shared memory-backed barrier, without its lock, which is unpickleable.
         self._shared_barrier = SharedBarrier(
             os.path.join(self._filelock_root, _get_path(self._shm_prefix_int, BARRIER_FILELOCK)),
             _get_path(self._shm_prefix_int, BARRIER))
@@ -544,15 +555,15 @@
 
         # Time of last access per shard. This is used to decide which shard(s) to evict when we run
         # out of space.
         self._shard_access_times = SharedArray(self.num_shards, np.uint64,
                                                _get_path(self._shm_prefix_int, SHARD_ACCESS_TIMES))
 
         # Initialize shared memory objects.
-        if world.is_local_leader:
+        if self._unique_rank_world.is_local_leader:
             # Set initial epoch (before any resumption).
             self.next_epoch = 0
 
             # Get cache usage due to streams.
             self.cache_usage = 0
             for stream in self.streams:
                 self.cache_usage += stream.get_index_size()
@@ -724,37 +735,36 @@
         # Ensure that we are backwards compatible with old checkpoint dataset state, since the
         # 'initial_physical_nodes' key may not be present.
         self.initial_physical_nodes = obj.get('initial_physical_nodes', None)
         self._set_shuffle_block_size(world)
 
         return epoch, sample_in_epoch
 
-    def _resume_incr_epoch(self, world: World) -> Tuple[int, int]:
+    def _resume_incr_epoch(self) -> Tuple[int, int]:
         """Start or resume training, pre-incrementing the next epoch.
 
-        Args:
-            world (World): World state.
+        This is called on each worker.
 
         Returns:
             Tuple[int, int]: What epoch this is, and sample offset in that epoch.
         """
         # Lazily create the shared barrier's FileLock, which contains a threading Lock, which is
         # unpickleable.
         if not hasattr(self._shared_barrier, 'lock'):
             self._shared_barrier.lock = FileLock(self._shared_barrier.filelock_path)
 
         # Either resume from checkpoint, or start from scratch.
         presumed_epoch = self.next_epoch
-        epoch, sample_in_epoch = self._resume(world, presumed_epoch)
+        epoch, sample_in_epoch = self._resume(self._parallel_worker_world, presumed_epoch)
 
         # Wait for everyone to get the epoch above.
-        self._shared_barrier(world.workers_per_node)
+        self._shared_barrier(self._unique_worker_world.workers_per_node)
 
         # Set the new next epoch.
-        if world.is_local_leader:
+        if self._unique_worker_world.is_local_leader:
             self.next_epoch = epoch + 1
 
         return epoch, sample_in_epoch
 
     def state_dict(self, num_samples: int, from_beginning: bool) -> Dict[str, Any]:
         """Get a dict containing training state (called from non-worker process).
 
@@ -767,15 +777,15 @@
             num_samples (int): The number of samples processed so far in the current epoch.
             from_beginning (int): Whether we are counting samples from the start of this epoch, or
                 the start of just this potentially resumed training run this epoch.
 
         Returns:
             Dict[str, Any]: The state.
         """
-        world = World()
+        world = self._parallel_rank_world
         epoch = self.next_epoch - 1
         epoch, offset = self._resume(world, epoch)
         if from_beginning:
             sample_in_epoch = num_samples
         else:
             sample_in_epoch = offset + num_samples
 
@@ -961,45 +971,60 @@
         name = _get_path(self._shm_prefix_int, EPOCH_DATA)
         size = int(np.prod(shape)) * np.int64().nbytes
         data_shm = SharedMemory(name=name, create=False, size=size, auto_cleanup=False)
         sample_ids = np.ndarray(shape, buffer=data_shm.buf, dtype=np.int64)
 
         return sample_ids, shape_shm, data_shm
 
-    def _get_work(self, world: World, epoch: int, sample_in_epoch: int) -> NDArray[np.int64]:
+    def _get_work(self, epoch: int, sample_in_epoch: int) -> NDArray[np.int64]:
         """Get this worker's partition of this epoch's sample space.
 
         Args:
-            world (World): World state.
             epoch (int): Which epoch it is.
             sample_in_epoch (int): Where we are in the epoch.
 
         Returns:
             Optional[NDArray[np.int64]]: Our partition of the epoch.
         """
         # Lazily create the shared barrier's FileLock, which contains a threading Lock, which is
         # unpickleable.
         if not hasattr(self._shared_barrier, 'lock'):
             self._shared_barrier.lock = FileLock(self._shared_barrier.filelock_path)
 
+        u_world = self._unique_worker_world
+        p_world = self._parallel_worker_world
+
         # Do expensive work that may use a lot of cores/memory just once, in the local leader.
-        if world.is_local_leader:
-            epoch_sample_ids = generate_work(self.batching_method, self, world, epoch,
+        if u_world.is_local_leader:
+            if self.replication is not None and not u_world.worker_of_rank:
+                logger.warning(f'The `replication` arg has been set and training is resuming ' +
+                               f'from sample {sample_in_epoch}. Make sure you are accounting ' +
+                               f"for sample replication when using StreamingDataset's " +
+                               f'`state_dict` method for deterministic resumption. Otherwise, ' +
+                               f'you will resume training from the wrong sample.')
+            # Ensure that batch_size is passed in, and is an integer. This is necessary for
+            # deterministic resumption and optimal performance.
+            if not isinstance(self.batch_size, int):
+                raise ValueError(f'Please pass `batch_size` to StreamingDataset. It should be ' +
+                                 f'set the same as the DataLoader, and is the number of samples ' +
+                                 f'per batch, for each device. It is necessary for ' +
+                                 f'deterministic resumption and optimal performance.')
+            epoch_sample_ids = generate_work(self.batching_method, self, p_world, epoch,
                                              sample_in_epoch)
             shape_shm, data_shm = self._share_work(epoch_sample_ids)
-            self._shared_barrier(world.workers_per_node)
+            self._shared_barrier(u_world.workers_per_node)
         else:
-            self._shared_barrier(world.workers_per_node)
+            self._shared_barrier(u_world.workers_per_node)
             epoch_sample_ids, shape_shm, data_shm = self._attach_work()
 
         # Each worker gets their portion of the work.
-        worker_sample_ids = epoch_sample_ids[world.node, world.rank_of_node,
-                                             world.worker_of_rank].flatten()
+        worker_sample_ids = epoch_sample_ids[p_world.node, p_world.rank_of_node,
+                                             p_world.worker_of_rank].flatten()
 
-        self._shared_barrier(world.workers_per_node)
+        self._shared_barrier(u_world.workers_per_node)
 
         # Now clean up after ourselves.
         shape_shm.cleanup()
         data_shm.cleanup()
 
         return worker_sample_ids
 
@@ -1433,19 +1458,20 @@
         if not hasattr(self, '_event'):
             self._event = Event()
         elif self._event.is_set():
             raise RuntimeError('Background thread failed. Check other traceback.')
 
         # Discover where we left off, if there is a checkpoint, or start at the next epoch.
         # Also pre-increment the epoch counter.
-        world = World()
-        epoch, sample_in_epoch = self._resume_incr_epoch(world)
+        self._unique_worker_world = self._unique_rank_world.detect_workers()
+        self._parallel_worker_world = self._parallel_rank_world.detect_workers()
+        epoch, sample_in_epoch = self._resume_incr_epoch()
 
         # Get this worker's partition of samples to process.
-        sample_ids = self._get_work(world, epoch, sample_in_epoch)
+        sample_ids = self._get_work(epoch, sample_in_epoch)
         if not len(sample_ids):  # Resumed at end of epoch, out of samples.
             return
 
         # Iterate over the samples while downloading ahead.
         self._iterator = it = _Iterator(sample_ids)
         prepare_future = self._executor.submit(self._prepare_thread, it)
         prepare_future.add_done_callback(self.on_exception)
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/distributed.py` & `mosaicml-streaming-0.7.5/streaming/base/distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/base/reader.py` & `mosaicml-streaming-0.7.5/streaming/base/format/base/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.7.5/streaming/base/format/base/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """Serialize samples into streaming dataset shards and index."""
 
 import json
 import logging
 import os
 import shutil
-import sys
 from abc import ABC, abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures._base import Future
 from threading import Event
 from time import sleep
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
@@ -60,14 +59,17 @@
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
             retry (int): Number of times to retry uploading a file to a remote location.
                 Default to ``2``.
+            exist_ok (bool): If the local directory exists and is not empty, whether to overwrite
+                the content or raise an error. `False` raises an error. `True` deletes the
+                content and starts fresh. Defaults to `False`.
     """
 
     format: str = ''  # Name of the format (like "mds", "csv", "json", etc).
 
     def __init__(self,
                  *,
                  out: Union[str, Tuple[str, str]],
@@ -96,15 +98,16 @@
             size_limit_value = bytes_to_int(size_limit)
             if size_limit_value < 0:
                 raise ValueError(f'`size_limit` must be greater than zero, instead, ' +
                                  f'found as {size_limit_value}.')
 
         # Validate keyword arguments
         invalid_kwargs = [
-            arg for arg in kwargs.keys() if arg not in ('progress_bar', 'max_workers', 'retry')
+            arg for arg in kwargs.keys()
+            if arg not in ('progress_bar', 'max_workers', 'retry', 'exist_ok')
         ]
         if invalid_kwargs:
             raise ValueError(f'Invalid Writer argument(s): {invalid_kwargs} ')
 
         self.keep_local = keep_local
         self.compression = compression
         self.hashes = hashes
@@ -112,14 +115,21 @@
         self.extra_bytes_per_shard = extra_bytes_per_shard
         self.extra_bytes_per_sample = extra_bytes_per_sample
         self.new_samples: List[bytes]
         self.new_shard_size: int
 
         self.shards = []
 
+        # Remove local directory if requested prior to creating writer
+        local = out if isinstance(out, str) else out[0]
+        if os.path.exists(local) and kwargs.get('exist_ok', False):
+            logger.warning(
+                f'Directory {local} exists and is not empty; exist_ok is set to True so will remove contents.'
+            )
+            shutil.rmtree(local)
         self.cloud_writer = CloudUploader.get(out, keep_local, kwargs.get('progress_bar', False),
                                               kwargs.get('retry', 2))
         self.local = self.cloud_writer.local
         self.remote = self.cloud_writer.remote
         # `max_workers`: The maximum number of threads that can be executed in parallel.
         # One thread is responsible for uploading one shard file to a remote location.
         self.executor = ThreadPoolExecutor(max_workers=kwargs.get('max_workers', None))
@@ -292,18 +302,15 @@
         self.executor.shutdown(wait=True)
         if self.remote and not self.keep_local:
             shutil.rmtree(self.local, ignore_errors=True)
 
     def cancel_future_jobs(self) -> None:
         """Shutting down the executor and cancel all the pending jobs."""
         # Beginning python v3.9, ThreadPoolExecutor.shutdown() has a new parameter `cancel_futures`
-        if sys.version_info[1] <= 8:  # check if python version <=3.8
-            self.executor.shutdown(wait=False)
-        else:
-            self.executor.shutdown(wait=False, cancel_futures=True)
+        self.executor.shutdown(wait=False, cancel_futures=True)
         if self.remote and not self.keep_local:
             shutil.rmtree(self.local, ignore_errors=True)
 
     def exception_callback(self, future: Future) -> None:
         """Raise an exception to the caller if exception generated by one of an async thread.
 
         Also, set the thread event to let other threads knows about the exception in one of the
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.7.5/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.7.5/streaming/base/format/json/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.7.5/streaming/base/format/json/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
+            exist_ok (bool): If the local directory exists and is not empty, whether to overwrite
+                the content or raise an error. `False` raises an error. `True` deletes the
+                content and starts fresh. Defaults to `False`.
     """
 
     format = 'json'
 
     def __init__(self,
                  *,
                  columns: Dict[str, str],
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/mds/encodings.py` & `mosaicml-streaming-0.7.5/streaming/base/format/mds/encodings.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         if dtype_int is None:
             raise ValueError(f'Unsupported dtype: {obj.dtype.name}.')
         if self.dtype is None:
             part = bytes([dtype_int])
             parts.append(part)
         else:
             if obj.dtype != self.dtype:
-                raise ValueError('Wrong dtype: expected {self.dtype}, got {obj.dtype.name}.')
+                raise ValueError(f'Wrong dtype: expected {self.dtype}, got {obj.dtype.name}.')
 
         # Encode shape, if not given in header.
         if self.shape is None:
             ndim = len(obj.shape)
             if 64 <= ndim:
                 raise ValueError('Array has too many axes: maximum 63, got {ndim}.')
             shape_arr = np.array(obj.shape, np.int64)
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.7.5/streaming/base/format/mds/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.7.5/streaming/base/format/mds/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,17 @@
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
+            exist_ok (bool): If the local directory exists and is not empty, whether to overwrite
+                the content or raise an error. `False` raises an error. `True` deletes the
+                content and starts fresh. Defaults to `False`.
     """
 
     format = 'mds'
     extra_bytes_per_sample = 4
 
     def __init__(self,
                  *,
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.7.5/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.7.5/streaming/base/format/xsv/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.7.5/streaming/base/format/xsv/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
         **kwargs (Any): Additional settings for the Writer.
 
             progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
                 a remote location. Default to ``False``.
             max_workers (int): Maximum number of threads used to upload output dataset files in
                 parallel to a remote location. One thread is responsible for uploading one shard
                 file to a remote location. Default to ``min(32, (os.cpu_count() or 1) + 4)``.
+            exist_ok (bool): If the local directory exists and is not empty, whether to overwrite
+                the content or raise an error. `False` raises an error. `True` deletes the
+                content and starts fresh. Defaults to `False`.
     """
 
     format = 'xsv'
 
     def __init__(self,
                  *,
                  columns: Dict[str, str],
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/hashing.py` & `mosaicml-streaming-0.7.5/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/local.py` & `mosaicml-streaming-0.7.5/streaming/base/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/partition/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def get_partitions(algo: str,
                    num_samples: int,
                    num_canonical_nodes: int,
                    num_physical_nodes: int,
                    ranks_per_node: int,
                    workers_per_rank: int,
-                   batch_size: Optional[int] = None,
+                   batch_size: int,
                    drop_first: int = 0,
                    initial_physical_nodes: Optional[int] = None) -> NDArray[np.int64]:
     """Partition the given number of samples to nodes, ranks, and workers.
 
     Either canonical or physical nodes must be evenly divisible by the other.
 
     It is suggested to set num_canonical_nodes higher than your expected number of physical nodes,
@@ -37,16 +37,16 @@
     Args:
         algo (str): Partition algorithm name.
         num_samples (int): Dataset size.
         num_canonical_nodes (int): Number of canonical nodes.
         num_physical_nodes (int): Number of physical nodes.
         ranks_per_node (int): Number of ranks per node.
         workers_per_rank (int): Number of worker partitions per rank.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int): Batch size of DataLoader and dataset, which affects how the dataset is
+            partitioned over the workers.
         drop_first (int): Number of samples seen already, which are dropped. Defaults to ``0``.
         initial_physical_nodes (int, optional): Number of physical nodes at the start of training.
             Defaults to ``None``.
 
     Returns:
         NDArray[np.int64]: Partitions of shape (physical nodes, ranks per node, workers per rank,
             batches per worker, batch size).
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/partition/orig.py` & `mosaicml-streaming-0.7.5/streaming/base/partition/orig.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_partitions_orig(num_samples: int,
                         num_canonical_nodes: int,
                         num_physical_nodes: int,
                         ranks_per_node: int,
                         workers_per_rank: int,
-                        batch_size: Optional[int] = None,
+                        batch_size: int,
                         drop_first: int = 0,
                         initial_physical_nodes: Optional[int] = None) -> NDArray[np.int64]:
     """Partition the given number of samples to nodes, ranks, and workers.
 
     Either canonical or physical nodes must be evenly divisible by the other.
 
     It is suggested to set num_canonical_nodes higher than your expected number of physical nodes,
@@ -32,16 +32,16 @@
 
     Args:
         num_samples (int): Dataset size.
         num_canonical_nodes (int): Number of canonical nodes.
         num_physical_nodes (int): Number of physical nodes.
         ranks_per_node (int): Number of ranks per node.
         workers_per_rank (int): Number of worker partitions per rank.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int): Batch size of DataLoader and dataset, which affects how the dataset is
+            partitioned over the workers.
         drop_first (int): Number of samples seen already, which are dropped. Defaults to ``0``.
         initial_physical_nodes (int, optional): Number of physical nodes at the start of training.
             Defaults to ``None``.
 
     Returns:
         NDArray[np.int64]: Partitions of shape (physical nodes, ranks per node, workers per rank,
             batches per worker, batch size).
@@ -57,16 +57,14 @@
                              'lead to each node downloading all shards')
     elif num_physical_nodes < num_canonical_nodes:
         if num_canonical_nodes % num_physical_nodes:
             raise ValueError('Either canonical or physical nodes must be evenly divisible by ' +
                              'the other, otherwise striping slices of shards over nodes may ' +
                              'lead to each node downloading all shards')
 
-    batch_size = batch_size or 1
-
     # If drop_first isn't a multiple of num_physical_nodes, round down to make it divisible.
     if drop_first % num_physical_nodes:
         logger.warning(
             '`drop_first` was not divisible by `num_physical_nodes`. Rounding it down ' +
             'to make it divisible.')
         drop_first -= drop_first % num_physical_nodes
 
@@ -77,15 +75,20 @@
     if num_canonical_nodes < num_physical_nodes:
         node_ratio = num_physical_nodes // num_canonical_nodes
         overflow = samples_per_canonical_node % node_ratio
         if overflow:
             padding = node_ratio - overflow
     padded_samples_per_canonical_node = samples_per_canonical_node + padding
 
-    if num_samples > num_canonical_nodes:
+    # For samples to be properly split across canonical nodes, there must be more samples than nodes.
+    # The edge case is when the number of samples is equal to the number of canonical nodes, but this only works when
+    #  there is an equal or greater number of canonical nodes than physical nodes.
+    # If these conditions are not met, an alternative sampling approach is used that leads to many repeats.
+    if num_samples > num_canonical_nodes or (num_samples == num_canonical_nodes and
+                                             num_canonical_nodes >= num_physical_nodes):
         # Create the initial sample ID matrix.
         #
         # ids: (canonical nodes, padded samples per canonical node).
         ids = np.arange(num_canonical_nodes * padded_samples_per_canonical_node, dtype=np.int64)
         ids = ids.reshape(num_canonical_nodes, padded_samples_per_canonical_node)
 
         # Adjust row offsets to ignore the padding.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/partition/relaxed.py` & `mosaicml-streaming-0.7.5/streaming/base/partition/relaxed.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_partitions_relaxed(num_samples: int,
                            num_canonical_nodes: int,
                            num_physical_nodes: int,
                            ranks_per_node: int,
                            workers_per_rank: int,
-                           batch_size: Optional[int] = None,
+                           batch_size: int,
                            drop_first: int = 0,
                            initial_physical_nodes: Optional[int] = None) -> NDArray[np.int64]:
     """Partition the given number of samples to nodes, ranks, and workers.
 
     Either canonical or physical nodes must be evenly divisible by the other when partitioning over
     the initial number of physical nodes. For partitions during resumption, the only constraint
     is that the global batch size, which remains constant during training, must be evenly divisible
@@ -35,16 +35,16 @@
 
     Args:
         num_samples (int): Dataset size.
         num_canonical_nodes (int): Number of canonical nodes.
         num_physical_nodes (int): Number of physical nodes.
         ranks_per_node (int): Number of ranks per node.
         workers_per_rank (int): Number of worker partitions per rank.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int): Batch size of DataLoader and dataset, which affects how the dataset is
+            partitioned over the workers.
         drop_first (int): Number of samples seen already, which are dropped. Defaults to ``0``.
         initial_physical_nodes (int, optional): Number of physical nodes at the start of training.
             Defaults to ``None``.
 
     Returns:
         NDArray[np.int64]: Partitions of shape (physical nodes, ranks per node, workers per rank,
             batches per worker, batch size).
@@ -61,15 +61,14 @@
         # which also requires that NCN be divisible by PN or vice versa.
         # Case 2: PN <= NCN and PN evenly divides NCN. The original partition algo can be used,
         # and will give better downloads per node as well.
         # Case 3: PN > NCN and NCN evenly divides PN. The original partition algo can be used.
         return get_partitions_orig(num_samples, num_canonical_nodes, num_physical_nodes,
                                    ranks_per_node, workers_per_rank, batch_size, drop_first)
     else:
-        batch_size = batch_size or 1
         # First, make a partition over the initial number of physical nodes and device batch size.
         # We assume that ranks_per_node and workers_per_rank stay constant during resumptions.
         global_batch_size = num_physical_nodes * ranks_per_node * batch_size
         initial_total_devices = initial_physical_nodes * ranks_per_node
         # Check for divisibility of the current global batch size and the initial total devices.
         # This should be true since the global batch size should not change in the middle of
         # training.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/sampling.py` & `mosaicml-streaming-0.7.5/streaming/base/sampling.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/array.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/array.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         name (str): Its name in shared memory.
     """
 
     def __init__(self, shape: Union[int, Tuple[int]], dtype: type, name: str) -> None:
         self.shape = np.empty(shape).shape
         self.dtype = dtype
         self.name = name
-        size = np.prod(shape) * dtype(0).nbytes
+        size = int(np.prod(shape) * dtype(0).nbytes)
         self.shm = SharedMemory(name=name, size=size)
 
     def numpy(self) -> NDArray:
         """Get as a numpy array.
 
         We can't just internally store and use this numpy array shared memory wrapper because it's
         not compatible with spawn.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/barrier.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/memory.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/memory.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/prefix.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/prefix.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shared/scalar.py` & `mosaicml-streaming-0.7.5/streaming/base/shared/scalar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/naive.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/naive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/py1b.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1b.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/py1br.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1br.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/py1e.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1e.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.7.5/streaming/base/shuffle/py2s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/spanner.py` & `mosaicml-streaming-0.7.5/streaming/base/spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/storage/__init__.py` & `mosaicml-streaming-0.7.5/streaming/base/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/storage/download.py` & `mosaicml-streaming-0.7.5/streaming/base/storage/download.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/storage/upload.py` & `mosaicml-streaming-0.7.5/streaming/base/storage/upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/stream.py` & `mosaicml-streaming-0.7.5/streaming/base/stream.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/base/util.py` & `mosaicml-streaming-0.7.5/streaming/base/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/crawl_webvid.py` & `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py` & `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
     # Create a Stream per sub-dataset, then pass them to a StreamingDataset.
     streams = []
     for name in sorted(subsets_present):
         dirname = os.path.join(args.mds_root, name)
         stream = Stream(local=dirname, proportion=1 / len(subsets_present))
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, epoch_size=50)
+    dataset = StreamingDataset(streams=streams, epoch_size=50, batch_size=1)
 
     # Print the size of each sub-dataset.
     for name, num_samples in zip(sorted(subsets_present), dataset.samples_per_stream):
         print(f'Subset "{name}": {num_samples} samples')
 
     # Iterate the combined dataset 3 times.
     for epoch in range(3):
```

### Comparing `mosaicml-streaming-0.7.4/streaming/multimodal/convert/webvid/extract_webvid_videos.py` & `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 def main(args: Namespace) -> None:
     """Convert an MP4-inside MDS dataset to an MP4-outside MDS dataset.
 
     Args:
         args (Namespace): Command-line arguments.
     """
     hashes = args.hashes.split(',') if args.hashes else []
-    dataset = StreamingDataset(local=getattr(args, 'in'))
+    dataset = StreamingDataset(local=getattr(args, 'in'), batch_size=1)
     with MDSWriter(out=args.out_mds,
                    columns=out_columns,
                    compression=args.compression,
                    hashes=hashes,
                    size_limit=args.size_limit) as out:
         for i, sample in tqdm(enumerate(dataset), total=dataset.num_samples):
             content_path = f'{i // 1000:03}/{i % 1000:03}.mp4'
```

### Comparing `mosaicml-streaming-0.7.4/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.7.5/streaming/multimodal/webvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
@@ -130,16 +131,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         extra_local (str, optional): Base destination of extra local sample downloads.
         extra_remote (str, optional): Base source of extra remote sample downloads.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/text/c4.py` & `mosaicml-streaming-0.7.5/streaming/text/c4.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,16 +59,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/c4.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/convert/pile.py` & `mosaicml-streaming-0.7.5/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/text/enwiki.py` & `mosaicml-streaming-0.7.5/streaming/text/enwiki.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
```

### Comparing `mosaicml-streaming-0.7.4/streaming/text/pile.py` & `mosaicml-streaming-0.7.5/streaming/text/pile.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/ade20k.py` & `mosaicml-streaming-0.7.5/streaming/vision/ade20k.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         joint_transform (callable, optional): A function/transforms that takes in an image and a
             target  and returns the transformed versions of both. Defaults to ``None``.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/base.py` & `mosaicml-streaming-0.7.5/streaming/vision/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                  validate_hash: Optional[str] = None,
                  keep_zip: bool = False,
                  epoch_size: Optional[int] = None,
                  predownload: Optional[int] = None,
                  cache_limit: Optional[int] = None,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
-                 batch_size: Optional[int] = None,
+                 batch_size: int,
                  shuffle: bool = False,
                  shuffle_algo: str = 'py1s',
                  shuffle_seed: int = 9176,
                  shuffle_block_size: int = 1 << 18,
                  transforms: Optional[Callable] = None,
                  transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None) -> None:
```

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/cifar10.py` & `mosaicml-streaming-0.7.5/streaming/vision/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/coco.py` & `mosaicml-streaming-0.7.5/streaming/vision/coco.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,17 @@
             source diversity). Defaults to ``None``, which is interpreted as 64 times the number
             of nodes of the initial run.
 
             .. note::
 
                 For sequential sample ordering, set ``shuffle`` to ``False`` and
                 ``num_canonical_nodes`` to the number of physical nodes of the initial run.
-        batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
-            partitioned over the workers. Defaults to ``None``.
+        batch_size (int, optional): Per-device batch size, the same as what is passed to the
+            DataLoader. This affects how the dataset is partitioned over the workers and is
+            necessary for deterministic resumption and optimal performance. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transform (callable, optional): A function/transform that takes in an image and bboxes and
             returns a transformed version. Defaults to ``None``.
```

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/base.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/coco.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,16 +177,16 @@
         img_bytes = open(img_filename, 'rb').read()
 
         yield {
             'img': img_bytes,
             'img_id': img_id,
             'htot': htot,
             'wtot': wtot,
-            'bbox_sizes': bbox_sizes,  # (_, 4) float32.
-            'bbox_labels': bbox_labels,  # int64.
+            'bbox_sizes': np.array(bbox_sizes, dtype=np.float32),  # (_,4) np.float32 array.
+            'bbox_labels': np.array(bbox_labels, dtype=np.int64),  # np.int64 array.
         }
 
 
 def main(args: Namespace) -> None:
     """Main: create COCO streaming dataset.
 
     Args:
@@ -198,16 +198,16 @@
         ValueError: Number of samples in a dataset does not match.
     """
     columns = {
         'img': 'jpeg',
         'img_id': 'int',
         'htot': 'int',
         'wtot': 'int',
-        'bbox_sizes': 'pkl',
-        'bbox_labels': 'pkl'
+        'bbox_sizes': 'ndarray:float32',
+        'bbox_labels': 'ndarray:int64',
     }
 
     for (split, expected_num_samples, shuffle) in [
         ('train', 117266, True),
         ('val', 4952, False),
     ]:
         out_split_dir = os.path.join(args.out_root, split)
```

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.7.5/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/streaming/vision/imagenet.py` & `mosaicml-streaming-0.7.5/streaming/vision/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_array.py` & `mosaicml-streaming-0.7.5/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_barrier.py` & `mosaicml-streaming-0.7.5/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_compression.py` & `mosaicml-streaming-0.7.5/tests/test_compression.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,14 +270,14 @@
     samples = SequenceDataset(num_samples)
     write_mds_dataset(out_root=remote,
                       columns=columns,
                       samples=samples,
                       size_limit=size_limit,
                       compression=None)
 
-    dataset = StreamingDataset(local=local, remote=compressed, shuffle=shuffle)
+    dataset = StreamingDataset(local=local, remote=compressed, shuffle=shuffle, batch_size=1)
 
     for _ in dataset:
         pass  # download sample
 
     dcmp = dircmp(remote, local)
     check_for_diff_files(dcmp, compression_ext)
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_distributed.py` & `mosaicml-streaming-0.7.5/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_download.py` & `mosaicml-streaming-0.7.5/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_encodings.py` & `mosaicml-streaming-0.7.5/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_eviction.py` & `mosaicml-streaming-0.7.5/tests/test_eviction.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             assert ops(set(os.listdir(local)), set(os.listdir(remote)))
 
 
 def shard_eviction_disabled(remote: str, local: str, keep_zip: bool):
     """
     With shard eviction disabled.
     """
-    dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip)
+    dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip, batch_size=1)
     for _ in range(2):
         for sample in dataset:  # pyright: ignore
             pass
 
     validate(remote, local, dataset, keep_zip, False)
     rmtree(local, ignore_errors=False)
 
@@ -56,15 +56,16 @@
 def shard_eviction_too_high(remote: str, local: str, keep_zip: bool):
     """
     With no shard evictions because cache_limit is bigger than the dataset.
     """
     dataset = StreamingDataset(remote=remote,
                                local=local,
                                keep_zip=keep_zip,
-                               cache_limit=1_000_000)
+                               cache_limit=1_000_000,
+                               batch_size=1)
     dataloader = DataLoader(dataset=dataset, num_workers=8)
     for _ in range(2):
         for _ in dataloader:
             pass
     validate(remote, local, dataset, keep_zip, False)
     rmtree(local, ignore_errors=False)
 
@@ -73,28 +74,29 @@
     """
     With shard eviction because cache_limit is smaller than the whole dataset.
     """
     cache_limit = '120kb' if keep_zip else '100kb'
     dataset = StreamingDataset(remote=remote,
                                local=local,
                                keep_zip=keep_zip,
-                               cache_limit=cache_limit)
+                               cache_limit=cache_limit,
+                               batch_size=1)
     dataloader = DataLoader(dataset=dataset, num_workers=8)
     for _ in range(2):
         for _ in dataloader:
             pass
     validate(remote, local, dataset, keep_zip, True)
     rmtree(local, ignore_errors=False)
 
 
 def manual_shard_eviction(remote: str, local: str, keep_zip: bool):
     """
     Manually downloading and evicting shards.
     """
-    dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip)
+    dataset = StreamingDataset(remote=remote, local=local, keep_zip=keep_zip, batch_size=1)
 
     for shard_id in range(dataset.num_shards):
         dataset.prepare_shard(shard_id)
 
     full = set(os.listdir(local))
 
     for shard_id in range(dataset.num_shards):
@@ -110,15 +112,15 @@
 
 
 def cache_limit_too_low(remote: str, local: str, keep_zip: bool):
     """
     With impossible shard eviction settings because cache_limit is set too low.
     """
     with pytest.raises(ValueError):
-        dataset = StreamingDataset(remote=remote, local=local, cache_limit='1kb')
+        dataset = StreamingDataset(remote=remote, local=local, cache_limit='1kb', batch_size=1)
         for _ in dataset:
             pass
     rmtree(local, ignore_errors=False)
 
 
 funcs = [
     shard_eviction_disabled, shard_eviction_too_high, shard_eviction, manual_shard_eviction,
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_hashing.py` & `mosaicml-streaming-0.7.5/tests/test_hashing.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
                    num_samples=num_samples,
                    compression=compression,
                    hashes=hashes,
                    size_limit=1 << 8)
 
     # Build StreamingDataset
     hash = hashes[0] if hashes is not None else None
-    dataset = StreamingDataset(local=local_dir, remote=remote_dir, validate_hash=hash)
+    dataset = StreamingDataset(local=local_dir,
+                               remote=remote_dir,
+                               validate_hash=hash,
+                               batch_size=1)
 
     # Append sample ID
     sample_order = []
     for sample in dataset:
         sample_order.append(sample['id'])
 
     # Test length
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_laziness.py` & `mosaicml-streaming-0.7.5/tests/test_laziness.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 from streaming import MDSWriter, StreamingDataset
 
 
 def one(remote: str, local: str):
     """
     Verify __getitem__ accesses.
     """
-    dataset = StreamingDataset(local=remote)
+    dataset = StreamingDataset(local=remote, batch_size=1)
     for i in range(dataset.num_samples):
         sample = dataset[i]
         assert sample['value'] == i
 
 
 def two(remote: str, local: str):
     """
     Verify __iter__ -> __getitem__ accesses.
     """
-    dataset = StreamingDataset(local=remote, num_canonical_nodes=1)
+    dataset = StreamingDataset(local=remote, num_canonical_nodes=1, batch_size=1)
     for i, sample in zip(range(dataset.num_samples), dataset):
         assert sample['value'] == i
 
 
 def three(remote: str, local: str):
     """
     Verify __getitem__ downloads/accesses.
     """
-    dataset = StreamingDataset(local=local, remote=remote)
+    dataset = StreamingDataset(local=local, remote=remote, batch_size=1)
     for i in range(dataset.num_samples):
         sample = dataset[i]
         assert sample['value'] == i
 
 
 def four(remote: str, local: str):
     """
     Verify __iter__ -> __getitem__ downloads/accesses.
     """
-    dataset = StreamingDataset(local=local, remote=remote, num_canonical_nodes=1)
+    dataset = StreamingDataset(local=local, remote=remote, num_canonical_nodes=1, batch_size=1)
     for i, sample in zip(range(dataset.num_samples), dataset):
         assert sample['value'] == i
     del dataset
 
 
 def five(remote: str, local: str):
     """
     Re-verify __getitem__ downloads/accesses.
     """
-    dataset = StreamingDataset(local=local, remote=remote)
+    dataset = StreamingDataset(local=local, remote=remote, batch_size=1)
     for i in range(dataset.num_samples):
         sample = dataset[i]
         assert sample['value'] == i
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 @pytest.mark.parametrize('func', [one, two, three, four, five])
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_local.py` & `mosaicml-streaming-0.7.5/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_mixing.py` & `mosaicml-streaming-0.7.5/tests/test_mixing.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,45 +36,45 @@
 
 def test_mix_none(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == list(range(8))
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
         assert stream.choose == 2
 
 
 def test_mix_choose_same(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, choose=2)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == list(range(8))
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
         assert stream.choose == 2
 
 
 def test_mix_choose_mul(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, choose=4)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [0, 1, 0, 1, 2, 3, 2, 3, 4, 5, 4, 5, 6, 7, 6, 7]
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 2
         assert stream.choose == 4
 
@@ -82,15 +82,15 @@
 def test_mix_choose_range(root: str):
     choices = [0, 2, 4, 6]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, choose=choices[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.choose == i * 2
 
@@ -98,15 +98,15 @@
 def test_mix_repeat(root: str):
     repeat = [0, 1, 2, 3]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, repeat=repeat[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.choose == i * 2
 
@@ -120,15 +120,15 @@
     ]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         repeat, choose = weights[i]
         stream = Stream(local=subroot, repeat=repeat, choose=choose)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.choose == i * 2
 
@@ -142,15 +142,15 @@
     ]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         repeat, choose = weights[i]
         stream = Stream(local=subroot, repeat=repeat, choose=choose)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.choose == i * 2
 
@@ -158,15 +158,15 @@
 def test_mix_proportion_equal(root: str):
     proportion = [1, 1, 1, 1]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, proportion=proportion[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [0, 1, 2, 3, 4, 5, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 1
         assert stream.choose == 2
 
@@ -174,30 +174,30 @@
 def test_mix_proportion_range(root: str):
     proportion = [0, 1 / 6, 2 / 6, 3 / 6]
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, proportion=proportion[i])
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, epoch_size=12, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, epoch_size=12, num_canonical_nodes=1, batch_size=1)
     assert dataset.num_samples == 8
     assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.choose == i * 2
 
 
 def test_mix_balance(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, choose=3)
         streams.append(stream)
-    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1)
+    dataset = StreamingDataset(streams=streams, num_canonical_nodes=1, batch_size=1)
     counts = np.zeros(8, np.int64)
     for _ in range(1000):
         for value in walk(dataset):
             counts[value] += 1
     rates = counts / counts.sum() * len(counts)
     for rate in rates:
         assert 0.975 < rate < 1.025
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_partition.py` & `mosaicml-streaming-0.7.5/tests/test_partition.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import warnings
 
 import numpy as np
 import pytest
 
 from streaming.base.partition import get_partitions
+from streaming.base.world import World
 
 
 @pytest.mark.parametrize('partition_algo', ['orig', 'relaxed'])
 def test_partition_walk(partition_algo: str):
     num_samples = 1000
     num_canonical_nodes = 176
     num_physical_nodes = 22
@@ -218,7 +219,86 @@
     for global_batch in partition:
         for sample in global_batch:
             samples_seen.append(sample)
             samples_seen_set.add(sample)
 
     assert len(samples_seen) == num_samples
     assert samples_seen_set == set(range(num_samples))
+
+
+@pytest.mark.parametrize('physical_nodes', [1, 4])
+@pytest.mark.parametrize('canonical_nodes', [12, 4, 64])
+@pytest.mark.parametrize('ranks_per_node', [8])
+@pytest.mark.parametrize('workers_per_rank', [1, 8])
+@pytest.mark.parametrize('batch_size', [2, 8])
+@pytest.mark.parametrize('num_samples', [1024, 16384])
+@pytest.mark.parametrize('sample_in_epoch', [0, 256])
+@pytest.mark.parametrize('replication', [2, 4])
+def test_replication_samples(physical_nodes: int, canonical_nodes: int, ranks_per_node: int,
+                             workers_per_rank: int, batch_size: int, num_samples: int,
+                             sample_in_epoch: int, replication: int):
+
+    # Create a World object reflecting the hardware -- the actual nodes and rank
+    actual_world = World(physical_nodes, ranks_per_node, workers_per_rank, 0)
+
+    # Create the World object with the given replication factor
+    replication_world = actual_world.replicate(replication)
+
+    # Get the sample partition using attributes from the replication World object
+    sample_ids = get_partitions('relaxed', num_samples, canonical_nodes,
+                                replication_world.num_nodes, replication_world.ranks_per_node,
+                                replication_world.workers_per_rank, batch_size, sample_in_epoch,
+                                replication_world.num_nodes)
+
+    # Loop over all of the actual nodes/workers/ranks and check that the samples are replicated
+    # according to the `replication` factor.
+    # Use World objects to correctly index into the sample_ids partition.
+    # This is what happens during actual training.
+    for n in range(physical_nodes):
+        for w in range(workers_per_rank):
+            for r in range(0, ranks_per_node, replication):
+                # Get the actual and replication World objects for this node/rank/worker.
+                # This ensures we have the right rank and worker indices in the World objects.
+                baseline_worker_id = (n * ranks_per_node + r) * workers_per_rank + w
+                baseline_actual_world = World(physical_nodes, ranks_per_node, workers_per_rank,
+                                              baseline_worker_id)
+                baseline_replication_world = baseline_actual_world.replicate(replication)
+                # Check that the sample ids are all the same for this replication group
+                baseline_sample_ids = sample_ids[baseline_replication_world.node,
+                                                 baseline_replication_world.rank_of_node,
+                                                 baseline_replication_world.worker_of_rank]
+                # Loop over the replication group and make sure the sample ids are all the same.
+                for i in range(1, replication):
+                    repeated_worker_id = (n * ranks_per_node + r + i) * workers_per_rank + w
+                    repeated_actual_world = World(physical_nodes, ranks_per_node, workers_per_rank,
+                                                  repeated_worker_id)
+                    repeated_replication_world = repeated_actual_world.replicate(replication)
+                    repeated_sample_ids = sample_ids[repeated_replication_world.node,
+                                                     repeated_replication_world.rank_of_node,
+                                                     repeated_replication_world.worker_of_rank]
+                    assert np.array_equal(baseline_sample_ids, repeated_sample_ids)
+
+
+@pytest.mark.parametrize('num_nodes', [4])
+@pytest.mark.parametrize('ranks_per_node', [8])
+@pytest.mark.parametrize('workers_per_rank', [2])
+@pytest.mark.parametrize('replication', [-10, 0])
+def test_replication_negative(num_nodes: int, ranks_per_node: int, workers_per_rank: int,
+                              replication: int):
+
+    orig_world = World(num_nodes, ranks_per_node, workers_per_rank, 0)
+
+    with pytest.raises(ValueError, match=f'Replication factor must be positive.*'):
+        orig_world.replicate(replication)
+
+
+@pytest.mark.parametrize('num_nodes', [4, 8])
+@pytest.mark.parametrize('ranks_per_node', [8])
+@pytest.mark.parametrize('workers_per_rank', [2])
+@pytest.mark.parametrize('replication', [7, 11])
+def test_replication_divides_world_size(num_nodes: int, ranks_per_node: int, workers_per_rank: int,
+                                        replication: int):
+
+    orig_world = World(num_nodes, ranks_per_node, workers_per_rank, 0)
+
+    with pytest.raises(ValueError, match=f'World size must be divisible by*'):
+        orig_world.replicate(replication)
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_reader.py` & `mosaicml-streaming-0.7.5/tests/test_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from streaming.base import StreamingDataset
 from tests.common.utils import convert_to_mds, copy_all_files
 
 logger = logging.getLogger(__name__)
 
 
-@pytest.mark.parametrize('batch_size', [None, 1, 2])
+@pytest.mark.parametrize('batch_size', [1, 2])
 @pytest.mark.parametrize('remote_arg', ['empty', 'same', 'different', 'local'])
 @pytest.mark.parametrize('shuffle', [False, True])
 @pytest.mark.parametrize('seed', [5151])
 @pytest.mark.parametrize('num_canonical_nodes', [1])
 @pytest.mark.parametrize('compression', [None, 'zstd:7'])
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dataset_sample_order(local_remote_dir: Any, batch_size: int, remote_arg: str,
@@ -79,15 +79,15 @@
     assert rcvd_samples == num_samples, \
         f'Only received {rcvd_samples} samples, expected {num_samples}'
     assert len(
         dataset
     ) == num_samples, f'Got dataset length={len(dataset)} samples, expected {num_samples}'
 
 
-@pytest.mark.parametrize('batch_size', [None, 1, 2])
+@pytest.mark.parametrize('batch_size', [1, 2])
 @pytest.mark.parametrize('seed', [8988])
 @pytest.mark.parametrize('shuffle', [False, True])
 @pytest.mark.parametrize('compression', [None, 'gz:3'])
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dataset_determinism(local_remote_dir: Any, batch_size: int, seed: int, shuffle: bool,
                              compression: str):
     remote_dir, local_dir = local_remote_dir
@@ -145,15 +145,16 @@
 
     # Build and iterate over a StreamingDataset
     with pytest.raises(FileNotFoundError) as exc_info:
         dataset = StreamingDataset(local=local_dir,
                                    remote=remote_dir,
                                    shuffle=False,
                                    download_timeout=1,
-                                   shuffle_seed=seed)
+                                   shuffle_seed=seed,
+                                   batch_size=1)
         for _ in dataset:
             pass
     assert exc_info.match(r'.*No such file or directory*')
 
 
 @pytest.mark.parametrize('created_ago', [0.5, 1.0])
 @pytest.mark.parametrize('download_timeout', [1])
@@ -176,15 +177,16 @@
                 os.path.join(local_dir, f'shard.00003.mds.tmp'))
     time.sleep(created_ago)
 
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=False,
                                download_timeout=download_timeout,
-                               shuffle_seed=seed)
+                               shuffle_seed=seed,
+                               batch_size=1)
 
     # Iterate over dataset and make sure there are no TimeoutErrors
     for _ in dataset:
         pass
 
 
 def _validate_sample(index: Union[int, slice, List[int], NDArray[np.int64]],
@@ -241,15 +243,16 @@
     if share_remote_local:
         local_dir = remote_dir
 
     # Build a StreamingDataset
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=False,
-                               shuffle_seed=seed)
+                               shuffle_seed=seed,
+                               batch_size=1)
 
     # Test retrieving random sample
     sample = dataset[index]
     _validate_sample(index, sample, len(dataset))
 
 
 @pytest.mark.usefixtures('local_remote_dir')
@@ -262,15 +265,15 @@
                    num_samples=117,
                    size_limit=1 << 8)
 
     # Build StreamingDataset for each split
     for split in splits:
         remote_split_dir = os.path.join(remote_dir, split)
         copy_all_files(remote_dir, remote_split_dir)
-        _ = StreamingDataset(local=local_dir, remote=remote_dir, split=split)
+        _ = StreamingDataset(local=local_dir, remote=remote_dir, split=split, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_invalid_index_json_exception(local_remote_dir: Tuple[str, str]):
     local_dir, remote_dir = local_remote_dir
     convert_to_mds(out_root=remote_dir,
                    dataset_name='sequencedataset',
@@ -282,15 +285,15 @@
 
     # Creates an empty file
     with open(os.path.join(local_dir, filename), 'w') as _:
         pass
 
     with pytest.raises(json.decoder.JSONDecodeError,
                        match=f'Index file at.*is empty or corrupted'):
-        _ = StreamingDataset(local=local_dir)
+        _ = StreamingDataset(local=local_dir, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_empty_shards_index_json_exception(local_remote_dir: Tuple[str, str]):
     local_dir, remote_dir = local_remote_dir
     convert_to_mds(out_root=remote_dir,
                    dataset_name='sequencedataset',
@@ -303,27 +306,27 @@
         os.mkdir(local_dir)
 
     # Creates a `index.json` file and write the content to it
     with open(os.path.join(local_dir, filename), 'w') as outfile:
         json.dump(content, outfile)
 
     with pytest.raises(RuntimeError, match=f'Stream contains no samples: .*'):
-        _ = StreamingDataset(local=local_dir)
+        _ = StreamingDataset(local=local_dir, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_accidental_shard_delete(local_remote_dir: Any):
     remote_dir, local_dir = local_remote_dir
     convert_to_mds(out_root=remote_dir,
                    dataset_name='sequencedataset',
                    num_samples=117,
                    size_limit=1 << 8)
     basename = 'shard.00000.mds'
     filename = os.path.join(local_dir, basename)
-    dataset = StreamingDataset(local=local_dir, remote=remote_dir)
+    dataset = StreamingDataset(local=local_dir, remote=remote_dir, batch_size=1)
     is_removed = False
     for _ in dataset:
         if os.path.exists(filename) and not is_removed:
             os.remove(filename)
             is_removed = True
     assert os.path.exists(filename), f'{basename} is missing'
     shutil.rmtree(local_dir, ignore_errors=True)
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_sampling.py` & `mosaicml-streaming-0.7.5/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_shared.py` & `mosaicml-streaming-0.7.5/tests/test_shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 # Copyright 2022-2024 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
-from typing import Tuple
+from typing import Tuple, Type
+from unittest.mock import patch
 
+import numpy as np
 import pytest
 
 from streaming.base import StreamingDataset
-from streaming.base.shared import get_shm_prefix
+from streaming.base.shared import SharedArray, get_shm_prefix
 from streaming.base.world import World
 from tests.common.utils import convert_to_mds
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_get_shm_prefix(local_remote_dir: Tuple[str, str]):
     local, remote = local_remote_dir
 
-    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[remote], world=World())
+    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[remote], world=World.detect())
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_get_shm_prefix_same_local_dir(local_remote_dir: Tuple[str, str]):
     local, remote = local_remote_dir
     with pytest.raises(ValueError, match='Reused local directory.*Provide a different one.'):
         _, _ = get_shm_prefix(streams_local=[local, local],
                               streams_remote=[remote, remote],
-                              world=World())
+                              world=World.detect())
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_get_shm_prefix_same_split_dir(local_remote_dir: Tuple[str, str]):
     local, remote = local_remote_dir
     _, _ = get_shm_prefix(streams_local=[local, remote],
                           streams_remote=[local, remote],
-                          world=World())
+                          world=World.detect())
     with pytest.raises(ValueError, match='Reused local directory.*vs.*Provide a different one.'):
         _, _ = get_shm_prefix(streams_local=[local, remote],
                               streams_remote=[local, remote],
-                              world=World())
+                              world=World.detect())
 
 
 def test_same_local_remote_none(local_remote_dir: Tuple[str, str]):
     local, _ = local_remote_dir
-    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[None], world=World())
-    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[None], world=World())
+    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[None], world=World.detect())
+    _, _ = get_shm_prefix(streams_local=[local], streams_remote=[None], world=World.detect())
 
 
 @pytest.mark.parametrize('from_beginning', [True, False])
 @pytest.mark.usefixtures('local_remote_dir')
 def test_load_get_state_dict_once(local_remote_dir: Tuple[str, str], from_beginning: bool):
     local, remote = local_remote_dir
     convert_to_mds(out_root=remote,
                    dataset_name='sequencedataset',
                    num_samples=117,
                    size_limit=1 << 8)
-    dataset = StreamingDataset(local=local, remote=remote)
+    dataset = StreamingDataset(local=local, remote=remote, batch_size=1)
 
     # Get the current dataset state dict
     old_state_dict = dataset.state_dict(0, from_beginning)
     assert old_state_dict is not None
 
     state_keys = list(old_state_dict.keys())
 
@@ -93,15 +95,15 @@
 @pytest.mark.usefixtures('local_remote_dir')
 def test_load_get_state_dict_multiple(local_remote_dir: Tuple[str, str], iterations: int):
     local, remote = local_remote_dir
     convert_to_mds(out_root=remote,
                    dataset_name='sequencedataset',
                    num_samples=117,
                    size_limit=1 << 8)
-    dataset = StreamingDataset(local=local, remote=remote)
+    dataset = StreamingDataset(local=local, remote=remote, batch_size=1)
 
     # Get the current dataset state dict
     old_state_dict = dataset.state_dict(0, False)
     assert old_state_dict is not None
 
     state_keys = list(old_state_dict.keys())
 
@@ -134,16 +136,25 @@
 @pytest.mark.usefixtures('local_remote_dir')
 def test_state_dict_too_large(local_remote_dir: Tuple[str, str]):
     local, remote = local_remote_dir
     convert_to_mds(out_root=remote,
                    dataset_name='sequencedataset',
                    num_samples=117,
                    size_limit=1 << 8)
-    dataset = StreamingDataset(local=local, remote=remote)
+    dataset = StreamingDataset(local=local, remote=remote, batch_size=1)
 
     # Make a state dict that is too large to fit in the allocated shared memory.
     import mmap
     key = 'a' * mmap.PAGESIZE
     big_state_dict = {key: 1}
 
     with pytest.raises(ValueError, match='The StreamingDataset state dict*'):
         dataset.load_state_dict(big_state_dict)
+
+
+@pytest.mark.parametrize('dtype', [np.int32, np.int64, np.float32, np.float64])
+@patch('streaming.base.shared.array.SharedMemory')
+def test_shared_array_size_is_integer(mock_shared_memory: Type, dtype: Type[np.dtype]):
+    SharedArray(3, dtype=dtype, name='test_shared_array')
+    mock_shared_memory.assert_called_once()
+    size_arg = mock_shared_memory.call_args[1]['size']
+    assert isinstance(size_arg, int), 'Size passed to SharedMemory is not an integer'
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_shuffle.py` & `mosaicml-streaming-0.7.5/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_spanner.py` & `mosaicml-streaming-0.7.5/tests/test_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_stream.py` & `mosaicml-streaming-0.7.5/tests/test_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,8 @@
     convert_to_mds(out_root=remote_dir, dataset_name='sequencedataset', num_samples=num_samples)
     if os.path.exists(os.path.join(remote_dir, 'index.json')):
         os.remove(os.path.join(remote_dir, 'index.json'))
     else:
         raise Exception(f"Missing {os.path.join(remote_dir, 'index.json')}")
     stream = Stream(remote=None, local=remote_dir)
     with pytest.raises(RuntimeError, match='No `remote` provided, but local file.*'):
-        _ = StreamingDataset(streams=[stream])
+        _ = StreamingDataset(streams=[stream], batch_size=1)
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_streaming.py` & `mosaicml-streaming-0.7.5/tests/test_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,46 @@
 
 from streaming.base import Stream, StreamingDataLoader, StreamingDataset
 from streaming.base.util import clean_stale_shared_memory
 from tests.common.utils import convert_to_mds
 
 
 @pytest.mark.usefixtures('local_remote_dir')
+def test_no_batch_size_exception(local_remote_dir: Tuple[str, str]):
+
+    remote_dir, local_dir = local_remote_dir
+    convert_to_mds(out_root=remote_dir,
+                   dataset_name='sequencedataset',
+                   num_samples=200,
+                   size_limit=1 << 8)
+
+    # Build StreamingDataset
+    dataset = StreamingDataset(local=local_dir, remote=remote_dir)
+    # Build DataLoader
+    dataloader = StreamingDataLoader(dataset=dataset, batch_size=2, num_workers=2, drop_last=True)
+
+    with pytest.raises(ValueError, match=f'Please pass `batch_size` to StreamingDataset*'):
+        # When we iterate through the dataloader, we should throw an error because
+        # we have not passed in batch size to the StreamingDataset. Instantiation of
+        # StreamingDataset is still fine though.
+        for _ in dataloader:
+            pass
+
+
+@pytest.mark.usefixtures('local_remote_dir')
 def test_new_defaults_warning(local_remote_dir: Tuple[str, str], caplog: Callable):
     caplog.set_level(logging.WARNING)
     local, remote = local_remote_dir
     convert_to_mds(out_root=remote,
                    dataset_name='sequencedataset',
                    num_samples=100,
                    size_limit=1 << 8)
 
     # Build a StreamingDataset with new defaults. Should warn about the new defaults changes.
-    dataset = StreamingDataset(local=local, remote=remote, shuffle=True)
+    dataset = StreamingDataset(local=local, remote=remote, shuffle=True, batch_size=4)
     dataloader = StreamingDataLoader(dataset=dataset, batch_size=4)
     for _ in dataloader:
         pass
 
     assert 'Because `predownload` was not specified,' in caplog.text
     assert 'Because `shuffle_block_size` was not specified,' in caplog.text
     assert 'Because `num_canonical_nodes` was not specified,' in caplog.text
@@ -511,15 +533,15 @@
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dataloader_mid_epoch_exit(local_remote_dir: Tuple[str, str], num_samples: int, seed: int):
     local, remote = local_remote_dir
     convert_to_mds(out_root=remote, dataset_name='sequencedataset', num_samples=num_samples)
 
     def run_one_iter(local: str, remote: str, seed: int) -> None:
         # Build a StreamingDataset
-        dataset = StreamingDataset(local=local, remote=remote, shuffle_seed=seed)
+        dataset = StreamingDataset(local=local, remote=remote, shuffle_seed=seed, batch_size=1)
 
         # Do one iteration
         it = iter(dataset)
         next(it)
         # Test if we can exit...
 
     p = Process(target=run_one_iter, args=(local, remote, seed))
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_streaming_remote.py` & `mosaicml-streaming-0.7.5/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_unsafe_types.py` & `mosaicml-streaming-0.7.5/tests/test_unsafe_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 def test_do_allow_unsafe_types_safe(local_remote_dir: Tuple[str, str]):
     local, _ = local_remote_dir
     columns = {'num': 'int'}
     with MDSWriter(out=local, columns=columns) as out:
         for num in range(100):
             sample = {'num': num}
             out.write(sample)
-    StreamingDataset(local=local, allow_unsafe_types=True)
+    StreamingDataset(local=local, allow_unsafe_types=True, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_do_allow_unsafe_types_unsafe(local_remote_dir: Tuple[str, str]):
     local, _ = local_remote_dir
     columns = {'num': 'pkl'}
     with MDSWriter(out=local, columns=columns) as out:
         for num in range(100):
             sample = {'num': num}
             out.write(sample)
-    StreamingDataset(local=local, allow_unsafe_types=True)
+    StreamingDataset(local=local, allow_unsafe_types=True, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dont_allow_unsafe_types_safe(local_remote_dir: Tuple[str, str]):
     local, _ = local_remote_dir
     columns = {'num': 'int'}
     with MDSWriter(out=local, columns=columns) as out:
         for num in range(100):
             sample = {'num': num}
             out.write(sample)
-    StreamingDataset(local=local)
+    StreamingDataset(local=local, batch_size=1)
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dont_allow_unsafe_types_unsafe(local_remote_dir: Tuple[str, str]):
     local, _ = local_remote_dir
     columns = {'num': 'pkl'}
     with MDSWriter(out=local, columns=columns) as out:
         for num in range(100):
             sample = {'num': num}
             out.write(sample)
     with pytest.raises(ValueError, match='.*contains an unsafe type.*'):
-        StreamingDataset(local=local)
+        StreamingDataset(local=local, batch_size=1)
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_upload.py` & `mosaicml-streaming-0.7.5/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.4/tests/test_util.py` & `mosaicml-streaming-0.7.5/tests/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     input_data = ['', '12kbb', '27mxb', '79bk', '79bb', '79 b    m', 'p 64', '64p']
     for value in input_data:
         with pytest.raises(ValueError, match=f'Unsupported value/suffix.*'):
             _ = number_abbrev_to_int(value)
 
 
 def test_clean_stale_shared_memory():
+    # Clean up the stale shared memory
+    clean_stale_shared_memory()
+
     # Create a leaked shared memory
     name = _get_path(0, RESUME)
     _ = BuiltinSharedMemory(name, True, 64)
 
     # Clean up the stale shared memory
     clean_stale_shared_memory()
```

### Comparing `mosaicml-streaming-0.7.4/tests/test_writer.py` & `mosaicml-streaming-0.7.5/tests/test_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -109,22 +109,50 @@
                        size_limit=size_limit) as out:
             for sample in dataset:
                 out.write(sample)
 
         # Apply the seed again for numpy determinism
         dataset.seed = seed
 
-        mds_dataset = StreamingDataset(local=local, shuffle=False)
+        mds_dataset = StreamingDataset(local=local, shuffle=False, batch_size=1)
         # Ensure length of dataset is equal
         assert len(dataset) == len(mds_dataset) == num_samples
 
         # Ensure sample iterator is deterministic
         for before, after in zip(dataset, mds_dataset):
             assert before == after
 
+    def test_exist_ok(self, local_remote_dir: Tuple[str, str]) -> None:
+        num_samples = 1000
+        size_limit = 4096
+        local, _ = local_remote_dir
+        dataset = SequenceDataset(num_samples)
+        columns = dict(zip(dataset.column_names, dataset.column_encodings))
+
+        # Write entire dataset initially
+        with MDSWriter(out=local, columns=columns, size_limit=size_limit) as out:
+            for sample in dataset:
+                out.write(sample)
+        num_orig_files = len(os.listdir(local))
+
+        # Write single sample with exist_ok set to True
+        with MDSWriter(out=local, columns=columns, size_limit=size_limit, exist_ok=True) as out:
+            out.write(dataset[0])
+        num_files = len(os.listdir(local))
+
+        # Two files for single sample (index.json and one shard)
+        assert num_files == 2
+        # Should be more files generated for the entire dataset, which are then deleted as exist_ok is True
+        assert num_orig_files > num_files
+
+        # Check exception is raised when exist_ok is False and local already exists
+        with pytest.raises(FileExistsError, match='Directory is not empty'):
+            with MDSWriter(out=local, columns=columns, size_limit=size_limit) as out:
+                out.write(dataset[0])
+
 
 class TestJSONWriter:
 
     @pytest.mark.parametrize('num_samples', [100])
     @pytest.mark.parametrize('size_limit', [32])
     def test_config(self, local_remote_dir: Tuple[str, str], num_samples: int,
                     size_limit: int) -> None:
@@ -165,22 +193,50 @@
                         size_limit=size_limit) as out:
             for sample in dataset:
                 out.write(sample)
 
         # Apply the seed again for numpy determinism
         dataset.seed = seed
 
-        mds_dataset = StreamingDataset(local=local, shuffle=False)
+        mds_dataset = StreamingDataset(local=local, shuffle=False, batch_size=1)
         # Ensure length of dataset is equal
         assert len(dataset) == len(mds_dataset) == num_samples
 
         # Ensure sample iterator is deterministic
         for before, after in zip(dataset, mds_dataset):
             assert before == after
 
+    def test_exist_ok(self, local_remote_dir: Tuple[str, str]) -> None:
+        num_samples = 1000
+        size_limit = 4096
+        local, _ = local_remote_dir
+        dataset = SequenceDataset(num_samples)
+        columns = dict(zip(dataset.column_names, dataset.column_encodings))
+
+        # Write entire dataset initially
+        with JSONWriter(out=local, columns=columns, size_limit=size_limit) as out:
+            for sample in dataset:
+                out.write(sample)
+        num_orig_files = len(os.listdir(local))
+
+        # Write single sample with exist_ok set to True
+        with JSONWriter(out=local, columns=columns, size_limit=size_limit, exist_ok=True) as out:
+            out.write(dataset[0])
+        num_files = len(os.listdir(local))
+
+        # Three files for single sample (index.json, one shard, and one shard metadata)
+        assert num_files == 3
+        # Should be more files generated for the entire dataset, which are then deleted as exist_ok is True
+        assert num_orig_files > num_files
+
+        # Check exception is raised when exist_ok is False and local already exists
+        with pytest.raises(FileExistsError, match='Directory is not empty'):
+            with JSONWriter(out=local, columns=columns, size_limit=size_limit) as out:
+                out.write(dataset[0])
+
 
 class TestXSVWriter:
 
     @pytest.mark.parametrize('num_samples', [100])
     @pytest.mark.parametrize('size_limit', [32])
     @pytest.mark.parametrize(('writer', 'name'), [(XSVWriter, 'xsv'), (TSVWriter, 'tsv'),
                                                   (CSVWriter, 'csv')])
@@ -245,14 +301,61 @@
                         size_limit=size_limit) as out:
                 for sample in dataset:
                     out.write(sample)
 
         # Apply the seed again for numpy determinism
         dataset.seed = seed
 
-        mds_dataset = StreamingDataset(local=local, shuffle=False)
+        mds_dataset = StreamingDataset(local=local, shuffle=False, batch_size=1)
         # Ensure length of dataset is equal
         assert len(dataset) == len(mds_dataset) == num_samples
 
         # Ensure sample iterator is deterministic
         for before, after in zip(dataset, mds_dataset):
             assert before == after
+
+    @pytest.mark.parametrize('writer', [XSVWriter, TSVWriter, CSVWriter])
+    def test_exist_ok(self, local_remote_dir: Tuple[str, str], writer: Any) -> None:
+        num_samples = 1000
+        size_limit = 4096
+        local, _ = local_remote_dir
+        dataset = SequenceDataset(num_samples)
+        columns = dict(zip(dataset.column_names, dataset.column_encodings))
+
+        # Write entire dataset initially
+        if writer.__name__ == XSVWriter.__name__:
+            with writer(out=local, columns=columns, size_limit=size_limit, separator=',') as out:
+                for sample in dataset:
+                    out.write(sample)
+        else:
+            with writer(out=local, columns=columns, size_limit=size_limit) as out:
+                for sample in dataset:
+                    out.write(sample)
+        num_orig_files = len(os.listdir(local))
+
+        # Write single sample with exist_ok set to True
+        if writer.__name__ == XSVWriter.__name__:
+            with writer(out=local,
+                        columns=columns,
+                        size_limit=size_limit,
+                        separator=',',
+                        exist_ok=True) as out:
+                out.write(dataset[0])
+        else:
+            with writer(out=local, columns=columns, size_limit=size_limit, exist_ok=True) as out:
+                out.write(dataset[0])
+        num_files = len(os.listdir(local))
+
+        # Three files for single sample (index.json, one shard, and one shard metadata)
+        assert num_files == 3
+        # Should be more files generated for the entire dataset, which are then deleted as exist_ok is True
+        assert num_orig_files > num_files
+
+        # Check exception is raised when exist_ok is False and local already exists
+        with pytest.raises(FileExistsError, match='Directory is not empty'):
+            if writer.__name__ == XSVWriter.__name__:
+                with writer(out=local, columns=columns, size_limit=size_limit,
+                            separator=',') as out:
+                    out.write(dataset[0])
+            else:
+                with writer(out=local, columns=columns, size_limit=size_limit) as out:
+                    out.write(dataset[0])
```

