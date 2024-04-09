# Comparing `tmp/waylay-beta-0.7.1.tar.gz` & `tmp/waylay-beta-9.9.9b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay-beta-0.7.1.tar", last modified: Tue Nov  7 12:23:44 2023, max compression
+gzip compressed data, was "waylay-beta-9.9.9b9.tar", last modified: Tue Apr  9 07:48:06 2024, max compression
```

## Comparing `waylay-beta-0.7.1.tar` & `waylay-beta-9.9.9b9.tar`

### file list

```diff
@@ -1,100 +1,15 @@
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.789765 waylay-beta-0.7.1/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      746 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/LICENSE.txt
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      214 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/MANIFEST.in
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     6648 2023-11-07 12:23:44.788385 waylay-beta-0.7.1/PKG-INFO
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2281 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/README.md
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.674831 waylay-beta-0.7.1/doc/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1825 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/doc/byoml_runtimes.json
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2529 2023-11-07 11:50:37.000000 waylay-beta-0.7.1/doc/dist.README.md
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1300 2023-11-07 12:23:44.793523 waylay-beta-0.7.1/setup.cfg
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2960 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/setup.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    81180 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/versioneer.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.794076 waylay-beta-0.7.1/waylay/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      272 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      498 2023-11-07 12:23:44.794172 waylay-beta-0.7.1/waylay/_version.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    16555 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/auth.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     7541 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/auth_interactive.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.687854 waylay-beta-0.7.1/waylay/cli/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       30 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       78 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/__main__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      680 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/_decorators.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     6014 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/configcli.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    18872 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/seriescli.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     3856 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/servicecli.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2251 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/cli/waylaycli.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     7653 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/client.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    13272 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/config.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2598 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/exceptions.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)        0 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/py.typed
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.690159 waylay-beta-0.7.1/waylay/service/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      617 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    17101 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/_base.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     9888 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/_decorators.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.691561 waylay-beta-0.7.1/waylay/service/analytics/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      554 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/analytics/__init__.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.703282 waylay-beta-0.7.1/waylay/service/byoml/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      176 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     6380 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/_decorators.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      784 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/_exceptions.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     8648 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/_model_archive.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      699 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      549 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/about.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     3753 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/framework.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    19669 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/model.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1937 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/byoml/runtime.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.706274 waylay-beta-0.7.1/waylay/service/data/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       76 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/data/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      517 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/data/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2528 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/data/events.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     5713 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/data/series.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.711111 waylay-beta-0.7.1/waylay/service/etl/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       86 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/etl/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      405 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/etl/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      956 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/etl/import_.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.730379 waylay-beta-0.7.1/waylay/service/queries/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      115 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     5337 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_decorators.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      907 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_exceptions.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      645 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_service.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.732269 waylay-beta-0.7.1/waylay/service/queries/_util/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      152 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_util/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    24251 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_util/df_parser.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    11006 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/_util/parse_util.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      540 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/about.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     9246 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/queries/query.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.734653 waylay-beta-0.7.1/waylay/service/resources/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       76 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/resources/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      586 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/resources/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     3622 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/resources/resource.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     3454 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/resources/resource_type.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.758471 waylay-beta-0.7.1/waylay/service/storage/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       94 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      906 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1096 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/about.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1554 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/bucket.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     7348 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/content.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     9415 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/object.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     4187 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/storage/subscription.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.766607 waylay-beta-0.7.1/waylay/service/timeseries/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      223 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      741 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/_service.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.769902 waylay-beta-0.7.1/waylay/service/timeseries/parser/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     5014 2023-11-06 12:19:44.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     8852 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/etlfile.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    16870 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/export_series.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    23753 2023-11-06 12:19:44.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/import_csv.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    12577 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/import_dataframe.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    31210 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/model.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      844 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/parser/util.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)    23767 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/timeseries/tool.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.770912 waylay-beta-0.7.1/waylay/service/util/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       81 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/util/__init__.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      644 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/util/_service.py
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     6160 2023-10-30 08:07:36.000000 waylay-beta-0.7.1/waylay/service/util/info.py
-drwxr-xr-x   0 claudiumuresan   (501) staff       (20)        0 2023-11-07 12:23:44.783278 waylay-beta-0.7.1/waylay_beta.egg-info/
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     6648 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/PKG-INFO
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     2532 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/SOURCES.txt
--rw-r--r--   0 claudiumuresan   (501) staff       (20)        1 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/dependency_links.txt
--rw-r--r--   0 claudiumuresan   (501) staff       (20)      106 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/entry_points.txt
--rw-r--r--   0 claudiumuresan   (501) staff       (20)     1181 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/requires.txt
--rw-r--r--   0 claudiumuresan   (501) staff       (20)       30 2023-11-07 12:23:44.000000 waylay-beta-0.7.1/waylay_beta.egg-info/top_level.txt
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-09 07:48:06.515569 waylay-beta-9.9.9b9/
+-rw-r--r--   0 thomas     (502) staff       (20)      746 2024-04-09 07:25:45.000000 waylay-beta-9.9.9b9/LICENSE.txt
+-rw-r--r--   0 thomas     (502) staff       (20)     1611 2024-04-09 07:48:06.515112 waylay-beta-9.9.9b9/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      349 2024-04-09 07:25:45.000000 waylay-beta-9.9.9b9/README.md
+-rw-r--r--   0 thomas     (502) staff       (20)      600 2024-04-09 07:25:45.000000 waylay-beta-9.9.9b9/pyproject.toml
+-rw-r--r--   0 thomas     (502) staff       (20)       38 2024-04-09 07:48:06.515627 waylay-beta-9.9.9b9/setup.cfg
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-09 07:48:06.509181 waylay-beta-9.9.9b9/waylay/
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-09 07:48:06.510827 waylay-beta-9.9.9b9/waylay/beta/
+-rw-r--r--   0 thomas     (502) staff       (20)       50 2024-04-09 07:25:45.000000 waylay-beta-9.9.9b9/waylay/beta/__init__.py
+drwxr-xr-x   0 thomas     (502) staff       (20)        0 2024-04-09 07:48:06.514780 waylay-beta-9.9.9b9/waylay_beta.egg-info/
+-rw-r--r--   0 thomas     (502) staff       (20)     1611 2024-04-09 07:48:06.000000 waylay-beta-9.9.9b9/waylay_beta.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (502) staff       (20)      234 2024-04-09 07:48:06.000000 waylay-beta-9.9.9b9/waylay_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        1 2024-04-09 07:48:06.000000 waylay-beta-9.9.9b9/waylay_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        7 2024-04-09 07:48:06.000000 waylay-beta-9.9.9b9/waylay_beta.egg-info/requires.txt
+-rw-r--r--   0 thomas     (502) staff       (20)        7 2024-04-09 07:48:06.000000 waylay-beta-9.9.9b9/waylay_beta.egg-info/top_level.txt
```

### Comparing `waylay-beta-0.7.1/LICENSE.txt` & `waylay-beta-9.9.9b9/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ISC License (ISC)
-Copyright 2020, Waylay
+Copyright 2024, Waylay
 
 Permission to use, copy, modify, and/or distribute this software for any purpose 
 with or without fee is hereby granted, provided that the above copyright notice 
 and this permission notice appear in all copies.
 
 THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
 REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
```

