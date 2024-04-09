# Comparing `tmp/reqless-0.13.1.tar.gz` & `tmp/reqless-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqless-0.13.1.tar", last modified: Sun Apr  7 00:45:31 2024, max compression
+gzip compressed data, was "reqless-0.13.2.tar", last modified: Tue Apr  9 17:25:42 2024, max compression
```

## Comparing `reqless-0.13.1.tar` & `reqless-0.13.2.tar`

### file list

```diff
@@ -1,105 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.099907 reqless-0.13.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.079908 reqless-0.13.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/main-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/other-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 00:44:24.000000 reqless-0.13.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-07 00:44:24.000000 reqless-0.13.1/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.079908 reqless-0.13.1/.meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/.meta/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-07 00:45:27.000000 reqless-0.13.1/.meta/coverage/badge.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-07 00:45:27.000000 reqless-0.13.1/.meta/coverage/report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-07 00:44:24.000000 reqless-0.13.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-07 00:44:24.000000 reqless-0.13.1/.safety-policy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-07 00:44:24.000000 reqless-0.13.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 00:44:24.000000 reqless-0.13.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-07 00:45:31.099907 reqless-0.13.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20235 2024-04-07 00:44:24.000000 reqless-0.13.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-07 00:44:24.000000 reqless-0.13.1/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-07 00:44:24.000000 reqless-0.13.1/bin/reqless-py-worker
--rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-07 00:44:24.000000 reqless-0.13.1/forgetful-bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-07 00:44:24.000000 reqless-0.13.1/provision.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-07 00:44:24.000000 reqless-0.13.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.087907 reqless-0.13.1/qmore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.087907 reqless-0.13.1/reqless/
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-07 00:45:30.000000 reqless-0.13.1/reqless/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/lua/
--rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-04-07 00:45:19.000000 reqless-0.13.1/reqless/lua/qless-lib.lua
--rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-04-07 00:45:19.000000 reqless-0.13.1/reqless/lua/qless.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/proctitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/queue_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.095908 reqless-0.13.1/reqless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.095908 reqless-0.13.1/reqless_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_job_processor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_worker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-07 00:45:01.000000 reqless-0.13.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:45:31.099907 reqless-0.13.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 00:44:24.000000 reqless-0.13.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-07 00:44:24.000000 reqless-0.13.1/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.596715 reqless-0.13.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.576715 reqless-0.13.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 17:24:38.000000 reqless-0.13.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 17:24:38.000000 reqless-0.13.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 17:24:38.000000 reqless-0.13.2/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.576715 reqless-0.13.2/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-09 17:25:39.000000 reqless-0.13.2/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-09 17:25:39.000000 reqless-0.13.2/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-09 17:24:38.000000 reqless-0.13.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 17:24:38.000000 reqless-0.13.2/.safety-policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-09 17:24:38.000000 reqless-0.13.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 17:24:38.000000 reqless-0.13.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-04-09 17:25:42.596715 reqless-0.13.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-09 17:24:38.000000 reqless-0.13.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 17:24:38.000000 reqless-0.13.2/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-09 17:24:38.000000 reqless-0.13.2/bin/reqless-py-worker
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-09 17:24:38.000000 reqless-0.13.2/forgetful-bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-09 17:24:38.000000 reqless-0.13.2/provision.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-09 17:24:38.000000 reqless-0.13.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.580715 reqless-0.13.2/reqless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.584715 reqless-0.13.2/reqless/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_job_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/abstract/abstract_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16499 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.584715 reqless-0.13.2/reqless/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-04-09 17:25:33.000000 reqless-0.13.2/reqless/lua/qless-lib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-04-09 17:25:33.000000 reqless-0.13.2/reqless/lua/qless.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/proctitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/qmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/qmore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/queue_resolvers/transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.588715 reqless-0.13.2/reqless/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.592715 reqless-0.13.2/reqless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 17:25:42.000000 reqless-0.13.2/reqless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:25:42.592715 reqless-0.13.2/reqless_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_job_processor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-09 17:24:38.000000 reqless-0.13.2/reqless_test/test_worker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-09 17:25:15.000000 reqless-0.13.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:25:42.596715 reqless-0.13.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-09 17:24:38.000000 reqless-0.13.2/whitelist.txt
```

### Comparing `reqless-0.13.1/.github/workflows/main-branch.yaml` & `reqless-0.13.2/.github/workflows/main-branch.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         uses: actions/checkout@v3
         with:
           submodules: true
           token: ${{ secrets.PAT_GITHUB_ACTIONS }}
 
       - uses: actions/setup-python@v4
         with:
+          cache: pip
           python-version: '3.9'
 
       - name: Install dependencies
         run: |
           sudo apt-get update && sudo apt-get install -y redis-server
           python -m venv venv
           source venv/bin/activate
@@ -50,15 +51,15 @@
             git diff
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
-          make nose
+          make test-with-coverage
           coverage report | tee .meta/coverage/report.txt
           coverage-badge -f -o .meta/coverage/badge.svg
           python -m build
 
       - name: Checkout tdg5/github-action-pack
         uses: actions/checkout@v4
         with:
```

### Comparing `reqless-0.13.1/.github/workflows/other-branch.yaml` & `reqless-0.13.2/.github/workflows/other-branch.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
       - name: Check out code
         uses: actions/checkout@v3
         with:
           submodules: true
 
       - uses: actions/setup-python@v4
         with:
+          cache: pip
           python-version: '3.9'
 
       - name: Install dependencies
         run: |
           sudo apt-get update && sudo apt-get install -y redis-server
           python -m venv venv
           source venv/bin/activate
@@ -45,10 +46,10 @@
             echo "make style caused file changes, failing!"
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
-          make nose
+          make test-with-coverage
           coverage report
           python -m build
```

### Comparing `reqless-0.13.1/.github/workflows/release.yaml` & `reqless-0.13.2/.github/workflows/release.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         uses: actions/checkout@v3
         with:
           submodules: true
           token: ${{ secrets.PAT_GITHUB_ACTIONS }}
 
       - uses: actions/setup-python@v4
         with:
+          cache: pip
           python-version: '3.9'
 
       - name: Install dependencies
         run: |
           sudo apt-get update && sudo apt-get install -y redis-server
           python -m venv venv
           source venv/bin/activate
@@ -56,15 +57,15 @@
             git diff
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
-          make nose
+          make test-with-coverage
           coverage report | tee .meta/coverage/report.txt
           coverage-badge -f -o .meta/coverage/badge.svg
           export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_REQLESS="$VERSION"
           python -m build
 
       - name: Publish package to pypi
         env:
```

### Comparing `reqless-0.13.1/.meta/coverage/badge.svg` & `reqless-0.13.2/.meta/coverage/badge.svg`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/.pre-commit-config.yaml` & `reqless-0.13.2/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,47 +7,47 @@
 repos:
   - repo: local
     hooks:
       - id: black
         name: black
         language: system
         entry: black
-        args: ["reqless", "qmore", "reqless_test"]
+        args: ["reqless", "reqless_test"]
         types: [python]
       - id: flake8
         name: flake8
         language: python
         entry: flake8p
-        args: ["reqless", "qmore", "reqless_test"]
+        args: ["reqless", "reqless_test"]
         types: [python]
         additional_dependencies:
           - darglint
           - dlint
           - flake8-comprehensions
           - flake8-eradicate
           - flake8-spellcheck
           - flake8-typing-imports
           - mccabe
           - pep8-naming
       - id: mypy
         name: Mypy check
         entry: mypy
         language: system
-        args: ["reqless", "qmore", "reqless_test"]
+        args: ["reqless", "reqless_test"]
         pass_filenames: false
       - id: isort
         name: isort
         entry: isort
-        args: ["reqless", "qmore", "reqless_test"]
+        args: ["reqless", "reqless_test"]
         language: system
       - id: removestar
         name: removestar
         language: system
         entry: removestar
-        args: ["-i", "reqless", "qmore", "reqless_test"]
+        args: ["-i", "reqless", "reqless_test"]
         types: [python]
       - id: safety-production-dependencies-check
         name: Safety production dependencies check
         entry: safety
         args: [check, --policy-file=.safety-policy.yaml, --full-report, --file]
         language: system
         files: requirements.txt
```

### Comparing `reqless-0.13.1/LICENSE` & `reqless-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/PKG-INFO` & `reqless-0.13.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.1
+Version: 0.13.2
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
-Keywords: job,qless,redis,reqless
+Keywords: job,qless,qmore,redis,reqless
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
@@ -24,28 +24,30 @@
 Requires-Dist: redis
 Requires-Dist: typing_extensions>=4.8.0
 Provides-Extra: dev
 Requires-Dist: black~=24.2.0; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: gevent~=24.2.1; extra == "dev"
 Requires-Dist: isort~=5.8.0; extra == "dev"
-Requires-Dist: mypy~=1.7.0; extra == "dev"
+Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
+Requires-Dist: setproctitle~=1.3.3; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
 Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
+Requires-Dist: types-redis~=4.6.0.11; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge~=1.1.0; extra == "test"
 Requires-Dist: mock; extra == "test"
-Requires-Dist: nose; extra == "test"
-Requires-Dist: rednose; extra == "test"
+Requires-Dist: pytest~=7.4.0; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
 [![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
 
@@ -125,15 +127,15 @@
 
 ```bash
 git clone git://github.com/tdg5/reqless-py.git
 cd reqless-py
 # qless-core is a submodule
 git submodule init
 git submodule update
-sudo python setup.py install
+pip install .
 ```
 
 ## Business Time!
 
 You've read this far -- you probably want to write some code now and turn them
 into jobs. Jobs are described essentially by two pieces of information -- a
 `class` and `data`. The class should have static methods that know how to
```

### Comparing `reqless-0.13.1/README.md` & `reqless-0.13.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 ```bash
 git clone git://github.com/tdg5/reqless-py.git
 cd reqless-py
 # qless-core is a submodule
 git submodule init
 git submodule update
-sudo python setup.py install
+pip install .
 ```
 
 ## Business Time!
 
 You've read this far -- you probably want to write some code now and turn them
 into jobs. Jobs are described essentially by two pieces of information -- a
 `class` and `data`. The class should have static methods that know how to
```

### Comparing `reqless-0.13.1/bin/reqless-py-worker` & `reqless-0.13.2/bin/reqless-py-worker`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/forgetful-bench.py` & `reqless-0.13.2/forgetful-bench.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/provision.sh` & `reqless-0.13.2/provision.sh`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/pyproject.toml` & `reqless-0.13.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=69",
   "setuptools-scm>=8.0.4",
-
 ]
 
 [project]
 authors = [{name = "Danny Guinther"}]
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
@@ -25,67 +24,82 @@
   "typing_extensions>=4.8.0",
 ]
 description = "Redis-based Queue Management"
 dynamic = ["version"]
 keywords = [
     "job",
     "qless",
+    "qmore",
     "redis",
     "reqless",
 ]
 license = {text = "MIT"}
 name = "reqless"
 readme = "README.md"
 requires-python = ">3.9.0"
 
 [project.optional-dependencies]
 dev = [
   "black~=24.2.0",
   "build~=1.0.3",
   "flake8-pyproject~=1.2.3",
   "flake8~=7.0.0",
+  "gevent~=24.2.1",
   "isort~=5.8.0",
-  "mypy~=1.7.0",
+  "mypy~=1.8.0",
   "pre-commit~=2.20.0",
   "removestar~=1.3.1",
   "safety==2.3.4",
+  "setproctitle~=1.3.3",
   "twine~=4.0.2",
   "types-decorator~=5.1.8.4",
   "types-mock~=5.1.0.2",
+  "types-redis~=4.6.0.11",
 ]
 test = [
     "coverage",
     "coverage-badge~=1.1.0",
     "mock",
-    "nose",
-    "rednose",
+    "pytest~=7.4.0",
     "setuptools>=69",
 ]
 all = ["reqless[dev,test]"]
 
 [project.urls]
 Homepage = "https://github.com/tdg5/reqless-py"
 Source = "https://github.com/tdg5/reqless-py"
 Tracker = "https://github.com/tdg5/reqless-py/issues"
 
 [tool.black]
 exclude = "reqless/(lua|qless-core)/.*"
-include = "(reqless(_test)?|qmore)/.*\\.py$"
+include = "(reqless(_test)?)/.*\\.py$"
 line-length = 88
 target-version = ["py39"]
 
+[tool.coverage.run]
+omit = [
+  "reqless/__version__.py",
+  "reqless/profile.py",
+]
+source = [
+  "reqless",
+]
+
+[tool.coverage.report]
+fail_under = 98
+
 [tool.flake8]
 exclude = ["reqless/lua", "reqless/qless-core"]
 ignore = ["E203", "E251", "E701", "N805", "W503", "DAR101", "DAR201", "DAR301", "DAR401"]
 max-line-length = 88
 min_python_version = "3.9.0"
 
 [tool.isort]
 include_trailing_comma = true
-known_first_party = ["reqless", "qmore", "reqless_test"]
+known_first_party = ["reqless", "reqless_test"]
 line_length = 88
 lines_after_imports = 2
 multi_line_output = 3
 profile = "black"
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 skip_glob = ["reqless/lua", "reqless/qless-core"]
 use_parentheses = true
@@ -96,39 +110,33 @@
 disallow_untyped_defs = true
 exclude = "^(reqless/qless-core|reqless/lua|fixtures|.*?\\.js|.*?\\.json)"
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_ignores = true
 
-[tool.nosetests]
-cover-branches = 1
-cover-erase = 1
-cover-min-percentage = 98
-cover-package = ["reqless", "qmore"]
-exe = 1
-logging-clear-handlers = 1
-rednose = 1
-verbosity = 2
-
 [tool.pytest.ini_options]
 markers = ["integration_test: marks tests as integration tests (deselect with '-m \"not integration_test\"')"]
+norecursedirs = [
+  "reqless/lua",
+  "reqless/qless-core",
+]
+testpaths = ["reqless_test"]
 
 [tool.setuptools]
 script-files = ["bin/reqless-py-worker"]
 
 [tool.setuptools.package-data]
 "reqless" = ["lua/*.lua", "py.typed"]
-"qmore" = ["py.typed"]
 
 [tool.setuptools.packages.find]
 include = [
-  "qmore",
   "reqless",
   "reqless.abstract",
+  "reqless.qmore",
   "reqless.queue_resolvers",
   "reqless.workers",
 ]
 where = ["."]
 
 [tool.setuptools_scm]
 version_file = "reqless/__version__.py"
```

### Comparing `reqless-0.13.1/qmore/client.py` & `reqless-0.13.2/reqless/qmore/client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/__init__.py` & `reqless-0.13.2/reqless/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/__init__.py` & `reqless-0.13.2/reqless/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_client.py` & `reqless-0.13.2/reqless/abstract/abstract_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_config.py` & `reqless-0.13.2/reqless/abstract/abstract_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_job.py` & `reqless-0.13.2/reqless/abstract/abstract_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_job_processor.py` & `reqless-0.13.2/reqless/abstract/abstract_job_processor.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_jobs.py` & `reqless-0.13.2/reqless/abstract/abstract_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_queue.py` & `reqless-0.13.2/reqless/abstract/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_queue_jobs.py` & `reqless-0.13.2/reqless/abstract/abstract_queue_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/abstract/abstract_throttle.py` & `reqless-0.13.2/reqless/abstract/abstract_throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/config.py` & `reqless-0.13.2/reqless/config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/importer.py` & `reqless-0.13.2/reqless/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,11 +34,11 @@
             Importer._loaded[class_name] = time.time()
         if hasattr(mod, "__file__") and mod.__file__:
             try:
                 mtime = os.stat(mod.__file__).st_mtime
                 if Importer._loaded[class_name] < mtime:
                     mod = importlib.reload(mod)
             except OSError:
-                logger.warn("Could not check modification time of %s", mod.__file__)
+                logger.warning("Could not check modification time of %s", mod.__file__)
 
         _class: Type = getattr(mod, class_name.rpartition(".")[2])
         return _class
```

### Comparing `reqless-0.13.1/reqless/job.py` & `reqless-0.13.2/reqless/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
         The motivation behind the `type` is so that similar errors can be
         grouped together. Optionally, updated data can be provided for the job.
         A job in any state can be marked as failed. If it has been given to a
         worker as a job, then its subsequent requests to heartbeat or complete
         that job will fail. Failed jobs are kept until they are canceled or
         completed. __Returns__ the id of the failed job if successful, or
         `False` on failure."""
-        logger.warn("Failing %s (%s): %s", self.jid, group, message)
+        logger.warning("Failing %s (%s): %s", self.jid, group, message)
         response: bool = self.client(
             "fail",
             self.jid,
             self.client.worker_name,
             group,
             message,
             self.data,
```

### Comparing `reqless-0.13.1/reqless/listener.py` & `reqless-0.13.2/reqless/listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/lua/qless-lib.lua` & `reqless-0.13.2/reqless/lua/qless-lib.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/lua/qless.lua` & `reqless-0.13.2/reqless/lua/qless.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/profile.py` & `reqless-0.13.2/reqless/profile.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/queue.py` & `reqless-0.13.2/reqless/queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/queue_resolvers/__init__.py` & `reqless-0.13.2/reqless/queue_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from datetime import datetime, timedelta, timezone
 from typing import Dict, List, Optional
 
-from qmore.client import QmoreClient
 from reqless import Client
 from reqless.abstract import AbstractQueueIdentifiersTransformer
+from reqless.qmore.client import QmoreClient
 
 
 class QmoreDynamicMappingQueueIdentifiersTransformer(
     AbstractQueueIdentifiersTransformer
 ):
     def __init__(
         self,
```

### Comparing `reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.2/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from datetime import datetime, timedelta, timezone
 from random import SystemRandom
 from typing import List, Optional
 
-from qmore.client import QmoreClient, QueuePriorityPattern
 from reqless import Client
 from reqless.abstract import AbstractQueueIdentifiersTransformer
+from reqless.qmore.client import QmoreClient, QueuePriorityPattern
 
 
 class QmoreDynamicPriorityQueueIdentifiersTransformer(
     AbstractQueueIdentifiersTransformer
 ):
     def __init__(
         self,
```

### Comparing `reqless-0.13.1/reqless/queue_resolvers/transforming_queue_resolver.py` & `reqless-0.13.2/reqless/queue_resolvers/transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/throttle.py` & `reqless-0.13.2/reqless/throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/workers/forking.py` & `reqless-0.13.2/reqless/workers/forking.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,27 @@
         self.count: int = self.kwargs.pop("workers", 0) or NUM_CPUS
         # A dictionary of child pids to information about them
         self.sandboxes: Dict[int, str] = {}
 
     def stop(self, sig: int = signal.SIGINT) -> None:
         """Stop all the workers, and then wait for them"""
         for cpid in self.sandboxes:
-            logger.warn("Stopping %i..." % cpid)
+            logger.warning("Stopping %i..." % cpid)
             try:
                 os.kill(cpid, sig)
             except OSError:  # pragma: no cover
                 logger.exception("Error stopping %s..." % cpid)
 
         # While we still have children running, wait for them
         # We edit the dictionary during the loop, so we need to copy its keys
         for cpid in list(self.sandboxes):
             try:
                 logger.info("Waiting for %i..." % cpid)
                 pid, status = os.waitpid(cpid, 0)
-                logger.warn("%i stopped with status %i" % (pid, status >> 8))
+                logger.warning("%i stopped with status %i" % (pid, status >> 8))
             except OSError:  # pragma: no cover
                 logger.exception("Error waiting for %i..." % cpid)
             finally:
                 self.sandboxes.pop(cpid, None)
 
     def spawn(self, **kwargs: Any) -> Worker:
         """Return a new worker for a child process"""
@@ -104,15 +104,15 @@
                         logger.exception("Exception in spawned worker")
                     finally:
                         os._exit(0)
 
         try:
             while not self.shutdown:
                 pid, status = os.wait()
-                logger.warn(
+                logger.warning(
                     "Worker %i died with status %i from signal %i"
                     % (pid, status >> 8, status & 0xFF)
                 )
                 sandbox = self.sandboxes.pop(pid)
                 cpid = os.fork()
                 if cpid:
                     logger.info("Spawned replacement worker %i" % cpid)
```

### Comparing `reqless-0.13.1/reqless/workers/greenlet.py` & `reqless-0.13.2/reqless/workers/greenlet.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self.greenlets.pop(job.jid, None)
             self.sandboxes.append(sandbox)
 
     def kill(self, jid: str) -> None:
         """Stop the greenlet processing the provided jid"""
         greenlet = self.greenlets.get(jid)
         if greenlet is not None:
-            logger.warn("Lost ownership of %s" % jid)
+            logger.warning("Lost ownership of %s" % jid)
             greenlet.kill()
 
     def run(self) -> None:
         """Work on jobs"""
         # Register signal handlers
         self.signals()
```

### Comparing `reqless-0.13.1/reqless/workers/serial.py` & `reqless-0.13.2/reqless/workers/serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/workers/util.py` & `reqless-0.13.2/reqless/workers/util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless/workers/worker.py` & `reqless-0.13.2/reqless/workers/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             # QUIT - Finish processing, but don't do any more work after that
             self.stop()
         elif signum == signal.SIGUSR1:
             # USR1 - Print the backtrace
             message = "".join(traceback.format_stack(frame))
             message = "Signaled traceback for %s:\n%s" % (os.getpid(), message)
             print(message, file=sys.stderr)
-            logger.warn(message)
+            logger.warning(message)
         elif signum == signal.SIGUSR2:
             # USR2 - Enter a debugger
             # Much thanks to http://stackoverflow.com/questions/132058
             data = {"_frame": frame}  # Allow access to frame object.
             if frame:
                 data.update(frame.f_globals)  # Unless shadowed by global
                 data.update(frame.f_locals)
```

### Comparing `reqless-0.13.1/reqless.egg-info/PKG-INFO` & `reqless-0.13.2/reqless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.1
+Version: 0.13.2
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
-Keywords: job,qless,redis,reqless
+Keywords: job,qless,qmore,redis,reqless
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
@@ -24,28 +24,30 @@
 Requires-Dist: redis
 Requires-Dist: typing_extensions>=4.8.0
 Provides-Extra: dev
 Requires-Dist: black~=24.2.0; extra == "dev"
 Requires-Dist: build~=1.0.3; extra == "dev"
 Requires-Dist: flake8-pyproject~=1.2.3; extra == "dev"
 Requires-Dist: flake8~=7.0.0; extra == "dev"
+Requires-Dist: gevent~=24.2.1; extra == "dev"
 Requires-Dist: isort~=5.8.0; extra == "dev"
-Requires-Dist: mypy~=1.7.0; extra == "dev"
+Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
+Requires-Dist: setproctitle~=1.3.3; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
 Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
+Requires-Dist: types-redis~=4.6.0.11; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge~=1.1.0; extra == "test"
 Requires-Dist: mock; extra == "test"
-Requires-Dist: nose; extra == "test"
-Requires-Dist: rednose; extra == "test"
+Requires-Dist: pytest~=7.4.0; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
 [![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
 
@@ -125,15 +127,15 @@
 
 ```bash
 git clone git://github.com/tdg5/reqless-py.git
 cd reqless-py
 # qless-core is a submodule
 git submodule init
 git submodule update
-sudo python setup.py install
+pip install .
 ```
 
 ## Business Time!
 
 You've read this far -- you probably want to write some code now and turn them
 into jobs. Jobs are described essentially by two pieces of information -- a
 `class` and `data`. The class should have static methods that know how to
```

### Comparing `reqless-0.13.1/reqless.egg-info/SOURCES.txt` & `reqless-0.13.2/reqless.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,21 @@
 Makefile
 README.md
 Vagrantfile
 forgetful-bench.py
 provision.sh
 pyproject.toml
 requirements.txt
-tox.ini
 whitelist.txt
 .github/workflows/main-branch.yaml
 .github/workflows/other-branch.yaml
 .github/workflows/release.yaml
 .meta/coverage/badge.svg
 .meta/coverage/report.txt
 bin/reqless-py-worker
-qmore/__init__.py
-qmore/client.py
-qmore/py.typed
 reqless/__init__.py
 reqless/__version__.py
 reqless/config.py
 reqless/exceptions.py
 reqless/importer.py
 reqless/job.py
 reqless/listener.py
@@ -53,14 +49,16 @@
 reqless/abstract/abstract_queue_resolver.py
 reqless/abstract/abstract_queues.py
 reqless/abstract/abstract_throttle.py
 reqless/abstract/abstract_throttles.py
 reqless/abstract/abstract_workers.py
 reqless/lua/qless-lib.lua
 reqless/lua/qless.lua
+reqless/qmore/__init__.py
+reqless/qmore/client.py
 reqless/queue_resolvers/__init__.py
 reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
 reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
 reqless/queue_resolvers/transforming_queue_resolver.py
 reqless/workers/__init__.py
 reqless/workers/forking.py
 reqless/workers/greenlet.py
```

### Comparing `reqless-0.13.1/reqless_test/common.py` & `reqless-0.13.2/reqless_test/common.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_client.py` & `reqless-0.13.2/reqless_test/test_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_config.py` & `reqless-0.13.2/reqless_test/test_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_events.py` & `reqless-0.13.2/reqless_test/test_events.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_forking.py` & `reqless-0.13.2/reqless_test/test_forking.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_greenlet.py` & `reqless-0.13.2/reqless_test/test_greenlet.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_importer.py` & `reqless-0.13.2/reqless_test/test_importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_job.py` & `reqless-0.13.2/reqless_test/test_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_job_processor_api.py` & `reqless-0.13.2/reqless_test/test_job_processor_api.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_listener.py` & `reqless-0.13.2/reqless_test/test_listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_qmore_client.py` & `reqless-0.13.2/reqless_test/test_qmore_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Dict, List, Mapping, Union
 
-from qmore.client import (
+from reqless.qmore.client import (
     QUEUE_IDENTIFIER_PATTERNS_KEY,
     QUEUE_PRIORITY_PATTERNS_KEY,
     QmoreClient,
     QueuePriorityPattern,
 )
 from reqless_test.common import TestReqless
```

### Comparing `reqless-0.13.1/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.2/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 from typing import Dict, List
 from uuid import uuid4
 
-from qmore.client import QmoreClient
+from reqless.qmore.client import QmoreClient
 from reqless.queue_resolvers.qmore_dynamic_mapping_queue_identifiers_transformer import (  # noqa: E501
     QmoreDynamicMappingQueueIdentifiersTransformer,
 )
 from reqless.queue_resolvers.transforming_queue_resolver import (
     TransformingQueueResolver,
 )
 from reqless_test.common import TestReqless
```

### Comparing `reqless-0.13.1/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.2/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from typing import List
 
-from qmore.client import QmoreClient, QueuePriorityPattern
+from reqless.qmore.client import QmoreClient, QueuePriorityPattern
 from reqless.queue_resolvers.qmore_dynamic_priority_queue_identifiers_transformer import (  # noqa: E501
     QmoreDynamicPriorityQueueIdentifiersTransformer,
 )
 from reqless.queue_resolvers.transforming_queue_resolver import (
     TransformingQueueResolver,
 )
 from reqless_test.common import TestReqless
```

### Comparing `reqless-0.13.1/reqless_test/test_queue.py` & `reqless-0.13.2/reqless_test/test_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_serial.py` & `reqless-0.13.2/reqless_test/test_serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_transforming_queue_resolver.py` & `reqless-0.13.2/reqless_test/test_transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_worker.py` & `reqless-0.13.2/reqless_test/test_worker.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/reqless_test/test_worker_util.py` & `reqless-0.13.2/reqless_test/test_worker_util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.1/requirements.txt` & `reqless-0.13.2/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,83 +1,79 @@
-appdirs==1.4.4
 async-timeout==4.0.3
 black==24.2.0
 build==1.0.3
-certifi==2023.11.17
+certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 charset-normalizer==3.3.2
 click==8.1.7
-colorama==0.4.6
-coverage==7.3.0
+coverage==7.4.4
 coverage-badge==1.1.0
 cryptography==42.0.5
 decorator==5.1.1
 distlib==0.3.7
 docutils==0.20.1
 dparse==0.6.3
+exceptiongroup==1.2.0
 filelock==3.13.1
 flake8==7.0.0
 Flake8-pyproject==1.2.3
-funcsigs==0.4
-gevent==22.10.2
-greenlet==2.0.1
+gevent==24.2.1
+greenlet==3.0.3
 hiredis==2.2.3
 identify==2.5.32
 idna==3.4
 importlib-metadata==6.8.0
+iniconfig==2.0.0
 isort==5.8.0
 jaraco.classes==3.3.0
 jeepney==0.8.0
 keyring==24.3.0
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
 mock==1.3.0
 more-itertools==10.1.0
-mypy==1.7.0
+mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.15
 nodeenv==1.8.0
-nose==1.3.7
 packaging==23.2
 pathspec==0.11.2
-pbr==1.8.1
+pbr==6.0.0
 pkginfo==1.9.6
 platformdirs==4.0.0
+pluggy==1.4.0
 pre-commit==2.20.0
 pycodestyle==2.11.1
 pycparser==2.21
 pyflakes==3.2.0
 Pygments==2.17.2
-pyparsing==3.1.1
 pyproject_hooks==1.0.0
-python-termstyle==0.1.10
+pytest==7.4.4
 PyYAML==6.0.1
 readme-renderer==42.0
 redis==5.0.0
-rednose==1.1.1
-regex==2023.10.3
 removestar==1.3.1
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.0
 ruamel.yaml==0.18.5
 ruamel.yaml.clib==0.2.8
 safety==2.3.4
 SecretStorage==3.3.3
-setproctitle==1.3.2
+setproctitle==1.3.3
 six==1.16.0
 toml==0.10.2
 tomli==2.0.1
 twine==4.0.2
 types-decorator==5.1.8.4
 types-mock==5.1.0.2
-types-pyOpenSSL==23.3.0.0
+types-pyOpenSSL==24.0.0.20240311
 types-redis==4.6.0.11
 typing_extensions==4.8.0
 urllib3==2.1.0
 virtualenv==20.24.7
 zipp==3.17.0
 zope.event==5.0
-zope.interface==6.0
+zope.interface==6.2
```

### Comparing `reqless-0.13.1/whitelist.txt` & `reqless-0.13.2/whitelist.txt`

 * *Files identical despite different names*

