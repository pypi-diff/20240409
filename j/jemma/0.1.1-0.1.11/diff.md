# Comparing `tmp/jemma-0.1.1.tar.gz` & `tmp/jemma-0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.1.tar", last modified: Tue Apr  9 05:01:07 2024, max compression
+gzip compressed data, was "jemma-0.1.11.tar", last modified: Tue Apr  9 05:16:34 2024, max compression
```

## Comparing `jemma-0.1.1.tar` & `jemma-0.1.11.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:01:07.992134 jemma-0.1.1/
--rw-r--r--   0 tolitius   (503) staff       (20)       99 2024-04-09 05:01:07.991657 jemma-0.1.1/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.1/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:01:07.990981 jemma-0.1.1/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)       99 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      194 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:01:07.000000 jemma-0.1.1/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:01:07.992255 jemma-0.1.1/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      461 2024-04-09 05:00:44.000000 jemma-0.1.1/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:16:34.233239 jemma-0.1.11/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:16:34.232672 jemma-0.1.11/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      702 2024-04-06 17:47:19.000000 jemma-0.1.11/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-09 05:16:34.232013 jemma-0.1.11/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      194 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       46 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-09 05:16:34.000000 jemma-0.1.11/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-09 05:16:34.233401 jemma-0.1.11/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-09 05:14:08.000000 jemma-0.1.11/setup.py
```

### Comparing `jemma-0.1.1/README.md` & `jemma-0.1.11/README.md`

 * *Files identical despite different names*

