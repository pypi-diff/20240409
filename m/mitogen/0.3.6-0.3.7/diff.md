# Comparing `tmp/mitogen-0.3.6.tar.gz` & `tmp/mitogen-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitogen-0.3.6.tar", last modified: Thu Apr  4 12:55:07 2024, max compression
+gzip compressed data, was "mitogen-0.3.7.tar", last modified: Tue Apr  9 08:14:03 2024, max compression
```

## Comparing `mitogen-0.3.6.tar` & `mitogen-0.3.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793728 mitogen-0.3.6/
--rw-r--r--   0 alex       (501) staff       (20)     1465 2022-06-24 21:10:35.000000 mitogen-0.3.6/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       16 2022-06-24 21:04:22.000000 mitogen-0.3.6/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-04 12:55:07.793673 mitogen-0.3.6/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      495 2022-06-24 21:10:35.000000 mitogen-0.3.6/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.782550 mitogen-0.3.6/ansible_mitogen/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/affinity.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.782931 mitogen-0.3.6/ansible_mitogen/compat/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    39735 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/connection.py
--rw-r--r--   0 alex       (501) staff       (20)     3851 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/loaders.py
--rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/logging.py
--rw-r--r--   0 alex       (501) staff       (20)    21609 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/mixins.py
--rw-r--r--   0 alex       (501) staff       (20)     9588 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/module_finder.py
--rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/parsing.py
--rw-r--r--   0 alex       (501) staff       (20)    22044 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/planner.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.783031 mitogen-0.3.6/ansible_mitogen/plugins/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.783524 mitogen-0.3.6/ansible_mitogen/plugins/action/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_fetch.py
--rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_get_stack.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.785716 mitogen-0.3.6/ansible_mitogen/plugins/connection/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_buildah.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_doas.py
--rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_docker.py
--rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_jail.py
--rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_kubectl.py
--rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_local.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxd.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_machinectl.py
--rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_podman.py
--rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_setns.py
--rw-r--r--   0 alex       (501) staff       (20)     3301 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_ssh.py
--rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_su.py
--rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_sudo.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.786339 mitogen-0.3.6/ansible_mitogen/plugins/strategy/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen.py
--rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_free.py
--rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
--rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-24 21:10:35.000000 mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_linear.py
--rw-r--r--   0 alex       (501) staff       (20)    24921 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/process.py
--rw-r--r--   0 alex       (501) staff       (20)    37900 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/runner.py
--rw-r--r--   0 alex       (501) staff       (20)    20677 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/services.py
--rw-r--r--   0 alex       (501) staff       (20)    12611 2024-03-28 16:09:46.000000 mitogen-0.3.6/ansible_mitogen/strategy.py
--rw-r--r--   0 alex       (501) staff       (20)    25091 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/target.py
--rw-r--r--   0 alex       (501) staff       (20)    27116 2024-03-28 16:31:39.000000 mitogen-0.3.6/ansible_mitogen/transport_config.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.786566 mitogen-0.3.6/ansible_mitogen/utils/
--rw-r--r--   0 alex       (501) staff       (20)      604 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/utils/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2586 2024-04-04 12:53:20.000000 mitogen-0.3.6/ansible_mitogen/utils/unsafe.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.791856 mitogen-0.3.6/mitogen/
--rw-r--r--   0 alex       (501) staff       (20)     4145 2024-04-04 12:53:20.000000 mitogen-0.3.6/mitogen/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2681 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/buildah.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.792865 mitogen-0.3.6/mitogen/compat/
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.6/mitogen/compat/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    20406 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/compat/pkgutil.py
--rw-r--r--   0 alex       (501) staff       (20)    17572 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/compat/tokenize.py
--rw-r--r--   0 alex       (501) staff       (20)   151746 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/core.py
--rw-r--r--   0 alex       (501) staff       (20)     6699 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/debug.py
--rw-r--r--   0 alex       (501) staff       (20)     4958 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/doas.py
--rw-r--r--   0 alex       (501) staff       (20)     3085 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/docker.py
--rw-r--r--   0 alex       (501) staff       (20)    15577 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/fakessh.py
--rw-r--r--   0 alex       (501) staff       (20)     8436 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/fork.py
--rw-r--r--   0 alex       (501) staff       (20)     2537 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/jail.py
--rw-r--r--   0 alex       (501) staff       (20)     2561 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/kubectl.py
--rw-r--r--   0 alex       (501) staff       (20)     2853 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/lxc.py
--rw-r--r--   0 alex       (501) staff       (20)     2844 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/lxd.py
--rw-r--r--   0 alex       (501) staff       (20)    55088 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/master.py
--rw-r--r--   0 alex       (501) staff       (20)     5093 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/minify.py
--rw-r--r--   0 alex       (501) staff       (20)     6624 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/os_fork.py
--rw-r--r--   0 alex       (501) staff       (20)    98171 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/parent.py
--rw-r--r--   0 alex       (501) staff       (20)     2730 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/podman.py
--rw-r--r--   0 alex       (501) staff       (20)     5392 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/profiler.py
--rw-r--r--   0 alex       (501) staff       (20)    12325 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/select.py
--rw-r--r--   0 alex       (501) staff       (20)    41699 2024-03-28 16:31:39.000000 mitogen-0.3.6/mitogen/service.py
--rw-r--r--   0 alex       (501) staff       (20)     8450 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/setns.py
--rw-r--r--   0 alex       (501) staff       (20)    10892 2024-03-28 16:09:56.000000 mitogen-0.3.6/mitogen/ssh.py
--rw-r--r--   0 alex       (501) staff       (20)     5656 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/su.py
--rw-r--r--   0 alex       (501) staff       (20)    12089 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/sudo.py
--rw-r--r--   0 alex       (501) staff       (20)     7133 2023-08-10 08:38:54.000000 mitogen-0.3.6/mitogen/unix.py
--rw-r--r--   0 alex       (501) staff       (20)     7694 2024-04-04 12:53:20.000000 mitogen-0.3.6/mitogen/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793492 mitogen-0.3.6/mitogen.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     2471 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/not-zip-safe
--rw-r--r--   0 alex       (501) staff       (20)       24 2024-04-04 12:55:07.000000 mitogen-0.3.6/mitogen.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)      206 2024-04-04 12:55:07.793921 mitogen-0.3.6/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)     3591 2024-03-28 16:31:39.000000 mitogen-0.3.6/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-04 12:55:07.793123 mitogen-0.3.6/tests/
--rw-r--r--   0 alex       (501) staff       (20)    20874 2024-03-28 16:31:39.000000 mitogen-0.3.6/tests/testlib.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.099621 mitogen-0.3.7/
+-rw-r--r--   0 alex       (501) staff       (20)     1465 2022-06-24 21:10:35.000000 mitogen-0.3.7/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)       16 2022-06-24 21:04:22.000000 mitogen-0.3.7/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-09 08:14:03.099560 mitogen-0.3.7/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      495 2022-06-24 21:10:35.000000 mitogen-0.3.7/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.086912 mitogen-0.3.7/ansible_mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    10196 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/affinity.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.087256 mitogen-0.3.7/ansible_mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    39735 2024-04-08 22:49:41.000000 mitogen-0.3.7/ansible_mitogen/connection.py
+-rw-r--r--   0 alex       (501) staff       (20)     3851 2024-04-09 08:11:01.000000 mitogen-0.3.7/ansible_mitogen/loaders.py
+-rw-r--r--   0 alex       (501) staff       (20)     4924 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)    21609 2024-04-08 22:49:41.000000 mitogen-0.3.7/ansible_mitogen/mixins.py
+-rw-r--r--   0 alex       (501) staff       (20)     9588 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/module_finder.py
+-rw-r--r--   0 alex       (501) staff       (20)     3122 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/parsing.py
+-rw-r--r--   0 alex       (501) staff       (20)    22044 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/planner.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.087343 mitogen-0.3.7/ansible_mitogen/plugins/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/plugins/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.087834 mitogen-0.3.7/ansible_mitogen/plugins/action/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/plugins/action/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     9840 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/action/mitogen_fetch.py
+-rw-r--r--   0 alex       (501) staff       (20)     2448 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/action/mitogen_get_stack.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.090265 mitogen-0.3.7/ansible_mitogen/plugins/connection/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1928 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_buildah.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     2088 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_docker.py
+-rw-r--r--   0 alex       (501) staff       (20)     1925 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     3119 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     3134 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_local.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     1924 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_machinectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     1935 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     1937 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_setns.py
+-rw-r--r--   0 alex       (501) staff       (20)     3301 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     1942 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_su.py
+-rw-r--r--   0 alex       (501) staff       (20)     1944 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_sudo.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.090941 mitogen-0.3.7/ansible_mitogen/plugins/strategy/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/ansible_mitogen/plugins/strategy/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2805 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen.py
+-rw-r--r--   0 alex       (501) staff       (20)     2811 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_free.py
+-rw-r--r--   0 alex       (501) staff       (20)     2943 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py
+-rw-r--r--   0 alex       (501) staff       (20)     2813 2022-06-24 21:10:35.000000 mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_linear.py
+-rw-r--r--   0 alex       (501) staff       (20)    24921 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/process.py
+-rw-r--r--   0 alex       (501) staff       (20)    37900 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/runner.py
+-rw-r--r--   0 alex       (501) staff       (20)    20677 2024-04-08 22:49:41.000000 mitogen-0.3.7/ansible_mitogen/services.py
+-rw-r--r--   0 alex       (501) staff       (20)    12611 2024-03-28 16:09:46.000000 mitogen-0.3.7/ansible_mitogen/strategy.py
+-rw-r--r--   0 alex       (501) staff       (20)    25091 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/target.py
+-rw-r--r--   0 alex       (501) staff       (20)    27116 2024-03-28 16:31:39.000000 mitogen-0.3.7/ansible_mitogen/transport_config.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.091338 mitogen-0.3.7/ansible_mitogen/utils/
+-rw-r--r--   0 alex       (501) staff       (20)      604 2024-04-08 22:49:41.000000 mitogen-0.3.7/ansible_mitogen/utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2586 2024-04-08 22:49:41.000000 mitogen-0.3.7/ansible_mitogen/utils/unsafe.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.097218 mitogen-0.3.7/mitogen/
+-rw-r--r--   0 alex       (501) staff       (20)     4145 2024-04-09 08:11:01.000000 mitogen-0.3.7/mitogen/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2681 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/buildah.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.098491 mitogen-0.3.7/mitogen/compat/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2022-06-24 21:04:22.000000 mitogen-0.3.7/mitogen/compat/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    20406 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/compat/pkgutil.py
+-rw-r--r--   0 alex       (501) staff       (20)    17572 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/compat/tokenize.py
+-rw-r--r--   0 alex       (501) staff       (20)   151746 2024-03-28 16:31:39.000000 mitogen-0.3.7/mitogen/core.py
+-rw-r--r--   0 alex       (501) staff       (20)     6699 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/debug.py
+-rw-r--r--   0 alex       (501) staff       (20)     4958 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/doas.py
+-rw-r--r--   0 alex       (501) staff       (20)     3085 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/docker.py
+-rw-r--r--   0 alex       (501) staff       (20)    15577 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/fakessh.py
+-rw-r--r--   0 alex       (501) staff       (20)     8436 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/fork.py
+-rw-r--r--   0 alex       (501) staff       (20)     2537 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/jail.py
+-rw-r--r--   0 alex       (501) staff       (20)     2561 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/kubectl.py
+-rw-r--r--   0 alex       (501) staff       (20)     2853 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/lxc.py
+-rw-r--r--   0 alex       (501) staff       (20)     2844 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/lxd.py
+-rw-r--r--   0 alex       (501) staff       (20)    55088 2024-03-28 16:31:39.000000 mitogen-0.3.7/mitogen/master.py
+-rw-r--r--   0 alex       (501) staff       (20)     5093 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/minify.py
+-rw-r--r--   0 alex       (501) staff       (20)     6624 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/os_fork.py
+-rw-r--r--   0 alex       (501) staff       (20)    98171 2024-03-28 16:31:39.000000 mitogen-0.3.7/mitogen/parent.py
+-rw-r--r--   0 alex       (501) staff       (20)     2730 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/podman.py
+-rw-r--r--   0 alex       (501) staff       (20)     5392 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/profiler.py
+-rw-r--r--   0 alex       (501) staff       (20)    12325 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/select.py
+-rw-r--r--   0 alex       (501) staff       (20)    41699 2024-03-28 16:31:39.000000 mitogen-0.3.7/mitogen/service.py
+-rw-r--r--   0 alex       (501) staff       (20)     8450 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/setns.py
+-rw-r--r--   0 alex       (501) staff       (20)    10892 2024-03-28 16:09:56.000000 mitogen-0.3.7/mitogen/ssh.py
+-rw-r--r--   0 alex       (501) staff       (20)     5656 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/su.py
+-rw-r--r--   0 alex       (501) staff       (20)    12089 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/sudo.py
+-rw-r--r--   0 alex       (501) staff       (20)     7133 2023-08-10 08:38:54.000000 mitogen-0.3.7/mitogen/unix.py
+-rw-r--r--   0 alex       (501) staff       (20)     7694 2024-04-08 22:49:41.000000 mitogen-0.3.7/mitogen/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.099322 mitogen-0.3.7/mitogen.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     1776 2024-04-09 08:14:03.000000 mitogen-0.3.7/mitogen.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     2471 2024-04-09 08:14:03.000000 mitogen-0.3.7/mitogen.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-09 08:14:03.000000 mitogen-0.3.7/mitogen.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-04 12:55:07.000000 mitogen-0.3.7/mitogen.egg-info/not-zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)       24 2024-04-09 08:14:03.000000 mitogen-0.3.7/mitogen.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)      206 2024-04-09 08:14:03.099835 mitogen-0.3.7/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)     3591 2024-03-28 16:31:39.000000 mitogen-0.3.7/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-09 08:14:03.098845 mitogen-0.3.7/tests/
+-rw-r--r--   0 alex       (501) staff       (20)    20874 2024-03-28 16:31:39.000000 mitogen-0.3.7/tests/testlib.py
```

### Comparing `mitogen-0.3.6/LICENSE` & `mitogen-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/PKG-INFO` & `mitogen-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.6
+Version: 0.3.7
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.6 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.7 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
 hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
 Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
```

### Comparing `mitogen-0.3.6/ansible_mitogen/affinity.py` & `mitogen-0.3.7/ansible_mitogen/affinity.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/connection.py` & `mitogen-0.3.7/ansible_mitogen/connection.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/loaders.py` & `mitogen-0.3.7/ansible_mitogen/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'module_utils_loader',
     'shell_loader',
     'strategy_loader',
 ]
 
 
 ANSIBLE_VERSION_MIN = (2, 10)
-ANSIBLE_VERSION_MAX = (2, 14)
+ANSIBLE_VERSION_MAX = (2, 16)
 
 NEW_VERSION_MSG = (
     "Your Ansible version (%s) is too recent. The most recent version\n"
     "supported by Mitogen for Ansible is %s.x. Please check the Mitogen\n"
     "release notes to see if a new version is available, otherwise\n"
     "subscribe to the corresponding GitHub issue to be notified when\n"
     "support becomes available.\n"
```

### Comparing `mitogen-0.3.6/ansible_mitogen/logging.py` & `mitogen-0.3.7/ansible_mitogen/logging.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/mixins.py` & `mitogen-0.3.7/ansible_mitogen/mixins.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/module_finder.py` & `mitogen-0.3.7/ansible_mitogen/module_finder.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/parsing.py` & `mitogen-0.3.7/ansible_mitogen/parsing.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/planner.py` & `mitogen-0.3.7/ansible_mitogen/planner.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_fetch.py` & `mitogen-0.3.7/ansible_mitogen/plugins/action/mitogen_fetch.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/action/mitogen_get_stack.py` & `mitogen-0.3.7/ansible_mitogen/plugins/action/mitogen_get_stack.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_buildah.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_doas.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_docker.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_docker.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_jail.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_kubectl.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_local.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_local.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxc.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_lxc.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_lxd.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_machinectl.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_machinectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_podman.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_setns.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_ssh.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_ssh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_su.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_su.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/connection/mitogen_sudo.py` & `mitogen-0.3.7/ansible_mitogen/plugins/connection/mitogen_sudo.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen.py` & `mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_free.py` & `mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py` & `mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/plugins/strategy/mitogen_linear.py` & `mitogen-0.3.7/ansible_mitogen/plugins/strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/process.py` & `mitogen-0.3.7/ansible_mitogen/process.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/runner.py` & `mitogen-0.3.7/ansible_mitogen/runner.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/services.py` & `mitogen-0.3.7/ansible_mitogen/services.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/strategy.py` & `mitogen-0.3.7/ansible_mitogen/strategy.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/target.py` & `mitogen-0.3.7/ansible_mitogen/target.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/transport_config.py` & `mitogen-0.3.7/ansible_mitogen/transport_config.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/utils/__init__.py` & `mitogen-0.3.7/ansible_mitogen/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/ansible_mitogen/utils/unsafe.py` & `mitogen-0.3.7/ansible_mitogen/utils/unsafe.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/__init__.py` & `mitogen-0.3.7/mitogen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 """
 On the Mitogen master, this is imported from ``mitogen/__init__.py`` as would
 be expected. On the slave, it is built dynamically during startup.
 """
 
 
 #: Library version as a tuple.
-__version__ = (0, 3, 6)
+__version__ = (0, 3, 7)
 
 
 #: This is :data:`False` in slave contexts. Previously it was used to prevent
 #: re-execution of :mod:`__main__` in single file programs, however that now
 #: happens automatically.
 is_master = True
```

### Comparing `mitogen-0.3.6/mitogen/buildah.py` & `mitogen-0.3.7/mitogen/buildah.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/compat/pkgutil.py` & `mitogen-0.3.7/mitogen/compat/pkgutil.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/compat/tokenize.py` & `mitogen-0.3.7/mitogen/compat/tokenize.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/core.py` & `mitogen-0.3.7/mitogen/core.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/debug.py` & `mitogen-0.3.7/mitogen/debug.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/doas.py` & `mitogen-0.3.7/mitogen/doas.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/docker.py` & `mitogen-0.3.7/mitogen/docker.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/fakessh.py` & `mitogen-0.3.7/mitogen/fakessh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/fork.py` & `mitogen-0.3.7/mitogen/fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/jail.py` & `mitogen-0.3.7/mitogen/jail.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/kubectl.py` & `mitogen-0.3.7/mitogen/kubectl.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/lxc.py` & `mitogen-0.3.7/mitogen/lxc.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/lxd.py` & `mitogen-0.3.7/mitogen/lxd.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/master.py` & `mitogen-0.3.7/mitogen/master.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/minify.py` & `mitogen-0.3.7/mitogen/minify.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/os_fork.py` & `mitogen-0.3.7/mitogen/os_fork.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/parent.py` & `mitogen-0.3.7/mitogen/parent.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/podman.py` & `mitogen-0.3.7/mitogen/podman.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/profiler.py` & `mitogen-0.3.7/mitogen/profiler.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/select.py` & `mitogen-0.3.7/mitogen/select.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/service.py` & `mitogen-0.3.7/mitogen/service.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/setns.py` & `mitogen-0.3.7/mitogen/setns.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/ssh.py` & `mitogen-0.3.7/mitogen/ssh.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/su.py` & `mitogen-0.3.7/mitogen/su.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/sudo.py` & `mitogen-0.3.7/mitogen/sudo.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/unix.py` & `mitogen-0.3.7/mitogen/unix.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen/utils.py` & `mitogen-0.3.7/mitogen/utils.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/mitogen.egg-info/PKG-INFO` & `mitogen-0.3.7/mitogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitogen
-Version: 0.3.6
+Version: 0.3.7
 Summary: Library for writing distributed self-replicating programs.
 Home-page: https://github.com/mitogen-hq/mitogen/
 Author: David Wilson
 License: New BSD
 Classifier: Environment :: Console
 Classifier: Framework :: Ansible
 Classifier: Intended Audience :: System Administrators
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mitogen Version: 0.3.6 Summary: Library for writing
+Metadata-Version: 2.1 Name: mitogen Version: 0.3.7 Summary: Library for writing
 distributed self-replicating programs. Home-page: https://github.com/mitogen-
 hq/mitogen/ Author: David Wilson License: New BSD Classifier: Environment ::
 Console Classifier: Framework :: Ansible Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 2.7 Classifier: Programming Language :: Python :: 3
```

### Comparing `mitogen-0.3.6/mitogen.egg-info/SOURCES.txt` & `mitogen-0.3.7/mitogen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/setup.py` & `mitogen-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `mitogen-0.3.6/tests/testlib.py` & `mitogen-0.3.7/tests/testlib.py`

 * *Files identical despite different names*

