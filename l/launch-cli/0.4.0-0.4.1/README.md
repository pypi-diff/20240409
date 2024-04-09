# Comparing `tmp/launch-cli-0.4.0.tar.gz` & `tmp/launch-cli-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch-cli-0.4.0.tar", last modified: Mon Apr  8 20:45:19 2024, max compression
+gzip compressed data, was "launch-cli-0.4.1.tar", last modified: Tue Apr  9 19:05:11 2024, max compression
```

## Comparing `launch-cli-0.4.0.tar` & `launch-cli-0.4.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 20:45:06.000000 launch-cli-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-08 20:45:19.760166 launch-cli-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-08 20:45:06.000000 launch-cli-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/launch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 20:45:19.000000 launch-cli-0.4.0/launch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-08 20:45:06.000000 launch-cli-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:45:19.760166 launch-cli-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.748166 launch-cli-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/common/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/helm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/helm/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/aws/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.752166 launch-cli-0.4.0/src/launch/automation/provider/az/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/az/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/provider/az/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/automation/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/automation/terragrunt/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/access/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/access/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/hooks/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/repo/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/repo/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/github/version/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/github/version/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/helm/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/helm/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/service/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/cli/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/cli/terragrunt/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.756166 launch-cli-0.4.0/src/launch/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/github/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/src/launch/local_repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/local_repo/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:19.760166 launch-cli-0.4.0/src/launch/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-08 20:45:06.000000 launch-cli-0.4.0/src/launch/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 19:04:59.000000 launch-cli-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-09 19:05:11.935057 launch-cli-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-09 19:04:59.000000 launch-cli-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/launch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:05:11.000000 launch-cli-0.4.1/launch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 19:04:59.000000 launch-cli-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:05:11.935057 launch-cli-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.923057 launch-cli-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/common/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/helm/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/aws/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/provider/az/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/az/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/provider/az/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.927057 launch-cli-0.4.1/src/launch/automation/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/automation/terragrunt/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/access/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/access/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/hooks/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/repo/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/github/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/github/version/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/helm/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/cli/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/cli/terragrunt/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.931057 launch-cli-0.4.1/src/launch/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/github/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/src/launch/local_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/local_repo/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:05:11.935057 launch-cli-0.4.1/src/launch/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-09 19:04:59.000000 launch-cli-0.4.1/src/launch/update.py
```

### Comparing `launch-cli-0.4.0/LICENSE` & `launch-cli-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/PKG-INFO` & `launch-cli-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.4.0
+Version: 0.4.1
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch-cli-0.4.0/README.md` & `launch-cli-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/launch_cli.egg-info/PKG-INFO` & `launch-cli-0.4.1/launch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.4.0
+Version: 0.4.1
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch-cli-0.4.0/launch_cli.egg-info/SOURCES.txt` & `launch-cli-0.4.1/launch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/pyproject.toml` & `launch-cli-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launch-cli"
-version = "0.4.0"
+version = "0.4.1"
 description = "CLI tooling for common Launch functions"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `launch-cli-0.4.0/src/launch/__init__.py` & `launch-cli-0.4.1/src/launch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from semver import Version
 
-VERSION = "0.4.0"
+VERSION = "0.4.1"
 
 SEMANTIC_VERSION = Version.parse(VERSION)
 GITHUB_ORG_NAME = "launchbynttdata"
 GITHUB_REPO_NAME = "launch-cli"
 SERVICE_SKELETON = "https://github.com/launchbynttdata/launch-terragrunt-skeleton.git"
 SKELETON_BRANCH = "main"
 MAIN_BRANCH = "main"
```

### Comparing `launch-cli-0.4.0/src/launch/automation/common/functions.py` & `launch-cli-0.4.1/src/launch/automation/common/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/automation/helm/functions.py` & `launch-cli-0.4.1/src/launch/automation/helm/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/automation/provider/aws/functions.py` & `launch-cli-0.4.1/src/launch/automation/provider/aws/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/automation/provider/az/functions.py` & `launch-cli-0.4.1/src/launch/automation/provider/az/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/automation/terragrunt/functions.py` & `launch-cli-0.4.1/src/launch/automation/terragrunt/functions.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/entrypoint.py` & `launch-cli-0.4.1/src/launch/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/github/access/commands.py` & `launch-cli-0.4.1/src/launch/cli/github/access/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/github/hooks/commands.py` & `launch-cli-0.4.1/src/launch/cli/github/hooks/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/github/repo/commands.py` & `launch-cli-0.4.1/src/launch/cli/github/repo/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/github/version/commands.py` & `launch-cli-0.4.1/src/launch/cli/github/version/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/helm/commands.py` & `launch-cli-0.4.1/src/launch/cli/helm/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/service/commands.py` & `launch-cli-0.4.1/src/launch/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/cli/terragrunt/commands.py` & `launch-cli-0.4.1/src/launch/cli/terragrunt/commands.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/env.py` & `launch-cli-0.4.1/src/launch/env.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/github/access.py` & `launch-cli-0.4.1/src/launch/github/access.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/github/auth.py` & `launch-cli-0.4.1/src/launch/github/auth.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/github/hooks.py` & `launch-cli-0.4.1/src/launch/github/hooks.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/github/repo.py` & `launch-cli-0.4.1/src/launch/github/repo.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/github/tags.py` & `launch-cli-0.4.1/src/launch/github/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/local_repo/predict.py` & `launch-cli-0.4.1/src/launch/local_repo/predict.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/local_repo/repo.py` & `launch-cli-0.4.1/src/launch/local_repo/repo.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/local_repo/tags.py` & `launch-cli-0.4.1/src/launch/local_repo/tags.py`

 * *Files identical despite different names*

### Comparing `launch-cli-0.4.0/src/launch/service/common.py` & `launch-cli-0.4.1/src/launch/service/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import re
 import shutil
 import uuid
 from pathlib import Path
 from typing import List
 
-import yaml
 from git.repo import Repo
 from jinja2 import Environment, FileSystemLoader
+from ruamel.yaml import YAML
 
 from launch import BUILD_DEPENDENCIES_DIR, SERVICE_SKELETON, SKELETON_BRANCH
 from launch.automation.common.functions import (
     extract_uuid_key,
     recursive_dictionary_merge,
 )
 
@@ -169,23 +169,23 @@
 
 
 def write_text(
     path: Path, data: dict, output_format: str = "json", indent: int = 4
 ) -> None:
     if output_format == "json":
         serialized_data = json.dumps(data, indent=indent)
+        path.write_text(serialized_data)
     elif output_format == "yaml":
-        serialized_data = yaml.dump(data, indent=indent)
+        yaml = YAML()
+        yaml.dump(data=data, stream=path)
     else:
         message = f"Unsupported output format: {output_format}"
         logger.error(message)
         raise ValueError(message)
 
-    path.write_text(serialized_data)
-
 
 def input_data_validation(input_data: dict) -> dict:
     if not "skeleton" in input_data:
         input_data["skeleton"]: dict[str, str] = {}
     if not "url" in input_data["skeleton"] or not input_data["skeleton"]["url"]:
         logger.info(f"No skeleton url provided, using default: {SERVICE_SKELETON}")
         input_data["skeleton"]["url"] = SERVICE_SKELETON
```

### Comparing `launch-cli-0.4.0/src/launch/update.py` & `launch-cli-0.4.1/src/launch/update.py`

 * *Files identical despite different names*

