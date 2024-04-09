# Comparing `tmp/arvados-python-client-2.7.1.tar.gz` & `tmp/arvados-python-client-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.7.1.tar", last modified: Tue Dec 12 20:51:46 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-python-client-2.7.2.tar", last modified: Tue Apr  9 20:11:19 2024, max compression
```

## Comparing `arvados-python-client-2.7.1.tar` & `arvados-python-client-2.7.2.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2457 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7332 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2265 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3511 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/_pycurlhelper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-12-12 20:51:44.000000 arvados-python-client-2.7.1/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21264 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    47762 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    93813 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2127 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    37771 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18760 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13311 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23714 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11886 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1564 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      988 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13562 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/http_to_keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    63649 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1208 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/logging.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8586 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2902 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3833 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28299 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados/vocabulary.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)   368111 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados-v1-discovery.json
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2096 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      348 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-12-12 20:51:45.000000 arvados-python-client-2.7.1/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/bin/arv-ws
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    15250 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/discovery2pydoc.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:46.000000 arvados-python-client-2.7.1/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    37955 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23177 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8687 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43674 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77476 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19428 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_http.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    83499 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9387 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-12-12 20:51:23.000000 arvados-python-client-2.7.1/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2457 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7874 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2265 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3511 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2024-04-09 20:11:17.000000 arvados-python-client-2.7.2/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21264 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    48875 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    93813 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6036 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    37771 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18760 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13311 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    24015 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3383 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11886 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57567 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1564 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      988 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9197 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13562 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    63190 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1208 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/logging.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8586 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2902 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3833 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28299 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados/vocabulary.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)   368111 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados-v1-discovery.json
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3417 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2149 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      348 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/bin/arv-ws
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    15250 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/discovery2pydoc.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4849 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10197 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:19.000000 arvados-python-client-2.7.2/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    37955 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23177 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8687 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10920 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43718 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6363 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_cmd_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77476 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19428 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    78007 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2440 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6382 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_storage_classes.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11337 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9387 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2024-04-09 20:11:07.000000 arvados-python-client-2.7.2/tests/test_vocabulary.py
```

### Comparing `arvados-python-client-2.7.1/LICENSE-2.0.txt` & `arvados-python-client-2.7.2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/PKG-INFO` & `arvados-python-client-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.7.1/README.rst` & `arvados-python-client-2.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/__init__.py` & `arvados-python-client-2.7.2/arvados/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 # SPDX-License-Identifier: Apache-2.0
 """Arvados Python SDK
 
 This module provides the entire Python SDK for Arvados. The most useful modules
 include:
 
-* arvados.api - After you `import arvados`, you can call `arvados.api.api` as
-  `arvados.api` to construct a client object.
+* arvados.api - After you `import arvados`, you can call `arvados.api` as a
+  shortcut to the client constructor function `arvados.api.api`.
 
 * arvados.collection - The `arvados.collection.Collection` class provides a
   high-level interface to read and write collections. It coordinates sending
   data to and from Keep, and synchronizing updates with the collection object.
 
 * arvados.util - Utility functions to use mostly in conjunction with the API
   client object and the results it returns.
@@ -22,23 +22,32 @@
 import logging as stdliblog
 import os
 import sys
 import types
 
 from collections import UserDict
 
-from .api import api, api_from_config, http_cache
+from . import api, errors, util
+from .api import api_from_config, http_cache
 from .collection import CollectionReader, CollectionWriter, ResumableCollectionWriter
 from arvados.keep import *
 from arvados.stream import *
 from .arvfile import StreamFileReader
 from .logging import log_format, log_date_format, log_handler
 from .retry import RetryLoop
-import arvados.errors as errors
-import arvados.util as util
+
+# Previous versions of the PySDK used to say `from .api import api`.  This
+# made it convenient to call the API client constructor, but difficult to
+# access the rest of the `arvados.api` module. The magic below fixes that
+# bug while retaining backwards compatibility: `arvados.api` is now the
+# module and you can import it normally, but we make that module callable so
+# all the existing code that says `arvados.api('v1', ...)` still works.
+class _CallableAPIModule(api.__class__):
+    __call__ = staticmethod(api.api)
+api.__class__ = _CallableAPIModule
 
 # Override logging module pulled in via `from ... import *`
 # so users can `import arvados.logging`.
 logging = sys.modules['arvados.logging']
 
 # Set up Arvados logging based on the user's configuration.
 # All Arvados code should log under the arvados hierarchy.
```

### Comparing `arvados-python-client-2.7.1/arvados/_normalize_stream.py` & `arvados-python-client-2.7.2/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/_pycurlhelper.py` & `arvados-python-client-2.7.2/arvados/_pycurlhelper.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/_ranges.py` & `arvados-python-client-2.7.2/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/api.py` & `arvados-python-client-2.7.2/arvados/api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/arvfile.py` & `arvados-python-client-2.7.2/arvados/arvfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
                  storage_classes_func=None):
         """keep: KeepClient object to use"""
         self._keep = keep
         self._bufferblocks = collections.OrderedDict()
         self._put_queue = None
         self._put_threads = None
         self.lock = threading.Lock()
-        self.prefetch_enabled = True
+        self.prefetch_lookahead = self._keep.num_prefetch_threads
         self.num_put_threads = put_threads or _BlockManager.DEFAULT_PUT_THREADS
         self.copies = copies
         self.storage_classes = storage_classes_func or (lambda: [])
         self._pending_write_size = 0
         self.threads_lock = threading.Lock()
         self.padding_block = None
         self.num_retries = num_retries
@@ -799,15 +799,15 @@
 
         self.stop_threads()
 
     def block_prefetch(self, locator):
         """Initiate a background download of a block.
         """
 
-        if not self.prefetch_enabled:
+        if not self.prefetch_lookahead:
             return
 
         with self.lock:
             if locator in self._bufferblocks:
                 return
 
         self._keep.block_prefetch(locator)
@@ -821,15 +821,15 @@
     read/write access.
 
     This object may be accessed from multiple threads.
 
     """
 
     __slots__ = ('parent', 'name', '_writers', '_committed',
-                 '_segments', 'lock', '_current_bblock', 'fuse_entry')
+                 '_segments', 'lock', '_current_bblock', 'fuse_entry', '_read_counter')
 
     def __init__(self, parent, name, stream=[], segments=[]):
         """
         ArvadosFile constructor.
 
         :stream:
           a list of Range objects representing a block stream
@@ -842,14 +842,15 @@
         self._writers = set()
         self._committed = False
         self._segments = []
         self.lock = parent.root_collection().lock
         for s in segments:
             self._add_segment(stream, s.locator, s.range_size)
         self._current_bblock = None
+        self._read_counter = 0
 
     def writable(self):
         return self.parent.writable()
 
     @synchronized
     def permission_expired(self, as_of_dt=None):
         """Returns True if any of the segment's locators is expired"""
@@ -1056,33 +1057,55 @@
          only return less data than requested when hitting EOF.
         """
 
         with self.lock:
             if size == 0 or offset >= self.size():
                 return b''
             readsegs = locators_and_ranges(self._segments, offset, size)
-            prefetch = locators_and_ranges(self._segments, offset + size, config.KEEP_BLOCK_SIZE * self.parent._my_block_manager()._keep.num_prefetch_threads, limit=32)
+
+            prefetch = None
+            prefetch_lookahead = self.parent._my_block_manager().prefetch_lookahead
+            if prefetch_lookahead:
+                # Doing prefetch on every read() call is surprisingly expensive
+                # when we're trying to deliver data at 600+ MiBps and want
+                # the read() fast path to be as lightweight as possible.
+                #
+                # Only prefetching every 128 read operations
+                # dramatically reduces the overhead while still
+                # getting the benefit of prefetching (e.g. when
+                # reading 128 KiB at a time, it checks for prefetch
+                # every 16 MiB).
+                self._read_counter = (self._read_counter+1) % 128
+                if self._read_counter == 1:
+                    prefetch = locators_and_ranges(self._segments,
+                                                   offset + size,
+                                                   config.KEEP_BLOCK_SIZE * prefetch_lookahead,
+                                                   limit=(1+prefetch_lookahead))
 
         locs = set()
         data = []
         for lr in readsegs:
             block = self.parent._my_block_manager().get_block_contents(lr.locator, num_retries=num_retries, cache_only=(bool(data) and not exact))
             if block:
                 blockview = memoryview(block)
-                data.append(blockview[lr.segment_offset:lr.segment_offset+lr.segment_size].tobytes())
+                data.append(blockview[lr.segment_offset:lr.segment_offset+lr.segment_size])
                 locs.add(lr.locator)
             else:
                 break
 
-        for lr in prefetch:
-            if lr.locator not in locs:
-                self.parent._my_block_manager().block_prefetch(lr.locator)
-                locs.add(lr.locator)
+        if prefetch:
+            for lr in prefetch:
+                if lr.locator not in locs:
+                    self.parent._my_block_manager().block_prefetch(lr.locator)
+                    locs.add(lr.locator)
 
-        return b''.join(data)
+        if len(data) == 1:
+            return data[0]
+        else:
+            return b''.join(data)
 
     @must_be_writable
     @synchronized
     def writeto(self, offset, data, num_retries):
         """Write `data` to the file starting at `offset`.
 
         This will update existing bytes and/or extend the size of the file as
```

### Comparing `arvados-python-client-2.7.1/arvados/cache.py` & `arvados-python-client-2.7.2/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/collection.py` & `arvados-python-client-2.7.2/arvados/collection.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/arv_copy.py` & `arvados-python-client-2.7.2/arvados/commands/arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/federation_migrate.py` & `arvados-python-client-2.7.2/arvados/commands/federation_migrate.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/get.py` & `arvados-python-client-2.7.2/arvados/commands/get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/keepdocker.py` & `arvados-python-client-2.7.2/arvados/commands/keepdocker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # Copyright (C) The Arvados Authors. All rights reserved.
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from builtins import next
 import argparse
 import collections
 import datetime
 import errno
+import fcntl
 import json
+import logging
 import os
 import re
+import subprocess
 import sys
 import tarfile
 import tempfile
-import shutil
-import _strptime
-import fcntl
+
+import ciso8601
 from operator import itemgetter
 from stat import *
 
-import subprocess
-
 import arvados
+import arvados.config
 import arvados.util
 import arvados.commands._util as arv_cmd
 import arvados.commands.put as arv_put
-from arvados.collection import CollectionReader
-import ciso8601
-import logging
-import arvados.config
-
 from arvados._version import __version__
 
 logger = logging.getLogger('arvados.keepdocker')
 logger.setLevel(logging.DEBUG if arvados.config.get('ARVADOS_DEBUG')
                 else logging.INFO)
 
 EARLIEST_DATETIME = datetime.datetime(datetime.MINYEAR, 1, 1, 0, 0, 0)
@@ -352,14 +347,33 @@
 
 def _uuid2pdh(api, uuid):
     return api.collections().list(
         filters=[['uuid', '=', uuid]],
         select=['portable_data_hash'],
     ).execute()['items'][0]['portable_data_hash']
 
+def load_image_metadata(image_file):
+    """Load an image manifest and config from an archive
+
+    Given an image archive as an open binary file object, this function loads
+    the image manifest and configuration, deserializing each from JSON and
+    returning them in a 2-tuple of dicts.
+    """
+    image_file.seek(0)
+    with tarfile.open(fileobj=image_file) as image_tar:
+        with image_tar.extractfile('manifest.json') as manifest_file:
+            image_manifest_list = json.load(manifest_file)
+        # Because arv-keepdocker only saves one image, there should only be
+        # one manifest.  This extracts that from the list and raises
+        # ValueError if there's not exactly one.
+        image_manifest, = image_manifest_list
+        with image_tar.extractfile(image_manifest['Config']) as config_file:
+            image_config = json.load(config_file)
+    return image_manifest, image_config
+
 def main(arguments=None, stdout=sys.stdout, install_sig_handlers=True, api=None):
     args = arg_parser.parse_args(arguments)
     if api is None:
         api = arvados.api('v1', num_retries=args.retries)
 
     if args.image is None or args.image == 'images':
         fmt = "{:30}  {:10}  {:12}  {:29}  {:20}\n"
@@ -528,29 +542,17 @@
         coll_uuid = arv_put.main(
             put_args + ['--filename', outfile_name, image_file.name], stdout=stdout,
             install_sig_handlers=install_sig_handlers).strip()
 
         # Managed properties could be already set
         coll_properties = api.collections().get(uuid=coll_uuid).execute(num_retries=args.retries).get('properties', {})
         coll_properties.update({"docker-image-repo-tag": image_repo_tag})
-
         api.collections().update(uuid=coll_uuid, body={"properties": coll_properties}).execute(num_retries=args.retries)
 
-        # Read the image metadata and make Arvados links from it.
-        image_file.seek(0)
-        image_tar = tarfile.open(fileobj=image_file)
-        image_hash_type, _, raw_image_hash = image_hash.rpartition(':')
-        if image_hash_type:
-            json_filename = raw_image_hash + '.json'
-        else:
-            json_filename = raw_image_hash + '/json'
-        json_file = image_tar.extractfile(image_tar.getmember(json_filename))
-        image_metadata = json.loads(json_file.read().decode('utf-8'))
-        json_file.close()
-        image_tar.close()
+        _, image_metadata = load_image_metadata(image_file)
         link_base = {'head_uuid': coll_uuid, 'properties': {}}
         if 'created' in image_metadata:
             link_base['properties']['image_timestamp'] = image_metadata['created']
         if args.project_uuid is not None:
             link_base['owner_uuid'] = args.project_uuid
 
         make_link(api, args.retries, 'docker_image_hash', image_hash, **link_base)
```

### Comparing `arvados-python-client-2.7.1/arvados/commands/ls.py` & `arvados-python-client-2.7.2/arvados/commands/ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/migrate19.py` & `arvados-python-client-2.7.2/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/put.py` & `arvados-python-client-2.7.2/arvados/commands/put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/run.py` & `arvados-python-client-2.7.2/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/commands/ws.py` & `arvados-python-client-2.7.2/arvados/commands/ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/config.py` & `arvados-python-client-2.7.2/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/crunch.py` & `arvados-python-client-2.7.2/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/diskcache.py` & `arvados-python-client-2.7.2/arvados/diskcache.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import stat
 import tempfile
 import fcntl
 import time
 import errno
 import logging
 import weakref
+import collections
 
 _logger = logging.getLogger('arvados.keep')
 
 cacheblock_suffix = ".keepcacheblock"
 
 class DiskCacheSlot(object):
     __slots__ = ("locator", "ready", "content", "cachedir", "filehandle", "linger")
@@ -27,34 +28,43 @@
         self.content = None
         self.cachedir = cachedir
         self.filehandle = None
         self.linger = None
 
     def get(self):
         self.ready.wait()
+        # 'content' can None, an empty byte string, or a nonempty mmap
+        # region.  If it is an mmap region, we want to advise the
+        # kernel we're going to use it.  This nudges the kernel to
+        # re-read most or all of the block if necessary (instead of
+        # just a few pages at a time), reducing the number of page
+        # faults and improving performance by 4x compared to not
+        # calling madvise.
+        if self.content:
+            self.content.madvise(mmap.MADV_WILLNEED)
         return self.content
 
     def set(self, value):
         tmpfile = None
         try:
             if value is None:
                 self.content = None
                 self.ready.set()
-                return
+                return False
 
             if len(value) == 0:
                 # Can't mmap a 0 length file
                 self.content = b''
                 self.ready.set()
-                return
+                return True
 
             if self.content is not None:
                 # Has been set already
                 self.ready.set()
-                return
+                return False
 
             blockdir = os.path.join(self.cachedir, self.locator[0:3])
             os.makedirs(blockdir, mode=0o700, exist_ok=True)
 
             final = os.path.join(blockdir, self.locator) + cacheblock_suffix
 
             self.filehandle = tempfile.NamedTemporaryFile(dir=blockdir, delete=False, prefix="tmp", suffix=cacheblock_suffix)
@@ -69,14 +79,15 @@
             self.filehandle.flush()
             os.rename(tmpfile, final)
             tmpfile = None
 
             self.content = mmap.mmap(self.filehandle.fileno(), 0, access=mmap.ACCESS_READ)
             # only set the event when mmap is successful
             self.ready.set()
+            return True
         finally:
             if tmpfile is not None:
                 # If the tempfile hasn't been renamed on disk yet, try to delete it.
                 try:
                     os.remove(tmpfile)
                 except:
                     pass
@@ -91,73 +102,69 @@
                 if content is not None:
                     return len(content)
             return 0
         else:
             return len(self.content)
 
     def evict(self):
-        if self.content is not None and len(self.content) > 0:
-            # The mmap region might be in use when we decided to evict
-            # it.  This can happen if the cache is too small.
-            #
-            # If we call close() now, it'll throw an error if
-            # something tries to access it.
-            #
-            # However, we don't need to explicitly call mmap.close()
-            #
-            # I confirmed in mmapmodule.c that that both close
-            # and deallocate do the same thing:
-            #
-            # a) close the file descriptor
-            # b) unmap the memory range
-            #
-            # So we can forget it in the cache and delete the file on
-            # disk, and it will tear it down after any other
-            # lingering Python references to the mapped memory are
-            # gone.
+        if not self.content:
+            return
 
-            blockdir = os.path.join(self.cachedir, self.locator[0:3])
-            final = os.path.join(blockdir, self.locator) + cacheblock_suffix
-            try:
-                fcntl.flock(self.filehandle, fcntl.LOCK_UN)
+        # The mmap region might be in use when we decided to evict
+        # it.  This can happen if the cache is too small.
+        #
+        # If we call close() now, it'll throw an error if
+        # something tries to access it.
+        #
+        # However, we don't need to explicitly call mmap.close()
+        #
+        # I confirmed in mmapmodule.c that that both close
+        # and deallocate do the same thing:
+        #
+        # a) close the file descriptor
+        # b) unmap the memory range
+        #
+        # So we can forget it in the cache and delete the file on
+        # disk, and it will tear it down after any other
+        # lingering Python references to the mapped memory are
+        # gone.
 
-                # try to get an exclusive lock, this ensures other
-                # processes are not using the block.  It is
-                # nonblocking and will throw an exception if we
-                # can't get it, which is fine because that means
-                # we just won't try to delete it.
-                #
-                # I should note here, the file locking is not
-                # strictly necessary, we could just remove it and
-                # the kernel would ensure that the underlying
-                # inode remains available as long as other
-                # processes still have the file open.  However, if
-                # you have multiple processes sharing the cache
-                # and deleting each other's files, you'll end up
-                # with a bunch of ghost files that don't show up
-                # in the file system but are still taking up
-                # space, which isn't particularly user friendly.
-                # The locking strategy ensures that cache blocks
-                # in use remain visible.
-                #
-                fcntl.flock(self.filehandle, fcntl.LOCK_EX | fcntl.LOCK_NB)
+        blockdir = os.path.join(self.cachedir, self.locator[0:3])
+        final = os.path.join(blockdir, self.locator) + cacheblock_suffix
+        try:
+            fcntl.flock(self.filehandle, fcntl.LOCK_UN)
 
-                os.remove(final)
-                return True
-            except OSError:
-                pass
-            finally:
-                self.filehandle = None
-                self.linger = weakref.ref(self.content)
-                self.content = None
-        return False
+            # try to get an exclusive lock, this ensures other
+            # processes are not using the block.  It is
+            # nonblocking and will throw an exception if we
+            # can't get it, which is fine because that means
+            # we just won't try to delete it.
+            #
+            # I should note here, the file locking is not
+            # strictly necessary, we could just remove it and
+            # the kernel would ensure that the underlying
+            # inode remains available as long as other
+            # processes still have the file open.  However, if
+            # you have multiple processes sharing the cache
+            # and deleting each other's files, you'll end up
+            # with a bunch of ghost files that don't show up
+            # in the file system but are still taking up
+            # space, which isn't particularly user friendly.
+            # The locking strategy ensures that cache blocks
+            # in use remain visible.
+            #
+            fcntl.flock(self.filehandle, fcntl.LOCK_EX | fcntl.LOCK_NB)
 
-    def gone(self):
-        # Test if an evicted object is lingering
-        return self.content is None and (self.linger is None or self.linger() is None)
+            os.remove(final)
+            return True
+        except OSError:
+            pass
+        finally:
+            self.filehandle = None
+            self.content = None
 
     @staticmethod
     def get_from_disk(locator, cachedir):
         blockdir = os.path.join(cachedir, locator[0:3])
         final = os.path.join(blockdir, locator) + cacheblock_suffix
 
         try:
@@ -233,20 +240,20 @@
         # sort by access time (atime), going from most recently
         # accessed (highest timestamp) to least recently accessed
         # (lowest timestamp).
         blocks.sort(key=lambda x: x[1], reverse=True)
 
         # Map in all the files we found, up to maxslots, if we exceed
         # maxslots, start throwing things out.
-        cachelist = []
+        cachelist: collections.OrderedDict = collections.OrderedDict()
         for b in blocks:
             got = DiskCacheSlot.get_from_disk(b[0], cachedir)
             if got is None:
                 continue
             if len(cachelist) < maxslots:
-                cachelist.append(got)
+                cachelist[got.locator] = got
             else:
                 # we found more blocks than maxslots, try to
                 # throw it out of the cache.
                 got.evict()
 
         return cachelist
```

### Comparing `arvados-python-client-2.7.1/arvados/errors.py` & `arvados-python-client-2.7.2/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/events.py` & `arvados-python-client-2.7.2/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/http_to_keep.py` & `arvados-python-client-2.7.2/arvados/http_to_keep.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/keep.py` & `arvados-python-client-2.7.2/arvados/keep.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
     @staticmethod
     def put(data, **kwargs):
         return Keep.global_client_object().put(data, **kwargs)
 
 class KeepBlockCache(object):
     def __init__(self, cache_max=0, max_slots=0, disk_cache=False, disk_cache_dir=None):
         self.cache_max = cache_max
-        self._cache = []
+        self._cache = collections.OrderedDict()
         self._cache_lock = threading.Lock()
         self._max_slots = max_slots
         self._disk_cache = disk_cache
         self._disk_cache_dir = disk_cache_dir
         self._cache_updating = threading.Condition(self._cache_lock)
 
         if self._disk_cache and self._disk_cache_dir is None:
@@ -229,102 +229,90 @@
                 self.cache_max = min(min(maxdisk, avail), (self._max_slots * 64 * 1024 * 1024))
             else:
                 # 256 MiB in RAM
                 self.cache_max = (256 * 1024 * 1024)
 
         self.cache_max = max(self.cache_max, 64 * 1024 * 1024)
 
+        self.cache_total = 0
         if self._disk_cache:
             self._cache = arvados.diskcache.DiskCacheSlot.init_cache(self._disk_cache_dir, self._max_slots)
+            for slot in self._cache.values():
+                self.cache_total += slot.size()
             self.cap_cache()
 
-
     class CacheSlot(object):
         __slots__ = ("locator", "ready", "content")
 
         def __init__(self, locator):
             self.locator = locator
             self.ready = threading.Event()
             self.content = None
 
         def get(self):
             self.ready.wait()
             return self.content
 
         def set(self, value):
+            if self.content is not None:
+                return False
             self.content = value
             self.ready.set()
+            return True
 
         def size(self):
             if self.content is None:
                 return 0
             else:
                 return len(self.content)
 
         def evict(self):
             self.content = None
-            return self.gone()
 
-        def gone(self):
-            return (self.content is None)
 
     def _resize_cache(self, cache_max, max_slots):
         # Try and make sure the contents of the cache do not exceed
         # the supplied maximums.
 
-        # Select all slots except those where ready.is_set() and content is
-        # None (that means there was an error reading the block).
-        self._cache = [c for c in self._cache if not (c.ready.is_set() and c.content is None)]
-        sm = sum([slot.size() for slot in self._cache])
-        while len(self._cache) > 0 and (sm > cache_max or len(self._cache) > max_slots):
-            for i in range(len(self._cache)-1, -1, -1):
-                # start from the back, find a slot that is a candidate to evict
-                if self._cache[i].ready.is_set():
-                    sz = self._cache[i].size()
-
-                    # If evict returns false it means the
-                    # underlying disk cache couldn't lock the file
-                    # for deletion because another process was using
-                    # it. Don't count it as reducing the amount
-                    # of data in the cache, find something else to
-                    # throw out.
-                    if self._cache[i].evict():
-                        sm -= sz
-
-                    # check to make sure the underlying data is gone
-                    if self._cache[i].gone():
-                        # either way we forget about it.  either the
-                        # other process will delete it, or if we need
-                        # it again and it is still there, we'll find
-                        # it on disk.
-                        del self._cache[i]
-                    break
+        if self.cache_total <= cache_max and len(self._cache) <= max_slots:
+            return
+
+        _evict_candidates = collections.deque(self._cache.values())
+        while _evict_candidates and (self.cache_total > cache_max or len(self._cache) > max_slots):
+            slot = _evict_candidates.popleft()
+            if not slot.ready.is_set():
+                continue
+
+            sz = slot.size()
+            slot.evict()
+            self.cache_total -= sz
+            del self._cache[slot.locator]
 
 
     def cap_cache(self):
         '''Cap the cache size to self.cache_max'''
         with self._cache_updating:
             self._resize_cache(self.cache_max, self._max_slots)
             self._cache_updating.notify_all()
 
     def _get(self, locator):
         # Test if the locator is already in the cache
-        for i in range(0, len(self._cache)):
-            if self._cache[i].locator == locator:
-                n = self._cache[i]
-                if i != 0:
-                    # move it to the front
-                    del self._cache[i]
-                    self._cache.insert(0, n)
-                return n
+        if locator in self._cache:
+            n = self._cache[locator]
+            if n.ready.is_set() and n.content is None:
+                del self._cache[n.locator]
+                return None
+            self._cache.move_to_end(locator)
+            return n
         if self._disk_cache:
             # see if it exists on disk
             n = arvados.diskcache.DiskCacheSlot.get_from_disk(locator, self._disk_cache_dir)
             if n is not None:
-                self._cache.insert(0, n)
+                self._cache[n.locator] = n
+                self.cache_total += n.size()
                 return n
         return None
 
     def get(self, locator):
         with self._cache_lock:
             return self._get(locator)
 
@@ -346,30 +334,31 @@
                     self._cache_updating.wait(timeout=0.2)
                     self._resize_cache(self.cache_max, self._max_slots-1)
 
                 if self._disk_cache:
                     n = arvados.diskcache.DiskCacheSlot(locator, self._disk_cache_dir)
                 else:
                     n = KeepBlockCache.CacheSlot(locator)
-                self._cache.insert(0, n)
+                self._cache[n.locator] = n
                 return n, True
 
     def set(self, slot, blob):
         try:
-            slot.set(blob)
+            if slot.set(blob):
+                self.cache_total += slot.size()
             return
         except OSError as e:
             if e.errno == errno.ENOMEM:
                 # Reduce max slots to current - 4, cap cache and retry
                 with self._cache_lock:
                     self._max_slots = max(4, len(self._cache) - 4)
             elif e.errno == errno.ENOSPC:
                 # Reduce disk max space to current - 256 MiB, cap cache and retry
                 with self._cache_lock:
-                    sm = sum([st.size() for st in self._cache])
+                    sm = sum(st.size() for st in self._cache.values())
                     self.cache_max = max((256 * 1024 * 1024), sm - (256 * 1024 * 1024))
             elif e.errno == errno.ENODEV:
                 _logger.error("Unable to use disk cache: The underlying filesystem does not support memory mapping.")
         except Exception as e:
             pass
         finally:
             # Check if we should evict things from the cache.  Either
@@ -379,15 +368,16 @@
             self.cap_cache()
 
         try:
             # Only gets here if there was an error the first time. The
             # exception handler adjusts limits downward in some cases
             # to free up resources, which would make the operation
             # succeed.
-            slot.set(blob)
+            if slot.set(blob):
+                self.cache_total += slot.size()
         except Exception as e:
             # It failed again.  Give up.
             slot.set(None)
             raise arvados.errors.KeepCacheError("Unable to save block %s to disk cache: %s" % (slot.locator, e))
 
         self.cap_cache()
 
@@ -920,15 +910,18 @@
         self.download_counter = Counter()
         self.put_counter = Counter()
         self.get_counter = Counter()
         self.hits_counter = Counter()
         self.misses_counter = Counter()
         self._storage_classes_unsupported_warning = False
         self._default_classes = []
-        self.num_prefetch_threads = num_prefetch_threads or 2
+        if num_prefetch_threads is not None:
+            self.num_prefetch_threads = num_prefetch_threads
+        else:
+            self.num_prefetch_threads = 2
         self._prefetch_queue = None
         self._prefetch_threads = None
 
         if local_store:
             self.local_store = local_store
             self.head = self.local_store_head
             self.get = self.local_store_get
@@ -1184,14 +1177,16 @@
                         break
                     if prefetch:
                         # this is request for a prefetch to fill in
                         # the cache, don't need to wait for the
                         # result, so if it is already in flight return
                         # immediately.  Clear 'slot' to prevent
                         # finally block from calling slot.set()
+                        if slot.ready.is_set():
+                            slot.get()
                         slot = None
                         return None
 
                     blob = slot.get()
                     if blob is not None:
                         self.hits_counter.add(1)
                         return blob
@@ -1422,14 +1417,17 @@
         """
         This relies on the fact that KeepClient implements a block cache,
         so repeated requests for the same block will not result in repeated
         downloads (unless the block is evicted from the cache.)  This method
         does not block.
         """
 
+        if self.block_cache.get(locator) is not None:
+            return
+
         self._start_prefetch_threads()
         self._prefetch_queue.put(locator)
 
     def stop_prefetch_threads(self):
         with self.lock:
             if self._prefetch_threads is not None:
                 for t in self._prefetch_threads:
```

### Comparing `arvados-python-client-2.7.1/arvados/logging.py` & `arvados-python-client-2.7.2/arvados/logging.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/retry.py` & `arvados-python-client-2.7.2/arvados/retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/safeapi.py` & `arvados-python-client-2.7.2/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/stream.py` & `arvados-python-client-2.7.2/arvados/stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/timer.py` & `arvados-python-client-2.7.2/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/util.py` & `arvados-python-client-2.7.2/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados/vocabulary.py` & `arvados-python-client-2.7.2/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados-v1-discovery.json` & `arvados-python-client-2.7.2/arvados-v1-discovery.json`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.7.2/arvados_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.7.1
+Version: 2.7.2
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.7.1/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.7.2/arvados_python_client.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -67,24 +67,26 @@
 tests/test_arv_ls.py
 tests/test_arv_normalize.py
 tests/test_arv_put.py
 tests/test_arv_ws.py
 tests/test_arvfile.py
 tests/test_benchmark_collections.py
 tests/test_cache.py
+tests/test_cmd_util.py
 tests/test_collections.py
 tests/test_crunch.py
 tests/test_errors.py
 tests/test_events.py
 tests/test_http.py
 tests/test_keep_client.py
 tests/test_keep_locator.py
 tests/test_retry.py
 tests/test_retry_job_helpers.py
 tests/test_safeapi.py
 tests/test_sdk.py
+tests/test_storage_classes.py
 tests/test_stream.py
 tests/test_util.py
 tests/test_vocabulary.py
 tests/performance/__init__.py
 tests/performance/performance_profiler.py
 tests/performance/test_a_sample.py
```

### Comparing `arvados-python-client-2.7.1/arvados_version.py` & `arvados-python-client-2.7.2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/bin/arv-normalize` & `arvados-python-client-2.7.2/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/discovery2pydoc.py` & `arvados-python-client-2.7.2/discovery2pydoc.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/setup.py` & `arvados-python-client-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/arvados_testutil.py` & `arvados-python-client-2.7.2/tests/arvados_testutil.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/keepstub.py` & `arvados-python-client-2.7.2/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/manifest_examples.py` & `arvados-python-client-2.7.2/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/performance/performance_profiler.py` & `arvados-python-client-2.7.2/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/run_test_server.py` & `arvados-python-client-2.7.2/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_api.py` & `arvados-python-client-2.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_copy.py` & `arvados-python-client-2.7.2/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_get.py` & `arvados-python-client-2.7.2/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_keepdocker.py` & `arvados-python-client-2.7.2/tests/test_arv_keepdocker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Copyright (C) The Arvados Authors. All rights reserved.
 #
 # SPDX-License-Identifier: Apache-2.0
 
-from __future__ import absolute_import
 import arvados
 import collections
+import collections.abc
 import copy
 import hashlib
+import logging
 import mock
 import os
 import subprocess
 import sys
 import tempfile
 import unittest
-import logging
+from pathlib import Path
+
+import parameterized
 
 import arvados.commands.keepdocker as arv_keepdocker
 from . import arvados_testutil as tutil
-from . import run_test_server
-
 
 class StopTest(Exception):
     pass
 
 
 class ArvKeepdockerTestCase(unittest.TestCase, tutil.VersionChecker):
     def run_arv_keepdocker(self, args, err, **kwargs):
@@ -222,7 +223,34 @@
             self.run_arv_keepdocker(['--force', 'testimage'], err)
 
         updated_properties = mocked_collection['properties']
         updated_properties.update({'docker-image-repo-tag': 'testimage:latest'})
         api().collections().update.assert_called_with(
             uuid=mocked_collection['uuid'],
             body={'properties': updated_properties})
+
+
+@parameterized.parameterized_class(('filename',), [
+    ('hello-world-ManifestV2.tar',),
+    ('hello-world-ManifestV2-OCILayout.tar',),
+])
+class ImageMetadataTestCase(unittest.TestCase):
+    DATA_PATH = Path(__file__).parent / 'data'
+
+    @classmethod
+    def setUpClass(cls):
+        cls.image_file = (cls.DATA_PATH / cls.filename).open('rb')
+
+    @classmethod
+    def tearDownClass(cls):
+        cls.image_file.close()
+
+    def setUp(self):
+        self.manifest, self.config = arv_keepdocker.load_image_metadata(self.image_file)
+
+    def test_image_manifest(self):
+        self.assertIsInstance(self.manifest, collections.abc.Mapping)
+        self.assertEqual(self.manifest.get('RepoTags'), ['hello-world:latest'])
+
+    def test_image_config(self):
+        self.assertIsInstance(self.config, collections.abc.Mapping)
+        self.assertEqual(self.config.get('created'), '2023-05-02T16:49:27Z')
```

### Comparing `arvados-python-client-2.7.1/tests/test_arv_ls.py` & `arvados-python-client-2.7.2/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_normalize.py` & `arvados-python-client-2.7.2/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_put.py` & `arvados-python-client-2.7.2/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arv_ws.py` & `arvados-python-client-2.7.2/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_arvfile.py` & `arvados-python-client-2.7.2/tests/test_arvfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,14 +627,15 @@
 class ArvadosFileReaderTestCase(StreamFileReaderTestCase):
     class MockParent(object):
         class MockBlockMgr(object):
             def __init__(self, blocks, nocache):
                 self.blocks = blocks
                 self.nocache = nocache
                 self._keep = ArvadosFileWriterTestCase.MockKeep({})
+                self.prefetch_lookahead = 0
 
             def block_prefetch(self, loc):
                 pass
 
             def get_block_contents(self, loc, num_retries=0, cache_only=False):
                 if self.nocache and cache_only:
                     return None
```

### Comparing `arvados-python-client-2.7.1/tests/test_benchmark_collections.py` & `arvados-python-client-2.7.2/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_cache.py` & `arvados-python-client-2.7.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_collections.py` & `arvados-python-client-2.7.2/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_crunch.py` & `arvados-python-client-2.7.2/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_errors.py` & `arvados-python-client-2.7.2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_events.py` & `arvados-python-client-2.7.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_http.py` & `arvados-python-client-2.7.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_keep_client.py` & `arvados-python-client-2.7.2/tests/test_keep_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from future import standard_library
 standard_library.install_aliases()
 from builtins import str
 from builtins import range
 from builtins import object
 import hashlib
 import mock
+from mock import patch
 import os
 import errno
 import pycurl
 import random
 import re
 import shutil
 import socket
 import sys
 import stat
 import tempfile
 import time
 import unittest
 import urllib.parse
+import mmap
 
 import parameterized
 
 import arvados
 import arvados.retry
 import arvados.util
 from . import arvados_testutil as tutil
@@ -621,130 +623,14 @@
         self.assertEqual(b'first response', head_resp)
         # First reponse was not cached because it was from a HEAD request.
         self.assertNotEqual(head_resp, get_resp)
 
 
 
 
-@tutil.skip_sleep
-@parameterized.parameterized_class([{"disk_cache": True}, {"disk_cache": False}])
-class KeepStorageClassesTestCase(unittest.TestCase, tutil.ApiClientMock, DiskCacheBase):
-    disk_cache = False
-
-    def setUp(self):
-        self.api_client = self.mock_keep_services(count=2)
-        self.keep_client = arvados.KeepClient(api_client=self.api_client, block_cache=self.make_block_cache(self.disk_cache))
-        self.data = b'xyzzy'
-        self.locator = '1271ed5ef305aadabc605b1609e24c52'
-
-    def tearDown(self):
-        DiskCacheBase.tearDown(self)
-
-    def test_multiple_default_storage_classes_req_header(self):
-        api_mock = self.api_client_mock()
-        api_mock.config.return_value = {
-            'StorageClasses': {
-                'foo': { 'Default': True },
-                'bar': { 'Default': True },
-                'baz': { 'Default': False }
-            }
-        }
-        api_client = self.mock_keep_services(api_mock=api_mock, count=2)
-        keep_client = arvados.KeepClient(api_client=api_client, block_cache=self.make_block_cache(self.disk_cache))
-        resp_hdr = {
-            'x-keep-storage-classes-confirmed': 'foo=1, bar=1',
-            'x-keep-replicas-stored': 1
-        }
-        with tutil.mock_keep_responses(self.locator, 200, **resp_hdr) as mock:
-            keep_client.put(self.data, copies=1)
-            req_hdr = mock.responses[0]
-            self.assertIn(
-                'X-Keep-Storage-Classes: bar, foo', req_hdr.getopt(pycurl.HTTPHEADER))
-
-    def test_storage_classes_req_header(self):
-        self.assertEqual(
-            self.api_client.config()['StorageClasses'],
-            {'default': {'Default': True}})
-        cases = [
-            # requested, expected
-            [['foo'], 'X-Keep-Storage-Classes: foo'],
-            [['bar', 'foo'], 'X-Keep-Storage-Classes: bar, foo'],
-            [[], 'X-Keep-Storage-Classes: default'],
-            [None, 'X-Keep-Storage-Classes: default'],
-        ]
-        for req_classes, expected_header in cases:
-            headers = {'x-keep-replicas-stored': 1}
-            if req_classes is None or len(req_classes) == 0:
-                confirmed_hdr = 'default=1'
-            elif len(req_classes) > 0:
-                confirmed_hdr = ', '.join(["{}=1".format(cls) for cls in req_classes])
-            headers.update({'x-keep-storage-classes-confirmed': confirmed_hdr})
-            with tutil.mock_keep_responses(self.locator, 200, **headers) as mock:
-                self.keep_client.put(self.data, copies=1, classes=req_classes)
-                req_hdr = mock.responses[0]
-                self.assertIn(expected_header, req_hdr.getopt(pycurl.HTTPHEADER))
-
-    def test_partial_storage_classes_put(self):
-        headers = {
-            'x-keep-replicas-stored': 1,
-            'x-keep-storage-classes-confirmed': 'foo=1'}
-        with tutil.mock_keep_responses(self.locator, 200, 503, **headers) as mock:
-            with self.assertRaises(arvados.errors.KeepWriteError):
-                self.keep_client.put(self.data, copies=1, classes=['foo', 'bar'], num_retries=0)
-            # 1st request, both classes pending
-            req1_headers = mock.responses[0].getopt(pycurl.HTTPHEADER)
-            self.assertIn('X-Keep-Storage-Classes: bar, foo', req1_headers)
-            # 2nd try, 'foo' class already satisfied
-            req2_headers = mock.responses[1].getopt(pycurl.HTTPHEADER)
-            self.assertIn('X-Keep-Storage-Classes: bar', req2_headers)
-
-    def test_successful_storage_classes_put_requests(self):
-        cases = [
-            # wanted_copies, wanted_classes, confirmed_copies, confirmed_classes, expected_requests
-            [ 1, ['foo'], 1, 'foo=1', 1],
-            [ 1, ['foo'], 2, 'foo=2', 1],
-            [ 2, ['foo'], 2, 'foo=2', 1],
-            [ 2, ['foo'], 1, 'foo=1', 2],
-            [ 1, ['foo', 'bar'], 1, 'foo=1, bar=1', 1],
-            [ 1, ['foo', 'bar'], 2, 'foo=2, bar=2', 1],
-            [ 2, ['foo', 'bar'], 2, 'foo=2, bar=2', 1],
-            [ 2, ['foo', 'bar'], 1, 'foo=1, bar=1', 2],
-            [ 1, ['foo', 'bar'], 1, None, 1],
-            [ 1, ['foo'], 1, None, 1],
-            [ 2, ['foo'], 2, None, 1],
-            [ 2, ['foo'], 1, None, 2],
-        ]
-        for w_copies, w_classes, c_copies, c_classes, e_reqs in cases:
-            headers = {'x-keep-replicas-stored': c_copies}
-            if c_classes is not None:
-                headers.update({'x-keep-storage-classes-confirmed': c_classes})
-            with tutil.mock_keep_responses(self.locator, 200, 200, **headers) as mock:
-                case_desc = 'wanted_copies={}, wanted_classes="{}", confirmed_copies={}, confirmed_classes="{}", expected_requests={}'.format(w_copies, ', '.join(w_classes), c_copies, c_classes, e_reqs)
-                self.assertEqual(self.locator,
-                    self.keep_client.put(self.data, copies=w_copies, classes=w_classes),
-                    case_desc)
-                self.assertEqual(e_reqs, mock.call_count, case_desc)
-
-    def test_failed_storage_classes_put_requests(self):
-        cases = [
-            # wanted_copies, wanted_classes, confirmed_copies, confirmed_classes, return_code
-            [ 1, ['foo'], 1, 'bar=1', 200],
-            [ 1, ['foo'], 1, None, 503],
-            [ 2, ['foo'], 1, 'bar=1, foo=0', 200],
-            [ 3, ['foo'], 1, 'bar=1, foo=1', 200],
-            [ 3, ['foo', 'bar'], 1, 'bar=2, foo=1', 200],
-        ]
-        for w_copies, w_classes, c_copies, c_classes, return_code in cases:
-            headers = {'x-keep-replicas-stored': c_copies}
-            if c_classes is not None:
-                headers.update({'x-keep-storage-classes-confirmed': c_classes})
-            with tutil.mock_keep_responses(self.locator, return_code, return_code, **headers):
-                case_desc = 'wanted_copies={}, wanted_classes="{}", confirmed_copies={}, confirmed_classes="{}"'.format(w_copies, ', '.join(w_classes), c_copies, c_classes)
-                with self.assertRaises(arvados.errors.KeepWriteError, msg=case_desc):
-                    self.keep_client.put(self.data, copies=w_copies, classes=w_classes, num_retries=0)
 
 @tutil.skip_sleep
 @parameterized.parameterized_class([{"disk_cache": True}, {"disk_cache": False}])
 class KeepXRequestIdTestCase(unittest.TestCase, tutil.ApiClientMock, DiskCacheBase):
     disk_cache = False
 
     def setUp(self):
@@ -1753,51 +1639,71 @@
 
         # Cache fails
         with self.assertRaises(arvados.errors.KeepCacheError):
             with tutil.mock_keep_responses(self.data, 200) as mock:
                 keep_client.get(self.locator)
 
 
-    @mock.patch('mmap.mmap')
-    def test_disk_cache_retry_write_error(self, mockmmap):
+    def test_disk_cache_retry_write_error(self):
         block_cache = arvados.keep.KeepBlockCache(disk_cache=True,
                                                   disk_cache_dir=self.disk_cache_dir)
 
         keep_client = arvados.KeepClient(api_client=self.api_client, block_cache=block_cache)
 
-        mockmmap.side_effect = (OSError(errno.ENOSPC, "no space"), self.data)
+        called = False
+        realmmap = mmap.mmap
+        def sideeffect_mmap(*args, **kwargs):
+            nonlocal called
+            if not called:
+                called = True
+                raise OSError(errno.ENOSPC, "no space")
+            else:
+                return realmmap(*args, **kwargs)
 
-        cache_max_before = block_cache.cache_max
+        with patch('mmap.mmap') as mockmmap:
+            mockmmap.side_effect = sideeffect_mmap
 
-        with tutil.mock_keep_responses(self.data, 200) as mock:
-            self.assertTrue(tutil.binary_compare(keep_client.get(self.locator), self.data))
+            cache_max_before = block_cache.cache_max
 
-        self.assertIsNotNone(keep_client.get_from_cache(self.locator))
+            with tutil.mock_keep_responses(self.data, 200) as mock:
+                self.assertTrue(tutil.binary_compare(keep_client.get(self.locator), self.data))
+
+            self.assertIsNotNone(keep_client.get_from_cache(self.locator))
 
         with open(os.path.join(self.disk_cache_dir, self.locator[0:3], self.locator+".keepcacheblock"), "rb") as f:
             self.assertTrue(tutil.binary_compare(f.read(), self.data))
 
         # shrank the cache in response to ENOSPC
         self.assertTrue(cache_max_before > block_cache.cache_max)
 
 
-    @mock.patch('mmap.mmap')
-    def test_disk_cache_retry_write_error2(self, mockmmap):
+    def test_disk_cache_retry_write_error2(self):
         block_cache = arvados.keep.KeepBlockCache(disk_cache=True,
                                                   disk_cache_dir=self.disk_cache_dir)
 
         keep_client = arvados.KeepClient(api_client=self.api_client, block_cache=block_cache)
 
-        mockmmap.side_effect = (OSError(errno.ENOMEM, "no memory"), self.data)
+        called = False
+        realmmap = mmap.mmap
+        def sideeffect_mmap(*args, **kwargs):
+            nonlocal called
+            if not called:
+                called = True
+                raise OSError(errno.ENOMEM, "no memory")
+            else:
+                return realmmap(*args, **kwargs)
 
-        slots_before = block_cache._max_slots
+        with patch('mmap.mmap') as mockmmap:
+            mockmmap.side_effect = sideeffect_mmap
 
-        with tutil.mock_keep_responses(self.data, 200) as mock:
-            self.assertTrue(tutil.binary_compare(keep_client.get(self.locator), self.data))
+            slots_before = block_cache._max_slots
 
-        self.assertIsNotNone(keep_client.get_from_cache(self.locator))
+            with tutil.mock_keep_responses(self.data, 200) as mock:
+                self.assertTrue(tutil.binary_compare(keep_client.get(self.locator), self.data))
+
+            self.assertIsNotNone(keep_client.get_from_cache(self.locator))
 
         with open(os.path.join(self.disk_cache_dir, self.locator[0:3], self.locator+".keepcacheblock"), "rb") as f:
             self.assertTrue(tutil.binary_compare(f.read(), self.data))
 
         # shrank the cache in response to ENOMEM
         self.assertTrue(slots_before > block_cache._max_slots)
```

### Comparing `arvados-python-client-2.7.1/tests/test_keep_locator.py` & `arvados-python-client-2.7.2/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_retry.py` & `arvados-python-client-2.7.2/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_retry_job_helpers.py` & `arvados-python-client-2.7.2/tests/test_retry_job_helpers.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_safeapi.py` & `arvados-python-client-2.7.2/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_sdk.py` & `arvados-python-client-2.7.2/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_stream.py` & `arvados-python-client-2.7.2/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_util.py` & `arvados-python-client-2.7.2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.7.1/tests/test_vocabulary.py` & `arvados-python-client-2.7.2/tests/test_vocabulary.py`

 * *Files identical despite different names*

