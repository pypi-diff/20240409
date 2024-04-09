# Comparing `tmp/modelbest_sdk-0.1.1.tar.gz` & `tmp/modelbest_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbest_sdk-0.1.1.tar", last modified: Sun Apr  7 08:02:30 2024, max compression
+gzip compressed data, was "modelbest_sdk-0.1.2.tar", last modified: Tue Apr  9 08:09:40 2024, max compression
```

## Comparing `modelbest_sdk-0.1.1.tar` & `modelbest_sdk-0.1.2.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.347490 modelbest_sdk-0.1.1/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       99 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/MANIFEST.in
--rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-07 08:02:30.347490 modelbest_sdk-0.1.1/PKG-INFO
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      488 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/README.md
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.336490 modelbest_sdk-0.1.1/modelbest_sdk/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/modelbest_sdk/__init__.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.337490 modelbest_sdk-0.1.1/modelbest_sdk/dataset/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2606 2024-04-03 09:06:32.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/cache.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.338490 modelbest_sdk-0.1.1/modelbest_sdk/dataset/collater/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/collater/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4998 2024-04-07 07:46:57.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/collater/batched_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       53 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/collater/collater.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3241 2024-04-03 08:49:54.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/cuda_prefetcher.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1158 2024-04-03 09:13:40.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/dataset_context_test.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7949 2024-04-07 07:50:10.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/mbtable_iterable_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2667 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/range.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.338490 modelbest_sdk-0.1.1/modelbest_sdk/dataset/sampler/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/sampler/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       56 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/sampler/sampler.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3980 2024-04-07 07:47:05.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/sampler/weighted_dataset.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2252 2024-04-07 07:47:28.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/table_record_dataset.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.339490 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:53:00.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1850 2024-04-03 08:51:12.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     6644 2024-04-03 10:33:19.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2220 2024-04-03 09:25:49.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      896 2024-04-03 07:56:34.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/utils.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      459 2024-04-03 09:14:58.000000 modelbest_sdk-0.1.1/modelbest_sdk/dataset/utils.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.339490 modelbest_sdk-0.1.1/modelbest_sdk/file_format/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/modelbest_sdk/file_format/__init__.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.339490 modelbest_sdk-0.1.1/modelbest_sdk/file_format/lib/
--rwxrwxr-x   0 emr-user  (1000) emr-user  (1000)  7114128 2024-03-26 09:17:44.000000 modelbest_sdk-0.1.1/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4768 2024-03-29 10:09:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2895 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable_builder.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4699 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable_partition.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.346490 modelbest_sdk-0.1.1/modelbest_sdk/proto/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      405 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/breadcrumb.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3060 2024-04-02 07:22:05.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/chatdoc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1136 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/const.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      830 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/context.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3846 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/data_base.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      631 2024-03-29 12:04:58.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/dataset_checkpoint.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      454 2024-04-03 08:15:57.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/dataset_context.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1806 2024-03-28 08:57:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/general_doc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1624 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/general_servlet_rpc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3408 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/linkinfo.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1501 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/mergeddoc.thrift
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      477 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.1/modelbest_sdk/proto/traindoc.thrift
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.337490 modelbest_sdk-0.1.1/modelbest_sdk.egg-info/
--rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-07 08:02:30.000000 modelbest_sdk-0.1.1/modelbest_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1817 2024-04-07 08:02:30.000000 modelbest_sdk-0.1.1/modelbest_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        1 2024-04-07 08:02:30.000000 modelbest_sdk-0.1.1/modelbest_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       19 2024-04-07 08:02:30.000000 modelbest_sdk-0.1.1/modelbest_sdk.egg-info/top_level.txt
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       38 2024-04-07 08:02:30.347490 modelbest_sdk-0.1.1/setup.cfg
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      708 2024-04-07 08:02:20.000000 modelbest_sdk-0.1.1/setup.py
-drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-07 08:02:30.347490 modelbest_sdk-0.1.1/test/
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-01 08:13:07.000000 modelbest_sdk-0.1.1/test/__init__.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1209 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.1/test/generate_data.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2682 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/test/test_mbtable.py
--rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2248 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.1/test/test_mbtable_partition.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       99 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/MANIFEST.in
+-rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/PKG-INFO
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      488 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/README.md
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.929721 modelbest_sdk-0.1.2/modelbest_sdk/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/__init__.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2606 2024-04-03 09:06:32.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/cache.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4909 2024-04-09 08:07:57.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/batched_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       53 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/collater.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3241 2024-04-03 08:49:54.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/cuda_prefetcher.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7949 2024-04-07 07:50:10.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/mbtable_iterable_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2667 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/range.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.931722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:33:51.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       56 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/sampler.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3980 2024-04-07 07:47:05.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/weighted_dataset.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3531 2024-04-08 12:38:43.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/table_record_dataset.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-04-03 03:53:00.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1928 2024-04-08 08:15:10.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/base_doc.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     7606 2024-04-08 12:19:40.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2220 2024-04-03 09:25:49.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      896 2024-04-03 07:56:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/utils.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      464 2024-04-08 12:39:26.000000 modelbest_sdk-0.1.2/modelbest_sdk/dataset/utils.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/file_format/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/__init__.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.932722 modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/
+-rwxrwxr-x   0 emr-user  (1000) emr-user  (1000)  7114128 2024-03-26 09:17:44.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4768 2024-03-29 10:09:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2895 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_builder.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4699 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_partition.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.940722 modelbest_sdk-0.1.2/modelbest_sdk/proto/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      405 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/breadcrumb.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3060 2024-04-02 07:22:05.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/chatdoc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1136 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/const.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      830 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/context.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3846 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/data_base.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      631 2024-03-29 12:04:58.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_checkpoint.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      454 2024-04-03 08:15:57.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_context.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1806 2024-03-28 08:57:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/general_doc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1624 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/general_servlet_rpc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     3408 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/linkinfo.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1501 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/mergeddoc.thrift
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      477 2024-03-26 07:14:29.000000 modelbest_sdk-0.1.2/modelbest_sdk/proto/traindoc.thrift
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.930722 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/
+-rw-r--r--   0 emr-user  (1000) emr-user  (1000)      984 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1842 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        1 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       19 2024-04-09 08:09:40.000000 modelbest_sdk-0.1.2/modelbest_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)       38 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/setup.cfg
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)      708 2024-04-09 08:09:34.000000 modelbest_sdk-0.1.2/setup.py
+drwxrwxr-x   0 emr-user  (1000) emr-user  (1000)        0 2024-04-09 08:09:40.941722 modelbest_sdk-0.1.2/test/
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)        0 2024-03-01 08:13:07.000000 modelbest_sdk-0.1.2/test/__init__.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1158 2024-04-03 09:13:40.000000 modelbest_sdk-0.1.2/test/dataset_context_test.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     1209 2024-04-03 03:07:45.000000 modelbest_sdk-0.1.2/test/generate_data.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     4115 2024-04-08 12:42:07.000000 modelbest_sdk-0.1.2/test/test_base.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2289 2024-04-09 08:09:00.000000 modelbest_sdk-0.1.2/test/test_checkpoint.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2682 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/test/test_mbtable.py
+-rw-rw-r--   0 emr-user  (1000) emr-user  (1000)     2248 2024-03-26 08:50:34.000000 modelbest_sdk-0.1.2/test/test_mbtable_partition.py
```

### Comparing `modelbest_sdk-0.1.1/PKG-INFO` & `modelbest_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbest_sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/cache.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/cache.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/collater/batched_dataset.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/collater/batched_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 # from modelbest_sdk.dataset.collater.collater import Collater
 from modelbest_sdk.dataset.sampler.weighted_dataset import WeightedDataset
 from modelbest_sdk.dataset.thrift_wrapper.base_doc import BaseDoc
 from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import *
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 
+def default_factory_list():
+    return list()
+
+def default_factory_dict():
+    return defaultdict(default_factory_list)
 
 class BatchedDataset(torch.utils.data.IterableDataset):
     def __init__(self, context, weighted_dataset, batch_size, max_len, drop_last=False):
         self.context = context
         self.weighted_dataset = weighted_dataset
         self.max_total_length = batch_size * max_len
         self.batch_size = 1
@@ -24,16 +29,15 @@
 
     def put(self, data):
         self.buffer.append(data)
         self.current_length += len(data['doc'].token_ids)
     
     def pop(self):
         lengths = []
-        indexes = defaultdict()
-        
+        indexes = defaultdict(default_factory_dict)        
         inputs = torch.zeros((self.batch_size, self.max_total_length), dtype=torch.int32)
         targets = torch.full((self.batch_size, self.max_total_length), dtype=torch.int32, fill_value=-100)
         dataset_ids = torch.full((self.batch_size, self.max_total_length), dtype=torch.int32, fill_value=-1)
         position_ids = torch.zeros((self.batch_size, self.max_total_length), dtype=torch.int32)
 
         span_begin = 0
         while self.buffer:
@@ -51,28 +55,23 @@
             # TODO: what if the inputs is longer than max_total_length?
             # RuntimeError: The expanded size of the tensor (16) must match the existing size (385) at non-singleton dimension 0.  Target sizes: [16].  Tensor sizes: [385]
             inputs[0, span_begin:span_end] = torch.tensor(token_ids, dtype=torch.int32)
             targets[0, span_begin:span_end] = torch.tensor(target_ids, dtype=torch.int32)
             dataset_ids[0, span_begin:span_end] = torch.tensor(dataset_idx, dtype=torch.int32)
             position_ids[0, span_begin:span_end] = torch.from_numpy(np.arange(len(token_ids), dtype=np.int32))
             lengths.append(len(token_ids))
-            if indexes.get(int(dataset_idx)) is None:
-                indexes[int(dataset_idx)] = {}
-            if indexes[int(dataset_idx)].get(chunk) is None:
-                indexes[int(dataset_idx)][chunk] = []
-                # TODO: better way
             indexes[int(dataset_idx)][chunk].append(index)
             span_begin = span_end
         cu_seqlens = torch.cat(
             [torch.tensor([0] + lengths).cumsum(dim=-1), torch.tensor([self.max_total_length], dtype=torch.int32)],
             dim=0,
         ).int()
         batch = {
-            "inputs": inputs,
-            "targets": targets,
+            "input_ids": inputs,
+            "target_ids": targets,
             "dataset_ids": dataset_ids,
             "indexes": indexes,
             "cu_seqlens": cu_seqlens,
             "max_seqlen": int(torch.max(cu_seqlens[1:] - cu_seqlens[:-1])),
             "lengths": torch.tensor(sum(lengths)).int(),
             "position_ids": position_ids,
             # TODO: add tags
@@ -80,22 +79,22 @@
         self.current_length = 0
         return batch
         # TODO: return data directly, and pack in collate_fn
         
 
     def will_exceed(self, data):
         return self.current_length + len(data['doc'].token_ids) > self.max_total_length
-        
 
     def __iter__(self):
         for data in self.weighted_dataset:
             if self.will_exceed(data):
                 yield self.pop()
             self.put(data)
-        # TODO: drop last batch if it is not full
+        if not self.drop_last and self.buffer:
+            yield self.pop()
 
     @staticmethod
     def collate_fn(batch):
         return batch[0]
     
 
 if __name__ == '__main__':
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/cuda_prefetcher.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/cuda_prefetcher.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/dataset_context_test.py` & `modelbest_sdk-0.1.2/test/dataset_context_test.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/mbtable_iterable_dataset.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/mbtable_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/range.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/range.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/sampler/weighted_dataset.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/sampler/weighted_dataset.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/table_record_dataset.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/table_record_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import os
 import torch
 from modelbest_sdk.dataset.collater.batched_dataset import BatchedDataset
 from modelbest_sdk.dataset.sampler.weighted_dataset import WeightedDataset
-from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import DatasetInfo, DatasetInfoList
+from modelbest_sdk.dataset.thrift_wrapper.dataset_checkpoint import DatasetCheckpointList, DatasetInfo, DatasetInfoList
 from modelbest_sdk.dataset.thrift_wrapper.dataset_context import DatasetContext
 
 
 class TableRecordDataset(torch.utils.data.IterableDataset):
     def __init__(
         self,
         context: DatasetContext,
@@ -13,14 +14,15 @@
         max_len=4096,
         prefetch_chunk_cnt=20,
         chunk_size=1024,
         num_workers=1,
         prefetch_factor=20,
         cuda_prefetch=True
     ):
+        self.context = context
         dataset_info_list = DatasetInfoList.load_from_file(context.dataset_config_path)
         
         self.weighted_dataset = WeightedDataset(
             context=context, 
             dataset_info_list=dataset_info_list,
             prefetch_chunk_cnt=prefetch_chunk_cnt,
             chunk_size=chunk_size
@@ -62,8 +64,28 @@
         return self.weighted_dataset.checkpoint()
     
     def load_checkpoint(self, checkpoint):
         self.weighted_dataset.load_checkpoint(checkpoint)
         
     def update(self, dataset_entries):
         self.weighted_dataset.update(dataset_entries)
-        
+    
+    def save(self):
+        path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_{self.context.rank}.mbt")
+        self.checkpoint().save_to_file(path)
+        
+    def resume(self):
+        new_world_size = self.context.world_size
+        first_rank_ckpt_path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_0.mbt")
+        cur_rank_ckpt_path = os.path.join(self.context.dataset_checkpoint_path, f"dataset_ckpt_rank_{self.context.rank}.mbt")
+        old_world_size = DatasetCheckpointList.load_from_file(first_rank_ckpt_path).world_size
+        if new_world_size == old_world_size:
+            self.weighted_dataset.load_checkpoint(DatasetCheckpointList.load_from_file(cur_rank_ckpt_path))
+        else:
+            merged_ckpt = None
+            for path in os.listdir(self.context.dataset_checkpoint_path):
+                abs_path = os.path.join(self.context.dataset_checkpoint_path, path)
+                if merged_ckpt is None:
+                    merged_ckpt = DatasetCheckpointList.load_from_file(abs_path)
+                else:
+                    merged_ckpt.merge(DatasetCheckpointList.load_from_file(abs_path))
+            self.load_checkpoint(merged_ckpt)
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/base_doc.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/base_doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,30 @@
 proto_dir = os.path.join(os.path.dirname(__file__), "../..", "proto")
 
 doc_thrift = thriftpy2.load(os.path.join(proto_dir, "traindoc.thrift"), module_name="doc_thrift")
 logger = logging.getLogger(__name__)
 
 
 class BaseDoc:
-    def __init__(self, token_ids, mask=None, docid=None, tag=None, token=None, tokenizer_version=None, reserved_col=None):
+    def __init__(self, token_ids=None, mask=None, docid=None, tag=None, token=None, tokenizer_version=None, reserved_col=None):
         self.token_ids = token_ids
         self.mask = mask
         self.docid = docid
         self.tag = tag
         self.token = token
         self.tokenizer_version = tokenizer_version
         self.reserved_col = reserved_col
     
     @staticmethod
     def deserialize(bin):
         return BaseDoc.from_thrift(deserialize(doc_thrift.BaseDoc(), bin))
     
+    def serialize(self):
+        return serialize(self.to_thrift())
+    
     def to_thrift(self):
         return doc_thrift.BaseDoc(
             token_ids=self.token_ids,
             mask=self.mask,
             docid=self.docid,
             tag=self.tag,
             token=self.token,
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_checkpoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 dc_thrift.Chunk.__hash__ = lambda self: hash((self.epoch, self.start, self.stop))
 
 logger = logging.getLogger(__name__)
 
 
 class DatasetCheckpointList:
     def __init__(self, checkpoint_list, world_size=None, tp_size=None):
-        self.checkpoint_list = checkpoint_list
+        self.checkpoint_list: List[DatasetCheckpoint] = checkpoint_list
         self.world_size = world_size
         self.tp_size = tp_size
         
     @staticmethod
     def load_from_file(path):
         return DatasetCheckpointList.from_thrift(deserialize(dc_thrift.DatasetCheckpointList(), Utils.load_from_file(path)))
 
@@ -39,26 +39,36 @@
     def from_thrift(thrift_checkpoint_list):
         checkpoint = [DatasetCheckpoint.from_thrift(checkpoint) for checkpoint in thrift_checkpoint_list.checkpoint_list]
         return DatasetCheckpointList(
             checkpoint_list=checkpoint,
             world_size=thrift_checkpoint_list.world_size,
             tp_size=thrift_checkpoint_list.tp_size
         )
-        
+    
+    def merge(self, other: 'DatasetCheckpointList'):
+        # Note that we assume that the two dataset checkpoint lists have the same length and the same order of datasets.
+        # merge the dataset with same path
+        for i in range(len(self.checkpoint_list)):
+            self.checkpoint_list[i].merge(other.checkpoint_list[i])
+            
     def __repr__(self) -> str:
         return f"DatasetCheckpointList(checkpoint_list={self.checkpoint_list}, world_size={self.world_size}, tp_size={self.tp_size})"
         
 
 
 class DatasetCheckpoint:
     def __init__(self, dataset_info, used=None, chunk_size=None, num_chunks=None):
-        self.dataset_info = dataset_info
+        self.dataset_info: DatasetInfo = dataset_info
         self.used: Used = used
         self.chunk_size = chunk_size
         self.num_chunks = num_chunks
+    
+    def merge(self, other: 'DatasetCheckpoint'):
+        assert self.dataset_info.path == other.dataset_info.path
+        self.used.merge(other.used)
 
     def to_thrift(self):
         thrift_dataset_info = self.dataset_info.to_thrift() if self.dataset_info else None
         thrift_used = self.used.to_thrift() if self.used else None
         return dc_thrift.DatasetCheckpoint(
             dataset_info=thrift_dataset_info,
             used=thrift_used,
@@ -131,15 +141,26 @@
 
 
 class Used:
     def __init__(self):
         self.active: Dict[Chunk, Set[int]] = {}
         self.done: Dict[int, Set[Chunk]] = {}
         self.epoch: int = 0
-
+    
+    def merge(self, other: 'Used'):
+        for chunk, index_set in other.active.items():
+            if chunk not in self.active:
+                self.active[chunk] = set()
+            self.active[chunk].update(index_set)
+        
+        for epoch, chunk_set in other.done.items():
+            if epoch not in self.done:
+                self.done[epoch] = set()
+            self.done[epoch].update(chunk_set)
+        
     def to_thrift(self):
         thrift_active = {chunk.to_thrift(): index_set for chunk, index_set in self.active.items()}
         thrift_done = {epoch: {chunk.to_thrift() for chunk in chunk_set} for epoch, chunk_set in self.done.items()}
         return dc_thrift.Used(active=thrift_active, done=thrift_done, epoch=self.epoch)
 
     @staticmethod
     def from_thrift(thrift_used):
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/dataset_context.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/dataset/thrift_wrapper/utils.py` & `modelbest_sdk-0.1.2/modelbest_sdk/dataset/thrift_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so` & `modelbest_sdk-0.1.2/modelbest_sdk/file_format/lib/libmbtable_sdk_shared.so`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable.py` & `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable_builder.py` & `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_builder.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/file_format/mbtable_partition.py` & `modelbest_sdk-0.1.2/modelbest_sdk/file_format/mbtable_partition.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/chatdoc.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/chatdoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/const.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/const.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/context.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/context.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/data_base.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/data_base.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/dataset_checkpoint.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/dataset_checkpoint.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/general_doc.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/general_doc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/general_servlet_rpc.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/general_servlet_rpc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/linkinfo.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/linkinfo.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk/proto/mergeddoc.thrift` & `modelbest_sdk-0.1.2/modelbest_sdk/proto/mergeddoc.thrift`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk.egg-info/PKG-INFO` & `modelbest_sdk-0.1.2/modelbest_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbest-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Everything about modelbest data include data format mbtable, dataset, dataloader, and tools
 Home-page: https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk
 Author: HankyZhao
 Author-email: zhq980115@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modelbest_sdk-0.1.1/modelbest_sdk.egg-info/SOURCES.txt` & `modelbest_sdk-0.1.2/modelbest_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 modelbest_sdk.egg-info/PKG-INFO
 modelbest_sdk.egg-info/SOURCES.txt
 modelbest_sdk.egg-info/dependency_links.txt
 modelbest_sdk.egg-info/top_level.txt
 modelbest_sdk/dataset/__init__.py
 modelbest_sdk/dataset/cache.py
 modelbest_sdk/dataset/cuda_prefetcher.py
-modelbest_sdk/dataset/dataset_context_test.py
 modelbest_sdk/dataset/mbtable_iterable_dataset.py
 modelbest_sdk/dataset/range.py
 modelbest_sdk/dataset/table_record_dataset.py
 modelbest_sdk/dataset/utils.py
 modelbest_sdk/dataset/collater/__init__.py
 modelbest_sdk/dataset/collater/batched_dataset.py
 modelbest_sdk/dataset/collater/collater.py
@@ -39,10 +38,13 @@
 modelbest_sdk/proto/dataset_context.thrift
 modelbest_sdk/proto/general_doc.thrift
 modelbest_sdk/proto/general_servlet_rpc.thrift
 modelbest_sdk/proto/linkinfo.thrift
 modelbest_sdk/proto/mergeddoc.thrift
 modelbest_sdk/proto/traindoc.thrift
 test/__init__.py
+test/dataset_context_test.py
 test/generate_data.py
+test/test_base.py
+test/test_checkpoint.py
 test/test_mbtable.py
 test/test_mbtable_partition.py
```

### Comparing `modelbest_sdk-0.1.1/setup.py` & `modelbest_sdk-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modelbest_sdk',
-    version='0.1.1',
+    version='0.1.2',
     author='HankyZhao',
     author_email='zhq980115@gmail.com',
     description='Everything about modelbest data include data format mbtable, dataset, dataloader, and tools',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url='https://codeup.aliyun.com/64ddb0a87f62ff9b3d23ca15/modelbest_sdk',
     packages=find_packages(),
```

### Comparing `modelbest_sdk-0.1.1/test/generate_data.py` & `modelbest_sdk-0.1.2/test/generate_data.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/test/test_mbtable.py` & `modelbest_sdk-0.1.2/test/test_mbtable.py`

 * *Files identical despite different names*

### Comparing `modelbest_sdk-0.1.1/test/test_mbtable_partition.py` & `modelbest_sdk-0.1.2/test/test_mbtable_partition.py`

 * *Files identical despite different names*

