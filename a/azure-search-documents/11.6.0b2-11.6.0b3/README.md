# Comparing `tmp/azure-search-documents-11.6.0b2.tar.gz` & `tmp/azure-search-documents-11.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-search-documents-11.6.0b2.tar", last modified: Wed Mar  6 01:06:13 2024, max compression
+gzip compressed data, was "azure-search-documents-11.6.0b3.tar", last modified: Mon Apr  8 19:38:40 2024, max compression
```

## Comparing `azure-search-documents-11.6.0b2.tar` & `azure-search-documents-11.6.0b3.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15812 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23232 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22200 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4081 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/TROUBLESHOOTING.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.863493 azure-search-documents-11.6.0b2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.863493 azure-search-documents-11.6.0b2/azure/search/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.867493 azure-search-documents-11.6.0b2/azure/search/documents/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1822 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      482 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_api_versions.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.867493 azure-search-documents-11.6.0b2/azure/search/documents/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2644 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4709 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      677 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.871493 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2654 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4832 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_search_index_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.871493 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48338 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/_documents_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.871493 azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3969 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   117033 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15647 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_search_index_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.871493 azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    66326 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/_documents_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      843 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_headers_mixin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6159 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_index_documents_batch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6326 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_paging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4902 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_queries.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38222 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_search_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      491 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_search_documents_error.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15064 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_search_indexing_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2193 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_search_indexing_buffered_sender_base.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1903 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      252 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.875493 azure-search-documents-11.6.0b2/azure/search/documents/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1553 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/_index_documents_batch_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6013 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/_paging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39096 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/_search_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15395 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/aio/_timer.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.875493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.875493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2410 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5999 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_search_service_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1216 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.875493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2420 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6142 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_search_service_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      956 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_vendor.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.879493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27284 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27285 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42751 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38620 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4008 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34101 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25922 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.879493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18651 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   541517 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    73511 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.883493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33426 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34097 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54682 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47543 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4897 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42553 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32425 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27197 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30999 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_search_indexer_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/_utils.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.883493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28240 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30031 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/_search_indexer_client.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.883493 azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12877 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_edm.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47306 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_index.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56166 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_models.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.883493 azure-search-documents-11.6.0b2/azure/search/documents/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2256 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/azure/search/documents/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23232 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8934 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       59 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-06 01:06:13.000000 azure-search-documents-11.6.0b2/azure_search_documents.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.887493 azure-search-documents-11.6.0b2/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6100 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.891492 azure-search-documents-11.6.0b2/samples/async_samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1659 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_analyze_text_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3587 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_authentication_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1679 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_autocomplete_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1899 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2364 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3083 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_data_source_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1797 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_facet_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1875 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_filter_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1721 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_get_document_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3501 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_index_alias_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1816 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_index_client_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4218 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_index_crud_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4321 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_indexers_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1912 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_query_session_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1800 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_search_client_send_request_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2369 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_semantic_search_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1705 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_simple_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1756 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_suggestions_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2546 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_synonym_map_operations_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7302 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/async_samples/sample_vector_search_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_analyze_text.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3361 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_authentication.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1564 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_autocomplete.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1788 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2166 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2826 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_data_source_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1672 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_facet_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1734 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_filter_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_get_document.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3275 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_index_alias_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1733 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_index_client_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_index_crud_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6067 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_indexer_datasource_skillset.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3878 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_indexers_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1792 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_query_session.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1717 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_search_client_send_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2395 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_semantic_search.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1584 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_simple_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1630 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_suggestions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2901 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_synonym_map_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7072 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/samples/sample_vector_search.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2399 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.895492 azure-search-documents-11.6.0b2/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/tests/async_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6471 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_buffered_sender_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1364 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_basic_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7227 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_buffered_sender_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6927 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_index_document_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6354 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_search_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4454 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_alias_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6323 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_data_source_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8070 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10270 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_skillset_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6112 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_synonym_map_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8040 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/async_tests/test_search_indexer_client_live_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1263 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:06:13.899492 azure-search-documents-11.6.0b2/tests/perfstress_tests/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/perfstress_tests/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2340 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/perfstress_tests/autocomplete.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2300 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/perfstress_tests/search_documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2305 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/perfstress_tests/suggest.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29583 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/search_service_preparer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_buffered_sender.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2164 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_index_documents_batch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3222 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_index_field_helpers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5887 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_queries.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_regex_flags.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14537 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2013 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_client_basic_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6790 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_client_buffered_sender_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6608 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_client_index_document_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5129 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_client_search_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5018 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4130 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client_alias_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6883 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client_data_source_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7627 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11708 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client_skillset_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5759 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_index_client_synonym_map_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7675 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_search_indexer_client_live.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4093 2024-03-06 01:05:25.000000 azure-search-documents-11.6.0b2/tests/test_serialization.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16245 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/MANIFEST.in
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23034 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22009 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4081 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/TROUBLESHOOTING.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.944076 azure-search-documents-11.6.0b3/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.944076 azure-search-documents-11.6.0b3/azure/search/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      251 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1822 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      482 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_api_versions.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2644 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4709 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      677 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      737 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2654 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4832 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_search_index_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.948076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48338 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_documents_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3969 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   117033 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15647 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_search_index_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      688 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    66326 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_documents_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_generated/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      843 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_headers_mixin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6159 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_index_documents_batch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6326 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_paging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4902 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_queries.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38222 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      491 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_documents_error.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15064 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender_base.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1903 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      252 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1553 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5980 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_index_documents_batch_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6013 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_paging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    39096 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15395 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      673 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/aio/_timer.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.952076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2410 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5999 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_search_service_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1216 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      743 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2420 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6142 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_search_service_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      956 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_vendor.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.956076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27284 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27285 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42751 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38620 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4038 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34101 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25922 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18753 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   541670 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    73409 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1221 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33426 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34097 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    54682 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47543 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4927 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42553 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32425 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27197 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30999 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_indexer_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3193 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.960076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1479 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28240 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30031 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_indexer_client.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.964076 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13422 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      624 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_edm.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    48235 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_index.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56166 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_models.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.964076 azure-search-documents-11.6.0b3/azure/search/documents/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2256 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/azure/search/documents/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/
+-rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    23034 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8934 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       52 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-04-08 19:38:40.000000 azure-search-documents-11.6.0b3/azure_search_documents.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       79 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.968076 azure-search-documents-11.6.0b3/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6100 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.972076 azure-search-documents-11.6.0b3/samples/async_samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1659 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_analyze_text_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3587 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1679 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_autocomplete_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1899 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2364 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3083 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_data_source_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1797 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_facet_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1875 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_filter_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1721 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_get_document_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3501 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_alias_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1816 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_client_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4218 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_index_crud_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4321 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_indexers_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1912 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_query_session_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1800 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_search_client_send_request_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2369 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_semantic_search_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1705 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_simple_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1756 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_suggestions_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2546 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_synonym_map_operations_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7302 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/async_samples/sample_vector_search_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_analyze_text.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3361 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_authentication.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1564 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_autocomplete.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1788 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2166 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2826 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_data_source_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1672 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_facet_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1734 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_filter_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1590 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_get_document.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3275 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_alias_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1733 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_client_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_index_crud_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6067 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_indexer_datasource_skillset.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3878 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_indexers_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1792 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_query_session.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1717 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_search_client_send_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2395 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_semantic_search.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1584 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_simple_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1630 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_suggestions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2901 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_synonym_map_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7072 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/samples/sample_vector_search.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2392 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.976076 azure-search-documents-11.6.0b3/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/tests/async_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6471 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_buffered_sender_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1364 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2157 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_basic_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7227 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_buffered_sender_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6927 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_index_document_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6354 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_search_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4454 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_alias_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3921 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6323 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_data_source_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8070 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10270 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_skillset_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6112 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_synonym_map_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8040 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/async_tests/test_search_indexer_client_live_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1263 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:38:40.980076 azure-search-documents-11.6.0b3/tests/perfstress_tests/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2340 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/autocomplete.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2300 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/search_documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2305 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/perfstress_tests/suggest.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29583 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/search_service_preparer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6451 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_buffered_sender.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2164 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_index_documents_batch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3222 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_index_field_helpers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5887 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_queries.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_regex_flags.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14537 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2013 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_basic_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6790 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_buffered_sender_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6608 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_index_document_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5129 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_client_search_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5018 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4130 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_alias_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6883 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_data_source_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7627 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11708 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_skillset_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5759 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_index_client_synonym_map_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7675 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_search_indexer_client_live.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4093 2024-04-08 19:37:13.000000 azure-search-documents-11.6.0b3/tests/test_serialization.py
```

### Comparing `azure-search-documents-11.6.0b2/CHANGELOG.md` & `azure-search-documents-11.6.0b3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Release History
 
+## 11.6.0b3 (2024-04-09)
+
+### Features Added
+
+- Added `IndexerExecutionEnvironment`, `IndexingMode`, `LineEnding`, `NativeBlobSoftDeleteDeletionDetectionPolicy`, `ScalarQuantizationCompressionConfiguration`, `ScalarQuantizationParameters`, `SearchServiceCounters`, `SearchServiceLimits`, `SearchServiceStatistics`, `VectorSearchCompressionConfiguration` & `VectorSearchCompressionTargetDataType`.
+- Added `stored` in `SearchField`.
+
 ## 11.6.0b2 (2024-03-05)
 
 ### Breaking Changes
 
 - `SearchIndexerSkillset`, `SearchField`, `SearchIndex`, `AnalyzeTextOptions`, `SearchResourceEncryptionKey`, `SynonymMap`, `SearchIndexerDataSourceConnection` are no longer subclasses of `_serialization.Model`.
 
 ### Bugs Fixed
```

### Comparing `azure-search-documents-11.6.0b2/LICENSE` & `azure-search-documents-11.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/PKG-INFO` & `azure-search-documents-11.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.6.0b2
+Version: 11.6.0b3
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core<2.0.0,>=1.28.0
-Requires-Dist: azure-common~=1.1
+Requires-Dist: azure-core>=1.28.0
+Requires-Dist: azure-common>=1.1
 Requires-Dist: isodate>=0.6.0
 
 # Azure AI Search client library for Python
 
 [Azure AI Search](https://docs.microsoft.com/azure/search/) (formerly known as "Azure Cognitive Search") is an AI-powered information retrieval platform that helps developers build rich search experiences and generative AI apps that combine large language models with enterprise data.
 
 Azure AI Search is well suited for the following application scenarios:
@@ -189,15 +189,15 @@
 
 **Semantic ranking** enhances the quality of search results for text-based queries. By enabling semantic ranking on your search service, you can improve the relevance of search results in two ways:
 - It applies secondary ranking to the initial result set, promoting the most semantically relevant results to the top.
 - It extracts and returns captions and answers in the response, which can be displayed on a search page to enhance the user's search experience.
 
 To learn more about semantic ranking, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview).
 
-**Vector search** is an information retrieval technique that overcomes the limitations of traditional keyword-based search. Instead of relying solely on lexical analysis and matching individual query terms, vector search uses algorithms for similarity and concept search. It represents documents and queries as vectors in a high-dimensional space called an embedding. By searching on vector representations of content, a vector query can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
+**Vector search** is an information retrieval technique that uses numeric representations of searchable documents and query strings. By searching for numeric representations of content that are most similar to the numeric query, vector search can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
 
 To learn how to index vector fields and perform vector search, you can refer to the [sample](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/search/azure-search-documents/samples/sample_vector_search.py). This sample provides detailed guidance on indexing vector fields and demonstrates how to perform vector search.
 
 Additionally, for more comprehensive information about vector search, including its concepts and usage, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview). The documentation provides in-depth explanations and guidance on leveraging the power of vector search in Azure AI Search.
 
 _The `Azure.Search.Documents` client library (v1) provides APIs for data plane operations. The
 previous `Microsoft.Azure.Search` client library (v10) is now retired. It has many similar looking APIs, so please be careful to avoid confusion when exploring online resources. A good rule of thumb is to check for the namespace
```

### Comparing `azure-search-documents-11.6.0b2/README.md` & `azure-search-documents-11.6.0b3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 
 **Semantic ranking** enhances the quality of search results for text-based queries. By enabling semantic ranking on your search service, you can improve the relevance of search results in two ways:
 - It applies secondary ranking to the initial result set, promoting the most semantically relevant results to the top.
 - It extracts and returns captions and answers in the response, which can be displayed on a search page to enhance the user's search experience.
 
 To learn more about semantic ranking, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview).
 
-**Vector search** is an information retrieval technique that overcomes the limitations of traditional keyword-based search. Instead of relying solely on lexical analysis and matching individual query terms, vector search uses algorithms for similarity and concept search. It represents documents and queries as vectors in a high-dimensional space called an embedding. By searching on vector representations of content, a vector query can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
+**Vector search** is an information retrieval technique that uses numeric representations of searchable documents and query strings. By searching for numeric representations of content that are most similar to the numeric query, vector search can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
 
 To learn how to index vector fields and perform vector search, you can refer to the [sample](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/search/azure-search-documents/samples/sample_vector_search.py). This sample provides detailed guidance on indexing vector fields and demonstrates how to perform vector search.
 
 Additionally, for more comprehensive information about vector search, including its concepts and usage, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview). The documentation provides in-depth explanations and guidance on leveraging the power of vector search in Azure AI Search.
 
 _The `Azure.Search.Documents` client library (v1) provides APIs for data plane operations. The
 previous `Microsoft.Azure.Search` client library (v10) is now retired. It has many similar looking APIs, so please be careful to avoid confusion when exploring online resources. A good rule of thumb is to check for the namespace
```

### Comparing `azure-search-documents-11.6.0b2/TROUBLESHOOTING.md` & `azure-search-documents-11.6.0b3/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/_configuration.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/_search_index_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/_serialization.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/_vendor.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_configuration.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/_search_index_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/_documents_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_documents_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/aio/operations/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_models_py3.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_models_py3.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/models/_search_index_client_enums.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/models/_search_index_client_enums.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/_documents_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_documents_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_generated/operations/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_headers_mixin.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_headers_mixin.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_index_documents_batch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_index_documents_batch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_paging.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_paging.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_queries.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_queries.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_search_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_search_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_search_indexing_buffered_sender.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_search_indexing_buffered_sender_base.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_search_indexing_buffered_sender_base.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/_utils.py` & `azure-search-documents-11.6.0b3/azure/search/documents/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/_index_documents_batch_async.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/_index_documents_batch_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/_paging.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/_paging.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/_search_client_async.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/_search_indexing_buffered_sender_async.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/_search_indexing_buffered_sender_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/aio/_timer.py` & `azure-search-documents-11.6.0b3/azure/search/documents/aio/_timer.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_configuration.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -39,10 +39,10 @@
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_search_service_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_search_service_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_serialization.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/_vendor.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_vendor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from azure.core.pipeline.transport import HttpRequest
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_configuration.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -39,10 +39,10 @@
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_search_service_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_search_service_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/_vendor.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from azure.core.pipeline.transport import HttpRequest
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -29,36 +29,36 @@
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class SearchServiceClientOperationsMixin(SearchServiceClientMixinABC):
     @distributed_trace_async
     async def get_service_statistics(
         self, request_options: Optional[_models.RequestOptions] = None, **kwargs: Any
-    ) -> _models.ServiceStatistics:
+    ) -> _models.SearchServiceStatistics:
         """Gets service level statistics for a search service.
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
-        :return: ServiceStatistics or the result of cls(response)
-        :rtype: ~azure.search.documents.indexes.models.ServiceStatistics
+        :return: SearchServiceStatistics or the result of cls(response)
+        :rtype: ~azure.search.documents.indexes.models.SearchServiceStatistics
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ServiceStatistics] = kwargs.pop("cls", None)
+        cls: ClsType[_models.SearchServiceStatistics] = kwargs.pop("cls", None)
 
         _x_ms_client_request_id = None
         if request_options is not None:
             _x_ms_client_request_id = request_options.x_ms_client_request_id
 
         _request = build_get_service_statistics_request(
             x_ms_client_request_id=_x_ms_client_request_id,
@@ -80,13 +80,13 @@
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("ServiceStatistics", pipeline_response)
+        deserialized = self._deserialize("SearchServiceStatistics", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AnalyzeRequest
 from ._models_py3 import AnalyzeResult
 from ._models_py3 import AnalyzedTokenInfo
 from ._models_py3 import AsciiFoldingTokenFilter
 from ._models_py3 import AzureActiveDirectoryApplicationCredentials
 from ._models_py3 import AzureMachineLearningSkill
 from ._models_py3 import AzureOpenAIEmbeddingSkill
 from ._models_py3 import AzureOpenAIParameters
 from ._models_py3 import AzureOpenAIVectorizer
-from ._models_py3 import BM25Similarity
+from ._models_py3 import BM25SimilarityAlgorithm
 from ._models_py3 import CharFilter
 from ._models_py3 import CjkBigramTokenFilter
-from ._models_py3 import ClassicSimilarity
+from ._models_py3 import ClassicSimilarityAlgorithm
 from ._models_py3 import ClassicTokenizer
 from ._models_py3 import CognitiveServicesAccount
 from ._models_py3 import CognitiveServicesAccountKey
 from ._models_py3 import CommonGramTokenFilter
 from ._models_py3 import ConditionalSkill
 from ._models_py3 import CorsOptions
 from ._models_py3 import CustomAnalyzer
@@ -136,36 +136,36 @@
 from ._models_py3 import SearchIndexerKnowledgeStoreTableProjectionSelector
 from ._models_py3 import SearchIndexerLimits
 from ._models_py3 import SearchIndexerSkill
 from ._models_py3 import SearchIndexerSkillset
 from ._models_py3 import SearchIndexerStatus
 from ._models_py3 import SearchIndexerWarning
 from ._models_py3 import SearchResourceEncryptionKey
+from ._models_py3 import SearchServiceCounters
+from ._models_py3 import SearchServiceLimits
+from ._models_py3 import SearchServiceStatistics
+from ._models_py3 import SearchSuggester
 from ._models_py3 import SemanticConfiguration
 from ._models_py3 import SemanticField
 from ._models_py3 import SemanticPrioritizedFields
 from ._models_py3 import SemanticSearch
 from ._models_py3 import SentimentSkill
 from ._models_py3 import SentimentSkillV3
-from ._models_py3 import ServiceCounters
-from ._models_py3 import ServiceLimits
-from ._models_py3 import ServiceStatistics
 from ._models_py3 import ShaperSkill
 from ._models_py3 import ShingleTokenFilter
-from ._models_py3 import Similarity
+from ._models_py3 import SimilarityAlgorithm
 from ._models_py3 import SkillNames
 from ._models_py3 import SnowballTokenFilter
 from ._models_py3 import SoftDeleteColumnDeletionDetectionPolicy
 from ._models_py3 import SplitSkill
 from ._models_py3 import SqlIntegratedChangeTrackingPolicy
 from ._models_py3 import StemmerOverrideTokenFilter
 from ._models_py3 import StemmerTokenFilter
 from ._models_py3 import StopAnalyzer
 from ._models_py3 import StopwordsTokenFilter
-from ._models_py3 import Suggester
 from ._models_py3 import SynonymMap
 from ._models_py3 import SynonymTokenFilter
 from ._models_py3 import TagScoringFunction
 from ._models_py3 import TagScoringParameters
 from ._models_py3 import TextTranslationSkill
 from ._models_py3 import TextWeights
 from ._models_py3 import TokenFilter
@@ -239,18 +239,18 @@
     "AnalyzedTokenInfo",
     "AsciiFoldingTokenFilter",
     "AzureActiveDirectoryApplicationCredentials",
     "AzureMachineLearningSkill",
     "AzureOpenAIEmbeddingSkill",
     "AzureOpenAIParameters",
     "AzureOpenAIVectorizer",
-    "BM25Similarity",
+    "BM25SimilarityAlgorithm",
     "CharFilter",
     "CjkBigramTokenFilter",
-    "ClassicSimilarity",
+    "ClassicSimilarityAlgorithm",
     "ClassicTokenizer",
     "CognitiveServicesAccount",
     "CognitiveServicesAccountKey",
     "CommonGramTokenFilter",
     "ConditionalSkill",
     "CorsOptions",
     "CustomAnalyzer",
@@ -366,36 +366,36 @@
     "SearchIndexerKnowledgeStoreTableProjectionSelector",
     "SearchIndexerLimits",
     "SearchIndexerSkill",
     "SearchIndexerSkillset",
     "SearchIndexerStatus",
     "SearchIndexerWarning",
     "SearchResourceEncryptionKey",
+    "SearchServiceCounters",
+    "SearchServiceLimits",
+    "SearchServiceStatistics",
+    "SearchSuggester",
     "SemanticConfiguration",
     "SemanticField",
     "SemanticPrioritizedFields",
     "SemanticSearch",
     "SentimentSkill",
     "SentimentSkillV3",
-    "ServiceCounters",
-    "ServiceLimits",
-    "ServiceStatistics",
     "ShaperSkill",
     "ShingleTokenFilter",
-    "Similarity",
+    "SimilarityAlgorithm",
     "SkillNames",
     "SnowballTokenFilter",
     "SoftDeleteColumnDeletionDetectionPolicy",
     "SplitSkill",
     "SqlIntegratedChangeTrackingPolicy",
     "StemmerOverrideTokenFilter",
     "StemmerTokenFilter",
     "StopAnalyzer",
     "StopwordsTokenFilter",
-    "Suggester",
     "SynonymMap",
     "SynonymTokenFilter",
     "TagScoringFunction",
     "TagScoringParameters",
     "TextTranslationSkill",
     "TextWeights",
     "TokenFilter",
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_models_py3.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
@@ -818,21 +818,21 @@
          ~azure.search.documents.indexes.models.AzureOpenAIParameters
         """
         super().__init__(name=name, **kwargs)
         self.kind: str = "azureOpenAI"
         self.azure_open_ai_parameters = azure_open_ai_parameters
 
 
-class Similarity(_serialization.Model):
+class SimilarityAlgorithm(_serialization.Model):
     """Base type for similarity algorithms. Similarity algorithms are used to calculate scores that
     tie queries to documents. The higher the score, the more relevant the document is to that
     specific query. Those scores are used to rank the search results.
 
     You probably want to use the sub-classes and not this class directly. Known sub-classes are:
-    BM25Similarity, ClassicSimilarity
+    BM25SimilarityAlgorithm, ClassicSimilarityAlgorithm
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: Required.
     :vartype odata_type: str
     """
 
@@ -842,26 +842,26 @@
 
     _attribute_map = {
         "odata_type": {"key": "@odata\\.type", "type": "str"},
     }
 
     _subtype_map = {
         "odata_type": {
-            "#Microsoft.Azure.Search.BM25Similarity": "BM25Similarity",
-            "#Microsoft.Azure.Search.ClassicSimilarity": "ClassicSimilarity",
+            "#Microsoft.Azure.Search.BM25Similarity": "BM25SimilarityAlgorithm",
+            "#Microsoft.Azure.Search.ClassicSimilarity": "ClassicSimilarityAlgorithm",
         }
     }
 
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.odata_type: Optional[str] = None
 
 
-class BM25Similarity(Similarity):
+class BM25SimilarityAlgorithm(SimilarityAlgorithm):
     """Ranking function based on the Okapi BM25 similarity algorithm. BM25 is a TF-IDF-like algorithm
     that includes length normalization (controlled by the 'b' parameter) as well as term frequency
     saturation (controlled by the 'k1' parameter).
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: Required.
@@ -1002,15 +1002,15 @@
         """
         super().__init__(name=name, **kwargs)
         self.odata_type: str = "#Microsoft.Azure.Search.CjkBigramTokenFilter"
         self.ignore_scripts = ignore_scripts
         self.output_unigrams = output_unigrams
 
 
-class ClassicSimilarity(Similarity):
+class ClassicSimilarityAlgorithm(SimilarityAlgorithm):
     """Legacy similarity algorithm which uses the Lucene TFIDFSimilarity implementation of TF-IDF.
     This variation of TF-IDF introduces static document length normalization as well as
     coordinating factors that penalize documents that only partially match the searched queries.
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: Required.
@@ -5721,15 +5721,15 @@
      "ia", "iu", "ga", "it", "ja", "Jns", "jv", "kea", "kac", "xnr", "krc", "kaa-cyrl", "kaa",
      "csb", "kk-cyrl", "kk-latn", "klr", "kha", "quc", "ko", "kfq", "kpy", "kos", "kum", "ku-arab",
      "ku-latn", "kru", "ky", "lkt", "la", "lt", "dsb", "smj", "lb", "bfz", "ms", "mt", "kmj", "gv",
      "mi", "mr", "mn", "cnr-cyrl", "cnr-latn", "nap", "ne", "niu", "nog", "sme", "nb", "no", "oc",
      "os", "ps", "fa", "pl", "pt", "pa", "ksh", "ro", "rm", "ru", "sck", "sm", "sa", "sat", "sco",
      "gd", "sr", "sr-Cyrl", "sr-Latn", "xsr", "srx", "sms", "sk", "sl", "so", "sma", "es", "sw",
      "sv", "tg", "tt", "tet", "thf", "to", "tr", "tk", "tyv", "hsb", "ur", "ug", "uz-arab",
-     "uz-cyrl", "uz", "vo", "wae", "cy", "fy", "yua", "za", "zu", "unk", and "is".
+     "uz-cyrl", "uz", "vo", "wae", "cy", "fy", "yua", "za", "zu", and "unk".
     :vartype default_language_code: str or ~azure.search.documents.indexes.models.OcrSkillLanguage
     :ivar should_detect_orientation: A value indicating to turn orientation detection on or not.
      Default is false.
     :vartype should_detect_orientation: bool
     :ivar line_ending: Defines the sequence of characters to use between the lines of text
      recognized by the OCR skill. The default value is "space". Known values are: "space",
      "carriageReturn", "lineFeed", and "carriageReturnLineFeed".
@@ -5794,15 +5794,15 @@
          "smn", "id", "ia", "iu", "ga", "it", "ja", "Jns", "jv", "kea", "kac", "xnr", "krc", "kaa-cyrl",
          "kaa", "csb", "kk-cyrl", "kk-latn", "klr", "kha", "quc", "ko", "kfq", "kpy", "kos", "kum",
          "ku-arab", "ku-latn", "kru", "ky", "lkt", "la", "lt", "dsb", "smj", "lb", "bfz", "ms", "mt",
          "kmj", "gv", "mi", "mr", "mn", "cnr-cyrl", "cnr-latn", "nap", "ne", "niu", "nog", "sme", "nb",
          "no", "oc", "os", "ps", "fa", "pl", "pt", "pa", "ksh", "ro", "rm", "ru", "sck", "sm", "sa",
          "sat", "sco", "gd", "sr", "sr-Cyrl", "sr-Latn", "xsr", "srx", "sms", "sk", "sl", "so", "sma",
          "es", "sw", "sv", "tg", "tt", "tet", "thf", "to", "tr", "tk", "tyv", "hsb", "ur", "ug",
-         "uz-arab", "uz-cyrl", "uz", "vo", "wae", "cy", "fy", "yua", "za", "zu", "unk", and "is".
+         "uz-arab", "uz-cyrl", "uz", "vo", "wae", "cy", "fy", "yua", "za", "zu", and "unk".
         :paramtype default_language_code: str or
          ~azure.search.documents.indexes.models.OcrSkillLanguage
         :keyword should_detect_orientation: A value indicating to turn orientation detection on or not.
          Default is false.
         :paramtype should_detect_orientation: bool
         :keyword line_ending: Defines the sequence of characters to use between the lines of text
          recognized by the OCR skill. The default value is "space". Known values are: "space",
@@ -7140,15 +7140,15 @@
     :ivar default_scoring_profile: The name of the scoring profile to use if none is specified in
      the query. If this property is not set and no scoring profile is specified in the query, then
      default scoring (tf-idf) will be used.
     :vartype default_scoring_profile: str
     :ivar cors_options: Options to control Cross-Origin Resource Sharing (CORS) for the index.
     :vartype cors_options: ~azure.search.documents.indexes.models.CorsOptions
     :ivar suggesters: The suggesters for the index.
-    :vartype suggesters: list[~azure.search.documents.indexes.models.Suggester]
+    :vartype suggesters: list[~azure.search.documents.indexes.models.SearchSuggester]
     :ivar analyzers: The analyzers for the index.
     :vartype analyzers: list[~azure.search.documents.indexes.models.LexicalAnalyzer]
     :ivar tokenizers: The tokenizers for the index.
     :vartype tokenizers: list[~azure.search.documents.indexes.models.LexicalTokenizer]
     :ivar token_filters: The token filters for the index.
     :vartype token_filters: list[~azure.search.documents.indexes.models.TokenFilter]
     :ivar char_filters: The character filters for the index.
@@ -7164,15 +7164,15 @@
      available for free search services, and is only available for paid services created on or after
      January 1, 2019.
     :vartype encryption_key: ~azure.search.documents.indexes.models.SearchResourceEncryptionKey
     :ivar similarity: The type of similarity algorithm to be used when scoring and ranking the
      documents matching a search query. The similarity algorithm can only be defined at index
      creation time and cannot be modified on existing indexes. If null, the ClassicSimilarity
      algorithm is used.
-    :vartype similarity: ~azure.search.documents.indexes.models.Similarity
+    :vartype similarity: ~azure.search.documents.indexes.models.SimilarityAlgorithm
     :ivar semantic_search: Defines parameters for a search index that influence semantic
      capabilities.
     :vartype semantic_search: ~azure.search.documents.indexes.models.SemanticSearch
     :ivar vector_search: Contains configuration options related to vector search.
     :vartype vector_search: ~azure.search.documents.indexes.models.VectorSearch
     :ivar e_tag: The ETag of the index.
     :vartype e_tag: str
@@ -7185,43 +7185,43 @@
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "fields": {"key": "fields", "type": "[SearchField]"},
         "scoring_profiles": {"key": "scoringProfiles", "type": "[ScoringProfile]"},
         "default_scoring_profile": {"key": "defaultScoringProfile", "type": "str"},
         "cors_options": {"key": "corsOptions", "type": "CorsOptions"},
-        "suggesters": {"key": "suggesters", "type": "[Suggester]"},
+        "suggesters": {"key": "suggesters", "type": "[SearchSuggester]"},
         "analyzers": {"key": "analyzers", "type": "[LexicalAnalyzer]"},
         "tokenizers": {"key": "tokenizers", "type": "[LexicalTokenizer]"},
         "token_filters": {"key": "tokenFilters", "type": "[TokenFilter]"},
         "char_filters": {"key": "charFilters", "type": "[CharFilter]"},
         "normalizers": {"key": "normalizers", "type": "[LexicalNormalizer]"},
         "encryption_key": {"key": "encryptionKey", "type": "SearchResourceEncryptionKey"},
-        "similarity": {"key": "similarity", "type": "Similarity"},
+        "similarity": {"key": "similarity", "type": "SimilarityAlgorithm"},
         "semantic_search": {"key": "semantic", "type": "SemanticSearch"},
         "vector_search": {"key": "vectorSearch", "type": "VectorSearch"},
         "e_tag": {"key": "@odata\\.etag", "type": "str"},
     }
 
     def __init__(
         self,
         *,
         name: str,
         fields: List["_models.SearchField"],
         scoring_profiles: Optional[List["_models.ScoringProfile"]] = None,
         default_scoring_profile: Optional[str] = None,
         cors_options: Optional["_models.CorsOptions"] = None,
-        suggesters: Optional[List["_models.Suggester"]] = None,
+        suggesters: Optional[List["_models.SearchSuggester"]] = None,
         analyzers: Optional[List["_models.LexicalAnalyzer"]] = None,
         tokenizers: Optional[List["_models.LexicalTokenizer"]] = None,
         token_filters: Optional[List["_models.TokenFilter"]] = None,
         char_filters: Optional[List["_models.CharFilter"]] = None,
         normalizers: Optional[List["_models.LexicalNormalizer"]] = None,
         encryption_key: Optional["_models.SearchResourceEncryptionKey"] = None,
-        similarity: Optional["_models.Similarity"] = None,
+        similarity: Optional["_models.SimilarityAlgorithm"] = None,
         semantic_search: Optional["_models.SemanticSearch"] = None,
         vector_search: Optional["_models.VectorSearch"] = None,
         e_tag: Optional[str] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword name: The name of the index. Required.
@@ -7233,15 +7233,15 @@
         :keyword default_scoring_profile: The name of the scoring profile to use if none is specified
          in the query. If this property is not set and no scoring profile is specified in the query,
          then default scoring (tf-idf) will be used.
         :paramtype default_scoring_profile: str
         :keyword cors_options: Options to control Cross-Origin Resource Sharing (CORS) for the index.
         :paramtype cors_options: ~azure.search.documents.indexes.models.CorsOptions
         :keyword suggesters: The suggesters for the index.
-        :paramtype suggesters: list[~azure.search.documents.indexes.models.Suggester]
+        :paramtype suggesters: list[~azure.search.documents.indexes.models.SearchSuggester]
         :keyword analyzers: The analyzers for the index.
         :paramtype analyzers: list[~azure.search.documents.indexes.models.LexicalAnalyzer]
         :keyword tokenizers: The tokenizers for the index.
         :paramtype tokenizers: list[~azure.search.documents.indexes.models.LexicalTokenizer]
         :keyword token_filters: The token filters for the index.
         :paramtype token_filters: list[~azure.search.documents.indexes.models.TokenFilter]
         :keyword char_filters: The character filters for the index.
@@ -7257,15 +7257,15 @@
          available for free search services, and is only available for paid services created on or after
          January 1, 2019.
         :paramtype encryption_key: ~azure.search.documents.indexes.models.SearchResourceEncryptionKey
         :keyword similarity: The type of similarity algorithm to be used when scoring and ranking the
          documents matching a search query. The similarity algorithm can only be defined at index
          creation time and cannot be modified on existing indexes. If null, the ClassicSimilarity
          algorithm is used.
-        :paramtype similarity: ~azure.search.documents.indexes.models.Similarity
+        :paramtype similarity: ~azure.search.documents.indexes.models.SimilarityAlgorithm
         :keyword semantic_search: Defines parameters for a search index that influence semantic
          capabilities.
         :paramtype semantic_search: ~azure.search.documents.indexes.models.SemanticSearch
         :keyword vector_search: Contains configuration options related to vector search.
         :paramtype vector_search: ~azure.search.documents.indexes.models.VectorSearch
         :keyword e_tag: The ETag of the index.
         :paramtype e_tag: str
@@ -8630,14 +8630,247 @@
         self.key_name = key_name
         self.key_version = key_version
         self.vault_uri = vault_uri
         self.access_credentials = access_credentials
         self.identity = identity
 
 
+class SearchServiceCounters(_serialization.Model):
+    """Represents service-level resource counters and quotas.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar alias_counter: Total number of aliases. Required.
+    :vartype alias_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar document_counter: Total number of documents across all indexes in the service. Required.
+    :vartype document_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar index_counter: Total number of indexes. Required.
+    :vartype index_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar indexer_counter: Total number of indexers. Required.
+    :vartype indexer_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar data_source_counter: Total number of data sources. Required.
+    :vartype data_source_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar storage_size_counter: Total size of used storage in bytes. Required.
+    :vartype storage_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar synonym_map_counter: Total number of synonym maps. Required.
+    :vartype synonym_map_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar skillset_counter: Total number of skillsets. Required.
+    :vartype skillset_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    :ivar vector_index_size_counter: Total memory consumption of all vector indexes within the
+     service, in bytes. Required.
+    :vartype vector_index_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
+    """
+
+    _validation = {
+        "alias_counter": {"required": True},
+        "document_counter": {"required": True},
+        "index_counter": {"required": True},
+        "indexer_counter": {"required": True},
+        "data_source_counter": {"required": True},
+        "storage_size_counter": {"required": True},
+        "synonym_map_counter": {"required": True},
+        "skillset_counter": {"required": True},
+        "vector_index_size_counter": {"required": True},
+    }
+
+    _attribute_map = {
+        "alias_counter": {"key": "aliasesCount", "type": "ResourceCounter"},
+        "document_counter": {"key": "documentCount", "type": "ResourceCounter"},
+        "index_counter": {"key": "indexesCount", "type": "ResourceCounter"},
+        "indexer_counter": {"key": "indexersCount", "type": "ResourceCounter"},
+        "data_source_counter": {"key": "dataSourcesCount", "type": "ResourceCounter"},
+        "storage_size_counter": {"key": "storageSize", "type": "ResourceCounter"},
+        "synonym_map_counter": {"key": "synonymMaps", "type": "ResourceCounter"},
+        "skillset_counter": {"key": "skillsetCount", "type": "ResourceCounter"},
+        "vector_index_size_counter": {"key": "vectorIndexSize", "type": "ResourceCounter"},
+    }
+
+    def __init__(
+        self,
+        *,
+        alias_counter: "_models.ResourceCounter",
+        document_counter: "_models.ResourceCounter",
+        index_counter: "_models.ResourceCounter",
+        indexer_counter: "_models.ResourceCounter",
+        data_source_counter: "_models.ResourceCounter",
+        storage_size_counter: "_models.ResourceCounter",
+        synonym_map_counter: "_models.ResourceCounter",
+        skillset_counter: "_models.ResourceCounter",
+        vector_index_size_counter: "_models.ResourceCounter",
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword alias_counter: Total number of aliases. Required.
+        :paramtype alias_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword document_counter: Total number of documents across all indexes in the service.
+         Required.
+        :paramtype document_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword index_counter: Total number of indexes. Required.
+        :paramtype index_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword indexer_counter: Total number of indexers. Required.
+        :paramtype indexer_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword data_source_counter: Total number of data sources. Required.
+        :paramtype data_source_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword storage_size_counter: Total size of used storage in bytes. Required.
+        :paramtype storage_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword synonym_map_counter: Total number of synonym maps. Required.
+        :paramtype synonym_map_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword skillset_counter: Total number of skillsets. Required.
+        :paramtype skillset_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        :keyword vector_index_size_counter: Total memory consumption of all vector indexes within the
+         service, in bytes. Required.
+        :paramtype vector_index_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
+        """
+        super().__init__(**kwargs)
+        self.alias_counter = alias_counter
+        self.document_counter = document_counter
+        self.index_counter = index_counter
+        self.indexer_counter = indexer_counter
+        self.data_source_counter = data_source_counter
+        self.storage_size_counter = storage_size_counter
+        self.synonym_map_counter = synonym_map_counter
+        self.skillset_counter = skillset_counter
+        self.vector_index_size_counter = vector_index_size_counter
+
+
+class SearchServiceLimits(_serialization.Model):
+    """Represents various service level limits.
+
+    :ivar max_fields_per_index: The maximum allowed fields per index.
+    :vartype max_fields_per_index: int
+    :ivar max_field_nesting_depth_per_index: The maximum depth which you can nest sub-fields in an
+     index, including the top-level complex field. For example, a/b/c has a nesting depth of 3.
+    :vartype max_field_nesting_depth_per_index: int
+    :ivar max_complex_collection_fields_per_index: The maximum number of fields of type
+     Collection(Edm.ComplexType) allowed in an index.
+    :vartype max_complex_collection_fields_per_index: int
+    :ivar max_complex_objects_in_collections_per_document: The maximum number of objects in complex
+     collections allowed per document.
+    :vartype max_complex_objects_in_collections_per_document: int
+    """
+
+    _attribute_map = {
+        "max_fields_per_index": {"key": "maxFieldsPerIndex", "type": "int"},
+        "max_field_nesting_depth_per_index": {"key": "maxFieldNestingDepthPerIndex", "type": "int"},
+        "max_complex_collection_fields_per_index": {"key": "maxComplexCollectionFieldsPerIndex", "type": "int"},
+        "max_complex_objects_in_collections_per_document": {
+            "key": "maxComplexObjectsInCollectionsPerDocument",
+            "type": "int",
+        },
+    }
+
+    def __init__(
+        self,
+        *,
+        max_fields_per_index: Optional[int] = None,
+        max_field_nesting_depth_per_index: Optional[int] = None,
+        max_complex_collection_fields_per_index: Optional[int] = None,
+        max_complex_objects_in_collections_per_document: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword max_fields_per_index: The maximum allowed fields per index.
+        :paramtype max_fields_per_index: int
+        :keyword max_field_nesting_depth_per_index: The maximum depth which you can nest sub-fields in
+         an index, including the top-level complex field. For example, a/b/c has a nesting depth of 3.
+        :paramtype max_field_nesting_depth_per_index: int
+        :keyword max_complex_collection_fields_per_index: The maximum number of fields of type
+         Collection(Edm.ComplexType) allowed in an index.
+        :paramtype max_complex_collection_fields_per_index: int
+        :keyword max_complex_objects_in_collections_per_document: The maximum number of objects in
+         complex collections allowed per document.
+        :paramtype max_complex_objects_in_collections_per_document: int
+        """
+        super().__init__(**kwargs)
+        self.max_fields_per_index = max_fields_per_index
+        self.max_field_nesting_depth_per_index = max_field_nesting_depth_per_index
+        self.max_complex_collection_fields_per_index = max_complex_collection_fields_per_index
+        self.max_complex_objects_in_collections_per_document = max_complex_objects_in_collections_per_document
+
+
+class SearchServiceStatistics(_serialization.Model):
+    """Response from a get service statistics request. If successful, it includes service level
+    counters and limits.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar counters: Service level resource counters. Required.
+    :vartype counters: ~azure.search.documents.indexes.models.SearchServiceCounters
+    :ivar limits: Service level general limits. Required.
+    :vartype limits: ~azure.search.documents.indexes.models.SearchServiceLimits
+    """
+
+    _validation = {
+        "counters": {"required": True},
+        "limits": {"required": True},
+    }
+
+    _attribute_map = {
+        "counters": {"key": "counters", "type": "SearchServiceCounters"},
+        "limits": {"key": "limits", "type": "SearchServiceLimits"},
+    }
+
+    def __init__(
+        self, *, counters: "_models.SearchServiceCounters", limits: "_models.SearchServiceLimits", **kwargs: Any
+    ) -> None:
+        """
+        :keyword counters: Service level resource counters. Required.
+        :paramtype counters: ~azure.search.documents.indexes.models.SearchServiceCounters
+        :keyword limits: Service level general limits. Required.
+        :paramtype limits: ~azure.search.documents.indexes.models.SearchServiceLimits
+        """
+        super().__init__(**kwargs)
+        self.counters = counters
+        self.limits = limits
+
+
+class SearchSuggester(_serialization.Model):
+    """Defines how the Suggest API should apply to a group of fields in the index.
+
+    Variables are only populated by the server, and will be ignored when sending a request.
+
+    All required parameters must be populated in order to send to server.
+
+    :ivar name: The name of the suggester. Required.
+    :vartype name: str
+    :ivar search_mode: A value indicating the capabilities of the suggester. Required. Default
+     value is "analyzingInfixMatching".
+    :vartype search_mode: str
+    :ivar source_fields: The list of field names to which the suggester applies. Each field must be
+     searchable. Required.
+    :vartype source_fields: list[str]
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "search_mode": {"required": True, "constant": True},
+        "source_fields": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "search_mode": {"key": "searchMode", "type": "str"},
+        "source_fields": {"key": "sourceFields", "type": "[str]"},
+    }
+
+    search_mode = "analyzingInfixMatching"
+
+    def __init__(self, *, name: str, source_fields: List[str], **kwargs: Any) -> None:
+        """
+        :keyword name: The name of the suggester. Required.
+        :paramtype name: str
+        :keyword source_fields: The list of field names to which the suggester applies. Each field must
+         be searchable. Required.
+        :paramtype source_fields: list[str]
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.source_fields = source_fields
+
+
 class SemanticConfiguration(_serialization.Model):
     """Defines a specific configuration to be used in the context of semantic capabilities.
 
     All required parameters must be populated in order to send to server.
 
     :ivar name: The name of the semantic configuration. Required.
     :vartype name: str
@@ -8972,201 +9205,14 @@
         super().__init__(name=name, description=description, context=context, inputs=inputs, outputs=outputs, **kwargs)
         self.odata_type: str = "#Microsoft.Skills.Text.V3.SentimentSkill"
         self.default_language_code = default_language_code
         self.include_opinion_mining = include_opinion_mining
         self.model_version = model_version
 
 
-class ServiceCounters(_serialization.Model):
-    """Represents service-level resource counters and quotas.
-
-    All required parameters must be populated in order to send to server.
-
-    :ivar alias_counter: Total number of aliases. Required.
-    :vartype alias_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar document_counter: Total number of documents across all indexes in the service. Required.
-    :vartype document_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar index_counter: Total number of indexes. Required.
-    :vartype index_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar indexer_counter: Total number of indexers. Required.
-    :vartype indexer_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar data_source_counter: Total number of data sources. Required.
-    :vartype data_source_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar storage_size_counter: Total size of used storage in bytes. Required.
-    :vartype storage_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar synonym_map_counter: Total number of synonym maps. Required.
-    :vartype synonym_map_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar skillset_counter: Total number of skillsets. Required.
-    :vartype skillset_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    :ivar vector_index_size_counter: Total memory consumption of all vector indexes within the
-     service, in bytes. Required.
-    :vartype vector_index_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
-    """
-
-    _validation = {
-        "alias_counter": {"required": True},
-        "document_counter": {"required": True},
-        "index_counter": {"required": True},
-        "indexer_counter": {"required": True},
-        "data_source_counter": {"required": True},
-        "storage_size_counter": {"required": True},
-        "synonym_map_counter": {"required": True},
-        "skillset_counter": {"required": True},
-        "vector_index_size_counter": {"required": True},
-    }
-
-    _attribute_map = {
-        "alias_counter": {"key": "aliasesCount", "type": "ResourceCounter"},
-        "document_counter": {"key": "documentCount", "type": "ResourceCounter"},
-        "index_counter": {"key": "indexesCount", "type": "ResourceCounter"},
-        "indexer_counter": {"key": "indexersCount", "type": "ResourceCounter"},
-        "data_source_counter": {"key": "dataSourcesCount", "type": "ResourceCounter"},
-        "storage_size_counter": {"key": "storageSize", "type": "ResourceCounter"},
-        "synonym_map_counter": {"key": "synonymMaps", "type": "ResourceCounter"},
-        "skillset_counter": {"key": "skillsetCount", "type": "ResourceCounter"},
-        "vector_index_size_counter": {"key": "vectorIndexSize", "type": "ResourceCounter"},
-    }
-
-    def __init__(
-        self,
-        *,
-        alias_counter: "_models.ResourceCounter",
-        document_counter: "_models.ResourceCounter",
-        index_counter: "_models.ResourceCounter",
-        indexer_counter: "_models.ResourceCounter",
-        data_source_counter: "_models.ResourceCounter",
-        storage_size_counter: "_models.ResourceCounter",
-        synonym_map_counter: "_models.ResourceCounter",
-        skillset_counter: "_models.ResourceCounter",
-        vector_index_size_counter: "_models.ResourceCounter",
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword alias_counter: Total number of aliases. Required.
-        :paramtype alias_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword document_counter: Total number of documents across all indexes in the service.
-         Required.
-        :paramtype document_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword index_counter: Total number of indexes. Required.
-        :paramtype index_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword indexer_counter: Total number of indexers. Required.
-        :paramtype indexer_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword data_source_counter: Total number of data sources. Required.
-        :paramtype data_source_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword storage_size_counter: Total size of used storage in bytes. Required.
-        :paramtype storage_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword synonym_map_counter: Total number of synonym maps. Required.
-        :paramtype synonym_map_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword skillset_counter: Total number of skillsets. Required.
-        :paramtype skillset_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        :keyword vector_index_size_counter: Total memory consumption of all vector indexes within the
-         service, in bytes. Required.
-        :paramtype vector_index_size_counter: ~azure.search.documents.indexes.models.ResourceCounter
-        """
-        super().__init__(**kwargs)
-        self.alias_counter = alias_counter
-        self.document_counter = document_counter
-        self.index_counter = index_counter
-        self.indexer_counter = indexer_counter
-        self.data_source_counter = data_source_counter
-        self.storage_size_counter = storage_size_counter
-        self.synonym_map_counter = synonym_map_counter
-        self.skillset_counter = skillset_counter
-        self.vector_index_size_counter = vector_index_size_counter
-
-
-class ServiceLimits(_serialization.Model):
-    """Represents various service level limits.
-
-    :ivar max_fields_per_index: The maximum allowed fields per index.
-    :vartype max_fields_per_index: int
-    :ivar max_field_nesting_depth_per_index: The maximum depth which you can nest sub-fields in an
-     index, including the top-level complex field. For example, a/b/c has a nesting depth of 3.
-    :vartype max_field_nesting_depth_per_index: int
-    :ivar max_complex_collection_fields_per_index: The maximum number of fields of type
-     Collection(Edm.ComplexType) allowed in an index.
-    :vartype max_complex_collection_fields_per_index: int
-    :ivar max_complex_objects_in_collections_per_document: The maximum number of objects in complex
-     collections allowed per document.
-    :vartype max_complex_objects_in_collections_per_document: int
-    """
-
-    _attribute_map = {
-        "max_fields_per_index": {"key": "maxFieldsPerIndex", "type": "int"},
-        "max_field_nesting_depth_per_index": {"key": "maxFieldNestingDepthPerIndex", "type": "int"},
-        "max_complex_collection_fields_per_index": {"key": "maxComplexCollectionFieldsPerIndex", "type": "int"},
-        "max_complex_objects_in_collections_per_document": {
-            "key": "maxComplexObjectsInCollectionsPerDocument",
-            "type": "int",
-        },
-    }
-
-    def __init__(
-        self,
-        *,
-        max_fields_per_index: Optional[int] = None,
-        max_field_nesting_depth_per_index: Optional[int] = None,
-        max_complex_collection_fields_per_index: Optional[int] = None,
-        max_complex_objects_in_collections_per_document: Optional[int] = None,
-        **kwargs: Any
-    ) -> None:
-        """
-        :keyword max_fields_per_index: The maximum allowed fields per index.
-        :paramtype max_fields_per_index: int
-        :keyword max_field_nesting_depth_per_index: The maximum depth which you can nest sub-fields in
-         an index, including the top-level complex field. For example, a/b/c has a nesting depth of 3.
-        :paramtype max_field_nesting_depth_per_index: int
-        :keyword max_complex_collection_fields_per_index: The maximum number of fields of type
-         Collection(Edm.ComplexType) allowed in an index.
-        :paramtype max_complex_collection_fields_per_index: int
-        :keyword max_complex_objects_in_collections_per_document: The maximum number of objects in
-         complex collections allowed per document.
-        :paramtype max_complex_objects_in_collections_per_document: int
-        """
-        super().__init__(**kwargs)
-        self.max_fields_per_index = max_fields_per_index
-        self.max_field_nesting_depth_per_index = max_field_nesting_depth_per_index
-        self.max_complex_collection_fields_per_index = max_complex_collection_fields_per_index
-        self.max_complex_objects_in_collections_per_document = max_complex_objects_in_collections_per_document
-
-
-class ServiceStatistics(_serialization.Model):
-    """Response from a get service statistics request. If successful, it includes service level
-    counters and limits.
-
-    All required parameters must be populated in order to send to server.
-
-    :ivar counters: Service level resource counters. Required.
-    :vartype counters: ~azure.search.documents.indexes.models.ServiceCounters
-    :ivar limits: Service level general limits. Required.
-    :vartype limits: ~azure.search.documents.indexes.models.ServiceLimits
-    """
-
-    _validation = {
-        "counters": {"required": True},
-        "limits": {"required": True},
-    }
-
-    _attribute_map = {
-        "counters": {"key": "counters", "type": "ServiceCounters"},
-        "limits": {"key": "limits", "type": "ServiceLimits"},
-    }
-
-    def __init__(self, *, counters: "_models.ServiceCounters", limits: "_models.ServiceLimits", **kwargs: Any) -> None:
-        """
-        :keyword counters: Service level resource counters. Required.
-        :paramtype counters: ~azure.search.documents.indexes.models.ServiceCounters
-        :keyword limits: Service level general limits. Required.
-        :paramtype limits: ~azure.search.documents.indexes.models.ServiceLimits
-        """
-        super().__init__(**kwargs)
-        self.counters = counters
-        self.limits = limits
-
-
 class ShaperSkill(SearchIndexerSkill):
     """A skill for reshaping the outputs. It creates a complex type to support composite fields (also
     known as multipart fields).
 
     All required parameters must be populated in order to send to server.
 
     :ivar odata_type: A URI fragment specifying the type of skill. Required.
@@ -9470,15 +9516,15 @@
     :vartype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
     :ivar outputs: The output of a skill is either a field in a search index, or a value that can
      be consumed as an input by another skill. Required.
     :vartype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
     :ivar default_language_code: A value indicating which language code to use. Default is ``en``.
      Known values are: "am", "bs", "cs", "da", "de", "en", "es", "et", "fi", "fr", "he", "hi", "hr",
      "hu", "id", "is", "it", "ja", "ko", "lv", "nb", "nl", "pl", "pt", "pt-br", "ru", "sk", "sl",
-     "sr", "sv", "tr", "ur", "zh", and "is".
+     "sr", "sv", "tr", "ur", and "zh".
     :vartype default_language_code: str or
      ~azure.search.documents.indexes.models.SplitSkillLanguage
     :ivar text_split_mode: A value indicating which split mode to perform. Known values are:
      "pages" and "sentences".
     :vartype text_split_mode: str or ~azure.search.documents.indexes.models.TextSplitMode
     :ivar maximum_page_length: The desired maximum page length. Default is 10000.
     :vartype maximum_page_length: int
@@ -9544,15 +9590,15 @@
         :paramtype inputs: list[~azure.search.documents.indexes.models.InputFieldMappingEntry]
         :keyword outputs: The output of a skill is either a field in a search index, or a value that
          can be consumed as an input by another skill. Required.
         :paramtype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
         :keyword default_language_code: A value indicating which language code to use. Default is
          ``en``. Known values are: "am", "bs", "cs", "da", "de", "en", "es", "et", "fi", "fr", "he",
          "hi", "hr", "hu", "id", "is", "it", "ja", "ko", "lv", "nb", "nl", "pl", "pt", "pt-br", "ru",
-         "sk", "sl", "sr", "sv", "tr", "ur", "zh", and "is".
+         "sk", "sl", "sr", "sv", "tr", "ur", and "zh".
         :paramtype default_language_code: str or
          ~azure.search.documents.indexes.models.SplitSkillLanguage
         :keyword text_split_mode: A value indicating which split mode to perform. Known values are:
          "pages" and "sentences".
         :paramtype text_split_mode: str or ~azure.search.documents.indexes.models.TextSplitMode
         :keyword maximum_page_length: The desired maximum page length. Default is 10000.
         :paramtype maximum_page_length: int
@@ -9822,58 +9868,14 @@
         self.odata_type: str = "#Microsoft.Azure.Search.StopwordsTokenFilter"
         self.stopwords = stopwords
         self.stopwords_list = stopwords_list
         self.ignore_case = ignore_case
         self.remove_trailing_stop_words = remove_trailing_stop_words
 
 
-class Suggester(_serialization.Model):
-    """Defines how the Suggest API should apply to a group of fields in the index.
-
-    Variables are only populated by the server, and will be ignored when sending a request.
-
-    All required parameters must be populated in order to send to server.
-
-    :ivar name: The name of the suggester. Required.
-    :vartype name: str
-    :ivar search_mode: A value indicating the capabilities of the suggester. Required. Default
-     value is "analyzingInfixMatching".
-    :vartype search_mode: str
-    :ivar source_fields: The list of field names to which the suggester applies. Each field must be
-     searchable. Required.
-    :vartype source_fields: list[str]
-    """
-
-    _validation = {
-        "name": {"required": True},
-        "search_mode": {"required": True, "constant": True},
-        "source_fields": {"required": True},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "search_mode": {"key": "searchMode", "type": "str"},
-        "source_fields": {"key": "sourceFields", "type": "[str]"},
-    }
-
-    search_mode = "analyzingInfixMatching"
-
-    def __init__(self, *, name: str, source_fields: List[str], **kwargs: Any) -> None:
-        """
-        :keyword name: The name of the suggester. Required.
-        :paramtype name: str
-        :keyword source_fields: The list of field names to which the suggester applies. Each field must
-         be searchable. Required.
-        :paramtype source_fields: list[str]
-        """
-        super().__init__(**kwargs)
-        self.name = name
-        self.source_fields = source_fields
-
-
 class SynonymMap(_serialization.Model):
     """Represents a synonym map definition.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
     All required parameters must be populated in order to send to server.
 
@@ -10145,35 +10147,34 @@
     :vartype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
     :ivar default_to_language_code: The language code to translate documents into for documents
      that don't specify the to language explicitly. Required. Known values are: "af", "ar", "bn",
      "bs", "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj", "fil",
      "fi", "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw", "tlh",
      "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt", "pt-br",
      "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty", "ta",
-     "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and "is".
+     "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
     :vartype default_to_language_code: str or
      ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
     :ivar default_from_language_code: The language code to translate documents from for documents
      that don't specify the from language explicitly. Known values are: "af", "ar", "bn", "bs",
      "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj", "fil", "fi",
      "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw", "tlh",
      "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt", "pt-br",
      "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty", "ta",
-     "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and "is".
+     "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
     :vartype default_from_language_code: str or
      ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
     :ivar suggested_from: The language code to translate documents from when neither the
      fromLanguageCode input nor the defaultFromLanguageCode parameter are provided, and the
      automatic language detection is unsuccessful. Default is ``en``. Known values are: "af", "ar",
      "bn", "bs", "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj",
      "fil", "fi", "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw",
      "tlh", "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt",
      "pt-br", "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty",
-     "ta", "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and
-     "is".
+     "ta", "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
     :vartype suggested_from: str or
      ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
     """
 
     _validation = {
         "odata_type": {"required": True},
         "inputs": {"required": True},
@@ -10226,35 +10227,34 @@
         :paramtype outputs: list[~azure.search.documents.indexes.models.OutputFieldMappingEntry]
         :keyword default_to_language_code: The language code to translate documents into for documents
          that don't specify the to language explicitly. Required. Known values are: "af", "ar", "bn",
          "bs", "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj", "fil",
          "fi", "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw", "tlh",
          "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt", "pt-br",
          "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty", "ta",
-         "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and "is".
+         "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
         :paramtype default_to_language_code: str or
          ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
         :keyword default_from_language_code: The language code to translate documents from for
          documents that don't specify the from language explicitly. Known values are: "af", "ar", "bn",
          "bs", "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj", "fil",
          "fi", "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw", "tlh",
          "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt", "pt-br",
          "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty", "ta",
-         "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and "is".
+         "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
         :paramtype default_from_language_code: str or
          ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
         :keyword suggested_from: The language code to translate documents from when neither the
          fromLanguageCode input nor the defaultFromLanguageCode parameter are provided, and the
          automatic language detection is unsuccessful. Default is ``en``. Known values are: "af", "ar",
          "bn", "bs", "bg", "yue", "ca", "zh-Hans", "zh-Hant", "hr", "cs", "da", "nl", "en", "et", "fj",
          "fil", "fi", "fr", "de", "el", "ht", "he", "hi", "mww", "hu", "is", "id", "it", "ja", "sw",
          "tlh", "tlh-Latn", "tlh-Piqd", "ko", "lv", "lt", "mg", "ms", "mt", "nb", "fa", "pl", "pt",
          "pt-br", "pt-PT", "otq", "ro", "ru", "sm", "sr-Cyrl", "sr-Latn", "sk", "sl", "es", "sv", "ty",
-         "ta", "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", "pa", and
-         "is".
+         "ta", "te", "th", "to", "tr", "uk", "ur", "vi", "cy", "yua", "ga", "kn", "mi", "ml", and "pa".
         :paramtype suggested_from: str or
          ~azure.search.documents.indexes.models.TextTranslationSkillLanguage
         """
         super().__init__(name=name, description=description, context=context, inputs=inputs, outputs=outputs, **kwargs)
         self.odata_type: str = "#Microsoft.Skills.Text.TranslationSkill"
         self.default_to_language_code = default_to_language_code
         self.default_from_language_code = default_from_language_code
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
@@ -1013,15 +1013,15 @@
     """Hindi"""
     MWW = "mww"
     """Hmong Daw (Latin)"""
     HOC = "hoc"
     """Ho (Devanagiri)"""
     HU = "hu"
     """Hungarian"""
-    IS = "is"
+    IS_ENUM = "is"
     """Icelandic"""
     SMN = "smn"
     """Inari Sami"""
     ID = "id"
     """Indonesian"""
     IA = "ia"
     """Interlingua"""
@@ -1225,16 +1225,14 @@
     """Yucatec Maya"""
     ZA = "za"
     """Zhuang"""
     ZU = "zu"
     """Zulu"""
     UNK = "unk"
     """Unknown (All)"""
-    IS_ENUM = "is"
-    """Icelandic"""
 
 
 class PhoneticEncoder(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Identifies the type of phonetic encoder to use with a PhoneticTokenFilter."""
 
     METAPHONE = "metaphone"
     """Encodes a token into a Metaphone value."""
@@ -1498,15 +1496,15 @@
     """Hindi"""
     HR = "hr"
     """Croatian"""
     HU = "hu"
     """Hungarian"""
     ID = "id"
     """Indonesian"""
-    IS = "is"
+    IS_ENUM = "is"
     """Icelandic"""
     IT = "it"
     """Italian"""
     JA = "ja"
     """Japanese"""
     KO = "ko"
     """Korean"""
@@ -1534,16 +1532,14 @@
     """Swedish"""
     TR = "tr"
     """Turkish"""
     UR = "ur"
     """Urdu"""
     ZH = "zh"
     """Chinese (Simplified)"""
-    IS_ENUM = "is"
-    """Icelandic"""
 
 
 class StemmerTokenFilterLanguage(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """The language to use for a stemmer token filter."""
 
     ARABIC = "arabic"
     """Selects the Lucene stemming tokenizer for Arabic."""
@@ -1783,15 +1779,15 @@
     """Hebrew"""
     HI = "hi"
     """Hindi"""
     MWW = "mww"
     """Hmong Daw"""
     HU = "hu"
     """Hungarian"""
-    IS = "is"
+    IS_ENUM = "is"
     """Icelandic"""
     ID = "id"
     """Indonesian"""
     IT = "it"
     """Italian"""
     JA = "ja"
     """Japanese"""
@@ -1875,16 +1871,14 @@
     """Kannada"""
     MI = "mi"
     """Maori"""
     ML = "ml"
     """Malayalam"""
     PA = "pa"
     """Punjabi"""
-    IS_ENUM = "is"
-    """Icelandic"""
 
 
 class TokenCharacterKind(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Represents classes of characters on which a token filter can operate."""
 
     LETTER = "letter"
     """Keeps letters in tokens."""
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_aliases_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_aliases_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_indexers_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexers_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_indexes_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_indexes_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_patch.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -52,36 +52,36 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 class SearchServiceClientOperationsMixin(SearchServiceClientMixinABC):
     @distributed_trace
     def get_service_statistics(
         self, request_options: Optional[_models.RequestOptions] = None, **kwargs: Any
-    ) -> _models.ServiceStatistics:
+    ) -> _models.SearchServiceStatistics:
         """Gets service level statistics for a search service.
 
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~azure.search.documents.indexes.models.RequestOptions
-        :return: ServiceStatistics or the result of cls(response)
-        :rtype: ~azure.search.documents.indexes.models.ServiceStatistics
+        :return: SearchServiceStatistics or the result of cls(response)
+        :rtype: ~azure.search.documents.indexes.models.SearchServiceStatistics
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ServiceStatistics] = kwargs.pop("cls", None)
+        cls: ClsType[_models.SearchServiceStatistics] = kwargs.pop("cls", None)
 
         _x_ms_client_request_id = None
         if request_options is not None:
             _x_ms_client_request_id = request_options.x_ms_client_request_id
 
         _request = build_get_service_statistics_request(
             x_ms_client_request_id=_x_ms_client_request_id,
@@ -103,13 +103,13 @@
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.ErrorResponse, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("ServiceStatistics", pipeline_response)
+        deserialized = self._deserialize("SearchServiceStatistics", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.1, generator: @autorest/python@6.13.8)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_search_index_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_search_indexer_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_search_indexer_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/_utils.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/_search_index_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/aio/_search_indexer_client.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/aio/_search_indexer_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,20 @@
     AzureOpenAIEmbeddingSkill,
     AzureOpenAIParameters,
     AzureOpenAIVectorizer,
     BlobIndexerDataToExtract,
     BlobIndexerImageAction,
     BlobIndexerParsingMode,
     BlobIndexerPDFTextRotationAlgorithm,
-    BM25Similarity,
+    BM25SimilarityAlgorithm,
     CharFilter,
     CharFilterName,
     CjkBigramTokenFilter,
-    ClassicSimilarity,
+    CjkBigramTokenFilterScripts,
+    ClassicSimilarityAlgorithm,
     ClassicTokenizer,
     CognitiveServicesAccount,
     CognitiveServicesAccountKey,
     CommonGramTokenFilter,
     ConditionalSkill,
     CorsOptions,
     CustomEntity,
@@ -88,18 +89,20 @@
     GetIndexStatisticsResult,
     HighWaterMarkChangeDetectionPolicy,
     HnswParameters,
     HnswAlgorithmConfiguration,
     ImageAnalysisSkill,
     ImageAnalysisSkillLanguage,
     ImageDetail,
+    IndexerExecutionEnvironment,
     IndexerExecutionResult,
     IndexerExecutionStatus,
     IndexProjectionMode,
     IndexerStatus,
+    IndexingMode,
     IndexingParameters,
     IndexingParametersConfiguration,
     IndexingSchedule,
     InputFieldMappingEntry,
     KeepTokenFilter,
     KeyPhraseExtractionSkill,
     KeyPhraseExtractionSkillLanguage,
@@ -110,38 +113,42 @@
     LexicalAnalyzer,
     LexicalNormalizer,
     LexicalNormalizerName,
     LexicalAnalyzerName,
     LexicalTokenizer,
     LexicalTokenizerName,
     LimitTokenFilter,
+    LineEnding,
     LuceneStandardAnalyzer,
     LuceneStandardTokenizer,
     MagnitudeScoringFunction,
     MagnitudeScoringParameters,
     MappingCharFilter,
     MergeSkill,
     MicrosoftLanguageStemmingTokenizer,
     MicrosoftLanguageTokenizer,
     MicrosoftStemmingTokenizerLanguage,
     MicrosoftTokenizerLanguage,
+    NativeBlobSoftDeleteDeletionDetectionPolicy,
     NGramTokenFilter,
     NGramTokenizer,
     OcrSkill,
     OcrSkillLanguage,
     OutputFieldMappingEntry,
     PathHierarchyTokenizerV2,
     PatternCaptureTokenFilter,
     PatternReplaceCharFilter,
     PatternReplaceTokenFilter,
     PhoneticEncoder,
     PhoneticTokenFilter,
     PIIDetectionSkill,
     PIIDetectionSkillMaskingMode,
     RegexFlags,
+    ScalarQuantizationCompressionConfiguration,
+    ScalarQuantizationParameters,
     ScoringFunction,
     ScoringFunctionAggregation,
     ScoringFunctionInterpolation,
     ScoringProfile,
     SearchIndexer,
     SearchIndexerCache,
     SearchIndexerDataContainer,
@@ -160,35 +167,38 @@
     SearchIndexerKnowledgeStoreProjection,
     SearchIndexerKnowledgeStoreProjectionSelector,
     SearchIndexerKnowledgeStoreTableProjectionSelector,
     SearchIndexerLimits,
     SearchIndexerSkill,
     SearchIndexerStatus,
     SearchIndexerWarning,
+    SearchServiceCounters,
+    SearchServiceLimits,
+    SearchServiceStatistics,
+    SearchSuggester,
     SemanticConfiguration,
     SemanticField,
     SemanticPrioritizedFields,
     SemanticSearch,
     SentimentSkillLanguage,
     ShaperSkill,
     ShingleTokenFilter,
-    Similarity,
+    SimilarityAlgorithm,
     SnowballTokenFilter,
     SnowballTokenFilterLanguage,
     SoftDeleteColumnDeletionDetectionPolicy,
     SplitSkill,
     SplitSkillLanguage,
     SqlIntegratedChangeTrackingPolicy,
     StemmerOverrideTokenFilter,
     StemmerTokenFilter,
     StemmerTokenFilterLanguage,
     StopAnalyzer,
     StopwordsList,
     StopwordsTokenFilter,
-    Suggester,
     SynonymTokenFilter,
     TagScoringFunction,
     TagScoringParameters,
     TextSplitMode,
     TextTranslationSkill,
     TextTranslationSkillLanguage,
     TextWeights,
@@ -198,14 +208,16 @@
     TruncateTokenFilter,
     UaxUrlEmailTokenizer,
     UniqueTokenFilter,
     VectorSearch,
     VectorSearchAlgorithmConfiguration,
     VectorSearchAlgorithmKind,
     VectorSearchAlgorithmMetric,
+    VectorSearchCompressionConfiguration,
+    VectorSearchCompressionTargetDataType,
     VectorSearchProfile,
     VectorSearchVectorizer,
     VectorSearchVectorizerKind,
     VisualFeature,
     WebApiSkill,
     WordDelimiterTokenFilter,
 )
@@ -223,38 +235,22 @@
     SentimentSkillVersion,
     SynonymMap,
 )
 
 SearchFieldDataType = _edm
 
 
-class BM25SimilarityAlgorithm(BM25Similarity):
-    pass
-
-
-class ClassicSimilarityAlgorithm(ClassicSimilarity):
-    pass
-
-
 class KeywordTokenizer(KeywordTokenizerV2):
     pass
 
 
 class PathHierarchyTokenizer(PathHierarchyTokenizerV2):
     pass
 
 
-class SimilarityAlgorithm(Similarity):
-    pass
-
-
-class SearchSuggester(Suggester):
-    pass
-
-
 __all__ = (
     "SearchAlias",
     "AnalyzeTextOptions",
     "AnalyzeResult",
     "AnalyzedTokenInfo",
     "AsciiFoldingTokenFilter",
     "AzureOpenAIEmbeddingSkill",
@@ -265,14 +261,15 @@
     "BlobIndexerImageAction",
     "BlobIndexerParsingMode",
     "BlobIndexerPDFTextRotationAlgorithm",
     "BM25SimilarityAlgorithm",
     "CharFilter",
     "CharFilterName",
     "CjkBigramTokenFilter",
+    "CjkBigramTokenFilterScripts",
     "ClassicSimilarityAlgorithm",
     "ClassicTokenizer",
     "CognitiveServicesAccount",
     "CognitiveServicesAccountKey",
     "CommonGramTokenFilter",
     "ComplexField",
     "ConditionalSkill",
@@ -312,21 +309,20 @@
     "GetIndexStatisticsResult",
     "HighWaterMarkChangeDetectionPolicy",
     "HnswParameters",
     "HnswAlgorithmConfiguration",
     "ImageAnalysisSkill",
     "ImageAnalysisSkillLanguage",
     "ImageDetail",
-    "IndexingSchedule",
-    "IndexingParameters",
-    "IndexingParametersConfiguration",
+    "IndexerExecutionEnvironment",
     "IndexerExecutionResult",
     "IndexerExecutionStatus",
     "IndexProjectionMode",
     "IndexerStatus",
+    "IndexingMode",
     "IndexingParameters",
     "IndexingParametersConfiguration",
     "IndexingSchedule",
     "InputFieldMappingEntry",
     "KeepTokenFilter",
     "KeyPhraseExtractionSkill",
     "KeyPhraseExtractionSkillLanguage",
@@ -337,24 +333,26 @@
     "LexicalAnalyzer",
     "LexicalAnalyzerName",
     "LexicalNormalizer",
     "LexicalNormalizerName",
     "LexicalTokenizer",
     "LexicalTokenizerName",
     "LimitTokenFilter",
+    "LineEnding",
     "LuceneStandardAnalyzer",
     "LuceneStandardTokenizer",
     "MagnitudeScoringFunction",
     "MagnitudeScoringParameters",
     "MappingCharFilter",
     "MergeSkill",
     "MicrosoftLanguageStemmingTokenizer",
     "MicrosoftLanguageTokenizer",
     "MicrosoftStemmingTokenizerLanguage",
     "MicrosoftTokenizerLanguage",
+    "NativeBlobSoftDeleteDeletionDetectionPolicy",
     "NGramTokenFilter",
     "NGramTokenizer",
     "OcrSkill",
     "OcrSkillLanguage",
     "OutputFieldMappingEntry",
     "PathHierarchyTokenizer",
     "PatternAnalyzer",
@@ -363,18 +361,21 @@
     "PatternReplaceTokenFilter",
     "PatternTokenizer",
     "PIIDetectionSkill",
     "PIIDetectionSkillMaskingMode",
     "PhoneticEncoder",
     "PhoneticTokenFilter",
     "RegexFlags",
+    "ScalarQuantizationCompressionConfiguration",
+    "ScalarQuantizationParameters",
     "ScoringFunction",
     "ScoringFunctionAggregation",
     "ScoringFunctionInterpolation",
     "ScoringProfile",
+    "SearchableField",
     "SearchField",
     "SearchIndex",
     "SearchIndexer",
     "SearchIndexerCache",
     "SearchIndexerDataContainer",
     "SearchIndexerDataIdentity",
     "SearchIndexerDataNoneIdentity",
@@ -394,15 +395,18 @@
     "SearchIndexerKnowledgeStoreTableProjectionSelector",
     "SearchIndexerLimits",
     "SearchIndexerSkill",
     "SearchIndexerSkillset",
     "SearchIndexerStatus",
     "SearchIndexerWarning",
     "SearchResourceEncryptionKey",
-    "SearchableField",
+    "SearchServiceCounters",
+    "SearchServiceLimits",
+    "SearchServiceStatistics",
+    "SearchSuggester",
     "SemanticConfiguration",
     "SemanticField",
     "SemanticPrioritizedFields",
     "SemanticSearch",
     "SentimentSkill",
     "SentimentSkillLanguage",
     "SentimentSkillVersion",
@@ -418,15 +422,14 @@
     "SqlIntegratedChangeTrackingPolicy",
     "StemmerOverrideTokenFilter",
     "StemmerTokenFilter",
     "StemmerTokenFilterLanguage",
     "StopAnalyzer",
     "StopwordsList",
     "StopwordsTokenFilter",
-    "SearchSuggester",
     "SuggestOptions",
     "SynonymMap",
     "SynonymTokenFilter",
     "TagScoringFunction",
     "TagScoringParameters",
     "TextSplitMode",
     "TextTranslationSkill",
@@ -438,14 +441,16 @@
     "TruncateTokenFilter",
     "UaxUrlEmailTokenizer",
     "UniqueTokenFilter",
     "VectorSearch",
     "VectorSearchAlgorithmConfiguration",
     "VectorSearchAlgorithmKind",
     "VectorSearchAlgorithmMetric",
+    "VectorSearchCompressionConfiguration",
+    "VectorSearchCompressionTargetDataType",
     "VectorSearchProfile",
     "VectorSearchVectorizer",
     "VectorSearchVectorizerKind",
     "VisualFeature",
     "WebApiSkill",
     "WordDelimiterTokenFilter",
     "SearchFieldDataType",
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_edm.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_edm.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_index.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,23 @@
         "Edm.ComplexType", and "Edm.Single".
     :vartype type: str or ~azure.search.documents.indexes.models.SearchFieldDataType
     :ivar key: A value indicating whether the field uniquely identifies documents in the index.
         Exactly one top-level field in each index must be chosen as the key field and it must be of
         type Edm.String. Key fields can be used to look up documents directly and update or delete
         specific documents. Default is false for simple fields and null for complex fields.
     :vartype key: bool
+    :ivar stored: An immutable value indicating whether the field will be persisted separately on
+       disk to be returned in a search result. You can disable this option if you don't plan to return
+       the field contents in a search response to save on storage overhead. This can only be set
+       during index creation and only for vector fields. This property cannot be changed for existing
+       fields or set as false for new fields. If this property is set as false, the property
+       'hidden' must be set to true. This property must be true or unset for key fields,
+       for new fields, and for non-vector fields, and it must be null for complex fields. Disabling
+       this property will reduce index storage requirements. The default is true for vector fields.
+    :vartype stored: bool
     :ivar searchable: A value indicating whether the field is full-text searchable. This means it
         will undergo analysis such as word-breaking during indexing. If you set a searchable field to a
         value like "sunny day", internally it will be split into the individual tokens "sunny" and
         "day". This enables full-text searches for these terms. Fields of type Edm.String or
         Collection(Edm.String) are searchable by default. This property must be false for simple fields
         of other non-string data types, and it must be null for complex fields. Note: searchable fields
         consume extra space in your index since Azure Cognitive Search will store an additional
@@ -165,14 +174,15 @@
     """
 
     def __init__(self, **kwargs):
         self.name = kwargs["name"]
         self.type = kwargs["type"]
         self.key = kwargs.get("key", None)
         self.hidden = kwargs.get("hidden", None)
+        self.stored = kwargs.get("stored", None)
         self.searchable = kwargs.get("searchable", None)
         self.filterable = kwargs.get("filterable", None)
         self.sortable = kwargs.get("sortable", None)
         self.facetable = kwargs.get("facetable", None)
         self.analyzer_name = kwargs.get("analyzer_name", None)
         self.search_analyzer_name = kwargs.get("search_analyzer_name", None)
         self.index_analyzer_name = kwargs.get("index_analyzer_name", None)
@@ -186,14 +196,15 @@
         fields = [pack_search_field(x) for x in self.fields] if self.fields else None
         retrievable = not self.hidden if self.hidden is not None else None
         return _SearchField(
             name=self.name,
             type=self.type,
             key=self.key,
             retrievable=retrievable,
+            stored=self.stored,
             searchable=self.searchable,
             filterable=self.filterable,
             sortable=self.sortable,
             facetable=self.facetable,
             analyzer=self.analyzer_name,
             search_analyzer=self.search_analyzer_name,
             index_analyzer=self.index_analyzer_name,
@@ -216,14 +227,15 @@
         except AttributeError:
             normalizer = None
         return cls(
             name=search_field.name,
             type=search_field.type,
             key=search_field.key,
             hidden=hidden,
+            stored=search_field.stored,
             searchable=search_field.searchable,
             filterable=search_field.filterable,
             sortable=search_field.sortable,
             facetable=search_field.facetable,
             analyzer_name=search_field.analyzer,
             search_analyzer_name=search_field.search_analyzer,
             index_analyzer_name=search_field.index_analyzer,
```

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/indexes/models/_models.py` & `azure-search-documents-11.6.0b3/azure/search/documents/indexes/models/_models.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure/search/documents/models/__init__.py` & `azure-search-documents-11.6.0b3/azure/search/documents/models/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/azure_search_documents.egg-info/PKG-INFO` & `azure-search-documents-11.6.0b3/azure_search_documents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.6.0b2
+Version: 11.6.0b3
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core<2.0.0,>=1.28.0
-Requires-Dist: azure-common~=1.1
+Requires-Dist: azure-core>=1.28.0
+Requires-Dist: azure-common>=1.1
 Requires-Dist: isodate>=0.6.0
 
 # Azure AI Search client library for Python
 
 [Azure AI Search](https://docs.microsoft.com/azure/search/) (formerly known as "Azure Cognitive Search") is an AI-powered information retrieval platform that helps developers build rich search experiences and generative AI apps that combine large language models with enterprise data.
 
 Azure AI Search is well suited for the following application scenarios:
@@ -189,15 +189,15 @@
 
 **Semantic ranking** enhances the quality of search results for text-based queries. By enabling semantic ranking on your search service, you can improve the relevance of search results in two ways:
 - It applies secondary ranking to the initial result set, promoting the most semantically relevant results to the top.
 - It extracts and returns captions and answers in the response, which can be displayed on a search page to enhance the user's search experience.
 
 To learn more about semantic ranking, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview).
 
-**Vector search** is an information retrieval technique that overcomes the limitations of traditional keyword-based search. Instead of relying solely on lexical analysis and matching individual query terms, vector search uses algorithms for similarity and concept search. It represents documents and queries as vectors in a high-dimensional space called an embedding. By searching on vector representations of content, a vector query can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
+**Vector search** is an information retrieval technique that uses numeric representations of searchable documents and query strings. By searching for numeric representations of content that are most similar to the numeric query, vector search can find relevant matches, even if the exact terms of the query are not present in the index. Moreover, vector search can be applied to various types of content, including images and videos and translated text, not just same-language text.
 
 To learn how to index vector fields and perform vector search, you can refer to the [sample](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/search/azure-search-documents/samples/sample_vector_search.py). This sample provides detailed guidance on indexing vector fields and demonstrates how to perform vector search.
 
 Additionally, for more comprehensive information about vector search, including its concepts and usage, you can refer to the [documentation](https://learn.microsoft.com/azure/search/vector-search-overview). The documentation provides in-depth explanations and guidance on leveraging the power of vector search in Azure AI Search.
 
 _The `Azure.Search.Documents` client library (v1) provides APIs for data plane operations. The
 previous `Microsoft.Azure.Search` client library (v10) is now retired. It has many similar looking APIs, so please be careful to avoid confusion when exploring online resources. A good rule of thumb is to check for the namespace
```

### Comparing `azure-search-documents-11.6.0b2/azure_search_documents.egg-info/SOURCES.txt` & `azure-search-documents-11.6.0b3/azure_search_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/README.md` & `azure-search-documents-11.6.0b3/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_analyze_text_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_analyze_text_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_authentication_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_authentication_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_autocomplete_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_autocomplete_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_buffered_sender_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_buffered_sender_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_crud_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_data_source_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_data_source_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_facet_query_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_facet_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_filter_query_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_filter_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_get_document_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_get_document_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_index_alias_crud_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_alias_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_index_client_send_request_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_client_send_request_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_index_crud_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_index_crud_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_indexers_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_indexers_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_query_session_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_query_session_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_search_client_send_request_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_search_client_send_request_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_semantic_search_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_semantic_search_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_simple_query_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_simple_query_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_suggestions_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_suggestions_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_synonym_map_operations_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_synonym_map_operations_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/async_samples/sample_vector_search_async.py` & `azure-search-documents-11.6.0b3/samples/async_samples/sample_vector_search_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_analyze_text.py` & `azure-search-documents-11.6.0b3/samples/sample_analyze_text.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_authentication.py` & `azure-search-documents-11.6.0b3/samples/sample_authentication.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_autocomplete.py` & `azure-search-documents-11.6.0b3/samples/sample_autocomplete.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_buffered_sender.py` & `azure-search-documents-11.6.0b3/samples/sample_buffered_sender.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_crud_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_data_source_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_data_source_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_facet_query.py` & `azure-search-documents-11.6.0b3/samples/sample_facet_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_filter_query.py` & `azure-search-documents-11.6.0b3/samples/sample_filter_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_get_document.py` & `azure-search-documents-11.6.0b3/samples/sample_get_document.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_index_alias_crud_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_index_alias_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_index_client_send_request.py` & `azure-search-documents-11.6.0b3/samples/sample_index_client_send_request.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_index_crud_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_index_crud_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_indexer_datasource_skillset.py` & `azure-search-documents-11.6.0b3/samples/sample_indexer_datasource_skillset.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_indexers_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_indexers_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_query_session.py` & `azure-search-documents-11.6.0b3/samples/sample_query_session.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_search_client_send_request.py` & `azure-search-documents-11.6.0b3/samples/sample_search_client_send_request.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_semantic_search.py` & `azure-search-documents-11.6.0b3/samples/sample_semantic_search.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_simple_query.py` & `azure-search-documents-11.6.0b3/samples/sample_simple_query.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_suggestions.py` & `azure-search-documents-11.6.0b3/samples/sample_suggestions.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_synonym_map_operations.py` & `azure-search-documents-11.6.0b3/samples/sample_synonym_map_operations.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/samples/sample_vector_search.py` & `azure-search-documents-11.6.0b3/samples/sample_vector_search.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/setup.py` & `azure-search-documents-11.6.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,12 +60,12 @@
             # Exclude packages that will be covered by PEP420 or nspkg
             "azure",
             "azure.search",
         ]
     ),
     python_requires=">=3.8",
     install_requires=[
-        "azure-core<2.0.0,>=1.28.0",
-        "azure-common~=1.1",
+        "azure-core>=1.28.0",
+        "azure-common>=1.1",
         "isodate>=0.6.0",
     ],
 )
```

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_buffered_sender_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_buffered_sender_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_basic_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_basic_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_buffered_sender_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_buffered_sender_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_index_document_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_index_document_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_client_search_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_client_search_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_alias_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_alias_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_data_source_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_data_source_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_skillset_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_skillset_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_index_client_synonym_map_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_index_client_synonym_map_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/async_tests/test_search_indexer_client_live_async.py` & `azure-search-documents-11.6.0b3/tests/async_tests/test_search_indexer_client_live_async.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/conftest.py` & `azure-search-documents-11.6.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/perfstress_tests/autocomplete.py` & `azure-search-documents-11.6.0b3/tests/perfstress_tests/autocomplete.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/perfstress_tests/search_documents.py` & `azure-search-documents-11.6.0b3/tests/perfstress_tests/search_documents.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/perfstress_tests/suggest.py` & `azure-search-documents-11.6.0b3/tests/perfstress_tests/suggest.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/search_service_preparer.py` & `azure-search-documents-11.6.0b3/tests/search_service_preparer.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_buffered_sender.py` & `azure-search-documents-11.6.0b3/tests/test_buffered_sender.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_index_documents_batch.py` & `azure-search-documents-11.6.0b3/tests/test_index_documents_batch.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_index_field_helpers.py` & `azure-search-documents-11.6.0b3/tests/test_index_field_helpers.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_queries.py` & `azure-search-documents-11.6.0b3/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_regex_flags.py` & `azure-search-documents-11.6.0b3/tests/test_regex_flags.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_client.py` & `azure-search-documents-11.6.0b3/tests/test_search_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_client_basic_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_client_basic_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_client_buffered_sender_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_client_buffered_sender_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_client_index_document_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_client_index_document_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_client_search_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_client_search_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client_alias_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client_alias_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client_data_source_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client_data_source_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client_skillset_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client_skillset_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_index_client_synonym_map_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_index_client_synonym_map_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_search_indexer_client_live.py` & `azure-search-documents-11.6.0b3/tests/test_search_indexer_client_live.py`

 * *Files identical despite different names*

### Comparing `azure-search-documents-11.6.0b2/tests/test_serialization.py` & `azure-search-documents-11.6.0b3/tests/test_serialization.py`

 * *Files identical despite different names*

