# Comparing `tmp/redisvl-0.1.2.tar.gz` & `tmp/redisvl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redisvl-0.1.2.tar", last modified: Fri Mar  1 20:40:49 2024, max compression
+gzip compressed data, was "redisvl-0.1.3.tar", last modified: Tue Apr  9 16:07:21 2024, max compression
```

## Comparing `redisvl-0.1.2.tar` & `redisvl-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-01 20:40:45.000000 redisvl-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-03-01 20:40:49.714859 redisvl-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-03-01 20:40:45.000000 redisvl-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-01 20:40:45.000000 redisvl-0.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.710859 redisvl-0.1.2/redisvl/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.710859 redisvl-0.1.2/redisvl/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.710859 redisvl-0.1.2/redisvl/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.710859 redisvl-0.1.2/redisvl/extensions/llmcache/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/extensions/llmcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/extensions/llmcache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/extensions/llmcache/semantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/index/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35935 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/index/index.py
--rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/index/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/query/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/query/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/redis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/redis/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/token_escaper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/utils/vectorize/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.714859 redisvl-0.1.2/redisvl/utils/vectorize/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/text/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/text/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/text/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/utils/vectorize/text/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 20:40:45.000000 redisvl-0.1.2/redisvl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 20:40:49.710859 redisvl-0.1.2/redisvl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13221 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-01 20:40:49.000000 redisvl-0.1.2/redisvl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-01 20:40:49.714859 redisvl-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-01 20:40:45.000000 redisvl-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 16:07:17.000000 redisvl-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-09 16:07:21.640422 redisvl-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-04-09 16:07:17.000000 redisvl-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-09 16:07:17.000000 redisvl-0.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.632422 redisvl-0.1.3/redisvl/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/extensions/llmcache/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/extensions/llmcache/semantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35935 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18469 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/index/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/token_escaper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/vectorize/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.640422 redisvl-0.1.3/redisvl/utils/vectorize/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/utils/vectorize/text/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 16:07:17.000000 redisvl-0.1.3/redisvl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:07:21.636422 redisvl-0.1.3/redisvl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 16:07:21.000000 redisvl-0.1.3/redisvl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 16:07:21.640422 redisvl-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-09 16:07:17.000000 redisvl-0.1.3/setup.py
```

### Comparing `redisvl-0.1.2/LICENSE` & `redisvl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/PKG-INFO` & `redisvl-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redisvl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client library and CLI for using Redis as a vector database
 Home-page: https://github.com/RedisVentures/redisvl
 Author: Redis Inc.
 License: MIT
 Project-URL: Source, https://github.com/RedisVentures/redisvl
 Project-URL: Documentation, https://www.redisvl.com
 Keywords: ai,redis,redis-client,vector-database,vector-search
@@ -277,15 +277,15 @@
     # store user queries and LLM responses in the semantic cache
     llmcache.store(
         prompt="What is the capital city of France?",
         response="Paris",
         metadata={}
     )
 
-    # quickly check the cache with a slightly different prompt (before invoiking an LLM)
+    # quickly check the cache with a slightly different prompt (before invoking an LLM)
     response = llmcache.check(prompt="What is France's capital city?")
     print(response[0]["response"])
     ```
     ```stdout
     >>> "Paris"
     ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redisvl Version: 0.1.2 Summary: Python client
+Metadata-Version: 2.1 Name: redisvl Version: 0.1.3 Summary: Python client
 library and CLI for using Redis as a vector database Home-page: https://
 github.com/RedisVentures/redisvl Author: Redis Inc. License: MIT Project-URL:
 Source, https://github.com/RedisVentures/redisvl Project-URL: Documentation,
 https://www.redisvl.com Keywords: ai,redis,redis-client,vector-database,vector-
 search Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -138,15 +138,15 @@
 production by leveraging previously generated knowledge. ```python from
 redisvl.extensions.llmcache import SemanticCache # init cache with TTL
 (expiration) policy and semantic distance threshhold llmcache = SemanticCache
 ( name="llmcache", ttl=360, redis_url="redis://localhost:6379" )
 llmcache.set_threshold(0.2) # can be changed on-demand # store user queries and
 LLM responses in the semantic cache llmcache.store( prompt="What is the capital
 city of France?", response="Paris", metadata={} ) # quickly check the cache
-with a slightly different prompt (before invoiking an LLM) response =
+with a slightly different prompt (before invoking an LLM) response =
 llmcache.check(prompt="What is France's capital city?") print(response[0]
 ["response"]) ``` ```stdout >>> "Paris" ``` > Learn more about Semantic Caching
 [here](https://www.redisvl.com/user_guide/llmcache_03.html). - **LLM Session
 Management (COMING SOON)** aims to improve personalization and accuracy of the
 LLM application by providing user chat session information and conversational
 memory. - **LLM Contextual Access Control (COMING SOON)** aims to improve
 security concerns by preventing malicious, irrelevant, or problematic user
```

### Comparing `redisvl-0.1.2/README.md` & `redisvl-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,15 @@
     # store user queries and LLM responses in the semantic cache
     llmcache.store(
         prompt="What is the capital city of France?",
         response="Paris",
         metadata={}
     )
 
-    # quickly check the cache with a slightly different prompt (before invoiking an LLM)
+    # quickly check the cache with a slightly different prompt (before invoking an LLM)
     response = llmcache.check(prompt="What is France's capital city?")
     print(response[0]["response"])
     ```
     ```stdout
     >>> "Paris"
     ```
```

#### html2text {}

```diff
@@ -127,15 +127,15 @@
 production by leveraging previously generated knowledge. ```python from
 redisvl.extensions.llmcache import SemanticCache # init cache with TTL
 (expiration) policy and semantic distance threshhold llmcache = SemanticCache
 ( name="llmcache", ttl=360, redis_url="redis://localhost:6379" )
 llmcache.set_threshold(0.2) # can be changed on-demand # store user queries and
 LLM responses in the semantic cache llmcache.store( prompt="What is the capital
 city of France?", response="Paris", metadata={} ) # quickly check the cache
-with a slightly different prompt (before invoiking an LLM) response =
+with a slightly different prompt (before invoking an LLM) response =
 llmcache.check(prompt="What is France's capital city?") print(response[0]
 ["response"]) ``` ```stdout >>> "Paris" ``` > Learn more about Semantic Caching
 [here](https://www.redisvl.com/user_guide/llmcache_03.html). - **LLM Session
 Management (COMING SOON)** aims to improve personalization and accuracy of the
 LLM application by providing user chat session information and conversational
 memory. - **LLM Contextual Access Control (COMING SOON)** aims to improve
 security concerns by preventing malicious, irrelevant, or problematic user
```

### Comparing `redisvl-0.1.2/redisvl/cli/index.py` & `redisvl-0.1.3/redisvl/cli/index.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/cli/main.py` & `redisvl-0.1.3/redisvl/cli/main.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/cli/stats.py` & `redisvl-0.1.3/redisvl/cli/stats.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/cli/utils.py` & `redisvl-0.1.3/redisvl/cli/utils.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/cli/version.py` & `redisvl-0.1.3/redisvl/cli/version.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/extensions/llmcache/base.py` & `redisvl-0.1.3/redisvl/extensions/llmcache/base.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/extensions/llmcache/semantic.py` & `redisvl-0.1.3/redisvl/extensions/llmcache/semantic.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 
     def __init__(
         self,
         name: str = "llmcache",
         prefix: Optional[str] = None,
         distance_threshold: float = 0.1,
         ttl: Optional[int] = None,
-        vectorizer: BaseVectorizer = HFTextVectorizer(
-            model="sentence-transformers/all-mpnet-base-v2"
-        ),
+        vectorizer: Optional[BaseVectorizer] = None,
         redis_client: Optional[Redis] = None,
         redis_url: str = "redis://localhost:6379",
         connection_args: Dict[str, Any] = {},
         **kwargs,
     ):
         """Semantic Cache for Large Language Models.
 
@@ -62,14 +60,20 @@
         """
         super().__init__(ttl)
 
         # Use the index name as the key prefix by default
         if prefix is None:
             prefix = name
 
+        # Set vectorizer default
+        if vectorizer is None:
+            vectorizer = HFTextVectorizer(
+                model="sentence-transformers/all-mpnet-base-v2"
+            )
+
         # build cache index schema
         schema = IndexSchema.from_dict({"index": {"name": name, "prefix": prefix}})
         # add fields
         schema.add_fields(
             [
                 {"name": self.prompt_field_name, "type": "text"},
                 {"name": self.response_field_name, "type": "text"},
```

### Comparing `redisvl-0.1.2/redisvl/index/index.py` & `redisvl-0.1.3/redisvl/index/index.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/index/storage.py` & `redisvl-0.1.3/redisvl/index/storage.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/query/filter.py` & `redisvl-0.1.3/redisvl/query/filter.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/query/query.py` & `redisvl-0.1.3/redisvl/query/query.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/redis/connection.py` & `redisvl-0.1.3/redisvl/redis/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import os
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Type
 
-from redis import ConnectionPool, Redis
+from redis import Redis
 from redis.asyncio import Redis as AsyncRedis
+from redis.asyncio import SSLConnection as ASSLConnection
+from redis.connection import (
+    AbstractConnection,
+    Connection,
+    ConnectionPool,
+    SSLConnection,
+)
 
 from redisvl.redis.constants import REDIS_REQUIRED_MODULES
 from redisvl.redis.utils import convert_bytes
 
 
 def get_address_from_env() -> str:
     """Get a redis connection from environment variables.
@@ -126,16 +133,26 @@
 
         Args:
             client (AsyncRedis): Asynchronous Redis client.
 
         Raises:
             ValueError: If required Redis modules are not installed.
         """
+        # pick the right connection class
+        connection_class: Type[AbstractConnection] = (
+            SSLConnection
+            if client.connection_pool.connection_class == ASSLConnection
+            else Connection
+        )
+        # set up a temp sync client
         temp_client = Redis(
-            connection_pool=ConnectionPool(**client.connection_pool.connection_kwargs)
+            connection_pool=ConnectionPool(
+                connection_class=connection_class,
+                **client.connection_pool.connection_kwargs,
+            )
         )
         RedisConnectionFactory.validate_redis_modules(
             temp_client, redis_required_modules
         )
 
     @staticmethod
     def _validate_redis_modules(
```

### Comparing `redisvl-0.1.2/redisvl/redis/utils.py` & `redisvl-0.1.3/redisvl/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/schema/fields.py` & `redisvl-0.1.3/redisvl/schema/fields.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/schema/schema.py` & `redisvl-0.1.3/redisvl/schema/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,36 @@
 from redisvl.schema.fields import BaseField, FieldFactory
 from redisvl.utils.log import get_logger
 
 logger = get_logger(__name__)
 SCHEMA_VERSION = "0.1.0"
 
 
+def custom_dict(model: BaseModel) -> Dict[str, Any]:
+    """
+    Custom serialization function that converts a Pydantic model to a dict,
+    serializing Enum fields to their values, and handling nested models and lists.
+    """
+
+    def serialize_item(item):
+        if isinstance(item, Enum):
+            return item.value.lower()
+        elif isinstance(item, dict):
+            return {key: serialize_item(value) for key, value in item.items()}
+        elif isinstance(item, list):
+            return [serialize_item(element) for element in item]
+        else:
+            return item
+
+    serialized_data = model.dict(exclude_none=True)
+    for key, value in serialized_data.items():
+        serialized_data[key] = serialize_item(value)
+    return serialized_data
+
+
 class StorageType(Enum):
     """
     Enumeration for the storage types supported in Redis.
 
     Attributes:
         HASH (str): Represents the 'hash' storage type in Redis.
         JSON (str): Represents the 'json' storage type in Redis.
@@ -59,22 +81,14 @@
     prefix: str = "rvl"
     """The prefix used for Redis keys associated with this index."""
     key_separator: str = ":"
     """The separator character used in designing Redis keys."""
     storage_type: StorageType = StorageType.HASH
     """The storage type used in Redis (e.g., 'hash' or 'json')."""
 
-    def dict(self, *args, **kwargs) -> Dict[str, Any]:
-        return {
-            "name": self.name,
-            "prefix": self.prefix,
-            "key_separator": self.key_separator,
-            "storage_type": self.storage_type.value,
-        }
-
 
 class IndexSchema(BaseModel):
     """A schema definition for a search index in Redis, used in RedisVL for
     configuring index settings and organizing vector and metadata fields.
 
     The class offers methods to create an index schema from a YAML file or a
     Python dictionary, supporting flexible schema definitions and easy
@@ -424,20 +438,21 @@
                 else:
                     logger.warn(
                         message=f"Error inferring field type for {field_name}: {e}"
                     )
         return fields
 
     def to_dict(self) -> Dict[str, Any]:
-        """Convert the index schema to a dictionary.
+        """Serialize the index schema model to a dictionary, handling Enums
+        and other special cases properly.
 
         Returns:
             Dict[str, Any]: The index schema as a dictionary.
         """
-        dict_schema = self.dict(exclude_none=True)
+        dict_schema = custom_dict(self)
         # cast fields back to a pure list
         dict_schema["fields"] = [
             field for field_name, field in dict_schema["fields"].items()
         ]
         return dict_schema
 
     def to_yaml(self, file_path: str, overwrite: bool = True) -> None:
```

### Comparing `redisvl-0.1.2/redisvl/utils/log.py` & `redisvl-0.1.3/redisvl/utils/log.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/token_escaper.py` & `redisvl-0.1.3/redisvl/utils/token_escaper.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/vectorize/base.py` & `redisvl-0.1.3/redisvl/utils/vectorize/base.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/vectorize/text/cohere.py` & `redisvl-0.1.3/redisvl/utils/vectorize/text/cohere.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/vectorize/text/huggingface.py` & `redisvl-0.1.3/redisvl/utils/vectorize/text/huggingface.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/vectorize/text/openai.py` & `redisvl-0.1.3/redisvl/utils/vectorize/text/openai.py`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/redisvl/utils/vectorize/text/vertexai.py` & `redisvl-0.1.3/redisvl/utils/vectorize/text/vertexai.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 
     This vectorizer is tailored for use in
     environments where integration with Google Cloud Platform (GCP) services is
     a key requirement.
 
     Utilizing this vectorizer requires an active GCP project and location
     (region), along with appropriate application credentials. These can be
-    provided through the `api_config` dictionary or by setting the corresponding
-    environment variables. Additionally, the vertexai python client must be
+    provided through the `api_config` dictionary or set the GOOGLE_APPLICATION_CREDENTIALS
+    env var. Additionally, the vertexai python client must be
     installed with `pip install google-cloud-aiplatform>=1.26`.
 
     .. code-block:: python
 
         # Synchronous embedding of a single text
         vectorizer = VertexAITextVectorizer(
             model="textembedding-gecko",
             api_config={
                 "project_id": "your_gcp_project_id", # OR set GCP_PROJECT_ID
                 "location": "your_gcp_location",     # OR set GCP_LOCATION
-                "google_application_credentials": "path_to_your_creds"
-                # OR set GOOGLE_APPLICATION_CREDENTIALS
             })
         embedding = vectorizer.embed("Hello, world!")
 
         # Asynchronous batch embedding of multiple texts
         embeddings = await vectorizer.embed_many(
             ["Hello, world!", "Goodbye, world!"],
             batch_size=2
@@ -47,15 +45,15 @@
     ):
         """Initialize the VertexAI vectorizer.
 
         Args:
             model (str): Model to use for embedding. Defaults to
                 'textembedding-gecko'.
             api_config (Optional[Dict], optional): Dictionary containing the
-                API key. Defaults to None.
+                API config details. Defaults to None.
 
         Raises:
             ImportError: If the google-cloud-aiplatform library is not installed.
             ValueError: If the API key is not provided.
         """
         # Fetch the project_id and location from api_config or environment variables
         project_id = (
@@ -75,33 +73,24 @@
         if not location:
             raise ValueError(
                 "Missing location. "
                 "Provide the location (region) in the api_config with key 'location' "
                 "or set the GCP_LOCATION environment variable."
             )
 
-        # Check for Google Application Credentials
-        if "GOOGLE_APPLICATION_CREDENTIALS" not in os.environ:
-            creds_path = (
-                api_config.get("google_application_credentials") if api_config else None
-            )
-            if creds_path:
-                os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = creds_path
-            else:
-                raise ValueError(
-                    "Missing Google Application Credentials. "
-                    "Provide the path to the credentials JSON file in the api_config with\
-                        key 'google_application_credentials' or set the \
-                            GOOGLE_APPLICATION_CREDENTIALS environment variable."
-                )
+        # Check for credentials
+        credentials = api_config.get("credentials") if api_config else None
+
         try:
             import vertexai
-            from vertexai.preview.language_models import TextEmbeddingModel
+            from vertexai.language_models import TextEmbeddingModel
 
-            vertexai.init(project=project_id, location=location)
+            vertexai.init(
+                project=project_id, location=location, credentials=credentials
+            )
         except ImportError:
             raise ImportError(
                 "VertexAI vectorizer requires the google-cloud-aiplatform library. "
                 "Please install with `pip install google-cloud-aiplatform>=1.26`"
             )
 
         client = TextEmbeddingModel.from_pretrained(model)
```

### Comparing `redisvl-0.1.2/redisvl.egg-info/PKG-INFO` & `redisvl-0.1.3/redisvl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redisvl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client library and CLI for using Redis as a vector database
 Home-page: https://github.com/RedisVentures/redisvl
 Author: Redis Inc.
 License: MIT
 Project-URL: Source, https://github.com/RedisVentures/redisvl
 Project-URL: Documentation, https://www.redisvl.com
 Keywords: ai,redis,redis-client,vector-database,vector-search
@@ -277,15 +277,15 @@
     # store user queries and LLM responses in the semantic cache
     llmcache.store(
         prompt="What is the capital city of France?",
         response="Paris",
         metadata={}
     )
 
-    # quickly check the cache with a slightly different prompt (before invoiking an LLM)
+    # quickly check the cache with a slightly different prompt (before invoking an LLM)
     response = llmcache.check(prompt="What is France's capital city?")
     print(response[0]["response"])
     ```
     ```stdout
     >>> "Paris"
     ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redisvl Version: 0.1.2 Summary: Python client
+Metadata-Version: 2.1 Name: redisvl Version: 0.1.3 Summary: Python client
 library and CLI for using Redis as a vector database Home-page: https://
 github.com/RedisVentures/redisvl Author: Redis Inc. License: MIT Project-URL:
 Source, https://github.com/RedisVentures/redisvl Project-URL: Documentation,
 https://www.redisvl.com Keywords: ai,redis,redis-client,vector-database,vector-
 search Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
@@ -138,15 +138,15 @@
 production by leveraging previously generated knowledge. ```python from
 redisvl.extensions.llmcache import SemanticCache # init cache with TTL
 (expiration) policy and semantic distance threshhold llmcache = SemanticCache
 ( name="llmcache", ttl=360, redis_url="redis://localhost:6379" )
 llmcache.set_threshold(0.2) # can be changed on-demand # store user queries and
 LLM responses in the semantic cache llmcache.store( prompt="What is the capital
 city of France?", response="Paris", metadata={} ) # quickly check the cache
-with a slightly different prompt (before invoiking an LLM) response =
+with a slightly different prompt (before invoking an LLM) response =
 llmcache.check(prompt="What is France's capital city?") print(response[0]
 ["response"]) ``` ```stdout >>> "Paris" ``` > Learn more about Semantic Caching
 [here](https://www.redisvl.com/user_guide/llmcache_03.html). - **LLM Session
 Management (COMING SOON)** aims to improve personalization and accuracy of the
 LLM application by providing user chat session information and conversational
 memory. - **LLM Contextual Access Control (COMING SOON)** aims to improve
 security concerns by preventing malicious, irrelevant, or problematic user
```

### Comparing `redisvl-0.1.2/redisvl.egg-info/SOURCES.txt` & `redisvl-0.1.3/redisvl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/setup.cfg` & `redisvl-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `redisvl-0.1.2/setup.py` & `redisvl-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "all": read_all_requirements(),
     "dev": read_dev_requirements()
 }
 
 
 setup(
     name="redisvl",
-    version="0.1.2",
+    version="0.1.3",
     python_requires=">=3.7",
     install_requires=read_requirements(),
     extras_require=extras_require,
     packages=find_packages(),
     package_data={
         "redisvl": [
             "requirements.txt", "requirements-dev.txt", "requirements-all.txt"
```

