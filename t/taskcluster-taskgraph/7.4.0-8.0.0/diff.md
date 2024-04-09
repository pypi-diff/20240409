# Comparing `tmp/taskcluster-taskgraph-7.4.0.tar.gz` & `tmp/taskcluster-taskgraph-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-7.4.0.tar", last modified: Tue Mar 26 16:34:08 2024, max compression
+gzip compressed data, was "taskcluster-taskgraph-8.0.0.tar", last modified: Tue Apr  9 15:51:35 2024, max compression
```

## Comparing `taskcluster-taskgraph-7.4.0.tar` & `taskcluster-taskgraph-8.0.0.tar`

### file list

```diff
@@ -1,152 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:08.002256 taskcluster-taskgraph-7.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-26 16:34:08.002256 taskcluster-taskgraph-7.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.986256 taskcluster-taskgraph-7.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 16:34:08.002256 taskcluster-taskgraph-7.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.982256 taskcluster-taskgraph-7.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.986256 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 16:34:07.000000 taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.986256 taskcluster-taskgraph-7.4.0/src/taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.990256 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    12880 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/files_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.990256 taskcluster-taskgraph-7.4.0/src/taskgraph/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/loader/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    28293 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/morph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.990256 taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.990256 taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/
--rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.990256 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/notify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.994256 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/
--rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/task_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:07.994256 taskcluster-taskgraph-7.4.0/src/taskgraph/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 16:34:08.002256 taskcluster-taskgraph-7.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_actions_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_files_changed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_morph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_optimize_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    15315 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_scripts_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_target_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_taskgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transform_chunking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transform_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transform_task_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_from_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_run_run_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_run_toolchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_transforms_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_cached_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_memoize.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_parameterization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_python_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_readonlydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    13497 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_treeherder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15598 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_workertypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-26 16:34:02.000000 taskcluster-taskgraph-7.4.0/test/test_util_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.686315 taskcluster-taskgraph-8.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.682315 taskcluster-taskgraph-8.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.686315 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 15:51:35.000000 taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12943 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29064 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/morph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.690315 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29990 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 runner    (1001) docker     (127)    30813 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45753 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.694315 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/notify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.694315 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/
+-rw-r--r--   0 runner    (1001) docker     (127)    17731 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52586 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.698315 taskcluster-taskgraph-8.0.0/src/taskgraph/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/set_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13057 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18019 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:51:35.706315 taskcluster-taskgraph-8.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_actions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_morph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15584 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_optimize_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15586 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_scripts_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_target_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_taskgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_chunking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transform_task_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_run_toolchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_transforms_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_cached_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_memoize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_parameterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_python_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_readonlydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1677 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2239 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_treeherder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_workertypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 15:51:28.000000 taskcluster-taskgraph-8.0.0/test/test_util_yaml.py
```

### Comparing `taskcluster-taskgraph-7.4.0/LICENSE` & `taskcluster-taskgraph-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/PKG-INFO` & `taskcluster-taskgraph-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 7.4.0
+Version: 8.0.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-7.4.0/README.rst` & `taskcluster-taskgraph-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/pyproject.toml` & `taskcluster-taskgraph-8.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/requirements/base.txt` & `taskcluster-taskgraph-8.0.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/requirements/dev.txt` & `taskcluster-taskgraph-8.0.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/requirements/test.txt` & `taskcluster-taskgraph-8.0.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/setup.py` & `taskcluster-taskgraph-8.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 7.4.0
+Version: 8.0.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-8.0.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 src/taskcluster_taskgraph.egg-info/requires.txt
 src/taskcluster_taskgraph.egg-info/top_level.txt
 src/taskgraph/__init__.py
 src/taskgraph/config.py
 src/taskgraph/create.py
 src/taskgraph/decision.py
 src/taskgraph/docker.py
-src/taskgraph/files_changed.py
 src/taskgraph/filter_tasks.py
 src/taskgraph/generator.py
 src/taskgraph/graph.py
 src/taskgraph/main.py
 src/taskgraph/morph.py
 src/taskgraph/parameters.py
 src/taskgraph/target_tasks.py
@@ -74,29 +73,29 @@
 src/taskgraph/util/keyed_by.py
 src/taskgraph/util/memoize.py
 src/taskgraph/util/parameterization.py
 src/taskgraph/util/path.py
 src/taskgraph/util/python_path.py
 src/taskgraph/util/readonlydict.py
 src/taskgraph/util/schema.py
+src/taskgraph/util/set_name.py
 src/taskgraph/util/shell.py
 src/taskgraph/util/taskcluster.py
 src/taskgraph/util/taskgraph.py
 src/taskgraph/util/templates.py
 src/taskgraph/util/time.py
 src/taskgraph/util/treeherder.py
 src/taskgraph/util/vcs.py
 src/taskgraph/util/verify.py
 src/taskgraph/util/workertypes.py
 src/taskgraph/util/yaml.py
 test/test_actions_rebuild_cached_tasks.py
 test/test_actions_registry.py
 test/test_create.py
 test/test_decision.py
-test/test_files_changed.py
 test/test_generator.py
 test/test_graph.py
 test/test_main.py
 test/test_morph.py
 test/test_optimize.py
 test/test_optimize_strategies.py
 test/test_parameters.py
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "7.4.0"
+__version__ = "8.0.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/config.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/create.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/decision.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         candidate_base_rev=options.get("base_rev"),
         head_rev=options.get("head_rev"),
         env_prefix=_get_env_prefix(graph_config),
     )
 
     # Define default filter list, as most configurations shouldn't need
     # custom filters.
+    parameters["files_changed"] = repo.get_changed_files("AM")
     parameters["filters"] = [
         "target_tasks_method",
     ]
     parameters["optimize_strategies"] = None
     parameters["optimize_target_tasks"] = True
     parameters["existing_tasks"] = {}
     parameters["do_not_optimize"] = []
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/main.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 def get_taskgraph_generator(root, parameters):
     """Helper function to make testing a little easier."""
     from taskgraph.generator import TaskGraphGenerator
 
     return TaskGraphGenerator(root_dir=root, parameters=parameters)
 
 
-def format_taskgraph(options, parameters, logfile=None):
+def format_taskgraph(options, parameters, overrides, logfile=None):
     import taskgraph
     from taskgraph.parameters import parameters_loader
 
     if logfile:
         handler = logging.FileHandler(logfile, mode="w")
         if logging.root.handlers:
             oldhandler = logging.root.handlers[-1]
@@ -135,15 +135,15 @@
 
     if options["fast"]:
         taskgraph.fast = True
 
     if isinstance(parameters, str):
         parameters = parameters_loader(
             parameters,
-            overrides={"target-kinds": options.get("target_kinds")},
+            overrides=overrides,
             strict=False,
         )
 
     tgg = get_taskgraph_generator(options.get("root"), parameters)
 
     tg = getattr(tgg, options["graph_attr"])
     tg = get_filtered_taskgraph(tg, options["tasks_regex"], options["exclude_keys"])
@@ -169,15 +169,15 @@
         print(
             f"Dumping result with parameters from {params_name}:",
             file=sys.stderr,
         )
     print(out + "\n", file=fh)
 
 
-def generate_taskgraph(options, parameters, logdir):
+def generate_taskgraph(options, parameters, overrides, logdir):
     from taskgraph.parameters import Parameters
 
     def logfile(spec):
         """Determine logfile given a parameters specification."""
         if logdir is None:
             return None
         return os.path.join(
@@ -185,22 +185,24 @@
             "{}_{}.log".format(options["graph_attr"], Parameters.format_spec(spec)),
         )
 
     # Don't bother using futures if there's only one parameter. This can make
     # tracebacks a little more readable and avoids additional process overhead.
     if len(parameters) == 1:
         spec = parameters[0]
-        out = format_taskgraph(options, spec, logfile(spec))
+        out = format_taskgraph(options, spec, overrides, logfile(spec))
         dump_output(out, options["output_file"])
         return 0
 
     futures = {}
     with ProcessPoolExecutor(max_workers=options["max_workers"]) as executor:
         for spec in parameters:
-            f = executor.submit(format_taskgraph, options, spec, logfile(spec))
+            f = executor.submit(
+                format_taskgraph, options, spec, overrides, logfile(spec)
+            )
             futures[f] = spec
 
     returncode = 0
     for future in as_completed(futures):
         output_file = options["output_file"]
         spec = futures[future]
         e = future.exception()
@@ -290,14 +292,23 @@
     "latest parameters file for the specified project from CI, or of the form "
     "`task-id=<decision task id>` to download parameters from the specified "
     "decision task. Can be specified multiple times, in which case multiple "
     "generations will happen from the same invocation (one per parameters "
     "specified).",
 )
 @argument(
+    "--force-local-files-changed",
+    default=False,
+    action="store_true",
+    help="Compute the 'files-changed' parameter from local version control, "
+    "even when explicitly using a parameter set that already has it defined. "
+    "Note that this is already the default behaviour when no parameters are "
+    "specified.",
+)
+@argument(
     "--no-optimize",
     dest="optimize",
     action="store_false",
     default="true",
     help="do not remove tasks from the graph that are found in the "
     "index (a.k.a. optimize the graph)",
 )
@@ -363,17 +374,19 @@
         logging.root.setLevel(logging.DEBUG)
 
     repo = None
     cur_rev = None
     diffdir = None
     output_file = options["output_file"]
 
-    if options["diff"]:
+    if options["diff"] or options["force_local_files_changed"]:
         repo = get_repository(os.getcwd())
 
+    if options["diff"]:
+        assert repo is not None
         if not repo.working_directory_clean():
             print(
                 "abort: can't diff taskgraph with dirty working directory",
                 file=sys.stderr,
             )
             return 1
 
@@ -389,23 +402,30 @@
             shutil.rmtree, diffdir
         )  # make sure the directory gets cleaned up
         options["output_file"] = os.path.join(
             diffdir, f"{options['graph_attr']}_{cur_rev_file}"
         )
         print(f"Generating {options['graph_attr']} @ {cur_rev}", file=sys.stderr)
 
+    overrides = {
+        "target-kinds": options.get("target_kinds"),
+    }
     parameters: List[Any[str, Parameters]] = options.pop("parameters")
     if not parameters:
-        overrides = {
-            "target-kinds": options.get("target_kinds"),
-        }
         parameters = [
             parameters_loader(None, strict=False, overrides=overrides)
         ]  # will use default values
 
+        # This is the default behaviour anyway, so no need to re-compute.
+        options["force_local_files_changed"] = False
+
+    elif options["force_local_files_changed"]:
+        assert repo is not None
+        overrides["files-changed"] = sorted(repo.get_changed_files("AM"))
+
     for param in parameters[:]:
         if isinstance(param, str) and os.path.isdir(param):
             parameters.remove(param)
             parameters.extend(
                 [
                     p.as_posix()
                     for p in Path(param).iterdir()
@@ -423,15 +443,15 @@
             os.makedirs(logdir)
     else:
         # Only setup logging if we have a single parameter spec. Otherwise
         # logging will go to files. This is also used as a hook for Gecko
         # to setup its `mach` based logging.
         setup_logging()
 
-    ret = generate_taskgraph(options, parameters, logdir)
+    ret = generate_taskgraph(options, parameters, overrides, logdir)
 
     if options["diff"]:
         assert diffdir is not None
         assert repo is not None
 
         # Reload taskgraph modules to pick up changes and clear global state.
         for mod in sys.modules.copy():
@@ -447,15 +467,15 @@
         try:
             repo.update(base_rev)
             base_rev = repo.head_rev[:12]
             options["output_file"] = os.path.join(
                 diffdir, f"{options['graph_attr']}_{base_rev_file}"
             )
             print(f"Generating {options['graph_attr']} @ {base_rev}", file=sys.stderr)
-            ret |= generate_taskgraph(options, parameters, logdir)
+            ret |= generate_taskgraph(options, parameters, overrides, logdir)
         finally:
             repo.update(cur_rev)
 
         # Generate diff(s)
         diffcmd = [
             "diff",
             "-U20",
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/optimize/strategies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from datetime import datetime
 
-from taskgraph import files_changed
 from taskgraph.optimize.base import OptimizationStrategy, register_strategy
+from taskgraph.util.path import match as match_path
 from taskgraph.util.taskcluster import find_task_id, status_task
 
 logger = logging.getLogger(__name__)
 
 
 @register_strategy("index-search")
 class IndexSearch(OptimizationStrategy):
@@ -44,19 +44,27 @@
                 pass
 
         return False
 
 
 @register_strategy("skip-unless-changed")
 class SkipUnlessChanged(OptimizationStrategy):
+
+    def check(self, files_changed, patterns):
+        for pattern in patterns:
+            for path in files_changed:
+                if match_path(path, pattern):
+                    return True
+        return False
+
     def should_remove_task(self, task, params, file_patterns):
         # pushlog_id == -1 - this is the case when run from a cron.yml job or on a git repository
         if params.get("repository_type") == "hg" and params.get("pushlog_id") == -1:
             return False
 
-        changed = files_changed.check(params, file_patterns)
+        changed = self.check(params["files_changed"], file_patterns)
         if not changed:
             logger.debug(
                 f'no files found matching a pattern in `skip-unless-changed` for "{task.label}"'
             )
             return True
         return False
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         Required("base_ref"): str,
         Required("base_rev"): str,
         Required("build_date"): int,
         Required("build_number"): int,
         Required("do_not_optimize"): [str],
         Required("enable_always_target"): Any(bool, [str]),
         Required("existing_tasks"): {str: str},
+        Required("files_changed"): [str],
         Required("filters"): [str],
         Required("head_ref"): str,
         Required("head_repository"): str,
         Required("head_rev"): str,
         Required("head_tag"): str,
         Required("level"): str,
         Required("moz_build_date"): str,
@@ -82,14 +83,15 @@
     repo_path = repo_root or os.getcwd()
     try:
         repo = get_repository(repo_path)
     except RuntimeError:
         # Use fake values if no repo is detected.
         repo = Mock(branch="", head_rev="", tool="git")
         repo.get_url.return_value = ""
+        repo.get_changed_files.return_value = []
 
     try:
         repo_url = repo.get_url()
         parsed_url = mozilla_repo_urls.parse(repo_url)
         project = parsed_url.repo_name
     except (
         CalledProcessError,
@@ -104,14 +106,15 @@
         "base_ref": "",
         "base_rev": "",
         "build_date": int(time.time()),
         "build_number": 1,
         "do_not_optimize": [],
         "enable_always_target": True,
         "existing_tasks": {},
+        "files_changed": repo.get_changed_files("AM"),
         "filters": ["target_tasks_method"],
         "head_ref": repo.branch or repo.head_rev,
         "head_repository": repo_url,
         "head_rev": repo.head_rev,
         "head_tag": "",
         "level": "3",
         "moz_build_date": datetime.now().strftime("%Y%m%d%H%M%S"),
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-8.0.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/task.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/chunking.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/from_deps.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from voluptuous import Any, Extra, Optional, Required
 
 from taskgraph.transforms.base import TransformSequence
 from taskgraph.transforms.run import fetches_schema
 from taskgraph.util.attributes import attrmatch
 from taskgraph.util.dependencies import GROUP_BY_MAP, get_dependencies
 from taskgraph.util.schema import Schema, validate_schema
+from taskgraph.util.set_name import SET_NAME_MAP
 
 FROM_DEPS_SCHEMA = Schema(
     {
         Required("from-deps"): {
             Optional(
                 "kinds",
                 description=dedent(
@@ -37,20 +38,22 @@
                 """.lstrip()
                 ),
             ): list,
             Optional(
                 "set-name",
                 description=dedent(
                     """
-                When True, `from_deps` will derive a name for the generated
-                tasks from the name of the primary dependency. Defaults to
-                True.
+                UPDATE ME AND DOCS
                 """.lstrip()
                 ),
-            ): bool,
+            ): Any(
+                None,
+                *SET_NAME_MAP,
+                {Any(*SET_NAME_MAP): object},
+            ),
             Optional(
                 "with-attributes",
                 description=dedent(
                     """
                 Limit dependencies to tasks whose attributes match
                 using :func:`~taskgraph.util.attributes.attrmatch`.
                 """.lstrip()
@@ -166,15 +169,15 @@
                 )
             groups = func(config, deps, arg)
         else:
             func = GROUP_BY_MAP[group_by]
             groups = func(config, deps)
 
         # Split the task, one per group.
-        set_name = from_deps.get("set-name", True)
+        set_name = from_deps.get("set-name", "strip-kind")
         copy_attributes = from_deps.get("copy-attributes", False)
         unique_kinds = from_deps.get("unique-kinds", True)
         fetches = from_deps.get("fetches", [])
         for group in groups:
             # Verify there is only one task per kind in each group.
             group_kinds = {t.kind for t in group}
             if unique_kinds and len(group_kinds) < len(group):
@@ -199,18 +202,16 @@
             new_task.setdefault("attributes", {})[
                 "primary-kind-dependency"
             ] = primary_kind
 
             primary_dep = [dep for dep in group if dep.kind == primary_kind][0]
 
             if set_name:
-                if primary_dep.label.startswith(primary_kind):
-                    new_task["name"] = primary_dep.label[len(primary_kind) + 1 :]
-                else:
-                    new_task["name"] = primary_dep.label
+                func = SET_NAME_MAP[set_name]
+                new_task["name"] = func(config, deps, primary_dep, primary_kind)
 
             if copy_attributes:
                 attrs = new_task.setdefault("attributes", {})
                 new_task["attributes"] = primary_dep.attributes.copy()
                 new_task["attributes"].update(attrs)
 
             if fetches:
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/__init__.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/common.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/index_search.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/run_task.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/run/toolchain.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/run/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/transforms/task_context.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/transforms/task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/cached_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import hashlib
 import time
 
 TARGET_CACHE_INDEX = "{cache_prefix}.cache.level-{level}.{type}.{name}.hash.{digest}"
-TARGET_PR_CACHE_INDEX = (
-    "{cache_prefix}.cache.head.{head_ref}.{type}.{name}.hash.{digest}"
-)
+TARGET_PR_CACHE_INDEX = "{cache_prefix}.cache.pr.{type}.{name}.hash.{digest}"
 EXTRA_CACHE_INDEXES = [
     "{cache_prefix}.cache.level-{level}.{type}.{name}.latest",
     "{cache_prefix}.cache.level-{level}.{type}.{name}.pushdate.{build_date_long}",
 ]
 
 
 def add_optimization(
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/parameterization.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,18 +79,19 @@
                 try:
                     task_id = dependencies[dependency]
                 except KeyError:
                     raise KeyError(
                         f"task '{label}' has no dependency named '{dependency}'"
                     )
 
-            assert artifact_name.startswith(
-                "public/"
-            ), f"artifact-reference only supports public artifacts, not `{artifact_name}`"
-            return get_artifact_url(task_id, artifact_name)
+            use_proxy = False
+            if not artifact_name.startswith("public/"):
+                use_proxy = True
+
+            return get_artifact_url(task_id, artifact_name, use_proxy=use_proxy)
 
         return ARTIFACT_REFERENCE_PATTERN.sub(repl, val)
 
     return _recurse(
         task_def,
         {
             "task-reference": task_reference,
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskcluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,30 +136,17 @@
         return yaml.load_stream(response.text)
     response.raw.read = functools.partial(response.raw.read, decode_content=True)
     return response.raw
 
 
 def get_artifact_url(task_id, path, use_proxy=False):
     artifact_tmpl = liburls.api(
-        get_root_url(False), "queue", "v1", "task/{}/artifacts/{}"
+        get_root_url(use_proxy), "queue", "v1", "task/{}/artifacts/{}"
     )
-    data = artifact_tmpl.format(task_id, path)
-    if use_proxy:
-        # Until Bug 1405889 is deployed, we can't download directly
-        # from the taskcluster-proxy.  Work around by using the /bewit
-        # endpoint instead.
-        # The bewit URL is the body of a 303 redirect, which we don't
-        # want to follow (which fetches a potentially large resource).
-        response = _do_request(
-            os.environ["TASKCLUSTER_PROXY_URL"] + "/bewit",
-            data=data,
-            allow_redirects=False,
-        )
-        return response.text
-    return data
+    return artifact_tmpl.format(task_id, path)
 
 
 def get_artifact(task_id, path, use_proxy=False):
     """
     Returns the artifact with the given path for the given task id.
 
     If the path ends with ".json" or ".yml", the content is deserialized as,
```

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-8.0.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-8.0.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_actions_registry.py` & `taskcluster-taskgraph-8.0.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_create.py` & `taskcluster-taskgraph-8.0.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_decision.py` & `taskcluster-taskgraph-8.0.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_generator.py` & `taskcluster-taskgraph-8.0.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_graph.py` & `taskcluster-taskgraph-8.0.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_main.py` & `taskcluster-taskgraph-8.0.0/test/test_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Any copyright is dedicated to the public domain.
 # http://creativecommons.org/publicdomain/zero/1.0/
 
 import os
+import sys
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 
 import taskgraph
 from taskgraph.graph import Graph
@@ -44,15 +45,15 @@
         ("full", ["_fake-t-0", "_fake-t-1", "_fake-t-2"]),
         ("target", ["_fake-t-0", "_fake-t-1"]),
         ("target-graph", ["_fake-t-0", "_fake-t-1"]),
         ("optimized", ["_fake-t-0", "_fake-t-1"]),
         ("morphed", ["_fake-t-0", "_fake-t-1"]),
     ),
 )
-def test_show_taskgraph(run_taskgraph, capsys, attr, expected):
+def test_show_taskgraph_attr(run_taskgraph, capsys, attr, expected):
     res = run_taskgraph([attr])
     assert res == 0
 
     out, err = capsys.readouterr()
     assert out.strip() == "\n".join(expected)
     assert "Dumping result" in err
 
@@ -68,14 +69,42 @@
     # Craft params to cause an exception
     res = run_taskgraph(
         ["full", "-p", "taskcluster/test/params"], params={"_kinds": None}
     )
     assert res == 1
 
 
+def test_show_taskgraph_force_local_files_changed(mocker, run_taskgraph):
+    repo = mocker.MagicMock()
+    repo.get_changed_files.return_value = ["foo.txt"]
+
+    m = mocker.MagicMock()
+    m.get_repository.return_value = repo
+    mocker.patch.dict(sys.modules, {"taskgraph.util.vcs": m})
+
+    res = run_taskgraph(["full"])
+    assert res == 0
+    assert not repo.get_changed_files.called
+
+    res = run_taskgraph(["full", "--force-local-files-changed"])
+    assert res == 0
+    assert not repo.get_changed_files.called
+
+    res = run_taskgraph(
+        [
+            "full",
+            "--force-local-files-changed",
+            "-p",
+            "taskcluster/test/params/mc-onpush.yml",
+        ]
+    )
+    assert res == 0
+    assert repo.get_changed_files.call_count == 1
+
+
 def test_tasks_regex(run_taskgraph, capsys):
     run_taskgraph(["full", "--tasks=_.*-t-1"])
     out, _ = capsys.readouterr()
     assert out.strip() == "_fake-t-1"
 
 
 def test_output_file(run_taskgraph, tmpdir):
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_morph.py` & `taskcluster-taskgraph-8.0.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_optimize.py` & `taskcluster-taskgraph-8.0.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_parameters.py` & `taskcluster-taskgraph-8.0.0/test/test_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         "base_ref": "base_ref",
         "base_rev": "base_rev",
         "build_date": 0,
         "build_number": 1,
         "do_not_optimize": [],
         "enable_always_target": True,
         "existing_tasks": {},
+        "files_changed": [],
         "filters": ["target_tasks_method"],
         "head_ref": "ref",
         "head_repository": "repository",
         "head_rev": "rev",
         "head_tag": "",
         "level": "3",
         "moz_build_date": "20191008095500",
@@ -294,14 +295,15 @@
                 "base_repository": "https://some.url",
                 "base_rev": "",
                 "build_date": 1663804800,
                 "build_number": 1,
                 "do_not_optimize": [],
                 "enable_always_target": True,
                 "existing_tasks": {},
+                "files_changed": ["foo.txt"],
                 "filters": ["target_tasks_method"],
                 "head_ref": "some-branch",
                 "head_repository": "https://some.url",
                 "head_rev": "headrev",
                 "head_tag": "",
                 "level": "3",
                 "moz_build_date": "20220922000000",
@@ -328,14 +330,15 @@
                 "base_repository": "https://some.url",
                 "base_rev": "",
                 "build_date": 1663804800,
                 "build_number": 1,
                 "do_not_optimize": [],
                 "enable_always_target": True,
                 "existing_tasks": {},
+                "files_changed": ["foo.txt"],
                 "filters": ["target_tasks_method"],
                 "head_ref": "some-branch",
                 "head_repository": "https://some.url",
                 "head_rev": "headrev",
                 "head_tag": "",
                 "level": "3",
                 "moz_build_date": "20220922000000",
@@ -362,14 +365,15 @@
                 "base_repository": "",
                 "base_rev": "",
                 "build_date": 1663804800,
                 "build_number": 1,
                 "do_not_optimize": [],
                 "enable_always_target": True,
                 "existing_tasks": {},
+                "files_changed": ["foo.txt"],
                 "filters": ["target_tasks_method"],
                 "head_ref": "some-branch",
                 "head_repository": "",
                 "head_rev": "headrev",
                 "head_tag": "",
                 "level": "3",
                 "moz_build_date": "20220922000000",
@@ -396,14 +400,15 @@
                 "base_repository": "",
                 "base_rev": "",
                 "build_date": 1663804800,
                 "build_number": 1,
                 "do_not_optimize": [],
                 "enable_always_target": True,
                 "existing_tasks": {},
+                "files_changed": [],
                 "filters": ["target_tasks_method"],
                 "head_ref": "",
                 "head_repository": "",
                 "head_rev": "",
                 "head_tag": "",
                 "level": "3",
                 "moz_build_date": "20220922000000",
@@ -430,14 +435,15 @@
         if is_repo:
             repo_mock = mock.MagicMock(
                 branch="some-branch",
                 head_rev="headrev",
                 tool="git",
             )
             repo_mock.get_url.return_value = "https://some.url"
+            repo_mock.get_changed_files.return_value = ["foo.txt"]
             return repo_mock
 
         raise RuntimeError
 
     monkeypatch.setattr(parameters, "get_repository", mock_get_repository)
 
     def mock_parse(url):
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-8.0.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-8.0.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_target_tasks.py` & `taskcluster-taskgraph-8.0.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_taskgraph.py` & `taskcluster-taskgraph-8.0.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transform_chunking.py` & `taskcluster-taskgraph-8.0.0/test/test_transform_chunking.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-8.0.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transform_task_context.py` & `taskcluster-taskgraph-8.0.0/test/test_transform_task_context.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_base.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_cached_tasks.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_from_deps.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,28 @@
 
 def assert_dont_set_name(tasks):
     handle_exception(tasks)
     assert len(tasks) == 1
     assert tasks[0]["name"] == "a-special-name"
 
 
+def assert_set_name_strip_kind(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 2
+    assert tasks[0]["name"] == "a"
+    assert tasks[1]["name"] == "b"
+
+
+def assert_set_name_retain_kind(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 2
+    assert tasks[0]["name"] == "a"
+    assert tasks[1]["name"] == "bar-b"
+
+
 def assert_group_by_all_with_fetch(tasks):
     handle_exception(tasks)
     assert len(tasks) == 1
     assert tasks[0]["dependencies"] == {
         "foo1": "foo1",
         "foo2": "foo2",
         "foo3": "foo3",
@@ -161,25 +175,51 @@
         ),
         pytest.param(
             # task
             {
                 "name": "a-special-name",
                 "from-deps": {
                     "group-by": "all",
-                    "set-name": False,
+                    "set-name": None,
                 },
             },
             # kind config
             None,
             # deps
             None,
             id="dont_set_name",
         ),
         pytest.param(
             # task
+            {
+                "from-deps": {
+                    "set-name": "strip-kind",
+                },
+            },
+            # kind config
+            None,
+            # deps
+            None,
+            id="set_name_strip_kind",
+        ),
+        pytest.param(
+            # task
+            {
+                "from-deps": {
+                    "set-name": "retain-kind",
+                },
+            },
+            # kind config
+            None,
+            # deps
+            None,
+            id="set_name_retain_kind",
+        ),
+        pytest.param(
+            # task
             {"from-deps": {}},
             # kind config
             None,
             # deps
             None,
             id="group_by_single",
         ),
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_run.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_run.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_run_run_task.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_run_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_run_toolchain.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_run_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_transforms_task.py` & `taskcluster-taskgraph-8.0.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_archive.py` & `taskcluster-taskgraph-8.0.0/test/test_util_archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_attributes.py` & `taskcluster-taskgraph-8.0.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_cached_tasks.py` & `taskcluster-taskgraph-8.0.0/test/test_util_cached_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,20 +80,18 @@
             "cached_task": {"digest": "abc", "name": "cache-name", "type": "cache-type"}
         },
         "optimization": {
             "index-search": [
                 "test-domain.cache.level-3.cache-type.cache-name.hash.abc",
                 "test-domain.cache.level-2.cache-type.cache-name.hash.abc",
                 "test-domain.cache.level-1.cache-type.cache-name.hash.abc",
-                "test-domain.cache.head.default.cache-type.cache-name.hash.abc",
+                "test-domain.cache.pr.cache-type.cache-name.hash.abc",
             ]
         },
-        "routes": [
-            "index.test-domain.cache.head.default.cache-type.cache-name.hash.abc"
-        ],
+        "routes": ["index.test-domain.cache.pr.cache-type.cache-name.hash.abc"],
     }
 
 
 def assert_pull_request_nocache(task):
     handle_exception(task)
     assert task == {
         "attributes": {
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-8.0.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_docker.py` & `taskcluster-taskgraph-8.0.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_memoize.py` & `taskcluster-taskgraph-8.0.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-8.0.0/test/test_util_parameterization.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,25 @@
             + "/api/queue/v1/task/tid1/artifacts/public/filename and "
             + _test_root_url()
             + "/api/queue/v1/task/tid2/artifacts/public/bar"
         },
     )
 
 
+def test_artifact_refs_private(monkeypatch, assert_artifact_refs):
+    "resolve_task_references resolves private artifact references"
+    tc_proxy_url = "https://taskcluster-proxy.net"
+    monkeypatch.setenv("TASKCLUSTER_PROXY_URL", tc_proxy_url)
+
+    assert_artifact_refs(
+        {"artifact-reference": "<edge1/private/foo>"},
+        f"{tc_proxy_url}/api/queue/v1/task/tid1/artifacts/private/foo",
+    )
+
+
 def test_artifact_refs_self():
     "resolve_task_references raises keyerror on artifact references to `self`"
     with pytest.raises(KeyError):
         resolve_task_references(
             "subject",
             {"artifact-reference": "<self/public/artifact>"},
             "tid-self",
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_path.py` & `taskcluster-taskgraph-8.0.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_python_path.py` & `taskcluster-taskgraph-8.0.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-8.0.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_schema.py` & `taskcluster-taskgraph-8.0.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-8.0.0/test/test_util_taskcluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,38 @@
     assert r.text == "method:post"
 
     responses.replace(responses.GET, "https://example.org", status=404)
     with pytest.raises(HTTPError):
         tc._do_request("https://example.org")
 
 
+@pytest.mark.parametrize(
+    "use_proxy,expected",
+    (
+        pytest.param(
+            False,
+            "https://tc.example.com/api/queue/v1/task/abc/artifacts/public/log.txt",
+            id="use_proxy=False",
+        ),
+        pytest.param(
+            True,
+            "https://taskcluster-proxy.net/api/queue/v1/task/abc/artifacts/public/log.txt",
+            id="use_proxy=True",
+        ),
+    ),
+)
+def test_get_artifact_url(monkeypatch, use_proxy, expected):
+    if use_proxy:
+        monkeypatch.setenv("TASKCLUSTER_PROXY_URL", "https://taskcluster-proxy.net")
+
+    task_id = "abc"
+    path = "public/log.txt"
+    assert tc.get_artifact_url(task_id, path, use_proxy) == expected
+
+
 def test_get_artifact(responses, root_url):
     tid = 123
     responses.add(
         responses.GET,
         f"{root_url}/api/queue/v1/task/{tid}/artifacts/artifact.txt",
         body="foobar",
     )
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_templates.py` & `taskcluster-taskgraph-8.0.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_time.py` & `taskcluster-taskgraph-8.0.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-8.0.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_vcs.py` & `taskcluster-taskgraph-8.0.0/test/test_util_vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import subprocess
 from textwrap import dedent
 
 import pytest
 
 from taskgraph.util.vcs import HgRepository, Repository, get_repository
 
-from .fixtures.vcs import create_remote_repo
-
 
 def test_get_repository(repo):
     r = get_repository(repo.path)
     assert isinstance(r, Repository)
 
     new_dir = os.path.join(repo.path, "new_dir")
     oldcwd = os.getcwd()
@@ -155,65 +153,65 @@
     assert repo.remote_name == remote_name
 
     if repo.tool == "git":
         repo.run("branch", "--unset-upstream")
         assert repo.remote_name == remote_name
 
 
-def test_all_remote_names(tmpdir, repo_with_remote):
+def test_all_remote_names(tmpdir, create_remote_repo, repo_with_remote):
     repo, remote_name = repo_with_remote
     assert repo.all_remote_names == [remote_name]
     create_remote_repo(tmpdir, repo, "upstream2", "remote_path2")
     assert repo.all_remote_names == [remote_name, "upstream2"]
 
 
-def test_remote_name_many_remotes(tmpdir, repo_with_remote):
+def test_remote_name_many_remotes(tmpdir, create_remote_repo, repo_with_remote):
     repo, _ = repo_with_remote
     create_remote_repo(tmpdir, repo, "upstream2", "remote_path2")
 
     if repo.tool == "git":
         assert repo.remote_name == "upstream2"  # Branch is set to an upstream one
         repo.run("branch", "--unset-upstream")
 
     assert repo.remote_name == "upstream"
 
 
-def test_remote_name_default_and_origin(tmpdir, repo_with_remote):
+def test_remote_name_default_and_origin(tmpdir, create_remote_repo, repo_with_remote):
     repo, _ = repo_with_remote
     remote_name = "origin" if repo.tool == "git" else "default"
     create_remote_repo(tmpdir, repo, remote_name, "remote_path2")
 
     if repo.tool == "git":
         repo.run("branch", "--unset-upstream")
 
     assert repo.remote_name == remote_name
 
 
-def test_default_branch_guess(repo):
+def test_default_branch_guess(default_git_branch, repo):
     if repo.tool == "git":
-        assert repo.default_branch == "refs/heads/master"
+        assert repo.default_branch == f"refs/heads/{default_git_branch}"
     else:
         assert repo.default_branch == "default"
 
 
-def test_default_branch_remote_query(repo_with_remote):
+def test_default_branch_remote_query(default_git_branch, repo_with_remote):
     repo, _ = repo_with_remote
     if repo.tool == "git":
-        assert repo.default_branch == "upstream/master"
+        assert repo.default_branch == f"upstream/{default_git_branch}"
     else:
         assert repo.default_branch == "default"
 
 
-def test_default_branch_cloned_metadata(tmpdir, repo):
+def test_default_branch_cloned_metadata(tmpdir, default_git_branch, repo):
     if repo.tool == "git":
         clone_repo_path = tmpdir / "cloned_repo"
         command = ("git", "clone", repo.path, clone_repo_path)
         subprocess.check_output(command, cwd=tmpdir)
         cloned_repo = get_repository(clone_repo_path)
-        assert cloned_repo.default_branch == "origin/master"
+        assert cloned_repo.default_branch == f"origin/{default_git_branch}"
 
 
 def assert_files(actual, expected):
     assert set(map(os.path.basename, actual)) == set(expected)
 
 
 def test_get_changed_files_no_changes(repo):
```

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_verify.py` & `taskcluster-taskgraph-8.0.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-8.0.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-7.4.0/test/test_util_yaml.py` & `taskcluster-taskgraph-8.0.0/test/test_util_yaml.py`

 * *Files identical despite different names*

