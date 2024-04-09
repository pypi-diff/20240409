# Comparing `tmp/fractal_server-2.0.0a2.tar.gz` & `tmp/fractal_server-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-2.0.0a2.tar", max compression
+gzip compressed data, was "fractal_server-2.0.0a3.tar", max compression
```

## Comparing `fractal_server-2.0.0a2.tar` & `fractal_server-2.0.0a3.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     1576 2024-04-05 13:18:12.006198 fractal_server-2.0.0a2/LICENSE
--rw-r--r--   0        0        0     2466 2024-04-05 13:18:12.006198 fractal_server-2.0.0a2/README.md
--rw-r--r--   0        0        0       24 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/__init__.py
--rw-r--r--   0        0        0     4958 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     4042 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      183 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0      567 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     3378 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1090 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/state.py
--rw-r--r--   0        0        0      413 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/dataset.py
--rw-r--r--   0        0        0     3304 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/job.py
--rw-r--r--   0        0        0      859 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/project.py
--rw-r--r--   0        0        0     2782 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/task.py
--rw-r--r--   0        0        0     3950 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v1/workflow.py
--rw-r--r--   0        0        0      400 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/dataset.py
--rw-r--r--   0        0        0     1535 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/job.py
--rw-r--r--   0        0        0      845 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/project.py
--rw-r--r--   0        0        0     3257 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/task.py
--rw-r--r--   0        0        0     1256 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/workflow.py
--rw-r--r--   0        0        0     2727 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/models/v2/workflowtask.py
--rw-r--r--   0        0        0        0 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/__init__.py
--rw-r--r--   0        0        0    13981 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/admin/v1.py
--rw-r--r--   0        0        0     8891 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/admin/v2.py
--rw-r--r--   0        0        0      315 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/__init__.py
--rw-r--r--   0        0        0      958 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/__init__.py
--rw-r--r--   0        0        0    11955 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/_aux_functions.py
--rw-r--r--   0        0        0    16911 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/dataset.py
--rw-r--r--   0        0        0     5436 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/job.py
--rw-r--r--   0        0        0    15765 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/project.py
--rw-r--r--   0        0        0     6123 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/task.py
--rw-r--r--   0        0        0     8457 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/task_collection.py
--rw-r--r--   0        0        0    10930 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/workflow.py
--rw-r--r--   0        0        0     5579 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/workflowtask.py
--rw-r--r--   0        0        0     1217 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/__init__.py
--rw-r--r--   0        0        0    14142 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/_aux_functions.py
--rw-r--r--   0        0        0     9702 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/dataset.py
--rw-r--r--   0        0        0     5765 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/images.py
--rw-r--r--   0        0        0     5334 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/job.py
--rw-r--r--   0        0        0     6091 2024-04-05 13:18:12.010198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/project.py
--rw-r--r--   0        0        0     7219 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/submit.py
--rw-r--r--   0        0        0     7130 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/task.py
--rw-r--r--   0        0        0     8466 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/task_collection.py
--rw-r--r--   0        0        0    12580 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/workflow.py
--rw-r--r--   0        0        0     8895 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/workflowtask.py
--rw-r--r--   0        0        0     4885 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/auth.py
--rw-r--r--   0        0        0        0 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/aux/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/aux/_job.py
--rw-r--r--   0        0        0      675 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/routes/aux/_runner.py
--rw-r--r--   0        0        0       16 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0      829 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/async_wrap.py
--rw-r--r--   0        0        0      119 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/components.py
--rw-r--r--   0        0        0     4159 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/exceptions.py
--rw-r--r--   0        0        0       65 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/__init__.py
--rw-r--r--   0        0        0     8841 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_batching.py
--rw-r--r--   0        0        0     1908 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
--rw-r--r--   0        0        0     4421 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    15552 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_slurm_config.py
--rw-r--r--   0        0        0     5123 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    44504 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/executor.py
--rw-r--r--   0        0        0     5852 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/remote.py
--rw-r--r--   0        0        0      206 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/filenames.py
--rw-r--r--   0        0        0     1254 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/set_start_and_last_task_index.py
--rw-r--r--   0        0        0     3219 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/task_files.py
--rw-r--r--   0        0        0    13608 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/__init__.py
--rw-r--r--   0        0        0    21238 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_common.py
--rw-r--r--   0        0        0     6919 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/__init__.py
--rw-r--r--   0        0        0     3147 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/_local_config.py
--rw-r--r--   0        0        0     1493 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/executor.py
--rw-r--r--   0        0        0    10839 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/__init__.py
--rw-r--r--   0        0        0     2732 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     5977 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0     3294 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/common.py
--rw-r--r--   0        0        0     4684 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v1/handle_failed_job.py
--rw-r--r--   0        0        0    12431 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/__init__.py
--rw-r--r--   0        0        0     6163 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/__init__.py
--rw-r--r--   0        0        0     3630 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/_local_config.py
--rw-r--r--   0        0        0     1614 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/executor.py
--rw-r--r--   0        0        0     4395 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/__init__.py
--rw-r--r--   0        0        0     2847 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     6621 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
--rw-r--r--   0        0        0      571 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/deduplicate_list.py
--rw-r--r--   0        0        0     5149 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/handle_failed_job.py
--rw-r--r--   0        0        0     1281 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/merge_outputs.py
--rw-r--r--   0        0        0    11027 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner.py
--rw-r--r--   0        0        0    10047 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner_functions.py
--rw-r--r--   0        0        0     3845 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner_functions_low_level.py
--rw-r--r--   0        0        0     1243 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/task_interface.py
--rw-r--r--   0        0        0      495 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/runner/v2/v1_compat.py
--rw-r--r--   0        0        0      157 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/__init__.py
--rw-r--r--   0        0        0     2549 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/_validators.py
--rw-r--r--   0        0        0     1787 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/json_schemas/manifest.json
--rw-r--r--   0        0        0      692 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/state.py
--rw-r--r--   0        0        0     3113 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/user.py
--rw-r--r--   0        0        0     2078 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/__init__.py
--rw-r--r--   0        0        0     4302 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/applyworkflow.py
--rw-r--r--   0        0        0     3444 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/dataset.py
--rw-r--r--   0        0        0     1274 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/dumps.py
--rw-r--r--   0        0        0     3829 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/manifest.py
--rw-r--r--   0        0        0     1218 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/project.py
--rw-r--r--   0        0        0     3704 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/task.py
--rw-r--r--   0        0        0     3057 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/task_collection.py
--rw-r--r--   0        0        0     4618 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v1/workflow.py
--rw-r--r--   0        0        0     1704 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/dataset.py
--rw-r--r--   0        0        0     2047 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/dumps.py
--rw-r--r--   0        0        0     3250 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/job.py
--rw-r--r--   0        0        0     6243 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/manifest.py
--rw-r--r--   0        0        0      814 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/project.py
--rw-r--r--   0        0        0     3607 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/task.py
--rw-r--r--   0        0        0     2993 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/task_collection.py
--rw-r--r--   0        0        0     1831 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/workflow.py
--rw-r--r--   0        0        0     3424 2024-04-05 13:18:12.014198 fractal_server-2.0.0a2/fractal_server/app/schemas/v2/workflowtask.py
--rw-r--r--   0        0        0    11203 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0    15080 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/config.py
--rw-r--r--   0        0        0      398 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/data_migrations/README.md
--rw-r--r--   0        0        0       88 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/images/__init__.py
--rw-r--r--   0        0        0     1536 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/images/models.py
--rw-r--r--   0        0        0     2204 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/images/tools.py
--rw-r--r--   0        0        0     3924 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/logger.py
--rw-r--r--   0        0        0     3001 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/main.py
--rw-r--r--   0        0        0       59 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/README
--rw-r--r--   0        0        0     2630 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      526 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     1157 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
--rw-r--r--   0        0        0     8770 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0     1632 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
--rw-r--r--   0        0        0     1353 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
--rw-r--r--   0        0        0     2684 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
--rw-r--r--   0        0        0     1115 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
--rw-r--r--   0        0        0     1057 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
--rw-r--r--   0        0        0      883 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
--rw-r--r--   0        0        0     1849 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
--rw-r--r--   0        0        0      867 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
--rw-r--r--   0        0        0      949 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
--rw-r--r--   0        0        0     8240 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/d71e732236cd_v2.py
--rw-r--r--   0        0        0      963 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
--rw-r--r--   0        0        0     1221 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
--rw-r--r--   0        0        0      746 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/syringe.py
--rw-r--r--   0        0        0       23 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0     5379 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/endpoint_operations.py
--rw-r--r--   0        0        0     3278 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/utils.py
--rw-r--r--   0        0        0     3775 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v1/_TaskCollectPip.py
--rw-r--r--   0        0        0    11725 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v1/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v1/get_collection_data.py
--rw-r--r--   0        0        0     3775 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v2/_TaskCollectPip.py
--rw-r--r--   0        0        0    12803 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v2/background_operations.py
--rw-r--r--   0        0        0      502 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/tasks/v2/get_collection_data.py
--rw-r--r--   0        0        0     2115 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/fractal_server/utils.py
--rw-r--r--   0        0        0     2948 2024-04-05 13:18:12.018198 fractal_server-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 fractal_server-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/README.md
+-rw-r--r--   0        0        0       24 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/__init__.py
+-rw-r--r--   0        0        0     4958 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     3378 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1090 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0      413 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/dataset.py
+-rw-r--r--   0        0        0     3304 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/job.py
+-rw-r--r--   0        0        0      859 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/project.py
+-rw-r--r--   0        0        0     2782 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/task.py
+-rw-r--r--   0        0        0     3950 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v1/workflow.py
+-rw-r--r--   0        0        0      400 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/__init__.py
+-rw-r--r--   0        0        0     1483 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/dataset.py
+-rw-r--r--   0        0        0     1535 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/job.py
+-rw-r--r--   0        0        0      845 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/project.py
+-rw-r--r--   0        0        0     3257 2024-04-09 08:34:24.912946 fractal_server-2.0.0a3/fractal_server/app/models/v2/task.py
+-rw-r--r--   0        0        0     1256 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/models/v2/workflow.py
+-rw-r--r--   0        0        0     2727 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/models/v2/workflowtask.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/__init__.py
+-rw-r--r--   0        0        0    13981 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/admin/v1.py
+-rw-r--r--   0        0        0     9706 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/admin/v2.py
+-rw-r--r--   0        0        0      315 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/__init__.py
+-rw-r--r--   0        0        0      958 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/__init__.py
+-rw-r--r--   0        0        0    11955 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0    16911 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/dataset.py
+-rw-r--r--   0        0        0     5436 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/job.py
+-rw-r--r--   0        0        0    15765 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/project.py
+-rw-r--r--   0        0        0     6123 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task.py
+-rw-r--r--   0        0        0     8457 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task_collection.py
+-rw-r--r--   0        0        0    10930 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     1217 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/__init__.py
+-rw-r--r--   0        0        0    14218 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/_aux_functions.py
+-rw-r--r--   0        0        0     9680 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/dataset.py
+-rw-r--r--   0        0        0     5956 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/images.py
+-rw-r--r--   0        0        0     5334 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/job.py
+-rw-r--r--   0        0        0     6024 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/project.py
+-rw-r--r--   0        0        0     7219 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/submit.py
+-rw-r--r--   0        0        0     7130 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task.py
+-rw-r--r--   0        0        0     8466 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task_collection.py
+-rw-r--r--   0        0        0    11845 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflow.py
+-rw-r--r--   0        0        0     8414 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflowtask.py
+-rw-r--r--   0        0        0     4885 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/auth.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/__init__.py
+-rw-r--r--   0        0        0     1248 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/_job.py
+-rw-r--r--   0        0        0      675 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/routes/aux/_runner.py
+-rw-r--r--   0        0        0       16 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0      829 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/async_wrap.py
+-rw-r--r--   0        0        0      119 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/components.py
+-rw-r--r--   0        0        0     4159 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/exceptions.py
+-rw-r--r--   0        0        0       65 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/__init__.py
+-rw-r--r--   0        0        0     8841 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_batching.py
+-rw-r--r--   0        0        0     1908 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py
+-rw-r--r--   0        0        0     4421 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    15552 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_slurm_config.py
+-rw-r--r--   0        0        0     5123 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    44504 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/executor.py
+-rw-r--r--   0        0        0     5852 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/remote.py
+-rw-r--r--   0        0        0      206 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/filenames.py
+-rw-r--r--   0        0        0     1254 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/set_start_and_last_task_index.py
+-rw-r--r--   0        0        0     3219 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/task_files.py
+-rw-r--r--   0        0        0    13608 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/__init__.py
+-rw-r--r--   0        0        0    21238 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_common.py
+-rw-r--r--   0        0        0     6919 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/__init__.py
+-rw-r--r--   0        0        0     3147 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_local_config.py
+-rw-r--r--   0        0        0     1493 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/executor.py
+-rw-r--r--   0        0        0    10839 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/__init__.py
+-rw-r--r--   0        0        0     2732 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     5977 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0     3294 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/common.py
+-rw-r--r--   0        0        0     4684 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v1/handle_failed_job.py
+-rw-r--r--   0        0        0    12431 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/__init__.py
+-rw-r--r--   0        0        0     6163 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/__init__.py
+-rw-r--r--   0        0        0     3630 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_local_config.py
+-rw-r--r--   0        0        0     1614 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/executor.py
+-rw-r--r--   0        0        0     4395 2024-04-09 08:34:24.916946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     6621 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py
+-rw-r--r--   0        0        0      571 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/deduplicate_list.py
+-rw-r--r--   0        0        0     5149 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/handle_failed_job.py
+-rw-r--r--   0        0        0     1281 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/merge_outputs.py
+-rw-r--r--   0        0        0    11119 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner.py
+-rw-r--r--   0        0        0    10087 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions.py
+-rw-r--r--   0        0        0     3845 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions_low_level.py
+-rw-r--r--   0        0        0     1376 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/task_interface.py
+-rw-r--r--   0        0        0      511 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/runner/v2/v1_compat.py
+-rw-r--r--   0        0        0      157 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/__init__.py
+-rw-r--r--   0        0        0     2549 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/_validators.py
+-rw-r--r--   0        0        0     1787 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/json_schemas/manifest.json
+-rw-r--r--   0        0        0      692 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/state.py
+-rw-r--r--   0        0        0     3113 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/user.py
+-rw-r--r--   0        0        0     2078 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/__init__.py
+-rw-r--r--   0        0        0     4302 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/applyworkflow.py
+-rw-r--r--   0        0        0     3444 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dataset.py
+-rw-r--r--   0        0        0     1274 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dumps.py
+-rw-r--r--   0        0        0     3829 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/manifest.py
+-rw-r--r--   0        0        0     1218 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/project.py
+-rw-r--r--   0        0        0     3704 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task.py
+-rw-r--r--   0        0        0     3057 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task_collection.py
+-rw-r--r--   0        0        0     4618 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v1/workflow.py
+-rw-r--r--   0        0        0     1704 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dataset.py
+-rw-r--r--   0        0        0     2047 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dumps.py
+-rw-r--r--   0        0        0     3250 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/job.py
+-rw-r--r--   0        0        0     6243 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/manifest.py
+-rw-r--r--   0        0        0      814 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/project.py
+-rw-r--r--   0        0        0     3607 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task.py
+-rw-r--r--   0        0        0     2993 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task_collection.py
+-rw-r--r--   0        0        0     1831 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflow.py
+-rw-r--r--   0        0        0     3903 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflowtask.py
+-rw-r--r--   0        0        0    11203 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0    15080 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/config.py
+-rw-r--r--   0        0        0      398 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/data_migrations/README.md
+-rw-r--r--   0        0        0       88 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/__init__.py
+-rw-r--r--   0        0        0     1540 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/models.py
+-rw-r--r--   0        0        0     2234 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/images/tools.py
+-rw-r--r--   0        0        0     3924 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/logger.py
+-rw-r--r--   0        0        0     3001 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2630 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      526 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     1157 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py
+-rw-r--r--   0        0        0     8770 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0     1632 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py
+-rw-r--r--   0        0        0     1353 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py
+-rw-r--r--   0        0        0     2684 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py
+-rw-r--r--   0        0        0     1115 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py
+-rw-r--r--   0        0        0     1057 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py
+-rw-r--r--   0        0        0      883 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py
+-rw-r--r--   0        0        0     1849 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py
+-rw-r--r--   0        0        0      867 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py
+-rw-r--r--   0        0        0      949 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py
+-rw-r--r--   0        0        0     8240 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/d71e732236cd_v2.py
+-rw-r--r--   0        0        0      963 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py
+-rw-r--r--   0        0        0     1221 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py
+-rw-r--r--   0        0        0      746 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/syringe.py
+-rw-r--r--   0        0        0       23 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0     5379 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/endpoint_operations.py
+-rw-r--r--   0        0        0     3278 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/utils.py
+-rw-r--r--   0        0        0     3775 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/_TaskCollectPip.py
+-rw-r--r--   0        0        0    11725 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v1/get_collection_data.py
+-rw-r--r--   0        0        0     3775 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/_TaskCollectPip.py
+-rw-r--r--   0        0        0    12803 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/background_operations.py
+-rw-r--r--   0        0        0      502 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/tasks/v2/get_collection_data.py
+-rw-r--r--   0        0        0     2115 2024-04-09 08:34:24.920946 fractal_server-2.0.0a3/fractal_server/utils.py
+-rw-r--r--   0        0        0     2948 2024-04-09 08:34:24.924946 fractal_server-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 fractal_server-2.0.0a3/PKG-INFO
```

### Comparing `fractal_server-2.0.0a2/LICENSE` & `fractal_server-2.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/README.md` & `fractal_server-2.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/__main__.py` & `fractal_server-2.0.0a3/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/alembic.ini` & `fractal_server-2.0.0a3/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/db/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/linkuserproject.py` & `fractal_server-2.0.0a3/fractal_server/app/models/linkuserproject.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/security.py` & `fractal_server-2.0.0a3/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/state.py` & `fractal_server-2.0.0a3/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v1/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v1/job.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v1/project.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v1/task.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v1/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,9 +47,9 @@
             JSON,
             nullable=False,
             server_default='{"attributes": {}, "types": {}}',
         )
     )
 
     @property
-    def image_paths(self) -> list[str]:
-        return [image["path"] for image in self.images]
+    def image_zarr_urls(self) -> list[str]:
+        return [image["zarr_url"] for image in self.images]
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/job.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/project.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/task.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/models/v2/workflowtask.py` & `fractal_server-2.0.0a3/fractal_server/app/models/v2/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/admin/v1.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/admin/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/admin/v2.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/admin/v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from ...models.security import UserOAuth as User
 from ...models.v1 import Task
 from ...models.v2 import JobV2
 from ...models.v2 import ProjectV2
 from ...runner.filenames import WORKFLOW_LOG_FILENAME
 from ...schemas.v2 import JobReadV2
 from ...schemas.v2 import JobUpdateV2
+from ...schemas.v2 import ProjectReadV2
 from ...security import current_active_superuser
 from ..aux._job import _write_shutdown_file
 from ..aux._job import _zip_folder_to_byte_stream
 from ..aux._runner import _check_backend_is_slurm
 
 router_admin_v2 = APIRouter()
 
@@ -48,14 +49,43 @@
         )
     _dt = dt.astimezone(timezone.utc)
     if Inject(get_settings).DB_ENGINE == "sqlite":
         return _dt.replace(tzinfo=None)
     return _dt
 
 
+@router_admin_v2.get("/project/", response_model=list[ProjectReadV2])
+async def view_project(
+    id: Optional[int] = None,
+    user_id: Optional[int] = None,
+    user: User = Depends(current_active_superuser),
+    db: AsyncSession = Depends(get_async_db),
+) -> list[ProjectReadV2]:
+    """
+    Query `ProjectV2` table.
+
+    Args:
+        id: If not `None`, select a given `project.id`.
+        user_id: If not `None`, select a given `project.user_id`.
+    """
+
+    stm = select(ProjectV2)
+
+    if id is not None:
+        stm = stm.where(ProjectV2.id == id)
+    if user_id is not None:
+        stm = stm.where(ProjectV2.user_list.any(User.id == user_id))
+
+    res = await db.execute(stm)
+    project_list = res.scalars().all()
+    await db.close()
+
+    return project_list
+
+
 @router_admin_v2.get("/job/", response_model=list[JobReadV2])
 async def view_job(
     id: Optional[int] = None,
     user_id: Optional[int] = None,
     project_id: Optional[int] = None,
     dataset_id: Optional[int] = None,
     workflow_id: Optional[int] = None,
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/_aux_functions.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/job.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/project.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/task.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/task_collection.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v1/workflowtask.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/_aux_functions.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/_aux_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 from fastapi import HTTPException
 from fastapi import status
+from sqlalchemy.orm.attributes import flag_modified
 from sqlmodel import select
 from sqlmodel.sql.expression import SelectOfScalar
 
 from ....db import AsyncSession
 from ....models.v1 import Task
 from ....models.v2 import DatasetV2
 from ....models.v2 import JobV2
@@ -484,14 +485,14 @@
         task_legacy_id=(task_id if is_legacy_task else None),
         args_non_parallel=final_args_non_parallel,
         args_parallel=final_args_parallel,
         meta_parallel=final_meta_parallel,
         meta_non_parallel=final_meta_non_parallel,
         **input_filters_kwarg,
     )
-    db.add(wf_task)
     db_workflow.task_list.insert(order, wf_task)
     db_workflow.task_list.reorder()  # type: ignore
+    flag_modified(db_workflow, "task_list")
     await db.commit()
     await db.refresh(wf_task)
 
     return wf_task
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,14 @@
     # Cascade operations: set foreign-keys to null for jobs which are in
     # relationship with the current dataset
     stm = select(JobV2).where(JobV2.dataset_id == dataset_id)
     res = await db.execute(stm)
     jobs = res.scalars().all()
     for job in jobs:
         job.dataset_id = None
-    await db.commit()
 
     # Delete dataset
     await db.delete(dataset)
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/images.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     attributes: dict[str, list[Any]]
     types: list[str]
 
     images: list[SingleImage]
 
 
 class ImageQuery(BaseModel):
-    path: Optional[str]
+    zarr_url: Optional[str]
     filters: Filters = Field(default_factory=Filters)
 
 
 @router.post(
     "/project/{project_id}/dataset/{dataset_id}/images/",
     status_code=status.HTTP_201_CREATED,
 )
@@ -52,19 +52,19 @@
 ) -> Response:
 
     output = await _get_dataset_check_owner(
         project_id=project_id, dataset_id=dataset_id, user_id=user.id, db=db
     )
     dataset = output["dataset"]
 
-    if new_image.path in dataset.image_paths:
+    if new_image.zarr_url in dataset.image_zarr_urls:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=(
-                f"Image with path '{new_image.path}' "
+                f"Image with zarr_url '{new_image.zarr_url}' "
                 f"already in DatasetV2 {dataset_id}",
             ),
         )
 
     dataset.images.append(new_image.dict())
     flag_modified(dataset, "images")
 
@@ -117,17 +117,21 @@
 
     types = list(
         set(type for image in images for type in image["types"].keys())
     )
 
     if query is not None:
 
-        if query.path is not None:
+        if query.zarr_url is not None:
             image = next(
-                (image for image in images if image["path"] == query.path),
+                (
+                    image
+                    for image in images
+                    if image["zarr_url"] == query.zarr_url
+                ),
                 None,
             )
             if image is None:
                 images = []
             else:
                 images = [image]
 
@@ -176,31 +180,35 @@
 @router.delete(
     "/project/{project_id}/dataset/{dataset_id}/images/",
     status_code=status.HTTP_204_NO_CONTENT,
 )
 async def delete_dataset_images(
     project_id: int,
     dataset_id: int,
-    path: str,
+    zarr_url: str,
     user: User = Depends(current_active_user),
     db: AsyncSession = Depends(get_async_db),
 ) -> Response:
 
     output = await _get_dataset_check_owner(
         project_id=project_id, dataset_id=dataset_id, user_id=user.id, db=db
     )
     dataset = output["dataset"]
 
     image_to_remove = next(
-        (image for image in dataset.images if image["path"] == path), None
+        (image for image in dataset.images if image["zarr_url"] == zarr_url),
+        None,
     )
     if image_to_remove is None:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
-            detail=f"No image with path '{path}' in DatasetV2 {dataset_id}.",
+            detail=(
+                f"No image with zarr_url '{zarr_url}' in "
+                f"DatasetV2 {dataset_id}."
+            ),
         )
 
     dataset.images.remove(image_to_remove)
     flag_modified(dataset, "images")
 
     await db.commit()
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/job.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/project.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         stm = select(JobV2).where(JobV2.workflow_id == wf.id)
         res = await db.execute(stm)
         jobs = res.scalars().all()
         for job in jobs:
             job.workflow_id = None
         # Delete workflow
         await db.delete(wf)
-    await db.commit()
 
     # Dataset
     stm = select(DatasetV2).where(DatasetV2.project_id == project_id)
     res = await db.execute(stm)
     datasets = res.scalars().all()
     for ds in datasets:
         # Cascade operations: set foreign-keys to null for jobs which are in
@@ -181,22 +180,19 @@
         stm = select(JobV2).where(JobV2.dataset_id == ds.id)
         res = await db.execute(stm)
         jobs = res.scalars().all()
         for job in jobs:
             job.dataset_id = None
         # Delete dataset
         await db.delete(ds)
-    await db.commit()
 
     # Job
     stm = select(JobV2).where(JobV2.project_id == project_id)
     res = await db.execute(stm)
     jobs = res.scalars().all()
     for job in jobs:
         job.project_id = None
 
-    await db.commit()
-
     await db.delete(project)
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/submit.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/submit.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/task.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/task_collection.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from ....db import AsyncSession
 from ....db import get_async_db
 from ....models.v1 import Task as TaskV1
 from ....models.v2 import JobV2
 from ....models.v2 import ProjectV2
 from ....models.v2 import TaskV2
 from ....models.v2 import WorkflowV2
-from ....schemas.v1 import WorkflowTaskCreateV1
 from ....schemas.v2 import WorkflowCreateV2
 from ....schemas.v2 import WorkflowExportV2
 from ....schemas.v2 import WorkflowImportV2
 from ....schemas.v2 import WorkflowReadV2
 from ....schemas.v2 import WorkflowTaskCreateV2
 from ....schemas.v2 import WorkflowUpdateV2
 from ....security import current_active_user
@@ -209,15 +208,14 @@
     # Cascade operations: set foreign-keys to null for jobs which are in
     # relationship with the current workflow
     stm = select(JobV2).where(JobV2.workflow_id == workflow_id)
     res = await db.execute(stm)
     jobs = res.scalars().all()
     for job in jobs:
         job.workflow_id = None
-    await db.commit()
 
     # Delete workflow
     await db.delete(workflow)
     await db.commit()
 
     return Response(status_code=status.HTTP_204_NO_CONTENT)
 
@@ -337,48 +335,33 @@
         **workflow.dict(exclude_none=True, exclude={"task_list"}),
     )
     db.add(db_workflow)
     await db.commit()
     await db.refresh(db_workflow)
 
     # Insert tasks
-    async with db:  # FIXME why?
 
-        for wf_task in workflow.task_list:
-            if wf_task.is_legacy_task is True:
-                # Identify task_id
-                source = wf_task.task_legacy.source
-                task_id = source_to_id_legacy[source]
-                # Prepare new_wf_task
-                new_wf_task = WorkflowTaskCreateV1(
-                    **wf_task.dict(exclude_none=True)
-                )
-                # Insert task
-                await _workflow_insert_task(
-                    **new_wf_task.dict(),
-                    is_legacy_task=True,
-                    workflow_id=db_workflow.id,
-                    task_id=task_id,
-                    db=db,
-                )
-            else:
-                # Identify task_id
-                source = wf_task.task.source
-                task_id = source_to_id[source]
-                # Prepare new_wf_task
-                new_wf_task = WorkflowTaskCreateV2(
-                    **wf_task.dict(exclude_none=True)
-                )
-                # Insert task
-                await _workflow_insert_task(
-                    **new_wf_task.dict(),
-                    workflow_id=db_workflow.id,
-                    task_id=task_id,
-                    db=db,
-                )
+    for wf_task in workflow.task_list:
+        if wf_task.is_legacy_task is True:
+            source = wf_task.task_legacy.source
+            task_id = source_to_id_legacy[source]
+        else:
+            source = wf_task.task.source
+            task_id = source_to_id[source]
+
+        new_wf_task = WorkflowTaskCreateV2(
+            **wf_task.dict(exclude_none=True, exclude={"task", "task_legacy"})
+        )
+        # Insert task
+        await _workflow_insert_task(
+            **new_wf_task.dict(),
+            workflow_id=db_workflow.id,
+            task_id=task_id,
+            db=db,
+        )
 
     await db.close()
     return db_workflow
 
 
 @router.get("/workflow/", response_model=list[WorkflowReadV2])
 async def get_user_workflows(
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/api/v2/workflowtask.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/api/v2/workflowtask.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,27 +87,26 @@
                 detail=(
                     "Cannot set `WorkflowTaskV2.meta_parallel` or "
                     "`WorkflowTask.args_parallel` if the associated Task "
                     "is `non_parallel`."
                 ),
             )
 
-    async with db:
-        workflow_task = await _workflow_insert_task(
-            workflow_id=workflow.id,
-            is_legacy_task=new_task.is_legacy_task,
-            task_id=task_id,
-            order=new_task.order,
-            meta_non_parallel=new_task.meta_non_parallel,
-            meta_parallel=new_task.meta_parallel,
-            args_non_parallel=new_task.args_non_parallel,
-            args_parallel=new_task.args_parallel,
-            input_filters=new_task.input_filters,
-            db=db,
-        )
+    workflow_task = await _workflow_insert_task(
+        workflow_id=workflow.id,
+        is_legacy_task=new_task.is_legacy_task,
+        task_id=task_id,
+        order=new_task.order,
+        meta_non_parallel=new_task.meta_non_parallel,
+        meta_parallel=new_task.meta_parallel,
+        args_non_parallel=new_task.args_non_parallel,
+        args_parallel=new_task.args_parallel,
+        input_filters=new_task.input_filters,
+        db=db,
+    )
 
     await db.close()
 
     return workflow_task
 
 
 @router.get(
@@ -208,25 +207,16 @@
             actual_args = default_args.copy()
             if value is not None:
                 for k, v in value.items():
                     actual_args[k] = v
             if not actual_args:
                 actual_args = None
             setattr(db_wf_task, key, actual_args)
-        elif key == "meta_parallel":
-            current_meta_parallel = deepcopy(db_wf_task.meta_parallel) or {}
-            current_meta_parallel.update(value)
-            setattr(db_wf_task, key, current_meta_parallel)
-        elif key == "meta_non_parallel":
-            current_meta_non_parallel = (
-                deepcopy(db_wf_task.meta_non_parallel) or {}
-            )
-            current_meta_non_parallel.update(value)
-            setattr(db_wf_task, key, current_meta_non_parallel)
-        # FIXME handle `input_filters`
+        elif key in ["meta_parallel", "meta_non_parallel", "input_filters"]:
+            setattr(db_wf_task, key, value)
         else:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
                 detail=f"patch_workflow_task endpoint cannot set {key=}",
             )
 
     await db.commit()
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/auth.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/auth.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/aux/_job.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/aux/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/routes/aux/_runner.py` & `fractal_server-2.0.0a3/fractal_server/app/routes/aux/_runner.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/async_wrap.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/async_wrap.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/exceptions.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_batching.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_check_jobs_status.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_check_jobs_status.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_slurm_config.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/executor.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/executors/slurm/remote.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/executors/slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/set_start_and_last_task_index.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/set_start_and_last_task_index.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/task_files.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/task_files.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_common.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/_local_config.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/_submit_setup.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_local/executor.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/_submit_setup.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/common.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v1/handle_failed_job.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v1/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/_local_config.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/_submit_setup.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_local/executor.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/_submit_setup.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/_slurm/get_slurm_config.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/_slurm/get_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/deduplicate_list.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/deduplicate_list.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/handle_failed_job.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/handle_failed_job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/merge_outputs.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/merge_outputs.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Callable
 from typing import Optional
 
 from ....images import Filters
 from ....images import SingleImage
 from ....images.tools import filter_image_list
-from ....images.tools import find_image_by_path
+from ....images.tools import find_image_by_zarr_url
 from ....images.tools import match_filter
 from ..filenames import FILTERS_FILENAME
 from ..filenames import HISTORY_FILENAME
 from ..filenames import IMAGES_FILENAME
 from .runner_functions import no_op_submit_setup_call
 from .runner_functions import run_v1_task_parallel
 from .runner_functions import run_v2_task_compound
@@ -62,15 +62,15 @@
             images=tmp_images,
             filters=Filters(**pre_filters),
         )
         # Verify that filtered images comply with task input_types
         for image in filtered_images:
             if not match_filter(image, Filters(types=task.input_types)):
                 raise ValueError(
-                    f"Filtered images include {image.dict()}, which does "
+                    f"Filtered images include {image}, which does "
                     f"not comply with {task.input_types=}."
                 )
 
         # TASK EXECUTION (V2)
         if not wftask.is_legacy_task:
             if task.type == "non_parallel":
                 current_task_output = run_v2_task_non_parallel(
@@ -119,95 +119,97 @@
                 logger_name=logger_name,
                 submit_setup_call=submit_setup_call,
             )
 
         # POST TASK EXECUTION
 
         # Update image list
-        current_task_output.check_paths_are_unique()
+        current_task_output.check_zarr_urls_are_unique()
         for image_obj in current_task_output.image_list_updates:
             image = image_obj.dict()
             # Edit existing image
-            if image["path"] in [_image["path"] for _image in tmp_images]:
+            if image["zarr_url"] in [
+                _image["zarr_url"] for _image in tmp_images
+            ]:
                 if (
                     image["origin"] is not None
-                    and image["origin"] != image["path"]
+                    and image["origin"] != image["zarr_url"]
                 ):
                     raise ValueError(
-                        f"Trying to edit an image with {image['path']=} "
+                        f"Trying to edit an image with {image['zarr_url']=} "
                         f"and {image['origin']=}."
                     )
-                image_search = find_image_by_path(
+                img_search = find_image_by_zarr_url(
                     images=tmp_images,
-                    path=image["path"],
+                    zarr_url=image["zarr_url"],
                 )
-                if image_search is None:
+                if img_search is None:
                     raise ValueError(
-                        f"Image with path {image['path']} not found, while "
-                        "updating image list."
+                        f"Image with zarr_url {image['zarr_url']} not found, "
+                        "while updating image list."
                     )
-                original_img = image_search["image"]
-                original_index = image_search["index"]
+                original_img = img_search["image"]
+                original_index = img_search["index"]
                 updated_attributes = copy(original_img["attributes"])
                 updated_types = copy(original_img["types"])
 
                 # Update image attributes/types with task output and manifest
                 updated_attributes.update(image["attributes"])
                 updated_types.update(image["types"])
                 updated_types.update(task.output_types)
 
                 # Update image in the dataset image list
                 tmp_images[original_index]["attributes"] = updated_attributes
                 tmp_images[original_index]["types"] = updated_types
             # Add new image
             else:
-                # Check that image['path'] is relative to zarr_dir
-                if not image["path"].startswith(zarr_dir):
+                # Check that image['zarr_url'] is relative to zarr_dir
+                if not image["zarr_url"].startswith(zarr_dir):
                     raise ValueError(
                         f"{zarr_dir} is not a parent directory of "
-                        f"{image['path']}"
+                        f"{image['zarr_url']}"
                     )
                 # Propagate attributes and types from `origin` (if any)
                 updated_attributes = {}
                 updated_types = {}
                 if image["origin"] is not None:
-                    image_search = find_image_by_path(
+                    img_search = find_image_by_zarr_url(
                         images=tmp_images,
-                        path=image["origin"],
+                        zarr_url=image["origin"],
                     )
-                    if image_search is not None:
-                        original_img = image_search["image"]
+                    if img_search is not None:
+                        original_img = img_search["image"]
                         updated_attributes = copy(original_img["attributes"])
                         updated_types = copy(original_img["types"])
                 # Update image attributes/types with task output and manifest
                 updated_attributes.update(image["attributes"])
                 updated_types.update(image["types"])
                 updated_types.update(task.output_types)
                 new_image = dict(
-                    path=image["path"],
+                    zarr_url=image["zarr_url"],
                     origin=image["origin"],
                     attributes=updated_attributes,
                     types=updated_types,
                 )
                 # Validate new image
                 SingleImage(**new_image)
                 # Add image into the dataset image list
                 tmp_images.append(new_image)
 
         # Remove images from tmp_images
-        for image_path in current_task_output.image_list_removals:
-            image_search = find_image_by_path(
-                images=tmp_images, path=image_path
+        for img_zarr_url in current_task_output.image_list_removals:
+            img_search = find_image_by_zarr_url(
+                images=tmp_images, zarr_url=img_zarr_url
             )
-            if image_search is None:
+            if img_search is None:
                 raise ValueError(
-                    f"Cannot remove missing image with path {image_path=}"
+                    f"Cannot remove missing image with zarr_url {img_zarr_url}"
                 )
             else:
-                tmp_images.pop(image_search["index"])
+                tmp_images.pop(img_search["index"])
 
         # Update filters.attributes:
         # current + (task_output: not really, in current examples..)
         if current_task_output.filters is not None:
             tmp_filters["attributes"].update(
                 current_task_output.filters.attributes
             )
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner_functions.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         workflow_dir=workflow_dir,
         workflow_dir_user=workflow_dir_user,
         submit_setup_call=submit_setup_call,
         which_type="non_parallel",
     )
 
     function_kwargs = dict(
-        paths=[image["path"] for image in images],
+        zarr_urls=[image["zarr_url"] for image in images],
         zarr_dir=zarr_dir,
         **(wftask.args_non_parallel or {}),
     )
     future = executor.submit(
         functools.partial(
             run_single_task,
             wftask=wftask,
@@ -156,15 +156,15 @@
         which_type="parallel",
     )
 
     list_function_kwargs = []
     for ind, image in enumerate(images):
         list_function_kwargs.append(
             dict(
-                path=image["path"],
+                zarr_url=image["zarr_url"],
                 **(wftask.args_parallel or {}),
             ),
         )
         list_function_kwargs[-1][_COMPONENT_KEY_] = _index_to_component(ind)
 
     results_iterator = executor.map(
         functools.partial(
@@ -219,15 +219,15 @@
         workflow_dir_user=workflow_dir_user,
         submit_setup_call=submit_setup_call,
         which_type="parallel",
     )
 
     # 3/A: non-parallel init task
     function_kwargs = dict(
-        paths=[image["path"] for image in images],
+        zarr_urls=[image["zarr_url"] for image in images],
         zarr_dir=zarr_dir,
         **(wftask.args_non_parallel or {}),
     )
     future = executor.submit(
         functools.partial(
             run_single_task,
             wftask=wftask,
@@ -249,15 +249,15 @@
     # 3/B: parallel part of a compound task
     _check_parallelization_list_size(parallelization_list)
 
     list_function_kwargs = []
     for ind, parallelization_item in enumerate(parallelization_list):
         list_function_kwargs.append(
             dict(
-                path=parallelization_item.path,
+                zarr_url=parallelization_item.zarr_url,
                 init_args=parallelization_item.init_args,
                 **(wftask.args_parallel or {}),
             ),
         )
         list_function_kwargs[-1][_COMPONENT_KEY_] = _index_to_component(ind)
 
     results_iterator = executor.map(
@@ -310,15 +310,15 @@
     )
 
     list_function_kwargs = []
     for ind, image in enumerate(images):
         list_function_kwargs.append(
             convert_v2_args_into_v1(
                 dict(
-                    path=image["path"],
+                    zarr_url=image["zarr_url"],
                     **(wftask.args_parallel or {}),
                 )
             ),
         )
         list_function_kwargs[-1][_COMPONENT_KEY_] = _index_to_component(ind)
 
     results_iterator = executor.map(
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/runner_functions_low_level.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/runner_functions_low_level.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/runner/v2/task_interface.py` & `fractal_server-2.0.0a3/fractal_server/app/runner/v2/task_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,32 +11,37 @@
     class Config:
         extra = "forbid"
 
     image_list_updates: list[SingleImage] = Field(default_factory=list)
     image_list_removals: list[str] = Field(default_factory=list)
     filters: Filters = Field(default_factory=Filters)
 
-    def check_paths_are_unique(self) -> None:
-        paths = [img.path for img in self.image_list_updates]
-        paths.extend(self.image_list_removals)
-        if len(paths) != len(set(paths)):
-            duplicates = [path for path in set(paths) if paths.count(path) > 1]
+    def check_zarr_urls_are_unique(self) -> None:
+        zarr_urls = [img.zarr_url for img in self.image_list_updates]
+        zarr_urls.extend(self.image_list_removals)
+        if len(zarr_urls) != len(set(zarr_urls)):
+            duplicates = [
+                zarr_url
+                for zarr_url in set(zarr_urls)
+                if zarr_urls.count(zarr_url) > 1
+            ]
             msg = (
-                "TaskOutput image-list updates/removals has non-unique paths:"
+                "TaskOutput image-list updates/removals has "
+                "non-unique zarr_urls:"
             )
             for duplicate in duplicates:
                 msg = f"{msg}\n{duplicate}"
             raise ValueError(msg)
 
 
 class InitArgsModel(BaseModel):
     class Config:
         extra = "forbid"
 
-    path: str
+    zarr_url: str
     init_args: dict[str, Any] = Field(default_factory=dict)
 
 
 class InitTaskOutput(BaseModel):
     class Config:
         extra = "forbid"
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/_validators.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/json_schemas/manifest.json` & `fractal_server-2.0.0a3/fractal_server/app/schemas/json_schemas/manifest.json`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/state.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/user.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/applyworkflow.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/dumps.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/manifest.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/project.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/task.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/task_collection.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v1/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/dataset.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/dumps.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/dumps.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/job.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/manifest.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/project.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/task.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/task_collection.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/workflow.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/app/schemas/v2/workflowtask.py` & `fractal_server-2.0.0a3/fractal_server/app/schemas/v2/workflowtask.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import Any
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Extra
 from pydantic import Field
+from pydantic import root_validator
 from pydantic import validator
 
 from .._validators import valint
 from ..v1.task import TaskExportV1
 from ..v1.task import TaskImportV1
 from ..v1.task import TaskReadV1
 from .task import TaskExportV2
@@ -34,37 +35,48 @@
     SUBMITTED = "submitted"
     DONE = "done"
     FAILED = "failed"
 
 
 class WorkflowTaskCreateV2(BaseModel, extra=Extra.forbid):
 
-    meta_parallel: Optional[dict[str, Any]]
     meta_non_parallel: Optional[dict[str, Any]]
+    meta_parallel: Optional[dict[str, Any]]
     args_non_parallel: Optional[dict[str, Any]]
     args_parallel: Optional[dict[str, Any]]
     order: Optional[int]
     input_filters: Filters = Field(default_factory=Filters)
 
     is_legacy_task: bool = False
 
     # Validators
 
     _order = validator("order", allow_reuse=True)(valint("order", min_val=0))
-    # FIXME validate: if `is_legacy_task`, `args_non_parallel` must be None
+
+    @root_validator
+    def validate_legacy_task(cls, values):
+        if values["is_legacy_task"] and (
+            values.get("meta_non_parallel") is not None
+            or values.get("args_non_parallel") is not None
+        ):
+            raise ValueError(
+                "If Task is legacy, 'args_non_parallel' and 'meta_non_parallel"
+                "must be None"
+            )
+        return values
 
 
 class WorkflowTaskReadV2(BaseModel):
 
     id: int
 
     workflow_id: int
     order: Optional[int]
-    meta_parallel: Optional[dict[str, Any]]
     meta_non_parallel: Optional[dict[str, Any]]
+    meta_parallel: Optional[dict[str, Any]]
 
     args_non_parallel: Optional[dict[str, Any]]
     args_parallel: Optional[dict[str, Any]]
 
     input_filters: Filters
 
     is_legacy_task: bool
@@ -73,16 +85,16 @@
     task: Optional[TaskReadV2]
     task_legacy_id: Optional[int]
     task_legacy: Optional[TaskReadV1]
 
 
 class WorkflowTaskUpdateV2(BaseModel):
 
-    meta_parallel: Optional[dict[str, Any]]
     meta_non_parallel: Optional[dict[str, Any]]
+    meta_parallel: Optional[dict[str, Any]]
     args_non_parallel: Optional[dict[str, Any]]
     args_parallel: Optional[dict[str, Any]]
     input_filters: Optional[Filters]
 
     # Validators
 
     @validator("meta_parallel", "meta_non_parallel")
@@ -92,28 +104,30 @@
                 "Overriding task parallelization level currently not allowed"
             )
         return m
 
 
 class WorkflowTaskImportV2(BaseModel):
 
-    meta_parallel: Optional[dict[str, Any]] = None
     meta_non_parallel: Optional[dict[str, Any]] = None
-    args: Optional[dict[str, Any]] = None  # FIXME
+    meta_parallel: Optional[dict[str, Any]] = None
+    args_non_parallel: Optional[dict[str, Any]] = None
+    args_parallel: Optional[dict[str, Any]] = None
 
     input_filters: Optional[Filters] = None
 
     is_legacy_task: bool = False
     task: Optional[TaskImportV2] = None
     task_legacy: Optional[TaskImportV1] = None
 
 
 class WorkflowTaskExportV2(BaseModel):
 
-    meta_parallel: Optional[dict[str, Any]] = None
     meta_non_parallel: Optional[dict[str, Any]] = None
-    args: Optional[dict[str, Any]] = None  # FIXME
+    meta_parallel: Optional[dict[str, Any]] = None
+    args_non_parallel: Optional[dict[str, Any]] = None
+    args_parallel: Optional[dict[str, Any]] = None
     input_filters: Filters = Field(default_factory=Filters)
 
     is_legacy_task: bool = False
     task: Optional[TaskExportV2]
     task_legacy: Optional[TaskExportV1]
```

### Comparing `fractal_server-2.0.0a2/fractal_server/app/security/__init__.py` & `fractal_server-2.0.0a3/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/config.py` & `fractal_server-2.0.0a3/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/images/models.py` & `fractal_server-2.0.0a3/fractal_server/images/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 
 class SingleImage(BaseModel):
 
-    path: str
+    zarr_url: str
     origin: Optional[str] = None
 
     attributes: dict[str, Any] = Field(default_factory=dict)
     types: dict[str, bool] = Field(default_factory=dict)
 
     @validator("attributes")
     def validate_attributes(
```

### Comparing `fractal_server-2.0.0a2/fractal_server/images/tools.py` & `fractal_server-2.0.0a3/fractal_server/images/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 from fractal_server.images import Filters
 
 
 ImageSearch = dict[Literal["image", "index"], Union[int, dict[str, Any]]]
 
 
-def find_image_by_path(
+def find_image_by_zarr_url(
     *,
     images: list[dict[str, Any]],
-    path: str,
+    zarr_url: str,
 ) -> Optional[ImageSearch]:
     """
-    Return a copy of the image with a given path, and its positional index.
+    Return a copy of the image with a given zarr_url, and its positional index.
 
     Arguments:
         images: List of images.
-        path: Path that the returned image must have.
+        zarr_url: Path that the returned image must have.
 
     Returns:
-        The first image from `images` which has path equal to `path`.
+        The first image from `images` which has zarr_url equal to `zarr_url`.
     """
-    image_paths = [img["path"] for img in images]
+    image_urls = [img["zarr_url"] for img in images]
     try:
-        ind = image_paths.index(path)
+        ind = image_urls.index(zarr_url)
     except ValueError:
         return None
     return dict(image=copy(images[ind]), index=ind)
 
 
 # FIXME: what is filters
 def match_filter(image: dict[str, Any], filters: Filters) -> bool:
```

### Comparing `fractal_server-2.0.0a2/fractal_server/logger.py` & `fractal_server-2.0.0a3/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/main.py` & `fractal_server-2.0.0a3/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/env.py` & `fractal_server-2.0.0a3/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/script.py.mako` & `fractal_server-2.0.0a3/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/4cedeb448a53_workflowtask_foreign_keys_not_nullables.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/70e77f1c38b0_add_applyworkflow_first_task_index_and_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/71eefd1dd202_add_slurm_accounts.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/84bf0fffde30_add_dumps_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/8f79bd162e35_add_docs_info_and_docs_link_to_task_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/97f444d47249_add_applyworkflow_project_dump.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/99ea79d9e5d2_add_dataset_history.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/9fd26a2b0de4_add_workflow_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/a7f4d6137b53_add_workflow_dump_to_applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/d4fe3708d309_make_applyworkflow_workflow_dump_non_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/d71e732236cd_v2.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/d71e732236cd_v2.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/e75cac726012_make_applyworkflow_start_timestamp_not_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/efa89c30e0a4_add_project_timestamp_created.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-2.0.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/syringe.py` & `fractal_server-2.0.0a3/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/endpoint_operations.py` & `fractal_server-2.0.0a3/fractal_server/tasks/endpoint_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/utils.py` & `fractal_server-2.0.0a3/fractal_server/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/v1/_TaskCollectPip.py` & `fractal_server-2.0.0a3/fractal_server/tasks/v1/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/v1/background_operations.py` & `fractal_server-2.0.0a3/fractal_server/tasks/v1/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/v2/_TaskCollectPip.py` & `fractal_server-2.0.0a3/fractal_server/tasks/v2/_TaskCollectPip.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/tasks/v2/background_operations.py` & `fractal_server-2.0.0a3/fractal_server/tasks/v2/background_operations.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/fractal_server/utils.py` & `fractal_server-2.0.0a3/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-2.0.0a2/pyproject.toml` & `fractal_server-2.0.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "2.0.0a2"
+version = "2.0.0a3"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -80,15 +80,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "2.0.0a2"
+current_version = "2.0.0a3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-2.0.0a2/PKG-INFO` & `fractal_server-2.0.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

