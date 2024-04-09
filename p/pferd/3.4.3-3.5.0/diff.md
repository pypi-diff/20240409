# Comparing `tmp/pferd-3.4.3.tar.gz` & `tmp/pferd-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pferd-3.4.3.tar", last modified: Tue Nov 29 18:41:28 2022, max compression
+gzip compressed data, was "pferd-3.5.0.tar", last modified: Wed Sep 13 21:31:50 2023, max compression
```

## Comparing `pferd-3.4.3.tar` & `pferd-3.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.851197 pferd-3.4.3/
--rw-r--r--   0 pavel      (501) staff       (20)     1164 2022-11-29 18:41:25.000000 pferd-3.4.3/LICENSE
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.847262 pferd-3.4.3/PFERD/
--rw-r--r--   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     5338 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/__main__.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.848210 pferd-3.4.3/PFERD/auth/
--rw-r--r--   0 pavel      (501) staff       (20)     1170 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     2194 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/authenticator.py
--rw-r--r--   0 pavel      (501) staff       (20)     1649 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/credential_file.py
--rw-r--r--   0 pavel      (501) staff       (20)     2234 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/keyring.py
--rw-r--r--   0 pavel      (501) staff       (20)     3914 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/pass_.py
--rw-r--r--   0 pavel      (501) staff       (20)     2052 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/simple.py
--rw-r--r--   0 pavel      (501) staff       (20)      865 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/auth/tfa.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.848813 pferd-3.4.3/PFERD/cli/
--rw-r--r--   0 pavel      (501) staff       (20)      700 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/cli/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     3415 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/cli/command_kit_ilias_web.py
--rw-r--r--   0 pavel      (501) staff       (20)     1199 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/cli/command_kit_ipd.py
--rw-r--r--   0 pavel      (501) staff       (20)     1688 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/cli/command_local.py
--rw-r--r--   0 pavel      (501) staff       (20)     7068 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/cli/parser.py
--rw-r--r--   0 pavel      (501) staff       (20)     6161 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/config.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.849426 pferd-3.4.3/PFERD/crawl/
--rw-r--r--   0 pavel      (501) staff       (20)     1013 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)    12151 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     8191 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/http_crawler.py
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.850274 pferd-3.4.3/PFERD/crawl/ilias/
--rw-r--r--   0 pavel      (501) staff       (20)      144 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/ilias/__init__.py
--rw-r--r--   0 pavel      (501) staff       (20)     7164 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/ilias/file_templates.py
--rw-r--r--   0 pavel      (501) staff       (20)     2199 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/ilias/ilias_html_cleaner.py
--rw-r--r--   0 pavel      (501) staff       (20)    39664 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/ilias/kit_ilias_html.py
--rw-r--r--   0 pavel      (501) staff       (20)    39209 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/ilias/kit_ilias_web_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     5832 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/kit_ipd_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     3676 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/crawl/local_crawler.py
--rw-r--r--   0 pavel      (501) staff       (20)     2774 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/deduplicator.py
--rw-r--r--   0 pavel      (501) staff       (20)     2808 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/limiter.py
--rw-r--r--   0 pavel      (501) staff       (20)     8530 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/logging.py
--rw-r--r--   0 pavel      (501) staff       (20)    17789 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/output_dir.py
--rw-r--r--   0 pavel      (501) staff       (20)     7430 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/pferd.py
--rw-r--r--   0 pavel      (501) staff       (20)     7944 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/report.py
--rw-r--r--   0 pavel      (501) staff       (20)    11927 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/transformer.py
--rw-r--r--   0 pavel      (501) staff       (20)     3858 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/utils.py
--rw-r--r--   0 pavel      (501) staff       (20)       33 2022-11-29 18:41:25.000000 pferd-3.4.3/PFERD/version.py
--rw-r--r--   0 pavel      (501) staff       (20)     6399 2022-11-29 18:41:28.851262 pferd-3.4.3/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     4654 2022-11-29 18:41:25.000000 pferd-3.4.3/README.md
-drwxr-xr-x   0 pavel      (501) staff       (20)        0 2022-11-29 18:41:28.851089 pferd-3.4.3/pferd.egg-info/
--rw-r--r--   0 pavel      (501) staff       (20)     6399 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/PKG-INFO
--rw-r--r--   0 pavel      (501) staff       (20)     1045 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/SOURCES.txt
--rw-r--r--   0 pavel      (501) staff       (20)        1 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/dependency_links.txt
--rw-r--r--   0 pavel      (501) staff       (20)       46 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/entry_points.txt
--rw-r--r--   0 pavel      (501) staff       (20)       86 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/requires.txt
--rw-r--r--   0 pavel      (501) staff       (20)        6 2022-11-29 18:41:28.000000 pferd-3.4.3/pferd.egg-info/top_level.txt
--rw-r--r--   0 pavel      (501) staff       (20)      781 2022-11-29 18:41:25.000000 pferd-3.4.3/pyproject.toml
--rw-r--r--   0 pavel      (501) staff       (20)      395 2022-11-29 18:41:28.851979 pferd-3.4.3/setup.cfg
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.673466 pferd-3.5.0/
+-rw-r--r--   0 pavel      (501) staff       (20)     1193 2023-09-13 21:31:47.000000 pferd-3.5.0/LICENSE
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.669602 pferd-3.5.0/PFERD/
+-rw-r--r--   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     5556 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/__main__.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.670418 pferd-3.5.0/PFERD/auth/
+-rw-r--r--   0 pavel      (501) staff       (20)     1170 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2194 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/authenticator.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1649 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/credential_file.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2234 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/keyring.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3914 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/pass_.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2052 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/simple.py
+-rw-r--r--   0 pavel      (501) staff       (20)      865 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/auth/tfa.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.671013 pferd-3.5.0/PFERD/cli/
+-rw-r--r--   0 pavel      (501) staff       (20)      700 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/cli/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3415 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/cli/command_kit_ilias_web.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1199 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/cli/command_kit_ipd.py
+-rw-r--r--   0 pavel      (501) staff       (20)     1688 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/cli/command_local.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7363 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/cli/parser.py
+-rw-r--r--   0 pavel      (501) staff       (20)     6270 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/config.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.671697 pferd-3.5.0/PFERD/crawl/
+-rw-r--r--   0 pavel      (501) staff       (20)     1013 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)    12151 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     8191 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/http_crawler.py
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.672364 pferd-3.5.0/PFERD/crawl/ilias/
+-rw-r--r--   0 pavel      (501) staff       (20)      144 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/ilias/__init__.py
+-rw-r--r--   0 pavel      (501) staff       (20)     9052 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/ilias/file_templates.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2209 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/ilias/ilias_html_cleaner.py
+-rw-r--r--   0 pavel      (501) staff       (20)    47330 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/ilias/kit_ilias_html.py
+-rw-r--r--   0 pavel      (501) staff       (20)    47060 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/ilias/kit_ilias_web_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     5832 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/kit_ipd_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3676 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/crawl/local_crawler.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2816 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/deduplicator.py
+-rw-r--r--   0 pavel      (501) staff       (20)     2808 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/limiter.py
+-rw-r--r--   0 pavel      (501) staff       (20)     9320 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/logging.py
+-rw-r--r--   0 pavel      (501) staff       (20)    18050 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/output_dir.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7442 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/pferd.py
+-rw-r--r--   0 pavel      (501) staff       (20)     7944 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/report.py
+-rw-r--r--   0 pavel      (501) staff       (20)    11927 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/transformer.py
+-rw-r--r--   0 pavel      (501) staff       (20)     3858 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/utils.py
+-rw-r--r--   0 pavel      (501) staff       (20)       33 2023-09-13 21:31:47.000000 pferd-3.5.0/PFERD/version.py
+-rw-r--r--   0 pavel      (501) staff       (20)     6597 2023-09-13 21:31:50.673382 pferd-3.5.0/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     4654 2023-09-13 21:31:47.000000 pferd-3.5.0/README.md
+drwxr-xr-x   0 pavel      (501) staff       (20)        0 2023-09-13 21:31:50.673071 pferd-3.5.0/pferd.egg-info/
+-rw-r--r--   0 pavel      (501) staff       (20)     6597 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/PKG-INFO
+-rw-r--r--   0 pavel      (501) staff       (20)     1045 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/SOURCES.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        1 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/dependency_links.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       46 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/entry_points.txt
+-rw-r--r--   0 pavel      (501) staff       (20)       86 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/requires.txt
+-rw-r--r--   0 pavel      (501) staff       (20)        6 2023-09-13 21:31:50.000000 pferd-3.5.0/pferd.egg-info/top_level.txt
+-rw-r--r--   0 pavel      (501) staff       (20)      781 2023-09-13 21:31:47.000000 pferd-3.5.0/pyproject.toml
+-rw-r--r--   0 pavel      (501) staff       (20)      395 2023-09-13 21:31:50.673740 pferd-3.5.0/setup.cfg
```

### Comparing `pferd-3.4.3/LICENSE` & `pferd-3.5.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Copyright 2019-2021 Garmelon, I-Al-Istannen, danstooamerican, pavelzw,
-                    TheChristophe, Scriptim, thelukasprobst, Toorero
+                    TheChristophe, Scriptim, thelukasprobst, Toorero,
+                    Mr-Pine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `pferd-3.4.3/PFERD/__main__.py` & `pferd-3.5.0/PFERD/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 
 def configure_logging_from_args(args: argparse.Namespace) -> None:
     if args.explain is not None:
         log.output_explain = args.explain
     if args.status is not None:
         log.output_status = args.status
+    if args.show_not_deleted is not None:
+        log.output_not_deleted = args.show_not_deleted
     if args.report is not None:
         log.output_report = args.report
 
     # We want to prevent any unnecessary output if we're printing the config to
     # stdout, otherwise it would not be a valid config file.
     if args.dump_config_to == "-":
         log.output_explain = False
@@ -68,14 +70,16 @@
     try:
         if args.explain is None:
             log.output_explain = config.default_section.explain()
         if args.status is None:
             log.output_status = config.default_section.status()
         if args.report is None:
             log.output_report = config.default_section.report()
+        if args.show_not_deleted is None:
+            log.output_not_deleted = config.default_section.show_not_deleted()
     except ConfigOptionError as e:
         log.error(str(e))
         sys.exit(1)
 
 
 def dump_config(args: argparse.Namespace, config: Config) -> None:
     log.explain_topic("Dumping config")
```

### Comparing `pferd-3.4.3/PFERD/auth/__init__.py` & `pferd-3.5.0/PFERD/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/authenticator.py` & `pferd-3.5.0/PFERD/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/credential_file.py` & `pferd-3.5.0/PFERD/auth/credential_file.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/keyring.py` & `pferd-3.5.0/PFERD/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/pass_.py` & `pferd-3.5.0/PFERD/auth/pass_.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/simple.py` & `pferd-3.5.0/PFERD/auth/simple.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/auth/tfa.py` & `pferd-3.5.0/PFERD/auth/tfa.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/cli/__init__.py` & `pferd-3.5.0/PFERD/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/cli/command_kit_ilias_web.py` & `pferd-3.5.0/PFERD/cli/command_kit_ilias_web.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/cli/command_kit_ipd.py` & `pferd-3.5.0/PFERD/cli/command_kit_ipd.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/cli/command_local.py` & `pferd-3.5.0/PFERD/cli/command_local.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/cli/parser.py` & `pferd-3.5.0/PFERD/cli/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,14 +211,19 @@
     help="print a report of all local changes before exiting"
 )
 PARSER.add_argument(
     "--share-cookies",
     action=BooleanOptionalAction,
     help="whether crawlers should share cookies where applicable"
 )
+PARSER.add_argument(
+    "--show-not-deleted",
+    action=BooleanOptionalAction,
+    help="print messages in status and report when PFERD did not delete a local only file"
+)
 
 
 def load_default_section(
         args: argparse.Namespace,
         parser: configparser.ConfigParser,
 ) -> None:
     section = parser[parser.default_section]
@@ -229,10 +234,12 @@
         section["explain"] = "yes" if args.explain else "no"
     if args.status is not None:
         section["status"] = "yes" if args.status else "no"
     if args.report is not None:
         section["report"] = "yes" if args.report else "no"
     if args.share_cookies is not None:
         section["share_cookies"] = "yes" if args.share_cookies else "no"
+    if args.show_not_deleted is not None:
+        section["show_not_deleted"] = "yes" if args.show_not_deleted else "no"
 
 
 SUBPARSERS = PARSER.add_subparsers(title="crawlers")
```

### Comparing `pferd-3.4.3/PFERD/config.py` & `pferd-3.5.0/PFERD/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 
     def status(self) -> bool:
         return self.s.getboolean("status", fallback=True)
 
     def report(self) -> bool:
         return self.s.getboolean("report", fallback=True)
 
+    def show_not_deleted(self) -> bool:
+        return self.s.getboolean("show_not_deleted", fallback=True)
+
     def share_cookies(self) -> bool:
         return self.s.getboolean("share_cookies", fallback=True)
 
 
 class Config:
     @staticmethod
     def _default_path() -> Path:
```

### Comparing `pferd-3.4.3/PFERD/crawl/__init__.py` & `pferd-3.5.0/PFERD/crawl/__init__.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/crawl/crawler.py` & `pferd-3.5.0/PFERD/crawl/crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/crawl/http_crawler.py` & `pferd-3.5.0/PFERD/crawl/http_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/crawl/ilias/file_templates.py` & `pferd-3.5.0/PFERD/crawl/ilias/file_templates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from enum import Enum
 from typing import Optional
 
+import bs4
+
+from PFERD.utils import soupify
+
 _link_template_plain = "{{link}}"
 _link_template_fancy = """
 <!DOCTYPE html>
 <html lang="en">
     <head>
         <meta charset="UTF-8">
         <title>ILIAS - Link: {{name}}</title>
@@ -90,40 +94,105 @@
 """.strip()  # noqa: E501 line too long
 
 _link_template_internet_shortcut = """
 [InternetShortcut]
 URL={{link}}
 """.strip()
 
+_learning_module_template = """
+<!DOCTYPE html>
+<html lang="en">
+    <head>
+        <meta charset="UTF-8">
+        <title>{{name}}</title>
+    </head>
+
+    <style>
+    * {
+        box-sizing: border-box;
+    }
+    .center-flex {
+        display: flex;
+        align-items: center;
+        justify-content: center;
+    }
+    .nav {
+        display: flex;
+        justify-content: space-between;
+    }
+    </style>
+    <body class="center-flex">
+{{body}}
+    </body>
+</html>
+"""
+
+
+def learning_module_template(body: bs4.Tag, name: str, prev: Optional[str], next: Optional[str]) -> str:
+    # Seems to be comments, ignore those.
+    for elem in body.select(".il-copg-mob-fullscreen-modal"):
+        elem.decompose()
+
+    nav_template = """
+        <div class="nav">
+            {{left}}
+            {{right}}
+        </div>
+    """
+    if prev and body.select_one(".ilc_page_lnav_LeftNavigation"):
+        text = body.select_one(".ilc_page_lnav_LeftNavigation").getText().strip()
+        left = f'<a href="{prev}">{text}</a>'
+    else:
+        left = "<span></span>"
+
+    if next and body.select_one(".ilc_page_rnav_RightNavigation"):
+        text = body.select_one(".ilc_page_rnav_RightNavigation").getText().strip()
+        right = f'<a href="{next}">{text}</a>'
+    else:
+        right = "<span></span>"
+
+    if top_nav := body.select_one(".ilc_page_tnav_TopNavigation"):
+        top_nav.replace_with(
+            soupify(nav_template.replace("{{left}}", left).replace("{{right}}", right).encode())
+        )
+
+    if bot_nav := body.select_one(".ilc_page_bnav_BottomNavigation"):
+        bot_nav.replace_with(soupify(nav_template.replace(
+            "{{left}}", left).replace("{{right}}", right).encode())
+        )
+
+    body = body.prettify()
+    return _learning_module_template.replace("{{body}}", body).replace("{{name}}", name)
+
 
 class Links(Enum):
     IGNORE = "ignore"
     PLAINTEXT = "plaintext"
     FANCY = "fancy"
     INTERNET_SHORTCUT = "internet-shortcut"
 
     def template(self) -> Optional[str]:
-        if self == self.FANCY:
+        if self == Links.FANCY:
             return _link_template_fancy
-        elif self == self.PLAINTEXT:
+        elif self == Links.PLAINTEXT:
             return _link_template_plain
-        elif self == self.INTERNET_SHORTCUT:
+        elif self == Links.INTERNET_SHORTCUT:
             return _link_template_internet_shortcut
-        elif self == self.IGNORE:
+        elif self == Links.IGNORE:
             return None
         raise ValueError("Missing switch case")
 
     def extension(self) -> Optional[str]:
-        if self == self.FANCY:
+        if self == Links.FANCY:
             return ".html"
-        elif self == self.PLAINTEXT:
+        elif self == Links.PLAINTEXT:
             return ".txt"
-        elif self == self.INTERNET_SHORTCUT:
+        elif self == Links.INTERNET_SHORTCUT:
             return ".url"
-        elif self == self.IGNORE:
+        elif self == Links.IGNORE:
             return None
         raise ValueError("Missing switch case")
 
     @staticmethod
     def from_string(string: str) -> "Links":
         try:
             return Links(string)
```

### Comparing `pferd-3.4.3/PFERD/crawl/ilias/ilias_html_cleaner.py` & `pferd-3.5.0/PFERD/crawl/ilias/ilias_html_cleaner.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,14 @@
 
     for dummy in soup.select(".ilc_text_block_Standard.ilc_Paragraph"):
         children = list(dummy.children)
         if not children:
             dummy.decompose()
         if len(children) > 1:
             continue
-        if type(children[0]) == Comment:
+        if isinstance(type(children[0]), Comment):
             dummy.decompose()
 
     for hrule_imposter in soup.find_all(class_="ilc_section_Separator"):
         hrule_imposter.insert(0, soup.new_tag("hr"))
 
     return soup
```

### Comparing `pferd-3.4.3/PFERD/crawl/ilias/kit_ilias_html.py` & `pferd-3.5.0/PFERD/crawl/ilias/kit_ilias_html.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import re
 from dataclasses import dataclass
 from datetime import date, datetime, timedelta
 from enum import Enum
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union, cast
 from urllib.parse import urljoin, urlparse
 
 from bs4 import BeautifulSoup, Tag
 
 from PFERD.logging import log
 from PFERD.utils import url_set_query_params
 
@@ -18,21 +18,26 @@
     EXERCISE = "exercise"
     EXERCISE_FILES = "exercise_files"  # own submitted files
     TEST = "test"                      # an online test. Will be ignored currently.
     FILE = "file"
     FOLDER = "folder"
     FORUM = "forum"
     LINK = "link"
+    INFO_TAB = "info_tab"
+    LEARNING_MODULE = "learning_module"
     BOOKING = "booking"
     MEETING = "meeting"
     SURVEY = "survey"
-    VIDEO = "video"
-    VIDEO_PLAYER = "video_player"
-    VIDEO_FOLDER = "video_folder"
-    VIDEO_FOLDER_MAYBE_PAGINATED = "video_folder_maybe_paginated"
+    SCORM_LEARNING_MODULE = "scorm_learning_module"
+    MEDIACAST_VIDEO_FOLDER = "mediacast_video_folder"
+    MEDIACAST_VIDEO = "mediacast_video"
+    OPENCAST_VIDEO = "opencast_video"
+    OPENCAST_VIDEO_PLAYER = "opencast_video_player"
+    OPENCAST_VIDEO_FOLDER = "opencast_video_folder"
+    OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED = "opencast_video_folder_maybe_paginated"
 
 
 @dataclass
 class IliasPageElement:
     type: IliasElementType
     url: str
     name: str
@@ -40,15 +45,16 @@
     description: Optional[str] = None
 
     def id(self) -> str:
         regexes = [
             r"eid=(?P<id>[0-9a-z\-]+)",
             r"file_(?P<id>\d+)",
             r"ref_id=(?P<id>\d+)",
-            r"target=[a-z]+_(?P<id>\d+)"
+            r"target=[a-z]+_(?P<id>\d+)",
+            r"mm_(?P<id>\d+)"
         ]
 
         for regex in regexes:
             if match := re.search(regex, self.url):
                 return match.groupdict()["id"]
 
         # Fall back to URL
@@ -67,44 +73,78 @@
 class IliasForumThread:
     title: str
     title_tag: Tag
     content_tag: Tag
     mtime: Optional[datetime]
 
 
+@dataclass
+class IliasLearningModulePage:
+    title: str
+    content: Tag
+    next_url: Optional[str]
+    previous_url: Optional[str]
+
+
 class IliasPage:
 
     def __init__(self, soup: BeautifulSoup, _page_url: str, source_element: Optional[IliasPageElement]):
         self._soup = soup
         self._page_url = _page_url
         self._page_type = source_element.type if source_element else None
         self._source_name = source_element.name if source_element else ""
 
+    @staticmethod
+    def is_root_page(soup: BeautifulSoup) -> bool:
+        permalink = soup.find(id="current_perma_link")
+        if permalink is None:
+            return False
+        value = permalink.attrs.get("value")
+        if value is None:
+            return False
+        return "goto.php?target=root_" in value
+
     def get_child_elements(self) -> List[IliasPageElement]:
         """
         Return all child page elements you can find here.
         """
         if self._is_video_player():
             log.explain("Page is a video player, extracting URL")
             return self._player_to_video()
-        if self._is_video_listing():
-            log.explain("Page is a video listing, searching for elements")
-            return self._find_video_entries()
+        if self._is_opencast_video_listing():
+            log.explain("Page is an opencast video listing, searching for elements")
+            return self._find_opencast_video_entries()
         if self._is_exercise_file():
             log.explain("Page is an exercise, searching for elements")
             return self._find_exercise_entries()
         if self._is_personal_desktop():
             log.explain("Page is the personal desktop, searching for elements")
             return self._find_personal_desktop_entries()
         if self._is_content_page():
             log.explain("Page is a content page, searching for elements")
             return self._find_copa_entries()
+        if self._is_info_tab():
+            log.explain("Page is info tab, searching for elements")
+            return self._find_info_tab_entries()
         log.explain("Page is a normal folder, searching for elements")
         return self._find_normal_entries()
 
+    def get_info_tab(self) -> Optional[IliasPageElement]:
+        tab: Optional[Tag] = self._soup.find(
+            name="a",
+            attrs={"href": lambda x: x and "cmdClass=ilinfoscreengui" in x}
+        )
+        if tab is not None:
+            return IliasPageElement(
+                IliasElementType.INFO_TAB,
+                self._abs_url_from_link(tab),
+                "infos"
+            )
+        return None
+
     def get_description(self) -> Optional[BeautifulSoup]:
         def is_interesting_class(name: str) -> bool:
             return name in ["ilCOPageSection", "ilc_Paragraph", "ilc_va_ihcap_VAccordIHeadCap"]
 
         paragraphs: List[Tag] = self._soup.findAll(class_=is_interesting_class)
         if not paragraphs:
             return None
@@ -122,14 +162,42 @@
                 continue
 
             raw_html += str(p) + "\n"
         raw_html = f"<body>\n{raw_html}\n</body>"
 
         return BeautifulSoup(raw_html, "html.parser")
 
+    def get_learning_module_data(self) -> Optional[IliasLearningModulePage]:
+        if not self._is_learning_module_page():
+            return None
+        content = self._soup.select_one("#ilLMPageContent")
+        title = self._soup.select_one(".ilc_page_title_PageTitle").getText().strip()
+        return IliasLearningModulePage(
+            title=title,
+            content=content,
+            next_url=self._find_learning_module_next(),
+            previous_url=self._find_learning_module_prev()
+        )
+
+    def _find_learning_module_next(self) -> Optional[str]:
+        for link in self._soup.select("a.ilc_page_rnavlink_RightNavigationLink"):
+            url = self._abs_url_from_link(link)
+            if "baseClass=ilLMPresentationGUI" not in url:
+                continue
+            return url
+        return None
+
+    def _find_learning_module_prev(self) -> Optional[str]:
+        for link in self._soup.select("a.ilc_page_lnavlink_LeftNavigationLink"):
+            url = self._abs_url_from_link(link)
+            if "baseClass=ilLMPresentationGUI" not in url:
+                continue
+            return url
+        return None
+
     def get_download_forum_data(self) -> Optional[IliasDownloadForumData]:
         form = self._soup.find("form", attrs={"action": lambda x: x and "fallbackCmd=showThreads" in x})
         if not form:
             return None
         post_url = self._abs_url_from_relative(form["action"])
 
         thread_ids = [f["value"] for f in form.find_all(attrs={"name": "thread_ids[]"})]
@@ -148,33 +216,39 @@
             if "trows=800" in self._page_url:
                 return None
             log.explain("Requesting *all* forum threads")
             return self._get_show_max_forum_entries_per_page_url()
         if self._is_ilias_opencast_embedding():
             log.explain("Unwrapping opencast embedding")
             return self.get_child_elements()[0]
-        if self._page_type == IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED:
+        if self._page_type == IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED:
             log.explain("Unwrapping video pagination")
-            return self._find_video_entries_paginated()[0]
+            return self._find_opencast_video_entries_paginated()[0]
         if self._contains_collapsed_future_meetings():
             log.explain("Requesting *all* future meetings")
             return self._uncollapse_future_meetings_url()
+        if not self._is_content_tab_selected():
+            if self._page_type != IliasElementType.INFO_TAB:
+                log.explain("Selecting content tab")
+                return self._select_content_page_url()
+            else:
+                log.explain("Crawling info tab, skipping content select")
         return None
 
     def _is_forum_page(self) -> bool:
         read_more_btn = self._soup.find(
             "button",
             attrs={"onclick": lambda x: x and "cmdClass=ilobjforumgui&cmd=markAllRead" in x}
         )
         return read_more_btn is not None
 
     def _is_video_player(self) -> bool:
         return "paella_config_file" in str(self._soup)
 
-    def _is_video_listing(self) -> bool:
+    def _is_opencast_video_listing(self) -> bool:
         if self._is_ilias_opencast_embedding():
             return True
 
         # Raw listing without ILIAS fluff
         video_element_table: Tag = self._soup.find(
             name="table", id=re.compile(r"tbl_xoct_.+")
         )
@@ -206,24 +280,58 @@
 
     def _is_content_page(self) -> bool:
         link = self._soup.find(id="current_perma_link")
         if not link:
             return False
         return "target=copa_" in link.get("value")
 
+    def _is_learning_module_page(self) -> bool:
+        link = self._soup.find(id="current_perma_link")
+        if not link:
+            return False
+        return "target=pg_" in link.get("value")
+
     def _contains_collapsed_future_meetings(self) -> bool:
         return self._uncollapse_future_meetings_url() is not None
 
     def _uncollapse_future_meetings_url(self) -> Optional[IliasPageElement]:
-        element = self._soup.find("a", attrs={"href": lambda x: x and "crs_next_sess=1" in x})
+        element = self._soup.find(
+            "a",
+            attrs={"href": lambda x: x and ("crs_next_sess=1" in x or "crs_prev_sess=1" in x)}
+        )
         if not element:
             return None
         link = self._abs_url_from_link(element)
         return IliasPageElement(IliasElementType.FOLDER, link, "show all meetings")
 
+    def _is_content_tab_selected(self) -> bool:
+        return self._select_content_page_url() is None
+
+    def _is_info_tab(self) -> bool:
+        might_be_info = self._soup.find("form", attrs={"name": lambda x: x == "formInfoScreen"}) is not None
+        return self._page_type == IliasElementType.INFO_TAB and might_be_info
+
+    def _select_content_page_url(self) -> Optional[IliasPageElement]:
+        tab = self._soup.find(
+            id="tab_view_content",
+            attrs={"class": lambda x: x is not None and "active" not in x}
+        )
+        # Already selected (or not found)
+        if not tab:
+            return None
+        link = tab.find("a")
+        if link:
+            link = self._abs_url_from_link(link)
+            return IliasPageElement(IliasElementType.FOLDER, link, "select content page")
+
+        _unexpected_html_warning()
+        log.warn_contd(f"Could not find content tab URL on {self._page_url!r}.")
+        log.warn_contd("PFERD might not find content on the course's main page.")
+        return None
+
     def _player_to_video(self) -> List[IliasPageElement]:
         # Fetch the actual video page. This is a small wrapper page initializing a javscript
         # player. Sadly we can not execute that JS. The actual video stream url is nowhere
         # on the page, but defined in a JS object inside a script tag, passed to the player
         # library.
         # We do the impossible and RegEx the stream JSON object out of the page's HTML source
         regex = re.compile(
@@ -239,22 +347,22 @@
         # parse it
         json_object = json.loads(json_str)
         streams = [stream for stream in json_object["streams"]]
 
         # and just fetch the lone video url!
         if len(streams) == 1:
             video_url = streams[0]["sources"]["mp4"][0]["src"]
-            return [IliasPageElement(IliasElementType.VIDEO, video_url, self._source_name)]
+            return [IliasPageElement(IliasElementType.OPENCAST_VIDEO, video_url, self._source_name)]
 
         log.explain(f"Found multiple videos for stream at {self._source_name}")
         items = []
         for stream in sorted(streams, key=lambda stream: stream["content"]):
             full_name = f"{self._source_name.replace('.mp4', '')} ({stream['content']}).mp4"
             video_url = stream["sources"]["mp4"][0]["src"]
-            items.append(IliasPageElement(IliasElementType.VIDEO, video_url, full_name))
+            items.append(IliasPageElement(IliasElementType.OPENCAST_VIDEO, video_url, full_name))
 
         return items
 
     def _get_show_max_forum_entries_per_page_url(self) -> Optional[IliasPageElement]:
         correct_link = self._soup.find(
             "a",
             attrs={"href": lambda x: x and "trows=800" in x and "cmd=showThreads" in x}
@@ -294,26 +402,44 @@
 
     def _find_copa_entries(self) -> List[IliasPageElement]:
         items: List[IliasPageElement] = []
         links: List[Tag] = self._soup.findAll(class_="ilc_flist_a_FileListItemLink")
 
         for link in links:
             url = self._abs_url_from_link(link)
-            name = _sanitize_path_name(link.getText().strip().replace("\t", ""))
+            name = re.sub(r"\([\d,.]+ [MK]B\)", "", link.getText()).strip().replace("\t", "")
+            name = _sanitize_path_name(name)
 
             if "file_id" not in url:
                 _unexpected_html_warning()
                 log.warn_contd(f"Found unknown content page item {name!r} with url {url!r}")
                 continue
 
             items.append(IliasPageElement(IliasElementType.FILE, url, name))
 
         return items
 
-    def _find_video_entries(self) -> List[IliasPageElement]:
+    def _find_info_tab_entries(self) -> List[IliasPageElement]:
+        items = []
+        links: List[Tag] = self._soup.select("a.il_ContainerItemCommand")
+
+        for link in links:
+            if "cmdClass=ilobjcoursegui" not in link["href"]:
+                continue
+            if "cmd=sendfile" not in link["href"]:
+                continue
+            items.append(IliasPageElement(
+                IliasElementType.FILE,
+                self._abs_url_from_link(link),
+                _sanitize_path_name(link.getText())
+            ))
+
+        return items
+
+    def _find_opencast_video_entries(self) -> List[IliasPageElement]:
         # ILIAS has three stages for video pages
         # 1. The initial dummy page without any videos. This page contains the link to the listing
         # 2. The video listing which might be paginated
         # 3. An unpaginated video listing (or at least one that includes 800 videos)
         #
         # We need to figure out where we are.
 
@@ -325,62 +451,62 @@
             # We are in stage 1
             # The page is actually emtpy but contains the link to stage 2
             content_link: Tag = self._soup.select_one("#tab_series a")
             url: str = self._abs_url_from_link(content_link)
             query_params = {"limit": "800", "cmd": "asyncGetTableGUI", "cmdMode": "asynch"}
             url = url_set_query_params(url, query_params)
             log.explain("Found ILIAS video frame page, fetching actual content next")
-            return [IliasPageElement(IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED, url, "")]
+            return [IliasPageElement(IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED, url, "")]
 
         is_paginated = self._soup.find(id=re.compile(r"tab_page_sel.+")) is not None
 
-        if is_paginated and not self._page_type == IliasElementType.VIDEO_FOLDER:
+        if is_paginated and not self._page_type == IliasElementType.OPENCAST_VIDEO_FOLDER:
             # We are in stage 2 - try to break pagination
-            return self._find_video_entries_paginated()
+            return self._find_opencast_video_entries_paginated()
 
-        return self._find_video_entries_no_paging()
+        return self._find_opencast_video_entries_no_paging()
 
-    def _find_video_entries_paginated(self) -> List[IliasPageElement]:
+    def _find_opencast_video_entries_paginated(self) -> List[IliasPageElement]:
         table_element: Tag = self._soup.find(name="table", id=re.compile(r"tbl_xoct_.+"))
 
         if table_element is None:
             log.warn("Couldn't increase elements per page (table not found). I might miss elements.")
-            return self._find_video_entries_no_paging()
+            return self._find_opencast_video_entries_no_paging()
 
         id_match = re.match(r"tbl_xoct_(.+)", table_element.attrs["id"])
         if id_match is None:
             log.warn("Couldn't increase elements per page (table id not found). I might miss elements.")
-            return self._find_video_entries_no_paging()
+            return self._find_opencast_video_entries_no_paging()
 
         table_id = id_match.group(1)
 
         query_params = {f"tbl_xoct_{table_id}_trows": "800",
                         "cmd": "asyncGetTableGUI", "cmdMode": "asynch"}
         url = url_set_query_params(self._page_url, query_params)
 
         log.explain("Disabled pagination, retrying folder as a new entry")
-        return [IliasPageElement(IliasElementType.VIDEO_FOLDER, url, "")]
+        return [IliasPageElement(IliasElementType.OPENCAST_VIDEO_FOLDER, url, "")]
 
-    def _find_video_entries_no_paging(self) -> List[IliasPageElement]:
+    def _find_opencast_video_entries_no_paging(self) -> List[IliasPageElement]:
         """
         Crawls the "second stage" video page. This page contains the actual video urls.
         """
         # Video start links are marked with an "Abspielen" link
         video_links: List[Tag] = self._soup.findAll(
             name="a", text=re.compile(r"\s*(Abspielen|Play)\s*")
         )
 
         results: List[IliasPageElement] = []
 
         for link in video_links:
-            results.append(self._listed_video_to_element(link))
+            results.append(self._listed_opencast_video_to_element(link))
 
         return results
 
-    def _listed_video_to_element(self, link: Tag) -> IliasPageElement:
+    def _listed_opencast_video_to_element(self, link: Tag) -> IliasPageElement:
         # The link is part of a table with multiple columns, describing metadata.
         # 6th or 7th child (1 indexed) is the modification time string. Try to find it
         # by parsing backwards from the end and finding something that looks like a date
         modification_time = None
         row: Tag = link.parent.parent.parent
         column_count = len(row.select("td.std"))
         for index in range(column_count, 0, -1):
@@ -399,15 +525,17 @@
         title += ".mp4"
 
         video_name: str = _sanitize_path_name(title)
 
         video_url = self._abs_url_from_link(link)
 
         log.explain(f"Found video {video_name!r} at {video_url}")
-        return IliasPageElement(IliasElementType.VIDEO_PLAYER, video_url, video_name, modification_time)
+        return IliasPageElement(
+            IliasElementType.OPENCAST_VIDEO_PLAYER, video_url, video_name, modification_time
+        )
 
     def _find_exercise_entries(self) -> List[IliasPageElement]:
         if self._soup.find(id="tab_submission"):
             log.explain("Found submission tab. This is an exercise detail page")
             return self._find_exercise_entries_detail_page()
         log.explain("Found no submission tab. This is an exercise root page")
         return self._find_exercise_entries_root_page()
@@ -542,17 +670,56 @@
                 result.append(self._file_to_element(element_name, abs_url, link))
                 continue
 
             log.explain(f"Found {element_name!r}")
             result.append(IliasPageElement(element_type, abs_url, element_name, description=description))
 
         result += self._find_cards()
+        result += self._find_mediacast_videos()
 
         return result
 
+    def _find_mediacast_videos(self) -> List[IliasPageElement]:
+        videos: List[IliasPageElement] = []
+
+        for elem in cast(List[Tag], self._soup.select(".ilPlayerPreviewOverlayOuter")):
+            element_name = _sanitize_path_name(
+                elem.select_one(".ilPlayerPreviewDescription").getText().strip()
+            )
+            if not element_name.endswith(".mp4"):
+                # just to make sure it has some kinda-alrightish ending
+                element_name = element_name + ".mp4"
+            video_element = elem.find(name="video")
+            if not video_element:
+                _unexpected_html_warning()
+                log.warn_contd(f"No <video> element found for mediacast video '{element_name}'")
+                continue
+
+            videos.append(IliasPageElement(
+                type=IliasElementType.MEDIACAST_VIDEO,
+                url=self._abs_url_from_relative(video_element.get("src")),
+                name=element_name,
+                mtime=self._find_mediacast_video_mtime(elem.findParent(name="td"))
+            ))
+
+        return videos
+
+    def _find_mediacast_video_mtime(self, enclosing_td: Tag) -> Optional[datetime]:
+        description_td: Tag = enclosing_td.findPreviousSibling("td")
+        if not description_td:
+            return None
+
+        meta_tag: Tag = description_td.find_all("p")[-1]
+        if not meta_tag:
+            return None
+
+        updated_str = meta_tag.getText().strip().replace("\n", " ")
+        updated_str = re.sub(".+?: ", "", updated_str)
+        return demangle_date(updated_str)
+
     def _is_in_expanded_meeting(self, tag: Tag) -> bool:
         """
         Returns whether a file is part of an expanded meeting.
         Has false positives for meetings themselves as their title is also "in the expanded meeting content".
         It is in the same general div and this whole thing is guesswork.
         Therefore, you should check for meetings before passing them in this function.
         """
@@ -681,15 +848,19 @@
             url = self._abs_url_from_relative(res.group(1))
             name = _sanitize_path_name(button.getText().strip())
             type = self._find_type_from_card(button)
             caption_parent = button.findParent(
                 "div",
                 attrs={"class": lambda x: x and "caption" in x},
             )
-            description = caption_parent.find_next_sibling("div").getText().strip()
+            caption_container = caption_parent.find_next_sibling("div")
+            if caption_container:
+                description = caption_container.getText().strip()
+            else:
+                description = None
 
             if not type:
                 _unexpected_html_warning()
                 log.warn_contd(f"Could not extract type for {button}")
                 continue
 
             result.append(IliasPageElement(type, url, name, description=description))
@@ -711,16 +882,16 @@
         if card_root is None:
             _unexpected_html_warning()
             log.warn_contd(f"Tried to figure out element type, but did not find an icon for {card_title}")
             return None
 
         icon: Tag = card_root.select_one(".il-card-repository-head .icon")
 
-        if "opencast" in icon["class"]:
-            return IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED
+        if "opencast" in icon["class"] or "xoct" in icon["class"]:
+            return IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED
         if "exc" in icon["class"]:
             return IliasElementType.EXERCISE
         if "webr" in icon["class"]:
             return IliasElementType.LINK
         if "book" in icon["class"]:
             return IliasElementType.BOOKING
         if "frm" in icon["class"]:
@@ -731,14 +902,18 @@
             return IliasElementType.TEST
         if "fold" in icon["class"]:
             return IliasElementType.FOLDER
         if "copa" in icon["class"]:
             return IliasElementType.FOLDER
         if "svy" in icon["class"]:
             return IliasElementType.SURVEY
+        if "file" in icon["class"]:
+            return IliasElementType.FILE
+        if "mcst" in icon["class"]:
+            return IliasElementType.MEDIACAST_VIDEO_FOLDER
 
         _unexpected_html_warning()
         log.warn_contd(f"Could not extract type from {icon} for card title {card_title}")
         return None
 
     @staticmethod
     def _find_type_from_link(
@@ -769,14 +944,23 @@
 
         if "cmd=showThreads" in parsed_url.query or "target=frm_" in parsed_url.query:
             return IliasElementType.FORUM
 
         if "cmdClass=ilobjtestgui" in parsed_url.query:
             return IliasElementType.TEST
 
+        if "baseClass=ilLMPresentationGUI" in parsed_url.query:
+            return IliasElementType.LEARNING_MODULE
+
+        if "baseClass=ilMediaCastHandlerGUI" in parsed_url.query:
+            return IliasElementType.MEDIACAST_VIDEO_FOLDER
+
+        if "baseClass=ilSAHSPresentationGUI" in parsed_url.query:
+            return IliasElementType.SCORM_LEARNING_MODULE
+
         # Booking and Meeting can not be detected based on the link. They do have a ref_id though, so
         # try to guess it from the image.
 
         # Everything with a ref_id can *probably* be opened to reveal nested things
         # video groups, directories, exercises, etc
         if "ref_id=" in parsed_url.query or "goto.php" in parsed_url.path:
             return IliasPage._find_type_from_folder_like(link_element, url)
@@ -810,25 +994,29 @@
 
         # Find the small descriptive icon to figure out the type
         img_tag: Optional[Tag] = found_parent.select_one("img.ilListItemIcon")
 
         if img_tag is None:
             img_tag = found_parent.select_one("img.icon")
 
-        if img_tag is None and found_parent.find("a", attrs={"href": lambda x: x and "crs_next_sess=" in x}):
+        is_session_expansion_button = found_parent.find(
+            "a",
+            attrs={"href": lambda x: x and ("crs_next_sess=" in x or "crs_prev_sess=" in x)}
+        )
+        if img_tag is None and is_session_expansion_button:
             log.explain("Found session expansion button, skipping it as it has no content")
             return None
 
         if img_tag is None:
             _unexpected_html_warning()
             log.warn_contd(f"Tried to figure out element type, but did not find an image for {url}")
             return None
 
         if "opencast" in str(img_tag["alt"]).lower():
-            return IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED
+            return IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED
 
         if str(img_tag["src"]).endswith("icon_exc.svg"):
             return IliasElementType.EXERCISE
 
         if str(img_tag["src"]).endswith("icon_webr.svg"):
             return IliasElementType.LINK
 
@@ -840,14 +1028,20 @@
 
         if str(img_tag["src"]).endswith("sess.svg"):
             return IliasElementType.MEETING
 
         if str(img_tag["src"]).endswith("icon_tst.svg"):
             return IliasElementType.TEST
 
+        if str(img_tag["src"]).endswith("icon_mcst.svg"):
+            return IliasElementType.MEDIACAST_VIDEO_FOLDER
+
+        if str(img_tag["src"]).endswith("icon_sahs.svg"):
+            return IliasElementType.SCORM_LEARNING_MODULE
+
         return IliasElementType.FOLDER
 
     @staticmethod
     def _normalize_meeting_name(meeting_name: str) -> str:
         """
         Normalizes meeting names, which have a relative time as their first part,
         to their date in ISO format.
```

### Comparing `pferd-3.4.3/PFERD/crawl/ilias/kit_ilias_web_crawler.py` & `pferd-3.5.0/PFERD/crawl/ilias/kit_ilias_web_crawler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import asyncio
+import base64
+import os
 import re
 from collections.abc import Awaitable, Coroutine
 from pathlib import PurePath
-from typing import Any, Callable, Dict, List, Optional, Set, Union, cast
+from typing import Any, Callable, Dict, List, Literal, Optional, Set, Union, cast
+from urllib.parse import urljoin
 
 import aiohttp
 import yarl
 from aiohttp import hdrs
 from bs4 import BeautifulSoup, Tag
 
 from ...auth import Authenticator, TfaAuthenticator
 from ...config import Config
 from ...logging import ProgressBar, log
 from ...output_dir import FileSink, Redownload
 from ...utils import fmt_path, soupify, url_set_query_param
 from ..crawler import AWrapped, CrawlError, CrawlToken, CrawlWarning, DownloadToken, anoncritical
 from ..http_crawler import HttpCrawler, HttpCrawlerSection
-from .file_templates import Links
+from .file_templates import Links, learning_module_template
 from .ilias_html_cleaner import clean, insert_base_markup
-from .kit_ilias_html import (IliasElementType, IliasForumThread, IliasPage, IliasPageElement,
-                             _sanitize_path_name, parse_ilias_forum_export)
+from .kit_ilias_html import (IliasElementType, IliasForumThread, IliasLearningModulePage, IliasPage,
+                             IliasPageElement, _sanitize_path_name, parse_ilias_forum_export)
 
 TargetType = Union[str, int]
 
 _ILIAS_URL = "https://ilias.studium.kit.edu"
 
 
 class KitShibbolethBackgroundLoginSuccessful():
@@ -78,24 +81,28 @@
         return self.s.getboolean("forums", fallback=False)
 
 
 _DIRECTORY_PAGES: Set[IliasElementType] = set([
     IliasElementType.EXERCISE,
     IliasElementType.EXERCISE_FILES,
     IliasElementType.FOLDER,
+    IliasElementType.INFO_TAB,
     IliasElementType.MEETING,
-    IliasElementType.VIDEO_FOLDER,
-    IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED,
+    IliasElementType.MEDIACAST_VIDEO_FOLDER,
+    IliasElementType.OPENCAST_VIDEO_FOLDER,
+    IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED,
 ])
 
 _VIDEO_ELEMENTS: Set[IliasElementType] = set([
-    IliasElementType.VIDEO,
-    IliasElementType.VIDEO_PLAYER,
-    IliasElementType.VIDEO_FOLDER,
-    IliasElementType.VIDEO_FOLDER_MAYBE_PAGINATED,
+    IliasElementType.MEDIACAST_VIDEO_FOLDER,
+    IliasElementType.MEDIACAST_VIDEO,
+    IliasElementType.OPENCAST_VIDEO,
+    IliasElementType.OPENCAST_VIDEO_PLAYER,
+    IliasElementType.OPENCAST_VIDEO_FOLDER,
+    IliasElementType.OPENCAST_VIDEO_FOLDER_MAYBE_PAGINATED,
 ])
 
 
 def _iorepeat(attempts: int, name: str, failure_is_error: bool = False) -> Callable[[AWrapped], AWrapped]:
     def decorator(f: AWrapped) -> AWrapped:
         async def wrapper(*args: Any, **kwargs: Any) -> Optional[Any]:
             last_exception: Optional[BaseException] = None
@@ -235,15 +242,15 @@
             elements.clear()
             async with cl:
                 next_stage_url: Optional[str] = url
                 current_parent = None
 
                 # Duplicated code, but the root page is special - we want to avoid fetching it twice!
                 while next_stage_url:
-                    soup = await self._get_page(next_stage_url)
+                    soup = await self._get_page(next_stage_url, root_page_allowed=True)
 
                     if current_parent is None and expected_id is not None:
                         perma_link_element: Tag = soup.find(id="current_perma_link")
                         if not perma_link_element or "crs_" not in perma_link_element.get("value"):
                             raise CrawlError("Invalid course id? Didn't find anything looking like a course")
 
                     log.explain_topic(f"Parsing HTML page for {fmt_path(cl.path)}")
@@ -252,14 +259,16 @@
                     if next_element := page.get_next_stage_element():
                         current_parent = next_element
                         next_stage_url = next_element.url
                     else:
                         next_stage_url = None
 
                 elements.extend(page.get_child_elements())
+                if info_tab := page.get_info_tab():
+                    elements.append(info_tab)
                 if description_string := page.get_description():
                     description.append(description_string)
 
         # Fill up our task list with the found elements
         await gather_elements()
 
         if description:
@@ -390,22 +399,34 @@
             log.status(
                 "[bold bright_black]",
                 "Ignored",
                 fmt_path(element_path),
                 "[bright_black](surveys contain no relevant data)"
             )
             return None
+        elif element.type == IliasElementType.SCORM_LEARNING_MODULE:
+            log.status(
+                "[bold bright_black]",
+                "Ignored",
+                fmt_path(element_path),
+                "[bright_black](scorm learning modules are not supported)"
+            )
+            return None
+        elif element.type == IliasElementType.LEARNING_MODULE:
+            return await self._handle_learning_module(element, element_path)
         elif element.type == IliasElementType.LINK:
             return await self._handle_link(element, element_path)
         elif element.type == IliasElementType.BOOKING:
             return await self._handle_booking(element, element_path)
-        elif element.type == IliasElementType.VIDEO:
+        elif element.type == IliasElementType.OPENCAST_VIDEO:
+            return await self._handle_file(element, element_path)
+        elif element.type == IliasElementType.OPENCAST_VIDEO_PLAYER:
+            return await self._handle_opencast_video(element, element_path)
+        elif element.type == IliasElementType.MEDIACAST_VIDEO:
             return await self._handle_file(element, element_path)
-        elif element.type == IliasElementType.VIDEO_PLAYER:
-            return await self._handle_video(element, element_path)
         elif element.type in _DIRECTORY_PAGES:
             return await self._handle_ilias_page(element.url, element, element_path)
         else:
             # This will retry it a few times, failing everytime. It doesn't make any network
             # requests, so that's fine.
             raise CrawlWarning(f"Unknown element type: {element.type!r}")
 
@@ -514,15 +535,15 @@
         async with self.session.get(export_url, allow_redirects=False) as resp:
             # No redirect means we were authenticated
             if hdrs.LOCATION not in resp.headers:
                 return soupify(await resp.read()).select_one("a").get("href").strip()
 
         raise CrawlError("resolve_link_target failed even after authenticating")
 
-    async def _handle_video(
+    async def _handle_opencast_video(
         self,
         element: IliasPageElement,
         element_path: PurePath,
     ) -> Optional[Coroutine[Any, Any, None]]:
         # Copy old mapping as it is likely still relevant
         if self.prev_report:
             self.report.add_custom_value(
@@ -535,58 +556,58 @@
         # is re-used if the video consists of a single stream. In that case the
         # file name is used and *not* the stream name the ilias html parser reported
         # to ensure backwards compatibility.
         maybe_dl = await self.download(element_path, mtime=element.mtime, redownload=Redownload.ALWAYS)
 
         # If we do not want to crawl it (user filter) or we have every file
         # from the cached mapping already, we can ignore this and bail
-        if not maybe_dl or self._all_videos_locally_present(element_path):
+        if not maybe_dl or self._all_opencast_videos_locally_present(element_path):
             # Mark all existing cideos as known so they do not get deleted
             # during dleanup. We "downloaded" them, just without actually making
             # a network request as we assumed they did not change.
-            for video in self._previous_contained_videos(element_path):
+            for video in self._previous_contained_opencast_videos(element_path):
                 await self.download(video)
 
             return None
 
-        return self._download_video(element_path, element, maybe_dl)
+        return self._download_opencast_video(element_path, element, maybe_dl)
 
-    def _previous_contained_videos(self, video_path: PurePath) -> List[PurePath]:
+    def _previous_contained_opencast_videos(self, video_path: PurePath) -> List[PurePath]:
         if not self.prev_report:
             return []
         custom_value = self.prev_report.get_custom_value(str(video_path))
         if not custom_value:
             return []
         names = cast(List[str], custom_value)
         folder = video_path.parent
         return [PurePath(folder, name) for name in names]
 
-    def _all_videos_locally_present(self, video_path: PurePath) -> bool:
-        if contained_videos := self._previous_contained_videos(video_path):
+    def _all_opencast_videos_locally_present(self, video_path: PurePath) -> bool:
+        if contained_videos := self._previous_contained_opencast_videos(video_path):
             log.explain_topic(f"Checking local cache for video {video_path.name}")
             all_found_locally = True
             for video in contained_videos:
-                transformed_path = self._to_local_video_path(video)
+                transformed_path = self._to_local_opencast_video_path(video)
                 if transformed_path:
                     exists_locally = self._output_dir.resolve(transformed_path).exists()
                     all_found_locally = all_found_locally and exists_locally
             if all_found_locally:
                 log.explain("Found all videos locally, skipping enumeration request")
                 return True
             log.explain("Missing at least one video, continuing with requests!")
         return False
 
-    def _to_local_video_path(self, path: PurePath) -> Optional[PurePath]:
+    def _to_local_opencast_video_path(self, path: PurePath) -> Optional[PurePath]:
         if transformed := self._transformer.transform(path):
             return self._deduplicator.fixup_path(transformed)
         return None
 
     @anoncritical
     @_iorepeat(3, "downloading video")
-    async def _download_video(
+    async def _download_opencast_video(
         self,
         original_path: PurePath,
         element: IliasPageElement,
         dl: DownloadToken
     ) -> None:
         stream_elements: List[IliasPageElement] = []
         async with dl as (bar, sink):
@@ -595,15 +616,15 @@
 
             if len(stream_elements) > 1:
                 log.explain(f"Found multiple video streams for {element.name}")
             else:
                 log.explain(f"Using single video mode for {element.name}")
                 stream_element = stream_elements[0]
 
-                transformed_path = self._to_local_video_path(original_path)
+                transformed_path = self._to_local_opencast_video_path(original_path)
                 if not transformed_path:
                     raise CrawlError(f"Download returned a path but transform did not for {original_path}")
 
                 # We do not have a local cache yet
                 if self._output_dir.resolve(transformed_path).exists():
                     log.explain(f"Video for {element.name} existed locally")
                 else:
@@ -691,15 +712,15 @@
         async with cl:
             next_stage_url = element.url
             while next_stage_url:
                 log.explain_topic(f"Parsing HTML page for {fmt_path(cl.path)}")
                 log.explain(f"URL: {next_stage_url}")
 
                 soup = await self._get_page(next_stage_url)
-                page = IliasPage(soup, next_stage_url, None)
+                page = IliasPage(soup, next_stage_url, element)
 
                 if next := page.get_next_stage_element():
                     next_stage_url = next.url
                 else:
                     break
 
             download_data = page.get_download_forum_data()
@@ -735,36 +756,178 @@
 
         async with maybe_dl as (bar, sink):
             content = element.title_tag.prettify()
             content += element.content_tag.prettify()
             sink.file.write(content.encode("utf-8"))
             sink.done()
 
-    async def _get_page(self, url: str) -> BeautifulSoup:
+    async def _handle_learning_module(
+        self,
+        element: IliasPageElement,
+        element_path: PurePath,
+    ) -> Optional[Coroutine[Any, Any, None]]:
+        maybe_cl = await self.crawl(element_path)
+        if not maybe_cl:
+            return None
+        return self._crawl_learning_module(element, maybe_cl)
+
+    @_iorepeat(3, "crawling learning module")
+    @anoncritical
+    async def _crawl_learning_module(self, element: IliasPageElement, cl: CrawlToken) -> None:
+        elements: List[IliasLearningModulePage] = []
+
+        async with cl:
+            log.explain_topic(f"Parsing initial HTML page for {fmt_path(cl.path)}")
+            log.explain(f"URL: {element.url}")
+            soup = await self._get_page(element.url)
+            page = IliasPage(soup, element.url, element)
+            if next := page.get_learning_module_data():
+                elements.extend(await self._crawl_learning_module_direction(
+                    cl.path, next.previous_url, "left", element
+                ))
+                elements.append(next)
+                elements.extend(await self._crawl_learning_module_direction(
+                    cl.path, next.next_url, "right", element
+                ))
+
+        # Reflect their natural ordering in the file names
+        for index, lm_element in enumerate(elements):
+            lm_element.title = f"{index:02}_{lm_element.title}"
+
+        tasks: List[Awaitable[None]] = []
+        for index, elem in enumerate(elements):
+            prev_url = elements[index - 1].title if index > 0 else None
+            next_url = elements[index + 1].title if index < len(elements) - 1 else None
+            tasks.append(asyncio.create_task(
+                self._download_learning_module_page(cl.path, elem, prev_url, next_url)
+            ))
+
+        # And execute them
+        await self.gather(tasks)
+
+    async def _crawl_learning_module_direction(
+        self,
+        path: PurePath,
+        start_url: Optional[str],
+        dir: Union[Literal["left"], Literal["right"]],
+        parent_element: IliasPageElement
+    ) -> List[IliasLearningModulePage]:
+        elements: List[IliasLearningModulePage] = []
+
+        if not start_url:
+            return elements
+
+        next_element_url: Optional[str] = start_url
+        counter = 0
+        while next_element_url:
+            log.explain_topic(f"Parsing HTML page for {fmt_path(path)} ({dir}-{counter})")
+            log.explain(f"URL: {next_element_url}")
+            soup = await self._get_page(next_element_url)
+            page = IliasPage(soup, next_element_url, parent_element)
+            if next := page.get_learning_module_data():
+                elements.append(next)
+                if dir == "left":
+                    next_element_url = next.previous_url
+                else:
+                    next_element_url = next.next_url
+            counter += 1
+
+        return elements
+
+    @anoncritical
+    @_iorepeat(3, "saving learning module page")
+    async def _download_learning_module_page(
+        self,
+        parent_path: PurePath,
+        element: IliasLearningModulePage,
+        prev: Optional[str],
+        next: Optional[str]
+    ) -> None:
+        path = parent_path / (_sanitize_path_name(element.title) + ".html")
+        maybe_dl = await self.download(path)
+        if not maybe_dl:
+            return
+        my_path = self._transformer.transform(maybe_dl.path)
+        if not my_path:
+            return
+
+        if prev:
+            prev_p = self._transformer.transform(parent_path / (_sanitize_path_name(prev) + ".html"))
+            if prev_p:
+                prev = os.path.relpath(prev_p, my_path.parent)
+            else:
+                prev = None
+        if next:
+            next_p = self._transformer.transform(parent_path / (_sanitize_path_name(next) + ".html"))
+            if next_p:
+                next = os.path.relpath(next_p, my_path.parent)
+            else:
+                next = None
+
+        async with maybe_dl as (bar, sink):
+            content = element.content
+            content = await self.internalize_images(content)
+            sink.file.write(learning_module_template(content, maybe_dl.path.name, prev, next).encode("utf-8"))
+            sink.done()
+
+    async def internalize_images(self, tag: Tag) -> Tag:
+        """
+        Tries to fetch ILIAS images and embed them as base64 data.
+        """
+        log.explain_topic("Internalizing images")
+        for elem in tag.find_all(recursive=True):
+            if not isinstance(elem, Tag):
+                continue
+            if elem.name == "img":
+                if src := elem.attrs.get("src", None):
+                    url = urljoin(_ILIAS_URL, src)
+                    if not url.startswith(_ILIAS_URL):
+                        continue
+                    log.explain(f"Internalizing {url!r}")
+                    img = await self._get_authenticated(url)
+                    elem.attrs["src"] = "data:;base64," + base64.b64encode(img).decode()
+            if elem.name == "iframe" and elem.attrs.get("src", "").startswith("//"):
+                # For unknown reasons the protocol seems to be stripped.
+                elem.attrs["src"] = "https:" + elem.attrs["src"]
+        return tag
+
+    async def _get_page(self, url: str, root_page_allowed: bool = False) -> BeautifulSoup:
         auth_id = await self._current_auth_id()
         async with self.session.get(url) as request:
             soup = soupify(await request.read())
             if self._is_logged_in(soup):
-                return soup
+                return self._verify_page(soup, url, root_page_allowed)
 
         # We weren't authenticated, so try to do that
         await self.authenticate(auth_id)
 
         # Retry once after authenticating. If this fails, we will die.
         async with self.session.get(url) as request:
             soup = soupify(await request.read())
             if self._is_logged_in(soup):
-                return soup
-        raise CrawlError("get_page failed even after authenticating")
+                return self._verify_page(soup, url, root_page_allowed)
+        raise CrawlError(f"get_page failed even after authenticating on {url!r}")
+
+    def _verify_page(self, soup: BeautifulSoup, url: str, root_page_allowed: bool) -> BeautifulSoup:
+        if IliasPage.is_root_page(soup) and not root_page_allowed:
+            raise CrawlError(
+                "Unexpectedly encountered ILIAS root page. "
+                "This usually happens because the ILIAS instance is broken. "
+                "If so, wait a day or two and try again. "
+                "It could also happen because a crawled element links to the ILIAS root page. "
+                "If so, use a transform with a ! as target to ignore the particular element. "
+                f"The redirect came from {url}"
+            )
+        return soup
 
     async def _post_authenticated(
         self,
         url: str,
         data: dict[str, Union[str, List[str]]]
-    ) -> BeautifulSoup:
+    ) -> bytes:
         auth_id = await self._current_auth_id()
 
         form_data = aiohttp.FormData()
         for key, val in data.items():
             form_data.add_field(key, val)
 
         async with self.session.post(url, data=form_data(), allow_redirects=False) as request:
@@ -776,14 +939,30 @@
 
         # Retry once after authenticating. If this fails, we will die.
         async with self.session.post(url, data=data, allow_redirects=False) as request:
             if request.status == 200:
                 return await request.read()
         raise CrawlError("post_authenticated failed even after authenticating")
 
+    async def _get_authenticated(self, url: str) -> bytes:
+        auth_id = await self._current_auth_id()
+
+        async with self.session.get(url, allow_redirects=False) as request:
+            if request.status == 200:
+                return await request.read()
+
+        # We weren't authenticated, so try to do that
+        await self.authenticate(auth_id)
+
+        # Retry once after authenticating. If this fails, we will die.
+        async with self.session.get(url, allow_redirects=False) as request:
+            if request.status == 200:
+                return await request.read()
+        raise CrawlError("get_authenticated failed even after authenticating")
+
     # We repeat this as the login method in shibboleth doesn't handle I/O errors.
     # Shibboleth is quite reliable as well, the repeat is likely not critical here.
     @ _iorepeat(3, "Login", failure_is_error=True)
     async def _authenticate(self) -> None:
         await self._shibboleth_login.login(self.session)
 
     @ staticmethod
```

### Comparing `pferd-3.4.3/PFERD/crawl/kit_ipd_crawler.py` & `pferd-3.5.0/PFERD/crawl/kit_ipd_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/crawl/local_crawler.py` & `pferd-3.5.0/PFERD/crawl/local_crawler.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/deduplicator.py` & `pferd-3.5.0/PFERD/deduplicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     i = 1
     while True:
         yield path.parent / f"{path.stem}{separator}{i}{path.suffix}"
         i += 1
 
 
 class Deduplicator:
-    FORBIDDEN_CHARS = '<>:"/\\|?*'
+    FORBIDDEN_CHARS = '<>:"/\\|?*' + "".join([chr(i) for i in range(0, 32)])
     FORBIDDEN_NAMES = {
         "CON", "PRN", "AUX", "NUL",
         "COM1", "COM2", "COM3", "COM4", "COM5", "COM6", "COM7", "COM8", "COM9",
         "LPT1", "LPT2", "LPT3", "LPT4", "LPT5", "LPT6", "LPT7", "LPT8", "LPT9",
     }
 
     def __init__(self, windows_paths: bool) -> None:
```

### Comparing `pferd-3.4.3/PFERD/limiter.py` & `pferd-3.5.0/PFERD/limiter.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/logging.py` & `pferd-3.5.0/PFERD/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         self._progress_suspended = False
         self._lock = asyncio.Lock()
         self._lines: List[str] = []
 
         # Whether different parts of the output are enabled or disabled
         self.output_explain = False
         self.output_status = True
+        self.output_not_deleted = True
         self.output_report = True
 
     def _update_live(self) -> None:
         elements = []
         if self._crawl_progress.task_ids:
             elements.append(self._crawl_progress)
         if self._download_progress.task_ids:
@@ -203,22 +204,41 @@
         argument which will be applied to the "action" string.
         """
 
         if self.output_status:
             action = escape(f"{action:<{self.STATUS_WIDTH}}")
             self.print(f"{style}{action}[/] {escape(text)} {suffix}")
 
+    def not_deleted(self, style: str, action: str, text: str, suffix: str = "") -> None:
+        """
+        Print a message for a local only file that wasn't
+        deleted while crawling. Allows markup in the "style"
+        argument which will be applied to the "action" string.
+        """
+
+        if self.output_status and self.output_not_deleted:
+            action = escape(f"{action:<{self.STATUS_WIDTH}}")
+            self.print(f"{style}{action}[/] {escape(text)} {suffix}")
+
     def report(self, text: str) -> None:
         """
         Print a report after crawling. Allows markup.
         """
 
         if self.output_report:
             self.print(text)
 
+    def report_not_deleted(self, text: str) -> None:
+        """
+        Print a report for a local only file that wasn't deleted after crawling. Allows markup.
+        """
+
+        if self.output_report and self.output_not_deleted:
+            self.print(text)
+
     @contextmanager
     def _bar(
             self,
             progress: Progress,
             description: str,
             total: Optional[float],
     ) -> Iterator[ProgressBar]:
```

### Comparing `pferd-3.4.3/PFERD/output_dir.py` & `pferd-3.5.0/PFERD/output_dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,22 +40,23 @@
 
 
 class OnConflict(Enum):
     PROMPT = "prompt"
     LOCAL_FIRST = "local-first"
     REMOTE_FIRST = "remote-first"
     NO_DELETE = "no-delete"
+    NO_DELETE_PROMPT_OVERWRITE = "no-delete-prompt-overwrite"
 
     @staticmethod
     def from_string(string: str) -> "OnConflict":
         try:
             return OnConflict(string)
         except ValueError:
             raise ValueError("must be one of 'prompt', 'local-first',"
-                             " 'remote-first', 'no-delete'")
+                             " 'remote-first', 'no-delete', 'no-delete-prompt-overwrite'")
 
 
 @dataclass
 class Heuristics:
     mtime: Optional[datetime]
 
 
@@ -260,15 +261,15 @@
     # files.
 
     async def _conflict_lfrf(
             self,
             on_conflict: OnConflict,
             path: PurePath,
     ) -> bool:
-        if on_conflict == OnConflict.PROMPT:
+        if on_conflict in {OnConflict.PROMPT, OnConflict.NO_DELETE_PROMPT_OVERWRITE}:
             async with log.exclusive_output():
                 prompt = f"Replace {fmt_path(path)} with remote file?"
                 return await prompt_yes_no(prompt, default=False)
         elif on_conflict == OnConflict.LOCAL_FIRST:
             return False
         elif on_conflict == OnConflict.REMOTE_FIRST:
             return True
@@ -279,15 +280,15 @@
         raise ValueError(f"{on_conflict!r} is not a valid conflict policy")
 
     async def _conflict_ldrf(
             self,
             on_conflict: OnConflict,
             path: PurePath,
     ) -> bool:
-        if on_conflict == OnConflict.PROMPT:
+        if on_conflict in {OnConflict.PROMPT, OnConflict.NO_DELETE_PROMPT_OVERWRITE}:
             async with log.exclusive_output():
                 prompt = f"Recursively delete {fmt_path(path)} and replace with remote file?"
                 return await prompt_yes_no(prompt, default=False)
         elif on_conflict == OnConflict.LOCAL_FIRST:
             return False
         elif on_conflict == OnConflict.REMOTE_FIRST:
             return True
@@ -299,15 +300,15 @@
 
     async def _conflict_lfrd(
             self,
             on_conflict: OnConflict,
             path: PurePath,
             parent: PurePath,
     ) -> bool:
-        if on_conflict == OnConflict.PROMPT:
+        if on_conflict in {OnConflict.PROMPT, OnConflict.NO_DELETE_PROMPT_OVERWRITE}:
             async with log.exclusive_output():
                 prompt = f"Delete {fmt_path(parent)} so remote file {fmt_path(path)} can be downloaded?"
                 return await prompt_yes_no(prompt, default=False)
         elif on_conflict == OnConflict.LOCAL_FIRST:
             return False
         elif on_conflict == OnConflict.REMOTE_FIRST:
             return True
@@ -326,15 +327,15 @@
             async with log.exclusive_output():
                 prompt = f"Delete {fmt_path(path)}?"
                 return await prompt_yes_no(prompt, default=False)
         elif on_conflict == OnConflict.LOCAL_FIRST:
             return False
         elif on_conflict == OnConflict.REMOTE_FIRST:
             return True
-        elif on_conflict == OnConflict.NO_DELETE:
+        elif on_conflict in {OnConflict.NO_DELETE, OnConflict.NO_DELETE_PROMPT_OVERWRITE}:
             return False
 
         # This should never be reached
         raise ValueError(f"{on_conflict!r} is not a valid conflict policy")
 
     def _tmp_path(self, base: Path, suffix_length: int) -> Path:
         prefix = "" if base.name.startswith(".") else "."
@@ -491,15 +492,15 @@
             try:
                 path.unlink()
                 log.status("[bold bright_magenta]", "Deleted", fmt_path(pure))
                 self._report.delete_file(pure)
             except OSError:
                 pass
         else:
-            log.status("[bold bright_magenta]", "Not deleted", fmt_path(pure))
+            log.not_deleted("[bold bright_magenta]", "Not deleted", fmt_path(pure))
             self._report.not_delete_file(pure)
 
     def load_prev_report(self) -> None:
         log.explain_topic(f"Loading previous report from {fmt_real_path(self._report_path)}")
         try:
             self._prev_report = Report.load(self._report_path)
             log.explain("Loaded report successfully")
```

### Comparing `pferd-3.4.3/PFERD/pferd.py` & `pferd-3.5.0/PFERD/pferd.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                 something_changed = True
                 log.report(f"  [bold bright_yellow]Changed[/] {fmt_path(path)}")
             for path in sorted(crawler.report.deleted_files):
                 something_changed = True
                 log.report(f"  [bold bright_magenta]Deleted[/] {fmt_path(path)}")
             for path in sorted(crawler.report.not_deleted_files):
                 something_changed = True
-                log.report(f"  [bold bright_magenta]Not deleted[/] {fmt_path(path)}")
+                log.report_not_deleted(f"  [bold bright_magenta]Not deleted[/] {fmt_path(path)}")
 
             for warning in crawler.report.encountered_warnings:
                 something_changed = True
                 log.report(f"  [bold bright_red]Warning[/] {warning}")
 
             for error in crawler.report.encountered_errors:
                 something_changed = True
```

### Comparing `pferd-3.4.3/PFERD/report.py` & `pferd-3.5.0/PFERD/report.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/transformer.py` & `pferd-3.5.0/PFERD/transformer.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PFERD/utils.py` & `pferd-3.5.0/PFERD/utils.py`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/PKG-INFO` & `pferd-3.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pferd
-Version: 3.4.3
+Version: 3.5.0
 Summary: Programm zum Flotten Einfachen Runterladen von Dateien
 Author-email: Garmelon <joscha@plugh.de>
 License: Copyright 2019-2021 Garmelon, I-Al-Istannen, danstooamerican, pavelzw,
-                            TheChristophe, Scriptim, thelukasprobst, Toorero
+                            TheChristophe, Scriptim, thelukasprobst, Toorero,
+                            Mr-Pine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
         the Software, and to permit persons to whom the Software is furnished to do so,
         subject to the following conditions:
@@ -25,14 +26,19 @@
         
 Project-URL: Homepage, https://github.com/Garmelon/PFERD
 Project-URL: Bug Tracker, https://github.com/Garmelon/PFERD/issues
 Project-URL: Source, https://github.com/Garmelon/PFERD
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: beautifulsoup4>=4.10.0
+Requires-Dist: rich>=11.0.0
+Requires-Dist: keyring>=23.5.0
+Requires-Dist: certifi>=2021.10.8
 
 # PFERD
 
 **P**rogramm zum **F**lotten, **E**infachen **R**unterladen von **D**ateien
 
 Other resources:
```

### Comparing `pferd-3.4.3/README.md` & `pferd-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/pferd.egg-info/PKG-INFO` & `pferd-3.5.0/pferd.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pferd
-Version: 3.4.3
+Version: 3.5.0
 Summary: Programm zum Flotten Einfachen Runterladen von Dateien
 Author-email: Garmelon <joscha@plugh.de>
 License: Copyright 2019-2021 Garmelon, I-Al-Istannen, danstooamerican, pavelzw,
-                            TheChristophe, Scriptim, thelukasprobst, Toorero
+                            TheChristophe, Scriptim, thelukasprobst, Toorero,
+                            Mr-Pine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
         the Software, and to permit persons to whom the Software is furnished to do so,
         subject to the following conditions:
@@ -25,14 +26,19 @@
         
 Project-URL: Homepage, https://github.com/Garmelon/PFERD
 Project-URL: Bug Tracker, https://github.com/Garmelon/PFERD/issues
 Project-URL: Source, https://github.com/Garmelon/PFERD
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp>=3.8.1
+Requires-Dist: beautifulsoup4>=4.10.0
+Requires-Dist: rich>=11.0.0
+Requires-Dist: keyring>=23.5.0
+Requires-Dist: certifi>=2021.10.8
 
 # PFERD
 
 **P**rogramm zum **F**lotten, **E**infachen **R**unterladen von **D**ateien
 
 Other resources:
```

### Comparing `pferd-3.4.3/pferd.egg-info/SOURCES.txt` & `pferd-3.5.0/pferd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pferd-3.4.3/pyproject.toml` & `pferd-3.5.0/pyproject.toml`

 * *Files identical despite different names*

