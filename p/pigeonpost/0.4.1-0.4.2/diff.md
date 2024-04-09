# Comparing `tmp/pigeonpost-0.4.1.tar.gz` & `tmp/pigeonpost-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pigeonpost-0.4.1.tar", last modified: Mon Apr  8 11:32:08 2024, max compression
+gzip compressed data, was "pigeonpost-0.4.2.tar", last modified: Tue Apr  9 16:20:48 2024, max compression
```

## Comparing `pigeonpost-0.4.1.tar` & `pigeonpost-0.4.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/conf/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/core/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.281261 pigeonpost-0.4.1/pigeon/default/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/default/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/files/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/files/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/http/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/http/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.285261 pigeonpost-0.4.1/pigeon/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/components/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/cache_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/content_negotiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/mediafiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/components/staticfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/conversion/mime/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/middleware/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/templating/templater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeon/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/pigeon/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/pigeonpost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 11:32:08.000000 pigeonpost-0.4.1/pigeonpost.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-08 11:32:08.289261 pigeonpost-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-08 11:32:02.000000 pigeonpost-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.992715 pigeonpost-0.4.2/pigeon/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.992715 pigeonpost-0.4.2/pigeon/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/core/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/default/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/files/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/http/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:47.996714 pigeonpost-0.4.2/pigeon/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/content_negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/mediafiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/components/staticfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/conversion/mime/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/middleware/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/templating/templater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeon/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3227 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/pigeon/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:20:48.000715 pigeonpost-0.4.2/pigeonpost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 16:20:47.000000 pigeonpost-0.4.2/pigeonpost.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 16:20:48.004715 pigeonpost-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-04-09 16:20:42.000000 pigeonpost-0.4.2/setup.py
```

### Comparing `pigeonpost-0.4.1/pigeon/conf/manager.py` & `pigeonpost-0.4.2/pigeon/conf/manager.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/conf/settings.py` & `pigeonpost-0.4.2/pigeon/conf/settings.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/core/app.py` & `pigeonpost-0.4.2/pigeon/core/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,18 +34,23 @@
 
         # run pigeon after everything has been configured (all decorators executed)
         atexit.register(Pigeon.run)
 
 
     @classmethod
     def run(cls) -> None:
-        log.info('STARTING SERVER')
-        # start server
-        server.start()
-        server.serve()
+        log.info('STARTING')
+        try:
+            # start server
+            server.start()
+            server.serve()
+        except PermissionError as e:
+            if e.errno == 13: log.critical("PERMISSION DENIED (PORTS 0-1024 REQUIRE ADMINISTRATIVE PRIVILEGES)")
+        except OSError as e:
+            if e.errno == 98: log.critical("ADDRESS ALREADY IN USE")
 
     # @decorator register view
     @classmethod
     def view(cls, target: str, mimetype: str='*/*', auth=None) -> Callable:
         def wrapper(func) -> Callable:
             log.debug(f'FOUND VIEW: ')
             log.sublog(f'TARGET: {target}:\nMIMETYPE: {mimetype}\nFUNC: {func}\nAUTH: {auth}')
```

### Comparing `pigeonpost-0.4.1/pigeon/core/handler.py` & `pigeonpost-0.4.2/pigeon/core/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import socket
 import pigeon.middleware as middleware
 import pigeon.utils.logger as logger
 from pigeon.http import HTTPRequest, HTTPResponse
+import traceback
 
 log = logger.Log('HANDLER', 'cyan')
 
 
 def receive_data(client_sock: socket.socket, size: int = 4096) -> bytes:
     while True:
         try:
@@ -33,27 +34,32 @@
         # client terminated connection
         if not data:
             log.debug(f'CONNECTION TO {client_address[0]}:{client_address[1]} LOST')
             return
 
         log.debug(f'RAW PACKET:\n{data}')
 
-        # parse request into HTTPRequest
-        request = middleware.preprocess(data)
-        if isinstance(request, HTTPRequest):
-            log.info(f'REQUEST: {request.path}')
-
-        # gather appropriate response for request
-        response = middleware.process(request)
-        response = middleware.postprocess(request, response)
-
-        # send response to client
-        log.verbose(f'SENDING RESPONSE TO {client_address[0]}:{client_address[1]}')
-        client_sock.sendall(response.__bytes__('ascii'))
-        log.verbose(f'RESPONSE SENT')
+        try:
+
+            # parse request into HTTPRequest
+            request = middleware.preprocess(data)
+            if isinstance(request, HTTPRequest):
+                log.info(f'REQUEST: {request.path}')
+
+            # gather appropriate response for request
+            response = middleware.process(request)
+            response = middleware.postprocess(request, response)
+
+            # send response to client
+            log.verbose(f'SENDING RESPONSE TO {client_address[0]}:{client_address[1]}')
+            client_sock.sendall(response.__bytes__('ascii'))
+            log.verbose(f'RESPONSE SENT')
+
+        except Exception as e:
+            log.error(f'EXCEPTION OCCURED WHILE HANDLING REQUEST FROM {client_address[0]}:{client_address[1]}: \n{"".join(traceback.format_tb(e.__traceback__))}\t{e}\n')
 
         # do not keep connection open on error
         if response.is_error:
             break
 
         # client asks to terminate connection
         if not request.tags.keep_alive:
```

### Comparing `pigeonpost-0.4.1/pigeon/core/secure.py` & `pigeonpost-0.4.2/pigeon/core/secure.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/core/server.py` & `pigeonpost-0.4.2/pigeon/core/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pigeon.templating.templater as templater
 import threading
 
 log = logger.Log('SERVER', '#bb88ff')
 
 
 def start():
-    log.info('STARTING...')
+    log.info('...STARTING')
 
     # load static files into memory
     if Manager.static_files_dir:
         log.info('LOADING STATIC FILES')
         static.load()
 
     if Manager.templates_dir:
```

### Comparing `pigeonpost-0.4.1/pigeon/files/media.py` & `pigeonpost-0.4.2/pigeon/files/media.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/files/static.py` & `pigeonpost-0.4.2/pigeon/files/static.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/http/message.py` & `pigeonpost-0.4.2/pigeon/http/message.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/http/request.py` & `pigeonpost-0.4.2/pigeon/http/request.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/http/response.py` & `pigeonpost-0.4.2/pigeon/http/response.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/auth.py` & `pigeonpost-0.4.2/pigeon/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/__init__.py` & `pigeonpost-0.4.2/pigeon/middleware/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/cache_control.py` & `pigeonpost-0.4.2/pigeon/middleware/components/cache_control.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/component.py` & `pigeonpost-0.4.2/pigeon/middleware/components/component.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/connection.py` & `pigeonpost-0.4.2/pigeon/middleware/components/connection.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/content_negotiation.py` & `pigeonpost-0.4.2/pigeon/middleware/components/content_negotiation.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/cors.py` & `pigeonpost-0.4.2/pigeon/middleware/components/cors.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/host.py` & `pigeonpost-0.4.2/pigeon/middleware/components/host.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/mediafiles.py` & `pigeonpost-0.4.2/pigeon/middleware/components/mediafiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/method.py` & `pigeonpost-0.4.2/pigeon/middleware/components/method.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/components/staticfiles.py` & `pigeonpost-0.4.2/pigeon/middleware/components/staticfiles.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/conversion/converter.py` & `pigeonpost-0.4.2/pigeon/middleware/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/conversion/mime/parsers.py` & `pigeonpost-0.4.2/pigeon/middleware/conversion/mime/parsers.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/pipe.py` & `pigeonpost-0.4.2/pigeon/middleware/pipe.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/processing.py` & `pigeonpost-0.4.2/pigeon/middleware/processing.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/tags.py` & `pigeonpost-0.4.2/pigeon/middleware/tags.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/middleware/views.py` & `pigeonpost-0.4.2/pigeon/middleware/views.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/templating/templater.py` & `pigeonpost-0.4.2/pigeon/templating/templater.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/utils/common.py` & `pigeonpost-0.4.2/pigeon/utils/common.py`

 * *Files identical despite different names*

### Comparing `pigeonpost-0.4.1/pigeon/utils/logger.py` & `pigeonpost-0.4.2/pigeon/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def _print_msg(self, *args, end, subname):
         print(self._build_prefix(subname), *args, end=end)
 
     def critical(self, *args, end='\n', subname=''):
         self.message_blocked = False
         with lock:
-            print('[bold red blink]CRITICAL [/]', end='')
+            print('[bold red]CRITICAL [/]', end='')
             self._print_msg(*args, end=end, subname=subname)
 
     def error(self, *args, end='\n', subname=''):
         self.message_blocked = False
         with lock:
             print('[#ffaaaa]ERROR    [/]', end='')
             self._print_msg(*args, end=end, subname=subname)
```

### Comparing `pigeonpost-0.4.1/pigeonpost.egg-info/SOURCES.txt` & `pigeonpost-0.4.2/pigeonpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

