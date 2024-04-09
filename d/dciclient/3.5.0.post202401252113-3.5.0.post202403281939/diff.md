# Comparing `tmp/dciclient-3.5.0.post202401252113.tar.gz` & `tmp/dciclient-3.5.0.post202403281939.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dciclient-3.5.0.post202401252113.tar", last modified: Wed Jan 31 16:47:57 2024, max compression
+gzip compressed data, was "dciclient-3.5.0.post202403281939.tar", last modified: Tue Apr  9 09:54:46 2024, max compression
```

## Comparing `dciclient-3.5.0.post202401252113.tar` & `dciclient-3.5.0.post202403281939.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.870094 dciclient-3.5.0.post202401252113/
--rw-r--r--   0 root         (0) root         (0)    10142 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/LICENSE
--rw-r--r--   0 root         (0) root         (0)       79 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10749 2024-01-31 16:47:57.870094 dciclient-3.5.0.post202401252113/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10025 2024-01-31 16:47:08.000000 dciclient-3.5.0.post202401252113/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.863094 dciclient-3.5.0.post202401252113/dciclient/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4876 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/create_component.py
--rw-r--r--   0 root         (0) root         (0)     6198 2024-01-31 16:47:08.000000 dciclient-3.5.0.post202401252113/dciclient/create_job.py
--rw-r--r--   0 root         (0) root         (0)     5376 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/diff_jobs.py
--rw-r--r--   0 root         (0) root         (0)     5317 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/find_latest_component.py
--rw-r--r--   0 root         (0) root         (0)     4068 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/printer.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/rhel_kernel.py
--rwxr-xr-x   0 root         (0) root         (0)     1236 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/shell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.865095 dciclient-3.5.0.post202401252113/dciclient/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.868094 dciclient-3.5.0.post202401252113/dciclient/v1/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/base.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/component.py
--rw-r--r--   0 root         (0) root         (0)     7447 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/context.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/feeder.py
--rw-r--r--   0 root         (0) root         (0)     3473 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/file.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/identity.py
--rw-r--r--   0 root         (0) root         (0)     4333 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/job.py
--rw-r--r--   0 root         (0) root         (0)     1896 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/jobs_events.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1362 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/product.py
--rw-r--r--   0 root         (0) root         (0)     2030 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/tag.py
--rw-r--r--   0 root         (0) root         (0)     1205 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/team.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/topic.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/api/user.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.870094 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27560 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/cli.py
--rw-r--r--   0 root         (0) root         (0)     1412 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/columns.py
--rw-r--r--   0 root         (0) root         (0)     2785 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/component.py
--rw-r--r--   0 root         (0) root         (0)     3905 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/context.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/feeder.py
--rw-r--r--   0 root         (0) root         (0)      996 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/file.py
--rw-r--r--   0 root         (0) root         (0)     3168 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/job.py
--rw-r--r--   0 root         (0) root         (0)      822 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/jobstate.py
--rw-r--r--   0 root         (0) root         (0)     1558 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1942 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/product.py
--rw-r--r--   0 root         (0) root         (0)     2426 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/purge.py
--rw-r--r--   0 root         (0) root         (0)     2316 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/remoteci.py
--rw-r--r--   0 root         (0) root         (0)     4084 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/runner.py
--rw-r--r--   0 root         (0) root         (0)     1574 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/team.py
--rw-r--r--   0 root         (0) root         (0)     2037 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/topic.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/user.py
--rw-r--r--   0 root         (0) root         (0)     1868 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/v1/utils.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/vault.py
--rw-r--r--   0 root         (0) root         (0)     1838 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/dciclient/vault_client.py
--rw-r--r--   0 root         (0) root         (0)       51 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:47:57.864094 dciclient-3.5.0.post202401252113/dciclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10749 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1716 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      392 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-01-31 16:47:57.000000 dciclient-3.5.0.post202401252113/dciclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-31 16:47:57.870094 dciclient-3.5.0.post202401252113/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     3218 2024-01-31 16:47:08.000000 dciclient-3.5.0.post202401252113/setup.py
--rwxr-xr-x   0 root         (0) root         (0)     1222 2024-01-31 16:47:07.000000 dciclient-3.5.0.post202401252113/start_db.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/
+-rw-r--r--   0 root         (0) root         (0)    10142 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10749 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10025 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.877608 dciclient-3.5.0.post202403281939/dciclient/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/create_component.py
+-rw-r--r--   0 root         (0) root         (0)     6198 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/create_job.py
+-rw-r--r--   0 root         (0) root         (0)     5376 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/diff_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/find_latest_component.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/printer.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/rhel_kernel.py
+-rwxr-xr-x   0 root         (0) root         (0)     1236 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.878608 dciclient-3.5.0.post202403281939/dciclient/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.880608 dciclient-3.5.0.post202403281939/dciclient/v1/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/base.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/component.py
+-rw-r--r--   0 root         (0) root         (0)     7447 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/context.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/feeder.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/file.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/identity.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/job.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/jobs_events.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/product.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/team.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/api/user.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.881608 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28064 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/columns.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/component.py
+-rw-r--r--   0 root         (0) root         (0)     3905 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/context.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/feeder.py
+-rw-r--r--   0 root         (0) root         (0)      996 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/file.py
+-rw-r--r--   0 root         (0) root         (0)     3168 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/job.py
+-rw-r--r--   0 root         (0) root         (0)      822 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/jobstate.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/product.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/purge.py
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/remoteci.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/runner.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/team.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/topic.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/user.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/v1/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/vault.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/dciclient/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 09:54:46.877608 dciclient-3.5.0.post202403281939/dciclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10749 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      392 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-09 09:54:46.000000 dciclient-3.5.0.post202403281939/dciclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 09:54:46.882608 dciclient-3.5.0.post202403281939/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     3218 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)     1222 2024-04-09 09:53:47.000000 dciclient-3.5.0.post202403281939/start_db.sh
```

### Comparing `dciclient-3.5.0.post202401252113/LICENSE` & `dciclient-3.5.0.post202403281939/LICENSE`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/PKG-INFO` & `dciclient-3.5.0.post202403281939/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dciclient
-Version: 3.5.0.post202401252113
+Version: 3.5.0.post202403281939
 Summary: Python client for DCI Control Server
 Home-page: https://github.com/redhat-cip/python-dciclient
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `dciclient-3.5.0.post202401252113/README.md` & `dciclient-3.5.0.post202403281939/README.md`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/create_component.py` & `dciclient-3.5.0.post202403281939/dciclient/create_component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/create_job.py` & `dciclient-3.5.0.post202403281939/dciclient/create_job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/diff_jobs.py` & `dciclient-3.5.0.post202403281939/dciclient/diff_jobs.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/find_latest_component.py` & `dciclient-3.5.0.post202403281939/dciclient/find_latest_component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/printer.py` & `dciclient-3.5.0.post202403281939/dciclient/printer.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/rhel_kernel.py` & `dciclient-3.5.0.post202403281939/dciclient/rhel_kernel.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/shell.py` & `dciclient-3.5.0.post202403281939/dciclient/shell.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/base.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 
 
 def list(context, resource, **kwargs):
     """List all resources"""
     data = utils.sanitize_kwargs(**kwargs)
     id = data.pop("id", None)
     subresource = data.pop("subresource", None)
+    # Note: Control Server gives precedence to "query" over "where"
+    if all(k in data for k in ["where", "query"]):
+        del data["where"]
 
     if subresource:
         uri = "%s/%s/%s/%s" % (context.dci_cs_api, resource, id, subresource)
     else:
         uri = "%s/%s" % (context.dci_cs_api, resource)
 
     return context.session.get(uri, timeout=HTTP_TIMEOUT, params=data)
```

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/component.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/context.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/context.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/feeder.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/feeder.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/file.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/file.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/identity.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/identity.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/job.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/jobs_events.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/jobs_events.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/jobstate.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/pipeline.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/product.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/product.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/remoteci.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/remoteci.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/tag.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/tag.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/team.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/team.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/topic.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/topic.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/api/user.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/api/user.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/exceptions.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/cli.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,20 @@
     # product commands
     p = subparsers.add_parser(
         "product-list", help="List all products.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="product-list")
 
     p = subparsers.add_parser(
         "product-create", help="Create a product.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
@@ -290,15 +295,20 @@
     # topic commands
     p = subparsers.add_parser(
         "topic-list", help="List all topics.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="topic-list")
 
     p = subparsers.add_parser(
         "topic-create", help="Create a topic.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
@@ -361,15 +371,20 @@
     p = subparsers.add_parser(
         "component-list", help="List all components.", parents=[base_parser]
     )
     p.add_argument("--topic-id", required=True, dest="id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="component-list")
 
     p = subparsers.add_parser(
         "component-create", help="Create a component.", parents=[base_parser]
     )
     p.add_argument("display_name", metavar="name")
@@ -445,15 +460,20 @@
         help="List files attached to a component.",
         parents=[base_parser],
     )
     p.add_argument("id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="component-file-list")
 
     p = subparsers.add_parser(
         "component-file-delete", help="Delete a component file.", parents=[base_parser]
     )
     p.add_argument("id")
@@ -465,15 +485,20 @@
     p = subparsers.add_parser(
         "file-list", help="List all files.", parents=[base_parser]
     )
     p.add_argument("job_id")
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="file-list")
 
     p = subparsers.add_parser("file-show", help="Show a file.", parents=[base_parser])
     p.add_argument("id")
     p.set_defaults(command="file-show")
 
@@ -484,15 +509,20 @@
     p.set_defaults(command="file-delete")
 
     # job commands
     p = subparsers.add_parser("job-list", help="List all jobs.", parents=[base_parser])
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=10)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="job-list")
 
     p = subparsers.add_parser("job-show", help="Show a job.", parents=[base_parser])
     p.add_argument("id")
     p.set_defaults(command="job-show")
 
@@ -589,15 +619,20 @@
     # remoteci commands
     p = subparsers.add_parser(
         "remoteci-list", help="List all remotecis.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="remoteci-list")
 
     p = subparsers.add_parser(
         "remoteci-create", help="Create a remoteci.", parents=[base_parser]
     )
     p.add_argument("--name", required=True)
@@ -711,15 +746,20 @@
 
     p = subparsers.add_parser(
         "pipeline-list", help="List all pipelines.", parents=[base_parser]
     )
     p.add_argument("--sort", default="-created_at")
     p.add_argument("--limit", default=50)
     p.add_argument("--offset", default=0)
-    p.add_argument("--where", help="Optional filter criteria", required=False)
+    p.add_argument(
+        "--where",
+        help="Optional filter criteria",
+        default="state:active",
+        required=False,
+    )
     p.add_argument("--query", help="Query language dsl", required=False)
     p.set_defaults(command="pipeline-list")
 
     p = subparsers.add_parser(
         "pipeline-update", help="Update a pipeline.", parents=[base_parser]
     )
     p.add_argument("id")
```

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/columns.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/columns.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/component.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/component.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/context.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/context.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/feeder.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/feeder.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/file.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/file.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/job.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/job.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/jobstate.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/jobstate.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/pipeline.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/product.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/product.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/purge.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/purge.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/remoteci.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/remoteci.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/runner.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/runner.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/team.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/team.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/topic.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/topic.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/shell_commands/user.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/shell_commands/user.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/v1/utils.py` & `dciclient-3.5.0.post202403281939/dciclient/v1/utils.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/vault.py` & `dciclient-3.5.0.post202403281939/dciclient/vault.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient/vault_client.py` & `dciclient-3.5.0.post202403281939/dciclient/vault_client.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/dciclient.egg-info/PKG-INFO` & `dciclient-3.5.0.post202403281939/dciclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dciclient
-Version: 3.5.0.post202401252113
+Version: 3.5.0.post202403281939
 Summary: Python client for DCI Control Server
 Home-page: https://github.com/redhat-cip/python-dciclient
 Author: Distributed CI team
 Author-email: distributed-ci@redhat.com
 License: Apache v2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `dciclient-3.5.0.post202401252113/dciclient.egg-info/SOURCES.txt` & `dciclient-3.5.0.post202403281939/dciclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/setup.py` & `dciclient-3.5.0.post202403281939/setup.py`

 * *Files identical despite different names*

### Comparing `dciclient-3.5.0.post202401252113/start_db.sh` & `dciclient-3.5.0.post202403281939/start_db.sh`

 * *Files identical despite different names*

