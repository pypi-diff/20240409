# Comparing `tmp/psp_liquids_daq_parser-0.0.4.tar.gz` & `tmp/psp_liquids_daq_parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psp_liquids_daq_parser-0.0.4.tar", last modified: Tue Apr  9 05:44:11 2024, max compression
+gzip compressed data, was "psp_liquids_daq_parser-0.0.5.tar", last modified: Tue Apr  9 07:07:46 2024, max compression
```

## Comparing `psp_liquids_daq_parser-0.0.4.tar` & `psp_liquids_daq_parser-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 05:44:09.000000 psp_liquids_daq_parser-0.0.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 05:44:11.700380 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-09 05:44:11.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-09 05:44:07.000000 psp_liquids_daq_parser-0.0.4/src/psp_liquids_daq_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:07:46.199916 psp_liquids_daq_parser-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35821 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-09 07:07:46.199916 psp_liquids_daq_parser-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 07:07:46.199916 psp_liquids_daq_parser-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:07:46.195916 psp_liquids_daq_parser-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 07:07:44.000000 psp_liquids_daq_parser-0.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/src/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/src/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 07:07:46.199916 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-09 07:07:46.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-09 07:07:46.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 07:07:46.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-09 07:07:46.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 07:07:46.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-09 07:07:41.000000 psp_liquids_daq_parser-0.0.5/src/psp_liquids_daq_parser.py
```

### Comparing `psp_liquids_daq_parser-0.0.4/LICENSE` & `psp_liquids_daq_parser-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psp_liquids_daq_parser-0.0.4/pyproject.toml` & `psp_liquids_daq_parser-0.0.5/pyproject.toml`

 * *Files identical despite different names*

