# Comparing `tmp/contest-builder-0.0.1.tar.gz` & `tmp/contest-builder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contest-builder-0.0.1.tar", last modified: Tue Apr  9 13:57:51 2024, max compression
+gzip compressed data, was "contest-builder-0.0.2.tar", last modified: Tue Apr  9 14:11:38 2024, max compression
```

## Comparing `contest-builder-0.0.1.tar` & `contest-builder-0.0.2.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1077 2023-08-17 14:07:48.000000 contest-builder-0.0.1/LICENSE
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)       72 2024-04-09 11:20:34.000000 contest-builder-0.0.1/MANIFEST.in
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 13:57:51.814888 contest-builder-0.0.1/PKG-INFO
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.1/README.md
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      891 2024-04-09 11:36:02.000000 contest-builder-0.0.1/pyproject.toml
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2024-04-09 13:57:51.814888 contest-builder-0.0.1/setup.cfg
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.810888 contest-builder-0.0.1/src/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.1/src/contest_builder/README.md
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:37:21.000000 contest-builder-0.0.1/src/contest_builder/__init__.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1475 2024-04-09 13:46:30.000000 contest-builder-0.0.1/src/contest_builder/__main__.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:38:07.000000 contest-builder-0.0.1/src/contest_builder/py.typed
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.810888 contest-builder-0.0.1/src/contest_builder/src/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/actions/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      993 2024-04-09 13:46:56.000000 contest-builder-0.0.1/src/contest_builder/src/actions/problem_actions.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/executors/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1496 2024-04-09 13:47:24.000000 contest-builder-0.0.1/src/contest_builder/src/executors/cpp_executor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1337 2024-04-09 13:48:11.000000 contest-builder-0.0.1/src/contest_builder/src/executors/executor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      709 2024-04-09 13:48:09.000000 contest-builder-0.0.1/src/contest_builder/src/executors/program_excecutor.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1000 2024-04-09 13:48:07.000000 contest-builder-0.0.1/src/contest_builder/src/executors/python_executor.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/generators/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2088 2024-04-09 13:48:00.000000 contest-builder-0.0.1/src/contest_builder/src/generators/contest_generator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1549 2024-04-09 13:48:04.000000 contest-builder-0.0.1/src/contest_builder/src/generators/problem_generator.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.810888 contest-builder-0.0.1/src/contest_builder/src/helpers/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/command/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      412 2024-04-09 13:48:20.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/command/command_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/config/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      246 2024-04-08 12:40:44.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/config/config.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1544 2024-04-09 13:48:43.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/config/local_config.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      226 2024-04-08 13:18:04.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/config/templates.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/file/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1994 2024-04-09 13:49:30.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/file/file_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/folder/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      294 2023-10-22 17:06:27.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/folder/folder_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/model/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/model/finders/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:48.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/model/finders/language_finder.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:58.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/model/finders/provider_finder.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      345 2024-04-09 13:50:04.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/model/language_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      162 2024-04-08 11:53:02.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/model/model_helper.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1153 2024-04-09 13:50:12.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/model/problem_helper.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1502 2024-04-09 13:31:59.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/arg_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      363 2024-04-09 13:50:31.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/cat_helper.py
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      930 2023-09-12 13:44:59.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/single_process.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/helpers/utils/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      259 2023-09-12 12:23:28.000000 contest-builder-0.0.1/src/contest_builder/src/helpers/utils/timer.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/mediators/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1090 2024-04-09 13:50:46.000000 contest-builder-0.0.1/src/contest_builder/src/mediators/contest_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1316 2024-04-09 13:50:50.000000 contest-builder-0.0.1/src/contest_builder/src/mediators/execution_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      995 2024-04-09 13:50:55.000000 contest-builder-0.0.1/src/contest_builder/src/mediators/init_mediator.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1204 2024-04-09 13:50:59.000000 contest-builder-0.0.1/src/contest_builder/src/mediators/problem_mediator.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/models/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1945 2024-04-09 13:51:05.000000 contest-builder-0.0.1/src/contest_builder/src/models/contest.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1358 2024-04-08 14:41:19.000000 contest-builder-0.0.1/src/contest_builder/src/models/language.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1995 2024-04-09 13:51:12.000000 contest-builder-0.0.1/src/contest_builder/src/models/problem.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      639 2024-04-08 14:42:03.000000 contest-builder-0.0.1/src/contest_builder/src/models/provider.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/src/types/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)       86 2023-09-11 19:49:53.000000 contest-builder-0.0.1/src/contest_builder/src/types/languages.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      129 2023-08-30 01:48:44.000000 contest-builder-0.0.1/src/contest_builder/src/types/name_types.py
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      123 2023-10-22 17:06:27.000000 contest-builder-0.0.1/src/contest_builder/src/types/providers.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/templates/
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/templates/codeforces/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1161 2023-10-22 17:06:27.000000 contest-builder-0.0.1/src/contest_builder/templates/codeforces/template.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder/templates/leetcode/
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      856 2023-10-22 17:06:27.000000 contest-builder-0.0.1/src/contest_builder/templates/leetcode/template.py
-drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:57:51.814888 contest-builder-0.0.1/src/contest_builder.egg-info/
--rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/PKG-INFO
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2248 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       66 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/entry_points.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       33 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/requires.txt
--rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2024-04-09 13:57:51.000000 contest-builder-0.0.1/src/contest_builder.egg-info/top_level.txt
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1077 2023-08-17 14:07:48.000000 contest-builder-0.0.2/LICENSE
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      149 2024-04-09 14:10:27.000000 contest-builder-0.0.2/MANIFEST.in
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 14:11:38.925238 contest-builder-0.0.2/PKG-INFO
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.2/README.md
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      891 2024-04-09 14:11:23.000000 contest-builder-0.0.2/pyproject.toml
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       38 2024-04-09 14:11:38.925238 contest-builder-0.0.2/setup.cfg
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.921238 contest-builder-0.0.2/src/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.921238 contest-builder-0.0.2/src/contest_builder/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     3494 2024-04-09 09:15:40.000000 contest-builder-0.0.2/src/contest_builder/README.md
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 11:37:21.000000 contest-builder-0.0.2/src/contest_builder/__init__.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1475 2024-04-09 13:46:30.000000 contest-builder-0.0.2/src/contest_builder/__main__.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/configs/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       53 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/configs/main.json
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 13:38:07.000000 contest-builder-0.0.2/src/contest_builder/py.typed
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.921238 contest-builder-0.0.2/src/contest_builder/src/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/actions/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      993 2024-04-09 13:46:56.000000 contest-builder-0.0.2/src/contest_builder/src/actions/problem_actions.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/executors/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1496 2024-04-09 13:47:24.000000 contest-builder-0.0.2/src/contest_builder/src/executors/cpp_executor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1337 2024-04-09 13:48:11.000000 contest-builder-0.0.2/src/contest_builder/src/executors/executor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      709 2024-04-09 13:48:09.000000 contest-builder-0.0.2/src/contest_builder/src/executors/program_excecutor.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1000 2024-04-09 13:48:07.000000 contest-builder-0.0.2/src/contest_builder/src/executors/python_executor.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/generators/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2088 2024-04-09 13:48:00.000000 contest-builder-0.0.2/src/contest_builder/src/generators/contest_generator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1549 2024-04-09 13:48:04.000000 contest-builder-0.0.2/src/contest_builder/src/generators/problem_generator.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.921238 contest-builder-0.0.2/src/contest_builder/src/helpers/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/command/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      412 2024-04-09 13:48:20.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/command/command_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/config/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      246 2024-04-09 14:06:02.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/config/config.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1544 2024-04-09 13:48:43.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/config/local_config.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      226 2024-04-08 13:18:04.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/config/templates.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/file/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1994 2024-04-09 13:49:30.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/file/file_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/folder/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      294 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/folder/folder_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/model/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/model/finders/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:48.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/model/finders/language_finder.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1439 2024-04-09 13:49:58.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/model/finders/provider_finder.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      345 2024-04-09 13:50:04.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/model/language_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      162 2024-04-08 11:53:02.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/model/model_helper.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1153 2024-04-09 13:50:12.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/model/problem_helper.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1502 2024-04-09 13:31:59.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/arg_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      363 2024-04-09 13:50:31.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/cat_helper.py
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      930 2023-09-12 13:44:59.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/single_process.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/helpers/utils/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)      259 2023-09-12 12:23:28.000000 contest-builder-0.0.2/src/contest_builder/src/helpers/utils/timer.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/mediators/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1090 2024-04-09 13:50:46.000000 contest-builder-0.0.2/src/contest_builder/src/mediators/contest_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1316 2024-04-09 13:50:50.000000 contest-builder-0.0.2/src/contest_builder/src/mediators/execution_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      995 2024-04-09 13:50:55.000000 contest-builder-0.0.2/src/contest_builder/src/mediators/init_mediator.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1204 2024-04-09 13:50:59.000000 contest-builder-0.0.2/src/contest_builder/src/mediators/problem_mediator.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/models/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1945 2024-04-09 13:51:05.000000 contest-builder-0.0.2/src/contest_builder/src/models/contest.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1358 2024-04-08 14:41:19.000000 contest-builder-0.0.2/src/contest_builder/src/models/language.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1995 2024-04-09 13:51:12.000000 contest-builder-0.0.2/src/contest_builder/src/models/problem.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      639 2024-04-08 14:42:03.000000 contest-builder-0.0.2/src/contest_builder/src/models/provider.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/src/types/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)       86 2023-09-11 19:49:53.000000 contest-builder-0.0.2/src/contest_builder/src/types/languages.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      129 2023-08-30 01:48:44.000000 contest-builder-0.0.2/src/contest_builder/src/types/name_types.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      123 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/src/types/providers.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/templates/
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/templates/codeforces/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     1161 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/templates/codeforces/template.py
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder/templates/leetcode/
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)      856 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/templates/leetcode/template.py
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2354 2023-10-22 17:06:27.000000 contest-builder-0.0.2/src/contest_builder/templates/template.json
+drwxrwxr-x   0 shamir0xe  (1000) shamir0xe  (1000)        0 2024-04-09 14:11:38.925238 contest-builder-0.0.2/src/contest_builder.egg-info/
+-rw-r--r--   0 shamir0xe  (1000) shamir0xe  (1000)     5407 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)     2330 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)        1 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       66 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       33 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/requires.txt
+-rw-rw-r--   0 shamir0xe  (1000) shamir0xe  (1000)       16 2024-04-09 14:11:38.000000 contest-builder-0.0.2/src/contest_builder.egg-info/top_level.txt
```

### Comparing `contest-builder-0.0.1/LICENSE` & `contest-builder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/PKG-INFO` & `contest-builder-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contest-builder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Competetive Programming Management Tool
 Author-email: shamir0xe <shamir0xe@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Amirhossein Shapoori
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `contest-builder-0.0.1/README.md` & `contest-builder-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/pyproject.toml` & `contest-builder-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "contest-builder"
-version = "0.0.1"
+version = "0.0.2"
 description = "Competetive Programming Management Tool"
 readme = "README.md"
 authors = [{ name = "shamir0xe", email = "shamir0xe@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `contest-builder-0.0.1/src/contest_builder/README.md` & `contest-builder-0.0.2/src/contest_builder/README.md`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/__main__.py` & `contest-builder-0.0.2/src/contest_builder/__main__.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/actions/problem_actions.py` & `contest-builder-0.0.2/src/contest_builder/src/actions/problem_actions.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/executors/cpp_executor.py` & `contest-builder-0.0.2/src/contest_builder/src/executors/cpp_executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/executors/executor.py` & `contest-builder-0.0.2/src/contest_builder/src/executors/executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/executors/program_excecutor.py` & `contest-builder-0.0.2/src/contest_builder/src/executors/program_excecutor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/executors/python_executor.py` & `contest-builder-0.0.2/src/contest_builder/src/executors/python_executor.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/generators/contest_generator.py` & `contest-builder-0.0.2/src/contest_builder/src/generators/contest_generator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/generators/problem_generator.py` & `contest-builder-0.0.2/src/contest_builder/src/generators/problem_generator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/config/local_config.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/config/local_config.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/file/file_helper.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/file/file_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/model/finders/language_finder.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/model/finders/language_finder.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/model/finders/provider_finder.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/model/finders/provider_finder.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/model/problem_helper.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/model/problem_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/arg_helper.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/arg_helper.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/helpers/terminal/single_process.py` & `contest-builder-0.0.2/src/contest_builder/src/helpers/terminal/single_process.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/mediators/contest_mediator.py` & `contest-builder-0.0.2/src/contest_builder/src/mediators/contest_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/mediators/execution_mediator.py` & `contest-builder-0.0.2/src/contest_builder/src/mediators/execution_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/mediators/init_mediator.py` & `contest-builder-0.0.2/src/contest_builder/src/mediators/init_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/mediators/problem_mediator.py` & `contest-builder-0.0.2/src/contest_builder/src/mediators/problem_mediator.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/models/contest.py` & `contest-builder-0.0.2/src/contest_builder/src/models/contest.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/models/language.py` & `contest-builder-0.0.2/src/contest_builder/src/models/language.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/models/problem.py` & `contest-builder-0.0.2/src/contest_builder/src/models/problem.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/src/models/provider.py` & `contest-builder-0.0.2/src/contest_builder/src/models/provider.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/templates/codeforces/template.py` & `contest-builder-0.0.2/src/contest_builder/templates/codeforces/template.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder/templates/leetcode/template.py` & `contest-builder-0.0.2/src/contest_builder/templates/leetcode/template.py`

 * *Files identical despite different names*

### Comparing `contest-builder-0.0.1/src/contest_builder.egg-info/PKG-INFO` & `contest-builder-0.0.2/src/contest_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contest-builder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Competetive Programming Management Tool
 Author-email: shamir0xe <shamir0xe@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Amirhossein Shapoori
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `contest-builder-0.0.1/src/contest_builder.egg-info/SOURCES.txt` & `contest-builder-0.0.2/src/contest_builder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/contest_builder/py.typed
 src/contest_builder.egg-info/PKG-INFO
 src/contest_builder.egg-info/SOURCES.txt
 src/contest_builder.egg-info/dependency_links.txt
 src/contest_builder.egg-info/entry_points.txt
 src/contest_builder.egg-info/requires.txt
 src/contest_builder.egg-info/top_level.txt
+src/contest_builder/configs/main.json
 src/contest_builder/src/actions/problem_actions.py
 src/contest_builder/src/executors/cpp_executor.py
 src/contest_builder/src/executors/executor.py
 src/contest_builder/src/executors/program_excecutor.py
 src/contest_builder/src/executors/python_executor.py
 src/contest_builder/src/generators/contest_generator.py
 src/contest_builder/src/generators/problem_generator.py
@@ -41,9 +42,10 @@
 src/contest_builder/src/models/contest.py
 src/contest_builder/src/models/language.py
 src/contest_builder/src/models/problem.py
 src/contest_builder/src/models/provider.py
 src/contest_builder/src/types/languages.py
 src/contest_builder/src/types/name_types.py
 src/contest_builder/src/types/providers.py
+src/contest_builder/templates/template.json
 src/contest_builder/templates/codeforces/template.py
 src/contest_builder/templates/leetcode/template.py
```

