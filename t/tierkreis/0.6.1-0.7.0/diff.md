# Comparing `tmp/tierkreis-0.6.1.tar.gz` & `tmp/tierkreis-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tierkreis-0.6.1.tar", last modified: Wed Mar 27 14:46:15 2024, max compression
+gzip compressed data, was "tierkreis-0.7.0.tar", last modified: Tue Apr  9 08:38:50 2024, max compression
```

## Comparing `tierkreis-0.6.1.tar` & `tierkreis-0.7.0.tar`

### file list

```diff
@@ -1,88 +1,78 @@
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.514640 tierkreis-0.6.1/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     6916 2024-03-27 14:46:15.514457 tierkreis-0.6.1/PKG-INFO
--rw-r--r--   0 alanlawrence   (503) staff       (20)     5303 2024-03-20 12:22:55.000000 tierkreis-0.6.1/README.md
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2149 2024-03-20 12:22:55.000000 tierkreis-0.6.1/pyproject.toml
--rw-r--r--   0 alanlawrence   (503) staff       (20)       38 2024-03-27 14:46:15.514679 tierkreis-0.6.1/setup.cfg
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.501291 tierkreis-0.6.1/tests/
--rw-r--r--   0 alanlawrence   (503) staff       (20)    30738 2024-03-04 15:40:21.000000 tierkreis-0.6.1/tests/test_builder.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     3467 2024-02-13 12:04:29.000000 tierkreis-0.6.1/tests/test_commontypes.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     7553 2024-03-26 09:05:06.000000 tierkreis-0.6.1/tests/test_frontend.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     5937 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tests/test_generics.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      834 2024-01-19 14:34:58.000000 tierkreis-0.6.1/tests/test_pyruntime.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2680 2024-02-13 12:04:29.000000 tierkreis-0.6.1/tests/test_pytket_worker.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     6541 2024-02-14 14:19:44.000000 tierkreis-0.6.1/tests/test_tierkreis_graph.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     9994 2024-03-04 15:40:21.000000 tierkreis-0.6.1/tests/test_type_check.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    12126 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tests/test_variants.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.502453 tierkreis-0.6.1/tierkreis/
--rw-r--r--   0 alanlawrence   (503) staff       (20)      423 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.503235 tierkreis-0.6.1/tierkreis/_build/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2034 2023-12-11 11:32:54.000000 tierkreis-0.6.1/tierkreis/_build/generate_protos.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)       22 2024-03-27 14:42:05.000000 tierkreis-0.6.1/tierkreis/_version.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    32054 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/builder.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     8197 2024-02-14 14:19:44.000000 tierkreis-0.6.1/tierkreis/cli.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.503875 tierkreis-0.6.1/tierkreis/client/
--rw-r--r--   0 alanlawrence   (503) staff       (20)      120 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/client/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      665 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/client/runtime_client.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     6292 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/client/server_client.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.504353 tierkreis-0.6.1/tierkreis/common_types/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     3267 2024-02-13 12:04:29.000000 tierkreis-0.6.1/tierkreis/common_types/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     3678 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/common_types/circuit.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.507021 tierkreis-0.6.1/tierkreis/core/
--rw-r--r--   0 alanlawrence   (503) staff       (20)      334 2024-01-19 14:34:58.000000 tierkreis-0.6.1/tierkreis/core/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      993 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/function.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    14621 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/graphviz.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     3559 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/internal.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      800 2024-02-13 12:04:29.000000 tierkreis-0.6.1/tierkreis/core/opaque_model.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.507207 tierkreis-0.6.1/tierkreis/core/protos/
--rw-r--r--   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.497602 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.507313 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/
--rw-r--r--   0 alanlawrence   (503) staff       (20)        0 2024-02-13 15:37:40.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.507418 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/graph/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     7073 2024-02-13 15:37:40.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.509639 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/runtime/
--rw-r--r--   0 alanlawrence   (503) staff       (20)    10619 2024-01-02 15:11:02.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.509892 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/signature/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     8624 2024-02-13 15:37:40.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510139 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/worker/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2467 2024-01-02 15:11:02.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510340 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/
--rw-r--r--   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510451 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/graph/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     7330 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510564 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/jobs/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     9122 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510685 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2834 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510820 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/signature/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     8629 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.510992 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/worker/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2504 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      631 2024-02-14 14:19:44.000000 tierkreis-0.6.1/tierkreis/core/python.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2299 2024-02-14 14:19:44.000000 tierkreis-0.6.1/tierkreis/core/signature.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    22367 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/tierkreis_graph.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     6796 2024-02-14 14:19:44.000000 tierkreis-0.6.1/tierkreis/core/type_errors.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2290 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/type_inference.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    21946 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/types.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     1616 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/utils.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    29576 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/core/values.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)        0 2023-10-02 13:01:20.000000 tierkreis-0.6.1/tierkreis/py.typed
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.511519 tierkreis-0.6.1/tierkreis/pyruntime/
--rw-r--r--   0 alanlawrence   (503) staff       (20)       38 2023-10-02 13:01:20.000000 tierkreis-0.6.1/tierkreis/pyruntime/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    21024 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/pyruntime/python_builtin.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    12560 2024-03-26 09:05:06.000000 tierkreis-0.6.1/tierkreis/pyruntime/python_runtime.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.513139 tierkreis-0.6.1/tierkreis/worker/
--rw-r--r--   0 alanlawrence   (503) staff       (20)       82 2023-10-02 13:01:20.000000 tierkreis-0.6.1/tierkreis/worker/__init__.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     1430 2024-02-05 15:36:33.000000 tierkreis-0.6.1/tierkreis/worker/callback.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      643 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/worker/exceptions.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)    10060 2024-03-25 15:49:30.000000 tierkreis-0.6.1/tierkreis/worker/namespace.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     1797 2024-03-20 12:22:55.000000 tierkreis-0.6.1/tierkreis/worker/prelude.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)      945 2023-12-11 11:32:54.000000 tierkreis-0.6.1/tierkreis/worker/tracing.py
--rw-r--r--   0 alanlawrence   (503) staff       (20)     9856 2024-03-27 14:40:51.000000 tierkreis-0.6.1/tierkreis/worker/worker.py
-drwxr-xr-x   0 alanlawrence   (503) staff       (20)        0 2024-03-27 14:46:15.513474 tierkreis-0.6.1/tierkreis.egg-info/
--rw-r--r--   0 alanlawrence   (503) staff       (20)     6916 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/PKG-INFO
--rw-r--r--   0 alanlawrence   (503) staff       (20)     2103 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/SOURCES.txt
--rw-r--r--   0 alanlawrence   (503) staff       (20)        1 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/dependency_links.txt
--rw-r--r--   0 alanlawrence   (503) staff       (20)       43 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/entry_points.txt
--rw-r--r--   0 alanlawrence   (503) staff       (20)      550 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/requires.txt
--rw-r--r--   0 alanlawrence   (503) staff       (20)       10 2024-03-27 14:46:15.000000 tierkreis-0.6.1/tierkreis.egg-info/top_level.txt
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.890560 tierkreis-0.7.0/
+-rw-r--r--   0 seyon      (502) staff       (20)     6928 2024-04-09 08:38:50.890315 tierkreis-0.7.0/PKG-INFO
+-rw-r--r--   0 seyon      (502) staff       (20)     5315 2024-04-08 15:53:23.000000 tierkreis-0.7.0/README.md
+-rw-r--r--   0 seyon      (502) staff       (20)     2149 2024-04-08 15:53:22.000000 tierkreis-0.7.0/pyproject.toml
+-rw-r--r--   0 seyon      (502) staff       (20)       38 2024-04-09 08:38:50.890614 tierkreis-0.7.0/setup.cfg
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.877149 tierkreis-0.7.0/tests/
+-rw-r--r--   0 seyon      (502) staff       (20)    29142 2024-04-09 08:38:37.000000 tierkreis-0.7.0/tests/test_builder.py
+-rw-r--r--   0 seyon      (502) staff       (20)     3467 2024-02-13 11:22:18.000000 tierkreis-0.7.0/tests/test_commontypes.py
+-rw-r--r--   0 seyon      (502) staff       (20)     7553 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_frontend.py
+-rw-r--r--   0 seyon      (502) staff       (20)     5937 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_generics.py
+-rw-r--r--   0 seyon      (502) staff       (20)      834 2024-02-13 11:22:18.000000 tierkreis-0.7.0/tests/test_pyruntime.py
+-rw-r--r--   0 seyon      (502) staff       (20)     2680 2024-02-09 15:49:47.000000 tierkreis-0.7.0/tests/test_pytket_worker.py
+-rw-r--r--   0 seyon      (502) staff       (20)     6541 2024-02-13 16:35:16.000000 tierkreis-0.7.0/tests/test_tierkreis_graph.py
+-rw-r--r--   0 seyon      (502) staff       (20)     9996 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tests/test_type_check.py
+-rw-r--r--   0 seyon      (502) staff       (20)    12126 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_variants.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.878931 tierkreis-0.7.0/tierkreis/
+-rw-r--r--   0 seyon      (502) staff       (20)      423 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.879895 tierkreis-0.7.0/tierkreis/_build/
+-rw-r--r--   0 seyon      (502) staff       (20)     2034 2024-01-31 13:06:30.000000 tierkreis-0.7.0/tierkreis/_build/generate_protos.py
+-rw-r--r--   0 seyon      (502) staff       (20)       22 2024-04-09 08:38:37.000000 tierkreis-0.7.0/tierkreis/_version.py
+-rw-r--r--   0 seyon      (502) staff       (20)    29295 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tierkreis/builder.py
+-rw-r--r--   0 seyon      (502) staff       (20)     8197 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/cli.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.880791 tierkreis-0.7.0/tierkreis/client/
+-rw-r--r--   0 seyon      (502) staff       (20)      120 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)      665 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/runtime_client.py
+-rw-r--r--   0 seyon      (502) staff       (20)     6292 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/server_client.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.881385 tierkreis-0.7.0/tierkreis/common_types/
+-rw-r--r--   0 seyon      (502) staff       (20)     3267 2024-02-09 15:49:47.000000 tierkreis-0.7.0/tierkreis/common_types/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)     3678 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/common_types/circuit.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.884718 tierkreis-0.7.0/tierkreis/core/
+-rw-r--r--   0 seyon      (502) staff       (20)      334 2023-12-12 17:11:07.000000 tierkreis-0.7.0/tierkreis/core/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)      993 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/function.py
+-rw-r--r--   0 seyon      (502) staff       (20)    14621 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/graphviz.py
+-rw-r--r--   0 seyon      (502) staff       (20)     3559 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/core/internal.py
+-rw-r--r--   0 seyon      (502) staff       (20)      800 2024-02-08 09:05:47.000000 tierkreis-0.7.0/tierkreis/core/opaque_model.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885125 tierkreis-0.7.0/tierkreis/core/protos/
+-rw-r--r--   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.872980 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885234 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/
+-rw-r--r--   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885346 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/
+-rw-r--r--   0 seyon      (502) staff       (20)     7330 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885491 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/
+-rw-r--r--   0 seyon      (502) staff       (20)     9122 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885641 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/
+-rw-r--r--   0 seyon      (502) staff       (20)     2834 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885803 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/
+-rw-r--r--   0 seyon      (502) staff       (20)     8629 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885959 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/
+-rw-r--r--   0 seyon      (502) staff       (20)     2504 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)      631 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/python.py
+-rw-r--r--   0 seyon      (502) staff       (20)     2299 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/signature.py
+-rw-r--r--   0 seyon      (502) staff       (20)    22367 2024-04-08 11:23:50.000000 tierkreis-0.7.0/tierkreis/core/tierkreis_graph.py
+-rw-r--r--   0 seyon      (502) staff       (20)     6796 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/type_errors.py
+-rw-r--r--   0 seyon      (502) staff       (20)     2290 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/type_inference.py
+-rw-r--r--   0 seyon      (502) staff       (20)    21946 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/core/types.py
+-rw-r--r--   0 seyon      (502) staff       (20)     1616 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/utils.py
+-rw-r--r--   0 seyon      (502) staff       (20)    28160 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tierkreis/core/values.py
+-rw-r--r--   0 seyon      (502) staff       (20)        0 2023-06-28 10:16:02.000000 tierkreis-0.7.0/tierkreis/py.typed
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.886890 tierkreis-0.7.0/tierkreis/pyruntime/
+-rw-r--r--   0 seyon      (502) staff       (20)       38 2023-12-05 11:53:45.000000 tierkreis-0.7.0/tierkreis/pyruntime/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)    21024 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/pyruntime/python_builtin.py
+-rw-r--r--   0 seyon      (502) staff       (20)    12559 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/pyruntime/python_runtime.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.888796 tierkreis-0.7.0/tierkreis/worker/
+-rw-r--r--   0 seyon      (502) staff       (20)       82 2023-12-05 11:53:45.000000 tierkreis-0.7.0/tierkreis/worker/__init__.py
+-rw-r--r--   0 seyon      (502) staff       (20)     1430 2024-02-01 14:26:16.000000 tierkreis-0.7.0/tierkreis/worker/callback.py
+-rw-r--r--   0 seyon      (502) staff       (20)      643 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/worker/exceptions.py
+-rw-r--r--   0 seyon      (502) staff       (20)    10452 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/worker/namespace.py
+-rw-r--r--   0 seyon      (502) staff       (20)     1797 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/worker/prelude.py
+-rw-r--r--   0 seyon      (502) staff       (20)      945 2023-12-07 09:29:31.000000 tierkreis-0.7.0/tierkreis/worker/tracing.py
+-rw-r--r--   0 seyon      (502) staff       (20)     9611 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/worker/worker.py
+drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.889089 tierkreis-0.7.0/tierkreis.egg-info/
+-rw-r--r--   0 seyon      (502) staff       (20)     6928 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/PKG-INFO
+-rw-r--r--   0 seyon      (502) staff       (20)     1812 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/SOURCES.txt
+-rw-r--r--   0 seyon      (502) staff       (20)        1 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/dependency_links.txt
+-rw-r--r--   0 seyon      (502) staff       (20)       43 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/entry_points.txt
+-rw-r--r--   0 seyon      (502) staff       (20)      550 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/requires.txt
+-rw-r--r--   0 seyon      (502) staff       (20)       10 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/top_level.txt
```

### Comparing `tierkreis-0.6.1/PKG-INFO` & `tierkreis-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: betterproto[compiler]==2.0.0b6
 Requires-Dist: protobuf<4,>=3.19
 Requires-Dist: grpclib<0.5,>=0.4.3rc
@@ -63,15 +63,15 @@
 
 You can now build a graph (Tierkreis program), optionally type check it and execute it. The recommended environment for this is a Jupyter notebook (especially given some operations are async).
 
 First we need the runtime we are going to execute on and a handle to the primitive functions available on that runtime.
 The python package comes with the `PyRuntime` which runs locally in your python environment.
 
 ```python
-from tierkreis.builder import graph, Namespace, Output, Input
+from tierkreis.builder import graph, Namespace, Output, ValueSource
 from tierkreis.pyruntime import PyRuntime
 
 cl = PyRuntime([]) # empty list for no extra workers
 sig = await cl.get_signature()
 ns = Namespace(sig) # get a handle to all functions
 print(ns.iadd)
 print(ns.unpack_pair)
@@ -85,15 +85,15 @@
 
 ### Build
 
 The `@graph` decorator allows you to build graphs using python functions.
 
 ```python
 @graph()
-def sum_pair(pair: Input) -> Output:
+def sum_pair(pair: ValueSource) -> Output:
     first, second = ns.unpack_pair(pair) # tierkreis functions can have multiple outputs
     return Output(ns.iadd(first, second))
 ```
 
 Calling the decorated function with no arguments (`sum_pair()`) returns a `TierkreisGraph`.
 
 ### Visualise
```

### Comparing `tierkreis-0.6.1/README.md` & `tierkreis-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 You can now build a graph (Tierkreis program), optionally type check it and execute it. The recommended environment for this is a Jupyter notebook (especially given some operations are async).
 
 First we need the runtime we are going to execute on and a handle to the primitive functions available on that runtime.
 The python package comes with the `PyRuntime` which runs locally in your python environment.
 
 ```python
-from tierkreis.builder import graph, Namespace, Output, Input
+from tierkreis.builder import graph, Namespace, Output, ValueSource
 from tierkreis.pyruntime import PyRuntime
 
 cl = PyRuntime([]) # empty list for no extra workers
 sig = await cl.get_signature()
 ns = Namespace(sig) # get a handle to all functions
 print(ns.iadd)
 print(ns.unpack_pair)
@@ -48,15 +48,15 @@
 
 ### Build
 
 The `@graph` decorator allows you to build graphs using python functions.
 
 ```python
 @graph()
-def sum_pair(pair: Input) -> Output:
+def sum_pair(pair: ValueSource) -> Output:
     first, second = ns.unpack_pair(pair) # tierkreis functions can have multiple outputs
     return Output(ns.iadd(first, second))
 ```
 
 Calling the decorated function with no arguments (`sum_pair()`) returns a `TierkreisGraph`.
 
 ### Visualise
```

### Comparing `tierkreis-0.6.1/pyproject.toml` & `tierkreis-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_builder.py` & `tierkreis-0.7.0/tests/test_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Callable, Tuple, cast, no_type_check
+from typing import TYPE_CHECKING, Callable, Tuple, cast
 
 import pytest
 
 from tierkreis.builder import (
     Break,
     Case,
     Const,
     Continue,
     Copyable,
     Else,
     If,
     IfElse,
-    Input,
     MakeTuple,
     Match,
     Namespace,
+    NodePort,
     Output,
     Scope,
     Tag,
     UnpackTuple,
     ValueSource,
     closure,
     current_builder,
@@ -35,33 +35,26 @@
     BoxNode,
     ConstNode,
     FunctionNode,
     GraphValue,
     TierkreisGraph,
 )
 from tierkreis.core.types import (
-    IntType,
-    MapType,
-    StringType,
     TierkreisPair,
-    UnpackRow,
-    VecType,
 )
 from tierkreis.core.utils import map_vals, rename_ports_graph
 from tierkreis.core.values import (
     BoolValue,
     FloatValue,
     IntValue,
-    MapValue,
     PairValue,
     StringValue,
     StructValue,
     TierkreisValue,
     TierkreisVariant,
-    VariantValue,
     VecValue,
 )
 from tierkreis.pyruntime import PyRuntime
 
 if TYPE_CHECKING:
     from tierkreis.builder import StablePortFunc
     from tierkreis.core.tierkreis_graph import NodePort, NodeRef
@@ -74,47 +67,45 @@
     return first.to_proto() == second.to_proto()
 
 
 def _vecs_graph() -> TierkreisGraph:
     tg = TierkreisGraph("g")
     con = tg.add_const([2, 4])
     tg.set_outputs(value=con)
-    tg.annotate_output(Labels.VALUE, VecType(IntType()))
     tg.output_order = [Labels.VALUE]
     return tg
 
 
 @pytest.fixture()
 def _vecs_graph_builder() -> TierkreisGraph:
     @graph()
-    def g() -> Output[VecValue[IntValue]]:
+    def g() -> Output:
         return Output(Const([2, 4]))
 
     return g
 
 
 def _structs_graph() -> TierkreisGraph:
     tg = TierkreisGraph("g")
     factory = tg.add_func(
         "make_struct",
         **map_vals(dict(height=12.3, name="hello", age=23), tg.add_const),
     )
     sturct = tg.add_func("unpack_struct", struct=factory["struct"])
 
     tg.set_outputs(value=sturct["age"])
-    tg.annotate_output("value", IntType())
     tg.output_order = [Labels.VALUE]
 
     return tg
 
 
 @pytest.fixture()
-def _structs_graph_builder(bi) -> TierkreisGraph:
+def _structs_graph_builder(bi: Namespace) -> TierkreisGraph:
     @graph()
-    def g() -> Output[IntValue]:
+    def g() -> Output:
         st_node = bi.make_struct(height=Const(12.3), name=Const("hello"), age=Const(23))
         return Output(st_node["struct"]["age"])
 
     return g
 
 
 def _maps_graph() -> TierkreisGraph:
@@ -123,106 +114,98 @@
     ins = tg.add_func(
         "insert_key",
         map=mp_val["map"],
         **map_vals(dict(key=5, val="bar"), tg.add_const),
     )
 
     tg.set_outputs(mp=ins["map"], vl=mp_val["val"])
-    tg.annotate_input("mp", MapType(IntType(), StringType()))
-    tg.annotate_output("mp", MapType(IntType(), StringType()))
-    tg.annotate_output("vl", StringType())
     tg.input_order = ["mp"]
     tg.output_order = ["mp", "vl"]
     return tg
 
 
 @pytest.fixture()
-def _maps_graph_builder(bi) -> TierkreisGraph:
-    @dataclass
-    class Mapout(UnpackRow):
-        mp: MapValue[IntValue, StringValue]
-        vl: StringValue
-
-    @graph()
-    def g(mp: Input[MapValue[IntValue, StringValue]]) -> Output[Mapout]:
+def _maps_graph_builder(bi: Namespace) -> TierkreisGraph:
+    @graph(output_order=["mp", "vl"])
+    def g(mp: ValueSource) -> Output:
         mp, val = bi.remove_key(mp, Const(3))
         return Output(bi.insert_key(mp, Const(5), Const("bar")), val)
 
     return g
 
 
 def _tag_match_graph() -> TierkreisGraph:
     id_graph = TierkreisGraph("foo")
     id_graph.set_outputs(value=id_graph.input[Labels.VALUE])
+    id_graph.output_order = [Labels.VALUE]
 
     tg = TierkreisGraph("g")
     in_v = tg.add_tag("foo", value=tg.add_const(4))
     m = tg.add_match(in_v, foo=tg.add_const(id_graph))
     e = tg.add_func("eval", thunk=m[Labels.THUNK])
     tg.set_outputs(value=e[Labels.VALUE])
-    tg.annotate_output("value", IntType())
     tg.output_order = [Labels.VALUE]
 
     return tg
 
 
 @pytest.fixture()
-def _tag_match_graph_builder(bi) -> TierkreisGraph:
+def _tag_match_graph_builder(bi: Namespace) -> TierkreisGraph:
     @graph()
-    def g() -> Output[IntValue]:
+    def g() -> Output:
         with Match(Tag("foo", Const(4))) as match:
             with Case("foo") as h1:
                 Output(h1.var_value)
         return Output(match.nref)
 
     return g
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "builder,expected_gen",
     [
-        ("_vecs_graph_builder", _vecs_graph),
-        ("_structs_graph_builder", _structs_graph),
+        # ("_vecs_graph_builder", _vecs_graph),
+        # ("_structs_graph_builder", _structs_graph),
         ("_maps_graph_builder", _maps_graph),
-        ("_tag_match_graph_builder", _tag_match_graph),
+        # ("_tag_match_graph_builder", _tag_match_graph),
     ],
 )
 async def test_builder_sample(
     builder: str,
     expected_gen: Callable[[], TierkreisGraph],
     client: RuntimeClient,
-    bi,  # for some reason fails without this
-    request,
+    bi: Namespace,  # for some reason fails without this
+    request: pytest.FixtureRequest,
 ) -> None:
     tg = request.getfixturevalue(builder)
-
-    assert _compare_graphs(tg, expected_gen())
+    assert tg.to_proto() == expected_gen().to_proto()
+    # assert _compare_graphs(tg, expected_gen())
     if client.can_type_check:
         tg = await client.type_check_graph(tg)
 
 
 def _big_sample_builder(bi: Namespace) -> TierkreisGraph:
-    def add2(x: ValueSource) -> Output[IntValue]:
+    def add2(x: ValueSource):
         return Output(bi.iadd(x, Const(2)))
 
-    def add5(x: ValueSource) -> Output[IntValue]:
+    def add5(x: ValueSource):
         return Output(bi.iadd(x, Const(5)))
 
     @dataclass
     class Point:
         p1: FloatValue
         p2: IntValue
 
     @graph()
-    def struc_id(in_st: Input[StructValue[Point]]) -> Output[StructValue[Point]]:
+    def struc_id(in_st: ValueSource) -> Output:
         return Output(in_st)
 
     @graph()
-    def func(v1: Input[IntValue], v2: Input) -> Output:
+    def func(v1: ValueSource, v2: ValueSource) -> Output:
         fst, scd = UnpackTuple(v2, 2)
         other_total = bi.iadd(fst, Const(3))
         dbl = double(bi)
         _tuple_out = MakeTuple(Const(True), Const("asdf"))
         total = dbl(v1)
 
         quadruple = bi.sequence(Const(dbl), Const(dbl))
@@ -232,15 +215,15 @@
         with IfElse(scd) as ifelse:
             with If():
                 add2(total4)
             with Else():
                 add5(total4)
 
         @loop()
-        def loop_def(initial_: Input[IntValue]) -> Output:
+        def loop_def(initial_):
             initial = Copyable(initial_)
             with IfElse(bi.ilt(initial, Const(100))) as loop_ifelse:
                 with If():
                     Continue(bi.iadd(initial, Const(5)))
                 with Else():
                     Break(initial)
             return Output(loop_ifelse.nref)
@@ -249,65 +232,60 @@
 
         return Output(o1=ifelse.nref, o2=loop_def(other_total))
 
     return func
 
 
 @pytest.mark.asyncio
-async def test_bigexample(client: RuntimeClient, bi) -> None:
+async def test_bigexample(client: RuntimeClient, bi: Namespace) -> None:
     tg = _big_sample_builder(bi)
     if not client.can_type_check:
         pytest.skip()
     tg = await client.type_check_graph(tg)
     assert sum(1 for _ in tg.nodes()) == 24
     for flag in (True, False):
         outputs = await client.run_graph(tg, v1=67, v2=(45, flag))
         outputs = await client.run_graph(tg, v1=67, v2=(45, flag))
         pyouts = {key: val.try_autopython() for key, val in outputs.items()}
         assert pyouts == {"o2": 103, "o1": 536 + (2 if flag else 5)}
 
 
 def double(bi: Namespace) -> TierkreisGraph:
     @graph()
-    def _double(value: Input[IntValue]) -> Output[IntValue]:
+    def _double(value: ValueSource) -> Output:
         return Output(bi.iadd(*bi.copy(value)))
 
     return _double
 
 
 @pytest.mark.asyncio
 async def test_double(client: RuntimeClient, bi: Namespace):
     out = await client.run_graph(double(bi), value=10)
     assert out == {"value": IntValue(20)}
 
 
 @pytest.mark.asyncio
 async def test_copy(client: RuntimeClient, bi: Namespace):
-    @dataclass
-    class CopyOut(UnpackRow):
-        a: Any
-        b: IntValue
-
-    @graph()
-    def copy_graph(y: Input[IntValue]) -> Output[CopyOut]:
+    @graph(output_order=["a", "b"])
+    def copy_graph(y: ValueSource) -> Output:
         return Output(*bi.copy(y))
 
     out = await client.run_graph(copy_graph, y=10)
     assert out == {"a": IntValue(10), "b": IntValue(10)}
 
 
 @pytest.mark.asyncio
 async def test_ifelse(client: RuntimeClient, bi: Namespace):
     # some graph type annotations are missing here to test this scenario
     @graph()
-    def triple(y: Input[IntValue]):
+    def triple(y: ValueSource) -> Output:
         return Output(bi.imul(y, Const(3)))
 
     @graph()
-    def ifelse(x: Input, flag) -> Output:
+    def ifelse(x: ValueSource, flag: ValueSource) -> Output:
         bias = Const(1)
         with IfElse(flag) as sw:
             with If():
                 Output(value=bi.iadd(bias, triple(x)))
             with Else():
                 Output(value=x)
         return Output(sw.nref)
@@ -332,15 +310,15 @@
 
 @pytest.mark.asyncio
 async def test_ifelse_copying(
     client: RuntimeClient,
     bi: Namespace,
 ):
     @graph()
-    def ifelse(x: Input[IntValue]) -> Output[IntValue]:
+    def ifelse(x: ValueSource) -> Output:
         pred = bi.eq(bi.imod(x, Const(2)), Const(0))
         x2 = Copyable(x)
         with IfElse(pred) as sw:
             with If():
                 Output(value=bi.idiv(x2, Const(2)))
             with Else():
                 Output(value=bi.iadd(bi.imul(x2, Const(3)), Const(1)))
@@ -357,15 +335,15 @@
     outs = await client.run_graph(ifelse, x=5)
     assert outs == {"value": IntValue(16)}
 
 
 @pytest.mark.asyncio
 async def test_copy_twice_inside_if(client: RuntimeClient, bi: Namespace):
     @graph()
-    def ifelse(x: Input[IntValue], flag: Input[BoolValue]) -> Output[IntValue]:
+    def ifelse(x: ValueSource, flag: ValueSource) -> Output:
         with IfElse(flag) as sw:
             with If():
                 c = Copyable(x)  # Copy in inner graph
                 Output(value=bi.imul(c, bi.iadd(c, Const(1))))
             with Else():
                 Output(value=x)
         return Output(sw.nref)
@@ -377,15 +355,15 @@
     assert outs[True] == {"value": IntValue(12)}
     assert outs[False] == {"value": IntValue(3)}
 
 
 @pytest.mark.asyncio
 async def test_copy_twice_from_outside_if(bi: Namespace):
     @lazy_graph()
-    def ifelse(x: Input[IntValue], flag: Input[BoolValue]) -> Output[IntValue]:
+    def ifelse(x: ValueSource, flag: ValueSource) -> Output:
         c = Copyable(x)  # This can only copy in outer graph
         with IfElse(flag) as sw:
             with If():
                 # Use copy twice in inner graph, this is not allowed
                 Output(value=bi.imul(c, bi.iadd(c, Const(1))))
             with Else():
                 Output(value=c)
@@ -394,23 +372,23 @@
     with pytest.raises(ValueError, match="Already captured"):
         _ = ifelse.graph
 
 
 @pytest.mark.asyncio
 async def test_loop(client: RuntimeClient, bi: Namespace):
     @graph()
-    def loopyg() -> Output[FloatValue]:
+    def loopyg() -> Output:
         incr = Const(1)
 
         @loop()
-        def loop_def(value: Input[IntValue]) -> Output:
+        def loop_def(value):
             x1, x2 = bi.copy(value)
 
             @closure()
-            def succ(x: Input[IntValue]) -> Output[IntValue]:
+            def succ(x):
                 return Output(value=bi.iadd(x, incr))
 
             with IfElse(bi.ilt(x1, Const(7))) as sw:
                 with If():
                     Continue(succ(x2))
                 with Else():
                     Break(bi.int_to_float(x2))
@@ -425,15 +403,15 @@
 async def test_match(client: RuntimeClient, bi: Namespace):
     @dataclass
     class _Vdict:
         list: VecValue[FloatValue]
         pair: PairValue[FloatValue, FloatValue]
 
     @graph()
-    def match(var: Input[VariantValue[_Vdict]]) -> Output:
+    def match(var: ValueSource) -> Output:
         factor = Const(2.0)
         with Match(var) as match:
             with Case("list") as h1:
                 lst, fst = bi.pop(h1.var_value)
                 Output(bi.push(lst, bi.fmul(fst, factor)))
             with Case("pair") as h2:
                 fst, scd = bi.unpack_pair(h2.var_value)
@@ -448,30 +426,27 @@
     assert (
         await client.run_graph(match, var=TierkreisVariant("list", [1.0, 2.0]))
     ) == {"value": VecValue(values=[FloatValue(value=1.0), FloatValue(value=4.0)])}
 
 
 @pytest.fixture()
 def _tuple_builder(bi: Namespace, sig: Signature) -> TierkreisGraph:
-    @dataclass
-    class TestPair(UnpackRow):
-        first: IntValue
-        second: StringValue
-
     @graph()
-    def main() -> Output[TestPair]:
-        return Output(*UnpackTuple(Const((2, "asdf")), 2))
+    def main() -> Output:
+        return Output(
+            **dict(zip(("first", "second"), UnpackTuple(Const((2, "asdf")), 2)))
+        )
 
     return main
 
 
 @pytest.fixture()
 def _if_no_inputs(bi: Namespace, sig: Signature) -> TierkreisGraph:
     @graph()
-    def main(pred: Input[BoolValue]) -> Output[IntValue]:
+    def main(pred: ValueSource) -> Output:
         with IfElse(pred) as ifelse:
             with If():
                 Output(Const(3))
             with Else():
                 Output(Const(5))
         return Output(ifelse.nref)
 
@@ -488,27 +463,27 @@
     ],
 )
 async def test_run_sample(
     client: RuntimeClient,
     builder: str,
     inputs: dict[str, TierkreisValue],
     expected_outputs: dict[str, TierkreisValue],
-    bi,
-    request,
+    bi: Namespace,
+    request: pytest.FixtureRequest,
 ) -> None:
     tg = request.getfixturevalue(builder)
 
     outputs = await client.run_graph(tg, **inputs)
     assert outputs == expected_outputs
 
 
 @pytest.mark.asyncio
-async def test_Copyable(bi, client: RuntimeClient) -> None:
+async def test_Copyable(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
-    def foo(a: Input[IntValue], b: Input[IntValue]) -> Output:
+    def foo(a: ValueSource, b: ValueSource) -> Output:
         assert num_copies(current_graph()) == 0
 
         # Even without an explicit Copy, discards should be removed
         f = bi.iadd(a=a, b=b)
         assert num_copies(current_graph()) == 0
 
         a_squared_plus_ab = bi.imul(a=Copyable(a), b=f)
@@ -520,25 +495,25 @@
 
     outputs = await client.run_graph(foo, a=2, b=3)
     assert outputs == {"out": IntValue(10), "res": IntValue(7)}
 
 
 @pytest.mark.asyncio
 async def test_unpacking(
-    bi,
+    bi: Namespace,
     client: RuntimeClient,
     sig: Signature,
 ) -> None:
     def num_unpacks() -> int:
         return sum(1 for n in current_graph().nodes() if n.is_unpack_node())
 
     pn = bi["python_nodes"]
 
     @graph()
-    def foo(a: Input[FloatValue], b: Input[IntValue]) -> Output:
+    def foo(a: ValueSource, b: ValueSource) -> Output:
         f = bi.make_struct(foo=a, bar=b)
         id_: "NodeRef" = pn.id_py(value=f["struct"])
         sturct: "NodePort" = id_["value"]
         old_proto = current_graph().to_proto()
 
         foo: "StablePortFunc" = sturct["foo"]
         assert num_unpacks() == 0
@@ -565,18 +540,18 @@
 def num_copies_unpacks() -> Tuple[int, int]:
     return (
         sum(1 for n in current_graph().nodes() if n.is_copy_node()),
         sum(1 for n in current_graph().nodes() if n.is_unpack_node()),
     )
 
 
-def test_cant_unpack_original_after_copy(bi) -> None:
+def test_cant_unpack_original_after_copy(bi: Namespace) -> None:
     @graph()
-    def foo(a: Input[StringValue], b: Input[FloatValue]) -> Output:
-        sturct: NodePort = bi.make_struct(foo=a, bar=b)["struct"]
+    def foo(a: ValueSource, b: ValueSource) -> Output:
+        sturct: ValueSource = bi.make_struct(foo=a, bar=b)["struct"]
 
         bi.discard(sturct["foo"])
         assert num_copies_unpacks() == (0, 1)
 
         cp = Copyable(sturct)
         o: Output = Output(whole=cp)
         assert num_copies_unpacks() == (1, 1)
@@ -587,17 +562,19 @@
                 sturct["bar"].resolve(), current_graph().output["second"]
             )
         assert proto == current_graph().to_proto()  # Did nothing
         return o
 
 
 @pytest.mark.asyncio
-async def test_can_unpack_copy_with_resolve(bi, client: RuntimeClient) -> None:
+async def test_can_unpack_copy_with_resolve(
+    bi: Namespace, client: RuntimeClient
+) -> None:
     @graph()
-    def foo(a: Input[IntValue], b: Input[IntValue]) -> Output:
+    def foo(a: ValueSource, b: ValueSource) -> Output:
         sturct = bi.make_struct(foo=a, bar=b)["struct"]
 
         s = bi.iadd(a=sturct["foo"], b=sturct["bar"])
         assert num_copies_unpacks() == (0, 1)
 
         cp = Copyable(sturct).resolve()
 
@@ -606,17 +583,17 @@
         return o
 
     outputs = await client.run_graph(foo, a=3, b=4)
     assert outputs == {"sum": IntValue(7), "product": IntValue(12)}
 
 
 @pytest.mark.asyncio
-async def test_Copyable_fields(bi, client: RuntimeClient) -> None:
+async def test_Copyable_fields(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
-    def foo(a: Input[IntValue], b: Input[IntValue]) -> Output:
+    def foo(a: ValueSource, b: ValueSource) -> Output:
         sturct = bi.make_struct(foo=a, bar=b)["struct"]
 
         s = bi.iadd(a=sturct["foo"], b=sturct["bar"])
         assert num_copies_unpacks() == (0, 1)
 
         return Output(
             sum=s,
@@ -626,90 +603,52 @@
     outputs = await client.run_graph(foo, a=3, b=4)
     assert outputs == {"sum": IntValue(7), "product": IntValue(12)}
 
 
 @pytest.mark.asyncio
 async def test_unpacking_nested(client: RuntimeClient) -> None:
     @graph()
-    def foo(arg: Input[Any]) -> Output:
+    def foo(arg: NodePort) -> Output:
         return Output(out=arg["outer"]["inner"])
 
     nested_val = FloatValue(42.0)
     argument: StructValue = StructValue(
         values={"outer": StructValue(values={"inner": nested_val})}
     )
 
     outputs = await client.run_graph(foo, arg=argument)
     assert outputs == {"out": nested_val}
 
 
-def test_retry_secs(bi) -> None:
+def test_retry_secs(bi: Namespace) -> None:
     pn = bi["python_nodes"]
 
     @graph()
-    def foo(arg: Input[Any]) -> Output:
+    def foo(arg: ValueSource) -> Output:
         return Output(res=pn.id_py(arg).with_retry_secs(2))
 
     (f,) = [n for n in foo.nodes() if isinstance(n, FunctionNode)]
     assert f.retry_secs == 2
 
 
-@pytest.mark.asyncio
-async def test_bad_annotations() -> None:
-    # pyright does not support no_type_check decorator
-    # so peppered with type: ignore
-    with pytest.raises(TypeError, match="return type"):
-
-        @no_type_check
-        @graph()  # type: ignore
-        def foo1(arg: Input[Any]) -> int:
-            return Output(out=arg)  # type: ignore
-
-    with pytest.raises(TypeError, match="return type"):
-
-        @no_type_check
-        @graph()
-        def foo2(arg: Input[Any]) -> Output[int]:  # type: ignore
-            return Output(out=arg)
-
-    with pytest.raises(TypeError, match="Graph builder function arguments"):
-
-        @no_type_check
-        @lazy_graph()
-        def foo3(arg: float) -> Output:
-            return Output(out=arg)  # type: ignore
-
-    with pytest.raises(ValueError, match="Cannot convert"):
-
-        @no_type_check
-        @lazy_graph()
-        def foo4(arg: Input[float]) -> Output:  # type: ignore
-            return Output(out=arg)
-
-
 @pytest.mark.skip_typecheck
 @pytest.mark.asyncio
 async def test_box_order(bi: Namespace, sig: Signature) -> None:
-    @dataclass
-    class TestOut(UnpackRow):
-        first: IntValue
-        lst: VecValue[PairValue[IntValue, StringValue]]
-
     @graph(type_check_sig=sig)
-    def push_pair(lst, first, second) -> Output[TestOut]:
+    def push_pair(lst: ValueSource, first: ValueSource, second: ValueSource) -> Output:
         first = Copyable(first)
         pair = bi.make_pair(first, second)
         return Output(lst=bi.push(lst, pair), first=first)
 
     assert push_pair.input_order == ["lst", "first", "second"]
-    assert push_pair.output_order == ["first", "lst"]
+    assert push_pair.output_order == ["lst", "first"]
 
     @graph(type_check_sig=sig)
     def test_g() -> Output:
-        i, lst = push_pair(Const([]), Const(3), Const("hello"))
+        lst, i = push_pair(Const([]), Const(3), Const("hello"))
         return Output(one=lst, two=i)
 
     box_n_name = next(
         n for n, nod in enumerate(test_g.nodes()) if isinstance(nod, BoxNode)
     )
     box_ins = {
         p2: n1
@@ -729,15 +668,15 @@
     assert len(box_outs) == 2
 
     assert ("first", "two") in box_outs
     assert ("lst", "one") in box_outs
 
 
 @pytest.mark.asyncio
-async def test_scope(bi, client: RuntimeClient) -> None:
+async def test_scope(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         with Scope():
             bi.discard(Const(3))
         assert len(current_builder().inner_scopes.values()) == 1
         return Output()
 
@@ -751,15 +690,15 @@
     )
     assert any([x.is_discard_node() for x in n.graph.nodes()])
     assert n.graph.inputs() == []
     assert n.graph.outputs() == []
 
 
 @pytest.mark.asyncio
-async def test_scope_capture_in(bi, client: RuntimeClient) -> None:
+async def test_scope_capture_in(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Const(3)
         with Scope():
             bi.discard(a)
         assert len(current_builder().inner_scopes.values()) == 1
         return Output()
@@ -774,15 +713,15 @@
     )
     assert any([x.is_discard_node() for x in n.graph.nodes()])
     assert n.graph.inputs() == ["_c0"]
     assert n.graph.outputs() == []
 
 
 @pytest.mark.asyncio
-async def test_scope_capture_out(bi, client: RuntimeClient) -> None:
+async def test_scope_capture_out(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         with Scope():
             a = Const(3)
         assert len(current_builder().inner_scopes.values()) == 1
         bi.discard(a)
         return Output()
@@ -797,15 +736,15 @@
     )
     assert not any([x.is_discard_node() for x in n.graph.nodes()])
     assert n.graph.inputs() == []
     assert n.graph.outputs() == ["_c0"]
 
 
 @pytest.mark.asyncio
-async def test_nested_scopes(bi, client: RuntimeClient) -> None:
+async def test_nested_scopes(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Const(3)
         with Scope():
             b = Const(2)
             c = bi.iadd(a, b)
             with Scope():
@@ -831,15 +770,15 @@
     )
     assert any([isinstance(x, BoxNode) for x in n.graph.nodes()])
     assert n.graph.inputs() == ["_c0"]
     assert sorted(n.graph.outputs()) == ["_c0", "_c1"]
 
 
 @pytest.mark.asyncio
-async def test_copyable_capture_in(bi, client: RuntimeClient) -> None:
+async def test_copyable_capture_in(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Copyable(Const(3))
         with Scope():
             bi.discard(a)
         with Scope():
             bi.discard(a)
@@ -849,15 +788,15 @@
         pytest.skip()
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 6
     assert any([n.is_copy_node() for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_copyable_capture_out_once(bi, client: RuntimeClient) -> None:
+async def test_copyable_capture_out_once(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         with Scope():
             a = Copyable(Const(3))
         bi.discard(a)
         return Output()
 
@@ -866,15 +805,17 @@
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 4
     assert not any([n.is_copy_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_copyable_capture_out_copied(bi, client: RuntimeClient) -> None:
+async def test_copyable_capture_out_copied(
+    bi: Namespace, client: RuntimeClient
+) -> None:
     @graph()
     def g() -> Output:
         with Scope():
             a = Copyable(Const(3))
             bi.discard(a)
         bi.discard(a)
         return Output()
@@ -884,15 +825,15 @@
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 4
     assert not any([n.is_copy_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_copyable_on_captured_input(bi, client: RuntimeClient) -> None:
+async def test_copyable_on_captured_input(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Const(3)
         with Scope():
             b = Copyable(a)
             bi.discard(b)
         bi.discard(b)
@@ -903,15 +844,15 @@
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 5
     assert not any([n.is_copy_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_copyable_dont_use(bi, client: RuntimeClient) -> None:
+async def test_copyable_dont_use(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Const(3)
         with Scope():
             b = Copyable(a)
         bi.discard(b)
         return Output()
@@ -921,15 +862,15 @@
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 5
     assert not any([n.is_copy_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_unpack_capture_in(bi, client: RuntimeClient) -> None:
+async def test_unpack_capture_in(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         a = Const(StructValue({"a": IntValue(1), "b": StringValue("hello")}))
         with Scope():
             bi.discard(a["a"])
         return Output()
 
@@ -938,15 +879,15 @@
     tc_graph = await client.type_check_graph(g)
     assert tc_graph.n_nodes == 6
     assert any([n.is_unpack_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.asyncio
-async def test_unpack_capture_out(bi, client: RuntimeClient) -> None:
+async def test_unpack_capture_out(bi: Namespace, client: RuntimeClient) -> None:
     @graph()
     def g() -> Output:
         with Scope():
             a = Const(StructValue({"a": IntValue(1), "b": StringValue("hello")}))
         bi.discard(a["a"])
         return Output()
 
@@ -956,30 +897,32 @@
     assert tc_graph.n_nodes == 4
     assert not any([n.is_unpack_node() for n in tc_graph.nodes()])
     assert any([isinstance(n, BoxNode) for n in tc_graph.nodes()])
 
 
 @pytest.mark.skip_typecheck
 @pytest.mark.asyncio
-async def test_parmap_builder(bi: Namespace, sig, pyruntime: PyRuntime) -> None:
+async def test_parmap_builder(
+    bi: Namespace, sig: Signature, pyruntime: PyRuntime
+) -> None:
     client = pyruntime  # We expect to make this pass for Rust runtime too soon
 
     @lazy_graph()
     def const_vec() -> Output:
         return Output(vec=Const([]))
 
     @lazy_graph(type_check_sig=sig)
-    def par_map_builder(f, ins) -> Output:
+    def par_map_builder(f: ValueSource, ins: ValueSource) -> Output:
         """Returns a graph which when evaluated applies f to each value in inps
         and collates the results."""
         f = bi.parallel(f, Const(rename_ports_graph({"vec": "vec"})))
         f = bi.sequence(f, Const(bi.push.to_graph(input_map={"item": "out"})))
 
         @loop()
-        def built(loop_dat) -> Output:
+        def built(loop_dat):
             vec: ValueSource = Copyable(loop_dat["vec"])
             with IfElse(bi.eq(Const([]), vec)) as loop_ifelse:
                 with If():
                     Break(loop_dat["big_g"])
                 with Else():
                     vec, i = bi.pop(vec)
 
@@ -990,15 +933,15 @@
             return Output(loop_ifelse.nref)
 
         par_f = built(bi.make_struct(vec=ins, big_g=Const(const_vec)))
 
         return Output(par_f)
 
     @graph()
-    def func(inp) -> Output:
+    def func(inp: ValueSource) -> Output:
         return Output(out=bi.imul(inp, Const(2)))
 
     ins = [2387, 123, 64]
     out = await client.run_graph(par_map_builder.graph, f=func, ins=ins)
 
     gv = out["value"]
 
@@ -1015,11 +958,12 @@
 
     # tg contains some type info, but has never been fully type-checked.
     # expected_graph contains no type information.
     # For comparison, we must make the two contain the same type information.
     tg = await client.type_check_graph(tg)
     exp = await client.type_check_graph(expected_graph)
     tg.name = exp.name
+    tg.output_order = ["vec"]
     assert _compare_graphs(tg, exp)
     out = await client.run_graph(tg)
 
     assert out["vec"].try_autopython() == [x * 2 for x in reversed(ins)]
```

### Comparing `tierkreis-0.6.1/tests/test_commontypes.py` & `tierkreis-0.7.0/tests/test_commontypes.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_frontend.py` & `tierkreis-0.7.0/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_generics.py` & `tierkreis-0.7.0/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_pyruntime.py` & `tierkreis-0.7.0/tests/test_pyruntime.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_pytket_worker.py` & `tierkreis-0.7.0/tests/test_pytket_worker.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_tierkreis_graph.py` & `tierkreis-0.7.0/tests/test_tierkreis_graph.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tests/test_type_check.py` & `tierkreis-0.7.0/tests/test_type_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Const,
     Continue,
     Else,
     If,
     IfElse,
     Output,
     Scope,
+    ValueSource,
     closure,
     graph,
     lazy_graph,
     loop,
 )
 from tierkreis.client import RuntimeClient, ServerRuntime
 from tierkreis.core.function import FunctionDeclaration
@@ -254,15 +255,15 @@
                 # ERROR
                 pass
         return Output()
 
     @lazy_graph(type_check_sig=sig)
     def lop() -> Output:
         @loop()
-        def lopdef(x) -> Output:
+        def lopdef(x):
             # ERROR
             with IfElse(Const(True)):
                 with If():
                     # ERROR
                     Continue(bi.iadd(Const(1), Const(1.0)))
                 with Else():
                     # ERROR
@@ -277,44 +278,44 @@
     @lazy_graph(type_check_sig=sig)
     def clos1() -> Output:
         # ERROR
         y = Const(1.0)
 
         @closure()
         # ERROR
-        def clos_def(x) -> Output:
+        def clos_def(x):
             # ERROR
             bi.iadd(x, y)
             return Output()
 
         return Output()
 
     @lazy_graph(type_check_sig=sig)
     def clos2() -> Output:
         @closure()
         # ERROR
-        def clos_def(x) -> Output:
+        def clos_def(x):
             # ERROR
             bi.iadd(x, Const(1))
             return Output()
 
         # ERROR
         _y = clos_def(Const(1.0))
 
         return Output()
 
     @lazy_graph(type_check_sig=sig)
-    def scop(x) -> Output:
+    def scop(x: ValueSource) -> Output:
         # ERROR
         with Scope():
             # ERROR
             with Scope():
                 # ERROR
-                x = _bad_nod()
-        return Output(x)
+                x2 = _bad_nod()
+        return Output(x2)
 
     for g in (ifelse, lop, clos1, clos2, scop):
         with pytest.raises(TierkreisTypeErrors) as e:
             _ = g.graph
         if (
             sys.platform.startswith("win")
             or int(platform.python_version_tuple()[1]) > 10
```

### Comparing `tierkreis-0.6.1/tests/test_variants.py` & `tierkreis-0.7.0/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/_build/generate_protos.py` & `tierkreis-0.7.0/tierkreis/_build/generate_protos.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/builder.py` & `tierkreis-0.7.0/tierkreis/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 from itertools import count
 from types import FrameType, TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
-    Generic,
     Iterable,
     Iterator,
     Mapping,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
-    get_args,
-    get_origin,
-    get_type_hints,
     overload,
 )
 
 from yachalk import chalk
 
 from tierkreis.core import Labels
 from tierkreis.core.function import FunctionDeclaration, FunctionName
@@ -45,20 +41,18 @@
     TagNode,
     TierkreisGraph,
     TierkreisNode,
     to_nodeport,
 )
 from tierkreis.core.type_errors import TierkreisTypeErrors
 from tierkreis.core.type_inference import infer_graph_types
-from tierkreis.core.types import TupleLabel, TypeScheme, UnionTag, UnpackRow
+from tierkreis.core.types import TupleLabel, TypeScheme, UnionTag
 from tierkreis.core.utils import graph_from_func, map_vals, rename_ports_graph
 from tierkreis.core.values import (
     TierkreisValue,
-    TKVal1,
-    tkvalue_to_tktype,
 )
 
 if TYPE_CHECKING:
     from tierkreis.core.types import GraphType, TierkreisType
 
 
 # magic for lazily creating nodes (and returning ports thereof)
@@ -155,32 +149,32 @@
 
 
 TGBuilder = TypeVar("TGBuilder", bound="GraphBuilder")
 
 
 class GraphBuilder(AbstractContextManager):
     graph: TierkreisGraph
-    inputs: dict[str, Optional["TierkreisType"]]
-    outputs: dict[str, Optional["TierkreisType"]]
+    inputs: list[str]
+    outputs: list[str]
     inner_scopes: dict[TierkreisGraph, CaptureOutwards]
     debug_info: dict[NodeRef, str]
     _state_token: Token["GraphBuilder"]
 
     def __init__(
         self,
-        inputs: Optional[Dict[str, Optional["TierkreisType"]]] = None,
-        outputs: Optional[Dict[str, Optional["TierkreisType"]]] = None,
+        inputs: list[str] | None = None,
+        outputs: list[str] | None = None,
         name: str = "",
         debug: bool = True,
     ) -> None:
         self.graph = TierkreisGraph(name)
-        self.inputs = inputs or {}
-        self.outputs = outputs or {}
+        self.inputs = inputs or []
+        self.outputs = outputs or []
         self.inner_scopes = {}
-        self.graph.input_order.extend(self.inputs.keys())
+        self.graph.input_order.extend(self.inputs)
         self.debug_info = {self.graph.input: _debug_str()} if debug else {}
 
     def input(self, name: str) -> NodePort:
         if name in self.inputs:
             return self.graph.input[name]
         raise RuntimeError("Input not declared.")
 
@@ -220,18 +214,14 @@
         nr: NodeRef,
         /,
         **incoming_wires: ValueSource,
     ) -> None:
         for tgt_port, vs in incoming_wires.items():
             src = _resolve(self.capture(vs))
             self.graph.add_edge(src, nr[tgt_port])
-            if src.node_ref == self.graph.input and (
-                inp_typ := self.inputs.get(src.port)
-            ):
-                self.graph.annotate_input(src.port, inp_typ)
 
     def add_node_to_graph(
         self,
         _tk_node: TierkreisNode,
         /,
         **incoming_wires: ValueSource,
     ) -> NodeRef:
@@ -254,16 +244,16 @@
 
 
 class CaptureBuilder(GraphBuilder):
     captured: dict[ValueSource, PortID]
 
     def __init__(
         self,
-        inputs: Optional[Dict[str, Optional["TierkreisType"]]] = None,
-        outputs: Optional[Dict[str, Optional["TierkreisType"]]] = None,
+        inputs: list[str] | None = None,
+        outputs: list[str] | None = None,
         name: str = "",
         debug: Optional[bool] = None,
     ) -> None:
         bool_debug = bool(current_builder().debug_info) if debug is None else debug
         super().__init__(inputs, outputs, name, bool_debug)
 
         self.captured = {}
@@ -386,38 +376,28 @@
             current_builder().inner_scopes[graph] = CaptureOutwards(graph, node_ref)
 
 
 def Tag(tag: str, value: ValueSource) -> NodePort:
     return current_builder().add_node_to_graph(TagNode(tag), value=value)[Labels.VALUE]
 
 
-OutAnnotation = TypeVar(
-    "OutAnnotation",
-    bound=Union[UnpackRow, TierkreisValue],
-)
-
-
-class Output(NodeRef, Generic[OutAnnotation]):
+class Output(NodeRef):
     def __init__(self, *args: ValueSource, **kwargs: ValueSource) -> None:
         s = current_builder()
 
         g = s.graph
 
-        for o in s.outputs:
-            g.output_order.append(o)
-
         if len(args) == 1 and len(kwargs) == 0:
             kwargs = {Labels.VALUE: args[0]}
         else:
-            kwargs = _combine_args_with_kwargs(s.outputs.keys(), *args, **kwargs)
+            kwargs = _combine_args_with_kwargs(s.outputs, *args, **kwargs)
 
         s.set_graph_outputs(**kwargs)
         for o in kwargs:
-            if ot := s.outputs.get(o):
-                g.annotate_output(o, ot)
+            g.output_order.append(o)
 
         super().__init__(g.output.idx, g)
 
 
 class _LoopOutput(Output):
     def __init__(self, loopout: ValueSource) -> None:
         super().__init__(value=loopout)
@@ -429,88 +409,23 @@
 
 
 class Break(_LoopOutput):
     def __init__(self, loopout: ValueSource) -> None:
         super().__init__(Tag(Labels.BREAK, loopout))
 
 
-def _vals_to_types(
-    d: dict[str, Optional[Type["TierkreisValue"]]],
-) -> dict[str, Optional["TierkreisType"]]:
-    return map_vals(
-        d, lambda arg: None if (arg is Any or arg is None) else tkvalue_to_tktype(arg)
-    )
-
-
-def _convert_input(t: Optional[Type["Input[TierkreisValue]"]]) -> Optional[Type]:
-    if t is not None:
-        if not (get_origin(t) == Input or t == Input):
-            raise TypeError(
-                "Graph builder function arguments must be ``Input``"
-                " with an optional ``TierkreisValue`` argument."
-                "For example Input[IntValue]"
-            )
-
-        args = get_args(t)
-        if args:
-            return args[0]
-    return None
-
-
-_RETURN_TYPE_ERROR = TypeError(
-    "Graph builder function must be annotated with return type `Output`."
-    " Optionally annotate with "
-    "`Output[TierkreisValue]` for a single return from port 'value',"
-    " or with a `UnpackRow` specifying the Row type of the ouput."
-)
-
-
-def _convert_return(ret: Type) -> dict[str, Optional["TierkreisType"]]:
-    if not (get_origin(ret) == Output or ret == Output):
-        raise _RETURN_TYPE_ERROR
-    args = get_args(ret)
-    if not args:
-        return {}
-    ret = args[0]
-    subc = cast(Type, get_origin(ret) or ret)
-    if issubclass(subc, UnpackRow):
-        return _vals_to_types(get_type_hints(ret))
-    if issubclass(subc, TierkreisValue):
-        return _vals_to_types({Labels.VALUE: ret})
-
-    raise _RETURN_TYPE_ERROR
-
-
-class Input(Generic[TKVal1], NodePort):
-    def __init__(self, port: PortID) -> None:
-        np = current_builder().graph.input[port]
-        super().__init__(np.node_ref, np.port)
+def _input_port(port: PortID) -> NodePort:
+    return current_builder().graph.input[port]
 
 
 _GraphDef = Callable[..., Output]
 
 
-def _get_edge_annotations(
-    f: _GraphDef,
-) -> tuple[
-    dict[str, Optional["TierkreisType"]],
-    dict[str, Optional["TierkreisType"]],
-]:
-    f_sig = inspect.signature(f)
-    inps = map_vals(
-        inspect.signature(f).parameters,
-        lambda x: None if x.annotation is inspect.Signature.empty else x.annotation,
-    )
-    out_types = (
-        {}
-        if f_sig.return_annotation is inspect.Signature.empty
-        else _convert_return(f_sig.return_annotation)
-    )
-    in_types = _vals_to_types(map_vals(inps, _convert_input))
-    return in_types, out_types
+def _get_input_names(f: _GraphDef) -> list[str]:
+    return list(inspect.signature(f).parameters.keys())
 
 
 class CapturedError(Exception):
     pass
 
 
 @dataclass(frozen=True)
@@ -530,28 +445,29 @@
 
 _GraphDecoratorType = Callable[[_GraphDef], TierkreisGraph]
 _LazyGraphDecoratorType = Callable[[_GraphDef], LazyGraph]
 
 
 def lazy_graph(
     name: Optional[str] = None,
-    type_check_sig: Optional[Signature] = None,
+    type_check_sig: Signature | None = None,
+    output_order: list[str] | None = None,
     debug: bool = True,
 ) -> _LazyGraphDecoratorType:
     def decorator_graph(f: _GraphDef) -> LazyGraph:
-        in_types, out_types = _get_edge_annotations(f)
+        input_order = _get_input_names(f)
         # Use getattr as _GraphDef doesn't specify that it has a __name__
         graph_name = name or getattr(f, "__name__")
         # graph_name = name or f.__name__  # type: ignore  # the alternative
 
         def wrapper() -> TierkreisGraph:
-            gb = GraphBuilder(in_types, out_types, name=graph_name, debug=debug)
+            gb = GraphBuilder(input_order, output_order, name=graph_name, debug=debug)
 
             with gb as sub_build:
-                f(*(Input(port) for port in in_types))
+                f(*(_input_port(port) for port in input_order))
 
             return (
                 sub_build.graph
                 if type_check_sig is None
                 else sub_build.type_check(type_check_sig)
             )
 
@@ -559,17 +475,18 @@
 
     return decorator_graph
 
 
 def graph(
     name: Optional[str] = None,
     type_check_sig: Optional[Signature] = None,
+    output_order: list[str] | None = None,
     debug: bool = True,
 ) -> _GraphDecoratorType:
-    dec = lazy_graph(name, type_check_sig, debug)
+    dec = lazy_graph(name, type_check_sig, output_order, debug)
 
     def decorator_graph(f: _GraphDef) -> TierkreisGraph:
         return dec(f).graph
 
     return decorator_graph
 
 
@@ -596,50 +513,48 @@
 
     def source_graph(self) -> TierkreisGraph:
         """The graph the port belongs to (or will)."""
         return _source_graph(self.graph_src)
 
 
 def closure(
-    name: Optional[str] = None, debug: bool = True
+    name: Optional[str] = None,
+    debug: bool = True,
+    output_order: list[str] | None = None,
 ) -> Callable[[_GraphDef], Thunk]:
     def decorator_graph(f: _GraphDef) -> Thunk:
-        in_types, out_types = _get_edge_annotations(f)
+        input_order = _get_input_names(f)
+
         # Use getattr as _GraphDef doesn't specify that it has a __name__
         graph_name = name or getattr(f, "__name__")
         # graph_name = name or f.__name__  # type: ignore  # the alternative
 
-        gb = CaptureBuilder(in_types, out_types, name=graph_name, debug=debug)
+        gb = CaptureBuilder(input_order, output_order, name=graph_name, debug=debug)
 
         with gb as sub_build:
-            f(*(Input(port) for port in in_types))
-        return Thunk(
-            _partial_thunk(sub_build, sub_build.captured),
-            list(in_types.keys()),
-            list(out_types.keys()),
-        )
+            f(*(_input_port(port) for port in input_order))
+        return Thunk(_partial_thunk(sub_build, sub_build.captured), input_order, [])
 
     return decorator_graph
 
 
 def loop(name: Optional[str] = None, debug: bool = True):
     def decorator_graph(f: _GraphDef):
-        in_types, out_types = _get_edge_annotations(f)
-        if len(in_types) != 1:
+        inps = _get_input_names(f)
+        if len(inps) != 1:
             raise ValueError("Loop body graph can only have one input.")
 
         # the loop node has input port "value"
         # allow body definitions to use any input names and map it
-        in_types = {Labels.VALUE: in_types.popitem()[1]}
         graph_name = name or getattr(f, "__name__")
 
         def wrapper(initial: ValueSource) -> NodePort:
-            gb = CaptureBuilder(in_types, out_types, name=graph_name, debug=debug)
+            gb = CaptureBuilder(inps, None, name=graph_name, debug=debug)
             with gb as sub_build:
-                f(Input(Labels.VALUE))
+                f(_input_port(Labels.VALUE))
 
             loop_node = current_builder().add_node_to_graph(
                 FunctionNode(FunctionName("loop")),
                 body=_partial_thunk(sub_build, sub_build.captured),
                 value=initial,
             )
             return loop_node[Labels.VALUE]
```

### Comparing `tierkreis-0.6.1/tierkreis/cli.py` & `tierkreis-0.7.0/tierkreis/cli.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/client/runtime_client.py` & `tierkreis-0.7.0/tierkreis/client/runtime_client.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/client/server_client.py` & `tierkreis-0.7.0/tierkreis/client/server_client.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/common_types/__init__.py` & `tierkreis-0.7.0/tierkreis/common_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/common_types/circuit.py` & `tierkreis-0.7.0/tierkreis/common_types/circuit.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/function.py` & `tierkreis-0.7.0/tierkreis/core/function.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/graphviz.py` & `tierkreis-0.7.0/tierkreis/core/graphviz.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/internal.py` & `tierkreis-0.7.0/tierkreis/core/internal.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/opaque_model.py` & `tierkreis-0.7.0/tierkreis/core/opaque_model.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py` & `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: v1alpha/graph.proto
+# sources: v1alpha1/graph.proto
 # plugin: python-betterproto
 # This file has been @generated
 import builtins
 from dataclasses import dataclass
 from typing import (
     Dict,
     List,
+    Optional,
 )
 
 import betterproto
 
 
 @dataclass(eq=False, repr=False)
 class Location(betterproto.Message):
@@ -117,26 +118,34 @@
 @dataclass(eq=False, repr=False)
 class FunctionName(betterproto.Message):
     namespaces: List[str] = betterproto.string_field(1)
     name: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
+class FunctionNode(betterproto.Message):
+    name: "FunctionName" = betterproto.message_field(1)
+    retry_secs: Optional[int] = betterproto.uint32_field(
+        2, optional=True, group="_retry_secs"
+    )
+
+
+@dataclass(eq=False, repr=False)
 class BoxNode(betterproto.Message):
     loc: "Location" = betterproto.message_field(1)
     graph: "Graph" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class Node(betterproto.Message):
     input: "Empty" = betterproto.message_field(1, group="node")
     output: "Empty" = betterproto.message_field(2, group="node")
     const: "Value" = betterproto.message_field(3, group="node")
     box: "BoxNode" = betterproto.message_field(4, group="node")
-    function: "FunctionName" = betterproto.message_field(5, group="node")
+    function: "FunctionNode" = betterproto.message_field(5, group="node")
     match: "Empty" = betterproto.message_field(6, group="node")
     tag: str = betterproto.string_field(7, group="node")
 
 
 @dataclass(eq=False, repr=False)
 class Edge(betterproto.Message):
     port_from: str = betterproto.string_field(1)
```

### Comparing `tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py` & `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: v1alpha/runtime.proto
+# sources: v1alpha1/jobs.proto
 # plugin: python-betterproto
+# This file has been @generated
+
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Dict,
     List,
     Optional,
 )
@@ -22,304 +24,262 @@
 if TYPE_CHECKING:
     import grpclib.server
     from betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class Callback(betterproto.Message):
-    uri: str = betterproto.string_field(1)
-    loc: "_graph__.Location" = betterproto.message_field(2)
-
-
-@dataclass(eq=False, repr=False)
-class RunTaskRequest(betterproto.Message):
+class StartJobRequest(betterproto.Message):
     graph: "_graph__.Graph" = betterproto.message_field(1)
     inputs: "_graph__.StructValue" = betterproto.message_field(2)
+    job_id: str = betterproto.string_field(3)
 
 
 @dataclass(eq=False, repr=False)
-class RunTaskResponse(betterproto.Message):
-    task_id: str = betterproto.string_field(1, group="result")
+class StartJobResponse(betterproto.Message):
+    job_id: str = betterproto.string_field(1, group="result")
     type_errors: "_signature__.TypeErrors" = betterproto.message_field(
         2, group="result"
     )
+    runtime_error: str = betterproto.string_field(3, group="result")
 
 
 @dataclass(eq=False, repr=False)
-class ListTasksRequest(betterproto.Message):
+class RunningJobsRequest(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
-class ListTasksResponse(betterproto.Message):
-    tasks: List["Task"] = betterproto.message_field(1)
+class RunningJobsResponse(betterproto.Message):
+    jobs: List["JobStatus"] = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class DeleteTaskRequest(betterproto.Message):
+class StopJobRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class DeleteTaskResponse(betterproto.Message):
+class StopJobResponse(betterproto.Message):
     pass
 
 
 @dataclass(eq=False, repr=False)
-class GetTaskRequest(betterproto.Message):
+class JobStatusRequest(betterproto.Message):
     id: str = betterproto.string_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class GetTaskResponse(betterproto.Message):
-    task: "Task" = betterproto.message_field(1)
+class JobStatusResponse(betterproto.Message):
+    status: "JobStatus" = betterproto.message_field(1)
 
 
 @dataclass(eq=False, repr=False)
-class AwaitTaskRequest(betterproto.Message):
-    id: str = betterproto.string_field(1)
-    timeout: int = betterproto.uint64_field(2)
-
+class Empty(betterproto.Message):
+    """
+    This is supposed to be `google.protobuf.Empty` but unfortunately there is
+    no support for this in `betterproto` yet.
+    """
 
-@dataclass(eq=False, repr=False)
-class AwaitTaskResponse(betterproto.Message):
-    task: "Task" = betterproto.message_field(1)
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class Task(betterproto.Message):
+class JobStatus(betterproto.Message):
     id: str = betterproto.string_field(1)
-    success: "_graph__.StructValue" = betterproto.message_field(2, group="status")
-    error: str = betterproto.string_field(3, group="status")
+    success: "Empty" = betterproto.message_field(2, group="status")
+    running: "Empty" = betterproto.message_field(3, group="status")
+    error: str = betterproto.string_field(4, group="status")
 
 
 @dataclass(eq=False, repr=False)
-class RunGraphRequest(betterproto.Message):
-    graph: "_graph__.Graph" = betterproto.message_field(1)
-    inputs: "_graph__.StructValue" = betterproto.message_field(2)
-    type_check: bool = betterproto.bool_field(3)
-    loc: "_graph__.Location" = betterproto.message_field(4)
-    escape: "Callback" = betterproto.message_field(5)
+class DeleteCompletedRequest(betterproto.Message):
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class RunGraphResponse(betterproto.Message):
-    success: "_graph__.StructValue" = betterproto.message_field(1, group="result")
-    error: str = betterproto.string_field(2, group="result")
-    type_errors: "_signature__.TypeErrors" = betterproto.message_field(
-        3, group="result"
-    )
-
+class DeleteCompletedResponse(betterproto.Message):
+    job_ids: List[str] = betterproto.string_field(1)
+    """ids of deleted jobs"""
 
-class RuntimeStub(betterproto.ServiceStub):
-    async def list_tasks(
-        self,
-        list_tasks_request: "ListTasksRequest",
-        *,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "ListTasksResponse":
-        return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/ListTasks",
-            list_tasks_request,
-            ListTasksResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
 
-    async def run_task(
+class JobControlStub(betterproto.ServiceStub):
+    async def running_jobs(
         self,
-        run_task_request: "RunTaskRequest",
+        running_jobs_request: "RunningJobsRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "RunTaskResponse":
+    ) -> "RunningJobsResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/RunTask",
-            run_task_request,
-            RunTaskResponse,
+            "/tierkreis.v1alpha1.jobs.JobControl/RunningJobs",
+            running_jobs_request,
+            RunningJobsResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def get_task(
+    async def start_job(
         self,
-        get_task_request: "GetTaskRequest",
+        start_job_request: "StartJobRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "GetTaskResponse":
+    ) -> "StartJobResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/GetTask",
-            get_task_request,
-            GetTaskResponse,
+            "/tierkreis.v1alpha1.jobs.JobControl/StartJob",
+            start_job_request,
+            StartJobResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def await_task(
+    async def job_status(
         self,
-        await_task_request: "AwaitTaskRequest",
+        job_status_request: "JobStatusRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "AwaitTaskResponse":
+    ) -> "JobStatusResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/AwaitTask",
-            await_task_request,
-            AwaitTaskResponse,
+            "/tierkreis.v1alpha1.jobs.JobControl/JobStatus",
+            job_status_request,
+            JobStatusResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def delete_task(
+    async def stop_job(
         self,
-        delete_task_request: "DeleteTaskRequest",
+        stop_job_request: "StopJobRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "DeleteTaskResponse":
+    ) -> "StopJobResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/DeleteTask",
-            delete_task_request,
-            DeleteTaskResponse,
+            "/tierkreis.v1alpha1.jobs.JobControl/StopJob",
+            stop_job_request,
+            StopJobResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    async def run_graph(
+    async def delete_completed(
         self,
-        run_graph_request: "RunGraphRequest",
+        delete_completed_request: "DeleteCompletedRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "RunGraphResponse":
+    ) -> "DeleteCompletedResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.runtime.Runtime/RunGraph",
-            run_graph_request,
-            RunGraphResponse,
+            "/tierkreis.v1alpha1.jobs.JobControl/DeleteCompleted",
+            delete_completed_request,
+            DeleteCompletedResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
 
-class RuntimeBase(ServiceBase):
-    async def list_tasks(
-        self, list_tasks_request: "ListTasksRequest"
-    ) -> "ListTasksResponse":
-        raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
+class JobControlBase(ServiceBase):
 
-    async def run_task(self, run_task_request: "RunTaskRequest") -> "RunTaskResponse":
+    async def running_jobs(
+        self, running_jobs_request: "RunningJobsRequest"
+    ) -> "RunningJobsResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def get_task(self, get_task_request: "GetTaskRequest") -> "GetTaskResponse":
+    async def start_job(
+        self, start_job_request: "StartJobRequest"
+    ) -> "StartJobResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def await_task(
-        self, await_task_request: "AwaitTaskRequest"
-    ) -> "AwaitTaskResponse":
+    async def job_status(
+        self, job_status_request: "JobStatusRequest"
+    ) -> "JobStatusResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def delete_task(
-        self, delete_task_request: "DeleteTaskRequest"
-    ) -> "DeleteTaskResponse":
+    async def stop_job(self, stop_job_request: "StopJobRequest") -> "StopJobResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def run_graph(
-        self, run_graph_request: "RunGraphRequest"
-    ) -> "RunGraphResponse":
+    async def delete_completed(
+        self, delete_completed_request: "DeleteCompletedRequest"
+    ) -> "DeleteCompletedResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
-    async def __rpc_list_tasks(
-        self, stream: "grpclib.server.Stream[ListTasksRequest, ListTasksResponse]"
-    ) -> None:
-        request = await stream.recv_message()
-        response = await self.list_tasks(request)
-        await stream.send_message(response)
-
-    async def __rpc_run_task(
-        self, stream: "grpclib.server.Stream[RunTaskRequest, RunTaskResponse]"
+    async def __rpc_running_jobs(
+        self, stream: "grpclib.server.Stream[RunningJobsRequest, RunningJobsResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.run_task(request)
+        response = await self.running_jobs(request)
         await stream.send_message(response)
 
-    async def __rpc_get_task(
-        self, stream: "grpclib.server.Stream[GetTaskRequest, GetTaskResponse]"
+    async def __rpc_start_job(
+        self, stream: "grpclib.server.Stream[StartJobRequest, StartJobResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.get_task(request)
+        response = await self.start_job(request)
         await stream.send_message(response)
 
-    async def __rpc_await_task(
-        self, stream: "grpclib.server.Stream[AwaitTaskRequest, AwaitTaskResponse]"
+    async def __rpc_job_status(
+        self, stream: "grpclib.server.Stream[JobStatusRequest, JobStatusResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.await_task(request)
+        response = await self.job_status(request)
         await stream.send_message(response)
 
-    async def __rpc_delete_task(
-        self, stream: "grpclib.server.Stream[DeleteTaskRequest, DeleteTaskResponse]"
+    async def __rpc_stop_job(
+        self, stream: "grpclib.server.Stream[StopJobRequest, StopJobResponse]"
     ) -> None:
         request = await stream.recv_message()
-        response = await self.delete_task(request)
+        response = await self.stop_job(request)
         await stream.send_message(response)
 
-    async def __rpc_run_graph(
-        self, stream: "grpclib.server.Stream[RunGraphRequest, RunGraphResponse]"
+    async def __rpc_delete_completed(
+        self,
+        stream: "grpclib.server.Stream[DeleteCompletedRequest, DeleteCompletedResponse]",
     ) -> None:
         request = await stream.recv_message()
-        response = await self.run_graph(request)
+        response = await self.delete_completed(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/tierkreis.v1alpha.runtime.Runtime/ListTasks": grpclib.const.Handler(
-                self.__rpc_list_tasks,
-                grpclib.const.Cardinality.UNARY_UNARY,
-                ListTasksRequest,
-                ListTasksResponse,
-            ),
-            "/tierkreis.v1alpha.runtime.Runtime/RunTask": grpclib.const.Handler(
-                self.__rpc_run_task,
+            "/tierkreis.v1alpha1.jobs.JobControl/RunningJobs": grpclib.const.Handler(
+                self.__rpc_running_jobs,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                RunTaskRequest,
-                RunTaskResponse,
+                RunningJobsRequest,
+                RunningJobsResponse,
             ),
-            "/tierkreis.v1alpha.runtime.Runtime/GetTask": grpclib.const.Handler(
-                self.__rpc_get_task,
+            "/tierkreis.v1alpha1.jobs.JobControl/StartJob": grpclib.const.Handler(
+                self.__rpc_start_job,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                GetTaskRequest,
-                GetTaskResponse,
+                StartJobRequest,
+                StartJobResponse,
             ),
-            "/tierkreis.v1alpha.runtime.Runtime/AwaitTask": grpclib.const.Handler(
-                self.__rpc_await_task,
+            "/tierkreis.v1alpha1.jobs.JobControl/JobStatus": grpclib.const.Handler(
+                self.__rpc_job_status,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                AwaitTaskRequest,
-                AwaitTaskResponse,
+                JobStatusRequest,
+                JobStatusResponse,
             ),
-            "/tierkreis.v1alpha.runtime.Runtime/DeleteTask": grpclib.const.Handler(
-                self.__rpc_delete_task,
+            "/tierkreis.v1alpha1.jobs.JobControl/StopJob": grpclib.const.Handler(
+                self.__rpc_stop_job,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                DeleteTaskRequest,
-                DeleteTaskResponse,
+                StopJobRequest,
+                StopJobResponse,
             ),
-            "/tierkreis.v1alpha.runtime.Runtime/RunGraph": grpclib.const.Handler(
-                self.__rpc_run_graph,
+            "/tierkreis.v1alpha1.jobs.JobControl/DeleteCompleted": grpclib.const.Handler(
+                self.__rpc_delete_completed,
                 grpclib.const.Cardinality.UNARY_UNARY,
-                RunGraphRequest,
-                RunGraphResponse,
+                DeleteCompletedRequest,
+                DeleteCompletedResponse,
             ),
         }
```

### Comparing `tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py` & `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: v1alpha/signature.proto
+# sources: v1alpha1/signature.proto
 # plugin: python-betterproto
 # This file has been @generated
 
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Dict,
@@ -167,15 +167,15 @@
         list_functions_request: "ListFunctionsRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "ListFunctionsResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.signature.Signature/ListFunctions",
+            "/tierkreis.v1alpha1.signature.Signature/ListFunctions",
             list_functions_request,
             ListFunctionsResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
@@ -186,15 +186,15 @@
         infer_type_request: "InferTypeRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "InferTypeResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.signature.TypeInference/InferType",
+            "/tierkreis.v1alpha1.signature.TypeInference/InferType",
             infer_type_request,
             InferTypeResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
@@ -212,15 +212,15 @@
     ) -> None:
         request = await stream.recv_message()
         response = await self.list_functions(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/tierkreis.v1alpha.signature.Signature/ListFunctions": grpclib.const.Handler(
+            "/tierkreis.v1alpha1.signature.Signature/ListFunctions": grpclib.const.Handler(
                 self.__rpc_list_functions,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 ListFunctionsRequest,
                 ListFunctionsResponse,
             ),
         }
 
@@ -237,14 +237,14 @@
     ) -> None:
         request = await stream.recv_message()
         response = await self.infer_type(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/tierkreis.v1alpha.signature.TypeInference/InferType": grpclib.const.Handler(
+            "/tierkreis.v1alpha1.signature.TypeInference/InferType": grpclib.const.Handler(
                 self.__rpc_infer_type,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 InferTypeRequest,
                 InferTypeResponse,
             ),
         }
```

### Comparing `tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py` & `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: v1alpha/worker.proto
+# sources: v1alpha1/worker.proto
 # plugin: python-betterproto
+# This file has been @generated
+
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     Dict,
     Optional,
 )
 
@@ -43,38 +45,39 @@
         run_function_request: "RunFunctionRequest",
         *,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "RunFunctionResponse":
         return await self._unary_unary(
-            "/tierkreis.v1alpha.worker.Worker/RunFunction",
+            "/tierkreis.v1alpha1.worker.Worker/RunFunction",
             run_function_request,
             RunFunctionResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
 
 class WorkerBase(ServiceBase):
+
     async def run_function(
         self, run_function_request: "RunFunctionRequest"
     ) -> "RunFunctionResponse":
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
 
     async def __rpc_run_function(
         self, stream: "grpclib.server.Stream[RunFunctionRequest, RunFunctionResponse]"
     ) -> None:
         request = await stream.recv_message()
         response = await self.run_function(request)
         await stream.send_message(response)
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
-            "/tierkreis.v1alpha.worker.Worker/RunFunction": grpclib.const.Handler(
+            "/tierkreis.v1alpha1.worker.Worker/RunFunction": grpclib.const.Handler(
                 self.__rpc_run_function,
                 grpclib.const.Cardinality.UNARY_UNARY,
                 RunFunctionRequest,
                 RunFunctionResponse,
             ),
         }
```

### Comparing `tierkreis-0.6.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py` & `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/python.py` & `tierkreis-0.7.0/tierkreis/core/python.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/signature.py` & `tierkreis-0.7.0/tierkreis/core/signature.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/tierkreis_graph.py` & `tierkreis-0.7.0/tierkreis/core/tierkreis_graph.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/type_errors.py` & `tierkreis-0.7.0/tierkreis/core/type_errors.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/type_inference.py` & `tierkreis-0.7.0/tierkreis/core/type_inference.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/types.py` & `tierkreis-0.7.0/tierkreis/core/types.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/utils.py` & `tierkreis-0.7.0/tierkreis/core/utils.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/core/values.py` & `tierkreis-0.7.0/tierkreis/core/values.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,20 @@
     Generic,
     Iterable,
     Mapping,
     Optional,
     Protocol,
     TypeVar,
     cast,
-    get_args,
-    get_origin,
-    get_type_hints,
 )
 from uuid import UUID
 
 import betterproto
 
 import tierkreis.core.protos.tierkreis.v1alpha1.graph as pg
-from tierkreis.core import types as TKType
 from tierkreis.core.internal import (
     ClassField,
     FieldExtractionError,
     generic_origin,
     python_struct_fields,
 )
 from tierkreis.core.opaque_model import (
@@ -723,53 +719,14 @@
     def from_proto(cls, value: pg.VariantValue) -> "TierkreisValue":
         return VariantValue(value.tag, TierkreisValue.from_proto(value.value))
 
 
 option_none: VariantValue = VariantValue(UnionTag.none_type_tag(), StructValue({}))
 
 
-def _typeddict_to_row(typeddict: dict[str, TierkreisValue]) -> TKType.Row:
-    return TKType.Row(
-        {key: tkvalue_to_tktype(val) for key, val in get_type_hints(typeddict).items()}
-    )
-
-
-def tkvalue_to_tktype(val_cls: typing.Type[TierkreisValue]) -> TierkreisType:
-    if get_origin(val_cls) == VecValue:
-        (inner,) = get_args(val_cls)
-        return TKType.VecType(tkvalue_to_tktype(inner))
-    if get_origin(val_cls) == VariantValue:
-        (typeddict,) = get_args(val_cls)
-        return TKType.VariantType(_typeddict_to_row(typeddict))
-
-    if get_origin(val_cls) == StructValue:
-        (typeddict,) = get_args(val_cls)
-        return TKType.StructType(_typeddict_to_row(typeddict))
-    if get_origin(val_cls) == PairValue:
-        first, second = get_args(val_cls)
-        return TKType.PairType(*map(tkvalue_to_tktype, (first, second)))
-    if get_origin(val_cls) == MapValue:
-        first, second = get_args(val_cls)
-        return TKType.MapType(*map(tkvalue_to_tktype, (first, second)))
-
-    if val_cls == IntValue:
-        return TKType.IntType()
-
-    if val_cls == BoolValue:
-        return TKType.BoolType()
-
-    if val_cls == FloatValue:
-        return TKType.FloatType()
-
-    if val_cls == StringValue:
-        return TKType.StringType()
-
-    raise ValueError("Cannot convert value class.")
-
-
 def _val_known_type(type_: typing.Type, value: Any) -> TierkreisValue:
     """Convert a python `value` to a TierkreisValue, given a python type annotation."""
     if type_ is int:
         return IntValue(value)
     if type_ is bool:
         return BoolValue(value)
     if type_ is float:
```

### Comparing `tierkreis-0.6.1/tierkreis/pyruntime/python_builtin.py` & `tierkreis-0.7.0/tierkreis/pyruntime/python_builtin.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/pyruntime/python_runtime.py` & `tierkreis-0.7.0/tierkreis/pyruntime/python_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 elif fname.namespaces == [] and fname.name == "map":
                     return await self._run_map(inps)
                 else:
                     function = self.root.get_function(fname)
                     if function is None:
                         raise FunctionNotFound(fname)
                     # For now the PyRuntime does not provide a stack trace
-                    return (await function.run(self, bytes(), StructValue(inps))).values
+                    return (await function.run(self, dict(), StructValue(inps))).values
 
             elif isinstance(tk_node, BoxNode):
                 return await self.run_graph(
                     tk_node.graph,
                     **inps,
                 )
```

### Comparing `tierkreis-0.6.1/tierkreis/worker/callback.py` & `tierkreis-0.7.0/tierkreis/worker/callback.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/worker/exceptions.py` & `tierkreis-0.7.0/tierkreis/worker/exceptions.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/worker/namespace.py` & `tierkreis-0.7.0/tierkreis/worker/namespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,26 @@
 
 import dataclasses
 import typing
 from ctypes import ArgumentError
 from dataclasses import dataclass, make_dataclass
 from functools import wraps
 from inspect import getdoc, isclass
-from typing import Awaitable, Callable, Dict, List, Mapping, Optional, Type, Union, cast
+from typing import (
+    Awaitable,
+    Callable,
+    Dict,
+    List,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Type,
+    Union,
+    cast,
+)
 
 from tierkreis.client.runtime_client import RuntimeClient
 from tierkreis.core.function import FunctionDeclaration, FunctionName
 from tierkreis.core.signature import Namespace as SigNamespace
 from tierkreis.core.signature import Signature
 from tierkreis.core.tierkreis_graph import Location
 from tierkreis.core.types import (
@@ -35,21 +46,26 @@
     NodeExecutionError,
 )
 
 from .tracing import get_tracer, span
 
 tracer = get_tracer(__name__)
 
+Metadata = MutableMapping[str, str | bytes]
+
+METADATA_ARG = "tierkreis_metadata"
+CALLBACK_ARG = "client"
+
 
 @dataclass
 class Function:
     """Registered python function.
     The second (bytes) argument is an encoded stack-trace."""
 
-    run: Callable[[RuntimeClient, bytes, StructValue], Awaitable[StructValue]]
+    run: Callable[[RuntimeClient, Metadata, StructValue], Awaitable[StructValue]]
     declaration: FunctionDeclaration
 
 
 def _snake_to_pascal(name: str) -> str:
     return name.replace("_", " ").title().replace(" ", "")
 
 
@@ -153,15 +169,15 @@
 
     def function(
         self,
         name: Optional[str] = None,
         constraints: Optional[List[Constraint]] = None,
         type_vars: Optional[Dict[Union[str, typing.TypeVar], Kind]] = None,
         callback: bool = False,
-        pass_stack: bool = False,
+        metadata_keys: list[str] | None = None,
     ) -> Callable[[Callable], Callable]:
         """Decorator to mark python function as available Namespace."""
 
         def decorator(func: Callable) -> Callable:
             func_name = name or func.__name__
 
             # Get input and output type hints
@@ -173,26 +189,26 @@
 
             struct_input = "inputs" in type_hints and _check_tkstruct_hint(
                 type_hints["inputs"]
             )
 
             if callback:
                 try:
-                    type_hints.pop("client")
+                    type_hints.pop(CALLBACK_ARG)
                 except KeyError:
                     raise ArgumentError(
                         "Functions with callbacks must have an argument 'client'"
                     )
 
-            if pass_stack:
+            if metadata_keys is not None:
                 try:
-                    type_hints.pop("stack")
+                    type_hints.pop(METADATA_ARG)
                 except KeyError:
                     raise ArgumentError(
-                        "Functions asking for stack trace must have an argument 'stack'"
+                        f"Functions asking for metadata values must have an argument '{METADATA_ARG}'"
                     )
 
             hint_inputs: Type = (
                 type_hints["inputs"]
                 if struct_input
                 else make_dataclass(
                     f"{_snake_to_pascal(func_name)}Inputs", type_hints.items()
@@ -208,15 +224,15 @@
                 )
             )
 
             # Wrap function with input and output conversions
             @wraps(func)
             async def wrapped_func(
                 runtime: RuntimeClient,
-                stack_trace: bytes,
+                metadata: Metadata,
                 inputs: StructValue,
             ) -> StructValue:
                 try:
                     with span(tracer, name="decoding inputs to python type"):
                         python_inputs = (
                             {"inputs": inputs.to_python(hint_inputs)}
                             if struct_input
@@ -225,17 +241,20 @@
                                 for name, val in inputs.values.items()
                             }
                         )
                 except Exception as error:
                     raise DecodeInputError(str(error)) from error
 
                 if callback:
-                    python_inputs["client"] = runtime
-                if pass_stack:
-                    python_inputs["stack"] = stack_trace
+                    python_inputs[CALLBACK_ARG] = runtime
+                if metadata_keys is not None:
+                    # unavailable keys are ignored
+                    python_inputs[METADATA_ARG] = {
+                        k: metadata.pop(k) for k in metadata_keys if k in metadata
+                    }
                 try:
                     python_outputs = await func(**python_inputs)
                 except Exception as error:
                     raise NodeExecutionError(error) from error
 
                 try:
                     with span(tracer, name="encoding outputs from python type"):
```

### Comparing `tierkreis-0.6.1/tierkreis/worker/prelude.py` & `tierkreis-0.7.0/tierkreis/worker/prelude.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/worker/tracing.py` & `tierkreis-0.7.0/tierkreis/worker/tracing.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.6.1/tierkreis/worker/worker.py` & `tierkreis-0.7.0/tierkreis/worker/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Worker server implementation."""
 
 import functools
 import sys
 from contextvars import ContextVar
 from tempfile import TemporaryDirectory
 from traceback import print_tb
-from typing import Any, Callable, Coroutine, Optional, cast
+from typing import Any, Callable, Coroutine, Optional
 
 import grpclib
 import grpclib.events
 import grpclib.server
 from grpclib.const import Status as StatusCode
 from grpclib.exceptions import GRPCError
 from grpclib.server import Server
@@ -31,15 +31,15 @@
 
 from .exceptions import (
     DecodeInputError,
     EncodeOutputError,
     FunctionNotFound,
     NodeExecutionError,
 )
-from .namespace import Namespace
+from .namespace import Metadata, Namespace
 from .tracing import _TRACING, context_token, get_tracer, span
 
 tracer = get_tracer(__name__)
 
 
 async def _event_recv_request(request: grpclib.events.RecvRequest):
     method_func = request.method_func
@@ -95,57 +95,53 @@
 
 class Worker:
     """Worker server."""
 
     root: Namespace
     server: Server
     pyruntime: PyRuntime
-    stack_trace: ContextVar[bytes]
+    metadata: ContextVar[Metadata]
 
     def __init__(self, root_namespace):
         self.root = root_namespace
         self.pyruntime = PyRuntime([root_namespace])
         self.server = Server(
             [SignatureServerImpl(self), WorkerServerImpl(self), RuntimeServerImpl(self)]
         )
-        self.stack_trace = ContextVar("stack_trace")
+        self.metadata = ContextVar("metadata")
 
         # Attach event listener for tracing
         self._add_request_listener(_event_recv_request)
-        # Attach event listener to extract stack trace from metadata
-        self._add_request_listener(self._record_stack_trace)
+        # Attach event listener to extract metadata
+        self._add_request_listener(self._record_metadata)
 
     async def run(
         self,
         function: FunctionName,
         inputs: StructValue,
         callback: pr.Callback,
-        stack_trace: bytes,
+        metadata: Metadata,
     ) -> StructValue:
         """Run function."""
         func = self.root.get_function(function)
         if func is None:
             raise FunctionNotFound(function)
 
         async with callback_server(callback) as cb:
-            return await func.run(cb, stack_trace, inputs)
+            return await func.run(cb, metadata, inputs)
 
-    async def _record_stack_trace(self, request: grpclib.events.RecvRequest) -> None:
-        # Metadata contains Union[str, bytes] but actual type should be bytes for "-bin" keys
-        stack_trace = cast(
-            bytes, request.metadata.pop("tierkreis-stack-trace-bin", None)
-        )
+    async def _record_metadata(self, request: grpclib.events.RecvRequest) -> None:
         method_func = request.method_func
 
         @functools.wraps(method_func)
         async def wrapped(stream: grpclib.server.Stream):
-            token = self.stack_trace.set(stack_trace)
+            token = self.metadata.set(request.metadata)
             await method_func(stream)
             # Good practice but probably not essential:
-            self.stack_trace.reset(token)
+            self.metadata.reset(token)
 
         request.method_func = wrapped
 
     def _add_request_listener(
         self,
         listener: Callable[[grpclib.events.RecvRequest], Coroutine[Any, Any, None]],
     ):
@@ -185,20 +181,20 @@
 
     async def run_function(
         self, run_function_request: pw.RunFunctionRequest
     ) -> RunFunctionResponse:
         function = run_function_request.function
         inputs = run_function_request.inputs
         callback = run_function_request.callback
-        stack_trace = self.worker.stack_trace.get()
+        metadata = self.worker.metadata.get()
         try:
             function_name = FunctionName.from_proto(function)
             inputs_struct = StructValue.from_proto_dict(inputs.map)
             outputs_struct = await self.worker.run(
-                function_name, inputs_struct, callback, stack_trace
+                function_name, inputs_struct, callback, metadata
             )
             with span(tracer, name="encoding python type in RunFunctionResponse proto"):
                 res = RunFunctionResponse(
                     outputs=pg.StructValue(outputs_struct.to_proto_dict())
                 )
             return res
         except DecodeInputError as err:
```

### Comparing `tierkreis-0.6.1/tierkreis.egg-info/PKG-INFO` & `tierkreis-0.7.0/tierkreis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: betterproto[compiler]==2.0.0b6
 Requires-Dist: protobuf<4,>=3.19
 Requires-Dist: grpclib<0.5,>=0.4.3rc
@@ -63,15 +63,15 @@
 
 You can now build a graph (Tierkreis program), optionally type check it and execute it. The recommended environment for this is a Jupyter notebook (especially given some operations are async).
 
 First we need the runtime we are going to execute on and a handle to the primitive functions available on that runtime.
 The python package comes with the `PyRuntime` which runs locally in your python environment.
 
 ```python
-from tierkreis.builder import graph, Namespace, Output, Input
+from tierkreis.builder import graph, Namespace, Output, ValueSource
 from tierkreis.pyruntime import PyRuntime
 
 cl = PyRuntime([]) # empty list for no extra workers
 sig = await cl.get_signature()
 ns = Namespace(sig) # get a handle to all functions
 print(ns.iadd)
 print(ns.unpack_pair)
@@ -85,15 +85,15 @@
 
 ### Build
 
 The `@graph` decorator allows you to build graphs using python functions.
 
 ```python
 @graph()
-def sum_pair(pair: Input) -> Output:
+def sum_pair(pair: ValueSource) -> Output:
     first, second = ns.unpack_pair(pair) # tierkreis functions can have multiple outputs
     return Output(ns.iadd(first, second))
 ```
 
 Calling the decorated function with no arguments (`sum_pair()`) returns a `TierkreisGraph`.
 
 ### Visualise
```

### Comparing `tierkreis-0.6.1/tierkreis.egg-info/SOURCES.txt` & `tierkreis-0.7.0/tierkreis.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -36,19 +36,14 @@
 tierkreis/core/tierkreis_graph.py
 tierkreis/core/type_errors.py
 tierkreis/core/type_inference.py
 tierkreis/core/types.py
 tierkreis/core/utils.py
 tierkreis/core/values.py
 tierkreis/core/protos/__init__.py
-tierkreis/core/protos/tierkreis/v1alpha/__init__.py
-tierkreis/core/protos/tierkreis/v1alpha/graph/__init__.py
-tierkreis/core/protos/tierkreis/v1alpha/runtime/__init__.py
-tierkreis/core/protos/tierkreis/v1alpha/signature/__init__.py
-tierkreis/core/protos/tierkreis/v1alpha/worker/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py
 tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py
 tierkreis/pyruntime/__init__.py
```

### Comparing `tierkreis-0.6.1/tierkreis.egg-info/requires.txt` & `tierkreis-0.7.0/tierkreis.egg-info/requires.txt`

 * *Files identical despite different names*

