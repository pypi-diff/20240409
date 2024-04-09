# Comparing `tmp/crawlab-ai-0.0.3.tar.gz` & `tmp/crawlab-ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlab-ai-0.0.3.tar", last modified: Sun Apr  7 06:00:08 2024, max compression
+gzip compressed data, was "crawlab-ai-0.0.4.tar", last modified: Tue Apr  9 09:40:41 2024, max compression
```

## Comparing `crawlab-ai-0.0.3.tar` & `crawlab-ai-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/crawlab_ai/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/crawlab_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/crawlab_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/cli/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/cli/gen_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/scrapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/scrapy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/scrapy/list_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/spider/article_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/spider/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/spider/list_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/crawlab_ai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/crawlab_ai/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.708392 crawlab-ai-0.0.4/crawlab_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-09 09:40:41.000000 crawlab-ai-0.0.4/crawlab_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 09:40:41.000000 crawlab-ai-0.0.4/crawlab_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:40:41.000000 crawlab-ai-0.0.4/crawlab_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 09:40:41.000000 crawlab-ai-0.0.4/crawlab_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-09 09:40:41.000000 crawlab-ai-0.0.4/crawlab_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:41.712392 crawlab-ai-0.0.4/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-09 09:40:18.000000 crawlab-ai-0.0.4/test/utils/test_auth.py
```

### Comparing `crawlab-ai-0.0.3/LICENSE` & `crawlab-ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlab-ai-0.0.3/README.md` & `crawlab-ai-0.0.4/README.md`

 * *Files identical despite different names*

