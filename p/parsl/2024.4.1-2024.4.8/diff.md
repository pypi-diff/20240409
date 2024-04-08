# Comparing `tmp/parsl-2024.4.1.tar.gz` & `tmp/parsl-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsl-2024.4.1.tar", last modified: Mon Apr  1 22:42:41 2024, max compression
+gzip compressed data, was "parsl-2024.4.8.tar", last modified: Mon Apr  8 22:42:43 2024, max compression
```

## Comparing `parsl-2024.4.1.tar` & `parsl-2024.4.8.tar`

### file list

```diff
@@ -1,533 +1,533 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.171953 parsl-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 22:42:37.000000 parsl-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 22:42:37.000000 parsl-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 22:42:41.167953 parsl-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-01 22:42:37.000000 parsl-2024.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/app/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/benchmark/perf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/oauth_ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/oauth_ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/oauth_ssh/oauth_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/ssh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/channels/ssh_il/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh_il/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/channels/ssh_il/ssh_il.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.111952 parsl-2024.4.1/parsl/concurrent/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/concurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ASPIRE1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/Azure.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ad_hoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/expanse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/illinoiscluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/osg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/polaris.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/stampede2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/toss3_llnl.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/configs/wqex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/data_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/file_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/rsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/data_provider/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/dataflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63593 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/dflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/rundirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/states.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/dataflow/taskrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.115952 parsl-2024.4.1/parsl/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/execute_parsl_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/flux/flux_instance_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/high_throughput/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37225 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/interchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/manager_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/monitoring_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/mpi_prefix_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/mpi_resource_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/probe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    41221 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/process_worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/high_throughput/zmq_pipes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/radical/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/radical/rpex_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10620 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/status_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.119952 parsl-2024.4.1/parsl/executors/taskvine/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    32531 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/factory_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/taskvine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/executors/workqueue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/exec_parsl_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    50038 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/executor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/job_status_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/jobs/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/launchers/launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/log_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/db_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.123952 parsl-2024.4.1/parsl/monitoring/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/queries/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    13900 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/task_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/static/
--rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-logo-white.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-monitor.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/monitoring/visualization/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/app.html
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/dag.html
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/resource_usage.html
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/task.html
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/workflow.html
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/templates/workflows_summary.html
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/monitoring/visualization/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/process_loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/ad_hoc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/ad_hoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/ad_hoc/ad_hoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/aws/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.127952 parsl-2024.4.1/parsl/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/azure/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cluster_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/cobalt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/cobalt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/cobalt/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/condor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/condor/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/googlecloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/googlecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/googlecloud/googlecloud.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/grid_engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/grid_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/grid_engine/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/kube.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/kubernetes/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/lsf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/lsf/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/pbspro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/pbspro.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/pbspro/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/slurm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.131952 parsl-2024.4.1/parsl/providers/torque/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/providers/torque/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.135952 parsl-2024.4.1/parsl/serialize/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/concretes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/serialize/proxystore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.135952 parsl-2024.4.1/parsl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/callables_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.139953 parsl-2024.4.1/parsl/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ad_hoc_cluster_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/azure_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/bluewaters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/bridges.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/cc_in2p3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/cooley_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ec2_single_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/ec2_spot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/frontera.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_ad_hoc_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_alternate.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_intask_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/htex_local_rsync_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_radical.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_radical_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_checkpoint_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_http_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/local_threads_no_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/midway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/nscc_singapore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/osg_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/petrelkube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/summit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/swan_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/taskvine_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/theta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/user_opts.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/configs/workqueue_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/latency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_local_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_scp_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_file_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_parsl_load_default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/integration/test_stress/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.143952 parsl-2024.4.1/parsl/tests/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_ad_hoc_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_log_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_memory_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_oauth_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_regression_220.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_udp_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/manual_tests/test_worker_count.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/scaling_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/htex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/local_threads.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/vineex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/vineex_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/wqex_condor.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/scaling_tests/wqex_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/site_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/site_config_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/site_tests/test_site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/sites/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_dynamic_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_launchers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_local_adhoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.147952 parsl-2024.4.1/parsl/tests/sites/test_mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/sites/test_worker_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_aalst_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_bash_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_apptimeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_keyword_overlaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_kwarg_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_bash_apps/test_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_callables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_channels/test_large_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_periodic.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_232.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_233.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_239.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_checkpointing/test_task_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_curvezmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_from_slides.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_tutorial_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_docs/test_workflow4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.151953 parsl-2024.4.1/parsl/tests/test_error_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_python_walltime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_rand_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_serialization_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_error_handling/test_wrap_with_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_htex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_connected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_cpu_affinity_explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_drain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_htex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_manager_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_missing_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_worker_failure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_htex/test_zmq_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.155953 parsl-2024.4.1/parsl/tests/test_monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_app_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_db_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_fuzz_zmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_incomplete_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_memoization_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_monitoring/test_viz_colouring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.159952 parsl-2024.4.1/parsl/tests/test_mpi_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_mpi_apps/test_resource_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.159952 parsl-2024.4.1/parsl/tests/test_providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_local_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_pbspro_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_slurm_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_slurm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_providers/test_submiterror_deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_python_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_arg_input_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_dep_standard_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_depfail_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_garbage_collect.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_import_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_lifted.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_mapred.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_ignore_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_joinapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_python_apps/test_type5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_radical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_radical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_radical/test_mpi_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_regression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1480.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_1653.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_221.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_226.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_2652.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_69a.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_854.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_97_parallelism_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_regression/test_98.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.163953 parsl-2024.4.1/parsl/tests/test_scaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_block_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_regression_1621.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_scaling/test_shutdown_scalein.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_2555_caching_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_htex_code_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_pack_resource_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_configured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_shutdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_shutdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_shutdown/test_kill_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_staging/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/staging_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_1316.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_docs_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_docs_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_elaborate_noop_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_file_staging.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_output_chain_filenames.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp_in_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_staging/test_staging_https.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_thread_parallelism.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_threads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_threads/test_lazy_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/test_utils/test_representation_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.167953 parsl-2024.4.1/parsl/usage_tracking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/usage_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/usage_tracking/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-01 22:42:37.000000 parsl-2024.4.1/parsl/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-01 22:42:39.000000 parsl-2024.4.1/parsl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:42:41.107952 parsl-2024.4.1/parsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-04-01 22:42:41.000000 parsl-2024.4.1/parsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 22:42:40.000000 parsl-2024.4.1/parsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-01 22:42:37.000000 parsl-2024.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:42:41.171953 parsl-2024.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-04-01 22:42:37.000000 parsl-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 22:42:39.000000 parsl-2024.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 22:42:39.000000 parsl-2024.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 22:42:43.329331 parsl-2024.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-08 22:42:39.000000 parsl-2024.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/app/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/benchmark/perf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl/channels/oauth_ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/oauth_ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/oauth_ssh/oauth_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/channels/ssh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/channels/ssh_il/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh_il/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/channels/ssh_il/ssh_il.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ASPIRE1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/Azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ad_hoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/expanse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/illinoiscluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/osg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/polaris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/stampede2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/toss3_llnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/configs/wqex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.281331 parsl-2024.4.8/parsl/data_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/file_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/data_provider/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/dataflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/dflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/rundirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/dataflow/taskrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/execute_parsl_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/flux/flux_instance_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.285331 parsl-2024.4.8/parsl/executors/high_throughput/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37225 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31491 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/interchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/manager_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/monitoring_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/mpi_prefix_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/mpi_resource_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/probe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41221 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/process_worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/high_throughput/zmq_pipes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/radical/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1368 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/radical/rpex_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/status_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/taskvine/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32531 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/factory_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/taskvine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/executors/workqueue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/exec_parsl_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50038 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/executor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5737 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      735 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/job_status_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/jobs/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.289331 parsl-2024.4.8/parsl/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/launchers/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/log_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37021 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/db_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/queries/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13923 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/task_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14199 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-logo-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      337 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-monitor.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/monitoring/visualization/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/dag.html
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/resource_usage.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/task.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/workflow.html
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/templates/workflows_summary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/monitoring/visualization/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/process_loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.293331 parsl-2024.4.8/parsl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/ad_hoc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/ad_hoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/ad_hoc/ad_hoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29009 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/aws/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18396 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/azure/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cluster_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/cobalt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/cobalt/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/condor/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/googlecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/googlecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/googlecloud/googlecloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/grid_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8565 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/grid_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/grid_engine/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/kube.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/kubernetes/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/lsf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11502 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/lsf/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/pbspro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/pbspro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/pbspro/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.297331 parsl-2024.4.8/parsl/providers/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/slurm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/providers/torque/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/providers/torque/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/concretes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/serialize/proxystore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.301331 parsl-2024.4.8/parsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/callables_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ad_hoc_cluster_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/azure_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/bluewaters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/bridges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/cc_in2p3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/cooley_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ec2_single_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/ec2_spot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/frontera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_ad_hoc_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_alternate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_intask_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/htex_local_rsync_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_radical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_radical_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_dfk_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_checkpoint_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_http_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/local_threads_no_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/midway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/nscc_singapore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/osg_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/petrelkube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/summit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/swan_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/taskvine_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/theta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/user_opts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/configs/workqueue_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/latency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.305331 parsl-2024.4.8/parsl/tests/integration/test_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/integration/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_local_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_scp_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_parsl_load_default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/integration/test_stress/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_ad_hoc_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_log_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_memory_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_oauth_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_regression_220.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_udp_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/manual_tests/test_worker_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/scaling_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/htex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/local_threads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3751 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/vineex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/vineex_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/wqex_condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/scaling_tests/wqex_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.309331 parsl-2024.4.8/parsl/tests/site_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/site_config_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/site_tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/sites/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_dynamic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_local_adhoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/sites/test_mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/sites/test_worker_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_aalst_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_bash_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_apptimeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_keyword_overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_kwarg_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_bash_apps/test_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_callables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_channels/test_large_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_periodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_233.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_239.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_checkpointing/test_task_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_curvezmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.313331 parsl-2024.4.8/parsl/tests/test_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_from_slides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_tutorial_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_docs/test_workflow4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_error_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_python_walltime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_rand_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_serialization_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_error_handling/test_wrap_with_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_htex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_connected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_cpu_affinity_explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_drain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_htex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_manager_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_missing_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_multiple_disconnected_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_worker_failure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_htex/test_zmq_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.317331 parsl-2024.4.8/parsl/tests/test_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_app_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_db_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_fuzz_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_incomplete_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_memoization_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_monitoring/test_viz_colouring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.321331 parsl-2024.4.8/parsl/tests/test_mpi_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_bad_mpi_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_mpi_apps/test_resource_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.321331 parsl-2024.4.8/parsl/tests/test_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_cobalt_deprecation_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_local_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_pbspro_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_slurm_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_slurm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_providers/test_submiterror_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_python_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_arg_input_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_dep_standard_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_depfail_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_garbage_collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_import_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_lifted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_mapred.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_joinapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_python_apps/test_type5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_radical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_radical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_radical/test_mpi_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1480.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_1653.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_226.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_2652.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_69a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_854.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_97_parallelism_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_regression/test_98.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_scaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_block_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_regression_1621.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_scaling/test_shutdown_scalein.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_2555_caching_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_htex_code_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_pack_resource_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.325331 parsl-2024.4.8/parsl/tests/test_shutdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_shutdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_shutdown/test_kill_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/staging_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_1316.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_docs_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_docs_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_elaborate_noop_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_file_staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_output_chain_filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp_in_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_staging/test_staging_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_thread_parallelism.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_threads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_threads/test_lazy_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/test_utils/test_representation_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.329331 parsl-2024.4.8/parsl/usage_tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/usage_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/usage_tracking/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-08 22:42:39.000000 parsl-2024.4.8/parsl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 22:42:41.000000 parsl-2024.4.8/parsl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:42:43.277331 parsl-2024.4.8/parsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 22:42:43.000000 parsl-2024.4.8/parsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 22:42:39.000000 parsl-2024.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 22:42:43.329331 parsl-2024.4.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-04-08 22:42:39.000000 parsl-2024.4.8/setup.py
```

### Comparing `parsl-2024.4.1/LICENSE` & `parsl-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/PKG-INFO` & `parsl-2024.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.4.1
+Version: 2024.4.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.04.01.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.4.1/README.rst` & `parsl-2024.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/__init__.py` & `parsl-2024.4.8/parsl/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/addresses.py` & `parsl-2024.4.8/parsl/addresses.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/app/app.py` & `parsl-2024.4.8/parsl/app/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/app/bash.py` & `parsl-2024.4.8/parsl/app/bash.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/app/errors.py` & `parsl-2024.4.8/parsl/app/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/app/futures.py` & `parsl-2024.4.8/parsl/app/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/app/python.py` & `parsl-2024.4.8/parsl/app/python.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/benchmark/perf.py` & `parsl-2024.4.8/parsl/benchmark/perf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/base.py` & `parsl-2024.4.8/parsl/channels/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/errors.py` & `parsl-2024.4.8/parsl/channels/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/local/local.py` & `parsl-2024.4.8/parsl/channels/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/oauth_ssh/oauth_ssh.py` & `parsl-2024.4.8/parsl/channels/oauth_ssh/oauth_ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/ssh/ssh.py` & `parsl-2024.4.8/parsl/channels/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/channels/ssh_il/ssh_il.py` & `parsl-2024.4.8/parsl/channels/ssh_il/ssh_il.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/concurrent/__init__.py` & `parsl-2024.4.8/parsl/concurrent/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/config.py` & `parsl-2024.4.8/parsl/config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/ASPIRE1.py` & `parsl-2024.4.8/parsl/configs/ASPIRE1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/Azure.py` & `parsl-2024.4.8/parsl/configs/Azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/ad_hoc.py` & `parsl-2024.4.8/parsl/configs/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/bridges.py` & `parsl-2024.4.8/parsl/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/cc_in2p3.py` & `parsl-2024.4.8/parsl/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/ec2.py` & `parsl-2024.4.8/parsl/configs/ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/expanse.py` & `parsl-2024.4.8/parsl/configs/expanse.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/frontera.py` & `parsl-2024.4.8/parsl/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/illinoiscluster.py` & `parsl-2024.4.8/parsl/configs/illinoiscluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/kubernetes.py` & `parsl-2024.4.8/parsl/configs/kubernetes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/midway.py` & `parsl-2024.4.8/parsl/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/osg.py` & `parsl-2024.4.8/parsl/configs/osg.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/polaris.py` & `parsl-2024.4.8/parsl/configs/polaris.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/stampede2.py` & `parsl-2024.4.8/parsl/configs/stampede2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/summit.py` & `parsl-2024.4.8/parsl/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/toss3_llnl.py` & `parsl-2024.4.8/parsl/configs/toss3_llnl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/vineex_local.py` & `parsl-2024.4.8/parsl/configs/vineex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/configs/wqex_local.py` & `parsl-2024.4.8/parsl/configs/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/curvezmq.py` & `parsl-2024.4.8/parsl/curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/data_manager.py` & `parsl-2024.4.8/parsl/data_provider/data_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/files.py` & `parsl-2024.4.8/parsl/data_provider/files.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/ftp.py` & `parsl-2024.4.8/parsl/data_provider/ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/globus.py` & `parsl-2024.4.8/parsl/data_provider/globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/http.py` & `parsl-2024.4.8/parsl/data_provider/http.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/rsync.py` & `parsl-2024.4.8/parsl/data_provider/rsync.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/data_provider/staging.py` & `parsl-2024.4.8/parsl/data_provider/staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/dflow.py` & `parsl-2024.4.8/parsl/dataflow/dflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -710,22 +710,26 @@
             logger.exception("Task {} requested invalid executor {}: config is\n{}".format(task_id, executor_label, self._config))
             raise ValueError("Task {} requested invalid executor {}".format(task_id, executor_label))
 
         try_id = task_record['fail_count']
 
         if self.monitoring is not None and self.monitoring.resource_monitoring_enabled:
             wrapper_logging_level = logging.DEBUG if self.monitoring.monitoring_debug else logging.INFO
-            (function, args, kwargs) = monitor_wrapper(function, args, kwargs, try_id, task_id,
-                                                       self.monitoring.monitoring_hub_url,
-                                                       self.run_id,
-                                                       wrapper_logging_level,
-                                                       self.monitoring.resource_monitoring_interval,
-                                                       executor.radio_mode,
-                                                       executor.monitor_resources(),
-                                                       self.run_dir)
+            (function, args, kwargs) = monitor_wrapper(f=function,
+                                                       args=args,
+                                                       kwargs=kwargs,
+                                                       x_try_id=try_id,
+                                                       x_task_id=task_id,
+                                                       monitoring_hub_url=self.monitoring.monitoring_hub_url,
+                                                       run_id=self.run_id,
+                                                       logging_level=wrapper_logging_level,
+                                                       sleep_dur=self.monitoring.resource_monitoring_interval,
+                                                       radio_mode=executor.radio_mode,
+                                                       monitor_resources=executor.monitor_resources(),
+                                                       run_dir=self.run_dir)
 
         with self.submitter_lock:
             exec_fu = executor.submit(function, task_record['resource_specification'], *args, **kwargs)
         self.update_task_state(task_record, States.launched)
 
         self._send_task_log_info(task_record)
 
@@ -1210,29 +1214,15 @@
         self.usage_tracker.send_end_message()
         self.usage_tracker.close()
 
         logger.info("Closing job status poller")
         self.job_status_poller.close()
         logger.info("Terminated job status poller")
 
-        logger.info("Scaling in and shutting down executors")
-
-        for ef in self.job_status_poller._executor_facades:
-            if not ef.executor.bad_state_is_set:
-                logger.info(f"Scaling in executor {ef.executor.label}")
-
-                # this code needs to be at least as many blocks as need
-                # cancelling, but it is safe to be more, as the scaling
-                # code will cope with being asked to cancel more blocks
-                # than exist.
-                block_count = len(ef.status)
-                ef.scale_in(block_count)
-
-            else:  # and bad_state_is_set
-                logger.warning(f"Not scaling in executor {ef.executor.label} because it is in bad state")
+        logger.info("Shutting down executors")
 
         for executor in self.executors.values():
             logger.info(f"Shutting down executor {executor.label}")
             executor.shutdown()
             logger.info(f"Shut down executor {executor.label}")
 
         logger.info("Terminated executors")
```

### Comparing `parsl-2024.4.1/parsl/dataflow/errors.py` & `parsl-2024.4.8/parsl/dataflow/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/futures.py` & `parsl-2024.4.8/parsl/dataflow/futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/memoization.py` & `parsl-2024.4.8/parsl/dataflow/memoization.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/rundirs.py` & `parsl-2024.4.8/parsl/dataflow/rundirs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/states.py` & `parsl-2024.4.8/parsl/dataflow/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/dataflow/taskrecord.py` & `parsl-2024.4.8/parsl/dataflow/taskrecord.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/errors.py` & `parsl-2024.4.8/parsl/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/base.py` & `parsl-2024.4.8/parsl/executors/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/errors.py` & `parsl-2024.4.8/parsl/executors/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/flux/execute_parsl_task.py` & `parsl-2024.4.8/parsl/executors/flux/execute_parsl_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/flux/executor.py` & `parsl-2024.4.8/parsl/executors/flux/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/flux/flux_instance_manager.py` & `parsl-2024.4.8/parsl/executors/flux/flux_instance_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/executor.py` & `parsl-2024.4.8/parsl/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/interchange.py` & `parsl-2024.4.8/parsl/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/mpi_prefix_composer.py` & `parsl-2024.4.8/parsl/executors/high_throughput/mpi_prefix_composer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/mpi_resource_management.py` & `parsl-2024.4.8/parsl/executors/high_throughput/mpi_resource_management.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/probe.py` & `parsl-2024.4.8/parsl/executors/high_throughput/probe.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/process_worker_pool.py` & `parsl-2024.4.8/parsl/executors/high_throughput/process_worker_pool.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/high_throughput/zmq_pipes.py` & `parsl-2024.4.8/parsl/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/radical/executor.py` & `parsl-2024.4.8/parsl/executors/radical/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/radical/rpex_master.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_master.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/radical/rpex_resources.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_resources.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/radical/rpex_worker.py` & `parsl-2024.4.8/parsl/executors/radical/rpex_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/status_handling.py` & `parsl-2024.4.8/parsl/executors/status_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,14 @@
                  should be done
         """
         if self._provider is None:
             return 0
         else:
             return self._provider.status_polling_interval
 
-    def _fail_job_async(self, block_id: str, message: str):
-        """Marks a job that has failed to start but would not otherwise be included in status()
-        as failed and report it in status()
-        """
-        self._simulated_status[block_id] = JobStatus(JobState.FAILED, message)
-
     @abstractproperty
     def outstanding(self) -> int:
         """This should return the number of tasks that the executor has been given to run (waiting to run, and running now)"""
 
         raise NotImplementedError("Classes inheriting from BlockProviderExecutor must implement "
                                   "outstanding()")
 
@@ -194,16 +188,15 @@
             logger.info(f"Allocated block ID {block_id}")
             try:
                 job_id = self._launch_block(block_id)
                 self.blocks_to_job_id[block_id] = job_id
                 self.job_ids_to_block[job_id] = block_id
                 block_ids.append(block_id)
             except Exception as ex:
-                self._fail_job_async(block_id,
-                                     "Failed to start block {}: {}".format(block_id, ex))
+                self._simulated_status[block_id] = JobStatus(JobState.FAILED, "Failed to start block {}: {}".format(block_id, ex))
         return block_ids
 
     @abstractmethod
     def scale_in(self, blocks: int) -> List[str]:
         """Scale in method.
 
         Cause the executor to reduce the number of blocks by count.
```

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/errors.py` & `parsl-2024.4.8/parsl/executors/taskvine/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/exec_parsl_function.py` & `parsl-2024.4.8/parsl/executors/taskvine/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/executor.py` & `parsl-2024.4.8/parsl/executors/taskvine/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/factory.py` & `parsl-2024.4.8/parsl/executors/taskvine/factory.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/factory_config.py` & `parsl-2024.4.8/parsl/executors/taskvine/factory_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/manager.py` & `parsl-2024.4.8/parsl/executors/taskvine/manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/manager_config.py` & `parsl-2024.4.8/parsl/executors/taskvine/manager_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/taskvine/utils.py` & `parsl-2024.4.8/parsl/executors/taskvine/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/threads.py` & `parsl-2024.4.8/parsl/executors/threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/workqueue/errors.py` & `parsl-2024.4.8/parsl/executors/workqueue/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/workqueue/exec_parsl_function.py` & `parsl-2024.4.8/parsl/executors/workqueue/exec_parsl_function.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/workqueue/executor.py` & `parsl-2024.4.8/parsl/executors/workqueue/executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess.py` & `parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/executors/workqueue/parsl_coprocess_stub.py` & `parsl-2024.4.8/parsl/executors/workqueue/parsl_coprocess_stub.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/jobs/error_handlers.py` & `parsl-2024.4.8/parsl/jobs/error_handlers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/jobs/job_status_poller.py` & `parsl-2024.4.8/parsl/jobs/job_status_poller.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 
 logger = logging.getLogger(__name__)
 
 
 class PolledExecutorFacade:
     def __init__(self, executor: BlockProviderExecutor, dfk: Optional["parsl.dataflow.dflow.DataFlowKernel"] = None):
         self._executor = executor
-        self._dfk = dfk
         self._interval = executor.status_polling_interval
         self._last_poll_time = 0.0
         self._status = {}  # type: Dict[str, JobStatus]
-        self.first = True
 
         # Create a ZMQ channel to send poll status to monitoring
         self.monitoring_enabled = False
-        if self._dfk and self._dfk.monitoring is not None:
+        if dfk and dfk.monitoring is not None:
             self.monitoring_enabled = True
-            hub_address = self._dfk.hub_address
-            hub_port = self._dfk.hub_zmq_port
+            hub_address = dfk.hub_address
+            hub_port = dfk.hub_zmq_port
             context = zmq.Context()
             self.hub_channel = context.socket(zmq.DEALER)
             self.hub_channel.set_hwm(0)
             self.hub_channel.connect("tcp://{}:{}".format(hub_address, hub_port))
             logger.info("Monitoring enabled on job status poller")
 
     def _should_poll(self, now: float) -> bool:
@@ -132,7 +130,23 @@
 
     def add_executors(self, executors: Sequence[BlockProviderExecutor]) -> None:
         for executor in executors:
             if executor.status_polling_interval > 0:
                 logger.debug("Adding executor {}".format(executor.label))
                 self._executor_facades.append(PolledExecutorFacade(executor, self.dfk))
         self._strategy.add_executors(executors)
+
+    def close(self):
+        super().close()
+        for ef in self._executor_facades:
+            if not ef.executor.bad_state_is_set:
+                logger.info(f"Scaling in executor {ef.executor.label}")
+
+                # this code needs to be at least as many blocks as need
+                # cancelling, but it is safe to be more, as the scaling
+                # code will cope with being asked to cancel more blocks
+                # than exist.
+                block_count = len(ef.status)
+                ef.scale_in(block_count)
+
+            else:  # and bad_state_is_set
+                logger.warning(f"Not scaling in executor {ef.executor.label} because it is in bad state")
```

### Comparing `parsl-2024.4.1/parsl/jobs/states.py` & `parsl-2024.4.8/parsl/jobs/states.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/jobs/strategy.py` & `parsl-2024.4.8/parsl/jobs/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     """
 
     idle_since: Optional[float]
     """The timestamp at which an executor became idle.
     If the executor is not idle, then None.
     """
 
+    first: bool
+    """True if this executor has not yet had a strategy poll.
+    """
+
 
 class Strategy:
     """Scaling strategy.
 
     As a workflow dag is processed by Parsl, new tasks are added and completed
     asynchronously. Parsl interfaces executors with execution providers to construct
     scalable executors to handle the variable work-load generated by the
@@ -140,25 +144,25 @@
 
         self.strategize = self.strategies[strategy]
 
         logger.debug("Scaling strategy: {0}".format(strategy))
 
     def add_executors(self, executors: Sequence[ParslExecutor]) -> None:
         for executor in executors:
-            self.executors[executor.label] = {'idle_since': None}
+            self.executors[executor.label] = {'idle_since': None, 'first': True}
 
     def _strategy_init_only(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
         """Scale up to init_blocks at the start, then nothing more.
         """
         for ef in executor_facades:
-            if ef.first:
-                executor = ef.executor
+            executor = ef.executor
+            if self.executors[executor.label]['first']:
                 logger.debug(f"strategy_init_only: scaling out {executor.provider.init_blocks} initial blocks for {executor.label}")
                 ef.scale_out(executor.provider.init_blocks)
-                ef.first = False
+                self.executors[executor.label]['first'] = False
             else:
                 logger.debug("strategy_init_only: doing nothing")
 
     def _strategy_simple(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
         self._general_strategy(executor_facades, strategy_type='simple')
 
     def _strategy_htex_auto_scale(self, executor_facades: List[jsp.PolledExecutorFacade]) -> None:
@@ -186,19 +190,19 @@
             executor = ef.executor
             label = executor.label
             if not isinstance(executor, BlockProviderExecutor):
                 logger.debug(f"Not strategizing for executor {label} because scaling not enabled")
                 continue
             logger.debug(f"Strategizing for executor {label}")
 
-            if ef.first:
+            if self.executors[label]['first']:
                 executor = ef.executor
                 logger.debug(f"Scaling out {executor.provider.init_blocks} initial blocks for {label}")
                 ef.scale_out(executor.provider.init_blocks)
-                ef.first = False
+                self.executors[label]['first'] = False
 
             # Tasks that are either pending completion
             active_tasks = executor.outstanding
 
             status = ef.status
 
             # FIXME we need to handle case where provider does not define these
```

### Comparing `parsl-2024.4.1/parsl/launchers/__init__.py` & `parsl-2024.4.8/parsl/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/launchers/base.py` & `parsl-2024.4.8/parsl/launchers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/launchers/launchers.py` & `parsl-2024.4.8/parsl/launchers/launchers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/log_utils.py` & `parsl-2024.4.8/parsl/log_utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/db_manager.py` & `parsl-2024.4.8/parsl/monitoring/db_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/monitoring.py` & `parsl-2024.4.8/parsl/monitoring/monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/queries/pandas.py` & `parsl-2024.4.8/parsl/monitoring/queries/pandas.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/radios.py` & `parsl-2024.4.8/parsl/monitoring/radios.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/remote.py` & `parsl-2024.4.8/parsl/monitoring/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from parsl.monitoring.message_type import MessageType
 from parsl.monitoring.radios import MonitoringRadio, UDPRadio, HTEXRadio, FilesystemRadio
 from typing import Any, Callable, Dict, List, Sequence, Tuple
 
 logger = logging.getLogger(__name__)
 
 
-def monitor_wrapper(f: Any,           # per app
+def monitor_wrapper(*,
+                    f: Any,           # per app
                     args: Sequence,   # per invocation
                     kwargs: Dict,     # per invocation
                     x_try_id: int,    # per invocation
                     x_task_id: int,   # per invocation
                     monitoring_hub_url: str,   # per workflow
                     run_id: str,      # per workflow
                     logging_level: int,  # per workflow
```

### Comparing `parsl-2024.4.1/parsl/monitoring/router.py` & `parsl-2024.4.8/parsl/monitoring/router.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/types.py` & `parsl-2024.4.8/parsl/monitoring/types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/app.py` & `parsl-2024.4.8/parsl/monitoring/visualization/app.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/models.py` & `parsl-2024.4.8/parsl/monitoring/visualization/models.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/task_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/task_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py` & `parsl-2024.4.8/parsl/monitoring/visualization/plots/default/workflow_resource_plots.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/static/parsl-logo-white.png` & `parsl-2024.4.8/parsl/monitoring/visualization/static/parsl-logo-white.png`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/app.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/app.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/dag.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/dag.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/layout.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/layout.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/resource_usage.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/resource_usage.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/task.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/task.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/workflow.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/workflow.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/templates/workflows_summary.html` & `parsl-2024.4.8/parsl/monitoring/visualization/templates/workflows_summary.html`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/monitoring/visualization/views.py` & `parsl-2024.4.8/parsl/monitoring/visualization/views.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/multiprocessing.py` & `parsl-2024.4.8/parsl/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/process_loggers.py` & `parsl-2024.4.8/parsl/process_loggers.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/__init__.py` & `parsl-2024.4.8/parsl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/ad_hoc/ad_hoc.py` & `parsl-2024.4.8/parsl/providers/ad_hoc/ad_hoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/aws/aws.py` & `parsl-2024.4.8/parsl/providers/aws/aws.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/azure/azure.py` & `parsl-2024.4.8/parsl/providers/azure/azure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/base.py` & `parsl-2024.4.8/parsl/providers/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/cluster_provider.py` & `parsl-2024.4.8/parsl/providers/cluster_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/cobalt/cobalt.py` & `parsl-2024.4.8/parsl/providers/cobalt/cobalt.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/condor/condor.py` & `parsl-2024.4.8/parsl/providers/condor/condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/condor/template.py` & `parsl-2024.4.8/parsl/providers/condor/template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/errors.py` & `parsl-2024.4.8/parsl/providers/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/googlecloud/googlecloud.py` & `parsl-2024.4.8/parsl/providers/googlecloud/googlecloud.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/grid_engine/grid_engine.py` & `parsl-2024.4.8/parsl/providers/grid_engine/grid_engine.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/kubernetes/kube.py` & `parsl-2024.4.8/parsl/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/local/local.py` & `parsl-2024.4.8/parsl/providers/local/local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/lsf/lsf.py` & `parsl-2024.4.8/parsl/providers/lsf/lsf.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/pbspro/pbspro.py` & `parsl-2024.4.8/parsl/providers/pbspro/pbspro.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/slurm/slurm.py` & `parsl-2024.4.8/parsl/providers/slurm/slurm.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/providers/torque/torque.py` & `parsl-2024.4.8/parsl/providers/torque/torque.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/serialize/base.py` & `parsl-2024.4.8/parsl/serialize/base.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/serialize/concretes.py` & `parsl-2024.4.8/parsl/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/serialize/errors.py` & `parsl-2024.4.8/parsl/serialize/errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/serialize/facade.py` & `parsl-2024.4.8/parsl/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/serialize/proxystore.py` & `parsl-2024.4.8/parsl/serialize/proxystore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/ad_hoc_cluster_htex.py` & `parsl-2024.4.8/parsl/tests/configs/ad_hoc_cluster_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/azure_single_node.py` & `parsl-2024.4.8/parsl/tests/configs/azure_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/bluewaters.py` & `parsl-2024.4.8/parsl/tests/configs/bluewaters.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/bridges.py` & `parsl-2024.4.8/parsl/tests/configs/bridges.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/cc_in2p3.py` & `parsl-2024.4.8/parsl/tests/configs/cc_in2p3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/comet.py` & `parsl-2024.4.8/parsl/tests/configs/comet.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/cooley_htex.py` & `parsl-2024.4.8/parsl/tests/configs/cooley_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/ec2_single_node.py` & `parsl-2024.4.8/parsl/tests/configs/ec2_single_node.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/ec2_spot.py` & `parsl-2024.4.8/parsl/tests/configs/ec2_spot.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/frontera.py` & `parsl-2024.4.8/parsl/tests/configs/frontera.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/htex_ad_hoc_cluster.py` & `parsl-2024.4.8/parsl/tests/configs/htex_ad_hoc_cluster.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/htex_local.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/htex_local_alternate.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_alternate.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/htex_local_intask_staging.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_intask_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/htex_local_rsync_staging.py` & `parsl-2024.4.8/parsl/tests/configs/htex_local_rsync_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/local_radical_mpi.py` & `parsl-2024.4.8/parsl/tests/configs/local_radical_mpi.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/local_threads_globus.py` & `parsl-2024.4.8/parsl/tests/configs/local_threads_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/midway.py` & `parsl-2024.4.8/parsl/tests/configs/midway.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/nscc_singapore.py` & `parsl-2024.4.8/parsl/tests/configs/nscc_singapore.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/osg_htex.py` & `parsl-2024.4.8/parsl/tests/configs/osg_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/petrelkube.py` & `parsl-2024.4.8/parsl/tests/configs/petrelkube.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/summit.py` & `parsl-2024.4.8/parsl/tests/configs/summit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/swan_htex.py` & `parsl-2024.4.8/parsl/tests/configs/swan_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/taskvine_ex.py` & `parsl-2024.4.8/parsl/tests/configs/taskvine_ex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/theta.py` & `parsl-2024.4.8/parsl/tests/configs/theta.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/user_opts.py` & `parsl-2024.4.8/parsl/tests/configs/user_opts.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/configs/workqueue_ex.py` & `parsl-2024.4.8/parsl/tests/configs/workqueue_ex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/conftest.py` & `parsl-2024.4.8/parsl/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/latency.py` & `parsl-2024.4.8/parsl/tests/integration/latency.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_local_channel.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_local_channel.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_scp_1.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_scp_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_1.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_errors.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_file_transport.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_file_transport.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_channels/test_ssh_interactive.py` & `parsl-2024.4.8/parsl/tests/integration/test_channels/test_ssh_interactive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_simple.py` & `parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/integration/test_stress/test_python_threads.py` & `parsl-2024.4.8/parsl/tests/integration/test_stress/test_python_threads.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/htex_local.py` & `parsl-2024.4.8/parsl/tests/manual_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_ad_hoc_htex.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_ad_hoc_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_basic.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_fan_in_out_htex_remote.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_log_filter.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_log_filter.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_memory_limits.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_memory_limits.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_regression_220.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_regression_220.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_udp_simple.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_udp_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/manual_tests/test_worker_count.py` & `parsl-2024.4.8/parsl/tests/manual_tests/test_worker_count.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/scaling_tests/htex_local.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/htex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/scaling_tests/test_scale.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/test_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/scaling_tests/wqex_condor.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/wqex_condor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/scaling_tests/wqex_local.py` & `parsl-2024.4.8/parsl/tests/scaling_tests/wqex_local.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/site_tests/site_config_selector.py` & `parsl-2024.4.8/parsl/tests/site_tests/site_config_selector.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/site_tests/test_provider.py` & `parsl-2024.4.8/parsl/tests/site_tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/site_tests/test_site.py` & `parsl-2024.4.8/parsl/tests/site_tests/test_site.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_affinity.py` & `parsl-2024.4.8/parsl/tests/sites/test_affinity.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_concurrent.py` & `parsl-2024.4.8/parsl/tests/sites/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_dynamic_executor.py` & `parsl-2024.4.8/parsl/tests/sites/test_dynamic_executor.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_ec2.py` & `parsl-2024.4.8/parsl/tests/sites/test_ec2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_local_adhoc.py` & `parsl-2024.4.8/parsl/tests/sites/test_local_adhoc.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/sites/test_worker_info.py` & `parsl-2024.4.8/parsl/tests/sites/test_worker_info.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_aalst_patterns.py` & `parsl-2024.4.8/parsl/tests/test_aalst_patterns.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_apptimeout.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_apptimeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_error_codes.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_kwarg_storage.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_kwarg_storage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_memoize_ignore_args_regr.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_multiline.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_multiline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_pipeline.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_bash_apps/test_stdout.py` & `parsl-2024.4.8/parsl/tests/test_bash_apps/test_stdout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_callables.py` & `parsl-2024.4.8/parsl/tests/test_callables.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_channels/test_large_output.py` & `parsl-2024.4.8/parsl/tests/test_channels/test_large_output.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_periodic.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_periodic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_1.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_2.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_python_checkpoint_3.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_python_checkpoint_3.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_232.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_232.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_233.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_233.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_regression_239.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_regression_239.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_checkpointing/test_task_exit.py` & `parsl-2024.4.8/parsl/tests/test_checkpointing/test_task_exit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_curvezmq.py` & `parsl-2024.4.8/parsl/tests/test_curvezmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_from_slides.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_from_slides.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_kwargs.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_kwargs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_tutorial_1.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_tutorial_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_workflow1.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_workflow2.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_docs/test_workflow4.py` & `parsl-2024.4.8/parsl/tests/test_docs/test_workflow4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_python_walltime.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_python_walltime.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_rand_fail.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_rand_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_retries.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retries.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_retry_handler_failure.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_retry_handler_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_serialization_fail.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_serialization_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_error_handling/test_wrap_with_logs.py` & `parsl-2024.4.8/parsl/tests/test_error_handling/test_wrap_with_logs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_flux.py` & `parsl-2024.4.8/parsl/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_connected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_connected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_cpu_affinity_explicit.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_cpu_affinity_explicit.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_disconnected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_drain.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_drain.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_htex.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_htex.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_manager_failure.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_manager_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_missing_worker.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_missing_worker.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_multiple_disconnected_blocks.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_multiple_disconnected_blocks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_worker_failure.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_worker_failure.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_htex/test_zmq_binding.py` & `parsl-2024.4.8/parsl/tests/test_htex/test_zmq_binding.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_app_names.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_app_names.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_db_locks.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_db_locks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_fuzz_zmq.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_fuzz_zmq.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_htex_init_blocks_vs_monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_incomplete_futures.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_incomplete_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_memoization_representation.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_memoization_representation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_monitoring/test_viz_colouring.py` & `parsl-2024.4.8/parsl/tests/test_monitoring/test_viz_colouring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_bad_mpi_config.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_bad_mpi_config.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_disabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_mode_enabled.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_prefix.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_prefix.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_mpi_scheduler.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_mpi_scheduler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_mpi_apps/test_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_mpi_apps/test_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_providers/test_local_provider.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_local_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_providers/test_pbspro_template.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_pbspro_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_providers/test_slurm_template.py` & `parsl-2024.4.8/parsl/tests/test_providers/test_slurm_template.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_arg_input_types.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_arg_input_types.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_context_manager.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_dep_standard_futures.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_dep_standard_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_depfail_propagation.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_depfail_propagation.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_fail.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_iterative.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_iterative.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_fibonacci_recursive.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_fibonacci_recursive.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_futures.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_futures.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_garbage_collect.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_garbage_collect.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_import_fail.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_import_fail.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_join.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_join.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_lifted.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_lifted.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_mapred.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_mapred.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_1.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_2.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_2.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_4.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_4.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_bad_id_for_memo.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_memoize_ignore_args.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_memoize_ignore_args.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_outputs.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_outputs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_pipeline.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_simple.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_simple.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_timeout.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_timeout.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_python_apps/test_type5.py` & `parsl-2024.4.8/parsl/tests/test_python_apps/test_type5.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_radical/test_mpi_funcs.py` & `parsl-2024.4.8/parsl/tests/test_radical/test_mpi_funcs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_1480.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1480.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1606_wait_for_current_tasks.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_1653.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_1653.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_221.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_221.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_226.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_226.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_2652.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_2652.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_69a.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_69a.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_854.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_854.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_regression/test_97_parallelism_0.py` & `parsl-2024.4.8/parsl/tests/test_regression/test_97_parallelism_0.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_scaling/test_block_error_handler.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_block_error_handler.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_scaling/test_regression_1621.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_regression_1621.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_scale_down_htex_auto_scale.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_scaling/test_shutdown_scalein.py` & `parsl-2024.4.8/parsl/tests/test_scaling/test_shutdown_scalein.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_2555_caching_deserializer.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_2555_caching_deserializer.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_basic.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_basic.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_htex_code_cache.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_htex_code_cache.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_pack_resource_spec.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_pack_resource_spec.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_configured.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_configured.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_serialization/test_proxystore_impl.py` & `parsl-2024.4.8/parsl/tests/test_serialization/test_proxystore_impl.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_shutdown/test_kill_monitoring.py` & `parsl-2024.4.8/parsl/tests/test_shutdown/test_kill_monitoring.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/staging_provider.py` & `parsl-2024.4.8/parsl/tests/test_staging/staging_provider.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_1316.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_1316.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_docs_1.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_docs_1.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_elaborate_noop_file.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_elaborate_noop_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_file.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_file_apps.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file_apps.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_file_staging.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_file_staging.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_output_chain_filenames.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_output_chain_filenames.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_staging_ftp_in_task.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_ftp_in_task.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_staging_globus.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_globus.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_staging/test_staging_https.py` & `parsl-2024.4.8/parsl/tests/test_staging/test_staging_https.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_summary.py` & `parsl-2024.4.8/parsl/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_thread_parallelism.py` & `parsl-2024.4.8/parsl/tests/test_thread_parallelism.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_threads/test_configs.py` & `parsl-2024.4.8/parsl/tests/test_threads/test_configs.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_threads/test_lazy_errors.py` & `parsl-2024.4.8/parsl/tests/test_threads/test_lazy_errors.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/tests/test_utils/test_representation_mixin.py` & `parsl-2024.4.8/parsl/tests/test_utils/test_representation_mixin.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/usage_tracking/usage.py` & `parsl-2024.4.8/parsl/usage_tracking/usage.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl/utils.py` & `parsl-2024.4.8/parsl/utils.py`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl.egg-info/PKG-INFO` & `parsl-2024.4.8/parsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: parsl
-Version: 2024.4.1
+Version: 2024.4.8
 Summary: Simple data dependent workflows in Python
 Home-page: https://github.com/Parsl/parsl
-Download-URL: https://github.com/Parsl/parsl/archive/2024.04.01.tar.gz
+Download-URL: https://github.com/Parsl/parsl/archive/2024.04.08.tar.gz
 Author: The Parsl Team
 Author-email: parsl@googlegroups.com
 License: Apache 2.0
 Keywords: Workflows,Scientific computing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `parsl-2024.4.1/parsl.egg-info/SOURCES.txt` & `parsl-2024.4.8/parsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/parsl.egg-info/requires.txt` & `parsl-2024.4.8/parsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `parsl-2024.4.1/setup.py` & `parsl-2024.4.8/setup.py`

 * *Files identical despite different names*

