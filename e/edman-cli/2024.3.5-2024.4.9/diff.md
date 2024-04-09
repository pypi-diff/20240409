# Comparing `tmp/edman_cli-2024.3.5.tar.gz` & `tmp/edman_cli-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_cli-2024.3.5.tar", last modified: Tue Mar  5 01:18:47 2024, max compression
+gzip compressed data, was "edman_cli-2024.4.9.tar", last modified: Tue Apr  9 01:48:09 2024, max compression
```

## Comparing `edman_cli-2024.3.5.tar` & `edman_cli-2024.4.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2024.3.5/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7264 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     5613 2023-11-20 08:06:08.000000 edman_cli-2024.3.5/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/edman_cli.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     7264 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1515 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/entry_points.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       76 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2024-03-05 01:18:47.000000 edman_cli-2024.3.5/edman_cli.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1471 2024-03-05 01:17:26.000000 edman_cli-2024.3.5/pyproject.toml
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.841134 edman_cli-2024.3.5/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16648 2023-11-17 06:13:18.000000 edman_cli-2024.3.5/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2305 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3523 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2757 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1626 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2666 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2297 2023-11-17 06:13:18.000000 edman_cli-2024.3.5/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3033 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2519 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2406 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2708 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2166 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2492 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2163 2023-05-24 05:52:45.000000 edman_cli-2024.3.5/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/setup.cfg
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    11565 2023-12-06 06:13:48.000000 edman_cli-2024.3.5/tests/test_action.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.841134 edman_cli-2024.3.5/venv/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/venv/bin/
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2024.3.5/venv/bin/jp.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2html.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2html4.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2html5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2latex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2man.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2odt.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2s5.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2xetex.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rst2xml.py
--rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 02:30:36.000000 edman_cli-2024.3.5/venv/bin/rstpep2html.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.841134 edman_cli-2024.3.5/venv/src/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/venv/src/edman-cli/
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/venv/src/edman-cli/scripts/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/action.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/assign_bson_type.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/db_create.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/db_destroy.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/entry.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_add.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_dl.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/find.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/item_delete.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/pullout.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/structure_convert.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/scripts/update.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-03-05 01:18:47.851134 edman_cli-2024.3.5/venv/src/edman-cli/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/tests/__init__.py
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2024.3.5/venv/src/edman-cli/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.680575 edman_cli-2024.4.9/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2024.4.9/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7264 2024-04-09 01:48:09.680575 edman_cli-2024.4.9/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     5613 2023-11-20 08:06:08.000000 edman_cli-2024.4.9/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.680575 edman_cli-2024.4.9/edman_cli.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     7264 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1515 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       76 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2024-04-09 01:48:09.000000 edman_cli-2024.4.9/edman_cli.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1471 2024-04-09 01:46:51.000000 edman_cli-2024.4.9/pyproject.toml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16648 2023-11-17 06:13:18.000000 edman_cli-2024.4.9/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2305 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3523 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2757 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1626 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2666 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2297 2023-11-17 06:13:18.000000 edman_cli-2024.4.9/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3033 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2519 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2406 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2708 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2166 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2492 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2163 2023-05-24 05:52:45.000000 edman_cli-2024.4.9/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2024-04-09 01:48:09.680575 edman_cli-2024.4.9/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    11565 2023-12-06 06:13:48.000000 edman_cli-2024.4.9/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.660575 edman_cli-2024.4.9/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2024.4.9/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      630 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-18 02:30:36.000000 edman_cli-2024.4.9/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.660575 edman_cli-2024.4.9/venv/src/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/venv/src/edman-cli/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/venv/src/edman-cli/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2024-04-09 01:48:09.670575 edman_cli-2024.4.9/venv/src/edman-cli/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/tests/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2024.4.9/venv/src/edman-cli/tests/test_action.py
```

### Comparing `edman_cli-2024.3.5/LICENSE.txt` & `edman_cli-2024.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/PKG-INFO` & `edman_cli-2024.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -20,15 +20,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pymongo~=4.6.2
 Requires-Dist: python-dateutil~=2.9.0.post0
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: edman~=2024.3.5
+Requires-Dist: edman~=2024.4.9
 
 edman_cli
 =========
 
 |py_version|
 
 |  EDMAN(KEK IMSS SBRC/PF Experimental Data Management System)用のコマンドラインスクリプト。
```

### Comparing `edman_cli-2024.3.5/README.rst` & `edman_cli-2024.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/edman_cli.egg-info/PKG-INFO` & `edman_cli-2024.4.9/edman_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edman_cli
-Version: 2024.3.5
+Version: 2024.4.9
 Summary: Sub-package of edman for cli applications and scripts.
 Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
         
         Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -20,15 +20,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pymongo~=4.6.2
 Requires-Dist: python-dateutil~=2.9.0.post0
 Requires-Dist: jmespath~=1.0.1
-Requires-Dist: edman~=2024.3.5
+Requires-Dist: edman~=2024.4.9
 
 edman_cli
 =========
 
 |py_version|
 
 |  EDMAN(KEK IMSS SBRC/PF Experimental Data Management System)用のコマンドラインスクリプト。
```

### Comparing `edman_cli-2024.3.5/edman_cli.egg-info/SOURCES.txt` & `edman_cli-2024.4.9/edman_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/edman_cli.egg-info/entry_points.txt` & `edman_cli-2024.4.9/edman_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/pyproject.toml` & `edman_cli-2024.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Database :: Front-Ends",
 ]
 dependencies = [
     "pymongo~=4.6.2",
     "python-dateutil~=2.9.0.post0",
     "jmespath~=1.0.1",
-    "edman~=2024.3.5",
+    "edman~=2024.4.9",
 ]
-version = "2024.3.5"
+version = "2024.4.9"
 
 [project.urls]
 "repository" = "https://github.com/ryde/edman_cli"
 
 [tool.setuptools.packages.find]
 exclude = ["tests"]
```

### Comparing `edman_cli-2024.3.5/scripts/action.py` & `edman_cli-2024.4.9/scripts/action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/assign_bson_type.py` & `edman_cli-2024.4.9/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/db_create.py` & `edman_cli-2024.4.9/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/db_destroy.py` & `edman_cli-2024.4.9/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/delete.py` & `edman_cli-2024.4.9/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/entry.py` & `edman_cli-2024.4.9/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/file_add.py` & `edman_cli-2024.4.9/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/file_delete.py` & `edman_cli-2024.4.9/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/file_dl.py` & `edman_cli-2024.4.9/scripts/file_dl.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/find.py` & `edman_cli-2024.4.9/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/item_delete.py` & `edman_cli-2024.4.9/scripts/item_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/pullout.py` & `edman_cli-2024.4.9/scripts/pullout.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/structure_convert.py` & `edman_cli-2024.4.9/scripts/structure_convert.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/scripts/update.py` & `edman_cli-2024.4.9/scripts/update.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/tests/test_action.py` & `edman_cli-2024.4.9/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/jp.py` & `edman_cli-2024.4.9/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2html.py` & `edman_cli-2024.4.9/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2html4.py` & `edman_cli-2024.4.9/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2html5.py` & `edman_cli-2024.4.9/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2latex.py` & `edman_cli-2024.4.9/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2man.py` & `edman_cli-2024.4.9/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2odt.py` & `edman_cli-2024.4.9/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2odt_prepstyles.py` & `edman_cli-2024.4.9/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2pseudoxml.py` & `edman_cli-2024.4.9/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2s5.py` & `edman_cli-2024.4.9/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2xetex.py` & `edman_cli-2024.4.9/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rst2xml.py` & `edman_cli-2024.4.9/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/bin/rstpep2html.py` & `edman_cli-2024.4.9/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/action.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/action.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/assign_bson_type.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/assign_bson_type.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/db_create.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/db_create.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/db_destroy.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/db_destroy.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/delete.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/entry.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/entry.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_add.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_add.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_delete.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/file_dl.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/file_dl.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/find.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/find.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/item_delete.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/item_delete.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/pullout.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/pullout.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/structure_convert.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/structure_convert.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/scripts/update.py` & `edman_cli-2024.4.9/venv/src/edman-cli/scripts/update.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/setup.py` & `edman_cli-2024.4.9/venv/src/edman-cli/setup.py`

 * *Files identical despite different names*

### Comparing `edman_cli-2024.3.5/venv/src/edman-cli/tests/test_action.py` & `edman_cli-2024.4.9/venv/src/edman-cli/tests/test_action.py`

 * *Files identical despite different names*

