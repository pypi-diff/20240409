# Comparing `tmp/jemma-0.1.11.tar.gz` & `tmp/jemma-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.11.tar", last modified: Tue Apr  9 05:16:34 2024, max compression
+gzip compressed data, was "jemma-0.1.12.tar", last modified: Tue Apr  9 05:19:00 2024, max compression
```

## Comparing `jemma-0.1.11.tar` & `jemma-0.1.12.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:16:34.233239 jemma-0.1.11/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:16:34.232672 jemma-0.1.11/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.11/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:16:34.232013 jemma-0.1.11/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      194 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       46 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:16:34.233401 jemma-0.1.11/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 05:14:08.000000 jemma-0.1.11/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.451711 jemma-0.1.12/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:19:00.451261 jemma-0.1.12/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.12/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.446487 jemma-0.1.12/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      268 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       46 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        8 2024-04-09 05:19:00.000000 jemma-0.1.12/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:19:00.451861 jemma-0.1.12/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 05:18:52.000000 jemma-0.1.12/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:19:00.450518 jemma-0.1.12/simmons/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.12/simmons/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2252 2024-04-09 00:53:24.000000 jemma-0.1.12/simmons/huddle.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5267 2024-04-09 03:45:46.000000 jemma-0.1.12/simmons/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2730 2024-04-09 01:01:04.000000 jemma-0.1.12/simmons/tools.py
```

### Comparing `jemma-0.1.11/README.md` & `jemma-0.1.12/README.md`

 * *Files identical despite different names*

